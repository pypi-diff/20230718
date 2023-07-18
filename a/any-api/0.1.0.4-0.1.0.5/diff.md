# Comparing `tmp/any_api-0.1.0.4.tar.gz` & `tmp/any_api-0.1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "any_api-0.1.0.4.tar", max compression
+gzip compressed data, was "any_api-0.1.0.5.tar", max compression
```

## Comparing `any_api-0.1.0.4.tar` & `any_api-0.1.0.5.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0    11357 2022-08-24 12:23:30.000000 any_api-0.1.0.4/LICENSE
--rw-r--r--   0        0        0       25 2023-05-16 10:09:38.209717 any_api-0.1.0.4/any_api/__init__.py
--rw-r--r--   0        0        0        0 2022-10-28 09:49:12.000000 any_api-0.1.0.4/any_api/asyncapi/__init__.py
--rw-r--r--   0        0        0     3851 2022-11-09 10:01:05.000000 any_api-0.1.0.4/any_api/asyncapi/asyncapi.py
--rw-r--r--   0        0        0        0 2022-10-28 09:49:12.000000 any_api-0.1.0.4/any_api/asyncapi/model/__init__.py
--rw-r--r--   0        0        0     5145 2022-11-09 10:01:05.000000 any_api-0.1.0.4/any_api/asyncapi/model/asyncapi_model.py
--rw-r--r--   0        0        0     4502 2022-11-09 09:55:15.000000 any_api-0.1.0.4/any_api/asyncapi/model/operation_model.py
--rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.4/any_api/base_api/__init__.py
--rw-r--r--   0        0        0     6158 2023-05-16 10:00:16.655653 any_api-0.1.0.4/any_api/base_api/base_api.py
--rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.4/any_api/base_api/model/__init__.py
--rw-r--r--   0        0        0      788 2022-11-06 17:22:33.000000 any_api-0.1.0.4/any_api/base_api/model/base_api_model.py
--rw-r--r--   0        0        0      657 2023-04-06 03:37:55.268257 any_api-0.1.0.4/any_api/openapi/__init__.py
--rw-r--r--   0        0        0     5399 2023-04-12 14:27:02.953045 any_api-0.1.0.4/any_api/openapi/model/__init__.py
--rw-r--r--   0        0        0     3980 2023-04-04 03:36:57.298823 any_api-0.1.0.4/any_api/openapi/model/links.py
--rw-r--r--   0        0        0    20056 2023-01-06 03:43:04.000000 any_api-0.1.0.4/any_api/openapi/model/openapi/__init__.py
--rw-r--r--   0        0        0     2884 2022-11-09 10:04:21.000000 any_api-0.1.0.4/any_api/openapi/model/openapi/basic.py
--rw-r--r--   0        0        0     1820 2022-11-09 10:04:21.000000 any_api-0.1.0.4/any_api/openapi/model/openapi/info.py
--rw-r--r--   0        0        0     6532 2023-05-16 10:08:36.253191 any_api-0.1.0.4/any_api/openapi/model/openapi/security.py
--rw-r--r--   0        0        0     1475 2023-04-04 03:56:13.829648 any_api-0.1.0.4/any_api/openapi/model/requests.py
--rw-r--r--   0        0        0     3515 2023-04-12 14:27:02.965022 any_api-0.1.0.4/any_api/openapi/model/responses.py
--rw-r--r--   0        0        0      388 2023-01-10 16:04:06.000000 any_api-0.1.0.4/any_api/openapi/model/util.py
--rw-r--r--   0        0        0    18433 2023-04-12 14:27:02.973007 any_api-0.1.0.4/any_api/openapi/openapi.py
--rw-r--r--   0        0        0        0 2022-10-28 10:06:44.000000 any_api-0.1.0.4/any_api/openapi/to/__init__.py
--rw-r--r--   0        0        0    11232 2023-01-04 16:22:51.000000 any_api-0.1.0.4/any_api/openapi/to/markdown.py
--rw-r--r--   0        0        0      285 2023-01-09 03:46:58.000000 any_api-0.1.0.4/any_api/openapi/web_ui/__init__.py
--rw-r--r--   0        0        0     1042 2022-10-25 03:45:48.000000 any_api-0.1.0.4/any_api/openapi/web_ui/elements.py
--rw-r--r--   0        0        0     1196 2022-10-25 03:54:12.000000 any_api-0.1.0.4/any_api/openapi/web_ui/rapidoc.py
--rw-r--r--   0        0        0     1021 2022-06-18 16:09:46.000000 any_api-0.1.0.4/any_api/openapi/web_ui/redoc.py
--rw-r--r--   0        0        0     1285 2022-06-18 16:09:46.000000 any_api-0.1.0.4/any_api/openapi/web_ui/swagger.py
--rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.4/any_api/util/__init__.py
--rw-r--r--   0        0        0     8233 2023-04-12 14:48:45.169102 any_api-0.1.0.4/any_api/util/by_pydantic.py
--rw-r--r--   0        0        0     4297 2022-11-02 11:53:55.000000 any_api-0.1.0.4/any_api/util/i18n.py
--rw-r--r--   0        0        0      193 2022-10-28 09:09:27.000000 any_api-0.1.0.4/any_api/util/util.py
--rw-r--r--   0        0        0     1634 2023-05-16 10:09:38.209717 any_api-0.1.0.4/pyproject.toml
--rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 any_api-0.1.0.4/setup.py
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 any_api-0.1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-08-24 12:23:30.000000 any_api-0.1.0.5/LICENSE
+-rw-r--r--   0        0        0       25 2023-07-18 15:38:08.714076 any_api-0.1.0.5/any_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:49:12.000000 any_api-0.1.0.5/any_api/asyncapi/__init__.py
+-rw-r--r--   0        0        0     3851 2022-11-09 10:01:05.000000 any_api-0.1.0.5/any_api/asyncapi/asyncapi.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:49:12.000000 any_api-0.1.0.5/any_api/asyncapi/model/__init__.py
+-rw-r--r--   0        0        0     5145 2022-11-09 10:01:05.000000 any_api-0.1.0.5/any_api/asyncapi/model/asyncapi_model.py
+-rw-r--r--   0        0        0     4502 2022-11-09 09:55:15.000000 any_api-0.1.0.5/any_api/asyncapi/model/operation_model.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.5/any_api/base_api/__init__.py
+-rw-r--r--   0        0        0     8083 2023-07-18 15:36:22.476205 any_api-0.1.0.5/any_api/base_api/base_api.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.5/any_api/base_api/model/__init__.py
+-rw-r--r--   0        0        0      788 2022-11-06 17:22:33.000000 any_api-0.1.0.5/any_api/base_api/model/base_api_model.py
+-rw-r--r--   0        0        0      657 2023-07-14 09:37:31.964475 any_api-0.1.0.5/any_api/openapi/__init__.py
+-rw-r--r--   0        0        0     5759 2023-07-18 15:36:22.476205 any_api-0.1.0.5/any_api/openapi/model/__init__.py
+-rw-r--r--   0        0        0     4208 2023-07-18 15:36:22.476205 any_api-0.1.0.5/any_api/openapi/model/links.py
+-rw-r--r--   0        0        0    20254 2023-07-18 15:36:22.480206 any_api-0.1.0.5/any_api/openapi/model/openapi/__init__.py
+-rw-r--r--   0        0        0     2884 2022-11-09 10:04:21.000000 any_api-0.1.0.5/any_api/openapi/model/openapi/basic.py
+-rw-r--r--   0        0        0     1820 2022-11-09 10:04:21.000000 any_api-0.1.0.5/any_api/openapi/model/openapi/info.py
+-rw-r--r--   0        0        0     6703 2023-07-18 15:36:22.480206 any_api-0.1.0.5/any_api/openapi/model/openapi/security.py
+-rw-r--r--   0        0        0     1816 2023-07-18 15:36:22.480206 any_api-0.1.0.5/any_api/openapi/model/requests.py
+-rw-r--r--   0        0        0     3531 2023-07-18 15:36:22.480206 any_api-0.1.0.5/any_api/openapi/model/responses.py
+-rw-r--r--   0        0        0      388 2023-01-10 16:04:06.000000 any_api-0.1.0.5/any_api/openapi/model/util.py
+-rw-r--r--   0        0        0    21921 2023-07-18 15:36:22.480206 any_api-0.1.0.5/any_api/openapi/openapi.py
+-rw-r--r--   0        0        0    20020 2023-07-18 15:36:22.480206 any_api-0.1.0.5/any_api/openapi/openapi_v1.py
+-rw-r--r--   0        0        0        0 2022-10-28 10:06:44.000000 any_api-0.1.0.5/any_api/openapi/to/__init__.py
+-rw-r--r--   0        0        0    11237 2023-07-18 15:36:22.480206 any_api-0.1.0.5/any_api/openapi/to/markdown.py
+-rw-r--r--   0        0        0      285 2023-01-09 03:46:58.000000 any_api-0.1.0.5/any_api/openapi/web_ui/__init__.py
+-rw-r--r--   0        0        0     1042 2022-10-25 03:45:48.000000 any_api-0.1.0.5/any_api/openapi/web_ui/elements.py
+-rw-r--r--   0        0        0     1196 2022-10-25 03:54:12.000000 any_api-0.1.0.5/any_api/openapi/web_ui/rapidoc.py
+-rw-r--r--   0        0        0     1021 2022-06-18 16:09:46.000000 any_api-0.1.0.5/any_api/openapi/web_ui/redoc.py
+-rw-r--r--   0        0        0     1285 2022-06-18 16:09:46.000000 any_api-0.1.0.5/any_api/openapi/web_ui/swagger.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.5/any_api/util/__init__.py
+-rw-r--r--   0        0        0     4343 2023-07-18 15:36:22.480206 any_api-0.1.0.5/any_api/util/by_pydantic.py
+-rw-r--r--   0        0        0     4297 2022-11-02 11:53:55.000000 any_api-0.1.0.5/any_api/util/i18n.py
+-rw-r--r--   0        0        0    11501 2023-07-18 15:36:22.480206 any_api-0.1.0.5/any_api/util/pydantic_adapter.py
+-rw-r--r--   0        0        0      193 2022-10-28 09:09:27.000000 any_api-0.1.0.5/any_api/util/util.py
+-rw-r--r--   0        0        0     1576 2023-07-18 15:38:08.714076 any_api-0.1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 any_api-0.1.0.5/setup.py
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 any_api-0.1.0.5/PKG-INFO
```

### Comparing `any_api-0.1.0.4/LICENSE` & `any_api-0.1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/asyncapi/asyncapi.py` & `any_api-0.1.0.5/any_api/asyncapi/asyncapi.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/asyncapi/model/asyncapi_model.py` & `any_api-0.1.0.5/any_api/asyncapi/model/asyncapi_model.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/asyncapi/model/operation_model.py` & `any_api-0.1.0.5/any_api/asyncapi/model/operation_model.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/base_api/base_api.py` & `any_api-0.1.0.5/any_api/base_api/base_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,56 @@
 import copy
 import json
-from typing import Any, Callable, Dict, Generic, Optional, Tuple, Type, TypeVar
+from typing import Any, Callable, Dict, Generic, List, Optional, Tuple, Type, TypeVar
 
 from pydantic import BaseModel
+from typing_extensions import Self
 
 from any_api.base_api.model.base_api_model import BaseAPIModel, BaseSecurityModel
 from any_api.openapi.model.openapi import TagModel
 from any_api.openapi.model.openapi.security import UserScopesOauth2SecurityModel
-from any_api.util import by_pydantic
+from any_api.util import pydantic_adapter
 
 __all__ = ["BaseAPI"]
 
 _ModelT = TypeVar("_ModelT", bound=BaseAPIModel)
+_ApiModelT = TypeVar("_ApiModelT")
 
 
-class BaseAPI(Generic[_ModelT]):
+class BaseAPI(Generic[_ModelT, _ApiModelT]):
     _api_model: _ModelT
     _schema_key: str = "schemas"
     _add_tag_dict: dict = {}
 
+    def __init__(self) -> None:
+        self._temp_model_list: List[_ApiModelT] = []
+        self._has_not_load_model: bool = False
+
+        self._model_name_map: pydantic_adapter.ModelNameMapType = {}
+        self._definitions: dict = {}
+        self._model_use_count: Dict[Type[BaseModel], int] = {}
+
+    def add_api_model(self, *api_model_list: _ApiModelT) -> "Self":
+        for api_model in api_model_list:
+            self._temp_model_list.append(api_model)
+        self._has_not_load_model = True
+        return self
+
+    def generate(self) -> None:
+        # The definition data must be reloaded each time the data is generated
+        self._load_definitions_by_api_model()
+        for api_model in self._temp_model_list:
+            self._add_request_to_api_model(api_model)
+
+    def _load_definitions_by_api_model(self) -> None:
+        raise NotImplementedError
+
+    def _add_request_to_api_model(self, api_model: _ApiModelT) -> "Self":
+        raise NotImplementedError
+
     def _add_tag(self, *tag_list: TagModel) -> None:
         for tag in tag_list:
             if tag.name not in self._add_tag_dict:
                 self._add_tag_dict[tag.name] = tag.description
                 self._api_model.tags.append(tag)
             elif tag.description != self._add_tag_dict[tag.name]:
                 raise ValueError(
@@ -62,49 +90,65 @@
                 self._replace_pydantic_definitions(value, parent_schema)
             elif isinstance(value, list):
                 for item in value:
                     if isinstance(item, dict):
                         self._replace_pydantic_definitions(item, parent_schema)
 
     def _xml_handler(self, schema_dict: dict) -> None:
+        """
+        Add XML support for schemas in a traversal and recursive manner,
+        the specific display method will be determined according to the media type,
+        and will not affect the data display of application/json
+        """
+        if "xml" in schema_dict:
+            return
         schema_dict["xml"] = {"name": schema_dict["title"]}
-        if "properties" in schema_dict:
-            for key, value in schema_dict["properties"].items():
-                if "type" not in value:
-                    continue
-                if value["type"] != "array":
-                    continue
-                value["xml"] = {"wrapped": True}
-                if "$ref" not in value["items"]:
-                    value["items"]["xml"] = {"name": value["title"]}
-        if "definitions" in schema_dict:
-            for _, _schema_dict in schema_dict["definitions"].items():
-                self._xml_handler(_schema_dict)
+        if "properties" not in schema_dict:
+            return
+        for key, value in schema_dict["properties"].items():
+            # nested schema handler
+            if "$ref" in value:
+                _, _, schema_key, key = value["$ref"].split("/")
+                self._xml_handler(self._api_model.components[self._schema_key][key])
+
+            # array handler
+            if value.get("type", "") != "array":
+                continue
+            value["xml"] = {"wrapped": True}
+            if "$ref" not in value["items"]:
+                value["items"]["xml"] = {"name": value["title"]}
+            else:
+                _, _, schema_key, key = value["items"]["$ref"].split("/")
+                self._xml_handler(self._api_model.components[self._schema_key][key])
+
+    def _get_not_in_components_model_schema(self, model: Type[BaseModel]) -> dict:
+        return pydantic_adapter.model_json_schema(model)
+
+    def _get_in_components_model_schema(self, model: Type[BaseModel]) -> Tuple[str, dict]:
+        global_model_name = self._model_name_map[model]
+        schema_dict: dict = self._definitions[self._model_name_map[model]]
+        return global_model_name, schema_dict
 
     def _schema_handle(
         self,
         model: Type[BaseModel],
         enable_move_to_component: bool = True,
         is_xml_model: bool = False,
-        model_name: Optional[str] = None,
     ) -> Tuple[str, dict]:
+        from any_api.util import by_pydantic
+
         global_model_name = by_pydantic.get_model_global_name(model)
-        if model_name:
-            global_model_name = f"{model_name}_{global_model_name}"
 
         if (
             global_model_name in self._api_model.components[self._schema_key]
             and enable_move_to_component
             and not is_xml_model
         ):
             return global_model_name, self._api_model.components[self._schema_key][global_model_name]
         schema_dict: dict = copy.deepcopy(by_pydantic.any_api_model_schema(model))
-        # set custom title
-        if model_name is not None:
-            schema_dict["title"] = model_name
         if is_xml_model:
             self._xml_handler(schema_dict)
         self._replace_pydantic_definitions(schema_dict)
         if "definitions" in schema_dict:
             # fix del schema dict
             del schema_dict["definitions"]
         if enable_move_to_component:
@@ -116,19 +160,22 @@
             _, _, schema_key, key = schema_dict["$ref"].split("/")
             return self._api_model.components[self._schema_key][key]
         else:
             return schema_dict
 
     @property
     def model(self) -> _ModelT:
+        if self._has_not_load_model:
+            self.generate()
+            self._has_not_load_model = False
         return self._api_model
 
     @property
     def dict(self) -> dict:
-        openapi_dict: dict = self.model.dict(exclude_none=True, by_alias=True)
+        openapi_dict: dict = pydantic_adapter.model_dump(self.model, exclude_none=True, by_alias=True)
         # if not openapi_dict["info"]["terms_of_service"]:
         #     del openapi_dict["info"]["terms_of_service"]
         #
         # if not openapi_dict["info"]["content"]:
         #     del openapi_dict["info"]["license"]
         return openapi_dict
```

### Comparing `any_api-0.1.0.4/any_api/base_api/model/base_api_model.py` & `any_api-0.1.0.5/any_api/base_api/model/base_api_model.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/openapi/__init__.py` & `any_api-0.1.0.5/any_api/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/openapi/model/__init__.py` & `any_api-0.1.0.5/any_api/openapi/model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
-from pydantic import BaseModel, Field, root_validator, validator
+from pydantic import BaseModel, Field, root_validator
 
 from any_api.base_api.model.base_api_model import BaseSecurityModel
+from any_api.util import pydantic_adapter
 
 from .links import LinksModel
 from .openapi import OperationModel, TagModel
 from .requests import RequestModel
 from .responses import (
     BaseResponseModel,
     FileResponseModel,
@@ -78,37 +79,40 @@
             ' Components Object. If the security scheme is of type "oauth2" or "openIdConnect",'
             " then the value is a list of scope names required for the execution, and the list MAY be empty "
             "if authorization does not require a specified scope. For other security scheme types,"
             " the array MUST be empty."
         ),
     )
 
-    @validator("path")
+    @pydantic_adapter.field_validator("path")
     def validate_path(cls, path: str) -> str:
         if not path.startswith("/"):
             raise ValueError("path must start with `/`")
         return path
 
     def add_to_operation_model(self, openapi_model: OperationModel) -> None:
         pass
 
-    @root_validator
+    @pydantic_adapter.model_validator(mode="before")
     def after_init(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Data association after initializing data"""
         if "request_dict" in values:
             request_dict: Dict[HttpParamTypeLiteral, List[RequestModel]] = values["request_dict"]
             for http_param_type_name, request_model_list in request_dict.items():
                 for request_model in request_model_list:
                     if isinstance(request_model.model, tuple):
                         model_tuple: Tuple[Type[BaseModel]] = request_model.model
                     else:
                         model_tuple = (request_model.model,)
                     for model in model_tuple:
-                        for field_name, field in model.__fields__.items():
-                            if "links" in field.field_info.extra:
-                                link_model: LinksModel = field.field_info.extra.pop("links")
+                        for field_name, field in pydantic_adapter.model_fields(model).items():
+                            extra_dict = pydantic_adapter.get_extra_by_field_info(field)
+                            if "links" in extra_dict:
+                                # TODO pydantic v2
+                                # TODO Although the Key is removed, the generated schema still contains this value
+                                link_model: LinksModel = extra_dict.pop("links")
                                 link_model.register(
-                                    param_name=field.field_info.alias or field_name,
+                                    param_name=pydantic_adapter.get_field_info(field).alias or field_name,
                                     http_param_type_name=http_param_type_name,
                                     operation_id=values["operation_id"],
                                 )
         return values
```

### Comparing `any_api-0.1.0.4/any_api/openapi/model/links.py` & `any_api-0.1.0.5/any_api/openapi/model/links.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import TYPE_CHECKING, List, Optional, Type
 
 from pydantic import BaseModel
 
 from any_api.openapi.model import openapi as openapi_model
+from any_api.util import pydantic_adapter
 
 if TYPE_CHECKING:
     from .response import BaseResponseModel
 
 
 __all__ = ["LinksModel"]
 
@@ -51,20 +52,25 @@
                     f"Check expr: {self.openapi_runtime_expr} error."
                     "Please refer to the section of the document(https://swagger.io/docs/specification/links/) "
                     "at `Runtime Expression Syntax`"
                 )  # pragma: no cover
 
             base_model: Type[BaseModel] = self.response_model.response_data  # type: ignore
             for key in key_list:
-                if key not in base_model.__fields__:
+                model_fields = pydantic_adapter.model_fields(base_model)
+                if key not in model_fields:
                     raise ValueError(
                         f"check expr:{self.openapi_runtime_expr} error "  # type: ignore
                         f"from {self.response_model.response_data}"  # type: ignore
                     )
-                temp_type: Type = base_model.__fields__[key].type_
+                if pydantic_adapter.is_v1:
+                    temp_type: Type = model_fields[key].type_
+                else:
+                    temp_type = model_fields[key].annotation
+
                 if issubclass(temp_type, BaseModel):
                     base_model = temp_type
         else:
             raise ValueError(
                 "Only support $response.headerXXX or $response.bodyXXX. "
                 "Please refer to the section of the document(https://swagger.io/docs/specification/links/) "
                 "at `Runtime Expression Syntax`"
```

### Comparing `any_api-0.1.0.4/any_api/openapi/model/openapi/__init__.py` & `any_api-0.1.0.5/any_api/openapi/model/openapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 """
 pydantic.Base Model to store Open API objects
 
 refer to: https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.0.3.md
 """
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import BaseModel, Extra, Field, root_validator
+from pydantic import BaseModel, Field
 from typing_extensions import Literal
 
+from any_api.util import pydantic_adapter
+
 from ..util import HttpMethodLiteral
 from .basic import ExampleModel, ExternalDocumentationModel, RefModel, ServerModel, ServerVariableModel
 from .info import Contact, InfoModel, License
 from .security import (
     ApiKeySecurityModel,
     HttpSecurityModel,
     Oauth2SecurityModel,
     OAuthFlowModel,
     OAuthFlowsModel,
     OpenIdConnectUrlSecurityModel,
     SecurityModelType,
 )
 
+if pydantic_adapter.is_v1:
+    from pydantic import Extra as ConfigDict
+else:
+    from pydantic import ConfigDict
+
 
 class TagModel(BaseModel):
     name: str = Field(description="The name of the tag.")
     description: str = Field(
         "", description="A short description for the tag. CommonMark syntax MAY be used for rich text representation."
     )
     external_docs: Optional[ExternalDocumentationModel] = Field(
@@ -103,21 +110,19 @@
         default="",
         alias="in",
         description='The location of the parameter. Possible values are "query", "header", "path" or "cookie".',
     )
     in_stub: Literal["query", "header", "path", "cookie"] = Field(
         description=(
             "This value is a stand-in for `in`, and the value is automatically synchronized to `in` when initialized"
-        )
+        ),
+        exclude=True,
     )
 
-    class Config:
-        fields = {"in_stub": {"exclude": True}}
-
-    @root_validator(pre=True)
+    @pydantic_adapter.model_validator(mode="before")
     def set_in(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         values["in"] = values["in_stub"]
         return values
 
 
 class EncodingModel(BaseModel):
     content_type: str = Field(
@@ -373,23 +378,26 @@
         default=None,
         description=(
             "An array of Server Objects, which provide connectivity information to a target server. "
             "If the servers property is not provided, or is an empty array, "
             "the default value would be a Server Object with a url value of /."
         ),
     )
+    if pydantic_adapter.is_v1:
+
+        class Config:
+            extra = ConfigDict.allow
 
-    class Config:
-        extra = Extra.allow
+    else:
+        model_config = ConfigDict(extra="allow")
 
 
 class OpenAPIModel(BaseModel):
     openapi: str = Field(
         "3.0.0",
-        const=True,
         description=(
             "This string MUST be the semantic version number of the OpenAPI Specification version that the OpenAPI"
             " document uses. The openapi field SHOULD be used by tooling specifications and clients to interpret"
             " the OpenAPI document. This is not related to the API info.version string."
         ),
     )
     info: InfoModel = Field(
```

### Comparing `any_api-0.1.0.4/any_api/openapi/model/openapi/basic.py` & `any_api-0.1.0.5/any_api/openapi/model/openapi/basic.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/openapi/model/openapi/info.py` & `any_api-0.1.0.5/any_api/openapi/model/openapi/info.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/openapi/model/openapi/security.py` & `any_api-0.1.0.5/any_api/openapi/model/openapi/security.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import BaseModel, Field, root_validator
+from pydantic import BaseModel, Field
 
 from any_api.base_api.model.base_api_model import BaseSecurityModel
 from any_api.openapi.model.util import SecurityHttpParamTypeLiteral
+from any_api.util import pydantic_adapter
 
 
 class OAuthFlowModel(BaseModel):
     authorization_url: Optional[str] = Field(
         default=None,
         alias="authorizationUrl",
         description="The authorization URL to be used for this flow. This MUST be in the form of a URL.",
@@ -44,15 +45,16 @@
     )
     authorization_code: Optional[OAuthFlowModel] = Field(
         alias="authorizationCode",
         default=None,
         description="Configuration for the OAuth Authorization Code flow. Previously called accessCode in OpenAPI 2.0.",
     )
 
-    @root_validator(pre=True)
+    @pydantic_adapter.model_validator(mode="before")
+    @classmethod
     def check_include_model(cls, values: Dict[str, OAuthFlowModel]) -> Dict[str, OAuthFlowModel]:
         for key, oauth_flow_model in values.items():
             if key in ("implicit", "authorizationCode"):
                 if oauth_flow_model.authorization_url is None:
                     raise ValueError(f"{key}->{oauth_flow_model.__class__.__name__}->`authorizationUrl` not be empty")
             if key in ("authorizationCode", "password", "clientCredentials"):
                 if oauth_flow_model.token_url is None:
@@ -62,26 +64,26 @@
 
 class OpenIdConnectUrlSecurityModel(BaseSecurityModel):
     open_id_connect_url: str = Field(
         alias="openIdConnectUrl",
         description="OpenId Connect URL to discover OAuth2 configuration values. This MUST be in the form of a URL.",
     )
 
-    @root_validator(pre=True)
+    @pydantic_adapter.model_validator(mode="before")
     def set_type(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         values["type"] = "openIdConnect"
         return values
 
 
 class Oauth2SecurityModel(BaseSecurityModel):
     flows: OAuthFlowsModel = Field(
         description="An object containing configuration information for the flow types supported."
     )
 
-    @root_validator(pre=True)
+    @pydantic_adapter.model_validator(mode="before")
     def set_type(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         values["type"] = "oauth2"
         return values
 
     def get_security_scope(self) -> List[str]:
         scope_list: List[str] = []
         if self.flows.authorization_code:
@@ -98,15 +100,16 @@
         return scope_list
 
 
 class UserScopesOauth2SecurityModel(Oauth2SecurityModel):
     use_scopes: List[str] = Field(description="Scope for the real use Oauth2SecurityModel", default_factory=list)
     model: Oauth2SecurityModel = Field(description="Parent Oauth2SecurityModel")
 
-    @root_validator(pre=True)
+    @pydantic_adapter.model_validator(mode="before")
+    @classmethod
     def set_type(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         model: Oauth2SecurityModel = values["model"]
         values["flows"] = model.flows
         all_scopes = model.get_security_scope()
         scopes = values["use_scopes"]
         _scopes_set = set(scopes) - set(all_scopes)
         if len(_scopes_set) > 0:
@@ -131,15 +134,16 @@
         alias="bearerFormat",
         description=(
             "A hint to the client to identify how the bearer token is formatted. Bearer tokens are usually generated by"
             " an authorization server, so this information is primarily for documentation purposes."
         ),
     )
 
-    @root_validator(pre=True)
+    @pydantic_adapter.model_validator(mode="before")
+    @classmethod
     def set_type(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         values["type"] = "http"
         return values
 
 
 class ApiKeySecurityModel(BaseSecurityModel):
     name: str = Field(description="The name of the header, query or cookie parameter to be used.")
@@ -147,21 +151,19 @@
         default="",
         alias="in",
         description=' The location of the API key. Valid values are "query", "header" or "cookie".',
     )
     in_stub: SecurityHttpParamTypeLiteral = Field(
         description=(
             "This value is a stand-in for `in`, and the value is automatically synchronized to `in` when initialized"
-        )
+        ),
+        exclude=True,
     )
 
-    class Config:
-        fields = {"in_stub": {"exclude": True}}
-
-    @root_validator(pre=True)
+    @pydantic_adapter.model_validator(mode="before")
     def set_type(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         values["type"] = "apiKey"
         values["in"] = values["in_stub"]
         return values
 
 
 SecurityModelType = Union[ApiKeySecurityModel, HttpSecurityModel, Oauth2SecurityModel, OpenIdConnectUrlSecurityModel]
```

### Comparing `any_api-0.1.0.4/any_api/openapi/model/requests.py` & `any_api-0.1.0.5/any_api/openapi/model/requests.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,15 +24,27 @@
 
     ################
     # content info #
     ################
     media_type_list: List[str] = Field("", description="OpenAPI media type")
     openapi_serialization: Optional[dict] = Field(None, description="OpenAPI serialization")
     model: Union[Type[BaseModel], Tuple[Type[BaseModel]]] = Field(description="request model")
-    model_key: Optional[str] = Field(
+
+    # e.g:
+    #   model schema:
+    #       {
+    #           'title': 'DynamicModel',
+    #           'type': 'object',
+    #           'properties': {'fake': {'title': 'Fake', 'format': 'binary', 'type': 'string'}},
+    #           'required': ['fake']
+    #       }
+    #
+    #   nested_model_key: fake
+    #   get really schema:
+    #       {'title': 'Fake', 'format': 'binary', 'type': 'string'}
+    nested_model_key: Optional[str] = Field(
         default=None,
         description=(
             "Usually the schema of the Request Body is the schema of the model,"
             " but sometimes the schema of a field of the model is required"
-            ' e.g. schema: { "type": "string", "format": "binary" }'
         ),
     )
```

### Comparing `any_api-0.1.0.4/any_api/openapi/model/responses.py` & `any_api-0.1.0.5/any_api/openapi/model/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Optional, Tuple, Type, Union
 
 from pydantic import BaseModel
 from typing_extensions import Literal
 
 from any_api.openapi.model import openapi as openapi_model
-from any_api.util.by_pydantic import gen_example_dict_from_schema
+from any_api.util.pydantic_adapter import gen_example_dict_from_schema
 
 __all__ = [
     "BaseResponseModel",
     "HtmlResponseModel",
     "JsonResponseModel",
     "FileResponseModel",
     "TextResponseModel",
@@ -19,20 +19,20 @@
 _resp_model_class_link_dict: Dict[str, Dict[str, openapi_model.LinkModel]] = {}
 
 
 class BaseResponseModel(object):
     """response model https://swagger.io/docs/specification/describing-responses/"""
 
     # response data
-    response_data: Union[Type[BaseModel], str, bytes, None]
+    response_data: Union[Type[BaseModel], str, bytes, None] = None
     # response media type
     media_type: str = "*/*"
 
-    # response name, if the value is empty, the name of the response_data object will be used
-    name: Optional[str] = None
+    # # response name, if the value is empty, the name of the response_data object will be used
+    # name: Optional[str] = None
     # response description
     description: Optional[str] = None
     # response header
     header: Optional[Type[BaseModel]] = None
     # response status code
     status_code: Union[Tuple[int, ...], Literal["default"]] = (200,)
```

### Comparing `any_api-0.1.0.4/any_api/openapi/openapi.py` & `any_api-0.1.0.5/any_api/openapi/openapi_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+import inspect
+import warnings
 from typing import Dict, List, Optional, Type
 
 from pydantic import BaseModel
 from typing_extensions import Literal
 
 from any_api.base_api.base_api import BaseAPI
 from any_api.openapi.model import ApiModel
 from any_api.openapi.model import openapi as openapi_model
 from any_api.openapi.model import requests, responses
 from any_api.openapi.model.util import HttpMethodLiteral, HttpParamTypeLiteral
+from any_api.util import pydantic_adapter
 
 __all__ = ["OpenAPI"]
 
+warnings.warn("This module is being deprecated, please use OpenAPI instead", DeprecationWarning, stacklevel=2)
 
-class OpenAPI(BaseAPI[openapi_model.OpenAPIModel]):
+
+class OpenAPI(BaseAPI[openapi_model.OpenAPIModel, ApiModel]):
     def __init__(
         self,
         openapi_info_model: Optional[openapi_model.InfoModel] = None,
         server_model_list: Optional[List[openapi_model.ServerModel]] = None,
         tag_model_list: Optional[List[openapi_model.TagModel]] = None,
         external_docs: Optional[openapi_model.ExternalDocumentationModel] = None,
         security_dict: Optional[Dict[str, openapi_model.SecurityModelType]] = None,
@@ -37,14 +42,15 @@
         if external_docs:
             self._api_model.external_docs = external_docs
         if security_dict:
             self._api_model.components["securitySchemes"] = security_dict
         if tag_model_list:
             for tag_model in tag_model_list:
                 self._add_tag(tag_model)
+        super().__init__()
 
     @classmethod
     def build(
         cls,
         openapi_info_model: Optional[openapi_model.InfoModel] = None,
         server_model_list: Optional[List[openapi_model.ServerModel]] = None,
         tag_model_list: Optional[List[openapi_model.TagModel]] = None,
@@ -160,16 +166,16 @@
                         **api_request.openapi_serialization
                     )
                     if "multipart/form-data" in content_dict:
                         self._get_real_schema_dict(content_dict[media_type].schema_)["properties"][key][
                             "description"
                         ] += "     \n >Swagger UI could not support, when media_type is multipart/form-data"
             else:
-                if api_request.model_key is not None:
-                    real_schema_dict = schema_dict["properties"][api_request.model_key]
+                if api_request.nested_model_key is not None:
+                    real_schema_dict = schema_dict["properties"][api_request.nested_model_key]
                 else:
                     real_schema_dict = {"$ref": f"#/components/schemas/{global_model_name}"}
                 if media_type in content_dict:
                     if request_body_is_array:
                         raise ValueError("request body is array, not support multi diff request body")
                     if "oneOf" not in content_dict[media_type].schema_:
                         content_dict[media_type].schema_["oneOf"] = []
@@ -255,15 +261,14 @@
                 getattr(resp_model, "response_data", None)
                 and isinstance(resp_model.response_data, type)
                 and issubclass(resp_model.response_data, BaseModel)
             ):
                 global_model_name, schema_dict = self._schema_handle(
                     resp_model.response_data,
                     is_xml_model="application/xml" == resp_model.media_type,
-                    model_name=resp_model.name,
                 )
 
             if isinstance(resp_model.status_code, str):
                 # support status_code is default
                 status_code_tuple: tuple = (resp_model.status_code,)
             else:
                 status_code_tuple = resp_model.status_code
@@ -327,18 +332,41 @@
                 else:
                     openapi_schema_dict = {"oneOf": path_list}
 
                 content_dict[media_type] = openapi_model.MediaTypeModel(schema=openapi_schema_dict)
             response_dict[status_code_str].content = content_dict
         operation_model.responses = response_dict
 
-    def add_api_model(self, *api_model_list: ApiModel) -> "OpenAPI":
-        for api_model in api_model_list:
-            self._add_request_to_api_model(api_model)
-        return self
+    def _load_definitions_by_api_model(self) -> None:
+        in_components_model_list: List[Type[BaseModel]] = []
+        for api_model in self._temp_model_list:
+            for param_type in HttpParamTypeLiteral.__args__:  # type: ignore
+                if param_type not in ("body", "form", "json", "multiform"):
+                    continue
+                request_list = api_model.request_dict.get(param_type, [])
+                if not request_list:
+                    continue
+                for api_request in request_list:
+                    if isinstance(api_request.model, tuple):
+                        for _model in api_request.model:
+                            in_components_model_list.append(_model)
+                    else:
+                        in_components_model_list.append(api_request.model)
+            for resp_model_class in api_model.response_list:
+                if not isinstance(resp_model_class, tuple):
+                    resp_model_class = (resp_model_class,)
+                for _resp_model_class in resp_model_class:
+                    resp_model: responses.BaseResponseModel = _resp_model_class()
+                    if (
+                        resp_model.response_data
+                        and inspect.isclass(resp_model.response_data)
+                        and issubclass(resp_model.response_data, BaseModel)
+                    ):
+                        in_components_model_list.append(resp_model.response_data)
+        self._model_name_map, self._definitions = pydantic_adapter.get_model_definitions(*in_components_model_list)
 
     def _add_request_to_api_model(self, api_model: ApiModel) -> "OpenAPI":
         path_dict: Dict[HttpMethodLiteral, openapi_model.OperationModel] = {}
         if api_model.path not in self._api_model.paths:
             self._api_model.paths[api_model.path] = path_dict
         else:
             path_dict = self._api_model.paths[api_model.path]
```

### Comparing `any_api-0.1.0.4/any_api/openapi/to/markdown.py` & `any_api-0.1.0.5/any_api/openapi/to/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from typing import Dict, List, Type, Union
 
 from typing_extensions import TypedDict
 
 from any_api.openapi.model import openapi as openapi_model
 from any_api.openapi.openapi import OpenAPI
-from any_api.util.by_pydantic import gen_example_dict_from_schema
 from any_api.util.i18n import I18n, I18nContext, i18n_local, join_i18n
+from any_api.util.pydantic_adapter import gen_example_dict_from_schema
 
 
 class ParamTypedDict(TypedDict):
     name: str
     required: bool
     description: str
     example: str
```

### Comparing `any_api-0.1.0.4/any_api/openapi/web_ui/elements.py` & `any_api-0.1.0.5/any_api/openapi/web_ui/elements.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/openapi/web_ui/rapidoc.py` & `any_api-0.1.0.5/any_api/openapi/web_ui/rapidoc.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/openapi/web_ui/redoc.py` & `any_api-0.1.0.5/any_api/openapi/web_ui/redoc.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/openapi/web_ui/swagger.py` & `any_api-0.1.0.5/any_api/openapi/web_ui/swagger.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/any_api/util/by_pydantic.py` & `any_api-0.1.0.5/any_api/util/pydantic_adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,154 @@
+"""
+Compatible with V1 and V 2 versions of pydantic
+"""
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Set, Tuple, Type, Union
-
-from pydantic import create_model
-from pydantic.schema import (
-    default_ref_template,
-    get_flat_models_from_model,
-    get_long_model_name,
-    get_model,
-    get_schema_ref,
-    model_process_schema,
-    normalize_name,
-)
-
-if TYPE_CHECKING:
-    from pydantic import BaseConfig, BaseModel
-    from pydantic.dataclasses import Dataclass
-    from pydantic.schema import TypeModelOrEnum, TypeModelSet
-
-
-__all__ = ["any_api_model_schema", "create_pydantic_model", "get_model_global_name", "gen_example_dict_from_schema"]
-
-global_name_model_map = {}
-global_conflicting_names: Set[str] = set()
+from functools import partial
+from typing import Any, Callable, Dict, Optional, Tuple, Type
 
+from pydantic import BaseConfig, BaseModel, create_model
+from pydantic.fields import FieldInfo
+from pydantic.version import VERSION
+
+is_v1: bool = VERSION.startswith("1")
+ModelNameMapType = Dict[Type[BaseModel], str]
+DefinitionsReturnType = Tuple[ModelNameMapType, dict]
+
+__all__ = [
+    # var
+    "is_v1",
+    "ModelNameMapType",
+    "DefinitionsReturnType",
+    "VERSION",
+    "ConfigDict",
+    # pydantic compat func
+    "get_model_definitions",
+    "model_json_schema",
+    "model_validator",
+    "model_dump",
+    "field_validator",
+    "model_fields",
+    # util func
+    "get_extra_by_field_info",
+    "create_pydantic_model",
+    "json_type_default_value_dict",
+    "gen_example_dict_from_schema",
+    "remove_any_of",
+]
+
+
+if is_v1:
+    from pydantic import root_validator as _model_validator
+    from pydantic import validator as _field_validator
+    from pydantic.fields import ModelField
+    from pydantic.schema import get_flat_models_from_model, get_model_name_map, model_process_schema
+
+    ConfigDict = dict
+
+    def get_model_definitions(
+        *model_sequence: Type[BaseModel], ref_prefix: str = "#/components/schemas/"
+    ) -> DefinitionsReturnType:
+        flat_models = set()
+        for model in model_sequence:
+            flat_models |= get_flat_models_from_model(model)
+        model_name_map = get_model_name_map(flat_models)
+
+        definitions: Dict[str, Dict[str, Any]] = {}
+        for model in flat_models:
+            m_schema, m_definitions, m_nested_models = model_process_schema(
+                model, model_name_map=model_name_map, ref_prefix=ref_prefix
+            )
+            definitions.update(m_definitions)
+            if model not in model_name_map:
+                raise ValueError(
+                    f"The current model may be a dynamically created model with a non-unique name."
+                    f" module:{model.__module__}, name:{model.__name__}"
+                )
+            model_name = model_name_map[model]
 
-def get_model_global_name(model: "TypeModelOrEnum") -> str:
-    return any_api_get_model_name_map({model})[model]
+            definitions[model_name] = m_schema
+        return model_name_map, definitions
 
+    def model_fields(model: Type[BaseModel]) -> Dict[str, ModelField]:
+        return model.__fields__
 
-def any_api_get_model_name_map(unique_models: "TypeModelSet") -> Dict["TypeModelOrEnum", str]:
-    """
-    Process a set of models and generate unique names for them to be used as keys in the JSON Schema
-    definitions. By default the names are the same as the class name. But if two models in different Python
+    def get_field_info(field: ModelField) -> FieldInfo:
+        return field.field_info
+
+else:
+    from pydantic import ConfigDict as _ConfigDict
+    from pydantic import field_validator as _field_validator
+    from pydantic import model_validator as _model_validator
+    from pydantic.json_schema import GenerateJsonSchema, JsonSchemaMode
+
+    ConfigDict = _ConfigDict  # type: ignore[misc]
+
+    def get_model_definitions(  # type: ignore[misc]
+        *model_sequence: Type[BaseModel],
+        ref_prefix: str = "#/components/schemas/{model}",
+        mode: JsonSchemaMode = "validation",
+    ) -> DefinitionsReturnType:
+        generate_instance = GenerateJsonSchema(by_alias=True, ref_template=ref_prefix)
+        model_name_map, definitions = generate_instance.generate_definitions(
+            [(model, mode, model.__pydantic_core_schema__) for model in model_sequence]
+        )
+        any_api_model_name_map = {}
+        replace_str = ref_prefix.split("{")[0]
+        for k, v in model_name_map.items():
+            any_api_model_name_map[k[0]] = v["$ref"].replace(replace_str, "")
+        return any_api_model_name_map, definitions
+
+    def model_fields(model: Type[FieldInfo]) -> Dict[str, FieldInfo]:
+        return model.model_fields
+
+    def get_field_info(field: FieldInfo) -> FieldInfo:
+        return field
+
+
+def model_json_schema(model: Type[BaseModel], definition_key: str = "$defs") -> dict:
+    if is_v1:
+        schema_dict = model.schema()
+        if "definitions" in schema_dict and definition_key != "definitions":
+            schema_dict[definition_key] = schema_dict["definitions"]
+    else:
+        from pydantic.json_schema import model_json_schema
 
+        schema_dict = model_json_schema(model)
+        if "$defs" in schema_dict and definition_key != "$defs":
+            schema_dict[definition_key] = schema_dict["$defs"]
+    return schema_dict
 
 
-    modules have the same name (e.g. "users.Model" and "items.Model"), the generated names will be
-    based on the Python module path for those conflicting models to prevent name collisions.
+def model_dump(model: BaseModel, **kwargs: Any) -> dict:
+    if is_v1:
+        return model.dict(**kwargs)
+    else:
+        return model.model_dump(**kwargs)
 
-    :param unique_models: a Python set of models
-    :return: dict mapping models to names
-    """
-    global global_name_model_map
-    global global_conflicting_names
 
-    for model in unique_models:
-        model_name = normalize_name(model.__name__)
-        if model_name in global_conflicting_names:
-            model_name = normalize_name(get_long_model_name(model))
-            global_name_model_map[model_name] = model
-        elif model_name in global_name_model_map:
-            if global_name_model_map[model_name] is model:
-                # No additional processing for the same model
-                continue
-            global_conflicting_names.add(model_name)
-            conflicting_model = global_name_model_map.pop(model_name)
-            global_name_model_map[normalize_name(get_long_model_name(conflicting_model))] = conflicting_model
-            global_name_model_map[normalize_name(get_long_model_name(model))] = model
+def model_validator(*, mode: str) -> Callable:
+    if mode == "before":
+        if is_v1:
+            return partial(_model_validator, pre=True)
         else:
-            global_name_model_map[model_name] = model
-    return {v: k for k, v in global_name_model_map.items()}
+            return _model_validator(mode=mode)
+    else:
+        raise RuntimeError(f"Not support `{mode}`")
 
 
-def any_api_model_schema(
-    model: Union[Type["BaseModel"], Type["Dataclass"]],
-    by_alias: bool = True,
-    ref_prefix: Optional[str] = None,
-    ref_template: str = default_ref_template,
-) -> Dict[str, Any]:
-    """
-    Generate a JSON Schema for one model. With all the sub-models defined in the ``definitions`` top-level
-    JSON key.
+def field_validator(*args: Any, **kwargs: Any) -> Callable:
+    return _field_validator(*args, **kwargs)
 
-    :param model: a Pydantic model (a class that inherits from BaseModel)
-    :param by_alias: generate the schemas using the aliases defined, if any
-    :param ref_prefix: the JSON Pointer prefix for schema references with ``$ref``, if None, will be set to the
-      default of ``#/definitions/``. Update it if you want the schemas to reference the definitions somewhere
-      else, e.g. for OpenAPI use ``#/components/schemas/``. The resulting generated schemas will still be at the
-      top-level key ``definitions``, so you can extract them from there. But all the references will have the set
-      prefix.
-    :param ref_template: Use a ``string.format()`` template for ``$ref`` instead of a prefix. This can be useful for
-      references that cannot be represented by ``ref_prefix`` such as a definition stored in another file. For a
-      sibling json file in a ``/schemas`` directory use ``"/schemas/${model}.json#"``.
-    :return: dict with the JSON Schema for the passed ``model``
-    """
-    model = get_model(model)
-    flat_models = get_flat_models_from_model(model)
-    model_name_map = any_api_get_model_name_map(flat_models)
-    model_name = model_name_map[model]
-    m_schema, m_definitions, nested_models = model_process_schema(
-        model, by_alias=by_alias, model_name_map=model_name_map, ref_prefix=ref_prefix, ref_template=ref_template
-    )
-    if model_name in nested_models:
-        # model_name is in Nested models, it has circular references
-        m_definitions[model_name] = m_schema  # pragma: no cover
-        m_schema = get_schema_ref(model_name, ref_prefix, ref_template, False)  # pragma: no cover
-    if m_definitions:
-        m_schema.update({"definitions": m_definitions})
-    return m_schema
+
+def get_extra_by_field_info(field: Any) -> dict:
+    if is_v1:
+        extra_dict: dict = field.field_info.extra
+    else:
+        extra_dict = field.json_schema_extra or {}
+    return extra_dict
 
 
 def create_pydantic_model(
     annotation_dict: Optional[Dict[str, Tuple[Type, Any]]] = None,
     class_name: str = "DynamicModel",
     pydantic_config: Optional[Type["BaseConfig"]] = None,
     pydantic_base: Optional[Type["BaseModel"]] = None,
@@ -198,7 +245,84 @@
                         raise KeyError(f"Can not found type: {key} in json type")
                     gen_dict[key] = json_type_default_value_dict[value["type"]]
                 else:
                     gen_dict[key] = "object"
             if isinstance(gen_dict[key], Enum):
                 gen_dict[key] = gen_dict[key].value
     return gen_dict
+
+
+def remove_any_of(schema_dict: dict) -> None:
+    """
+    Fix issue:  https://github.com/pydantic/pydantic/issues/6647
+    remove schema anyOf key
+
+    e.g.:
+            class Demo(BaseModel):
+                a: Optional[in] = Field()
+
+        pydantic v1 output:
+            {
+                'title': 'Demo',
+                'type': 'object',
+                'properties': {'a': {'$ref': '#/definitions/SubDemo'}},
+                'definitions': {
+                    'SubDemo': {
+                        'title': 'SubDemo',
+                        'type': 'object',
+                        'properties': {'a': {'title': 'A', 'type': 'integer'}},
+                        'required': ['a']}
+                }
+            }
+
+        pydantic v2 output:
+            {
+                '$defs': {
+                    'SubDemo': {
+                        'properties': {'a': {'title': 'A', 'type': 'integer'}},
+                        'required': ['a'],
+                        'title': 'SubDemo',
+                        'type': 'object'
+                    }
+                },
+                'properties': {'a': {'anyOf': [{'$ref': '#/$defs/SubDemo'}, {'type': 'null'}]}},
+                'required': ['a'],
+                'title': 'Demo',
+                'type': 'object'
+            }
+    """
+    for k in list(schema_dict.keys()):
+        v = schema_dict[k]
+        if isinstance(v, dict):
+            if "anyOf" in v:
+                any_of_sub_value = {}
+                any_of_value = v["anyOf"]
+                if len(any_of_value) == 2:
+                    if any_of_value[0].get("type", "") == "null":
+                        any_of_sub_value = any_of_value[1]
+                    elif any_of_value[1].get("type", "") == "null":
+                        any_of_sub_value = any_of_value[0]
+
+                if "$ref" in any_of_sub_value:
+                    v.update(any_of_sub_value)
+                    v.pop("anyOf")
+                elif "items" in any_of_sub_value and "$ref" in any_of_sub_value["items"]:
+                    # some like:
+                    # {
+                    #   'tags':
+                    #       {
+                    #           'anyOf': [
+                    #               {'items': {'$ref': '#/components/schemas/Tag'}, 'type': 'array'},
+                    #               {'type': 'null'}
+                    #            ],
+                    #            'default': None,
+                    #            'title': 'Tags'
+                    #       }
+                    # }
+                    v.update(any_of_sub_value)
+                    v.pop("anyOf")
+            else:
+                remove_any_of(v)
+        elif isinstance(v, list):
+            for item in v:
+                if isinstance(item, dict):
+                    remove_any_of(item)
```

### Comparing `any_api-0.1.0.4/any_api/util/i18n.py` & `any_api-0.1.0.5/any_api/util/i18n.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.4/pyproject.toml` & `any_api-0.1.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 [tool.poetry]
 name = "any-api"
-version = "v0.1.0.4"
+version = "v0.1.0.5"
 description = "Quick and easy to create OpenAPI/AsyncAPI, and provide corresponding extensions"
 authors = ["so1n <qaz6803609@163.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pydantic = "^1.9.2"
+pydantic = ">=1.9.2, <3.0.0"
 
 [tool.poetry.dev-dependencies]
-black = "20.8b1"
-mypy = "0.790"
-pytest = "6.1.2"
-isort = "5.6.4"
+pytest = "6.2.5"
 coverage = "5.5"
 pytest-mock = "3.5.1"
 python-multipart = "0.0.5"
 pre-commit = "2.14.0"
-autoflake = "1.4"
-
 
 
 [tool.poetry-dynamic-versioning]
 enable = false
 metadata=false
 vcs = "git"
 format = "v{base}"
```

### Comparing `any_api-0.1.0.4/setup.py` & `any_api-0.1.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,19 @@
  'any_api.openapi.web_ui',
  'any_api.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pydantic>=1.9.2,<2.0.0']
+['pydantic>=1.9.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'any-api',
-    'version': '0.1.0.4',
+    'version': '0.1.0.5',
     'description': 'Quick and easy to create OpenAPI/AsyncAPI, and provide corresponding extensions',
     'long_description': 'None',
     'author': 'so1n',
     'author_email': 'qaz6803609@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `any_api-0.1.0.4/PKG-INFO` & `any_api-0.1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: any-api
-Version: 0.1.0.4
+Version: 0.1.0.5
 Summary: Quick and easy to create OpenAPI/AsyncAPI, and provide corresponding extensions
 License: Apache-2.0
 Author: so1n
 Author-email: qaz6803609@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.9.2,<2.0.0)
+Requires-Dist: pydantic (>=1.9.2,<3.0.0)
```

