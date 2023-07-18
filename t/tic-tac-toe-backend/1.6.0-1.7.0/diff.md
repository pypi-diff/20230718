# Comparing `tmp/tic-tac-toe-backend-1.6.0.tar.gz` & `tmp/tic-tac-toe-backend-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tic-tac-toe-backend-1.6.0.tar", last modified: Fri Jul 14 01:56:00 2023, max compression
+gzip compressed data, was "tic-tac-toe-backend-1.7.0.tar", last modified: Tue Jul 18 02:03:36 2023, max compression
```

## Comparing `tic-tac-toe-backend-1.6.0.tar` & `tic-tac-toe-backend-1.7.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:56:00.534744 tic-tac-toe-backend-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-14 01:56:00.534744 tic-tac-toe-backend-1.6.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1532 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:56:00.534744 tic-tac-toe-backend-1.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1182 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:56:00.530743 tic-tac-toe-backend-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:56:00.530743 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-14 01:56:00.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-14 01:56:00.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:56:00.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-14 01:56:00.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 01:56:00.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:56:00.530743 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:56:00.530743 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:56:00.530743 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      474 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/operations/get_.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/operations/get_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/operations/put_games.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:56:00.530743 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2969 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/shared/move.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/shared/moveparameter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/shared/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5163 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:56:00.534744 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-14 01:55:48.000000 tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:36.667218 tic-tac-toe-backend-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-18 02:03:36.667218 tic-tac-toe-backend-1.7.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1532 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 02:03:36.667218 tic-tac-toe-backend-1.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1182 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:36.663217 tic-tac-toe-backend-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:36.663217 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-18 02:03:36.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-18 02:03:36.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:03:36.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 02:03:36.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 02:03:36.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:36.667218 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:36.667218 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:36.667218 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/errors/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/errors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:36.667218 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      215 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      474 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/operations/get_.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      481 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/operations/get_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/operations/put_games.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:36.667218 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      671 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2969 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/shared/move.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/shared/moveparameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/shared/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5630 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:03:36.667218 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-18 02:03:22.000000 tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/utils/utils.py
```

### Comparing `tic-tac-toe-backend-1.6.0/LICENSE.md` & `tic-tac-toe-backend-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.6.0/PKG-INFO` & `tic-tac-toe-backend-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tic-tac-toe-backend
-Version: 1.6.0
+Version: 1.7.0
 Summary: Tic Tac Toe Backend Python Client SDK
 Home-page: UNKNOWN
 Author: Shain Lafazan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `tic-tac-toe-backend-1.6.0/README.md` & `tic-tac-toe-backend-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.6.0/setup.py` & `tic-tac-toe-backend-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="tic-tac-toe-backend",
-    version="1.6.0",
+    version="1.7.0",
     author="Shain Lafazan",
     description="Tic Tac Toe Backend Python Client SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backend.egg-info/PKG-INFO` & `tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tic-tac-toe-backend
-Version: 1.6.0
+Version: 1.7.0
 Summary: Tic Tac Toe Backend Python Client SDK
 Home-page: UNKNOWN
 Author: Shain Lafazan
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backend.egg-info/SOURCES.txt` & `tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backend.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 src/tic_tac_toe_backend.egg-info/dependency_links.txt
 src/tic_tac_toe_backend.egg-info/requires.txt
 src/tic_tac_toe_backend.egg-info/top_level.txt
 src/tic_tac_toe_backends/__init__.py
 src/tic_tac_toe_backends/sdk.py
 src/tic_tac_toe_backends/sdkconfiguration.py
 src/tic_tac_toe_backends/models/__init__.py
+src/tic_tac_toe_backends/models/errors/__init__.py
+src/tic_tac_toe_backends/models/errors/sdkerror.py
 src/tic_tac_toe_backends/models/operations/__init__.py
 src/tic_tac_toe_backends/models/operations/get_.py
 src/tic_tac_toe_backends/models/operations/get_version.py
 src/tic_tac_toe_backends/models/operations/put_games.py
 src/tic_tac_toe_backends/models/shared/__init__.py
 src/tic_tac_toe_backends/models/shared/move.py
 src/tic_tac_toe_backends/models/shared/moveparameter.py
```

### Comparing `tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/shared/__init__.py` & `tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/models/shared/move.py` & `tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/models/shared/move.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/sdk.py` & `tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/sdk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from tic_tac_toe_backends import utils
-from tic_tac_toe_backends.models import operations
+from tic_tac_toe_backends.models import errors, operations
 
 class TicTacToeBackends:
     r"""Game Engine API for Tic Tac Toe: Game Engine API for Tic Tac Toe"""
 
     sdk_configuration: SDKConfiguration
 
     def __init__(self,
@@ -59,14 +59,16 @@
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def get_version(self) -> operations.GetVersionResponse:
         r"""Root endpoint.
         <br/>Returns the package name and version.<br/><br/>
@@ -84,14 +86,16 @@
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetVersionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def put_games(self, request: bytes) -> operations.PutGamesResponse:
         r"""Games endpoint. Creates the next game state from the previous game state.
         <br/>Accepts a GameState and Move.<br/><br/>Returns a Move including the before and after GameStates.<br/>
@@ -114,11 +118,13 @@
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PutGamesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, '*/*'):
                 res.body = http_res.content
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/sdkconfiguration.py` & `tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/sdkconfiguration.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '1.6.0'
-    gen_version: str = '2.65.0'
+    sdk_version: str = '1.7.0'
+    gen_version: str = '2.70.0'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/utils/retries.py` & `tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/utils/retries.py`

 * *Files identical despite different names*

### Comparing `tic-tac-toe-backend-1.6.0/src/tic_tac_toe_backends/utils/utils.py` & `tic-tac-toe-backend-1.7.0/src/tic_tac_toe_backends/utils/utils.py`

 * *Files identical despite different names*

