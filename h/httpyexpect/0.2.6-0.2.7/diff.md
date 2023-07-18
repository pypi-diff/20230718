# Comparing `tmp/httpyexpect-0.2.6.tar.gz` & `tmp/httpyexpect-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpyexpect-0.2.6.tar", last modified: Tue Jun 13 11:06:33 2023, max compression
+gzip compressed data, was "httpyexpect-0.2.7.tar", last modified: Tue Jul 18 12:30:28 2023, max compression
```

## Comparing `httpyexpect-0.2.6.tar` & `httpyexpect-0.2.7.tar`

### file list

```diff
@@ -1,51 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.911759 httpyexpect-0.2.6/httpyexpect/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.911759 httpyexpect-0.2.6/httpyexpect/client/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/httpyexpect/server/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/httpyexpect/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/server/handlers/fastapi_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.911759 httpyexpect-0.2.6/httpyexpect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.911759 httpyexpect-0.2.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/test_fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_server_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.124498 httpyexpect-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-18 12:30:28.124498 httpyexpect-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.116498 httpyexpect-0.2.7/httpyexpect/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/httpyexpect/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/client/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/client/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/client/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/httpyexpect/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/httpyexpect/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/server/handlers/fastapi_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/httpyexpect/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.116498 httpyexpect-0.2.7/httpyexpect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-18 12:30:28.000000 httpyexpect-0.2.7/httpyexpect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-18 12:30:28.000000 httpyexpect-0.2.7/httpyexpect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:30:28.000000 httpyexpect-0.2.7/httpyexpect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:30:27.000000 httpyexpect-0.2.7/httpyexpect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 12:30:28.000000 httpyexpect-0.2.7/httpyexpect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 12:30:28.000000 httpyexpect-0.2.7/httpyexpect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/scripts/get_package_name.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/scripts/license_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/scripts/script_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/scripts/script_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/scripts/script_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/scripts/script_utils/fastapi_app_location.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4576 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/scripts/update_http_exception_schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/scripts/update_template_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-18 12:30:28.124498 httpyexpect-0.2.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.116498 httpyexpect-0.2.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/integration/test_fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:30:28.120498 httpyexpect-0.2.7/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/unit/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/unit/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/unit/test_server_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/unit/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-18 12:30:18.000000 httpyexpect-0.2.7/tests/unit/test_validation.py
```

### Comparing `httpyexpect-0.2.6/LICENSE` & `httpyexpect-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/PKG-INFO` & `httpyexpect-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpyexpect
-Version: 0.2.6
+Version: 0.2.7
 Summary: An opinionated way to translate server side HTTP errors to the client side.
 Home-page: https://github.com/ghga-de/httpyexpect
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `httpyexpect-0.2.6/README.md` & `httpyexpect-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect/__init__.py` & `httpyexpect-0.2.7/httpyexpect/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """An opinionated way to translate server side HTTP errors to the client side."""
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
```

### Comparing `httpyexpect-0.2.6/httpyexpect/base_exception.py` & `httpyexpect-0.2.7/httpyexpect/base_exception.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect/client/__init__.py` & `httpyexpect-0.2.7/httpyexpect/client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,9 +16,10 @@
 
 """A sub-package for translating server-side HTTP exceptions into client-side python
 exceptions.
 """
 
 
 # shortcuts:
+from httpyexpect.client.custom_types import Response  # noqa: F401
 from httpyexpect.client.mapping import ExceptionMapping  # noqa: F401
 from httpyexpect.client.translator import ResponseTranslator  # noqa: F401
```

### Comparing `httpyexpect-0.2.6/httpyexpect/client/custom_types.py` & `httpyexpect-0.2.7/httpyexpect/client/custom_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Custom types and type aliases."""
 
-from typing import Callable, Literal, Mapping
+from typing import Any, Callable, Literal, Mapping, Protocol
 
 ExceptionFactoryParam = Literal["status_code", "exception_id", "description", "data"]
 StatusCode = int
 ExceptionId = str
 ExceptionFactory = Callable[..., Exception]
 ExceptionMappingSpec = Mapping[StatusCode, object]
+
+
+class Response(Protocol):
+    """Any Response that is compatible with httpx and requests."""
+
+    status_code: int
+    """Status code of the Response"""
+
+    def json(self, **kwargs: Any) -> Any:
+        """JSON representation of the Response"""
+        ...
```

### Comparing `httpyexpect-0.2.6/httpyexpect/client/exceptions.py` & `httpyexpect-0.2.7/httpyexpect/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect/client/mapping.py` & `httpyexpect-0.2.7/httpyexpect/client/mapping.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect/client/translator.py` & `httpyexpect-0.2.7/httpyexpect/client/translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,54 +15,55 @@
 #
 
 """Logic to translate responses to HTTP calls to python exceptions."""
 
 from typing import Optional
 
 import pydantic
-import requests
 
+from httpyexpect.client.custom_types import Response
 from httpyexpect.client.exceptions import UnstructuredError
 from httpyexpect.client.mapping import ExceptionMapping
 from httpyexpect.models import HttpExceptionBody
 from httpyexpect.validation import ValidationError, assert_error_code
 
 
 class ResponseTranslator:
     """Translates a specific response to an HTTP call using an ExceptionMapping to
     python exceptions (in case of an error code)."""
 
-    def __init__(self, response: requests.Response, *, exception_map: ExceptionMapping):
+    def __init__(self, response: Response, *, exception_map: ExceptionMapping):
         """Initialize the translator.
 
         Args:
             response:
-                A response to an HTTP call performed with the `requests` library.
+                A response to an HTTP call performed e.g. with the `httpx` or `requests`
+                library.
             exception_map:
                 An exception mapping specifying translations between status codes plus
                 exception IDs and python exceptions.
         """
 
         self._exception_map = exception_map
         self._response = response
 
     @staticmethod
-    def _get_validated_exception_body(response: requests.Response) -> HttpExceptionBody:
+    def _get_validated_exception_body(response: Response) -> HttpExceptionBody:
         """Validates the response body against the HttpyExceptionBody model"""
         body = response.json()
         try:
             return HttpExceptionBody(**body)
         except pydantic.ValidationError as error:
             raise UnstructuredError(
                 status_code=response.status_code, body=body
             ) from error
 
     @classmethod
     def _construct_exception(
-        cls, response: requests.Response, exception_map: ExceptionMapping
+        cls, response: Response, exception_map: ExceptionMapping
     ) -> Exception:
         """Construct a python exception from a response."""
 
         # validate and parse the body of the exception response:
         body = cls._get_validated_exception_body(response)
 
         # get a factory kit that ships the exception factory together with instructions
```

### Comparing `httpyexpect-0.2.6/httpyexpect/models.py` & `httpyexpect-0.2.7/httpyexpect/models.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect/server/__init__.py` & `httpyexpect-0.2.7/httpyexpect/server/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect/server/exceptions.py` & `httpyexpect-0.2.7/httpyexpect/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect/server/handlers/__init__.py` & `httpyexpect-0.2.7/httpyexpect/server/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect/server/handlers/fastapi_.py` & `httpyexpect-0.2.7/httpyexpect/server/handlers/fastapi_.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect/validation.py` & `httpyexpect-0.2.7/httpyexpect/validation.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/httpyexpect.egg-info/PKG-INFO` & `httpyexpect-0.2.7/httpyexpect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpyexpect
-Version: 0.2.6
+Version: 0.2.7
 Summary: An opinionated way to translate server side HTTP errors to the client side.
 Home-page: https://github.com/ghga-de/httpyexpect
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `httpyexpect-0.2.6/httpyexpect.egg-info/SOURCES.txt` & `httpyexpect-0.2.7/httpyexpect.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 httpyexpect/client/exceptions.py
 httpyexpect/client/mapping.py
 httpyexpect/client/translator.py
 httpyexpect/server/__init__.py
 httpyexpect/server/exceptions.py
 httpyexpect/server/handlers/__init__.py
 httpyexpect/server/handlers/fastapi_.py
+scripts/__init__.py
+scripts/get_package_name.py
+scripts/license_checker.py
+scripts/update_http_exception_schema.py
+scripts/update_template_files.py
+scripts/script_utils/__init__.py
+scripts/script_utils/cli.py
+scripts/script_utils/fastapi_app_location.py
 tests/fixtures/__init__.py
 tests/fixtures/utils.py
 tests/integration/__init__.py
 tests/integration/test_client.py
 tests/integration/test_fastapi.py
 tests/integration/fixtures/__init__.py
 tests/integration/fixtures/utils.py
```

### Comparing `httpyexpect-0.2.6/setup.cfg` & `httpyexpect-0.2.7/setup.cfg`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 	License :: OSI Approved :: Apache Software License
 	Topic :: Internet :: WWW/HTTP :: HTTP Servers
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
-install_requires = 
 python_requires = >= 3.9
+install_requires = 
 
 [options.package_data]
 * = *.yaml, *.json, *.html
 
 [options.extras_require]
 fastapi = 
 	fastapi>=0.96.0
```

### Comparing `httpyexpect-0.2.6/setup.py` & `httpyexpect-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/fixtures/__init__.py` & `httpyexpect-0.2.7/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/fixtures/utils.py` & `httpyexpect-0.2.7/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/integration/__init__.py` & `httpyexpect-0.2.7/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/integration/fixtures/__init__.py` & `httpyexpect-0.2.7/tests/integration/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/integration/fixtures/utils.py` & `httpyexpect-0.2.7/tests/integration/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/integration/test_client.py` & `httpyexpect-0.2.7/tests/unit/test_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,86 +10,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""Client-side integration tests."""
+"""Test validation logic of pydantic models."""
 
-from unittest.mock import Mock
+from contextlib import nullcontext
 
 import pytest
+from pydantic import ValidationError
 
-from httpyexpect.client import ExceptionMapping, ResponseTranslator
 from httpyexpect.models import HttpExceptionBody
 
 
-class ExceptionA(RuntimeError):
-    """An Exception."""
-
-
-class ExceptionB(RuntimeError):
-    """Another Exception"""
-
-
-class ExceptionC(RuntimeError):
-    """Yet, another Exception"""
-
-
 @pytest.mark.parametrize(
-    "status_code, body, expected_exception",
+    "exception_id, description, data, is_valid",
     [
+        ("testException1", "My test description.", {"test": "test"}, True),
+        # Id starts with number:
+        ("1testException", "My test description.", {"test": "test"}, False),
+        # Id to short:
+        ("te", "My test description.", {"test": "test"}, False),
+        # Id uses non allowed characters:
+        ("teßtException", "My test description.", {"test": "test"}, False),
+        # Id is too long:
         (
-            400,
-            HttpExceptionBody(
-                exception_id="testA", description="test", data={"test": "test"}
-            ),
-            ExceptionA,
-        ),
-        (
-            400,
-            HttpExceptionBody(
-                exception_id="testB", description="test", data={"test": "test"}
-            ),
-            ExceptionB,
-        ),
-        (
-            500,
-            HttpExceptionBody(
-                exception_id="testC", description="test", data={"test": "test"}
-            ),
-            ExceptionC,
+            "TestExceptionWithABitMoreThan40Characters",
+            "My test description.",
+            {"test": "test"},
+            False,
         ),
+        # A string as data:
+        ("testException1", "My test description.", "test", False),
     ],
 )
-def test_typical_client_usage(
-    status_code: int, body: HttpExceptionBody, expected_exception: type[Exception]
+def test_http_exception_body(
+    exception_id: str, description: str, data: dict, is_valid: bool
 ):
-    """Test the typical way how the client may use the `ResponseTranslator` together
-    with the `ExceptionMapping` classes."""
-    spec = {
-        400: {
-            "testA": lambda exception_id, description, data: ExceptionA(),
-            "testB": lambda data: ExceptionB(),
-        },
-        500: {"testC": lambda: ExceptionC()},
-    }
-
-    # create http response mock:
-    response = Mock()
-    response.status_code = status_code
-    response.json.return_value = body.dict()
-
-    # create a exception mapping:
-    exception_map = ExceptionMapping(spec)
-
-    # initialize the ResponseTranslator:
-    translator = ResponseTranslator(response, exception_map=exception_map)
-
-    # translate and get the python exception object:
-    obtained_exception = translator.get_error()
-    assert isinstance(obtained_exception, expected_exception)
-
-    # translate into python exception and raise it:
-    with pytest.raises(expected_exception):
-        translator.raise_for_error()
+    """Test validation logic of the HTTPExceptionBody model."""
+
+    with nullcontext() if is_valid else pytest.raises(ValidationError):  # type: ignore
+        HttpExceptionBody(exception_id=exception_id, description=description, data=data)
```

### Comparing `httpyexpect-0.2.6/tests/integration/test_fastapi.py` & `httpyexpect-0.2.7/tests/integration/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/unit/__init__.py` & `httpyexpect-0.2.7/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/unit/fixtures/__init__.py` & `httpyexpect-0.2.7/tests/unit/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/unit/fixtures/utils.py` & `httpyexpect-0.2.7/tests/unit/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/unit/test_mapping.py` & `httpyexpect-0.2.7/tests/unit/test_mapping.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/unit/test_server_exceptions.py` & `httpyexpect-0.2.7/tests/unit/test_server_exceptions.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/unit/test_translator.py` & `httpyexpect-0.2.7/tests/unit/test_translator.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.6/tests/unit/test_validation.py` & `httpyexpect-0.2.7/tests/unit/test_validation.py`

 * *Files identical despite different names*

