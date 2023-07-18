# Comparing `tmp/django_api_decorator-0.1.7.tar.gz` & `tmp/django_api_decorator-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_api_decorator-0.1.7.tar", max compression
+gzip compressed data, was "django_api_decorator-0.2.0a1.tar", max compression
```

## Comparing `django_api_decorator-0.1.7.tar` & `django_api_decorator-0.2.0a1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/LICENSE
--rw-r--r--   0        0        0      373 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/__init__.py
--rw-r--r--   0        0        0      390 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/apps.py
--rw-r--r--   0        0        0    17702 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/decorators.py
--rw-r--r--   0        0        0        0 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/management/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/management/commands/generate_api_schemas.py
--rw-r--r--   0        0        0    13052 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/openapi.py
--rw-r--r--   0        0        0        0 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/py.typed
--rw-r--r--   0        0        0     1574 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/schema_file.py
--rw-r--r--   0        0        0     1585 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/type_utils.py
--rw-r--r--   0        0        0      870 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/types.py
--rw-r--r--   0        0        0     1993 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/django_api_decorator/utils.py
--rw-r--r--   0        0        0     1075 2023-07-14 14:25:19.879207 django_api_decorator-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 django_api_decorator-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-18 10:44:42.553767 django_api_decorator-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0      373 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/apps.py
+-rw-r--r--   0        0        0    12218 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/decorators.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/management/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/management/commands/generate_api_schemas.py
+-rw-r--r--   0        0        0     8958 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/openapi.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/py.typed
+-rw-r--r--   0        0        0     1552 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/schema_file.py
+-rw-r--r--   0        0        0     1037 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/types.py
+-rw-r--r--   0        0        0     1993 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/utils.py
+-rw-r--r--   0        0        0     1074 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 django_api_decorator-0.2.0a1/PKG-INFO
```

### Comparing `django_api_decorator-0.1.7/LICENSE` & `django_api_decorator-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.1.7/django_api_decorator/decorators.py` & `django_api_decorator-0.2.0a1/django_api_decorator/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,24 @@
-import dataclasses
-import datetime
 import functools
 import inspect
-import json
 import logging
-import types
 import typing
 from collections.abc import Callable, Mapping
-from typing import Any, Protocol, TypedDict, cast
+from typing import Annotated, Any, TypedDict
 
 import pydantic
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist, ValidationError
 from django.db import transaction
 from django.http import Http404, HttpRequest, HttpResponse, JsonResponse
 from django.views.decorators.http import require_http_methods
-from pydantic.json import pydantic_encoder
+from pydantic.fields import FieldInfo
+from pydantic.functional_validators import BeforeValidator
+from pydantic_core import PydanticUndefined
 
-from .type_utils import (
-    is_list,
-    is_optional,
-    is_union,
-    unwrap_list_item_type,
-    unwrap_optional,
-)
 from .types import ApiMeta, FieldError, PublicAPIError
 
 P = typing.ParamSpec("P")
 T = typing.TypeVar("T")
 
 Annotation = Any
 
@@ -77,40 +68,40 @@
     atomic = (
         atomic
         if atomic is not None
         else getattr(settings, "API_DECORATOR_DEFAULT_ATOMIC", True)
     )
 
     def default_auth_check(request: HttpRequest) -> bool:
-        return request.user.is_authenticated
+        return hasattr(request, "user") and request.user.is_authenticated
 
     _auth_check = (
         auth_check
         if auth_check is not None
         else getattr(settings, "API_DECORATOR_AUTH_CHECK", default_auth_check)
     )
 
     def decorator(func: Callable[..., Any]) -> Callable[..., HttpResponse]:
         signature = inspect.signature(func)
 
         # Get a function that we can call to extract view parameters from
         # the requests query parameters.
-        parse_query_params = _get_query_param_parser(
+        query_params_model = _get_query_params_model(
             parameters=signature.parameters, query_params=query_params or []
         )
 
         # If the method has a "body" argument, get a function to call to parse
         # the request body into the type expected by the view.
-        body_parser: BodyParser | None = None
+        body_adapter = None
         if "body" in signature.parameters:
-            body_parser = _get_body_parser(parameter=signature.parameters["body"])
+            body_adapter = _get_body_adapter(parameter=signature.parameters["body"])
 
         # Get a function to use for encoding the value returned from the view
         # into a request we can return to the client.
-        response_encoder = _get_response_encoder(
+        response_adapter = _get_response_adapter(
             type_annotation=signature.return_annotation
         )
 
         @functools.wraps(func)
         @transaction.non_atomic_requests()
         @require_http_methods([method])
         def inner(request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
@@ -120,19 +111,27 @@
                 return JsonResponse({"errors": ["Login required"]}, status=401)
 
             try:
                 extra_kwargs = {}
 
                 # Parse the request body if the request method allows a body and the
                 # view has requested that we should parse the body.
-                if _can_have_body(request.method) and body_parser:
-                    extra_kwargs["body"] = body_parser(request=request)
+                if _can_have_body(request.method) and body_adapter:
+                    extra_kwargs["body"] = body_adapter.validate_json(request.body)
 
                 # Parse query params and add them to the parameters given to the view.
-                extra_kwargs.update(parse_query_params(request))
+                raw_query_params: dict[str, Any] = {}
+                for key in request.GET:
+                    if value := request.GET.getlist(key):
+                        raw_query_params[key] = value[0] if len(value) == 1 else value
+                    else:
+                        raw_query_params[key] = True
+
+                query_params = query_params_model.model_validate(raw_query_params)
+                extra_kwargs.update(query_params.model_dump(exclude_defaults=True))
             except (
                 ValidationError,
                 pydantic.ValidationError,
             ) as e:
                 # Normalize and return a unified error message payload
                 return handle_validation_error(exception=e)
 
@@ -172,297 +171,111 @@
             # If the view returned an HttpRequest object, return that directly.
             # This can happen anytime regardless of what the view is typed to
             # return because of CSRF protections, that is called before the view
             # and may return an HttpResponse immediately without calling the view.
             if isinstance(response, HttpResponse):
                 return response
 
+            if not response_adapter:
+                raise TypeError(
+                    f"{func} is annotated to return an http response, but returned "
+                    f"{type(response)}"
+                )
+
             # Encode the response from the view to json and create a response object.
-            return response_encoder(payload=response, status=response_status)
+            payload = response_adapter.dump_json(response)
+            return HttpResponse(
+                payload, status=response_status, content_type="application/json"
+            )
 
         inner._api_meta = ApiMeta(  # type: ignore[attr-defined]
             method=method,
             query_params=query_params or [],
             response_status=response_status,
+            body_adapter=body_adapter,
+            query_params_model=query_params_model,
+            response_adapter=response_adapter,
         )
         return inner
 
     return decorator
 
 
 #######################
 # Query param parsing #
 #######################
 
 
-class Validator(Protocol):
-    def __call__(self, value: str, *, query_param_name: str) -> Any:
-        ...
-
-
-class _missing:
-    """Marker for missing query parameters"""
-
-
-def _validate_int(value: str, *, query_param_name: str) -> int:
-    try:
-        return int(value)
-    except (TypeError, ValueError):
-        raise ValidationError(f"{query_param_name} must be an integer")
+def validate_boolean(value: Any) -> Any:
+    return True if value == "" else value
 
 
-def _validate_bool(value: str, *, query_param_name: str) -> bool:
-    value = value.lower().strip()
+TYPE_MAPPING = {
+    bool: Annotated[bool, BeforeValidator(validate_boolean)],  # type: ignore[call-arg]
+}
 
-    if value in ("", "yes", "on", "true", "1"):
-        return True
 
-    if value in ("no", "off", "false", "0"):
-        return False
-
-    raise ValidationError(f"{query_param_name} must be a boolean")
-
-
-def _validate_date(value: str, *, query_param_name: str) -> datetime.date:
-    try:
-        return datetime.date.fromisoformat(value)
-    except ValueError:
-        raise ValidationError(f"{query_param_name} must be a valid date")
-
-
-def _get_validator(parameter: inspect.Parameter) -> Validator:
-    annotation = parameter.annotation
-    if annotation is inspect.Parameter.empty:
-        raise ValueError(
-            f"Parameter {parameter.name} specified as a query param must have a"
-            f" type annotation."
-        )
-
-    param_is_optional = is_optional(annotation)
-
-    if param_is_optional and parameter.default is inspect.Parameter.empty:
-        raise ValueError(
-            f"Parameter {parameter.name} specified as an optional param must have a"
-            f" default value."
-        )
-
-    if annotation is str or (param_is_optional and unwrap_optional(annotation) is str):
-        return lambda value, query_param_name: value
-
-    if annotation is int or (param_is_optional and unwrap_optional(annotation) is int):
-        return _validate_int
-
-    if annotation is datetime.date or (
-        param_is_optional and unwrap_optional(annotation) is datetime.date
-    ):
-        return _validate_date
-
-    if annotation is bool or (
-        param_is_optional and unwrap_optional(annotation) is bool
-    ):
-        return _validate_bool
-
-    raise ValueError(
-        f"Unsupported type annotation for query param {parameter.name}: {annotation}"
-    )
-
-
-def _get_query_param_parser(
+def _get_query_params_model(
     *,
     parameters: Mapping[str, inspect.Parameter],
     query_params: list[str],
-) -> Callable[[HttpRequest], Mapping[str, Any]]:
-    query_param_mapping = (
-        {query_param.replace("_", "-"): query_param for query_param in query_params}
-        if query_params
-        else {}
-    )
-    query_param_validators = {
-        query_param: _get_validator(parameters[arg_name])
-        for query_param, arg_name in query_param_mapping.items()
-    }
-    required_params = {
-        arg_name
-        for query_param, arg_name in query_param_mapping.items()
-        if parameters[arg_name].default is inspect.Parameter.empty
-    }
-
-    def parser(request: HttpRequest) -> Mapping[str, Any]:
-        validated = {}
-
-        for query_param, arg_name in query_param_mapping.items():
-            validator = query_param_validators[query_param]
-            value = request.GET.get(query_param, _missing)
-
-            # If the argument is required, make sure it has a value
-            if value is _missing:
-                if arg_name in required_params:
-                    raise ValidationError(
-                        f"Query parameter {query_param} must be specified"
-                    )
-            else:
-                validated[arg_name] = validator(
-                    cast(str, value), query_param_name=query_param
-                )
-
-        return validated
+) -> pydantic.BaseModel:
+    if any(arg_name not in parameters for arg_name in query_params):
+        raise TypeError("All parameters specified in query_params must exist")
+
+    fields: dict[str, tuple[Any, FieldInfo]] = {}
+
+    for arg_name in query_params:
+        annotation = parameters[arg_name].annotation
+        annotation = TYPE_MAPPING.get(annotation, annotation)
+        field = pydantic.fields.Field(
+            default=(
+                parameters[arg_name].default
+                if not parameters[arg_name].default == inspect.Parameter.empty
+                else PydanticUndefined
+            ),
+            alias=arg_name.replace("_", "-") if "_" in arg_name else None,
+        )
+        fields[arg_name] = (annotation, field)
 
-    return parser
+    return pydantic.create_model(  # type: ignore[no-any-return,call-overload]
+        "QueryParams", **fields
+    )
 
 
 ################
 # Body parsing #
 ################
 
 
-class BodyParser(Protocol):
-    def __call__(self, *, request: HttpRequest) -> Any:
-        ...
-
-
 def _can_have_body(method: str | None) -> bool:
     return method in ("POST", "PATCH", "PUT")
 
 
-def _get_body_parser(*, parameter: inspect.Parameter) -> BodyParser:
+def _get_body_adapter(*, parameter: inspect.Parameter) -> pydantic.TypeAdapter[Any]:
     annotation = parameter.annotation
     if annotation is inspect.Parameter.empty:
         raise TypeError("The body parameter must have a type annotation")
 
-    body_is_list = is_list(type_annotation=annotation)
-    if body_is_list:
-        annotation = unwrap_list_item_type(type_annotation=annotation)
-
-    if issubclass(annotation, pydantic.BaseModel):
-        return _pydantic_parser(model_cls=annotation, body_is_list=body_is_list)
-
-    raise ValueError(
-        f"Annotation for body parameter must be a django-rest-framework or pydantic "
-        f"serializer class, the current type annotation is: {annotation}"
-    )
-
-
-def _pydantic_parser(
-    *, model_cls: type[pydantic.BaseModel], body_is_list: bool
-) -> BodyParser:
-    def parser(
-        *, request: HttpRequest
-    ) -> pydantic.BaseModel | list[pydantic.BaseModel]:
-        try:
-            data = json.loads(request.body)
-        except json.decoder.JSONDecodeError as e:
-            raise ValidationError("Invalid JSON") from e
-
-        if body_is_list:
-            if not isinstance(data, list):
-                raise ValidationError("Expected request body to be a list")
-
-            if not len(data):
-                raise ValidationError("Empty list not allowed")
-
-            result = []
-            for i, element in enumerate(data):
-                if not isinstance(element, dict):
-                    raise ValidationError(f"Expected list element {i} to be an object")
-
-                result.append(model_cls(**element))
-            return result
-
-        else:
-            if not isinstance(data, dict):
-                raise ValidationError("Expected request body to be an object")
-
-            instance = model_cls(**data)
-            return instance
-
-    return parser
+    return pydantic.TypeAdapter(annotation)
 
 
 #####################
 # Response encoding #
 #####################
 
 
-class ResponseEncoder(Protocol):
-    def __call__(self, *, payload: Any, status: int) -> HttpResponse:
-        ...
-
-
-def _is_class(*, type_annotation: Annotation) -> bool:
-    return inspect.isclass(type_annotation) and (
-        type(type_annotation)
-        is not types.GenericAlias  # type: ignore[comparison-overlap]
-    )
-
-
-def _get_response_encoder(*, type_annotation: Annotation) -> ResponseEncoder:
-    type_is_class = _is_class(type_annotation=type_annotation)
-
-    if type_is_class and issubclass(type_annotation, HttpResponse):
-        return lambda payload, status: payload
-
-    if dataclasses.is_dataclass(type_annotation):
-        return _dataclass_encoder
-
-    if type_is_class and issubclass(type_annotation, pydantic.BaseModel):
-        return _pydantic_encoder
-
-    # We need to unwrap inner list and union annotations
-    # to verify whether we support them.
-    inner_type_annotations: tuple[type, ...] = tuple()
-
-    type_is_list = is_list(type_annotation=type_annotation)
-    type_is_union = is_union(type_annotation=type_annotation)
-
-    if type_is_list or type_is_union:
-        inner_type_annotations = typing.get_args(type_annotation)
-
-    if inner_type_annotations and all(
-        _is_class(type_annotation=t) for t in inner_type_annotations
-    ):
-        # Pydantic encoder supports both list and Union wrappers
-        if all(issubclass(t, pydantic.BaseModel) for t in inner_type_annotations):
-            return _pydantic_encoder
-
-        if any(issubclass(t, pydantic.BaseModel) for t in inner_type_annotations):
-            raise NotImplementedError(
-                "@api: We only support all values being pydantic models in a union"
-            )
-
-        if any(dataclasses.is_dataclass(t) for t in inner_type_annotations):
-            raise NotImplementedError(
-                "@api: We do not support encoding dataclasses inside lists or unions"
-            )
-
-    # Assume any other response can be JSON encoded. We might want to restrict
-    # this to some verified types 🤔
-    return _json_encoder
-
-
-def _json_encoder(*, payload: Any, status: int) -> HttpResponse:
-    return JsonResponse(
-        payload,
-        status=status,
-        json_dumps_params={"default": pydantic_encoder},
-        safe=False,
-    )
-
-
-def _pydantic_encoder(payload: Any, status: int) -> HttpResponse:
-    return JsonResponse(
-        payload,
-        status=status,
-        json_dumps_params={"default": pydantic_encoder},
-        safe=False,
-    )
-
-
-def _dataclass_encoder(*, payload: Any, status: int) -> HttpResponse:
-    data = dataclasses.asdict(payload)
-    return _json_encoder(payload=data, status=status)
+def _get_response_adapter(
+    *, type_annotation: Annotation
+) -> pydantic.TypeAdapter[Any] | None:
+    if type_annotation == inspect.Parameter.empty:
+        raise TypeError("Missing annotation for return type of api view")
+    if type(type_annotation) is type and issubclass(type_annotation, HttpResponse):
+        return None
+    return pydantic.TypeAdapter(type_annotation)
 
 
 ##################
 # Error handling #
 ##################
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_api_decorator-0.1.7/django_api_decorator/management/commands/generate_api_schemas.py` & `django_api_decorator-0.2.0a1/django_api_decorator/management/commands/generate_api_schemas.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.1.7/django_api_decorator/openapi.py` & `django_api_decorator-0.2.0a1/django_api_decorator/openapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,25 @@
 import dataclasses
-import inspect
 import logging
 import re
-import typing
 from collections.abc import Callable, Sequence
-from datetime import date
-from typing import TYPE_CHECKING, Any, Union, cast
+from typing import Any, cast
 
 import pydantic
-import pydantic.schema
 from django.http import HttpResponse
 from django.urls.resolvers import RoutePattern, URLPattern, URLResolver
-from pydantic import BaseModel
-from pydantic.utils import get_model
+from pydantic_core import PydanticUndefined
 
-from .type_utils import (
-    get_inner_list_type,
-    is_optional,
-    is_pydantic_model,
-    is_union,
-    unwrap_optional,
-)
 from .types import ApiMeta
 
-if TYPE_CHECKING:
-    from pydantic.dataclasses import Dataclass
-
 logger = logging.getLogger(__name__)
 
 schema_ref = "#/components/schemas/{model}"
 
 
-def is_type_supported(t: type) -> bool:
-    """
-    Controls whether or not we support the provided type as request body or response
-    data.
-    """
-
-    try:
-        return is_pydantic_model(t)
-    except TypeError:
-        return False
-
-
-def name_for_type(t: type) -> str:
-    """
-    Returns OpenAPI schema for the provided type.
-    """
-
-    assert is_type_supported(t)
-
-    # normalize_name removes special characters like [] from generics.
-    # get_model gets the pydantic model, even if a pydantic dataclass is used.
-
-    return pydantic.schema.normalize_name(get_model(t).__name__)
-
-
-def schema_type_ref(t: type, *, is_list: bool = False) -> dict[str, Any]:
-    """
-    Returns a openapi reference to the provided type, and optionally wraps it in an
-    array
-    """
-
-    reference = {"$ref": schema_ref.format(model=name_for_type(t))}
-
-    if is_list:
-        return {
-            "type": "array",
-            "items": reference,
-        }
-
-    return reference
-
-
 def get_resolved_url_patterns(
     base_patterns: Sequence[URLResolver | URLPattern],
 ) -> list[tuple[URLPattern, str]]:
     """
     Given a list of base URL patterns, this function digs down into the URL hierarchy
     and evaluates the full URLs of all django views that have a simple path (e.g. no
     regex). Returns a list of tuples with each RoutePattern and its full URL.
@@ -140,201 +83,101 @@
     # Replaces e.g. "/x/<str:hello>/<int:hi>/" with "/x/{hello}/{hi}/" and also
     # populates the parameters variable.
     path = re.sub(r"<([a-zA-Z0-9_]+):([a-zA-Z0-9_]+)>", replacer, path)
 
     return path, parameters
 
 
-def get_schema_for_type_annotation(
-    input_type_annotation: type,
-) -> tuple[dict[str, Any] | None, list[type]]:
-    """
-    Helper function that generates a OpenAPI schema based on an input_type_annotation
-    Supports pydantic models directly, or with Union / list wrappers.
-    """
-
-    type_is_union = is_union(type_annotation=input_type_annotation)
-    if type_is_union:
-        type_annotations = typing.get_args(input_type_annotation)
-    else:
-        type_annotations = (input_type_annotation,)
-
-    # List of schemas we generate based on the return types (to support oneOf union
-    # types)
-    schemas = []
-    inner_type_annotations = []
-
-    for t in type_annotations:
-        type_annotation, type_is_list = get_inner_list_type(t)
-        if type_annotation is not None and is_type_supported(type_annotation):
-            schemas.append(schema_type_ref(type_annotation, is_list=type_is_list))
-            inner_type_annotations.append(type_annotation)
-        else:
-            # If one of the type's are not supported, skip the view
-            return None, []
-
-    if type_is_union and len(schemas) > 0:
-        return {"oneOf": schemas}, inner_type_annotations
-
-    if len(schemas) == 1:
-        return schemas[0], inner_type_annotations
-
-    return None, []
-
-
 def paths_and_types_for_view(
     *, view_name: str, callback: Callable[..., HttpResponse], resolved_url: str
-) -> tuple[dict[str, Any], list[type]]:
+) -> tuple[dict[str, Any], dict[str, Any]]:
     api_meta: ApiMeta | None = getattr(callback, "_api_meta", None)
 
     assert api_meta is not None
 
-    signature = inspect.signature(callback)
-
     # Types that should be included in the schema object (referenced via
     # schema_type_ref)
-    types: list[type] = []
-
-    schema, return_types = get_schema_for_type_annotation(signature.return_annotation)
+    components: dict[str, Any] = {}
 
-    if schema:
-        types += return_types
-        api_response = {"content": {"application/json": {"schema": schema}}}
+    def to_ref_if_object(schema: dict[str, Any]) -> dict[str, Any]:
+        if schema.get("type", None) == "object" and "title" in schema:
+            name = schema["title"]
+            ref = schema_ref.format(model=name)
+            components[name] = schema
+            return {"$ref": ref}
+
+        return schema
+
+    if api_meta.response_adapter:
+        response_schema = api_meta.response_adapter.json_schema(ref_template=schema_ref)
+        if defs := response_schema.pop("$defs", None):
+            components.update(defs)
+        response_schema = to_ref_if_object(response_schema)
+        api_response = {"content": {"application/json": {"schema": response_schema}}}
     else:
         api_response = {}
-        logger.debug(
-            "Return type of %s (%s) unsupported: %s",
-            resolved_url,
-            view_name,
-            signature.return_annotation,
-        )
 
-    additional_data = {}
+    request_body = {}
+    if api_meta.body_adapter:
+        body_schema = api_meta.body_adapter.json_schema(ref_template=schema_ref)
+        if defs := body_schema.pop("$defs", None):
+            components.update(defs)
 
-    if "body" in signature.parameters:
-        body_schema, body_return_types = get_schema_for_type_annotation(
-            signature.parameters["body"].annotation
-        )
-        if body_schema:
-            types += body_return_types
-            additional_data = {
-                "requestBody": {
-                    "required": True,
-                    "content": {"application/json": {"schema": body_schema}},
-                }
+        body_schema = to_ref_if_object(body_schema)
+
+        request_body = {
+            "requestBody": {
+                "required": True,
+                "content": {"application/json": {"schema": body_schema}},
             }
-        else:
-            logger.debug(
-                "Body type of %s (%s) unsupported: %s",
-                resolved_url,
-                view_name,
-                signature.parameters["body"].annotation,
-            )
+        }
 
-    path, url_parameters = django_path_to_openapi_url_and_parameters(resolved_url)
+    path, parameters = django_path_to_openapi_url_and_parameters(resolved_url)
 
-    query_parameters = openapi_query_parameters(
-        query_params=api_meta.query_params, signature=signature
-    )
+    for name, field in api_meta.query_params_model.model_fields.items():
+        schema = pydantic.TypeAdapter(field.annotation).json_schema(
+            ref_template=schema_ref
+        )
+        schema = to_ref_if_object(schema)
+
+        param = {
+            "name": field.alias or name,
+            "in": "query",
+            "required": field.is_required(),
+            "schema": schema,
+        }
+        if field.default != PydanticUndefined:
+            param["default"] = field.default
+        parameters.append(param)
 
     # Assuming standard django folder structure with [project name]/[app name]/....
     app_name = callback.__module__.split(".")[1]
 
     paths = {
         path: {
             api_meta.method.lower(): {
                 "operationId": view_name,
                 # Note: We could consider allowing users to pass a description into
                 # @api() instead of using the function docstring.
                 "description": callback.__doc__ or "",
                 # Tags are useful for grouping operations in codegen
                 "tags": [app_name],
-                "parameters": url_parameters + query_parameters,
-                **additional_data,
+                "parameters": parameters,
+                **request_body,
                 "responses": {
                     api_meta.response_status: {
                         "description": "",
                         **api_response,
                     }
                 },
             }
         }
     }
 
-    return paths, types
-
-
-def openapi_query_parameters(
-    *, query_params: list[str], signature: inspect.Signature
-) -> list[dict[str, Any]]:
-    """
-    Converts a function signature and a list of query params into openapi query
-    parameters.
-    """
-
-    parameters = []
-    for query_param in query_params:
-        query_url_name = query_param.replace("_", "-")
-
-        parameter = signature.parameters[query_param]
-
-        annotation = parameter.annotation
-        has_default = parameter.default != inspect.Parameter.empty
-
-        param_is_optional = is_optional(annotation)
-        if param_is_optional:
-            annotation = unwrap_optional(annotation)
-
-        schema = None
-
-        if annotation is str:
-            schema = {"type": "string"}
-
-        if annotation is int:
-            schema = {"type": "integer"}
-
-        if annotation is date:
-            schema = {"type": "string", "format": "date"}
-
-        if annotation is bool:
-            schema = {"type": "boolean"}
-
-        if schema is None:
-            logger.warning(
-                "Could not generate types for query param %s with type %s.",
-                query_url_name,
-                annotation,
-            )
-            continue
-
-        parameters.append(
-            {
-                "name": query_url_name,
-                "in": "query",
-                "required": not (param_is_optional or has_default),
-                "schema": schema,
-            }
-        )
-
-    return parameters
-
-
-def schemas_for_types(api_types: list[type]) -> dict[str, Any]:
-    # This only supports Pydantic models for now.
-    assert all(
-        hasattr(t, "__pydantic_model__") or issubclass(t, BaseModel) for t in api_types
-    )
-
-    return cast(
-        dict[str, Any],
-        pydantic.schema.schema(
-            cast(Sequence[Union[type[BaseModel], type["Dataclass"]]], api_types),
-            ref_template=schema_ref,
-        )["definitions"],
-    )
+    return paths, components
 
 
 def generate_api_spec(
     urlpatterns: Sequence[URLResolver | URLPattern],
 ) -> dict[str, Any]:
     """
     Entrypoint for generating an API spec. The function input is a list of URL patterns.
@@ -396,37 +239,37 @@
 
         else:
             logger.debug(
                 "Skipping view %s because it is not using @api decorator", pattern.name
             )
 
     api_paths: dict[str, Any] = {}
-    api_types = []
+    api_components = {}
 
     for operation in operations:
-        paths, types = paths_and_types_for_view(
+        paths, components = paths_and_types_for_view(
             view_name=operation.name,
             callback=operation.callback,
             resolved_url=operation.url,
         )
-        api_types += types
+        api_components.update(components)
 
         for path, val in paths.items():
             if path in api_paths:
                 # Merge operations that have the same URL but different http methods
                 api_paths[path].update(val)
             else:
                 api_paths[path] = val
 
-    api_schemas = schemas_for_types(api_types)
-
     api_spec = {
         "openapi": "3.0.0",
         "info": {"title": "API overview", "version": "0.0.1"},
         "paths": api_paths,
-        "components": {"schemas": api_schemas},
+        "components": {"schemas": api_components},
     }
 
-    logger.info("Generated %s paths and %s schemas", len(api_paths), len(api_schemas))
+    logger.info(
+        "Generated %s paths and %s schemas", len(api_paths), len(api_components)
+    )
     logger.info("%s @api annotated views", len(operations))
 
     return api_spec
```

### Comparing `django_api_decorator-0.1.7/django_api_decorator/schema_file.py` & `django_api_decorator-0.2.0a1/django_api_decorator/schema_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def get_api_spec() -> dict[str, Any]:
     if not hasattr(settings, "ROOT_URLCONF"):
         raise ValueError(
             "ROOT_URLCONF must be set in settings in order to generate an api spec."
         )
 
-    urlpatterns = import_module(settings.ROOT_URLCONF).urlpatterns  # type: ignore[misc]
+    urlpatterns = import_module(settings.ROOT_URLCONF).urlpatterns
 
     return generate_api_spec(urlpatterns=urlpatterns)
 
 
 def get_path() -> Path:
     if not hasattr(settings, "API_DECORATOR_SCHEMA_PATH"):
         raise ValueError(
```

### Comparing `django_api_decorator-0.1.7/django_api_decorator/types.py` & `django_api_decorator-0.2.0a1/django_api_decorator/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass
 from typing import Any, TypedDict
 
+from pydantic import BaseModel, TypeAdapter
+
 
 class FieldError(TypedDict):
     message: str
     code: str | None
 
 
 @dataclass
@@ -13,14 +15,17 @@
     Dataclass used on @api decorated views to preserve some information that cannot
     be inferred when inspecting the view.
     """
 
     method: str
     query_params: list[str]
     response_status: int
+    query_params_model: BaseModel
+    body_adapter: TypeAdapter[Any] | None
+    response_adapter: TypeAdapter[Any] | None
 
 
 class PublicAPIError(Exception):
     """
     Exception for public facing errors.
     Raises an ApiException in the frontend.
     """
```

### Comparing `django_api_decorator-0.1.7/django_api_decorator/utils.py` & `django_api_decorator-0.2.0a1/django_api_decorator/utils.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.1.7/pyproject.toml` & `django_api_decorator-0.2.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "django-api-decorator"
-version = "0.1.7"
+version = "0.2.0a1"
 description = "A collection of tools to build function based Django APIs"
 authors = ["Oda <tech@oda.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/django-api-decorator"
 repository = "https://github.com/kolonialno/django-api-decorator"
 packages = [{include = "django_api_decorator"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Django = ">=3"
-pydantic = "^1.10.2"
+pydantic = "^2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
```

### Comparing `django_api_decorator-0.1.7/PKG-INFO` & `django_api_decorator-0.2.0a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: django-api-decorator
-Version: 0.1.7
+Version: 0.2.0a1
 Summary: A collection of tools to build function based Django APIs
 Home-page: https://github.com/kolonialno/django-api-decorator
 License: MIT
 Author: Oda
 Author-email: tech@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=3)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/kolonialno/django-api-decorator
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   Django API Decorator
 </h1>
```

