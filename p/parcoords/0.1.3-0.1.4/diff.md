# Comparing `tmp/parcoords-0.1.3.tar.gz` & `tmp/parcoords-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parcoords-0.1.3.tar", last modified: Mon Jul  3 16:39:09 2023, max compression
+gzip compressed data, was "parcoords-0.1.4.tar", last modified: Tue Jul 18 13:44:30 2023, max compression
```

## Comparing `parcoords-0.1.3.tar` & `parcoords-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:39:09.469583 parcoords-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 16:38:59.000000 parcoords-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-03 16:39:09.469583 parcoords-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-03 16:38:59.000000 parcoords-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:39:09.465583 parcoords-0.1.3/parcoords/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 16:38:59.000000 parcoords-0.1.3/parcoords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-03 16:38:59.000000 parcoords-0.1.3/parcoords/parcoords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:39:09.469583 parcoords-0.1.3/parcoords.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:39:09.469583 parcoords-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-03 16:38:59.000000 parcoords-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:44:30.946907 parcoords-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-18 13:44:20.000000 parcoords-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-18 13:44:30.946907 parcoords-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-18 13:44:20.000000 parcoords-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:44:30.942907 parcoords-0.1.4/parcoords/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 13:44:20.000000 parcoords-0.1.4/parcoords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-18 13:44:20.000000 parcoords-0.1.4/parcoords/parcoords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:44:30.946907 parcoords-0.1.4/parcoords.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-18 13:44:30.000000 parcoords-0.1.4/parcoords.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-18 13:44:30.000000 parcoords-0.1.4/parcoords.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:44:30.000000 parcoords-0.1.4/parcoords.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 13:44:30.000000 parcoords-0.1.4/parcoords.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 13:44:30.000000 parcoords-0.1.4/parcoords.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:44:30.946907 parcoords-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-18 13:44:20.000000 parcoords-0.1.4/setup.py
```

### Comparing `parcoords-0.1.3/LICENSE.txt` & `parcoords-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `parcoords-0.1.3/PKG-INFO` & `parcoords-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parcoords
-Version: 0.1.3
+Version: 0.1.4
 Summary: Parallel coordinates plotting
 Home-page: https://github.com/VoigtPeter/parcoords
 Author: Peter Voigt
 License: MIT
 Project-URL: Documentation, https://voigtpeter.github.io/parcoords/index.html
 Project-URL: Source, https://github.com/VoigtPeter/parcoords
 Keywords: parallel coordinates,parallel-coordinates,plot,hyperparameter,visualization
```

### Comparing `parcoords-0.1.3/README.md` & `parcoords-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `parcoords-0.1.3/parcoords/parcoords.py` & `parcoords-0.1.4/parcoords/parcoords.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     if axs is None:
         # initialize figure and axes
         fig, axs = plt.subplots(
             1,
             no_of_cols - 1,
             figsize=figsize,
             sharey="none",
+            gridspec_kw=dict(wspace=0),
         )
         axs = np.append(axs, axs[-1].twinx())
 
         # calculate limits from data & transform nominal columns
         ylims = []
         for i, (column, ax) in enumerate(zip(values, axs)):
             if not all(isinstance(item, (int, float)) for item in column):
```

### Comparing `parcoords-0.1.3/parcoords.egg-info/PKG-INFO` & `parcoords-0.1.4/parcoords.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parcoords
-Version: 0.1.3
+Version: 0.1.4
 Summary: Parallel coordinates plotting
 Home-page: https://github.com/VoigtPeter/parcoords
 Author: Peter Voigt
 License: MIT
 Project-URL: Documentation, https://voigtpeter.github.io/parcoords/index.html
 Project-URL: Source, https://github.com/VoigtPeter/parcoords
 Keywords: parallel coordinates,parallel-coordinates,plot,hyperparameter,visualization
```

### Comparing `parcoords-0.1.3/setup.py` & `parcoords-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import setuptools
 
 
 setuptools.setup(
     name="parcoords",
-    version="0.1.3",
+    version="0.1.4",
     author="Peter Voigt",
     url="https://github.com/VoigtPeter/parcoords",
     project_urls={
         "Documentation": "https://voigtpeter.github.io/parcoords/index.html",
         "Source": "https://github.com/VoigtPeter/parcoords",
     },
     packages=["parcoords"],
```

