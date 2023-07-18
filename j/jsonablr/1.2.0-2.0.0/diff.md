# Comparing `tmp/jsonablr-1.2.0.tar.gz` & `tmp/jsonablr-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonablr-1.2.0.tar", max compression
+gzip compressed data, was "jsonablr-2.0.0.tar", max compression
```

## Comparing `jsonablr-1.2.0.tar` & `jsonablr-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-06-26 17:24:04.431422 jsonablr-1.2.0/LICENSE
--rw-r--r--   0        0        0     1870 2023-07-18 10:05:13.463125 jsonablr-1.2.0/README.md
--rw-r--r--   0        0        0      118 2023-06-27 16:27:20.064626 jsonablr-1.2.0/jsonablr/__init__.py
--rw-r--r--   0        0        0     6822 2023-07-18 10:05:13.464090 jsonablr-1.2.0/jsonablr/main.py
--rw-r--r--   0        0        0      561 2023-07-18 10:19:53.104279 jsonablr-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 jsonablr-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-26 17:24:04.431422 jsonablr-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1976 2023-07-04 20:21:45.058502 jsonablr-2.0.0/README.md
+-rw-r--r--   0        0        0      118 2023-06-27 16:27:20.064626 jsonablr-2.0.0/jsonablr/__init__.py
+-rw-r--r--   0        0        0     6364 2023-07-04 20:14:08.067419 jsonablr-2.0.0/jsonablr/main.py
+-rw-r--r--   0        0        0      560 2023-07-04 20:24:06.354425 jsonablr-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 jsonablr-2.0.0/PKG-INFO
```

### Comparing `jsonablr-1.2.0/LICENSE` & `jsonablr-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonablr-1.2.0/README.md` & `jsonablr-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # JsonAblr
 
 JsonAblr is a Python library that allows you to encode variables into a format that represents a JSON object. It provides a simple and intuitive way to convert variables into a JSON-like structure, making it easier to store and transmit data.
 
 This was heavily inspired by FastAPI's `jsonable_encoder`.
 
+- JsonAblr now requires Pydantic 2.0 or above. If you are using Pydantic 1.x, please use JsonAblr 1.1.1.
+
 ## Features
 
 - Encode variables into a JSON-like format
 - Supports various data types including strings, numbers, lists, dictionaries, dates, Pydantic models, dataclasses and more
 - Easy to use
 - Customizable for your own types
```

### Comparing `jsonablr-1.2.0/jsonablr/main.py` & `jsonablr-2.0.0/jsonablr/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Encoders
 """
 from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Set, Union
 from datetime import datetime, date, timezone
 import dataclasses
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
-from pydantic import BaseModel
-from pydantic.json import ENCODERS_BY_TYPE
+from pydantic import BaseModel, create_model
 
 
 def datetime_encoder(dateval: datetime) -> str:
     datestr = dateval.astimezone(tz=timezone.utc).isoformat(
         sep='T',
         timespec='milliseconds'
     )
@@ -40,63 +39,57 @@
     sqlalchemy_safe: bool = True
     preserve_set: bool = False
 
 
 def encode(data: Any, **options) -> dict:
     encoder = JsonAblr(
         encoders=options.pop('encoders', {}),
-        **Options.parse_obj(options).dict()
+        **Options.model_validate(options).model_dump()
     )
     return encoder(data)
 
 
 def encode_output(func=None, **options):
     encoder = JsonAblr(
         encoders=options.pop('encoders', {}),
-        **Options.parse_obj(options).dict()
+        **Options.model_validate(options).model_dump()
     )
 
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             return encoder.encode(func(*args, **kwargs))
         return wrapper
 
     return decorator if func is None else decorator(func)
 
 
-encoder_map:  Dict[Callable[[Any], Any], Tuple[Any, ...]] = {}
-for type_, encoder in ENCODERS_BY_TYPE.items():
-    encoder_map.setdefault(encoder, tuple())
-    encoder_map[encoder] += (type_,)
-
-
 class JsonAblr:
 
     def __init__(self, encoders: Optional[Dict[Any, Callable]] = None, **options) -> None:
         self.encoders = {
             **default_encoders,
             **(encoders or {})
         }
-        self._options = Options.parse_obj(options)
+        self._options = Options.model_validate(options)
         self._override_options = None
 
     @property
     def options(self) -> Options:
-        return Options.parse_obj({
-            **self._options.dict(),
-            **(self._override_options.dict() if self._override_options else {})
+        return Options.model_validate({
+            **self._options.model_dump(),
+            **(self._override_options.model_dump() if self._override_options else {})
         })
 
     def __call__(self, obj: Any, **options) -> Any:
         return self.encode(obj, **options)
 
     def encode(self, obj: Any, **options) -> Any:
         if options:
-            self._override_options = Options.parse_obj(options)
+            self._override_options = Options.model_validate(options)
         encoded = self._encode(obj)
         self._override_options = None
         return encoded
 
     def _encode(self, obj: Any) -> Any:
 
         custom_encoder = self.get_encoder(self.encoders, obj)
@@ -123,24 +116,17 @@
 
         if self.options.preserve_set and isinstance(obj, (set, frozenset)):
             return self.handle_set(obj)
 
         if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
             return self.handle_list_type(obj)
 
-        encoder = ENCODERS_BY_TYPE.get(type(obj))
-        if encoder:
-            return encoder(obj)
-
-        for encoder, types in encoder_map.items():
-            if isinstance(obj, types):
-                return encoder(obj)
-
         try:
-            data = dict(obj)
+            ObjModel = create_model('ObjModel', obj=(type(obj), ...))
+            return ObjModel(obj=obj).model_dump(mode='json')['obj']
         except Exception as e:
             errors: List[Exception] = []
             errors.append(e)
             try:
                 data = vars(obj)
             except Exception as e:
                 errors.append(e)
@@ -156,31 +142,26 @@
             return encoders[type(obj)]
         for type_, encoder in encoders.items():
             if isinstance(obj, type_):
                 return encoder
 
     def handle_pydantic_model(self, obj: BaseModel) -> dict:
 
-        obj_dict = obj.dict(**self.options.dict(include={
+        obj_dict = obj.model_dump(**self.options.model_dump(include={
             'include',
             'exclude',
             'by_alias',
             'exclude_unset',
             'exclude_none',
             'exclude_defaults'
         }))
 
-        json_encoders = getattr(obj.__config__, 'json_encoders', {})
-
-        if '__root__' in obj_dict:
-            obj_dict = obj_dict['__root__']
-
         encoder = self.__class__(
-            encoders={**json_encoders, **(self.encoders or {})},
-            **self.options.dict(include={
+            encoders=self.encoders,
+            **self.options.model_dump(include={
                 'exclude_none',
                 'exclude_defaults',
                 'sqlalchemy_safe',
                 'preserve_set'
             })
         )
         return encoder.encode(obj_dict)
@@ -197,15 +178,15 @@
         if self.options.include is not None:
             allowed_keys &= set(self.options.include)
         if self.options.exclude is not None:
             allowed_keys -= set(self.options.exclude)
 
         encoder = self.__class__(
             self.encoders,
-            **self.options.dict(
+            **self.options.model_dump(
                 include={
                     'by_alias',
                     'exclude_unset',
                     'exclude_none',
                     'exclude_defaults',
                     'sqlalchemy_safe',
                     'preserve_set'
```

### Comparing `jsonablr-1.2.0/pyproject.toml` & `jsonablr-2.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 authors = ["Bernard van Niekerk <bernard.van.niekerk@icloud.com>"]
 description = "Serialize Pydantic models and non-JSONable types into a JSONable variable."
 name = "jsonablr"
 readme = "README.md"
 repository = "https://github.com/frizzy/jsonablr.git"
-version = "1.2.0"
+version = "2.0.0"
 
 [tool.poetry.dependencies]
-pydantic = "^1.10"
-python = "^3.7"
+pydantic = "^2.0"
+python = "^3.8"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
```

### Comparing `jsonablr-1.2.0/PKG-INFO` & `jsonablr-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: jsonablr
-Version: 1.2.0
+Version: 2.0.0
 Summary: Serialize Pydantic models and non-JSONable types into a JSONable variable.
 Home-page: https://github.com/frizzy/jsonablr.git
 Author: Bernard van Niekerk
 Author-email: bernard.van.niekerk@icloud.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/frizzy/jsonablr.git
 Description-Content-Type: text/markdown
 
 # JsonAblr
 
 JsonAblr is a Python library that allows you to encode variables into a format that represents a JSON object. It provides a simple and intuitive way to convert variables into a JSON-like structure, making it easier to store and transmit data.
 
 This was heavily inspired by FastAPI's `jsonable_encoder`.
 
+- JsonAblr now requires Pydantic 2.0 or above. If you are using Pydantic 1.x, please use JsonAblr 1.1.1.
+
 ## Features
 
 - Encode variables into a JSON-like format
 - Supports various data types including strings, numbers, lists, dictionaries, dates, Pydantic models, dataclasses and more
 - Easy to use
 - Customizable for your own types
```

