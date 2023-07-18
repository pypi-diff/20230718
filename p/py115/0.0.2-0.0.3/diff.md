# Comparing `tmp/py115-0.0.2.tar.gz` & `tmp/py115-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py115-0.0.2.tar", last modified: Sun Jul  9 10:34:09 2023, max compression
+gzip compressed data, was "py115-0.0.3.tar", last modified: Tue Jul 18 13:26:46 2023, max compression
```

## Comparing `py115-0.0.2.tar` & `py115-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-09 10:33:59.000000 py115-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-09 10:34:09.537325 py115-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-09 10:33:59.000000 py115-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.533325 py115-0.0.2/py115/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-09 10:33:59.000000 py115-0.0.2/py115/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/py115/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/py115/_internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/m115.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/qrcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/py115/_internal/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/_xor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/ec115.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/crypto/m115.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/oss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.537325 py115-0.0.2/py115/_internal/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/protocol/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/protocol/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-09 10:33:59.000000 py115-0.0.2/py115/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-09 10:33:59.000000 py115-0.0.2/py115/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-09 10:33:59.000000 py115-0.0.2/py115/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-07-09 10:33:59.000000 py115-0.0.2/py115/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-09 10:33:59.000000 py115-0.0.2/py115/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 10:34:09.533325 py115-0.0.2/py115.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 10:34:09.000000 py115-0.0.2/py115.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-09 10:33:59.000000 py115-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 10:33:59.000000 py115-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 10:34:09.537325 py115-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-09 10:33:59.000000 py115-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:26:46.083304 py115-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-18 13:26:14.000000 py115-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-18 13:26:46.083304 py115-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-18 13:26:14.000000 py115-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:26:46.079304 py115-0.0.3/py115/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-18 13:26:14.000000 py115-0.0.3/py115/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:26:46.083304 py115-0.0.3/py115/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:26:46.083304 py115-0.0.3/py115/_internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/m115.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/qrcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:26:46.083304 py115-0.0.3/py115/_internal/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/crypto/_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/crypto/_xor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/crypto/ec115.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/crypto/m115.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/oss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:26:46.083304 py115-0.0.3/py115/_internal/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/protocol/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/protocol/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-18 13:26:14.000000 py115-0.0.3/py115/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-18 13:26:14.000000 py115-0.0.3/py115/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-18 13:26:14.000000 py115-0.0.3/py115/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-07-18 13:26:14.000000 py115-0.0.3/py115/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-07-18 13:26:14.000000 py115-0.0.3/py115/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:26:46.079304 py115-0.0.3/py115.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-18 13:26:46.000000 py115-0.0.3/py115.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-18 13:26:46.000000 py115-0.0.3/py115.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:26:46.000000 py115-0.0.3/py115.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 13:26:46.000000 py115-0.0.3/py115.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 13:26:46.000000 py115-0.0.3/py115.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 13:26:14.000000 py115-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 13:26:14.000000 py115-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:26:46.083304 py115-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 13:26:14.000000 py115-0.0.3/setup.py
```

### Comparing `py115-0.0.2/LICENSE` & `py115-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/PKG-INFO` & `py115-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py115
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SDK for 115 cloud storage service.
 Author-email: deadblue <public@dead.blue>
 License: MIT License
         
         Copyright 2023 deadblue
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of 
@@ -25,16 +25,18 @@
         CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/deadblue/py115
 Project-URL: Documentation, https://py115.readthedocs.io/en/latest/
 Keywords: 115,cloud-storage,sdk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =====
 PY115
```

### Comparing `py115-0.0.2/README.rst` & `py115-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/__init__.py` & `py115-0.0.3/py115/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 storage = cloud.storage()
 
 for file in storage.list():
     print(f'File: {file.name}')
 
 """
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 import py115.cloud
 import py115.types
 
 def connect(
         credential: py115.types.Credential = None,
         protocol_kwargs: dict=  None
```

### Comparing `py115-0.0.2/py115/_internal/api/dir.py` & `py115-0.0.3/py115/_internal/api/dir.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/api/file.py` & `py115-0.0.3/py115/_internal/api/file.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/api/m115.py` & `py115-0.0.3/py115/_internal/api/m115.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/api/offline.py` & `py115-0.0.3/py115/_internal/api/offline.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/api/qrcode.py` & `py115-0.0.3/py115/_internal/api/qrcode.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,42 +2,35 @@
 
 import time as timelib
 import typing
 
 from py115._internal.protocol import api
 
 
-_client_id_mapping = {
+_app_id_mapping = {
     'web': 0,
     'mac': 7,
     'linux': 7,
     'windows': 7,
 }
 
-_image_url_template = 'https://qrcodeapi.115.com/api/1.0/%(platform)s/1.0/qrcode?qrfrom=1&client=%(client_id)d&uid=%(uid)s'
-
-
-Platform = typing.Literal[
-    'web', 'mac', 'linux', 'windows'
-]
-
 
 class _BaseApi(api.ApiSpec):
 
     def parse_result(self, result: dict) -> typing.Any:
         if result.get('state', 0) != 1:
             raise api.ApiException(code=result.get('code'))
         return result.get('data')
 
 
 class TokenApi(_BaseApi):
 
-    def __init__(self, platform: Platform = 'web') -> None:
+    def __init__(self, app_name: str) -> None:
         super().__init__(
-            f'https://qrcodeapi.115.com/api/1.0/{platform}/1.0/token', True
+            f'https://qrcodeapi.115.com/api/1.0/{app_name}/1.0/token', True
         )
 
 
 class StatusApi(_BaseApi):
 
     def __init__(self, uid: str, time: int, sign: str) -> None:
         super().__init__('https://qrcodeapi.115.com/get/status/', False)
@@ -56,24 +49,20 @@
             raise api.ApiException(code)
         result_data = result.get('data', {})
         return result_data.get('status', 0)
 
 
 class LoginApi(_BaseApi):
 
-    def __init__(self, platform: Platform, uid: str) -> None:
+    def __init__(self, app_name: str, uid: str) -> None:
         super().__init__(
-            f'https://passportapi.115.com/app/1.0/{platform}/1.0/login/qrcode', True
+            f'https://passportapi.115.com/app/1.0/{app_name}/1.0/login/qrcode', True
         )
         self.update_from({
             'account': uid,
-            'app': platform
+            'app': app_name
         })
 
 
-def get_image_url(platform: Platform, uid: str) -> str:
-    params = {
-        'platform': platform,
-        'client_id': _client_id_mapping.get(platform),
-        'uid': uid
-    }
-    return _image_url_template % params
+def get_image_url(app_name: str, uid: str) -> str:
+    app_id = _app_id_mapping.get(app_name, 0)
+    return f'https://qrcodeapi.115.com/api/1.0/{app_name}/1.0/qrcode?qrfrom=1&client={app_id}d&uid={uid}'
```

### Comparing `py115-0.0.2/py115/_internal/api/upload.py` & `py115-0.0.3/py115/_internal/api/upload.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/crypto/_rsa.py` & `py115-0.0.3/py115/_internal/crypto/_rsa.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/crypto/_xor.py` & `py115-0.0.3/py115/_internal/crypto/_xor.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/crypto/ec115.py` & `py115-0.0.3/py115/_internal/crypto/ec115.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/crypto/m115.py` & `py115-0.0.3/py115/_internal/crypto/m115.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/protocol/api.py` & `py115-0.0.3/py115/_internal/protocol/api.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/protocol/client.py` & `py115-0.0.3/py115/_internal/protocol/client.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/_internal/utils.py` & `py115-0.0.3/py115/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/cloud.py` & `py115-0.0.3/py115/cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 import typing
 
 from py115._internal.protocol.client import Client
 from py115._internal.api import qrcode, upload, version
 
 from py115 import login, services
-from py115.types import Credential, LoginPlatform
+from py115.types import AppType, Credential
+
+
+_app_names = [
+    'web', 'mac', 'linux', 'windows'
+]
 
 
 class Cloud(login._Handler):
     """115 cloud service.
 
     Args:
         credential (py115.types.Credential): Credential object.
@@ -57,28 +62,29 @@
             py115.types.Credential: Credential object, or None when credential is invalid.
         """
         # TODO: Check credential before return.
         return Credential.from_dict(
             self._client.export_cookies()
         )
 
-    def qrcode_login(self, platform: LoginPlatform) -> login.QrcodeSession:
+    def qrcode_login(self, app_type: AppType) -> login.QrcodeSession:
         """Start QRcode login session.
 
         Args:
-            platform (py115.types.LoginPlatform): Platform to login.
+            app_type (py115.types.AppType): App to login.
 
         Returns:
             py115.login.QrcodeSession: QRcode login session.
         """
-        token = self._client.execute_api(qrcode.TokenApi(platform.value))
+        app_name = _app_names[app_type.value]
+        token = self._client.execute_api(qrcode.TokenApi(app_name))
         return login.QrcodeSession._create(
             client=self._client,
             handler=self,
-            platform=platform.value,
+            app_name=app_name,
             uid=token.get('uid'), 
             time=token.get('time'),
             sign=token.get('sign')
         )
 
     def _on_login(self) -> bool:
         try:
```

### Comparing `py115-0.0.2/py115/login.py` & `py115-0.0.3/py115/login.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 
 
 class QrcodeSession:
     """QRcode login session."""
 
     _client: Client
     _handler: _Handler
-    _platform: str
+    _app_name: str
     _uid: str
     _time: int
     _sign: str
 
     image_data: bytes
     """QRcode image data"""
 
     @classmethod
-    def _create(cls, client: Client, handler: _Handler, platform: str, uid: str, time: int, sign: str):
+    def _create(cls, client: Client, handler: _Handler, app_name: str, uid: str, time: int, sign: str):
         s = cls()
         s._client = client
         s._handler = handler
-        s._platform = platform
+        s._app_name = app_name
         s._uid = uid
         s._time = time
         s._sign = sign
-        s.image_data = client.fetch(qrcode.get_image_url(platform, uid))
+        s.image_data = client.fetch(qrcode.get_image_url(app_name, uid))
         return s
 
     def poll(self) -> bool:
         """Poll QRcode status.
         This method will block until login is done, or QRcode is invalid.
 
         Returns:
@@ -53,15 +53,15 @@
                 uid=self._uid,
                 time=self._time,
                 sign=self._sign
             ))
             if status == 2:
                 # Allowed, start login
                 self._client.execute_api(qrcode.LoginApi(
-                    platform=self._platform,
+                    app_name=self._app_name,
                     uid=self._uid
                 ))
                 return self._handler._on_login()
                 
             elif status < 0:
                 # Canceled or Expired
                 return False
```

### Comparing `py115-0.0.2/py115/services.py` & `py115-0.0.3/py115/services.py`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/py115/types.py` & `py115-0.0.3/py115/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 __author__ = 'deadblue'
 
 from datetime import datetime
-from enum import IntEnum, StrEnum
+from enum import IntEnum
 
 from py115._internal import oss, utils
 
 
-class LoginPlatform(StrEnum):
+class AppType(IntEnum):
+    """App to login."""
 
-    Web = "web"
-    """Web."""
-
-    Mac = "mac"
-    """MAC App."""
-
-    Linux = "linux"
-    """Linux App."""
-
-    Windows = "windows"
-    """Windows App."""
+    Web = 0
+    """Login as web"""
+    Mac = 1
+    """Login as MAC app"""
+    Linux = 2
+    """Login as Linux app"""
+    Windows = 3
+    """Login as Windows app"""
 
 
 class _Base:
     """Base clase for all types."""
 
     def __repr__(self) -> str:
         cls_name = type(self).__name__
```

### Comparing `py115-0.0.2/py115.egg-info/PKG-INFO` & `py115-0.0.3/py115.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py115
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SDK for 115 cloud storage service.
 Author-email: deadblue <public@dead.blue>
 License: MIT License
         
         Copyright 2023 deadblue
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of 
@@ -25,16 +25,18 @@
         CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/deadblue/py115
 Project-URL: Documentation, https://py115.readthedocs.io/en/latest/
 Keywords: 115,cloud-storage,sdk
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =====
 PY115
```

### Comparing `py115-0.0.2/py115.egg-info/SOURCES.txt` & `py115-0.0.3/py115.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py115-0.0.2/pyproject.toml` & `py115-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 keywords = [
     "115", "cloud-storage", "sdk"
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">=3.9"
 dynamic = ["dependencies", "version"]
 
 [project.urls]
 Homepage = "https://github.com/deadblue/py115"
```

