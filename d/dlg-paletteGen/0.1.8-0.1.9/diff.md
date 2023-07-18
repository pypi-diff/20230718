# Comparing `tmp/dlg_paletteGen-0.1.8.tar.gz` & `tmp/dlg_paletteGen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlg_paletteGen-0.1.8.tar", last modified: Wed Feb  1 15:55:17 2023, max compression
+gzip compressed data, was "dlg_paletteGen-0.1.9.tar", last modified: Wed Jul  5 14:41:18 2023, max compression
```

## Comparing `dlg_paletteGen-0.1.8.tar` & `dlg_paletteGen-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:55:17.522805 dlg_paletteGen-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-02-01 15:55:17.518805 dlg_paletteGen-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:55:17.514804 dlg_paletteGen-0.1.8/dlg_paletteGen/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/dlg_paletteGen/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/dlg_paletteGen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/dlg_paletteGen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30783 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/dlg_paletteGen/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28476 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/dlg_paletteGen/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/dlg_paletteGen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/dlg_paletteGen/support_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:55:17.518805 dlg_paletteGen-0.1.8/dlg_paletteGen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-02-01 15:55:17.000000 dlg_paletteGen-0.1.8/dlg_paletteGen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-01 15:55:17.000000 dlg_paletteGen-0.1.8/dlg_paletteGen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 15:55:17.000000 dlg_paletteGen-0.1.8/dlg_paletteGen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-01 15:55:17.000000 dlg_paletteGen-0.1.8/dlg_paletteGen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-01 15:55:17.000000 dlg_paletteGen-0.1.8/dlg_paletteGen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-01 15:55:17.000000 dlg_paletteGen-0.1.8/dlg_paletteGen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 15:55:17.522805 dlg_paletteGen-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:55:17.518805 dlg_paletteGen-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:55:17.518805 dlg_paletteGen-0.1.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/tests/data/example_casatask.py
--rw-r--r--   0 runner    (1001) docker     (123)    38718 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/tests/data/example_eagle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/tests/data/example_google.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/tests/data/example_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/tests/data/example_rascil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/tests/data/example_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-02-01 15:55:05.000000 dlg_paletteGen-0.1.8/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:18.141582 dlg_paletteGen-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-05 14:41:18.141582 dlg_paletteGen-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:18.137581 dlg_paletteGen-0.1.9/dlg_paletteGen/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/dlg_paletteGen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/dlg_paletteGen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/dlg_paletteGen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36129 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/dlg_paletteGen/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/dlg_paletteGen/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/dlg_paletteGen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/dlg_paletteGen/support_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:18.137581 dlg_paletteGen-0.1.9/dlg_paletteGen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-05 14:41:18.000000 dlg_paletteGen-0.1.9/dlg_paletteGen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-05 14:41:18.000000 dlg_paletteGen-0.1.9/dlg_paletteGen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:41:18.000000 dlg_paletteGen-0.1.9/dlg_paletteGen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-05 14:41:18.000000 dlg_paletteGen-0.1.9/dlg_paletteGen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 14:41:18.000000 dlg_paletteGen-0.1.9/dlg_paletteGen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 14:41:18.000000 dlg_paletteGen-0.1.9/dlg_paletteGen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:41:18.141582 dlg_paletteGen-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:18.141582 dlg_paletteGen-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:41:18.141582 dlg_paletteGen-0.1.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/data/example_casatask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38718 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/data/example_eagle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/data/example_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/data/example_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/data/example_rascil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/data/example_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/data/hifa_importdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-05 14:41:06.000000 dlg_paletteGen-0.1.9/tests/test_base.py
```

### Comparing `dlg_paletteGen-0.1.8/HISTORY.md` & `dlg_paletteGen-0.1.9/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Added tag filter. [Andreas Wicenec]
+- Ignore .vscode dir. [Andreas Wicenec]
+- Ignore .vscode. [Andreas Wicenec]
+- Added support for constructParam. [Andreas Wicenec]
+- Refactored Field into dataclass. [Andreas Wicenec]
+- Added recursion into sub-modules. [Andreas Wicenec]
+- Initial support for module parsing. [Andreas Wicenec]
+- Release: version 0.1.8 🚀 [Andreas Wicenec]
+- Doc updates. [Andreas Wicenec]
+- Release: version 0.1.8 🚀 [Andreas Wicenec]
+- More documentation. [Andreas Wicenec]
+
+
+0.1.8 (2023-02-01)
+------------------
+- Release: version 0.1.8 🚀 [Andreas Wicenec]
 - Release: version 0.1.7 🚀 [Andreas Wicenec]
 - Fixed inconsistency between black and isort. [Andreas Wicenec]
 - Release: version 0.1.7 🚀 [Andreas Wicenec]
 - Updated links. [Andreas Wicenec]
 - Release: version 0.1.7 🚀 [Andreas Wicenec]
 - Release: version 0.1.7 🚀 [Andreas Wicenec]
```

### Comparing `dlg_paletteGen-0.1.8/LICENSE` & `dlg_paletteGen-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.1.8/PKG-INFO` & `dlg_paletteGen-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlg_paletteGen
-Version: 0.1.8
+Version: 0.1.9
 Summary: DALiuGE palette generator tool
 Home-page: https://github.com/ICRAR/dlg_paletteGen/
 Author: ICRAR
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 [![codecov](https://codecov.io/gh/ICRAR/dlg_paletteGen/branch/main/graph/badge.svg?token=dlg_paletteGen_token_here)](https://codecov.io/gh/ICRAR/dlg_paletteGen)
 [![CI](https://github.com/ICRAR/dlg_paletteGen/actions/workflows/main.yml/badge.svg)](https://github.com/ICRAR/dlg_paletteGen/actions/workflows/main.yml)
 
 This is the palette generator of the [DALiuGE](https://daliuge.readthedocs.io) system.
 
 It processes a file or a directory of source files and
 produces a DALiuGE compatible palette file containing the
-information required to use the identified functions and classes and methods to construct logical graphs in [EAGLE](https://eagle-dlg.readthedocs.io).
+information required to use the identified functions and classes and methods to construct computational workflows in [EAGLE](https://eagle-dlg.readthedocs.io).
 For more information please refer to the [documentation](https://icrar.github.io/dlg_paletteGen/).
 
 ## Install it from PyPI
 
 ```bash
 pip install dlg_paletteGen
 ```
@@ -41,15 +41,15 @@
 
 usage: dlg_paletteGen [-h] [-m MODULE] [-t TAG] [-c] [-r] [-s] [-v] idir ofile
 
 This is the palette generator of the DALiuGE system.
 
 It processes a file or a directory of source files and
 produces a DALiuGE compatible palette file containing the
-information required to use functions and components in graphs.
+information required to use functions and components in workflows.
 For more information please refer to the documentation
 https://daliuge.readthedocs.io/en/latest/development/app_development/eagle_app_integration.html#automatic-eagle-palette-generation
 
 positional arguments:
   idir                  input directory path or file name
   ofile                 output file name
```

### Comparing `dlg_paletteGen-0.1.8/README.md` & `dlg_paletteGen-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![codecov](https://codecov.io/gh/ICRAR/dlg_paletteGen/branch/main/graph/badge.svg?token=dlg_paletteGen_token_here)](https://codecov.io/gh/ICRAR/dlg_paletteGen)
 [![CI](https://github.com/ICRAR/dlg_paletteGen/actions/workflows/main.yml/badge.svg)](https://github.com/ICRAR/dlg_paletteGen/actions/workflows/main.yml)
 
 This is the palette generator of the [DALiuGE](https://daliuge.readthedocs.io) system.
 
 It processes a file or a directory of source files and
 produces a DALiuGE compatible palette file containing the
-information required to use the identified functions and classes and methods to construct logical graphs in [EAGLE](https://eagle-dlg.readthedocs.io).
+information required to use the identified functions and classes and methods to construct computational workflows in [EAGLE](https://eagle-dlg.readthedocs.io).
 For more information please refer to the [documentation](https://icrar.github.io/dlg_paletteGen/).
 
 ## Install it from PyPI
 
 ```bash
 pip install dlg_paletteGen
 ```
@@ -32,15 +32,15 @@
 
 usage: dlg_paletteGen [-h] [-m MODULE] [-t TAG] [-c] [-r] [-s] [-v] idir ofile
 
 This is the palette generator of the DALiuGE system.
 
 It processes a file or a directory of source files and
 produces a DALiuGE compatible palette file containing the
-information required to use functions and components in graphs.
+information required to use functions and components in workflows.
 For more information please refer to the documentation
 https://daliuge.readthedocs.io/en/latest/development/app_development/eagle_app_integration.html#automatic-eagle-palette-generation
 
 positional arguments:
   idir                  input directory path or file name
   ofile                 output file name
```

### Comparing `dlg_paletteGen-0.1.8/dlg_paletteGen/base.py` & `dlg_paletteGen-0.1.9/dlg_paletteGen/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 
 TODO: This whole tool needs re-factoring into separate class files
 (compound, child, grandchild, grandgrandchild, node, param, pluggable parsers)
 Should also be made separate sub-repo with proper installation and entry point.
 
 """
 import csv
+import importlib
 import json
 import os
+import sys
+import types
 import xml.etree.ElementTree as ET
-from typing import Any, Union
+from typing import Any, Union, _SpecialForm
 
 from blockdag import build_block_dag
 
-from dlg_paletteGen.classes import Child
+from dlg_paletteGen.classes import Child, DetailedDescription, Field
 from dlg_paletteGen.support_functions import (
     Language,
     check_text_element,
     create_uuid,
     get_next_key,
+    get_submodules,
     logger,
 )
 
 KNOWN_PARAM_DATA_TYPES = [
     "String",
     "Integer",
     "Float",
@@ -47,18 +51,21 @@
     "ParameterSet",
     "EnvironmentVariables",
 ]
 
 KNOWN_FIELD_TYPES = [
     "ComponentParameter",
     "ApplicationArgument",
+    "ConstructParameter",
     "InputPort",
     "OutputPort",
 ]
 
+KNOWN_USAGE_TYPES = ["NoPort", "InputPort", "OutputPort", "InputOutput"]
+
 BLOCKDAG_DATA_FIELDS = [
     "inputPorts",
     "outputPorts",
     "applicationArgs",
     "category",
     "fields",
 ]
@@ -201,52 +208,56 @@
 
 def create_field(
     internal_name: str,
     external_name: str,
     value: str,
     value_type: str,
     field_type: str,
-    access: str,
-    options: str,
-    precious: bool,
-    positional: bool,
-    description: str,
+    usage: str,
+    access: str = "readonly",
+    options: str = "",
+    precious: bool = False,
+    positional: bool = False,
+    description: str = "",
 ):
     """
-    TODO: field should be a dataclass
-    For now just create a dict using the values provided
+    This function creates a new Field object and returns its associated
+    dictionary
 
     :param internal_name: str, the internal name of the parameter
     :param external_name: str, the visible name of the parameter
     :param value: str, the value of the parameter
     :param value_type: str, the type of the value
     :param field_type: str, the type of the field
+    :param usage: str, the usage for this field (NoPort, InputPort, OutputPort,
+    InputOutput)
     :param access: str, readwrite|readonly (default readonly)
     :param options: str, options
     :param precious: bool,
         should this parameter appear, even if empty or None
     :param positional: bool,
         is this a positional parameter
     :param description: str, the description used in the palette
 
     :returns field: dict
     """
-    return {
-        "text": external_name,
-        "name": internal_name,
-        "value": value,
-        "defaultValue": value,
-        "description": description,
-        "type": value_type,
-        "fieldType": field_type,
-        "readonly": access == "readonly",
-        "options": options,
-        "precious": precious,
-        "positional": positional,
-    }
+    field = Field(
+        internal_name,
+        external_name,
+        value,
+        value_type,
+        field_type,
+        usage,
+        access,
+        options,
+        precious,
+        positional,
+        description,
+    )
+    return field.to_dict()
 
 
 def alert_if_missing(message: str, fields: list, internal_name: str):
     """
     Produce a warning message using `text` if a field with `internal_name`
     does not exist.
 
@@ -278,31 +289,55 @@
         parts = row
 
     # init attributes of the param
     external_name = ""
     default_value = ""
     value_type = "String"
     field_type = "cparam"
+    usage = "NoPort"
     access = "readwrite"
     options: list = []
     precious = False
     positional = False
     description = ""
 
     # assign attributes (if present)
     if len(parts) > 0:
-        external_name = parts[0]
+        external_name = parts[0].strip()
     if len(parts) > 1:
-        default_value = parts[1]
+        default_value = parts[1].strip()
     if len(parts) > 2:
-        value_type = parts[2]
+        value_type = parts[2].strip()
     if len(parts) > 3:
-        field_type = parts[3]
+        field_type = parts[3].strip()
+        if field_type.count(",") > 0:
+            field_type, usage = parts[3].strip().split(",", 1)
+        field_type = field_type.strip()
+        usage = usage.strip()
+        if field_type not in KNOWN_FIELD_TYPES:
+            logger.warning(
+                message
+                + " "
+                + external_name
+                + " field_type '%s' unknown "
+                + "using ComponentParameter!",
+                field_type,
+            )
+        if usage not in KNOWN_USAGE_TYPES:
+            logger.warning(
+                message
+                + " "
+                + external_name
+                + " %s usage '%s' unknown "
+                + "using NoPort!",
+                field_type,
+                usage,
+            )
     if len(parts) > 4:
-        access = parts[4]
+        access = parts[4].strip()
     else:
         logger.warning(
             message
             + " "
             + field_type
             + " ("
             + external_name
@@ -352,14 +387,15 @@
         description = parts[8]
 
     return (
         external_name,
         default_value,
         value_type,
         field_type,
+        usage,
         access,
         options,
         precious,
         positional,
         description,
     )
 
@@ -385,17 +421,18 @@
     tag = ""
     construct = ""
     inputPorts: list = []
     outputPorts: list = []
     inputLocalPorts: list = []
     outputLocalPorts: list = []
     fields: list = []
+    construct_fields = []
     applicationArgs: list = []
 
-    # process the params
+    # process the params into fields for the palette
     for param in params:
         if not isinstance(param, dict):
             logger.error(
                 "param %s has wrong type %s. Ignoring!", param, type(param)
             )
             continue
         key = param["key"]
@@ -415,14 +452,15 @@
         else:
             internal_name = key
             (
                 external_name,
                 default_value,
                 value_type,
                 field_type,
+                usage,
                 access,
                 options,
                 precious,
                 positional,
                 description,
             ) = parse_value(text, value)
 
@@ -482,25 +520,29 @@
             # create a field from this data
             field = create_field(
                 internal_name,
                 external_name,
                 default_value,
                 value_type,
                 field_type,
+                usage,
                 access,
                 options,
                 precious,
                 positional,
                 description,
             )
 
             # add the field to the correct list in the component, based on
             # fieldType
             if field_type in KNOWN_FIELD_TYPES:
-                fields.append(field)
+                if field_type == "ConstructParameter":
+                    construct_fields.append(field)
+                else:
+                    fields.append(field)
             else:
                 logger.warning(
                     text
                     + " '"
                     + external_name
                     + "' field_type is Unknown: "
                     + field_type
@@ -532,14 +574,15 @@
             "inputPorts": inputPorts,
             "outputPorts": outputPorts,
             "inputLocalPorts": inputLocalPorts,
             "outputLocalPorts": outputLocalPorts,
             "inputAppFields": [],
             "outputAppFields": [],
             "fields": fields,
+            "constructFields": construct_fields,
             "applicationArgs": applicationArgs,
             "repositoryUrl": GITREPO,
             "commitHash": VERSION,
             "paletteDownloadUrl": "",
             "dataHash": "",
         },
     )
@@ -581,23 +624,25 @@
         json.dump(palette, outfile, indent=4)
 
 
 def process_compounddefs(
     output_xml_filename: str,
     allow_missing_eagle_start: bool = True,
     language: Language = Language.PYTHON,
+    tag: str = "",
 ) -> list:
     """
     Extract and process the compounddef elements.
 
     :param output_xml_filename: str, File name for the XML file produced by
         doxygen
     :param allow_missing_eagle_start: bool, Treat non-daliuge tagged classes
         and functions
     :param language: Language, can be [2] for Python, 1 for C or 0 for Unknown
+    :param tag: The filter tag to be used for EAGLE components
 
     :returns nodes
     """
     # load and parse the input xml file
     tree = ET.parse(output_xml_filename)
 
     xml_root = tree.getroot()
@@ -621,15 +666,15 @@
         if kind not in ["class", "namespace"]:
             # we'll ignore this compound
             continue
 
         if is_eagle_node:
             params = process_compounddef_eagle(compounddef)
 
-            ns = params_to_nodes(params)
+            ns = params_to_nodes(params, tag=tag)
             nodes.extend(ns)
 
         if not is_eagle_node and allow_missing_eagle_start:  # not eagle node
             logger.info("Handling compound: %s", compoundname)
             # ET.tostring(compounddef, encoding="unicode"),
             # )
             functions = process_compounddef_default(compounddef, language)
@@ -656,14 +701,15 @@
 
                     if alreadyPresent:
                         # TODO: Originally this was suppressed, but in reality
                         # multiple functions with the same name are possible
                         logger.warning(
                             "Function has multiple entires: %s", n["text"]
                         )
+                        n["text"] = f"{compoundname}.{n['text']}"
                     nodes.append(n)
         if not is_eagle_node and not allow_missing_eagle_start:
             logger.warning(
                 "None EAGLE tagged component '%s' identified. "
                 + "Not parsing it due to setting. "
                 + "Consider using the -s flag.",
                 compoundname,
@@ -890,14 +936,15 @@
         "paletteDownloadUrl": "",
         "dataHash": "",
         "key": get_next_key(),
         "text": node_type + "/" + node["text"],
     }
 
     if node_type in ["Scatter", "Gather", "MKN"]:
+        construct_node["fields"] = node["constructFields"]
         construct_node["inputAppFields"] = node["fields"]
         construct_node["inputAppArgs"] = node["applicationArgs"]
         construct_node["inputApplicationKey"] = node["key"]
         construct_node["inputApplicationName"] = node["text"]
         construct_node["inputApplicationType"] = node["category"]
         construct_node["inputApplicationDescription"] = node["description"]
         construct_node["inputLocalPorts"] = node["outputPorts"]
@@ -912,25 +959,25 @@
         construct_node["outputPorts"] = []
     else:
         pass  # not sure what to do for branch
 
     return construct_node
 
 
-def params_to_nodes(params: list) -> list:
+def params_to_nodes(params: list, tag: str = "") -> list:
     """
     Generate a list of nodes from the params found
 
     :param params: list, the parameters to be converted
+    :param tag: The filter taf to be used
 
     :returns list of node dictionaries
     """
     # logger.debug("params_to_nodes: %s", params)
     result = []
-    tag = ""
     gitrepo = ""
     version = "0.1"
 
     # if no params were found, or only the name and description were found,
     # then don't bother creating a node
     if len(params) > 2:
         # create a node
@@ -954,23 +1001,26 @@
         if data["tag"] == tag or tag == "":  # type: ignore
             logger.debug("Adding component: " + node["text"])
             result.append(node)
 
             # if a construct is found, add to nodes
             if data["construct"] != "":
                 logger.info(
-                    "Adding component: "
+                    "Adding construct component: "
                     + data["construct"]
                     + "/"
                     + node["text"]
                 )
                 construct_node = create_construct_node(data["construct"], node)
                 construct_node["repositoryUrl"] = gitrepo
                 construct_node["commitHash"] = version
                 result.append(construct_node)
+            # have to get rid of them for the non-construct nodes
+            if "constructFields" in node:
+                del node["constructFields"]
 
     return result
 
 
 def prepare_and_write_palette(nodes: list, outputfile: str):
     """
     Prepare and write the palette in JSON format.
@@ -988,7 +1038,104 @@
     block_dag = build_block_dag(vertices, [], data_fields=BLOCKDAG_DATA_FIELDS)
 
     # write the output json file
     write_palette_json(
         outputfile, nodes, GITREPO, VERSION, block_dag  # type: ignore
     )
     logger.info("Wrote " + str(len(nodes)) + " component(s)")
+
+
+def module_get(mod: types.ModuleType):
+    """ """
+    logger.debug(f">>>>>>>>> Processing members for module: {mod.__name__}")
+    content = dir(mod)
+    count = 0
+    # logger.info("Content of %s: %s", mod, content)
+    name = mod.__name__
+    members = []
+    for c in content:
+        if c[0] == "_":
+            # TODO: Deal with __init__
+            # NOTE: PyBind11 classes can have multiple constructors
+            continue
+        m = getattr(mod, c)
+        if not callable(m) or isinstance(m, _SpecialForm):
+            logger.warning("Member %s is not callable", m)
+            # TODO: not sure what to do with these. Usually they
+            # are class parameters.
+            continue
+        else:
+            count += 1
+            name = (
+                f"{mod.__name__}.{m.__name__}"
+                if hasattr(m, "__name__")
+                else f"{mod.__name__}.Unknown"
+            )
+            members.append(name)
+            if m.__doc__ and len(m.__doc__) > 0:
+                dd = DetailedDescription(m.__doc__)
+                logger.debug(f">>> Processing member {name}")
+                logger.debug(f"Brief description: {dd.brief_descr}")
+                if len(dd.params) > 0:
+                    logger.debug("Parameters: %s", dd.params)
+            elif hasattr(m, "__name__"):
+                logger.warning("Member '%s' has no description!", name)
+            else:
+                logger.warning(
+                    "Entity '%s' has neither descr. nor __name__", m
+                )
+
+            if hasattr(m, "__members__"):
+                # this takes care of enum types, but needs some
+                # serious thinking for DALiuGE. Note that enums
+                # from PyBind11 have a generic type, but still
+                # the __members__ dict.
+                # print("\nMembers:")
+                # print(m.__members__)
+                pass
+    logger.info("Module %s has %d members", name, count)
+    return members
+
+
+def module_hook(
+    mod_name: str, modules: dict = {}, recursive: bool = True
+) -> "tuple[dict, int]":
+    """
+    This is the starting point of a function dissecting the
+    docs for an imported module.
+
+    TODO: Generate palette from description and params.
+    TODO: At some point this might be the main entry point for
+    the whole parsing, but means that the module has to be installed.
+
+    :param mod_name: str, the name of the module to be treated
+    :param recursive: bool, treat sub-modules [True]
+
+    :returns: Number of modules processed
+    """
+    member_count = 0
+    mod_count = 0
+    if mod_name not in sys.builtin_module_names:
+        try:
+            mod = importlib.import_module(mod_name)
+        except ImportError:
+            logger.error("Module %s can't be loaded!", mod_name)
+            raise
+    modules.update({mod_name: module_get(mod)})
+    mod_count += 1
+    if recursive:
+        sub_modules = get_submodules(mod)
+        sub_mods = [
+            x[1]
+            for x in sub_modules
+            if (x[1][0] != "_" and x[1][:4] != "test")
+        ]  # get the names; ignore test modules
+        if len(sub_mods) > 0:
+            logger.debug("sub_modules of %s: %s", mod_name, sub_mods)
+        for sub_mod in sub_mods:
+            mod_load = f"{mod_name}.{sub_mod}"
+            # modules.update({mod_load: {}})
+            modules, mod_count = module_hook(mod_load, modules=modules)
+            mod_count += len(modules)
+    member_count = sum([len(m) for m in modules])
+    logger.info("%d, %d", len(modules), member_count)
+    return modules, mod_count
```

### Comparing `dlg_paletteGen-0.1.8/dlg_paletteGen/classes.py` & `dlg_paletteGen-0.1.9/dlg_paletteGen/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import xml.etree.ElementTree as ET
+from dataclasses import dataclass
 from typing import Union
 
 from dlg_paletteGen.support_functions import (
     VALUE_TYPES,
     Language,
     cleanString,
     logger,
@@ -15,28 +16,29 @@
     """
     Class performs parsing of detailed description elements.
     This class is used for both compound (e.g. class) level descriptions
     as well as function/method level.
     """
 
     KNOWN_FORMATS = {
-        "rEST": r"\n(:param|:returns|Returns:) .*",
-        "Google": r"\nArgs:",
-        "Numpy": r"\nParameters\n----------",
+        "rEST": r"\n\s*(:param|:returns|Returns:) .*",
+        "Google": r"\n\s*Args:",
+        "Numpy": r"\n\s*Parameters\s*\n\s*----------",
         "casa": r"\n-{2,20}? parameter",
     }
 
     def __init__(self, descr: str):
         """
         :param descr: Text of the detaileddescription node
         """
         self.description = descr
         self.format = ""
         self._identify_format()
         self.main_descr, self.params = self.process_descr()
+        self.brief_descr = self.main_descr.split(".")[0] + "."
 
     def _process_rEST(self, detailed_description) -> tuple:
         """
         Parse parameter descirptions found in a detailed_description tag. This
         assumes rEST style documentation.
 
         :param detailed_description: str, the content of the description XML
@@ -141,18 +143,22 @@
 
         :param dd: str, the content of the detailed description tag
 
         :returns: tuple, description and parameter dictionary
         """
         logger.debug("Processing Numpy style doc_strings")
         ds = "\n".join(
-            [d.strip() for d in dd.split("\n")]
+            [d.strip() for d in dd.split(r"\s*\n")]
         )  # remove whitespace from lines
         # extract main documentation (up to Parameters line)
-        (description, rest) = ds.split("\nParameters\n----------\n")
+        try:
+            (description, rest) = re.split(self.KNOWN_FORMATS["Numpy"], ds)
+        except ValueError:
+            logger.debug("Problem parsing NumPy format")
+            return (ds, {})
         # extract parameter documentation (up to Returns line)
         pds = rest.split(r"\nReturns\n-------\n")
         spds = re.split(r"([\w_]+) :", pds[0])[1:]  # split :param lines
         pdict = dict(zip(spds[::2], spds[1::2]))  # create initial param dict
         pdict = {
             k: {
                 "desc": v.replace("\n", " "),
@@ -180,15 +186,15 @@
             [d.strip() for d in dd.split("\n")]
         )  # remove whitespace from lines
         # extract main documentation (up to Parameters line)
         (description, rest) = ds.split("\nArgs:")
         # logger.debug("Splitting: %s %s", description, rest)
         # extract parameter documentation (up to Returns line)
         pds = rest.split("\nReturns:\n")
-        spds = re.split(r"\n?([\w_]+)\s?\((\w+)\)\s?:", pds[0])[
+        spds = re.split(r"\n?([\w_]+)\s?\((.+)\)\s?:", pds[0])[
             1:
         ]  # split :param lines
         pdict = dict(
             zip(spds[::3], zip(spds[1::3], spds[2::3]))
         )  # create initial param dict
         pdict = {
             k: {
@@ -276,44 +282,44 @@
         if ds and ds.count("\n") > 0:
             dd = self.description.split("\n")
             ds = "\n".join([d.strip() for d in dd])
         for k, v in self.KNOWN_FORMATS.items():
             rc = re.compile(v)
             if rc.search(ds):
                 self.format = k
-        if not self.format:
-            logger.warning("Unknown param desc format!")
 
     def process_descr(self):
         """
         Helper function to provide plugin style parsers for various
         formats.
         """
         do = f"_process_{self.format}"
         if hasattr(self, do) and callable(func := getattr(self, do)):
             logger.debug("Calling %s parser function", do)
             return func(self.description)
         else:
-            logger.warning("Format not recognized or can't execute %s", do)
-            logger.warning("Returning description unparsed!")
+            if do[-1] == "_":
+                logger.debug("Format not recognized.")
+            else:
+                logger.debug("Can't execute %s", do)
             return (self.description, {})
 
 
 class GreatGrandChild:
     """
     The great-grandchild class performs most of the parsing to construct the
     palette nodes from the doxygen XML.
     """
 
     def __init__(
         self,
         ggchild: ET.Element = ET.Element("dummy"),
         func_name: str = "Unknown",
         return_type: str = "Unknown",
-        parent_member: Union["Child", None] = None,
+        parent_member: Union[dict, None] = None,
     ):
         """
         Constructor of great-grandchild object.
 
         :param ggchild: dict, if existing great-grandchild
         :param func_name: str, the function name
         :param return_type: str, the return type of the component
@@ -325,17 +331,19 @@
         self.return_type = return_type
         if ggchild:
             self.member = self.process_GreatGrandChild(
                 ggchild, parent_member=parent_member
             )
         else:
             self.member = {"params": []}
+        self.isclass = False
+        self.usage = "NoPort"
 
     def process_GreatGrandChild(
-        self, ggchild: ET.Element, parent_member: Union["Child", None] = None
+        self, ggchild: ET.Element, parent_member: Union[dict, None] = None
     ):
         """
         Process GreatGrandChild
 
         :param ggchild: dict, the great grandchild element
         :param parent_member: dict, member dict from parent class
         """
@@ -354,14 +362,15 @@
                 {"key": "text", "direction": None, "value": self.func_name}
             )
             logger.debug("Function name: %s", self.func_name)
         elif ggchild.tag == "argsstring":  # type: ignore
             args = ggchild.text[1:-1]  # type: ignore
             args = [a.strip() for a in args.split(",")]
             if "self" in args:
+                self.isclass = True
                 class_name = self.func_path.rsplit(".", 1)[-1]
                 self.func_name = f"{class_name}::{self.func_name}"
                 logger.debug(
                     "Class function --> modified name: %s",
                     self.func_name,
                 )
 
@@ -421,14 +430,16 @@
                             value_type = ggggchild.text  # type:ignore
                 if gggchild.tag == "declname":
                     name = gggchild.text  # type:ignore
                 if gggchild.tag == "defname":
                     name = gggchild.text  # type:ignore
                 if gggchild.tag == "defval":
                     default_value = gggchild.text  # type:ignore
+            if name == "self":
+                self.usage = "NoPort"
             if (
                 name in self.member["params"]
                 and "type" in self.member["params"][name]
             ):
                 logger.debug(
                     "Existing type definition found for %s: %s",
                     name,
@@ -441,43 +452,55 @@
 
             # add the param
             if str(value_type) == "String":
                 default_value = str(default_value).replace("'", "")
                 if default_value.find("/") >= 0:
                     default_value = f'"{default_value}"'
             # attach description from parent, if available
-            if parent_member and name in parent_member.member["params"]:
-                member_desc = parent_member.member["params"][name]
+            if parent_member and name in parent_member["params"]:
+                member_desc = parent_member["params"][name]
+                logger.debug(
+                    "Parent member: %s", parent_member["params"][name]
+                )
             else:
                 member_desc = ""
-
+            self.usage = (
+                "OutputPort" if self.isclass and name == "self" else "NoPort"
+            )
+            self.usage = (
+                "InputPort"
+                if not self.isclass and name == "self"
+                else "NoPort"
+            )
             logger.debug(
                 "adding param: %s",
                 {
                     "key": str(name),
                     "direction": "in",
                     "value": str(name)
                     + "/"
                     + str(default_value)
                     + "/"
                     + str(value_type)
-                    + "/ApplicationArgument/readwrite//False/False/"
+                    + f"/ApplicationArgument,{self.usage}"
+                    + "/readwrite//False/False/"
                     + member_desc,
                 },
             )
             self.member["params"].append(
                 {
                     "key": str(name),
                     "direction": "in",
                     "value": str(name)
                     + "/"
                     + str(default_value)
                     + "/"
                     + str(value_type)
-                    + "/ApplicationArgument/readwrite//False/False/"
+                    + f"/ApplicationArgument,{self.usage}"
+                    + "/readwrite//False/False/"
                     + member_desc,
                 }
             )
 
         elif ggchild.tag == "definition":  # type: ignore
             self.return_type = ggchild.text.strip().split(" ")[  # type: ignore
                 0
@@ -512,34 +535,36 @@
                 )
                 self.member["params"].append(
                     {
                         "key": "func_name",
                         "direction": None,
                         "value": "Function Name/"
                         + f"{self.func_path}.{self.func_name}"
-                        + "/String/ApplicationArgument/readonly/"
+                        + f"/String/ApplicationArgument,{self.usage}/readonly/"
                         + "/False/True/Python function name",
                     }
                 )
                 self.member["params"].append(
                     {
                         "key": "input_parser",
                         "direction": None,
                         "value": "Input Parser/pickle/Select/"
-                        + "ApplicationArgument/readwrite/pickle,eval,"
+                        + f"ApplicationArgument,{self.usage}"
+                        + "/readwrite/pickle,eval,"
                         + "npy,path,dataurl/False/False/Input port "
                         + "parsing technique",
                     }
                 )
                 self.member["params"].append(
                     {
                         "key": "output_parser",
                         "direction": None,
                         "value": "Output Parser/pickle/Select/"
-                        + "ApplicationArgument/readwrite/pickle,eval,npy,path,"
+                        + f"ApplicationArgument,{self.usage}"
+                        + "/readwrite/pickle,eval,npy,path,"
                         + "dataurl/False/False/Output port parsing technique",
                     }
                 )
         else:
             logger.debug(
                 "Ignored great grandchild element: %s",
                 ggchild.tag,  # type: ignore
@@ -606,14 +631,16 @@
             logger.debug("Parsing detaileddescription")
             # logger.debug("Child: %s", ET.tostring(child, encoding="unicode"))
             self.type = "description"
             # TODO: The following likely means that we are dealing with a C
             #       module and this is just a dirty workaround rather than
             #        a fix probably need to add a plain C parser.
             dStr = child[0][0].text if len(child[0]) > 0 else child[0]
+            if dStr is None:
+                dStr = ""
             self.description = dStr  # type: ignore
             ddO = DetailedDescription(dStr)  # type: ignore
             self.format = ddO.format
             if self.format == "casa":
                 self.casa_mode = True
                 self.description, self.member["params"] = (
                     ddO.main_descr,
@@ -621,24 +648,23 @@
                 )
 
         if child.tag == "sectiondef" and child.get("kind") in [  # type: ignore
             "func",
             "public-func",
         ]:
             self.type = "function"
+            member = parent.member if parent else None
             logger.debug(
                 "Processing %d grand children; parent: %s",
                 len(child),
-                parent.member if parent else "<undefined>",
+                member if member else "<undefined>",
             )
             for grandchild in child:
                 gmember = self._process_grandchild(
-                    grandchild,
-                    language,
-                    # parent=self
+                    grandchild, language, parent_members=member
                 )
                 if gmember is None:
                     logger.debug("Bailing out of grandchild processing!")
                     continue
                 elif gmember != self.member:
                     # logger.debug("Adding grandchild members: %s", gmember)
                     self.member["params"].extend(gmember["params"])
@@ -646,15 +672,15 @@
             logger.debug("Finished processing grand children")
         self.members = members
 
     def _process_grandchild(
         self,
         gchild: ET.Element,
         language: Language,
-        # parent: Union["Child", None] = None,
+        parent_members: Union[dict, None] = None,
     ) -> Union[dict, None]:
         """
         Private function to process a grandchild element
         Starts the construction of the member data structure
 
         :param gchild: dict, the parsed grandchild element from XML
         :param language: int, the languange indicator flag,
@@ -679,17 +705,18 @@
                         "value": "DynlibApp",
                     }
                 )
                 member["params"].append(
                     {
                         "key": "libpath",
                         "direction": None,
-                        "value": "Library Path//String/ComponentParameter/"
-                        + "readwrite//False/False/The location of the shared "
-                        + "object/DLL that implements this application",
+                        "value": "Library Path//String/ComponentParameter,"
+                        + "NoPort/readwrite//False/False/The location of the"
+                        + " shared object/DLL that implements this"
+                        + " application",
                     }
                 )
             elif language == Language.PYTHON:
                 member["params"].append(
                     {
                         "key": "category",
                         "direction": None,
@@ -697,50 +724,55 @@
                     }
                 )
                 member["params"].append(
                     {
                         "key": "appclass",
                         "direction": None,
                         "value": "Application Class/dlg.apps.pyfunc.PyFuncApp/"
-                        + "String/ComponentParameter/readwrite//False/False/"
+                        + "String/ComponentParameter,NoPort/readwrite//False/"
+                        + "False/"
                         + "The python class that implements this application",
                     }
                 )
 
             member["params"].append(
                 {
                     "key": "execution_time",
                     "direction": None,
-                    "value": "Execution Time/5/Integer/ComponentParameter/"
+                    "value": "Execution Time/5/Integer/ComponentParameter,"
+                    + "NoPort/"
                     + "readwrite//False/False/Estimate of execution time "
                     + "(in seconds) for this application.",
                 }
             )
             member["params"].append(
                 {
                     "key": "num_cpus",
                     "direction": None,
-                    "value": "No. of CPUs/1/Integer/ComponentParameter/"
+                    "value": "No. of CPUs/1/Integer/ComponentParameter,NoPort/"
                     + "readwrite//False/False/Number of cores used.",
                 }
             )
             member["params"].append(
                 {
                     "key": "group_start",
                     "direction": None,
-                    "value": "Group start/false/Boolean/ComponentParameter/"
+                    "value": "Group start/false/Boolean/ComponentParameter,"
+                    + "NoPort/"
                     + "readwrite//False/False/Is this node the start of "
                     + "a group?",
                 }
             )
 
             logger.debug("Processing %d great grand children", len(gchild))
             gg = GreatGrandChild()
             for ggchild in gchild:
-                gg.process_GreatGrandChild(ggchild, parent_member=self)
+                gg.process_GreatGrandChild(
+                    ggchild, parent_member=parent_members
+                )
                 if gg.member is None:
                     logger.debug(
                         "Bailing out ggchild processing: %s", gg.member
                     )
                     del gg
                     return None
             if gg.member != member and gg.member["params"] not in [None, []]:
@@ -750,7 +782,38 @@
                 "Finished processing of function definition: '%s:%s'",
                 gg.func_path,
                 gg.func_name,
             )
             del gg
 
         return member
+
+
+@dataclass
+class Field:
+    internal_name: str
+    external_name: str
+    value: str
+    value_type: str
+    field_type: str
+    usage: str
+    access: str = "readonly"
+    options: str = ""
+    precious: bool = False
+    positional: bool = False
+    description: str = ""
+
+    def to_dict(self):
+        return {
+            "text": self.external_name,
+            "name": self.internal_name,
+            "value": self.value,
+            "defaultValue": self.value,
+            "description": self.description,
+            "type": self.value_type,
+            "fieldType": self.field_type,
+            "usage": self.usage,
+            "readonly": self.access == "readonly",
+            "options": self.options,
+            "precious": self.precious,
+            "positional": self.positional,
+        }
```

### Comparing `dlg_paletteGen-0.1.8/dlg_paletteGen/cli.py` & `dlg_paletteGen-0.1.9/dlg_paletteGen/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 import tempfile
 
 import pkg_resources
 
 # isort: ignore
 from dlg_paletteGen.base import (
     Language,
-    logger,
+    module_hook,
     prepare_and_write_palette,
     process_compounddefs,
 )
 from dlg_paletteGen.support_functions import (
     DOXYGEN_SETTINGS,
     process_doxygen,
     process_xml,
+    logger,
 )
 
 NAME = "dlg_paletteGen"
 VERSION = pkg_resources.require(NAME)[0].version
 
 
 def get_args():
@@ -108,14 +109,15 @@
     language = Language.C if args.c else Language.PYTHON
     return (
         args.idir,
         args.tag,
         args.ofile,
         args.parse_all,
         args.module,
+        args.recursive,
         language,
     )
 
 
 def check_environment_variables() -> bool:
     """
     Check environment variables and set them if not defined.
@@ -154,14 +156,15 @@
         sys.exit(1)
     (
         inputdir,
         tag,
         outputfile,
         allow_missing_eagle_start,
         module_path,
+        recursive,
         language,
     ) = get_args()
     logger.info("PROJECT_NAME:" + os.environ.get("PROJECT_NAME"))
     logger.info("PROJECT_VERSION:" + os.environ.get("PROJECT_VERSION"))
     logger.info("GIT_REPO:" + os.environ.get("GIT_REPO"))
 
     logger.info("Input Directory:" + inputdir)
@@ -169,25 +172,32 @@
     logger.info("Output File:" + outputfile)
     logger.info("Allow missing EAGLE_START:" + str(allow_missing_eagle_start))
     logger.info("Module Path:" + module_path)
 
     # create a temp directory for the output of doxygen
     output_directory = tempfile.TemporaryDirectory()
 
-    # add extra doxygen setting for input and output locations
-    DOXYGEN_SETTINGS.update({"PROJECT_NAME": os.environ.get("PROJECT_NAME")})
-    DOXYGEN_SETTINGS.update({"INPUT": inputdir})
-    DOXYGEN_SETTINGS.update({"OUTPUT_DIRECTORY": output_directory.name})
-
-    process_doxygen(language=language)
-    output_xml_filename = process_xml()
-
-    # get environment variables
-    # gitrepo = os.environ.get("GIT_REPO")
-    # version = os.environ.get("PROJECT_VERSION")
+    if len(module_path) > 0:
+        modules, mod_count = module_hook(module_path, recursive=recursive)
+        # member_count = sum([len(m) for m in modules])
+        logger.info(">>>>> Number of modules processed: %d", mod_count)
+    else:
+        # add extra doxygen setting for input and output locations
+        DOXYGEN_SETTINGS.update(
+            {"PROJECT_NAME": os.environ.get("PROJECT_NAME")}
+        )
+        DOXYGEN_SETTINGS.update({"INPUT": inputdir})
+        DOXYGEN_SETTINGS.update({"OUTPUT_DIRECTORY": output_directory.name})
+
+        process_doxygen(language=language)
+        output_xml_filename = process_xml()
 
-    nodes = process_compounddefs(
-        output_xml_filename, allow_missing_eagle_start, language
-    )
-    prepare_and_write_palette(nodes, outputfile)
-    # cleanup the output directory
+        # get environment variables
+        # gitrepo = os.environ.get("GIT_REPO")
+        # version = os.environ.get("PROJECT_VERSION")
+
+        nodes = process_compounddefs(
+            output_xml_filename, allow_missing_eagle_start, language, tag
+        )
+        prepare_and_write_palette(nodes, outputfile)
+        # cleanup the output directory
     output_directory.cleanup()
```

### Comparing `dlg_paletteGen-0.1.8/dlg_paletteGen/support_functions.py` & `dlg_paletteGen-0.1.9/dlg_paletteGen/support_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 import subprocess
 import tempfile
 import types
 import uuid
 import xml.etree.ElementTree as ET
 from enum import Enum
+from pkgutil import iter_modules
 
 DOXYGEN_SETTINGS = {
     "OPTIMIZE_OUTPUT_JAVA": "YES",
     "AUTOLINK_SUPPORT": "NO",
     "IDL_PROPERTY_SUPPORT": "NO",
     "EXCLUDE_PATTERNS": "*/web/*, CMakeLists.txt",
     "VERBATIM_HEADERS": "NO",
@@ -60,14 +61,15 @@
         return formatter.format(record)
 
 
 # create console handler with a higher log level
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 
+
 ch.setFormatter(CustomFormatter())
 
 logger = logging.getLogger(__name__)
 logger.addHandler(ch)
 
 next_key = -1
 
@@ -325,7 +327,29 @@
         )
 
     # debug - copy output xml to local dir
     # TODO: do this only if DEBUG is enabled
     os.system("cp " + output_xml_filename + " output.xml")
     logger.info("Wrote doxygen XML to output.xml")
     return output_xml_filename
+
+
+def get_submodules(module):
+    """
+    Retrieve names of sub-modules using iter_modules.
+    This will also return sub-packages. Third tuple
+    item is a flag ispkg indicating that.
+
+    :module module: module object to be searched
+
+    :returns iterator[tuple]
+    """
+    if not isinstance(module, types.ModuleType):
+        logger.warning(
+            "Provided object %s is not a module: %s",
+            module,
+            type(module),
+        )
+        return iter([])
+    if hasattr(module, "__path__"):
+        return iter_modules(module.__path__)
+    return iter([])
```

### Comparing `dlg_paletteGen-0.1.8/dlg_paletteGen.egg-info/PKG-INFO` & `dlg_paletteGen-0.1.9/dlg_paletteGen.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlg-paletteGen
-Version: 0.1.8
+Version: 0.1.9
 Summary: DALiuGE palette generator tool
 Home-page: https://github.com/ICRAR/dlg_paletteGen/
 Author: ICRAR
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 [![codecov](https://codecov.io/gh/ICRAR/dlg_paletteGen/branch/main/graph/badge.svg?token=dlg_paletteGen_token_here)](https://codecov.io/gh/ICRAR/dlg_paletteGen)
 [![CI](https://github.com/ICRAR/dlg_paletteGen/actions/workflows/main.yml/badge.svg)](https://github.com/ICRAR/dlg_paletteGen/actions/workflows/main.yml)
 
 This is the palette generator of the [DALiuGE](https://daliuge.readthedocs.io) system.
 
 It processes a file or a directory of source files and
 produces a DALiuGE compatible palette file containing the
-information required to use the identified functions and classes and methods to construct logical graphs in [EAGLE](https://eagle-dlg.readthedocs.io).
+information required to use the identified functions and classes and methods to construct computational workflows in [EAGLE](https://eagle-dlg.readthedocs.io).
 For more information please refer to the [documentation](https://icrar.github.io/dlg_paletteGen/).
 
 ## Install it from PyPI
 
 ```bash
 pip install dlg_paletteGen
 ```
@@ -41,15 +41,15 @@
 
 usage: dlg_paletteGen [-h] [-m MODULE] [-t TAG] [-c] [-r] [-s] [-v] idir ofile
 
 This is the palette generator of the DALiuGE system.
 
 It processes a file or a directory of source files and
 produces a DALiuGE compatible palette file containing the
-information required to use functions and components in graphs.
+information required to use functions and components in workflows.
 For more information please refer to the documentation
 https://daliuge.readthedocs.io/en/latest/development/app_development/eagle_app_integration.html#automatic-eagle-palette-generation
 
 positional arguments:
   idir                  input directory path or file name
   ofile                 output file name
```

### Comparing `dlg_paletteGen-0.1.8/dlg_paletteGen.egg-info/SOURCES.txt` & `dlg_paletteGen-0.1.9/dlg_paletteGen.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 tests/conftest.py
 tests/test_base.py
 tests/data/example_casatask.py
 tests/data/example_eagle.py
 tests/data/example_google.py
 tests/data/example_numpy.py
 tests/data/example_rascil.py
-tests/data/example_rest.py
+tests/data/example_rest.py
+tests/data/hifa_importdata.py
```

### Comparing `dlg_paletteGen-0.1.8/setup.py` & `dlg_paletteGen-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.1.8/tests/data/example_casatask.py` & `dlg_paletteGen-0.1.9/tests/data/example_casatask.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.1.8/tests/data/example_eagle.py` & `dlg_paletteGen-0.1.9/tests/data/example_eagle.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.1.8/tests/data/example_google.py` & `dlg_paletteGen-0.1.9/tests/data/example_google.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.1.8/tests/data/example_numpy.py` & `dlg_paletteGen-0.1.9/tests/data/example_numpy.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.1.8/tests/data/example_rascil.py` & `dlg_paletteGen-0.1.9/tests/data/example_rascil.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.1.8/tests/data/example_rest.py` & `dlg_paletteGen-0.1.9/tests/data/example_rest.py`

 * *Files identical despite different names*

### Comparing `dlg_paletteGen-0.1.8/tests/test_base.py` & `dlg_paletteGen-0.1.9/tests/test_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     This method returns the new process.
     """
 
     cmdline = ["dlg_paletteGen"]
     if args:
         cmdline.extend(args)
+    logging.info("Starting process: %s %s", cmdline, subproc_args)
     return subprocess.Popen(cmdline, **subproc_args)
 
 
 # class MainTest(unittest.TestCase):
 def test_base():
     assert NAME == "dlg_paletteGen"
 
@@ -163,35 +164,39 @@
     with open(output, "r") as f:
         newcontent = json.load(f)
     logging.info("OUTPUT: %s", newcontent)
     # can't use a hash, since output contains hashed keys
     assert len(newcontent["nodeDataArray"][0]["fields"]) == 14
 
 
-def test_CLI_run_casatask(tmpdir: str, shared_datadir: str):
+def test_CLI_run_casatask2(tmpdir: str, shared_datadir: str):
     """
     Test the CLI just using input and output.
 
     :param tmpdir: the path to the temp directory to use
     :param shared_datadir: the path the the local directory
     """
-    input = str(shared_datadir.absolute()) + "/example_casatask.py"
+    input = str(shared_datadir.absolute()) + "/hifa_importdata.py"
     logging.info("path: %s", input)
     output = tmpdir + "t.palette"
     p = start_process(
-        ("-rs", input, output),
+        ("-rvs", input, output),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
     out, err = p.communicate()
     assert p.returncode == 0
-    # logging.info("Captured output: %s", err)
+    logging.info(
+        "===================== Procedure output start ================="
+    )
+    logging.info("Captured output: %s", err.decode())
+    logging.info("===================== Procedure output end ===============")
     with open(input, "r") as f:
         content = f.read()
-    logging.info("INPUT: %s", content)
+    # logging.info("INPUT: %s", content)
     with open(output, "r") as f:
         newcontent = json.load(f)
     logging.info("OUTPUT: %s", newcontent)
     # can't use a hash, since output contains hashed keys
     assert newcontent["modelData"]["commitHash"] == "0.1"
 
 
@@ -208,15 +213,15 @@
     p = start_process(
         ("-s", "-v", input, output),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
     out, err = p.communicate()
     assert p.returncode == 0
-    # logging.info("Captured output: %s", err)
+    # logging.info("Captured output: %s", out)
     with open(input, "r") as f:
         content = f.read()
     logging.info("INPUT: %s", content)
     with open(output, "r") as f:
         newcontent = json.load(f)
     logging.info("OUTPUT: %s", newcontent)
     # can't use a hash, since output contains hashed keys
```

