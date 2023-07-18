# Comparing `tmp/robocorp_storage-0.3.0.tar.gz` & `tmp/robocorp_storage-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_storage-0.3.0.tar", max compression
+gzip compressed data, was "robocorp_storage-0.3.1.tar", max compression
```

## Comparing `robocorp_storage-0.3.0.tar` & `robocorp_storage-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      385 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/README.md
--rw-r--r--   0        0        0      801 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7283 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/__init__.py
--rw-r--r--   0        0        0     6044 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_client.py
--rw-r--r--   0        0        0     2354 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_environment.py
--rw-r--r--   0        0        0     6343 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_requests.py
--rw-r--r--   0        0        0     1904 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_types.py
--rw-r--r--   0        0        0      170 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/_utils.py
--rw-r--r--   0        0        0        0 2023-07-12 14:17:29.782968 robocorp_storage-0.3.0/src/robocorp/storage/py.typed
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 robocorp_storage-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      385 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/README.md
+-rw-r--r--   0        0        0      801 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7286 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/__init__.py
+-rw-r--r--   0        0        0     6044 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_client.py
+-rw-r--r--   0        0        0     2354 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_environment.py
+-rw-r--r--   0        0        0     6343 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_requests.py
+-rw-r--r--   0        0        0     1904 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_types.py
+-rw-r--r--   0        0        0      170 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/py.typed
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 robocorp_storage-0.3.1/PKG-INFO
```

### Comparing `robocorp_storage-0.3.0/pyproject.toml` & `robocorp_storage-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-storage"
-version = "0.3.0"
+version = "0.3.1"
 description = "Robocorp Asset Storage library"
 authors = [
 	"Cosmin P. <cosmin@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
```

### Comparing `robocorp_storage-0.3.0/src/robocorp/storage/__init__.py` & `robocorp_storage-0.3.1/src/robocorp/storage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ._client import AssetNotFound, AssetUploadFailed
 
 if TYPE_CHECKING:
     from ._client import AssetsClient
     from ._requests import Response
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 JSON = Union[dict[str, "JSON"], list["JSON"], str, int, float, bool, None]
 
 LOGGER = logging.getLogger(__name__)
 
 # Known (additional) mimetypes from file extensions
@@ -173,15 +173,15 @@
     try:
         details = client.get_asset(asset_id=f"name:{name}")
         LOGGER.debug("Updating existing asset with id: %s", details["id"])
     except AssetNotFound:
         details = client.create_asset(name=name)
         LOGGER.debug("Created new asset with id: %s", details["id"])
 
-    LOGGER.info("Uploading asset (content-type: %s)", name, content_type)
+    LOGGER.info("Uploading asset %r (content-type: %s)", name, content_type)
     client.upload_asset(details["id"], content, content_type, wait)
 
 
 def set_text(name: str, text: str, wait: bool = True):
     """Create or update an asset to contain the given string.
 
     Arguments:
```

### Comparing `robocorp_storage-0.3.0/src/robocorp/storage/_client.py` & `robocorp_storage-0.3.1/src/robocorp/storage/_client.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-0.3.0/src/robocorp/storage/_environment.py` & `robocorp_storage-0.3.1/src/robocorp/storage/_environment.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-0.3.0/src/robocorp/storage/_requests.py` & `robocorp_storage-0.3.1/src/robocorp/storage/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-0.3.0/src/robocorp/storage/_types.py` & `robocorp_storage-0.3.1/src/robocorp/storage/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-0.3.0/PKG-INFO` & `robocorp_storage-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-storage
-Version: 0.3.0
+Version: 0.3.1
 Summary: Robocorp Asset Storage library
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Cosmin P.
 Author-email: cosmin@robocorp.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

