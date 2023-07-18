# Comparing `tmp/coderfastapi-1.9.0.tar.gz` & `tmp/coderfastapi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coderfastapi-1.9.0.tar", last modified: Tue May 30 12:31:10 2023, max compression
+gzip compressed data, was "coderfastapi-2.0.0.tar", last modified: Tue Jul 18 13:15:41 2023, max compression
```

## Comparing `coderfastapi-1.9.0.tar` & `coderfastapi-2.0.0.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.711315 coderfastapi-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 12:31:10.711315 coderfastapi-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.703315 coderfastapi-1.9.0/coderfastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.703315 coderfastapi-1.9.0/coderfastapi/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/handlers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.703315 coderfastapi-1.9.0/coderfastapi/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.707315 coderfastapi-1.9.0/coderfastapi/lib/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.711315 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/query.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:10.703315 coderfastapi-1.9.0/coderfastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 12:31:10.000000 coderfastapi-1.9.0/coderfastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-30 12:30:40.000000 coderfastapi-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:31:10.711315 coderfastapi-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.778530 coderfastapi-2.0.0/coderfastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.778530 coderfastapi-2.0.0/coderfastapi/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/handlers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.778530 coderfastapi-2.0.0/coderfastapi/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/decorators/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/coderfastapi/lib/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.778530 coderfastapi-2.0.0/coderfastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/setup.cfg
```

### Comparing `coderfastapi-1.9.0/coderfastapi/lib/decorators.py` & `coderfastapi-2.0.0/coderfastapi/lib/decorators/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from functools import wraps
 from http import HTTPStatus
 from typing import Awaitable, Callable, Optional, TypeVar
 
 from fastapi import HTTPException
 
+from coderfastapi.lib.decorators.pagination import paginate  # noqa
+
 T = TypeVar("T")
 
 
 def http_require(
     entity_name: str,
 ) -> Callable[[Callable[..., Awaitable[Optional[T]]]], Callable[..., Awaitable[T]]]:
     def decorate(
```

### Comparing `coderfastapi-1.9.0/coderfastapi/lib/router.py` & `coderfastapi-2.0.0/coderfastapi/lib/router.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py` & `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py` & `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py` & `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/__init__.py` & `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.9.0/coderfastapi/lib/security/policies/authorization/user.py` & `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.9.0/coderfastapi/lib/signature.py` & `coderfastapi-2.0.0/coderfastapi/lib/signature.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-1.9.0/coderfastapi/lib/validation/schemas/pagination.py` & `coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/pagination.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from base64 import urlsafe_b64decode, urlsafe_b64encode
 from typing import Any, Callable, Iterator, Self
 
-import orjson
 from codercore.db.pagination import Cursor
 from codercore.lib.collection import Direction
 from pydantic import BaseModel
 
 
 class CursorSchema(BaseModel, Cursor):
     last_id: Any
@@ -37,12 +36,12 @@
         return {
             "last_id": self.last_id,
             "last_value": self.last_value,
             "direction": self.direction,
         }
 
     def encode(self) -> bytes:
-        return urlsafe_b64encode(orjson.dumps(self._dict()))
+        return urlsafe_b64encode(self.json().encode())
 
     @staticmethod
     def decode(v: bytes) -> Self:
-        return CursorSchema(**orjson.loads(urlsafe_b64decode(v)))
+        return CursorSchema.parse_raw(urlsafe_b64decode(v))
```

### Comparing `coderfastapi-1.9.0/coderfastapi.egg-info/SOURCES.txt` & `coderfastapi-2.0.0/coderfastapi.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 README.md
 pyproject.toml
 coderfastapi/__init__.py
+coderfastapi/test.py
 coderfastapi.egg-info/PKG-INFO
 coderfastapi.egg-info/SOURCES.txt
 coderfastapi.egg-info/dependency_links.txt
 coderfastapi.egg-info/requires.txt
 coderfastapi.egg-info/top_level.txt
 coderfastapi/handlers/__init__.py
 coderfastapi/handlers/version.py
 coderfastapi/lib/__init__.py
-coderfastapi/lib/decorators.py
 coderfastapi/lib/router.py
 coderfastapi/lib/signature.py
+coderfastapi/lib/decorators/__init__.py
+coderfastapi/lib/decorators/pagination.py
 coderfastapi/lib/security/__init__.py
 coderfastapi/lib/security/acl.py
 coderfastapi/lib/security/policies/__init__.py
 coderfastapi/lib/security/policies/authentication/__init__.py
 coderfastapi/lib/security/policies/authentication/jwt/__init__.py
 coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
 coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
```

### Comparing `coderfastapi-1.9.0/pyproject.toml` & `coderfastapi-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coderfastapi"
-version = "1.9.0"
+version = "2.0.0"
 description = "coderfastapi"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
-    'codercore ~= 2.2',
+    'codercore ~= 3.0',
     'fastapi[all] ~= 0.89',
     'orjson ~= 3.8',
     'pydantic ~= 1.10',
     'python-jose ~= 3.3',
 ]
 
 [project.optional-dependencies]
@@ -28,15 +28,15 @@
     'black ~= 22.12',
     'bumpver ~= 2022.1120',
     'flake8 ~= 6.0',
     'isort ~= 5.12',
 ]
 
 [tool.bumpver]
-current_version = "1.9.0"
+current_version = "2.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

