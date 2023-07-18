# Comparing `tmp/quokka-project-0.5.1.tar.gz` & `tmp/quokka-project-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quokka-project-0.5.1.tar", last modified: Thu Mar 16 10:29:34 2023, max compression
+gzip compressed data, was "quokka-project-0.5.2.tar", last modified: Tue Jul 18 19:40:25 2023, max compression
```

## Comparing `quokka-project-0.5.1.tar` & `quokka-project-0.5.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:29:34.841886 quokka-project-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-03-16 10:29:29.000000 quokka-project-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-16 10:29:34.841886 quokka-project-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-03-16 10:29:29.000000 quokka-project-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:29:34.837886 quokka-project-0.5.1/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:29:34.837886 quokka-project-0.5.1/bindings/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:29:34.837886 quokka-project-0.5.1/bindings/python/quokka/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/addresser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:29:34.841886 quokka-project-0.5.1/bindings/python/quokka/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/analysis/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/analysis/calling_convention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/analysis/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/analysis/replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/analysis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:29:34.841886 quokka-project-0.5.1/bindings/python/quokka/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/backends/capstone.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/backends/pypcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/program.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25403 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/quokka_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-03-16 10:29:29.000000 quokka-project-0.5.1/bindings/python/quokka/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:29:34.841886 quokka-project-0.5.1/bindings/python/quokka_project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-16 10:29:34.000000 quokka-project-0.5.1/bindings/python/quokka_project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-16 10:29:34.000000 quokka-project-0.5.1/bindings/python/quokka_project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 10:29:34.000000 quokka-project-0.5.1/bindings/python/quokka_project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-16 10:29:34.000000 quokka-project-0.5.1/bindings/python/quokka_project.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 10:29:34.000000 quokka-project-0.5.1/bindings/python/quokka_project.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 10:29:34.841886 quokka-project-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-16 10:29:29.000000 quokka-project-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:40:25.194939 quokka-project-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-18 19:40:22.000000 quokka-project-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-18 19:40:25.194939 quokka-project-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-18 19:40:22.000000 quokka-project-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:40:25.190939 quokka-project-0.5.2/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:40:25.190939 quokka-project-0.5.2/bindings/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:40:25.194939 quokka-project-0.5.2/bindings/python/quokka/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/addresser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:40:25.194939 quokka-project-0.5.2/bindings/python/quokka/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/analysis/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/analysis/calling_convention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/analysis/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/analysis/replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/analysis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:40:25.194939 quokka-project-0.5.2/bindings/python/quokka/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/backends/capstone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/backends/pypcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22990 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25403 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/quokka_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17921 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 19:40:22.000000 quokka-project-0.5.2/bindings/python/quokka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:40:25.194939 quokka-project-0.5.2/bindings/python/quokka_project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-18 19:40:25.000000 quokka-project-0.5.2/bindings/python/quokka_project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-18 19:40:25.000000 quokka-project-0.5.2/bindings/python/quokka_project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:40:25.000000 quokka-project-0.5.2/bindings/python/quokka_project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-18 19:40:25.000000 quokka-project-0.5.2/bindings/python/quokka_project.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 19:40:25.000000 quokka-project-0.5.2/bindings/python/quokka_project.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:40:25.194939 quokka-project-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-18 19:40:22.000000 quokka-project-0.5.2/setup.py
```

### Comparing `quokka-project-0.5.1/LICENSE` & `quokka-project-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.1/PKG-INFO` & `quokka-project-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka-project
-Version: 0.5.1
+Version: 0.5.2
 Summary: Quokka : A Fast and Accurate Binary Exporter
 Home-page: https://github.com/quarkslab/quokka
 Author: Alexis <dm> Challande
 Author-email: achallande@quarkslab.com
 License: Apache-2
 Project-URL: Documentation, https://quarkslab.github.io/quokka/
 Project-URL: Bug Tracker, https://github.com/quarkslab/quokka/issues
@@ -62,14 +62,16 @@
 ```
 
 ### IDA Plugin
 
 Note: The IDA plugin is not needed to read a `Quokka` generated file. It is
 only used to generate them.
 
+Quokka is currently compatible with IDA 7.3+
+
 The plugin is built on the CI and available in the
 [Release](https://github.com/quarkslab/quokka/releases/new) tab.
 
 To download the plugin, get the file named `quokka_plugin**.so`.
 
 ## Usage
```

### Comparing `quokka-project-0.5.1/README.md` & `quokka-project-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 ```
 
 ### IDA Plugin
 
 Note: The IDA plugin is not needed to read a `Quokka` generated file. It is
 only used to generate them.
 
+Quokka is currently compatible with IDA 7.3+
+
 The plugin is built on the CI and available in the
 [Release](https://github.com/quarkslab/quokka/releases/new) tab.
 
 To download the plugin, get the file named `quokka_plugin**.so`.
 
 ## Usage
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/__init__.py` & `quokka-project-0.5.2/bindings/python/quokka/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Quokka : A pythonic program manipulation tool
 
 Quokka is a module designed to help using an exported program from a Python(ic) API.
 It must be used with the exported version of a file (a Quokka file) and the binary
 itself.
 """
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.5.1"
-__quokka_version__ = "0.5.1"
+from quokka.version import __version__
 
 import quokka.analysis
 import quokka.backends
 import quokka.quokka_pb2 as pb
 
 from quokka.addresser import Addresser
 
@@ -66,14 +65,15 @@
 from quokka.utils import (
     md5_file,
     sha256_file,
     check_hash,
     get_isa,
     convert_address_size,
     get_arch,
+    parse_version,
 )
 
 __all__ = [
     # From addresser.py
     "Addresser",
     # From block.py
     "Block",
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/addresser.py` & `quokka-project-0.5.2/bindings/python/quokka/addresser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Addresser : handle addresses management"""
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/analysis/__init__.py` & `quokka-project-0.5.2/bindings/python/quokka/analysis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Analysis modules
 
 This module contain some utilities function to manipulate the binaries.
 """
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,14 +20,18 @@
     QuokkaArch,
     ArchEnum,
     ArchX86,
     ArchX64,
     ArchARM,
     ArchARM64,
     ArchARMThumb,
+    ArchMIPS,
+    ArchMIPS64,
+    ArchPPC,
+    ArchPPC64,
 )
 
 from quokka.analysis.calling_convention import (
     CallingConvention,
     CCdecl,
     Stdcall,
     Fastcall,
@@ -52,14 +56,18 @@
     "QuokkaArch",
     "ArchEnum",
     "ArchX86",
     "ArchX64",
     "ArchARM",
     "ArchARM64",
     "ArchARMThumb",
+    "ArchMIPS",
+    "ArchMIPS64",
+    "ArchPPC",
+    "ArchPPC64",
     # From calling_convention.py
     "CallingConvention",
     "CCdecl",
     "Stdcall",
     "Fastcall",
     "MicrosoftAMD64",
     "SystemVAMD",
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/analysis/arch.py` & `quokka-project-0.5.2/bindings/python/quokka/analysis/arch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Architecture module"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,15 +24,15 @@
 
 def make_enums(
     capstone_module: ModuleType, items: List[str], blacklist: List[str], flags_enums: List[str]
 ) -> List:
     """Make enums from capstone module
 
     Dynamically generate enums from capstone constants
-    0
+
     Arguments:
         capstone_module: Capstone module
         items: Name of enums
         blacklist: Fields to not consider
         flags_enums: List of flag enums
 
     Returns:
@@ -159,15 +159,15 @@
 
     frame_pointer = regs.FP
     stack_pointer = regs.SP
     inst_pointer = regs.PC
 
 
 class ArchARMThumb(ArchARM):  # type: ignore
-    """Arch Arm Thum definition"""
+    """Arch Arm Thumb definition"""
 
     thumb: bool = True
 
 
 class ArchARM64(QuokkaArch):  # type: ignore
     """Arch Arm64 definition"""
 
@@ -225,7 +225,95 @@
         insts.TBZ,
         insts.TBNZ,
     ]
 
     frame_pointer = regs.FP
     stack_pointer = regs.SP  # TODO(dm)!
     inst_pointer = regs.X28
+
+
+class ArchMIPS(QuokkaArch):  # type: ignore
+    """Arch MIPS definition"""
+
+    (
+        grps,
+        insts,
+        op,
+        regs,
+    ) = make_enums(
+        capstone_module=capstone.mips_const,
+        items=[
+            "GRP",
+            "INS",
+            "OP",
+            "REG",
+        ],
+        blacklist=["ENDING", "INVALID"],
+        flags_enums=[],
+    )
+
+    compared_mnemonics = [
+        insts.CMP,
+        insts.CMPI,
+        insts.CMPU,
+        insts.CMPGU,
+        insts.CMPGDU,
+    ]
+
+    address_size = 32
+
+    frame_pointer = regs.FP  # R30
+    stack_pointer = regs.SP  # R29
+    inst_pointer = regs.PC   # REG_PC
+
+
+class ArchMIPS64(ArchMIPS):  # type: ignore
+    """Arch MIPS64 definition"""
+
+    address_size = 64
+
+
+class ArchPPC(QuokkaArch):  # type: ignore
+    """Arch PPC definition"""
+
+    (
+        bc,
+        bh,
+        grps,
+        insts,
+        op,
+        regs,
+    ) = make_enums(
+        capstone_module=capstone.ppc_const,
+        items=[
+            "BC",
+            "BH",
+            "GRP",
+            "INS",
+            "OP",
+            "REG",
+        ],
+        blacklist=["ENDING", "INVALID"],
+        flags_enums=[],
+    )
+
+    compared_mnemonics = [
+        insts.CMPB,
+        insts.CMPD,
+        insts.CMPDI,
+        insts.CMPLD,
+        insts.CMPLW,
+        insts.CMPW,
+        insts.CMPWI,
+    ]
+
+    address_size = 32
+
+    frame_pointer = regs.R1  #
+    stack_pointer = regs.R1  # GPR1
+    inst_pointer = regs.CTR
+
+
+class ArchPPC64(ArchPPC):  # type: ignore
+    """Arch PPC64 definition"""
+
+    address_size = 64
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/analysis/calling_convention.py` & `quokka-project-0.5.2/bindings/python/quokka/analysis/calling_convention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Calling conventions"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/analysis/env.py` & `quokka-project-0.5.2/bindings/python/quokka/analysis/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Environment module"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/analysis/replacer.py` & `quokka-project-0.5.2/bindings/python/quokka/analysis/replacer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/analysis/utils.py` & `quokka-project-0.5.2/bindings/python/quokka/analysis/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Utilities functions for the analysis"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/backends/__init__.py` & `quokka-project-0.5.2/bindings/python/quokka/backends/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Backends integration"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/backends/capstone.py` & `quokka-project-0.5.2/bindings/python/quokka/backends/capstone.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Capstone integration"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,38 +15,58 @@
 
 from __future__ import annotations
 import capstone
 
 import quokka
 import quokka.analysis
 
-from quokka.types import AddressT, Type, Optional
+from quokka.types import AddressT, Endianness, Type, Optional
 
 
-def get_capstone_context(arch: Type[quokka.analysis.QuokkaArch]) -> capstone.Cs:
+def get_capstone_context(
+        arch: Type[quokka.analysis.QuokkaArch],
+        endian: Type[Endianness] = Endianness.LITTLE_ENDIAN) -> capstone.Cs:
     """Compute the capstone context for the program
 
     The Capstone context is used to decode instructions afterwards. Since we are
     interested in most of the details, we already set the details to True.
 
     Arguments:
         arch: Quokka program architecture
 
     Returns:
         A capstone Cs instance
     """
+    endian_mapping = {
+        Endianness.BIG_ENDIAN: capstone.CS_MODE_BIG_ENDIAN,
+        Endianness.LITTLE_ENDIAN: capstone.CS_MODE_LITTLE_ENDIAN,
+    }
+    capstone_endian = endian_mapping[endian]
+
     mapping = {
         quokka.analysis.ArchARM: (capstone.CS_ARCH_ARM, capstone.CS_MODE_ARM),
         quokka.analysis.ArchARM64: (capstone.CS_ARCH_ARM64, capstone.CS_MODE_ARM),
         quokka.analysis.ArchX86: (capstone.CS_ARCH_X86, capstone.CS_MODE_32),
         quokka.analysis.ArchX64: (capstone.CS_ARCH_X86, capstone.CS_MODE_64),
         quokka.analysis.ArchARMThumb: (
             capstone.CS_ARCH_ARM,
             capstone.CS_MODE_THUMB,
         ),
+        quokka.analysis.ArchMIPS: (
+            capstone.CS_ARCH_MIPS,
+            capstone.CS_MODE_32 + capstone_endian),
+        quokka.analysis.ArchMIPS64: (
+            capstone.CS_ARCH_MIPS,
+            capstone.CS_MODE_64 + capstone_endian),
+        quokka.analysis.ArchPPC: (
+            capstone.CS_ARCH_PPC,
+            capstone.CS_MODE_32 + capstone_endian),
+        quokka.analysis.ArchPPC64: (
+            capstone.CS_ARCH_PPC,
+            capstone.CS_MODE_64 + capstone_endian),
     }
 
     try:
         capstone_arch, capstone_mode = mapping.get(arch)
     except TypeError as exc:
         raise quokka.CapstoneError("Unable to find the Architecture") from exc
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/backends/pypcode.py` & `quokka-project-0.5.2/bindings/python/quokka/backends/pypcode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """PyPCode integration"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,15 +18,15 @@
 import itertools
 import logging
 
 import pypcode
 
 import quokka
 import quokka.analysis
-from quokka.types import Any, Dict, List, Sequence, Type, Optional
+from quokka.types import Any, Dict, Endianness, List, Sequence, Type, Optional
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def get_arch_from_string(target_id: str) -> pypcode.ArchLanguage:
     """Find the architecture for an arch based on the target identification
 
@@ -45,15 +45,16 @@
             if lang.id == target_id:
                 return lang
 
     raise quokka.PypcodeError("Unable to find the appropriate arch: missing lang")
 
 
 def get_pypcode_context(
-    arch: Type[quokka.analysis.QuokkaArch],
+        arch: Type[quokka.analysis.QuokkaArch],
+        endian: Type[Endianness] = Endianness.LITTLE_ENDIAN
 ) -> pypcode.Context:
     """Convert an arch from Quokka to Pypcode
 
     For the moment, only the arch described in quokka.analysis are supported.
     This method is a bit slow because enum are generated by pypcode on the fly but should
     be executed only once.
 
@@ -68,23 +69,30 @@
     """
     names: Dict[Type[quokka.analysis.arch.QuokkaArch], str] = {
         quokka.analysis.ArchX64: "x86:LE:64:default",
         quokka.analysis.ArchX86: "x86:LE:32:default",
         quokka.analysis.ArchARM: "ARM:LE:32:v8",
         quokka.analysis.ArchARM64: "AARCH64:LE:64:v8A",
         quokka.analysis.ArchARMThumb: "ARM:LE:32:v8T",
+        quokka.analysis.ArchMIPS: "MIPS:LE:32:default",
+        quokka.analysis.ArchMIPS: "MIPS:LE:64:default",
+        quokka.analysis.ArchPPC: "PowerPC:LE:32:default",
+        quokka.analysis.ArchPPC64: "PowerPC:LE:64:default",
     }
 
     try:
         target_id = names[arch]
     except KeyError as exc:
         raise quokka.PypcodeError(
             "Unable to find the appropriate arch: missing id"
         ) from exc
 
+    if endian == Endianness.BIG_ENDIAN:
+        target_id = target_id.replace(":LE:", ":BE:")
+
     pcode_arch = get_arch_from_string(target_id)
     return pypcode.Context(pcode_arch)
 
 
 def equality(self: pypcode.ContextObj, other: Any) -> bool:
     """Check if two pypcode objets are the same
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/block.py` & `quokka-project-0.5.2/bindings/python/quokka/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Methods to use and deal with blocks in a binary."""
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/data.py` & `quokka-project-0.5.2/bindings/python/quokka/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Data management.
 
 A data is a piece of information that isn't code.
 """
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/exc.py` & `quokka-project-0.5.2/bindings/python/quokka/exc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Exceptions for quokka.
 
 All exceptions must derive from the QuokkaError.
 """
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/executable.py` & `quokka-project-0.5.2/bindings/python/quokka/executable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Executable: management of the binary file in itself."""
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/function.py` & `quokka-project-0.5.2/bindings/python/quokka/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Functions and chunk management"""
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/instruction.py` & `quokka-project-0.5.2/bindings/python/quokka/instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Methods to deal with instructions and operands within a binary"""
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/program.py` & `quokka-project-0.5.2/bindings/python/quokka/program.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Program
 
 This is the main class of Quokka.
 It deals with the most common abstraction, the Program.
 """
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -96,20 +96,29 @@
         self.export_file: pathlib.Path = pathlib.Path(export_file)
         with open(self.export_file, "rb") as fd:
             self.proto.ParseFromString(fd.read())
 
         # Export mode
         self.mode: ExporterMode = ExporterMode.from_proto(self.proto.exporter_meta.mode)
 
-        # Check if it matches the version
-        if self.proto.exporter_meta.version != quokka.__quokka_version__:
+        # Version checking
+        # A change in the major version might break backward compatibility
+        proto_version = quokka.parse_version(self.proto.exporter_meta.version)
+        current_version = quokka.parse_version(quokka.__version__)
+        if proto_version[0] != current_version[0]:
             self.logger.warning(
                 "The exported file has been generated by a different version of Quokka."
                 f" The file has been generated by Quokka {self.proto.exporter_meta.version}"
-                f" while python-quokka uses {quokka.__quokka_version__}"
+                f" while you are using {quokka.__version__}"
+            )
+        elif self.proto.exporter_meta.version != quokka.__version__:
+            self.logger.debug(
+                "Version mismatch detected but still compatible with the exported file."
+                f" The file has been generated by Quokka {self.proto.exporter_meta.version}"
+                f" while you are using {quokka.__version__}"
             )
 
         # Check if the hashes matches between the export file and the exec
         if not quokka.check_hash(self.proto.meta.hash, pathlib.Path(exec_path)):
             self.logger.error("Hash does not match with file.")
             raise quokka.QuokkaError("Hash mismatch")
 
@@ -168,15 +177,15 @@
     def hash(self) -> str:
         """Returns the hash value of the binary (either sha256 or MD5)."""
         return self.proto.meta.hash.hash_value
 
     @cached_property
     def capstone(self) -> capstone.Cs:
         """Compute a capstone context"""
-        return quokka.backends.get_capstone_context(self.arch)
+        return quokka.backends.get_capstone_context(self.arch, self.endianness)
 
     @cached_property
     def call_graph(self) -> networkx.DiGraph:
         """Compute the Call Graph of the binary
 
         Every node in the call graph is a chunk (and not a function).
 
@@ -196,15 +205,15 @@
                     )
 
         return call_graph
 
     @cached_property
     def pypcode(self) -> pypcode.Context:
         """Generate the Pypcode context."""
-        return quokka.backends.get_pypcode_context(self.arch)
+        return quokka.backends.get_pypcode_context(self.arch, self.endianness)
 
     @cached_property
     def structures(self) -> List[quokka.Structure]:
         """Structures accessor
 
         Allows to retrieve the different structures of a program (as defined by the
         disassembler).
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/quokka_pb2.py` & `quokka-project-0.5.2/bindings/python/quokka/quokka_pb2.py`

 * *Files identical despite different names*

### Comparing `quokka-project-0.5.1/bindings/python/quokka/reference.py` & `quokka-project-0.5.2/bindings/python/quokka/reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     - A Type
 
 As they are stored in a complex manner, this module deals with their resolution,
 i.e. how to resolve the pointed object.
 
 There is room for improvement here. ;)
 """
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/segment.py` & `quokka-project-0.5.2/bindings/python/quokka/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Segment management"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/structure.py` & `quokka-project-0.5.2/bindings/python/quokka/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Structure management"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/types.py` & `quokka-project-0.5.2/bindings/python/quokka/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Types used in Quokka"""
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka/utils.py` & `quokka-project-0.5.2/bindings/python/quokka/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Utilities functions"""
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,14 +24,18 @@
     QuokkaArch,
     ArchEnum,
     ArchX86,
     ArchX64,
     ArchARM,
     ArchARM64,
     ArchARMThumb,
+    ArchMIPS,
+    ArchMIPS64,
+    ArchPPC,
+    ArchPPC64,
 )
 
 from quokka.types import Type
 
 logger = logging.getLogger()
 
 
@@ -137,19 +141,39 @@
             32: ArchARM,
             64: ArchARM64,
         },
         ArchEnum.X86: {
             32: ArchX86,
             64: ArchX64,
         },
+        ArchEnum.MIPS: {
+            32: ArchMIPS,
+            64: ArchMIPS64,
+        },
+        ArchEnum.PPC: {
+            32: ArchPPC,
+            64: ArchPPC64,
+        },
     }
 
     platform_arch = mapping.get(isa)
     if platform_arch is None:
         return QuokkaArch
 
     arch = platform_arch.get(address_size, QuokkaArch)
 
     if arch == ArchARM and is_thumb:
         arch = ArchARMThumb
 
     return arch
+
+
+def parse_version(version: str) -> tuple[int, int, int]:
+    """Parse the version returning a tuple with the major, minor and patch"""
+
+    parsed = tuple(map(int, version.split(".")))
+    if len(parsed) != 3:
+        raise ValueError(
+            f"Version {version} doesn't respect the format MAJOR.MINOR.PATCH"
+        )
+
+    return parsed
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka_project.egg-info/PKG-INFO` & `quokka-project-0.5.2/bindings/python/quokka_project.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka-project
-Version: 0.5.1
+Version: 0.5.2
 Summary: Quokka : A Fast and Accurate Binary Exporter
 Home-page: https://github.com/quarkslab/quokka
 Author: Alexis <dm> Challande
 Author-email: achallande@quarkslab.com
 License: Apache-2
 Project-URL: Documentation, https://quarkslab.github.io/quokka/
 Project-URL: Bug Tracker, https://github.com/quarkslab/quokka/issues
@@ -62,14 +62,16 @@
 ```
 
 ### IDA Plugin
 
 Note: The IDA plugin is not needed to read a `Quokka` generated file. It is
 only used to generate them.
 
+Quokka is currently compatible with IDA 7.3+
+
 The plugin is built on the CI and available in the
 [Release](https://github.com/quarkslab/quokka/releases/new) tab.
 
 To download the plugin, get the file named `quokka_plugin**.so`.
 
 ## Usage
```

### Comparing `quokka-project-0.5.1/bindings/python/quokka_project.egg-info/SOURCES.txt` & `quokka-project-0.5.2/bindings/python/quokka_project.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 bindings/python/quokka/py.typed
 bindings/python/quokka/quokka_pb2.py
 bindings/python/quokka/reference.py
 bindings/python/quokka/segment.py
 bindings/python/quokka/structure.py
 bindings/python/quokka/types.py
 bindings/python/quokka/utils.py
+bindings/python/quokka/version.py
 bindings/python/quokka/analysis/__init__.py
 bindings/python/quokka/analysis/arch.py
 bindings/python/quokka/analysis/calling_convention.py
 bindings/python/quokka/analysis/env.py
 bindings/python/quokka/analysis/replacer.py
 bindings/python/quokka/analysis/utils.py
 bindings/python/quokka/backends/__init__.py
```

### Comparing `quokka-project-0.5.1/setup.py` & `quokka-project-0.5.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # -*- coding: utf-8 -*-
 
-#  Copyright 2022 Quarkslab
+#  Copyright 2022-2023 Quarkslab
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from setuptools import setup
+from os.path import normpath
 
 with open("README.md", "r") as fd:
     readme = fd.read()
 
+main_ns = {}
+ver_path = normpath('bindings/python/quokka/version.py')
+with open(ver_path) as ver_file:
+    exec(ver_file.read(), main_ns)
+
 setup(
     name="quokka-project",
-    version="0.5.1",
+    version=main_ns['__version__'],
     author="Alexis <dm> Challande",
     author_email="achallande@quarkslab.com",
     url="https://github.com/quarkslab/quokka",
     project_urls={
         "Documentation": "https://quarkslab.github.io/quokka/",
         "Bug Tracker": "https://github.com/quarkslab/quokka/issues",
         "Source": "https://github.com/quarkslab/quokka/",
```

