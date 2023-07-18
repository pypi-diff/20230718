# Comparing `tmp/json-any-2023.7.tar.gz` & `tmp/json-any-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-any-2023.7.tar", last modified: Mon Jul 17 09:52:06 2023, max compression
+gzip compressed data, was "json-any-2023.8.tar", last modified: Tue Jul 18 10:02:17 2023, max compression
```

## Comparing `json-any-2023.7.tar` & `json-any-2023.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.954990 json-any-2023.7/
--rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.7/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-17 09:52:06.954990 json-any-2023.7/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.7/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3458 2022-07-04 09:18:29.000000 json-any-2023.7/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.948323 json-any-2023.7/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.7/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/json_any/
--rw-r--r--   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2023.7/json_any/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/json_any/catalog/
--rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.7/json_any/catalog/module.py
--rw-r--r--   0 eric      (1000) users      (984)     4964 2023-07-13 14:00:49.000000 json-any-2023.7/json_any/catalog/type.py
--rw-r--r--   0 eric      (1000) users      (984)     1892 2023-07-13 12:46:11.000000 json-any-2023.7/json_any/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/json_any/extension/
--rw-r--r--   0 eric      (1000) users      (984)     2417 2023-07-13 15:36:06.000000 json-any-2023.7/json_any/extension/module.py
--rw-r--r--   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2023.7/json_any/extension/numpy.py
--rw-r--r--   0 eric      (1000) users      (984)     3671 2023-07-13 15:38:58.000000 json-any-2023.7/json_any/extension/type.py
--rw-r--r--   0 eric      (1000) users      (984)    11552 2023-07-13 14:17:27.000000 json-any-2023.7/json_any/json_to_object.py
--rw-r--r--   0 eric      (1000) users      (984)    12704 2023-07-13 15:16:14.000000 json-any-2023.7/json_any/object_to_json.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.954990 json-any-2023.7/json_any/task/
--rw-r--r--   0 eric      (1000) users      (984)     3348 2023-07-17 07:04:05.000000 json-any-2023.7/json_any/task/compression.py
--rw-r--r--   0 eric      (1000) users      (984)     8258 2023-07-17 09:48:29.000000 json-any-2023.7/json_any/task/storage.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-17 09:49:52.000000 json-any-2023.7/json_any/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-17 09:52:06.951656 json-any-2023.7/json_any.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4220 2023-07-17 09:52:06.000000 json-any-2023.7/json_any.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      544 2023-07-17 09:52:06.000000 json-any-2023.7/json_any.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-17 09:52:06.000000 json-any-2023.7/json_any.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-17 09:52:06.000000 json-any-2023.7/json_any.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.7/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-17 09:52:06.954990 json-any-2023.7/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5320 2023-07-13 15:24:10.000000 json-any-2023.7/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/
+-rw-r--r--   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2023.8/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4780 2023-07-18 10:02:17.239552 json-any-2023.8/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2023.8/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     4018 2023-07-17 12:03:11.000000 json-any-2023.8/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.236219 json-any-2023.8/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2023.8/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any/
+-rw-r--r--   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2023.8/json_any/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any/catalog/
+-rw-r--r--   0 eric      (1000) users      (984)     2192 2023-07-10 12:59:03.000000 json-any-2023.8/json_any/catalog/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     5042 2023-07-17 12:17:06.000000 json-any-2023.8/json_any/catalog/type.py
+-rw-r--r--   0 eric      (1000) users      (984)     1892 2023-07-13 12:46:11.000000 json-any-2023.8/json_any/constant.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any/extension/
+-rw-r--r--   0 eric      (1000) users      (984)     2417 2023-07-13 15:36:06.000000 json-any-2023.8/json_any/extension/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2023.8/json_any/extension/numpy.py
+-rw-r--r--   0 eric      (1000) users      (984)     3306 2023-07-18 09:13:52.000000 json-any-2023.8/json_any/extension/type.py
+-rw-r--r--   0 eric      (1000) users      (984)    11694 2023-07-18 09:14:44.000000 json-any-2023.8/json_any/json_to_object.py
+-rw-r--r--   0 eric      (1000) users      (984)    12906 2023-07-18 09:15:09.000000 json-any-2023.8/json_any/object_to_json.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any/task/
+-rw-r--r--   0 eric      (1000) users      (984)     3348 2023-07-17 07:04:05.000000 json-any-2023.8/json_any/task/compression.py
+-rw-r--r--   0 eric      (1000) users      (984)     8258 2023-07-17 09:48:29.000000 json-any-2023.8/json_any/task/storage.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-17 12:24:04.000000 json-any-2023.8/json_any/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-18 10:02:17.239552 json-any-2023.8/json_any.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4780 2023-07-18 10:02:17.000000 json-any-2023.8/json_any.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      544 2023-07-18 10:02:17.000000 json-any-2023.8/json_any.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-18 10:02:17.000000 json-any-2023.8/json_any.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        9 2023-07-18 10:02:17.000000 json-any-2023.8/json_any.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2023.8/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-18 10:02:17.239552 json-any-2023.8/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5320 2023-07-13 15:24:10.000000 json-any-2023.8/setup.py
```

### Comparing `json-any-2023.7/PKG-INFO` & `json-any-2023.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.7
+Version: 2023.8
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
@@ -70,22 +70,23 @@
 Installation
 ============
 
 This project is published
 on the `Python Package Index (PyPI) <https://pypi.org/>`_
 at: |PYPI_PROJECT_URL|_.
 It should be installable from Python distribution platforms or Integrated Development Environments (IDEs).
-Otherwise, it can be installed from a command console:
+Otherwise, it can be installed from a command console using `pip <https://pip.pypa.io/>`_:
 
-- For all users, after acquiring administrative rights:
-    - First installation: ``pip install`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --upgrade`` |PYPI_NAME_LITERAL|
-- For the current user (no administrative rights required):
-    - First installation: ``pip install --user`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+|              | For all users (after acquiring administrative rights) | For the current user (no administrative rights required) |
++==============+=======================================================+==========================================================+
+| Installation | ``pip install`` |PYPI_NAME_LITERAL|                   | ``pip install --user`` |PYPI_NAME_LITERAL|               |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+| Update       | ``pip install --upgrade`` |PYPI_NAME_LITERAL|         | ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|     |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
 
 
 
 Documentation
 =============
 
 The documentation is available at |DOCUMENTATION_URL|_.
```

### Comparing `json-any-2023.7/README-LICENCE-utf8.txt` & `json-any-2023.8/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/README.rst` & `json-any-2023.8/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -51,22 +51,23 @@
 Installation
 ============
 
 This project is published
 on the `Python Package Index (PyPI) <https://pypi.org/>`_
 at: |PYPI_PROJECT_URL|_.
 It should be installable from Python distribution platforms or Integrated Development Environments (IDEs).
-Otherwise, it can be installed from a command console:
+Otherwise, it can be installed from a command console using `pip <https://pip.pypa.io/>`_:
 
-- For all users, after acquiring administrative rights:
-    - First installation: ``pip install`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --upgrade`` |PYPI_NAME_LITERAL|
-- For the current user (no administrative rights required):
-    - First installation: ``pip install --user`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+|              | For all users (after acquiring administrative rights) | For the current user (no administrative rights required) |
++==============+=======================================================+==========================================================+
+| Installation | ``pip install`` |PYPI_NAME_LITERAL|                   | ``pip install --user`` |PYPI_NAME_LITERAL|               |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+| Update       | ``pip install --upgrade`` |PYPI_NAME_LITERAL|         | ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|     |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
 
 
 
 Documentation
 =============
 
 The documentation is available at |DOCUMENTATION_URL|_.
```

### Comparing `json-any-2023.7/documentation/wiki/description.asciidoc` & `json-any-2023.8/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/json_any/__init__.py` & `json-any-2023.8/json_any/__init__.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/json_any/catalog/module.py` & `json-any-2023.8/json_any/catalog/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/json_any/catalog/type.py` & `json-any-2023.8/json_any/catalog/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,19 @@
 from datetime import date as date_t
 from datetime import datetime as date_time_t
 from datetime import time as time_t
 from datetime import timedelta as time_delta_t
 from datetime import timezone as time_zone_t
 from enum import Enum as enum_t
 from io import BytesIO as io_bytes_t
+from io import StringIO as io_string_t
 from pathlib import PurePath as path_t
+from typing import Any
 from typing import NamedTuple as named_tuple_t
-from typing import Any, Sequence
+from typing import Sequence
 from uuid import UUID as uuid_t
 
 from json_any.catalog.module import grph, nmpy, pnds, pypl, sprs
 from json_any.constant import MODULE_TYPE_SEPARATOR
 
 BUILTIN_BYTES_CONTAINERS = (bytes, bytearray)
 BUILTIN_CONTAINERS = (frozenset, list, set, tuple)
@@ -88,14 +90,15 @@
 
 _AddJsonTypes(
     (
         date_t,
         date_time_t,
         enum_t,
         io_bytes_t,
+        io_string_t,
         named_tuple_t,
         py_array_t,
         time_delta_t,
         time_t,
         time_zone_t,
         uuid_t,
     )
```

### Comparing `json-any-2023.7/json_any/constant.py` & `json-any-2023.8/json_any/constant.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/json_any/extension/module.py` & `json-any-2023.8/json_any/extension/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/json_any/extension/numpy.py` & `json-any-2023.8/json_any/extension/numpy.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/json_any/extension/type.py` & `json-any-2023.8/json_any/extension/type.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,39 +26,36 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
-from types import GenericAlias
-from typing import Any, Callable, Union, get_origin
+from typing import Any, Callable, Union
 
-from json_any.catalog.type import enum_t
 from json_any.constant import MODULE_TYPE_SEPARATOR
 from json_any.extension.module import ElementInModule
 
 builders_h = dict[str, Callable[[Any], Any]]
 description_h = tuple[str, Any]
 descriptors_h = dict[str, Callable[[Any], Any]]
 
 
 class unfound_t:
     pass
 
 
 def QualifiedType(instance_or_type: Union[Any, type], /) -> str:
     """"""
-    # TODO: Explain why an enum_t instance must not be processed by TypeOfInstance.
-    if (type(instance_or_type) is type) or issubclass(instance_or_type, enum_t):
-        type_ = instance_or_type
+    if isinstance(instance_or_type, type):
+        instance_type = instance_or_type
     else:
-        type_ = TypeOfInstance(instance_or_type)
+        instance_type = type(instance_or_type)
 
-    return f"{type_.__module__}{MODULE_TYPE_SEPARATOR}{type_.__name__}"
+    return f"{instance_type.__module__}{MODULE_TYPE_SEPARATOR}{instance_type.__name__}"
 
 
 def TypeFromJsonType(
     json_type: str, /, *, prefix: str = "", should_continue_on_error: bool = False
 ) -> type:
     """"""
     module, type_ = json_type[prefix.__len__() :].split(
@@ -71,25 +68,17 @@
             output = unfound_t
         else:
             raise TypeError(error)
 
     return output
 
 
-def TypeOfInstance(instance: Any, /) -> type:
-    """"""
-    if isinstance(instance, GenericAlias):
-        return get_origin(type(instance))
-
-    return type(instance)
-
-
 def IsNamedTuple(instance: Any, /) -> bool:
     """"""
-    instance_type = TypeOfInstance(instance)
+    instance_type = type(instance)
     if hasattr(instance_type, "_make"):
         try:
             as_tuple = tuple(instance)
         except TypeError:
             return False
 
         return instance_type._make(as_tuple) == instance
```

### Comparing `json-any-2023.7/json_any/json_to_object.py` & `json-any-2023.8/json_any/json_to_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     ContainerWithName,
     TypeIsInModule,
     TypeNameOf,
     date_t,
     date_time_t,
     enum_t,
     io_bytes_t,
+    io_string_t,
     named_tuple_t,
     py_array_t,
     time_delta_t,
     time_t,
     time_zone_t,
     uuid_t,
 )
@@ -173,15 +174,17 @@
     elif json_type == JSON_TYPE[time_delta_t]:
         output = time_delta_t(*instance)
     elif json_type == JSON_TYPE[py_array_t]:
         as_list, typecode = instance
         output = py_array_t(typecode)
         output.fromlist(as_list)
     elif json_type == JSON_TYPE[io_bytes_t]:
-        output = io_bytes_t(instance.encode(encoding="iso-8859-1"))
+        output = io_bytes_t(initial_bytes=instance.encode(encoding="iso-8859-1"))
+    elif json_type == JSON_TYPE[io_string_t]:
+        output = io_string_t(initial_value=instance, newline="")
     elif json_type.startswith(JSON_TYPE_PREFIX_PATHLIB):
         type_name = json_type[JSON_TYPE_PREFIX_PATHLIB.__len__() :]
         output_t = getattr(pthl, type_name)
         output = output_t(instance)
     elif TypeIsInModule(json_type, sprs):
         type_name = TypeNameOf(json_type)
         output_t = getattr(sprs, type_name)
```

### Comparing `json-any-2023.7/json_any/object_to_json.py` & `json-any-2023.8/json_any/object_to_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     NUMPY_ARRAY_CLASSES,
     PANDAS_CLASSES,
     SCIPY_ARRAY_CLASSES,
     date_t,
     date_time_t,
     enum_t,
     io_bytes_t,
+    io_string_t,
     named_tuple_t,
     path_t,
     py_array_t,
     time_delta_t,
     time_t,
     time_zone_t,
     uuid_t,
@@ -70,15 +71,14 @@
     AsScalarRepresentation,
     IsNumpyScalar,
 )
 from json_any.extension.type import (
     IsFullyDataclassBased,
     IsNamedTuple,
     QualifiedType,
-    TypeOfInstance,
     description_h,
     descriptors_h,
 )
 
 _HISTORY_INDENTATION = 4 * " "
 
 
@@ -102,15 +102,15 @@
     history_level: str,
     /,
     *,
     highest_level_call: bool = False,
     descriptors: descriptors_h = None,
 ) -> description_h:
     """"""
-    instance_type = TypeOfInstance(instance)
+    instance_type = type(instance)
     json_type = JSON_TYPE.get(instance_type, None)
     qualified_type = QualifiedType(instance_type)
 
     if descriptors is None:
         descriptors = {}
     if qualified_type in descriptors:
         DescriptionForJSON = descriptors[qualified_type]
@@ -180,14 +180,18 @@
     elif instance_type is py_array_t:
         jsonable = (instance.tolist(), instance.typecode)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type is io_bytes_t:
         # Buffer is assumed to be open (i.e. no instance.closed check).
         jsonable = instance.getvalue().decode(encoding="iso-8859-1")
         history.append(f"{history_level}{json_type}:{jsonable}")
+    elif instance_type is io_string_t:
+        # Buffer is assumed to be open (i.e. no instance.closed check).
+        jsonable = instance.getvalue()
+        history.append(f"{history_level}{json_type}:{jsonable}")
     elif issubclass(instance_type, path_t):
         json_type = f"{JSON_TYPE_PREFIX_PATHLIB}{instance_type.__name__}"
         jsonable = str(instance)
         history.append(f"{history_level}{json_type}:{jsonable}")
     elif instance_type in SCIPY_ARRAY_CLASSES:
         jsonable = AsMostConciseRepresentation(instance.toarray())
         history.append(f"{history_level}{json_type}:{jsonable}")
```

### Comparing `json-any-2023.7/json_any/task/compression.py` & `json-any-2023.8/json_any/task/compression.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/json_any/task/storage.py` & `json-any-2023.8/json_any/task/storage.py`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/json_any/version.py` & `json-any-2023.8/json_any/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.7"
+__version__ = "2023.8"
```

### Comparing `json-any-2023.7/json_any.egg-info/PKG-INFO` & `json-any-2023.8/json_any.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2023.7
+Version: 2023.8
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
@@ -70,22 +70,23 @@
 Installation
 ============
 
 This project is published
 on the `Python Package Index (PyPI) <https://pypi.org/>`_
 at: |PYPI_PROJECT_URL|_.
 It should be installable from Python distribution platforms or Integrated Development Environments (IDEs).
-Otherwise, it can be installed from a command console:
+Otherwise, it can be installed from a command console using `pip <https://pip.pypa.io/>`_:
 
-- For all users, after acquiring administrative rights:
-    - First installation: ``pip install`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --upgrade`` |PYPI_NAME_LITERAL|
-- For the current user (no administrative rights required):
-    - First installation: ``pip install --user`` |PYPI_NAME_LITERAL|
-    - Installation update: ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+|              | For all users (after acquiring administrative rights) | For the current user (no administrative rights required) |
++==============+=======================================================+==========================================================+
+| Installation | ``pip install`` |PYPI_NAME_LITERAL|                   | ``pip install --user`` |PYPI_NAME_LITERAL|               |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
+| Update       | ``pip install --upgrade`` |PYPI_NAME_LITERAL|         | ``pip install --user --upgrade`` |PYPI_NAME_LITERAL|     |
++--------------+-------------------------------------------------------+----------------------------------------------------------+
 
 
 
 Documentation
 =============
 
 The documentation is available at |DOCUMENTATION_URL|_.
```

### Comparing `json-any-2023.7/json_any.egg-info/SOURCES.txt` & `json-any-2023.8/json_any.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-any-2023.7/setup.py` & `json-any-2023.8/setup.py`

 * *Files identical despite different names*

