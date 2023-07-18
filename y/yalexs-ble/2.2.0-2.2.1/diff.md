# Comparing `tmp/yalexs_ble-2.2.0.tar.gz` & `tmp/yalexs_ble-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs_ble-2.2.0.tar", max compression
+gzip compressed data, was "yalexs_ble-2.2.1.tar", max compression
```

## Comparing `yalexs_ble-2.2.0.tar` & `yalexs_ble-2.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/LICENSE
--rw-r--r--   0        0        0     3663 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/README.md
--rw-r--r--   0        0        0     2419 2023-07-13 04:55:24.387369 yalexs_ble-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      871 2023-07-13 04:55:24.359368 yalexs_ble-2.2.0/src/yalexs_ble/__init__.py
--rw-r--r--   0        0        0     2225 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/const.py
--rw-r--r--   0        0        0    16785 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/lock.py
--rw-r--r--   0        0        0    39986 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/push.py
--rw-r--r--   0        0        0        0 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/py.typed
--rw-r--r--   0        0        0     2324 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/secure_session.py
--rw-r--r--   0        0        0    10542 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/session.py
--rw-r--r--   0        0        0     2642 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/util.py
--rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 yalexs_ble-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-07-18 05:05:30.646046 yalexs_ble-2.2.1/LICENSE
+-rw-r--r--   0        0        0     3663 2023-07-18 05:05:30.646046 yalexs_ble-2.2.1/README.md
+-rw-r--r--   0        0        0     2419 2023-07-18 05:05:31.538074 yalexs_ble-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      871 2023-07-18 05:05:31.510074 yalexs_ble-2.2.1/src/yalexs_ble/__init__.py
+-rw-r--r--   0        0        0     2225 2023-07-18 05:05:30.650046 yalexs_ble-2.2.1/src/yalexs_ble/const.py
+-rw-r--r--   0        0        0    16785 2023-07-18 05:05:30.650046 yalexs_ble-2.2.1/src/yalexs_ble/lock.py
+-rw-r--r--   0        0        0    39986 2023-07-18 05:05:30.650046 yalexs_ble-2.2.1/src/yalexs_ble/push.py
+-rw-r--r--   0        0        0        0 2023-07-18 05:05:30.650046 yalexs_ble-2.2.1/src/yalexs_ble/py.typed
+-rw-r--r--   0        0        0     2324 2023-07-18 05:05:30.650046 yalexs_ble-2.2.1/src/yalexs_ble/secure_session.py
+-rw-r--r--   0        0        0    10937 2023-07-18 05:05:30.650046 yalexs_ble-2.2.1/src/yalexs_ble/session.py
+-rw-r--r--   0        0        0     2642 2023-07-18 05:05:30.650046 yalexs_ble-2.2.1/src/yalexs_ble/util.py
+-rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 yalexs_ble-2.2.1/PKG-INFO
```

### Comparing `yalexs_ble-2.2.0/LICENSE` & `yalexs_ble-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.0/README.md` & `yalexs_ble-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.0/pyproject.toml` & `yalexs_ble-2.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yalexs-ble"
-version = "2.2.0"
+version = "2.2.1"
 description = "Bluetooth control of Yale and August locks"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/yalexs-ble"
 documentation = "https://yalexs-ble.readthedocs.io"
 classifiers = [
```

### Comparing `yalexs_ble-2.2.0/src/yalexs_ble/__init__.py` & `yalexs_ble-2.2.1/src/yalexs_ble/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     local_name_is_unique,
     local_name_to_serial,
     serial_to_local_name,
     unique_id_from_device_adv,
     unique_id_from_local_name_address,
 )
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 
 __all__ = [
     "AuthError",
     "ConnectionInfo",
     "DisconnectedError",
     "DoorStatus",
     "Lock",
```

### Comparing `yalexs_ble-2.2.0/src/yalexs_ble/const.py` & `yalexs_ble-2.2.1/src/yalexs_ble/const.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.0/src/yalexs_ble/lock.py` & `yalexs_ble-2.2.1/src/yalexs_ble/lock.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.0/src/yalexs_ble/push.py` & `yalexs_ble-2.2.1/src/yalexs_ble/push.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.0/src/yalexs_ble/secure_session.py` & `yalexs_ble-2.2.1/src/yalexs_ble/secure_session.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.0/src/yalexs_ble/session.py` & `yalexs_ble-2.2.1/src/yalexs_ble/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import time
-from typing import Callable
+from functools import partial
+from typing import Any, Callable
 
 import async_timeout
 from bleak import BleakClient
 from bleak_retry_connector import BleakError
 from cryptography.hazmat.primitives.ciphers import (
     Cipher,
     CipherContext,
@@ -43,14 +44,19 @@
     """No advertisement data."""
 
 
 class BluetoothError(YaleXSBLEError):
     """Bluetooth error."""
 
 
+def _on_disconnected(task: asyncio.Task[Any], fut: asyncio.Future[None]) -> None:
+    if task and not task.done():
+        task.cancel()
+
+
 class Session:
     _write_characteristic = WRITE_CHARACTERISTIC
     _read_characteristic = READ_CHARACTERISTIC
 
     def __init__(
         self,
         client: BleakClient,
@@ -254,37 +260,38 @@
             )
             # If we send commands to fast the lock may crash and stop
             # advertising. This is a workaround to avoid that since
             # it means a battery pull is required to recover.
             await asyncio.sleep(COOLDOWN_TIME - cooldown_remain)
         assert self.cipher_encrypt is not None, "Cipher not set"  # nosec
         self._write_checksum(command)
-        task = asyncio.current_task()
         disconnected_future = asyncio.get_running_loop().create_future()
-        self._disconnected_futures.add(disconnected_future)
-
-        def _on_disconnected(fut: asyncio.Future[None]) -> None:
-            if task and not task.done():
-                task.cancel()
-
-        disconnected_future.add_done_callback(_on_disconnected)
+        disconnected_futures = self._disconnected_futures
+        disconnected_futures.add(disconnected_future)
+        disconnected_callback = partial(_on_disconnected, asyncio.current_task())
+        disconnected_future.add_done_callback(disconnected_callback)
         try:
             return await self._write(command, command_name)
         except BleakError as err:
             if self._first_request and util.is_key_error(err):
                 raise AuthError(
                     f"Authentication error: key or slot (key index) is incorrect: {err}"
                 ) from err
             if util.is_disconnected_error(err):
                 raise DisconnectedError(f"{self.name}: {err}") from err
             raise
         except asyncio.CancelledError:
+            if not disconnected_future.done():
+                # If we get cancelled and the disconnect callback hasn't
+                # been called yet, it came from somewhere else and we should
+                # raise to propagate it
+                raise
             _LOGGER.debug(
                 "%s: `%s` cancelled due to disconnect during write",
                 self.name,
                 command_name,
             )
             raise DisconnectedError(f"{self.name}: Disconnected")
         finally:
-            self._disconnected_futures.discard(disconnected_future)
-            disconnected_future.remove_done_callback(_on_disconnected)
+            disconnected_futures.discard(disconnected_future)
+            disconnected_future.remove_done_callback(disconnected_callback)
             self._first_request = False
```

### Comparing `yalexs_ble-2.2.0/src/yalexs_ble/util.py` & `yalexs_ble-2.2.1/src/yalexs_ble/util.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.2.0/PKG-INFO` & `yalexs_ble-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs-ble
-Version: 2.2.0
+Version: 2.2.1
 Summary: Bluetooth control of Yale and August locks
 Home-page: https://github.com/bdraco/yalexs-ble
 License: GNU General Public License v3.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yalexs-ble Version: 2.2.0 Summary: Bluetooth
+Metadata-Version: 2.1 Name: yalexs-ble Version: 2.2.1 Summary: Bluetooth
 control of Yale and August locks Home-page: https://github.com/bdraco/yalexs-
 ble License: GNU General Public License v3.0 Author: J. Nick Koston Author-
 email: nick@koston.org Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: Other/Proprietary License Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

