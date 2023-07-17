# Comparing `tmp/climatePy-0.4.33.tar.gz` & `tmp/climatePy-0.4.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.33.tar", last modified: Mon Jul 17 22:08:41 2023, max compression
+gzip compressed data, was "climatePy-0.4.34.tar", last modified: Mon Jul 17 22:39:15 2023, max compression
```

## Comparing `climatePy-0.4.33.tar` & `climatePy-0.4.34.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.430617 climatePy-0.4.33/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-17 22:08:37.000000 climatePy-0.4.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-17 22:08:41.430617 climatePy-0.4.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-17 22:08:37.000000 climatePy-0.4.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.386617 climatePy-0.4.33/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22670 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    63216 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    32241 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.386617 climatePy-0.4.33/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.386617 climatePy-0.4.33/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:08:41.430617 climatePy-0.4.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-17 22:08:39.000000 climatePy-0.4.33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.430617 climatePy-0.4.33/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:37.000000 climatePy-0.4.33/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-17 22:08:37.000000 climatePy-0.4.33/tests/test_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-17 22:08:37.000000 climatePy-0.4.33/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-17 22:08:37.000000 climatePy-0.4.33/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.495348 climatePy-0.4.34/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-17 22:39:12.000000 climatePy-0.4.34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-17 22:39:15.495348 climatePy-0.4.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-17 22:39:12.000000 climatePy-0.4.34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.451347 climatePy-0.4.34/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22670 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63216 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32241 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.451347 climatePy-0.4.34/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.451347 climatePy-0.4.34/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:39:15.495348 climatePy-0.4.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-17 22:39:14.000000 climatePy-0.4.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.495348 climatePy-0.4.34/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:12.000000 climatePy-0.4.34/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-17 22:39:12.000000 climatePy-0.4.34/tests/test_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-17 22:39:12.000000 climatePy-0.4.34/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-17 22:39:12.000000 climatePy-0.4.34/tests/test_utils.py
```

### Comparing `climatePy-0.4.33/LICENSE` & `climatePy-0.4.34/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/PKG-INFO` & `climatePy-0.4.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.33
+Version: 0.4.34
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.33/README.md` & `climatePy-0.4.34/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/climatePy/__init__.py` & `climatePy-0.4.34/climatePy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from ._climatepy_filter import climatepy_filter
 from ._dap import dap, dap_crop, dap_get
 from ._shortcuts import getTerraClim, getTerraClimNormals, getGridMET, getMACA, \
     get3DEP, getLOCA, getPRISM, getPolaris, \
     getBCCA, getLivneh, getLivneh_fluxes, getISRIC_soils, getDaymet, \
     getVIC, getNASADEM, getWorldClim, getCHIRPS, getLCMAP, getNLDAS, getGLDAS, getMODIS
 from ._netrc_utils import writeDodsrc, writeNetrc, getNetrcPath, getDodsrcPath, checkNetrc, checkDodsrc
+from ._extract_sites import extract_sites
 
 __all__ = [
     'params',
     'climatepy_filter',
     'dap',
     'dap_crop',
     'dap_get',
@@ -45,14 +46,15 @@
     'getNASADEM', 
     'getWorldClim', 
     'getCHIRPS', 
     'getLCMAP',
     'getNLDAS',
     'getGLDAS',
     'getMODIS',
+    'extract_sites',
     'writeDodsrc',
     'writeNetrc',
     'getNetrcPath',
     'getDodsrcPath',
     'checkNetrc',
     'checkDodsrc'
 ]
```

### Comparing `climatePy-0.4.33/climatePy/_climatepy_filter.py` & `climatePy-0.4.34/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/climatePy/_dap.py` & `climatePy-0.4.34/climatePy/_dap.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/climatePy/_extract_sites.py` & `climatePy-0.4.34/climatePy/_extract_sites.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/climatePy/_netrc_utils.py` & `climatePy-0.4.34/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/climatePy/_shortcuts.py` & `climatePy-0.4.34/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/climatePy/_utils.py` & `climatePy-0.4.34/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/climatePy/data/catalog.csv` & `climatePy-0.4.34/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.34/climatePy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.33
+Version: 0.4.34
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.33/setup.py` & `climatePy-0.4.34/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.33',
+    version='0.4.34',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.33/tests/test_extract_sites.py` & `climatePy-0.4.34/tests/test_extract_sites.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/tests/test_shortcuts.py` & `climatePy-0.4.34/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.33/tests/test_utils.py` & `climatePy-0.4.34/tests/test_utils.py`

 * *Files identical despite different names*

