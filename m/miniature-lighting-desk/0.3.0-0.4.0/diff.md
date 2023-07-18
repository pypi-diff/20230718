# Comparing `tmp/miniature_lighting_desk-0.3.0.tar.gz` & `tmp/miniature_lighting_desk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniature_lighting_desk-0.3.0.tar", max compression
+gzip compressed data, was "miniature_lighting_desk-0.4.0.tar", max compression
```

## Comparing `miniature_lighting_desk-0.3.0.tar` & `miniature_lighting_desk-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.3.0/LICENSE
--rw-r--r--   0        0        0       43 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.3.0/miniature_lighting_desk/__init__.py
--rw-r--r--   0        0        0    10677 2023-07-11 22:48:36.988372 miniature_lighting_desk-0.3.0/miniature_lighting_desk/async_hal.py
--rw-r--r--   0        0        0     2506 2023-07-11 22:51:31.421704 miniature_lighting_desk-0.3.0/miniature_lighting_desk/cli.py
--rw-r--r--   0        0        0     3000 2023-07-10 21:46:19.949131 miniature_lighting_desk-0.3.0/miniature_lighting_desk/local_gui.py
--rw-r--r--   0        0        0     4404 2023-07-10 21:52:08.892461 miniature_lighting_desk-0.3.0/miniature_lighting_desk/server.py
--rw-r--r--   0        0        0      815 2023-07-11 23:11:04.385027 miniature_lighting_desk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 miniature_lighting_desk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.4.0/LICENSE
+-rw-r--r--   0        0        0       43 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.4.0/miniature_lighting_desk/__init__.py
+-rw-r--r--   0        0        0    10963 2023-07-18 20:04:26.429778 miniature_lighting_desk-0.4.0/miniature_lighting_desk/async_hal.py
+-rw-r--r--   0        0        0     3578 2023-07-18 20:54:58.919753 miniature_lighting_desk-0.4.0/miniature_lighting_desk/cli.py
+-rw-r--r--   0        0        0     3000 2023-07-10 21:46:19.949131 miniature_lighting_desk-0.4.0/miniature_lighting_desk/local_gui.py
+-rw-r--r--   0        0        0     4404 2023-07-10 21:52:08.892461 miniature_lighting_desk-0.4.0/miniature_lighting_desk/server.py
+-rw-r--r--   0        0        0      833 2023-07-18 20:59:28.543084 miniature_lighting_desk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 miniature_lighting_desk-0.4.0/PKG-INFO
```

### Comparing `miniature_lighting_desk-0.3.0/LICENSE` & `miniature_lighting_desk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.3.0/miniature_lighting_desk/async_hal.py` & `miniature_lighting_desk-0.4.0/miniature_lighting_desk/async_hal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from abc import ABC, abstractmethod
 from functools import partial
 from re import search
 from threading import Thread
-from time import sleep
+from time import monotonic, sleep
 
 import usb
 from aioserial import AioSerial
 from jsonrpcclient import parse, parse_json, request_json
 
 
 class ControllerError(Exception):
@@ -106,14 +106,20 @@
         """Connect controller to wifi network."""
 
     @abstractmethod
     def wifi_status(self) -> dict:
         """Get controller wifi status."""
 
 
+class FreqencyMixin:
+    @abstractmethod
+    def frequency(self, frequency_hz: int | None):
+        """Get or set pwm frequency."""
+
+
 class MockController(ControllerABC):
     def __init__(self, *args, no_channels=8, **kwargs):
         self.no_channels = no_channels
         self.vals = [0] * no_channels
         self.max_brightness = 100
         super().__init__(*args, **kwargs)
 
@@ -192,15 +198,15 @@
     def scale_brightness(self, unscaled: int) -> int:
         return self.max_brightness - unscaled
 
     def unscale_brightness(self, scaled: int) -> int:
         return self.max_brightness - scaled
 
 
-class SerialRpcController(WifiControllerABC):
+class SerialRpcController(WifiControllerABC, FreqencyMixin):
     def __init__(self, *args, port="/dev/ttyUSB0", **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.serial = AioSerial(port=port, baudrate=460800)
         self.lock = asyncio.Lock()
         self.no_channels = self.sync_call("channel_count")
         self.max_brightness = self.sync_call("max_brightness")
 
@@ -219,43 +225,45 @@
 
     async def _async_get_brightness(self, channel: int) -> int:
         return await self.call("get_brightness", channel=channel)
 
     async def _async_set_brightness(
         self, channel: int, brightness: int, pause: float = 0
     ) -> None:
-        return await self.call("set_brightness", channel=channel, brightness=brightness)
+        start = monotonic()
+        await self.call("set_brightness", channel=channel, brightness=brightness)
+        await asyncio.sleep(max(0, pause - (monotonic() - start)))
 
     scale_brightness = unscale_brightness = lambda s, x: x
 
     def wifi(self, ssid: str, password: str):
         return self.sync_call("wifi_connect", ssid=ssid, key=password)
 
     def wifi_status(self):
         return self.sync_call("wifi_status")
 
     def repl(self):
         return self.sync_call("repl")
 
+    def frequency(self, frequency_hz: int | None = None) -> int:
+        return self.sync_call("frequency", val_hz=frequency_hz)
+
 
 class Channel:
     """Class to represent a particular channel on the controller."""
 
     def __init__(
         self,
         controller: ControllerABC,
         channel_number,
-        on_brightness=256,
-        off_brightness=0,
     ):
         self.controller = controller
         self.channel_number = channel_number
         self._query()  # get brightness
-        self.on_brightness = on_brightness
-        self.off_brightness = off_brightness
+        self.on_brightness = controller.max_brightness
 
     def _query(self):
         """Get current value from controller."""
         self.value = self.controller.get_brightness(self.channel_number)
 
     def _set_value(self):
         """Write value for channel to controller."""
@@ -269,21 +277,21 @@
     def get_brightness(self):
         """Get brightness for channel as an integer between 0 and 255."""
         return self.value
 
     def set_percent_brightness(self, brightness):
         """Set brightness for channel as a percentage, represented by a float between 0
         and 1."""
-        self.value = round(brightness * 256)
+        self.value = round(brightness * self.on_brightness)
         self._set_value()
 
     def get_percent_brightness(self):
         """Get brightness for channel as a percentage, represented by a float between 0
         and 1."""
-        return self.value / 255
+        return self.value / self.on_brightness
 
     def fade_on(self, fade_time=1):
         """
         Fade on in fade_time seconds.
 
         Note that the channel thinks this is atomic, i.e. it has no idea
         of the actual brightness during the fade (although cancelling
@@ -300,17 +308,17 @@
         Fade off in fade_time seconds.
 
         Note that the channel thinks this is atomic, i.e. it has no idea
         of the actual brightness during the fade (although cancelling
         will query the controller for it.)
         """
         self.fade_future = self.controller.fade_brightness(
-            self.channel_number, self.value, self.off_brightness, fade_time
+            self.channel_number, self.value, 0, fade_time
         )
-        self.value = self.off_brightness
+        self.value = 0
 
     def cancel_fade(self):
         """Cancel ongoing fade and then query controller for actual channel value."""
         self.fade_future.cancel()
         self._query()
```

### Comparing `miniature_lighting_desk-0.3.0/miniature_lighting_desk/local_gui.py` & `miniature_lighting_desk-0.4.0/miniature_lighting_desk/local_gui.py`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.3.0/miniature_lighting_desk/server.py` & `miniature_lighting_desk-0.4.0/miniature_lighting_desk/server.py`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.3.0/pyproject.toml` & `miniature_lighting_desk-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miniature-lighting-desk"
-version = "0.3.0"
+version = "0.4.0"
 description = "Desk software for Miniature Lighting Controller"
 authors = ["John Maximilian <2e0byo@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyusb = "^1.2.1"
@@ -12,14 +12,15 @@
 autobahn = {extras = ["serialization"], version = "^23.6.2"}
 click = "^8.0.3"
 mkdocstrings = "^0.17.0"
 typer = "^0.9.0"
 rich = "^13.4.2"
 jsonrpcclient = "^4.0.3"
 aioserial = "^1.3.1"
+pyserial = "^3.5"
 
 [tool.poetry.scripts]
 lighting_desk = "miniature_lighting_desk.cli:app"
 
 [tool.poetry.dev-dependencies]
 devtools = "^0.8.0"
 mkdocs = "^1.2.3"
```

### Comparing `miniature_lighting_desk-0.3.0/PKG-INFO` & `miniature_lighting_desk-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniature-lighting-desk
-Version: 0.3.0
+Version: 0.4.0
 Summary: Desk software for Miniature Lighting Controller
 License: MIT
 Author: John Maximilian
 Author-email: 2e0byo@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,10 +13,11 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aioserial (>=1.3.1,<2.0.0)
 Requires-Dist: autobahn[serialization] (>=23.6.2,<24.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: jsonrpcclient (>=4.0.3,<5.0.0)
 Requires-Dist: mkdocstrings (>=0.17.0,<0.18.0)
+Requires-Dist: pyserial (>=3.5,<4.0)
 Requires-Dist: pyusb (>=1.2.1,<2.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

