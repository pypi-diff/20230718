# Comparing `tmp/experiment-config-0.21.tar.gz` & `tmp/experiment-config-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-config-0.21.tar", last modified: Tue Jul 18 01:39:52 2023, max compression
+gzip compressed data, was "experiment-config-0.22.tar", last modified: Tue Jul 18 01:46:03 2023, max compression
```

## Comparing `experiment-config-0.21.tar` & `experiment-config-0.22.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.501080 experiment-config-0.21/
--rw-r--r--   0 ahalev     (502) staff       (20)     1073 2023-01-29 22:38:50.000000 experiment-config-0.21/LICENSE.txt
--rw-r--r--   0 ahalev     (502) staff       (20)     9190 2023-07-18 01:39:52.500814 experiment-config-0.21/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)     8789 2023-05-31 22:41:55.000000 experiment-config-0.21/README.md
--rw-r--r--   0 ahalev     (502) staff       (20)       38 2023-07-18 01:39:52.501133 experiment-config-0.21/setup.cfg
--rw-r--r--   0 ahalev     (502) staff       (20)      930 2023-07-18 01:20:43.000000 experiment-config-0.21/setup.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.497728 experiment-config-0.21/src/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.498987 experiment-config-0.21/src/experiment_config.egg-info/
--rw-r--r--   0 ahalev     (502) staff       (20)     9190 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)      411 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/SOURCES.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/dependency_links.txt
--rw-r--r--   0 ahalev     (502) staff       (20)       28 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/requires.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        7 2023-07-18 01:39:52.000000 experiment-config-0.21/src/experiment_config.egg-info/top_level.txt
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.499678 experiment-config-0.21/src/expfig/
--rw-r--r--   0 ahalev     (502) staff       (20)      138 2023-05-31 22:41:55.000000 experiment-config-0.21/src/expfig/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     8349 2023-07-18 01:16:28.000000 experiment-config-0.21/src/expfig/fig.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:39:52.500576 experiment-config-0.21/src/expfig/logging/
--rw-r--r--   0 ahalev     (502) staff       (20)       76 2023-07-16 23:55:34.000000 experiment-config-0.21/src/expfig/logging/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1905 2023-07-17 20:30:35.000000 experiment-config-0.21/src/expfig/logging/log_dir.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1018 2023-07-16 23:55:34.000000 experiment-config-0.21/src/expfig/logging/logger.py
--rw-r--r--   0 ahalev     (502) staff       (20)     6919 2023-07-18 01:15:42.000000 experiment-config-0.21/src/expfig/namespacify.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:46:03.000885 experiment-config-0.22/
+-rw-r--r--   0 ahalev     (502) staff       (20)     1073 2023-01-29 22:38:50.000000 experiment-config-0.22/LICENSE.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)     9201 2023-07-18 01:46:03.000631 experiment-config-0.22/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)     8789 2023-05-31 22:41:55.000000 experiment-config-0.22/README.md
+-rw-r--r--   0 ahalev     (502) staff       (20)       38 2023-07-18 01:46:03.000925 experiment-config-0.22/setup.cfg
+-rw-r--r--   0 ahalev     (502) staff       (20)      947 2023-07-18 01:44:46.000000 experiment-config-0.22/setup.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:46:02.997888 experiment-config-0.22/src/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:46:02.999038 experiment-config-0.22/src/experiment_config.egg-info/
+-rw-r--r--   0 ahalev     (502) staff       (20)     9201 2023-07-18 01:46:02.000000 experiment-config-0.22/src/experiment_config.egg-info/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)      411 2023-07-18 01:46:02.000000 experiment-config-0.22/src/experiment_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2023-07-18 01:46:02.000000 experiment-config-0.22/src/experiment_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)       28 2023-07-18 01:46:02.000000 experiment-config-0.22/src/experiment_config.egg-info/requires.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        7 2023-07-18 01:46:02.000000 experiment-config-0.22/src/experiment_config.egg-info/top_level.txt
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:46:02.999727 experiment-config-0.22/src/expfig/
+-rw-r--r--   0 ahalev     (502) staff       (20)      138 2023-05-31 22:41:55.000000 experiment-config-0.22/src/expfig/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     8349 2023-07-18 01:16:28.000000 experiment-config-0.22/src/expfig/fig.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-07-18 01:46:03.000408 experiment-config-0.22/src/expfig/logging/
+-rw-r--r--   0 ahalev     (502) staff       (20)       76 2023-07-16 23:55:34.000000 experiment-config-0.22/src/expfig/logging/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1905 2023-07-17 20:30:35.000000 experiment-config-0.22/src/expfig/logging/log_dir.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1018 2023-07-16 23:55:34.000000 experiment-config-0.22/src/expfig/logging/logger.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     6919 2023-07-18 01:15:42.000000 experiment-config-0.22/src/expfig/namespacify.py
```

### Comparing `experiment-config-0.21/LICENSE.txt` & `experiment-config-0.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `experiment-config-0.21/PKG-INFO` & `experiment-config-0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: experiment-config
-Version: 0.21
+Version: 0.22
 Summary: A yaml-based configuration for reproducible python experiments.
 Maintainer: Avishai Halev
 Maintainer-email: avishaihalev@gmail.com
 License: MIT License
-Project-URL: Source Code, https://github.com/ahalev/experiment-config
+Project-URL: Source Code, https://github.com/ahalev/experiment-config/tree/v0.22
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 ## Installation
```

### Comparing `experiment-config-0.21/README.md` & `experiment-config-0.22/README.md`

 * *Files identical despite different names*

### Comparing `experiment-config-0.21/setup.py` & `experiment-config-0.22/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'A yaml-based configuration for reproducible python experiments.'
-VERSION = '0.21'
+VERSION = '0.22'
 MAINTAINER = 'Avishai Halev'
 MAINTAINER_EMAIL = 'avishaihalev@gmail.com'
 LICENSE = 'MIT License'
 PROJECT_URLS = {
-    'Source Code': 'https://github.com/ahalev/experiment-config'
+    'Source Code': f'https://github.com/ahalev/experiment-config/tree/v{VERSION}'
 }
 EXTRAS = {
     'dev': ['pytest']
 }
 
 setup(
     name='experiment-config',
```

### Comparing `experiment-config-0.21/src/experiment_config.egg-info/PKG-INFO` & `experiment-config-0.22/src/experiment_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: experiment-config
-Version: 0.21
+Version: 0.22
 Summary: A yaml-based configuration for reproducible python experiments.
 Maintainer: Avishai Halev
 Maintainer-email: avishaihalev@gmail.com
 License: MIT License
-Project-URL: Source Code, https://github.com/ahalev/experiment-config
+Project-URL: Source Code, https://github.com/ahalev/experiment-config/tree/v0.22
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 ## Installation
```

### Comparing `experiment-config-0.21/src/expfig/fig.py` & `experiment-config-0.22/src/expfig/fig.py`

 * *Files identical despite different names*

### Comparing `experiment-config-0.21/src/expfig/logging/log_dir.py` & `experiment-config-0.22/src/expfig/logging/log_dir.py`

 * *Files identical despite different names*

### Comparing `experiment-config-0.21/src/expfig/logging/logger.py` & `experiment-config-0.22/src/expfig/logging/logger.py`

 * *Files identical despite different names*

### Comparing `experiment-config-0.21/src/expfig/namespacify.py` & `experiment-config-0.22/src/expfig/namespacify.py`

 * *Files identical despite different names*

