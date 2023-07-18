# Comparing `tmp/mathjson-solver-1.6.0.tar.gz` & `tmp/mathjson-solver-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathjson-solver-1.6.0.tar", last modified: Tue May 30 10:10:05 2023, max compression
+gzip compressed data, was "mathjson-solver-1.6.1.tar", last modified: Tue Jul 18 04:58:32 2023, max compression
```

## Comparing `mathjson-solver-1.6.0.tar` & `mathjson-solver-1.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/
--rw-rw-r--   0 martins   (1000) martins   (1000)     1071 2022-05-02 08:10:45.000000 mathjson-solver-1.6.0/LICENSE
--rw-rw-r--   0 martins   (1000) martins   (1000)     7111 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/PKG-INFO
--rw-rw-r--   0 martins   (1000) martins   (1000)     6582 2023-05-22 07:13:26.000000 mathjson-solver-1.6.0/README.md
--rw-rw-r--   0 martins   (1000) martins   (1000)       85 2022-05-02 14:01:31.000000 mathjson-solver-1.6.0/pyproject.toml
--rw-rw-r--   0 martins   (1000) martins   (1000)      654 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/setup.cfg
--rw-rw-r--   0 martins   (1000) martins   (1000)      829 2023-05-30 10:07:07.000000 mathjson-solver-1.6.0/setup.py
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/src/
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/src/mathjson_solver/
--rw-rw-r--   0 martins   (1000) martins   (1000)      102 2022-05-23 07:31:11.000000 mathjson-solver-1.6.0/src/mathjson_solver/__init__.py
--rw-rw-r--   0 martins   (1000) martins   (1000)     8486 2023-05-30 10:04:14.000000 mathjson-solver-1.6.0/src/mathjson_solver/__main__.py
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/
--rw-rw-r--   0 martins   (1000) martins   (1000)     7111 2023-05-30 10:10:05.000000 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/PKG-INFO
--rw-rw-r--   0 martins   (1000) martins   (1000)      313 2023-05-30 10:10:05.000000 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/SOURCES.txt
--rw-rw-r--   0 martins   (1000) martins   (1000)        1 2023-05-30 10:10:05.000000 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/dependency_links.txt
--rw-rw-r--   0 martins   (1000) martins   (1000)       16 2023-05-30 10:10:05.000000 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/top_level.txt
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/tests/
--rw-rw-r--   0 martins   (1000) martins   (1000)     7571 2023-05-30 10:06:48.000000 mathjson-solver-1.6.0/tests/test_with_pytest.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     1071 2022-05-02 08:10:45.000000 mathjson-solver-1.6.1/LICENSE
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7867 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/PKG-INFO
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7338 2023-07-18 04:55:26.000000 mathjson-solver-1.6.1/README.md
+-rw-rw-r--   0 martins   (1000) martins   (1000)       85 2022-05-02 14:01:31.000000 mathjson-solver-1.6.1/pyproject.toml
+-rw-rw-r--   0 martins   (1000) martins   (1000)      654 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/setup.cfg
+-rw-rw-r--   0 martins   (1000) martins   (1000)      829 2023-07-18 04:37:12.000000 mathjson-solver-1.6.1/setup.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.349267 mathjson-solver-1.6.1/src/
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/src/mathjson_solver/
+-rw-rw-r--   0 martins   (1000) martins   (1000)      102 2022-05-23 07:31:11.000000 mathjson-solver-1.6.1/src/mathjson_solver/__init__.py
+-rw-rw-r--   0 martins   (1000) martins   (1000)     8671 2023-07-18 04:35:03.000000 mathjson-solver-1.6.1/src/mathjson_solver/__main__.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7867 2023-07-18 04:58:32.000000 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/PKG-INFO
+-rw-rw-r--   0 martins   (1000) martins   (1000)      313 2023-07-18 04:58:32.000000 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martins   (1000) martins   (1000)        1 2023-07-18 04:58:32.000000 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martins   (1000) martins   (1000)       16 2023-07-18 04:58:32.000000 mathjson-solver-1.6.1/src/mathjson_solver.egg-info/top_level.txt
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-07-18 04:58:32.353267 mathjson-solver-1.6.1/tests/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7852 2023-07-18 04:36:34.000000 mathjson-solver-1.6.1/tests/test_with_pytest.py
```

### Comparing `mathjson-solver-1.6.0/LICENSE` & `mathjson-solver-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mathjson-solver-1.6.0/PKG-INFO` & `mathjson-solver-1.6.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathjson-solver
-Version: 1.6.0
+Version: 1.6.1
 Summary: Utilities for MathJSON evaluation
 Home-page: https://github.com/LongenesisLtd/mathjson-solver
 Author: Martins Mednis
 Author-email: mrt@mednis.info
 Project-URL: Bug Tracker, https://github.com/LongenesisLtd/mathjson-solver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -93,17 +93,26 @@
 * `Equal`
 * `Greater`
 * `GreaterEqual`
 * `Less`
 * `LessEqual`
 * `NotEqual`
 
+### Membership operators
+* `In`
+* `NotIn`
+* `ContainsAnyOf`
+* `ContainsAllOf`
+* `ContainsNoneOf`
+
 ### Typecasting
+* `Str`
 * `Int`
 * `Float`
+* `Not`
 
 ### Additional constructs
 * `Constants`
 
 
 ## Examples
 ```python
@@ -131,24 +140,38 @@
 ["Round", -5.123456]              # -5
 ["Array", 1, 2]                   # ["Array", 1, 2]
 
 ["Max", ["Array", 1, 2, 3, 5, 2]] # 5
 ["Max", ["Array", 1, 2, ["Sum", 2, 4, 3], 5, 2]]  # 9
 ["Median", ["Array", 1, 2, 3, 5, 2]]              # 2
 ["Average", ["Array", 1, 2, 3, 5, 2]]             # 2.6
+["Average", ["Array"]]                            # None
+
 ["Length", ["Array", 1, 2, 3, 5, 2, 9]]           # 6
 ["Length", ["Array"]]                             # 0
 ["Any", ["Array", 0, 0, False, 0, 0]]             # False
 ["Any", ["Array", 0, 1, False, 0, 0]]             # True
 ["All", ["Array", 0, 1, False, 0, 0]]             # False
 ["All", ["Array", 0, 1, False, "", 0]]            # False
 ["All", ["Array", 2, 1, True, "zz", 2]]           # True
 ["Int", "12"]                     # 12
 ["Int", "12.2"]                   # 12
 ["Float", "12.2"]                 # 12.2
+["Str", 12]                       # "12"
+["Str", "12"]                     # "12"
+["Str", "aabb"]                   # "aabb"
+["Not", True]                      # False
+["Not", 0]                         # True
+
+["In", 2, ["Array", 1, 2, 3]]     # True
+["In", 4, ["Array", 1, 2, 3]]     # False
+["ContainsAnyOf", ["Array", 1, 2, 3], ["Array", 3, 4, 5, 6]]     # True
+["ContainsAnyOf", ["Array", 1, 2, 3], ["Array", 4, 5, 6]]        # False
+["ContainsAllOf", ["Array", 1, 2, 3], ["Array", 1, 2, 3]]        # True
+["ContainsAllOf", ["Array", 1, 2], ["Array", 1, 2, 3]]           # False
 ```
 
 ### Constants
 ```
 [
     "Constants",
     ["constant_name1", <expression>],
```

### Comparing `mathjson-solver-1.6.0/README.md` & `mathjson-solver-1.6.1/src/mathjson_solver.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: mathjson-solver
+Version: 1.6.1
+Summary: Utilities for MathJSON evaluation
+Home-page: https://github.com/LongenesisLtd/mathjson-solver
+Author: Martins Mednis
+Author-email: mrt@mednis.info
+Project-URL: Bug Tracker, https://github.com/LongenesisLtd/mathjson-solver/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MathJSON Solver
 
 [![Gitter](https://badges.gitter.im/mathjson-solver/community.svg)](https://gitter.im/mathjson-solver/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 _MathJSON Solver_ is a Python module to numerically evaluate MathJSON expressions. It was created by [Longenesis](https://longenesis.com/team) to add numerical evaluation capability of user generated mathematical expressions in Longenesis digital health products and later released as open source project. Its development was inspired by [CortexJS](https://cortexjs.io/compute-engine/) Compute Engine.
 
 Please ask questions and share feedback in our Gitter chat [https://gitter.im/mathjson-solver/community](https://gitter.im/mathjson-solver/community).
@@ -78,17 +93,26 @@
 * `Equal`
 * `Greater`
 * `GreaterEqual`
 * `Less`
 * `LessEqual`
 * `NotEqual`
 
+### Membership operators
+* `In`
+* `NotIn`
+* `ContainsAnyOf`
+* `ContainsAllOf`
+* `ContainsNoneOf`
+
 ### Typecasting
+* `Str`
 * `Int`
 * `Float`
+* `Not`
 
 ### Additional constructs
 * `Constants`
 
 
 ## Examples
 ```python
@@ -116,24 +140,38 @@
 ["Round", -5.123456]              # -5
 ["Array", 1, 2]                   # ["Array", 1, 2]
 
 ["Max", ["Array", 1, 2, 3, 5, 2]] # 5
 ["Max", ["Array", 1, 2, ["Sum", 2, 4, 3], 5, 2]]  # 9
 ["Median", ["Array", 1, 2, 3, 5, 2]]              # 2
 ["Average", ["Array", 1, 2, 3, 5, 2]]             # 2.6
+["Average", ["Array"]]                            # None
+
 ["Length", ["Array", 1, 2, 3, 5, 2, 9]]           # 6
 ["Length", ["Array"]]                             # 0
 ["Any", ["Array", 0, 0, False, 0, 0]]             # False
 ["Any", ["Array", 0, 1, False, 0, 0]]             # True
 ["All", ["Array", 0, 1, False, 0, 0]]             # False
 ["All", ["Array", 0, 1, False, "", 0]]            # False
 ["All", ["Array", 2, 1, True, "zz", 2]]           # True
 ["Int", "12"]                     # 12
 ["Int", "12.2"]                   # 12
 ["Float", "12.2"]                 # 12.2
+["Str", 12]                       # "12"
+["Str", "12"]                     # "12"
+["Str", "aabb"]                   # "aabb"
+["Not", True]                      # False
+["Not", 0]                         # True
+
+["In", 2, ["Array", 1, 2, 3]]     # True
+["In", 4, ["Array", 1, 2, 3]]     # False
+["ContainsAnyOf", ["Array", 1, 2, 3], ["Array", 3, 4, 5, 6]]     # True
+["ContainsAnyOf", ["Array", 1, 2, 3], ["Array", 4, 5, 6]]        # False
+["ContainsAllOf", ["Array", 1, 2, 3], ["Array", 1, 2, 3]]        # True
+["ContainsAllOf", ["Array", 1, 2], ["Array", 1, 2, 3]]           # False
 ```
 
 ### Constants
 ```
 [
     "Constants",
     ["constant_name1", <expression>],
```

### Comparing `mathjson-solver-1.6.0/setup.cfg` & `mathjson-solver-1.6.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mathjson-solver
-version = 1.6.0
+version = 1.6.1
 author = Martins Mednis
 author_email = mrt@mednis.info
 description = Utilities for MathJSON evaluation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/LongenesisLtd/mathjson-solver
 project_urls =
```

### Comparing `mathjson-solver-1.6.0/setup.py` & `mathjson-solver-1.6.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mathjson-solver",
-    version="1.6.0",
+    version="1.6.1",
     author="Martins Mednis",
     author_email="mrt@mednis.info",
     description="Utilities for MathJSON evaluation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LongenesisLtd/mathjson-solver",
     project_urls={
```

### Comparing `mathjson-solver-1.6.0/src/mathjson_solver/__main__.py` & `mathjson-solver-1.6.1/src/mathjson_solver/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -225,14 +225,18 @@
                 "All": All,
                 "Array": Arr,
                 "In": In,
                 "Not_in": Not_in,
                 "Contains_any_of": Contains_any_of,
                 "Contains_all_of": Contains_all_of,
                 "Contains_none_of": Contains_none_of,
+                "NotIn": Not_in,
+                "ContainsAnyOf": Contains_any_of,
+                "ContainsAllOf": Contains_all_of,
+                "ContainsNoneOf": Contains_none_of,
                 "Int": Int,
                 "Float": Float,
                 "Str": Str,
                 "Not": Not,
             }
             if s[0] in constructs:
                 try:
```

### Comparing `mathjson-solver-1.6.0/src/mathjson_solver.egg-info/PKG-INFO` & `mathjson-solver-1.6.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: mathjson-solver
-Version: 1.6.0
-Summary: Utilities for MathJSON evaluation
-Home-page: https://github.com/LongenesisLtd/mathjson-solver
-Author: Martins Mednis
-Author-email: mrt@mednis.info
-Project-URL: Bug Tracker, https://github.com/LongenesisLtd/mathjson-solver/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MathJSON Solver
 
 [![Gitter](https://badges.gitter.im/mathjson-solver/community.svg)](https://gitter.im/mathjson-solver/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 _MathJSON Solver_ is a Python module to numerically evaluate MathJSON expressions. It was created by [Longenesis](https://longenesis.com/team) to add numerical evaluation capability of user generated mathematical expressions in Longenesis digital health products and later released as open source project. Its development was inspired by [CortexJS](https://cortexjs.io/compute-engine/) Compute Engine.
 
 Please ask questions and share feedback in our Gitter chat [https://gitter.im/mathjson-solver/community](https://gitter.im/mathjson-solver/community).
@@ -93,17 +78,26 @@
 * `Equal`
 * `Greater`
 * `GreaterEqual`
 * `Less`
 * `LessEqual`
 * `NotEqual`
 
+### Membership operators
+* `In`
+* `NotIn`
+* `ContainsAnyOf`
+* `ContainsAllOf`
+* `ContainsNoneOf`
+
 ### Typecasting
+* `Str`
 * `Int`
 * `Float`
+* `Not`
 
 ### Additional constructs
 * `Constants`
 
 
 ## Examples
 ```python
@@ -131,24 +125,38 @@
 ["Round", -5.123456]              # -5
 ["Array", 1, 2]                   # ["Array", 1, 2]
 
 ["Max", ["Array", 1, 2, 3, 5, 2]] # 5
 ["Max", ["Array", 1, 2, ["Sum", 2, 4, 3], 5, 2]]  # 9
 ["Median", ["Array", 1, 2, 3, 5, 2]]              # 2
 ["Average", ["Array", 1, 2, 3, 5, 2]]             # 2.6
+["Average", ["Array"]]                            # None
+
 ["Length", ["Array", 1, 2, 3, 5, 2, 9]]           # 6
 ["Length", ["Array"]]                             # 0
 ["Any", ["Array", 0, 0, False, 0, 0]]             # False
 ["Any", ["Array", 0, 1, False, 0, 0]]             # True
 ["All", ["Array", 0, 1, False, 0, 0]]             # False
 ["All", ["Array", 0, 1, False, "", 0]]            # False
 ["All", ["Array", 2, 1, True, "zz", 2]]           # True
 ["Int", "12"]                     # 12
 ["Int", "12.2"]                   # 12
 ["Float", "12.2"]                 # 12.2
+["Str", 12]                       # "12"
+["Str", "12"]                     # "12"
+["Str", "aabb"]                   # "aabb"
+["Not", True]                      # False
+["Not", 0]                         # True
+
+["In", 2, ["Array", 1, 2, 3]]     # True
+["In", 4, ["Array", 1, 2, 3]]     # False
+["ContainsAnyOf", ["Array", 1, 2, 3], ["Array", 3, 4, 5, 6]]     # True
+["ContainsAnyOf", ["Array", 1, 2, 3], ["Array", 4, 5, 6]]        # False
+["ContainsAllOf", ["Array", 1, 2, 3], ["Array", 1, 2, 3]]        # True
+["ContainsAllOf", ["Array", 1, 2], ["Array", 1, 2, 3]]           # False
 ```
 
 ### Constants
 ```
 [
     "Constants",
     ["constant_name1", <expression>],
```

### Comparing `mathjson-solver-1.6.0/tests/test_with_pytest.py` & `mathjson-solver-1.6.1/tests/test_with_pytest.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             ["In", ["Add", "a", "b"], ["Array", 1, 2, ["Add", 15, 16], 4]],
             False,
         ),
         ({"a": [10, 20, 30]}, ["In", 20, "a"], True),
         ({"a": [10, 20, 30]}, ["In", 21, "a"], False),
         ({}, ["Not_in", 2, ["Array", 1, 2, 3]], False),
         ({}, ["Not_in", 4, ["Array", 1, 2, 3]], True),
+        ({}, ["NotIn", 4, ["Array", 1, 2, 3]], True),
         ({"a": [10, 20, 30]}, ["Not_in", 20, "a"], False),
         ({"a": [10, 20, 30]}, ["Not_in", 21, "a"], True),
         ({}, ["Contains_any_of", ["Array", 1, 2, 3], ["Array", 1, 2, 3]], True),
         ({}, ["Contains_any_of", ["Array", 2, 3], ["Array", 1, 2]], True),
         ({}, ["Contains_any_of", ["Array", 1, 2, 3], ["Array", 3, 4, 5, 6]], True),
         ({}, ["Contains_any_of", ["Array", 1, 2, 3], ["Array", 4, 5, 6]], False),
         (
@@ -136,24 +137,27 @@
                 ["Array", 1, ["Add", 1, 1], 3],
                 ["Array", 4, 5, ["Add", 3, 3]],
             ],
             False,
         ),
         ({"a": [10, 20, 30]}, ["Contains_any_of", "a", ["Array", 1, 20, 3]], True),
         ({"b": [1, 20, 3]}, ["Contains_any_of", ["Array", 1, 2, 3], "b"], True),
+        ({"b": [1, 20, 3]}, ["ContainsAnyOf", ["Array", 1, 2, 3], "b"], True),
         ({"a": [10, 20, 30], "b": [1, 20, 3]}, ["Contains_any_of", "a", "b"], True),
         ({"a": [10, 20, 30], "b": [1, 2, 3]}, ["Contains_any_of", "a", "b"], False),
         ({}, ["Contains_all_of", ["Array", 1, 2, 3], ["Array", 1, 2, 3]], True),
         ({}, ["Contains_all_of", ["Array", 1, 2], ["Array", 1, 2, 3]], False),
         ({}, ["Contains_all_of", ["Array", 1, 2, 3], ["Array", 1, 2]], True),
         ({}, ["Contains_all_of", ["Array", 1, 2, 3], ["Array", 2]], True),
+        ({}, ["ContainsAllOf", ["Array", 1, 2, 3], ["Array", 2]], True),
         ({"a": [10, 20, 30], "b": [1, 20, 3]}, ["Contains_all_of", "a", "b"], False),
         ({"a": [1, 2, 3], "b": [1, 2]}, ["Contains_all_of", "a", "b"], True),
         ({}, ["Contains_none_of", ["Array", 1, 2, 3], ["Array", 1, 2, 3]], False),
         ({}, ["Contains_none_of", ["Array", 1, 2], ["Array", 2, 3]], False),
+        ({}, ["ContainsNoneOf", ["Array", 1, 2], ["Array", 2, 3]], False),
         ({}, ["Contains_none_of", ["Array", 1, 2, 3], ["Array", 4, 5]], True),
         ({}, ["Not", True], False),
         ({}, ["Not", 0], True),
         ({}, ["Not", ["In", 2, ["Array", 1, 2, 3]]], False),
     ],
 )
 def test_solver_simple(parameters, expression, expected_result):
```

