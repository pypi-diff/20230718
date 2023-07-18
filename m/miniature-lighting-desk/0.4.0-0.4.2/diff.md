# Comparing `tmp/miniature_lighting_desk-0.4.0.tar.gz` & `tmp/miniature_lighting_desk-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniature_lighting_desk-0.4.0.tar", max compression
+gzip compressed data, was "miniature_lighting_desk-0.4.2.tar", max compression
```

## Comparing `miniature_lighting_desk-0.4.0.tar` & `miniature_lighting_desk-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.4.0/LICENSE
--rw-r--r--   0        0        0       43 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.4.0/miniature_lighting_desk/__init__.py
--rw-r--r--   0        0        0    10963 2023-07-18 20:04:26.429778 miniature_lighting_desk-0.4.0/miniature_lighting_desk/async_hal.py
--rw-r--r--   0        0        0     3578 2023-07-18 20:54:58.919753 miniature_lighting_desk-0.4.0/miniature_lighting_desk/cli.py
--rw-r--r--   0        0        0     3000 2023-07-10 21:46:19.949131 miniature_lighting_desk-0.4.0/miniature_lighting_desk/local_gui.py
--rw-r--r--   0        0        0     4404 2023-07-10 21:52:08.892461 miniature_lighting_desk-0.4.0/miniature_lighting_desk/server.py
--rw-r--r--   0        0        0      833 2023-07-18 20:59:28.543084 miniature_lighting_desk-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 miniature_lighting_desk-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.4.2/LICENSE
+-rw-r--r--   0        0        0       43 2023-07-10 18:17:21.789236 miniature_lighting_desk-0.4.2/miniature_lighting_desk/__init__.py
+-rw-r--r--   0        0        0    10974 2023-07-18 21:08:07.596413 miniature_lighting_desk-0.4.2/miniature_lighting_desk/async_hal.py
+-rw-r--r--   0        0        0     3578 2023-07-18 20:54:58.919753 miniature_lighting_desk-0.4.2/miniature_lighting_desk/cli.py
+-rw-r--r--   0        0        0     3000 2023-07-10 21:46:19.949131 miniature_lighting_desk-0.4.2/miniature_lighting_desk/local_gui.py
+-rw-r--r--   0        0        0     4404 2023-07-10 21:52:08.892461 miniature_lighting_desk-0.4.2/miniature_lighting_desk/server.py
+-rw-r--r--   0        0        0      833 2023-07-18 21:12:17.086411 miniature_lighting_desk-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 miniature_lighting_desk-0.4.2/PKG-INFO
```

### Comparing `miniature_lighting_desk-0.4.0/LICENSE` & `miniature_lighting_desk-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.4.0/miniature_lighting_desk/async_hal.py` & `miniature_lighting_desk-0.4.2/miniature_lighting_desk/async_hal.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     @abstractmethod
     def wifi_status(self) -> dict:
         """Get controller wifi status."""
 
 
 class FreqencyMixin:
     @abstractmethod
-    def frequency(self, frequency_hz: int | None):
+    def frequency(self, frequency_hz: "int | None" = None):
         """Get or set pwm frequency."""
 
 
 class MockController(ControllerABC):
     def __init__(self, *args, no_channels=8, **kwargs):
         self.no_channels = no_channels
         self.vals = [0] * no_channels
@@ -240,15 +240,15 @@
 
     def wifi_status(self):
         return self.sync_call("wifi_status")
 
     def repl(self):
         return self.sync_call("repl")
 
-    def frequency(self, frequency_hz: int | None = None) -> int:
+    def frequency(self, frequency_hz: "int | None" = None) -> int:
         return self.sync_call("frequency", val_hz=frequency_hz)
 
 
 class Channel:
     """Class to represent a particular channel on the controller."""
 
     def __init__(
```

### Comparing `miniature_lighting_desk-0.4.0/miniature_lighting_desk/cli.py` & `miniature_lighting_desk-0.4.2/miniature_lighting_desk/cli.py`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.4.0/miniature_lighting_desk/local_gui.py` & `miniature_lighting_desk-0.4.2/miniature_lighting_desk/local_gui.py`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.4.0/miniature_lighting_desk/server.py` & `miniature_lighting_desk-0.4.2/miniature_lighting_desk/server.py`

 * *Files identical despite different names*

### Comparing `miniature_lighting_desk-0.4.0/pyproject.toml` & `miniature_lighting_desk-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miniature-lighting-desk"
-version = "0.4.0"
+version = "0.4.2"
 description = "Desk software for Miniature Lighting Controller"
 authors = ["John Maximilian <2e0byo@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyusb = "^1.2.1"
```

### Comparing `miniature_lighting_desk-0.4.0/PKG-INFO` & `miniature_lighting_desk-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniature-lighting-desk
-Version: 0.4.0
+Version: 0.4.2
 Summary: Desk software for Miniature Lighting Controller
 License: MIT
 Author: John Maximilian
 Author-email: 2e0byo@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

