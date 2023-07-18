# Comparing `tmp/csbschema-1.0.4.tar.gz` & `tmp/csbschema-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csbschema-1.0.4.tar", last modified: Mon Apr 10 14:56:48 2023, max compression
+gzip compressed data, was "csbschema-1.0.5.tar", last modified: Tue Jul 18 19:28:30 2023, max compression
```

## Comparing `csbschema-1.0.4.tar` & `csbschema-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-04-10 14:56:48.831504 csbschema-1.0.4/
--rw-r--r--   0 miles      (505) staff       (20)     1143 2023-01-23 01:58:17.000000 csbschema-1.0.4/LICENSE.txt
--rw-r--r--   0 miles      (505) staff       (20)      213 2023-04-10 14:31:46.000000 csbschema-1.0.4/MANIFEST.in
--rw-r--r--   0 miles      (505) staff       (20)     4151 2023-04-10 14:56:48.831371 csbschema-1.0.4/PKG-INFO
--rw-r--r--   0 miles      (505) staff       (20)     3542 2023-04-10 14:31:46.000000 csbschema-1.0.4/README.md
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-04-10 14:56:48.828666 csbschema-1.0.4/csbschema/
--rw-r--r--   0 miles      (505) staff       (20)     1418 2023-04-10 14:31:46.000000 csbschema-1.0.4/csbschema/__init__.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-04-10 14:56:48.830011 csbschema-1.0.4/csbschema/cmd/
--rw-r--r--   0 miles      (505) staff       (20)      285 2023-01-23 01:58:17.000000 csbschema-1.0.4/csbschema/cmd/__init__.py
--rw-r--r--   0 miles      (505) staff       (20)     1360 2023-01-23 01:58:17.000000 csbschema-1.0.4/csbschema/cmd/__main__.py
--rw-r--r--   0 miles      (505) staff       (20)     1230 2023-02-15 18:16:21.000000 csbschema-1.0.4/csbschema/cmd/validate.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-04-10 14:56:48.831219 csbschema-1.0.4/csbschema/data/
--rw-r--r--   0 miles      (505) staff       (20)    22704 2023-04-10 14:31:46.000000 csbschema-1.0.4/csbschema/data/CSB-schema-3_0_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    20601 2023-04-10 14:31:46.000000 csbschema-1.0.4/csbschema/data/CSB-schema-3_1_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)    20519 2023-04-10 14:31:46.000000 csbschema-1.0.4/csbschema/data/CSB-schema-3_2_0-BETA.json
--rw-r--r--   0 miles      (505) staff       (20)    20280 2023-04-10 14:31:46.000000 csbschema-1.0.4/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
--rw-r--r--   0 miles      (505) staff       (20)        0 2023-03-08 19:42:06.000000 csbschema-1.0.4/csbschema/data/__init__.py
--rw-r--r--   0 miles      (505) staff       (20)    20153 2023-04-10 14:31:46.000000 csbschema-1.0.4/csbschema/validators.py
-drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-04-10 14:56:48.829508 csbschema-1.0.4/csbschema.egg-info/
--rw-r--r--   0 miles      (505) staff       (20)     4151 2023-04-10 14:56:48.000000 csbschema-1.0.4/csbschema.egg-info/PKG-INFO
--rw-r--r--   0 miles      (505) staff       (20)      580 2023-04-10 14:56:48.000000 csbschema-1.0.4/csbschema.egg-info/SOURCES.txt
--rw-r--r--   0 miles      (505) staff       (20)        1 2023-04-10 14:56:48.000000 csbschema-1.0.4/csbschema.egg-info/dependency_links.txt
--rw-r--r--   0 miles      (505) staff       (20)       58 2023-04-10 14:56:48.000000 csbschema-1.0.4/csbschema.egg-info/entry_points.txt
--rw-r--r--   0 miles      (505) staff       (20)      135 2023-04-10 14:56:48.000000 csbschema-1.0.4/csbschema.egg-info/requires.txt
--rw-r--r--   0 miles      (505) staff       (20)       10 2023-04-10 14:56:48.000000 csbschema-1.0.4/csbschema.egg-info/top_level.txt
--rw-r--r--   0 miles      (505) staff       (20)     1055 2023-04-10 14:51:54.000000 csbschema-1.0.4/pyproject.toml
--rw-r--r--   0 miles      (505) staff       (20)       38 2023-04-10 14:56:48.831543 csbschema-1.0.4/setup.cfg
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.276269 csbschema-1.0.5/
+-rw-r--r--   0 miles      (505) staff       (20)     1143 2023-01-23 01:58:17.000000 csbschema-1.0.5/LICENSE.txt
+-rw-r--r--   0 miles      (505) staff       (20)      213 2023-04-10 14:31:46.000000 csbschema-1.0.5/MANIFEST.in
+-rw-r--r--   0 miles      (505) staff       (20)     4268 2023-07-18 19:28:30.276134 csbschema-1.0.5/PKG-INFO
+-rw-r--r--   0 miles      (505) staff       (20)     3659 2023-07-18 19:26:57.000000 csbschema-1.0.5/README.md
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.272978 csbschema-1.0.5/csbschema/
+-rw-r--r--   0 miles      (505) staff       (20)     1418 2023-07-18 19:26:57.000000 csbschema-1.0.5/csbschema/__init__.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.274724 csbschema-1.0.5/csbschema/cmd/
+-rw-r--r--   0 miles      (505) staff       (20)      285 2023-01-23 01:58:17.000000 csbschema-1.0.5/csbschema/cmd/__init__.py
+-rw-r--r--   0 miles      (505) staff       (20)     1360 2023-01-23 01:58:17.000000 csbschema-1.0.5/csbschema/cmd/__main__.py
+-rw-r--r--   0 miles      (505) staff       (20)     1230 2023-02-15 18:16:21.000000 csbschema-1.0.5/csbschema/cmd/validate.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.275973 csbschema-1.0.5/csbschema/data/
+-rw-r--r--   0 miles      (505) staff       (20)    22704 2023-04-10 14:31:46.000000 csbschema-1.0.5/csbschema/data/CSB-schema-3_0_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    20601 2023-04-10 14:31:46.000000 csbschema-1.0.5/csbschema/data/CSB-schema-3_1_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)    20519 2023-04-10 14:31:46.000000 csbschema-1.0.5/csbschema/data/CSB-schema-3_2_0-BETA.json
+-rw-r--r--   0 miles      (505) staff       (20)    20280 2023-04-10 14:31:46.000000 csbschema-1.0.5/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json
+-rw-r--r--   0 miles      (505) staff       (20)        0 2023-03-08 19:42:06.000000 csbschema-1.0.5/csbschema/data/__init__.py
+-rw-r--r--   0 miles      (505) staff       (20)    20170 2023-07-18 19:26:57.000000 csbschema-1.0.5/csbschema/validators.py
+drwxr-xr-x   0 miles      (505) staff       (20)        0 2023-07-18 19:28:30.273917 csbschema-1.0.5/csbschema.egg-info/
+-rw-r--r--   0 miles      (505) staff       (20)     4268 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/PKG-INFO
+-rw-r--r--   0 miles      (505) staff       (20)      580 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/SOURCES.txt
+-rw-r--r--   0 miles      (505) staff       (20)        1 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/dependency_links.txt
+-rw-r--r--   0 miles      (505) staff       (20)       58 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/entry_points.txt
+-rw-r--r--   0 miles      (505) staff       (20)      135 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/requires.txt
+-rw-r--r--   0 miles      (505) staff       (20)       10 2023-07-18 19:28:30.000000 csbschema-1.0.5/csbschema.egg-info/top_level.txt
+-rw-r--r--   0 miles      (505) staff       (20)     1055 2023-04-10 14:51:54.000000 csbschema-1.0.5/pyproject.toml
+-rw-r--r--   0 miles      (505) staff       (20)       38 2023-07-18 19:28:30.276308 csbschema-1.0.5/setup.cfg
```

### Comparing `csbschema-1.0.4/LICENSE.txt` & `csbschema-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.4/PKG-INFO` & `csbschema-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csbschema
-Version: 1.0.4
+Version: 1.0.5
 Summary: JSON Schema and validator for IHO B-12 Crowdsourced Bathymetry metadata and data
 Author-email: Brian Miles <bmiles@ccom.unh.edu>, Brian Calder <brc@ccom.unh.edu>
 Project-URL: Homepage, https://github.com/CCOMJHC/csbschema
 Project-URL: Bug Tracker, https://github.com/CCOMJHC/csbschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,19 @@
 # csbschema
 
 `csbschema` defines a JSON Schema and validator (implemented in Pyhon) for 
 [IHO B-12 Crowdsourced Bathymetry](https://iho.int/uploads/user/pubs/Drafts/CSB-Guidance_Document-Edition_3.0.pdf) 
 metadata and data.
 
 # Installation
+To install from PyPi, first create a virtual environment for your project, then:
+```shell
+pip install csbschema
+```
+
 Clone or download this repository, then run:
 ```shell
 $ pip install .
 ```
 
 # Usage
 
@@ -73,17 +78,17 @@
 ```shell
 $ csbschema validate -f docs/IHO/b12_v3_2_0-BETA_example.json --version 3.2.0-BETA
 CSB data file 'docs/IHO/b12_v3_2_0-BETA_example.json' successfully validated against schema '3.2.0-BETA'.
 ```
 > Run `csbschema validate --help` for more information about validating against different versions of the schema.
 
 # Testing
-First, install csbschema with test dependencies:
+First, install test dependencies:
 ```shell
-$ pip install ".[test]"
+$ pip install -r requirements-test.txt
 ```
 
 Then run unit tests:
 ```shell
 $ pytest tests/unit/test_*.py
 ```
```

### Comparing `csbschema-1.0.4/README.md` & `csbschema-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 # csbschema
 
 `csbschema` defines a JSON Schema and validator (implemented in Pyhon) for 
 [IHO B-12 Crowdsourced Bathymetry](https://iho.int/uploads/user/pubs/Drafts/CSB-Guidance_Document-Edition_3.0.pdf) 
 metadata and data.
 
 # Installation
+To install from PyPi, first create a virtual environment for your project, then:
+```shell
+pip install csbschema
+```
+
 Clone or download this repository, then run:
 ```shell
 $ pip install .
 ```
 
 # Usage
 
@@ -58,17 +63,17 @@
 ```shell
 $ csbschema validate -f docs/IHO/b12_v3_2_0-BETA_example.json --version 3.2.0-BETA
 CSB data file 'docs/IHO/b12_v3_2_0-BETA_example.json' successfully validated against schema '3.2.0-BETA'.
 ```
 > Run `csbschema validate --help` for more information about validating against different versions of the schema.
 
 # Testing
-First, install csbschema with test dependencies:
+First, install test dependencies:
 ```shell
-$ pip install ".[test]"
+$ pip install -r requirements-test.txt
 ```
 
 Then run unit tests:
 ```shell
 $ pytest tests/unit/test_*.py
 ```
```

### Comparing `csbschema-1.0.4/csbschema/__init__.py` & `csbschema-1.0.5/csbschema/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import Tuple, Union
 
 from csbschema import validators
 
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
 
 
 B12_VERSION_3_0_0_2023_03 = '3.0.0-2023-03'
 XYZ_B12_VERSION_3_0_0_2023_03 = 'XYZ-3.0.0-2023-03'
 B12_VERSION_3_1_0_2023_03 = '3.1.0-2023-03'
 B12_VERSION_3_2_0_BETA = '3.2.0-BETA'
```

### Comparing `csbschema-1.0.4/csbschema/cmd/__main__.py` & `csbschema-1.0.5/csbschema/cmd/__main__.py`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.4/csbschema/cmd/validate.py` & `csbschema-1.0.5/csbschema/cmd/validate.py`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.4/csbschema/data/CSB-schema-3_0_0-2023-03.json` & `csbschema-1.0.5/csbschema/data/CSB-schema-3_0_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.4/csbschema/data/CSB-schema-3_1_0-2023-03.json` & `csbschema-1.0.5/csbschema/data/CSB-schema-3_1_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.4/csbschema/data/CSB-schema-3_2_0-BETA.json` & `csbschema-1.0.5/csbschema/data/CSB-schema-3_2_0-BETA.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.4/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json` & `csbschema-1.0.5/csbschema/data/XYZ-CSB-schema-3_0_0-2023-03.json`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.4/csbschema/validators.py` & `csbschema-1.0.5/csbschema/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 def _get_validator(schema_rsrc_name: str) -> Draft202012Validator:
     """
     :param schema_rsrc_name: Internal resource name of schema document to use for validation
     :return: Draft202012Validator instance
     """
     schema_path = _get_schema_file(schema_rsrc_name)
-    with schema_path.open('r') as f:
+    with schema_path.open('r', encoding='utf8') as f:
         schema = json.load(f)
     return jsonschema.Draft202012Validator(schema)
 
 
 def _open_document(document_path: Union[Path, str]) -> Union[dict, list]:
     with open(document_path, 'rb') as f:
         with mmap.mmap(f.fileno(), length=0, access=mmap.ACCESS_READ) as mm:
```

### Comparing `csbschema-1.0.4/csbschema.egg-info/PKG-INFO` & `csbschema-1.0.5/csbschema.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csbschema
-Version: 1.0.4
+Version: 1.0.5
 Summary: JSON Schema and validator for IHO B-12 Crowdsourced Bathymetry metadata and data
 Author-email: Brian Miles <bmiles@ccom.unh.edu>, Brian Calder <brc@ccom.unh.edu>
 Project-URL: Homepage, https://github.com/CCOMJHC/csbschema
 Project-URL: Bug Tracker, https://github.com/CCOMJHC/csbschema/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,19 @@
 # csbschema
 
 `csbschema` defines a JSON Schema and validator (implemented in Pyhon) for 
 [IHO B-12 Crowdsourced Bathymetry](https://iho.int/uploads/user/pubs/Drafts/CSB-Guidance_Document-Edition_3.0.pdf) 
 metadata and data.
 
 # Installation
+To install from PyPi, first create a virtual environment for your project, then:
+```shell
+pip install csbschema
+```
+
 Clone or download this repository, then run:
 ```shell
 $ pip install .
 ```
 
 # Usage
 
@@ -73,17 +78,17 @@
 ```shell
 $ csbschema validate -f docs/IHO/b12_v3_2_0-BETA_example.json --version 3.2.0-BETA
 CSB data file 'docs/IHO/b12_v3_2_0-BETA_example.json' successfully validated against schema '3.2.0-BETA'.
 ```
 > Run `csbschema validate --help` for more information about validating against different versions of the schema.
 
 # Testing
-First, install csbschema with test dependencies:
+First, install test dependencies:
 ```shell
-$ pip install ".[test]"
+$ pip install -r requirements-test.txt
 ```
 
 Then run unit tests:
 ```shell
 $ pytest tests/unit/test_*.py
 ```
```

### Comparing `csbschema-1.0.4/csbschema.egg-info/SOURCES.txt` & `csbschema-1.0.5/csbschema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csbschema-1.0.4/pyproject.toml` & `csbschema-1.0.5/pyproject.toml`

 * *Files identical despite different names*

