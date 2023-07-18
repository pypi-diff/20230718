# Comparing `tmp/dqfit-0.1.2.tar.gz` & `tmp/dqfit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqfit-0.1.2.tar", last modified: Tue Jul 18 14:55:11 2023, max compression
+gzip compressed data, was "dqfit-0.1.3.tar", last modified: Tue Jul 18 15:02:27 2023, max compression
```

## Comparing `dqfit-0.1.2.tar` & `dqfit-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,50 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:55:11.171248 dqfit-0.1.2/
--rw-r--r--   0 parker     (501) staff       (20)       11 2023-07-18 14:46:45.000000 dqfit-0.1.2/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)     3895 2023-07-18 14:55:11.171108 dqfit-0.1.2/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     3643 2023-07-18 14:46:48.000000 dqfit-0.1.2/README.md
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:55:11.164959 dqfit-0.1.2/dqfit/
--rw-r--r--   0 parker     (501) staff       (20)      817 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:55:11.163512 dqfit-0.1.2/dqfit/data/
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:55:11.166576 dqfit-0.1.2/dqfit/data/context/
--rw-r--r--   0 parker     (501) staff       (20)     7309 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/data/context/COLE.json
--rw-r--r--   0 parker     (501) staff       (20)   104281 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/data/context/hello-world.json
--rw-r--r--   0 parker     (501) staff       (20)      628 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/data/context/patient-demographic.json
--rw-r--r--   0 parker     (501) staff       (20)      170 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/data/context/systolic.json
--rw-r--r--   0 parker     (501) staff       (20)   125219 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/data/context/uscdi.json
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:55:11.163620 dqfit-0.1.2/dqfit/data/synthetic/
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:55:11.166781 dqfit-0.1.2/dqfit/data/synthetic/synthea_1/
--rw-r--r--   0 parker     (501) staff       (20)    10600 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_1/hello-world-bundle.json
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:55:11.170721 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/
--rw-r--r--   0 parker     (501) staff       (20)   448345 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Aaron697_Veum823_f11ade6b-fae3-c20d-0a46-e344db669410.json
--rw-r--r--   0 parker     (501) staff       (20)  1853828 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Abdul218_Gislason620_81469779-7e7f-4864-6fdc-41e52a68ba80.json
--rw-r--r--   0 parker     (501) staff       (20)   250797 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Addie421_Weber641_6d7ea981-c548-3d1e-0b59-ba2acbb149d2.json
--rw-r--r--   0 parker     (501) staff       (20)   313530 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Adele475_Barton704_4d604ebf-23a9-7a3f-affe-ec4c69f1644d.json
--rw-r--r--   0 parker     (501) staff       (20)   514069 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Adena533_Rice937_3470129b-6f4d-27d6-b25b-65a2903514b6.json
--rw-r--r--   0 parker     (501) staff       (20)   406074 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Adina377_Barton704_5bde62b3-df9f-623d-e6f8-bd335bc02dc0.json
--rw-r--r--   0 parker     (501) staff       (20)   608466 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Adrian111_Collins926_c9e3828c-7466-5f82-a675-213e088c6e7c.json
--rw-r--r--   0 parker     (501) staff       (20)   252925 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Agustin437_Russel238_fc56a4f3-04d6-364a-5131-803138497da1.json
--rw-r--r--   0 parker     (501) staff       (20)   689780 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Aida517_Spencer878_87bc62d9-7a08-3ecf-0723-d3d918698e0c.json
--rw-r--r--   0 parker     (501) staff       (20)   449052 2023-07-18 14:46:45.000000 dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Aileen250_Bahringer146_5cc757f3-f20b-e88f-c23e-5faee619e6ac.json
--rw-r--r--   0 parker     (501) staff       (20)     9164 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/dimensions.py
--rw-r--r--   0 parker     (501) staff       (20)      928 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)     2994 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/io.py
--rw-r--r--   0 parker     (501) staff       (20)     6045 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/model.py
--rw-r--r--   0 parker     (501) staff       (20)     3341 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/population.py
--rw-r--r--   0 parker     (501) staff       (20)     3065 2023-07-18 14:46:48.000000 dqfit-0.1.2/dqfit/transform.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:55:11.165826 dqfit-0.1.2/dqfit.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)     3895 2023-07-18 14:55:11.000000 dqfit-0.1.2/dqfit.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1472 2023-07-18 14:55:11.000000 dqfit-0.1.2/dqfit.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-18 14:55:11.000000 dqfit-0.1.2/dqfit.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)       61 2023-07-18 14:55:11.000000 dqfit-0.1.2/dqfit.egg-info/requires.txt
--rw-r--r--   0 parker     (501) staff       (20)        6 2023-07-18 14:55:11.000000 dqfit-0.1.2/dqfit.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      457 2023-07-18 14:55:04.000000 dqfit-0.1.2/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-18 14:55:11.171280 dqfit-0.1.2/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      141 2023-07-18 14:46:45.000000 dqfit-0.1.2/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 15:02:27.475533 dqfit-0.1.3/
+-rw-r--r--   0 parker     (501) staff       (20)       11 2023-07-18 14:46:45.000000 dqfit-0.1.3/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)     3895 2023-07-18 15:02:27.475384 dqfit-0.1.3/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     3643 2023-07-18 14:46:48.000000 dqfit-0.1.3/README.md
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 15:02:27.467886 dqfit-0.1.3/dqfit/
+-rw-r--r--   0 parker     (501) staff       (20)      843 2023-07-18 14:58:50.000000 dqfit-0.1.3/dqfit/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 15:02:27.469486 dqfit-0.1.3/dqfit/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)     1516 2023-07-18 14:59:56.000000 dqfit-0.1.3/dqfit/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    12001 2023-07-18 14:59:56.000000 dqfit-0.1.3/dqfit/__pycache__/dimensions.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2159 2023-07-18 14:59:57.000000 dqfit-0.1.3/dqfit/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6028 2023-07-18 14:59:57.000000 dqfit-0.1.3/dqfit/__pycache__/io.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     9974 2023-07-18 14:59:57.000000 dqfit-0.1.3/dqfit/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5971 2023-07-18 14:59:57.000000 dqfit-0.1.3/dqfit/__pycache__/population.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3637 2023-07-18 14:59:57.000000 dqfit-0.1.3/dqfit/__pycache__/transform.cpython-311.pyc
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 15:02:27.465427 dqfit-0.1.3/dqfit/data/
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 15:02:27.470343 dqfit-0.1.3/dqfit/data/context/
+-rw-r--r--   0 parker     (501) staff       (20)     7309 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/data/context/COLE.json
+-rw-r--r--   0 parker     (501) staff       (20)   104281 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/data/context/hello-world.json
+-rw-r--r--   0 parker     (501) staff       (20)      628 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/data/context/patient-demographic.json
+-rw-r--r--   0 parker     (501) staff       (20)      170 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/data/context/systolic.json
+-rw-r--r--   0 parker     (501) staff       (20)   125219 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/data/context/uscdi.json
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 15:02:27.465524 dqfit-0.1.3/dqfit/data/synthetic/
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 15:02:27.470699 dqfit-0.1.3/dqfit/data/synthetic/synthea_1/
+-rw-r--r--   0 parker     (501) staff       (20)    10600 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_1/hello-world-bundle.json
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 15:02:27.474971 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/
+-rw-r--r--   0 parker     (501) staff       (20)   448345 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Aaron697_Veum823_f11ade6b-fae3-c20d-0a46-e344db669410.json
+-rw-r--r--   0 parker     (501) staff       (20)  1853828 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Abdul218_Gislason620_81469779-7e7f-4864-6fdc-41e52a68ba80.json
+-rw-r--r--   0 parker     (501) staff       (20)   250797 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Addie421_Weber641_6d7ea981-c548-3d1e-0b59-ba2acbb149d2.json
+-rw-r--r--   0 parker     (501) staff       (20)   313530 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Adele475_Barton704_4d604ebf-23a9-7a3f-affe-ec4c69f1644d.json
+-rw-r--r--   0 parker     (501) staff       (20)   514069 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Adena533_Rice937_3470129b-6f4d-27d6-b25b-65a2903514b6.json
+-rw-r--r--   0 parker     (501) staff       (20)   406074 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Adina377_Barton704_5bde62b3-df9f-623d-e6f8-bd335bc02dc0.json
+-rw-r--r--   0 parker     (501) staff       (20)   608466 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Adrian111_Collins926_c9e3828c-7466-5f82-a675-213e088c6e7c.json
+-rw-r--r--   0 parker     (501) staff       (20)   252925 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Agustin437_Russel238_fc56a4f3-04d6-364a-5131-803138497da1.json
+-rw-r--r--   0 parker     (501) staff       (20)   689780 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Aida517_Spencer878_87bc62d9-7a08-3ecf-0723-d3d918698e0c.json
+-rw-r--r--   0 parker     (501) staff       (20)   449052 2023-07-18 14:46:45.000000 dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Aileen250_Bahringer146_5cc757f3-f20b-e88f-c23e-5faee619e6ac.json
+-rw-r--r--   0 parker     (501) staff       (20)     9164 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/dimensions.py
+-rw-r--r--   0 parker     (501) staff       (20)      928 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)     2994 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/io.py
+-rw-r--r--   0 parker     (501) staff       (20)     6045 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/model.py
+-rw-r--r--   0 parker     (501) staff       (20)     3341 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/population.py
+-rw-r--r--   0 parker     (501) staff       (20)     3065 2023-07-18 14:46:48.000000 dqfit-0.1.3/dqfit/transform.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 15:02:27.468679 dqfit-0.1.3/dqfit.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)     3895 2023-07-18 15:02:27.000000 dqfit-0.1.3/dqfit.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1768 2023-07-18 15:02:27.000000 dqfit-0.1.3/dqfit.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-18 15:02:27.000000 dqfit-0.1.3/dqfit.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)       61 2023-07-18 15:02:27.000000 dqfit-0.1.3/dqfit.egg-info/requires.txt
+-rw-r--r--   0 parker     (501) staff       (20)        6 2023-07-18 15:02:27.000000 dqfit-0.1.3/dqfit.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      457 2023-07-18 15:02:10.000000 dqfit-0.1.3/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-18 15:02:27.475566 dqfit-0.1.3/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      141 2023-07-18 14:46:45.000000 dqfit-0.1.3/setup.py
```

### Comparing `dqfit-0.1.2/PKG-INFO` & `dqfit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqfit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data Quality Fitness Index Tool
 Author: Parker Holcomb
 Project-URL: Homepage, https://github.com/clinicalqualitydata/dqfit-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Quickstart:
```

### Comparing `dqfit-0.1.2/README.md` & `dqfit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/__init__.py` & `dqfit-0.1.3/dqfit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 from typing import List
 
-from dotenv import load_dotenv
+from dotenv import load_dotenv, find_dotenv
 
-load_dotenv()
+load_dotenv(find_dotenv())
 
 from dqfit.dimensions import Complete, Conformant, Plausible, Recent
 from dqfit.io import (get_bundle_paths, load_context, read_bundle_resources,
                       read_fhir)
 from dqfit.model import Index
 from dqfit.transform import transform_to_fhir_path
```

### Comparing `dqfit-0.1.2/dqfit/data/context/COLE.json` & `dqfit-0.1.3/dqfit/data/context/COLE.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/context/hello-world.json` & `dqfit-0.1.3/dqfit/data/context/hello-world.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/context/patient-demographic.json` & `dqfit-0.1.3/dqfit/data/context/patient-demographic.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/context/uscdi.json` & `dqfit-0.1.3/dqfit/data/context/uscdi.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_1/hello-world-bundle.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_1/hello-world-bundle.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Aaron697_Veum823_f11ade6b-fae3-c20d-0a46-e344db669410.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Aaron697_Veum823_f11ade6b-fae3-c20d-0a46-e344db669410.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Abdul218_Gislason620_81469779-7e7f-4864-6fdc-41e52a68ba80.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Abdul218_Gislason620_81469779-7e7f-4864-6fdc-41e52a68ba80.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Addie421_Weber641_6d7ea981-c548-3d1e-0b59-ba2acbb149d2.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Addie421_Weber641_6d7ea981-c548-3d1e-0b59-ba2acbb149d2.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Adele475_Barton704_4d604ebf-23a9-7a3f-affe-ec4c69f1644d.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Adele475_Barton704_4d604ebf-23a9-7a3f-affe-ec4c69f1644d.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Adena533_Rice937_3470129b-6f4d-27d6-b25b-65a2903514b6.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Adena533_Rice937_3470129b-6f4d-27d6-b25b-65a2903514b6.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Adina377_Barton704_5bde62b3-df9f-623d-e6f8-bd335bc02dc0.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Adina377_Barton704_5bde62b3-df9f-623d-e6f8-bd335bc02dc0.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Adrian111_Collins926_c9e3828c-7466-5f82-a675-213e088c6e7c.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Adrian111_Collins926_c9e3828c-7466-5f82-a675-213e088c6e7c.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Agustin437_Russel238_fc56a4f3-04d6-364a-5131-803138497da1.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Agustin437_Russel238_fc56a4f3-04d6-364a-5131-803138497da1.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Aida517_Spencer878_87bc62d9-7a08-3ecf-0723-d3d918698e0c.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Aida517_Spencer878_87bc62d9-7a08-3ecf-0723-d3d918698e0c.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/data/synthetic/synthea_10/Aileen250_Bahringer146_5cc757f3-f20b-e88f-c23e-5faee619e6ac.json` & `dqfit-0.1.3/dqfit/data/synthetic/synthea_10/Aileen250_Bahringer146_5cc757f3-f20b-e88f-c23e-5faee619e6ac.json`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/dimensions.py` & `dqfit-0.1.3/dqfit/dimensions.py`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/helpers.py` & `dqfit-0.1.3/dqfit/helpers.py`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/io.py` & `dqfit-0.1.3/dqfit/io.py`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/model.py` & `dqfit-0.1.3/dqfit/model.py`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/population.py` & `dqfit-0.1.3/dqfit/population.py`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit/transform.py` & `dqfit-0.1.3/dqfit/transform.py`

 * *Files identical despite different names*

### Comparing `dqfit-0.1.2/dqfit.egg-info/PKG-INFO` & `dqfit-0.1.3/dqfit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqfit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data Quality Fitness Index Tool
 Author: Parker Holcomb
 Project-URL: Homepage, https://github.com/clinicalqualitydata/dqfit-python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Quickstart:
```

### Comparing `dqfit-0.1.2/dqfit.egg-info/SOURCES.txt` & `dqfit-0.1.3/dqfit.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 dqfit/population.py
 dqfit/transform.py
 dqfit.egg-info/PKG-INFO
 dqfit.egg-info/SOURCES.txt
 dqfit.egg-info/dependency_links.txt
 dqfit.egg-info/requires.txt
 dqfit.egg-info/top_level.txt
+dqfit/__pycache__/__init__.cpython-311.pyc
+dqfit/__pycache__/dimensions.cpython-311.pyc
+dqfit/__pycache__/helpers.cpython-311.pyc
+dqfit/__pycache__/io.cpython-311.pyc
+dqfit/__pycache__/model.cpython-311.pyc
+dqfit/__pycache__/population.cpython-311.pyc
+dqfit/__pycache__/transform.cpython-311.pyc
 dqfit/data/context/COLE.json
 dqfit/data/context/hello-world.json
 dqfit/data/context/patient-demographic.json
 dqfit/data/context/systolic.json
 dqfit/data/context/uscdi.json
 dqfit/data/synthetic/synthea_1/hello-world-bundle.json
 dqfit/data/synthetic/synthea_10/Aaron697_Veum823_f11ade6b-fae3-c20d-0a46-e344db669410.json
```

