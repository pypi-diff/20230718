# Comparing `tmp/spectree-1.1.5.tar.gz` & `tmp/spectree-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectree-1.1.5.tar", last modified: Mon Jul  3 11:49:39 2023, max compression
+gzip compressed data, was "spectree-1.2.0.tar", last modified: Tue Jul 18 02:33:59 2023, max compression
```

## Comparing `spectree-1.1.5.tar` & `spectree-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.403936 spectree-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-03 11:49:27.000000 spectree-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 11:49:27.000000 spectree-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-03 11:49:39.403936 spectree-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17910 2023-07-03 11:49:27.000000 spectree-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-03 11:49:27.000000 spectree-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:49:39.403936 spectree-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 11:49:27.000000 spectree-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.399936 spectree-1.1.5/spectree/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.403936 spectree-1.1.5/spectree/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/falcon_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/flask_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/quart_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/plugins/starlette_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-07-03 11:49:27.000000 spectree-1.1.5/spectree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.399936 spectree-1.1.5/spectree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 11:49:39.000000 spectree-1.1.5/spectree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:49:39.403936 spectree-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_falcon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_falcon_asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_flask_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_flask_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_quart.py
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_plugin_starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-03 11:49:27.000000 spectree-1.1.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:33:59.461594 spectree-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-18 02:33:48.000000 spectree-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 02:33:48.000000 spectree-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-07-18 02:33:59.461594 spectree-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17938 2023-07-18 02:33:48.000000 spectree-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-18 02:33:48.000000 spectree-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 02:33:59.461594 spectree-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-18 02:33:48.000000 spectree-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:33:59.457594 spectree-1.2.0/spectree/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:33:59.457594 spectree-1.2.0/spectree/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/plugins/falcon_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/plugins/flask_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/plugins/quart_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/plugins/starlette_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-18 02:33:48.000000 spectree-1.2.0/spectree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:33:59.457594 spectree-1.2.0/spectree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-07-18 02:33:59.000000 spectree-1.2.0/spectree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-18 02:33:59.000000 spectree-1.2.0/spectree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:33:59.000000 spectree-1.2.0/spectree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-18 02:33:59.000000 spectree-1.2.0/spectree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 02:33:59.000000 spectree-1.2.0/spectree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:33:59.461594 spectree-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_plugin_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_plugin_falcon_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_plugin_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_plugin_flask_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_plugin_flask_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_plugin_quart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_plugin_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-18 02:33:48.000000 spectree-1.2.0/tests/test_utils.py
```

### Comparing `spectree-1.1.5/LICENSE` & `spectree-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/PKG-INFO` & `spectree-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.5
+Version: 1.2.0
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
@@ -40,15 +40,15 @@
 
 Yet another library to generate OpenAPI documents and validate requests & responses with Python annotations.
 
 ## Features
 
 * Less boilerplate code, only annotations, no need for YAML :sparkles:
 * Generate API document with [Redoc UI](https://github.com/Redocly/redoc) or [Swagger UI](https://github.com/swagger-api/swagger-ui) :yum:
-* Validate query, JSON data, response data with [pydantic](https://github.com/samuelcolvin/pydantic/) :wink:
+* Validate query, JSON data, response data with [pydantic](https://github.com/samuelcolvin/pydantic/) :wink: (we support both v1 and v2)
 * Current support:
   * Flask [demo](#flask)
   * Quart [demo](#quart)
   * Falcon [demo](#falcon)
   * Starlette [demo](#starlette)
 
 ## Quick Start
```

### Comparing `spectree-1.1.5/README.md` & `spectree-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Yet another library to generate OpenAPI documents and validate requests & responses with Python annotations.
 
 ## Features
 
 * Less boilerplate code, only annotations, no need for YAML :sparkles:
 * Generate API document with [Redoc UI](https://github.com/Redocly/redoc) or [Swagger UI](https://github.com/swagger-api/swagger-ui) :yum:
-* Validate query, JSON data, response data with [pydantic](https://github.com/samuelcolvin/pydantic/) :wink:
+* Validate query, JSON data, response data with [pydantic](https://github.com/samuelcolvin/pydantic/) :wink: (we support both v1 and v2)
 * Current support:
   * Flask [demo](#flask)
   * Quart [demo](#quart)
   * Falcon [demo](#falcon)
   * Starlette [demo](#starlette)
 
 ## Quick Start
```

### Comparing `spectree-1.1.5/pyproject.toml` & `spectree-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spectree"
-version = "1.1.5"
+version = "1.2.0"
 dynamic = []
 description = "generate OpenAPI document and validate request&response with Python annotations."
 readme = "README.md"
 license = {text = "Apache-2.0"}
 requires-python = ">=3.8"
 authors = [
     { name = "Keming Yang", email = "kemingy94@gmail.com" },
@@ -18,30 +18,30 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "pydantic>=1.2,<2",
+    "pydantic>=1.2,<3",
 ]
 
 [project.optional-dependencies]
 dev = [
     "autoflake>=1.4,<3.0",
     "black>=22.3,<24.0",
     "flake8>=4,<7",
     "isort~=5.10",
     "mypy>=0.971",
     "pre-commit",
     "pytest~=7.1",
     "syrupy>=4.0",
 ]
 email = [
-    "pydantic[email]>=1.2,<2",
+    "pydantic[email]>=1.2,<3",
 ]
 falcon = [
     "falcon>=3.0.0",
 ]
 flask = [
     "flask",
 ]
```

### Comparing `spectree-1.1.5/setup.py` & `spectree-1.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 
 # this file is kept for GitHub's dependency graph
 
 setup(
     name="spectree",
     install_requires=[
-        "pydantic>=1.2,<2",
+        "pydantic>=1.2,<3",
     ],
     extras_require={
-        "email": ["pydantic[email]>=1.2,<2"],
+        "email": ["pydantic[email]>=1.2,<3"],
         "flask": ["flask"],
         "quart": ["quart"],
         "falcon": ["falcon>=3.0.0"],
         "starlette": ["starlette[full]"],
         "dev": [
             "pytest~=7.1",
             "flake8>=4,<7",
```

### Comparing `spectree-1.1.5/spectree/_types.py` & `spectree-1.2.0/spectree/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,18 @@
     Mapping,
     Optional,
     Sequence,
     Type,
     Union,
 )
 
-from pydantic import BaseModel
 from typing_extensions import Protocol
 
+from ._pydantic import BaseModel
+
 ModelType = Type[BaseModel]
 OptionalModelType = Optional[ModelType]
 NamingStrategy = Callable[[ModelType], str]
 NestedNamingStrategy = Callable[[str, str], str]
 
 
 class MultiDict(Protocol):
```

### Comparing `spectree-1.1.5/spectree/config.py` & `spectree-1.2.0/spectree/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import warnings
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Union
 
-from pydantic import AnyUrl, BaseModel, BaseSettings, EmailStr, root_validator
-
+from ._pydantic import AnyUrl, BaseModel, BaseSettings, EmailStr, root_validator
 from .models import SecurityScheme, Server
 from .page import DEFAULT_PAGE_TEMPLATES
 
 # Fall back to a str field if email-validator is not installed.
 if TYPE_CHECKING:
     EmailFieldType = str
 else:
```

### Comparing `spectree-1.1.5/spectree/models.py` & `spectree-1.2.0/spectree/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from enum import Enum
 from typing import Any, Dict, Optional, Sequence
 
-from pydantic import BaseModel, Field, root_validator, validator
+from ._pydantic import BaseModel, Field, root_validator, validator
 
 # OpenAPI names validation regexp
 OpenAPI_NAME_RE = re.compile(r"^[A-Za-z0-9-._]+")
 
 
 class ExternalDocs(BaseModel):
     description: str = ""
```

### Comparing `spectree-1.1.5/spectree/page.py` & `spectree-1.2.0/spectree/page.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/spectree/plugins/__init__.py` & `spectree-1.2.0/spectree/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/spectree/plugins/base.py` & `spectree-1.2.0/spectree/plugins/base.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/spectree/plugins/falcon_plugin.py` & `spectree-1.2.0/spectree/plugins/falcon_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 import re
 from functools import partial
 from typing import Any, Callable, Dict, List, Mapping, Optional, get_type_hints
 
 from falcon import HTTP_400, HTTP_415, HTTPError
 from falcon.routing.compiled import _FIELD_PATTERN as FALCON_FIELD_PATTERN
-from pydantic import ValidationError
 
+from .._pydantic import ValidationError
 from .._types import ModelType
 from ..response import Response
 from .base import BasePlugin
 
 
 class OpenAPI:
     def __init__(self, spec: Mapping[str, str]):
```

### Comparing `spectree-1.1.5/spectree/plugins/flask_plugin.py` & `spectree-1.2.0/spectree/plugins/flask_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Callable, Mapping, Optional, Tuple, get_type_hints
 
 from flask import Blueprint, abort, current_app, jsonify, make_response, request
-from pydantic import BaseModel, ValidationError
 from werkzeug.routing import parse_converter_args
 
+from .._pydantic import BaseModel, ValidationError
 from .._types import ModelType
 from ..response import Response
 from ..utils import get_multidict_items, werkzeug_parse_rule
 from .base import BasePlugin, Context
 
 
 class FlaskPlugin(BasePlugin):
```

### Comparing `spectree-1.1.5/spectree/plugins/quart_plugin.py` & `spectree-1.2.0/spectree/plugins/quart_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 from typing import Any, Callable, Mapping, Optional, Tuple, get_type_hints
 
-from pydantic import BaseModel, ValidationError
 from quart import Blueprint, abort, current_app, jsonify, make_response, request
 from werkzeug.routing import parse_converter_args
 
+from .._pydantic import BaseModel, ValidationError
 from .._types import ModelType
 from ..response import Response
 from ..utils import get_multidict_items, werkzeug_parse_rule
 from .base import BasePlugin, Context
 
 
 class QuartPlugin(BasePlugin):
```

### Comparing `spectree-1.1.5/spectree/plugins/starlette_plugin.py` & `spectree-1.2.0/spectree/plugins/starlette_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import inspect
 from collections import namedtuple
 from functools import partial
 from json import JSONDecodeError
 from typing import Any, Callable, Optional, get_type_hints
 
-from pydantic import ValidationError
 from starlette.convertors import CONVERTOR_TYPES
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, JSONResponse
 from starlette.routing import compile_path
 
+from .._pydantic import ValidationError
 from .._types import ModelType
 from ..response import Response
 from .base import BasePlugin, Context
 
 METHODS = {"get", "post", "put", "patch", "delete"}
 Route = namedtuple("Route", ["path", "methods", "func"])
```

### Comparing `spectree-1.1.5/spectree/response.py` & `spectree-1.2.0/spectree/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from http import HTTPStatus
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
-from pydantic import BaseModel
-
+from ._pydantic import BaseModel
 from ._types import ModelType, NamingStrategy, OptionalModelType
 from .utils import gen_list_model, get_model_key, parse_code
 
 # according to https://tools.ietf.org/html/rfc2616#section-10
 # https://tools.ietf.org/html/rfc7231#section-6.1
 # https://developer.mozilla.org/sv-SE/docs/Web/HTTP/Status
 DEFAULT_CODE_DESC: Dict[str, str] = dict(
```

### Comparing `spectree-1.1.5/spectree/spec.py` & `spectree-1.2.0/spectree/spec.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/spectree/utils.py` & `spectree-1.2.0/spectree/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
-from pydantic import BaseModel, ValidationError
-
+from ._pydantic import BaseModel, ValidationError
 from ._types import ModelType, MultiDict, NamingStrategy, NestedNamingStrategy
 
 # parse HTTP status code to get the code
 HTTP_CODE = re.compile(r"^HTTP_(?P<code>\d{3})$")
 
 RE_FLASK_RULE = re.compile(
     r"""
```

### Comparing `spectree-1.1.5/spectree.egg-info/PKG-INFO` & `spectree-1.2.0/spectree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectree
-Version: 1.1.5
+Version: 1.2.0
 Summary: generate OpenAPI document and validate request&response with Python annotations.
 Author-email: Keming Yang <kemingy94@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/0b01001001/spectree
 Project-URL: documentation, https://0b01001001.github.io/spectree/
 Project-URL: repository, https://github.com/0b01001001/spectree
 Project-URL: changelog, https://github.com/0b01001001/spectree/releases
@@ -40,15 +40,15 @@
 
 Yet another library to generate OpenAPI documents and validate requests & responses with Python annotations.
 
 ## Features
 
 * Less boilerplate code, only annotations, no need for YAML :sparkles:
 * Generate API document with [Redoc UI](https://github.com/Redocly/redoc) or [Swagger UI](https://github.com/swagger-api/swagger-ui) :yum:
-* Validate query, JSON data, response data with [pydantic](https://github.com/samuelcolvin/pydantic/) :wink:
+* Validate query, JSON data, response data with [pydantic](https://github.com/samuelcolvin/pydantic/) :wink: (we support both v1 and v2)
 * Current support:
   * Flask [demo](#flask)
   * Quart [demo](#quart)
   * Falcon [demo](#falcon)
   * Starlette [demo](#starlette)
 
 ## Quick Start
```

### Comparing `spectree-1.1.5/spectree.egg-info/SOURCES.txt` & `spectree-1.2.0/spectree.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 spectree/__init__.py
+spectree/_pydantic.py
 spectree/_types.py
 spectree/config.py
 spectree/models.py
 spectree/page.py
 spectree/py.typed
 spectree/response.py
 spectree/spec.py
```

### Comparing `spectree-1.1.5/tests/test_config.py` & `spectree-1.2.0/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import string
 from typing import Type
 
 import pytest
-from pydantic import ValidationError
 
 from spectree import SecurityScheme
+from spectree._pydantic import ValidationError
 from spectree.config import Configuration, EmailFieldType
 
 from .common import SECURITY_SCHEMAS, WRONG_SECURITY_SCHEMAS_DATA
 
 
 def test_config_license():
     config = Configuration(license={"name": "MIT"})
```

### Comparing `spectree-1.1.5/tests/test_plugin.py` & `spectree-1.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/tests/test_plugin_falcon.py` & `spectree-1.2.0/tests/test_plugin_falcon.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/tests/test_plugin_falcon_asgi.py` & `spectree-1.2.0/tests/test_plugin_falcon_asgi.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/tests/test_plugin_flask.py` & `spectree-1.2.0/tests/test_plugin_flask.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/tests/test_plugin_flask_blueprint.py` & `spectree-1.2.0/tests/test_plugin_flask_blueprint.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/tests/test_plugin_flask_view.py` & `spectree-1.2.0/tests/test_plugin_flask_view.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/tests/test_plugin_quart.py` & `spectree-1.2.0/tests/test_plugin_quart.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/tests/test_plugin_starlette.py` & `spectree-1.2.0/tests/test_plugin_starlette.py`

 * *Files identical despite different names*

### Comparing `spectree-1.1.5/tests/test_response.py` & `spectree-1.2.0/tests/test_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, get_type_hints
 
 import pytest
-from pydantic import BaseModel
 
+from spectree._pydantic import BaseModel
 from spectree.models import ValidationError
 from spectree.response import DEFAULT_CODE_DESC, Response
 from spectree.utils import gen_list_model
 
 from .common import JSON, DemoModel, get_model_path_key
```

### Comparing `spectree-1.1.5/tests/test_spec.py` & `spectree-1.2.0/tests/test_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from falcon import App as FalconApp
 from flask import Flask
-from pydantic import BaseModel
 from starlette.applications import Starlette
 
 from spectree import Response
+from spectree._pydantic import BaseModel
 from spectree.config import Configuration
 from spectree.models import Server, ValidationError
 from spectree.plugins.flask_plugin import FlaskPlugin
 from spectree.spec import SpecTree
 
 from .common import get_paths
```

### Comparing `spectree-1.1.5/tests/test_utils.py` & `spectree-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

