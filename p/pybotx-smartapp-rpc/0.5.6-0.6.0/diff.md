# Comparing `tmp/pybotx_smartapp_rpc-0.5.6.tar.gz` & `tmp/pybotx_smartapp_rpc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotx_smartapp_rpc-0.5.6.tar", max compression
+gzip compressed data, was "pybotx_smartapp_rpc-0.6.0.tar", max compression
```

## Comparing `pybotx_smartapp_rpc-0.5.6.tar` & `pybotx_smartapp_rpc-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6421 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/LICENSE
--rw-r--r--   0        0        0     6618 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/README.md
--rw-r--r--   0        0        0      849 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/__init__.py
--rw-r--r--   0        0        0      126 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/empty_args.py
--rw-r--r--   0        0        0      658 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/exception_handlers.py
--rw-r--r--   0        0        0      417 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/middlewares/__init__.py
--rw-r--r--   0        0        0      650 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/middlewares/empty_args_middleware.py
--rw-r--r--   0        0        0     1445 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/middlewares/exception_middleware.py
--rw-r--r--   0        0        0        0 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/models/__init__.py
--rw-r--r--   0        0        0      182 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/models/errors.py
--rw-r--r--   0        0        0      964 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/models/method.py
--rw-r--r--   0        0        0      284 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/models/request.py
--rw-r--r--   0        0        0     2404 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/models/responses.py
--rw-r--r--   0        0        0        0 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/py.typed
--rw-r--r--   0        0        0     3279 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/router.py
--rw-r--r--   0        0        0     2604 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/rpc.py
--rw-r--r--   0        0        0     1271 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/smartapp.py
--rw-r--r--   0        0        0      844 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/typing.py
--rw-r--r--   0        0        0      647 2023-02-21 08:54:18.249664 pybotx_smartapp_rpc-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     7571 1970-01-01 00:00:00.000000 pybotx_smartapp_rpc-0.5.6/setup.py
--rw-r--r--   0        0        0     7185 1970-01-01 00:00:00.000000 pybotx_smartapp_rpc-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     6421 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/LICENSE
+-rw-r--r--   0        0        0    12454 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/README.md
+-rw-r--r--   0        0        0      849 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/empty_args.py
+-rw-r--r--   0        0        0      658 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/exception_handlers.py
+-rw-r--r--   0        0        0      417 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/middlewares/__init__.py
+-rw-r--r--   0        0        0      650 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/middlewares/empty_args_middleware.py
+-rw-r--r--   0        0        0     1445 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/middlewares/exception_middleware.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/models/__init__.py
+-rw-r--r--   0        0        0      205 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/models/errors.py
+-rw-r--r--   0        0        0     1260 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/models/method.py
+-rw-r--r--   0        0        0      284 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/models/request.py
+-rw-r--r--   0        0        0     2395 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/models/responses.py
+-rw-r--r--   0        0        0     5518 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/openapi_utils.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/py.typed
+-rw-r--r--   0        0        0     5969 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/router.py
+-rw-r--r--   0        0        0     2682 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/rpc.py
+-rw-r--r--   0        0        0     1271 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/smartapp.py
+-rw-r--r--   0        0        0      844 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/typing.py
+-rw-r--r--   0        0        0      621 2023-07-18 08:17:31.326490 pybotx_smartapp_rpc-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    13031 1970-01-01 00:00:00.000000 pybotx_smartapp_rpc-0.6.0/PKG-INFO
```

### Comparing `pybotx_smartapp_rpc-0.5.6/LICENSE` & `pybotx_smartapp_rpc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/__init__.py` & `pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/exception_handlers.py` & `pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/middlewares/empty_args_middleware.py` & `pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/middlewares/empty_args_middleware.py`

 * *Files identical despite different names*

### Comparing `pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/middlewares/exception_middleware.py` & `pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/middlewares/exception_middleware.py`

 * *Files identical despite different names*

### Comparing `pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/models/responses.py` & `pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/models/responses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import asdict, dataclass, field
+from dataclasses import dataclass, field
 from typing import Any, Dict, Generic, List, TypeVar, Union
 
 from pybotx import File
 from pydantic import BaseModel
 from pydantic.error_wrappers import ValidationError
 
 from pybotx_smartapp_rpc.models.errors import RPCError
@@ -40,15 +40,15 @@
     files: List[File] = field(default_factory=list)
     encrypted: bool = True
 
     def jsonable_dict(self) -> Dict[str, Any]:
         return {
             "status": "error",
             "type": "smartapp_rpc",
-            "errors": [asdict(error) for error in self.errors],
+            "errors": [error.dict() for error in self.errors],
         }
 
 
 def build_invalid_rpc_request_error_response(
     exc: ValidationError,
 ) -> RPCErrorResponse:
     return RPCErrorResponse(
```

### Comparing `pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/rpc.py` & `pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/rpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,18 @@
             chat_id=event.chat.id,
             data=rpc_response.jsonable_dict(),
             ref=event.ref,
             files=rpc_response.files,
             encrypted=rpc_response.encrypted,
         )
 
+    @property
+    def router(self) -> RPCRouter:
+        return self._router
+
     def _insert_exception_middleware(
         self,
         user_exception_handlers: ExceptionHandlerDict,
     ) -> None:
         exception_handlers: ExceptionHandlerDict = {
             Exception: default_exception_handler,
             RPCErrorExc: rpc_exception_handler,
```

### Comparing `pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/smartapp.py` & `pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/smartapp.py`

 * *Files identical despite different names*

### Comparing `pybotx_smartapp_rpc-0.5.6/pybotx_smartapp_rpc/typing.py` & `pybotx_smartapp_rpc-0.6.0/pybotx_smartapp_rpc/typing.py`

 * *Files identical despite different names*

### Comparing `pybotx_smartapp_rpc-0.5.6/pyproject.toml` & `pybotx_smartapp_rpc-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "pybotx-smartapp-rpc"
-version = "0.5.6"
+version = "0.6.0"
 description = "eXpress SmartApp JSON-RPC library"
 authors = ["Arseniy Zhiltsov <arseniy.zhiltsov@ccsteam.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 
 pybotx = ">=0.53.2,<0.56.0"
 
-pydantic = "^1.8.2"
-fastapi = ">=0.70.0,<0.75.0"
+pydantic = "^1.10.8"
 
 [tool.poetry.dev-dependencies]
 add-trailing-comma = "^2.2.1"
 black = "22.3.0"
-isort = "^4.3"
+isort = "5.10.1"
 autoflake = "^1.4"
 mypy = "0.910"
 wemake-python-styleguide = "0.16.1"
 
 pytest = "^7.0.1"
 pytest-asyncio = "^0.18.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

