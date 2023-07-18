# Comparing `tmp/SherLocking-0.0.4.tar.gz` & `tmp/SherLocking-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SherLocking-0.0.4.tar", last modified: Tue Jul 18 21:19:40 2023, max compression
+gzip compressed data, was "SherLocking-0.0.5.tar", last modified: Tue Jul 18 21:22:53 2023, max compression
```

## Comparing `SherLocking-0.0.4.tar` & `SherLocking-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 21:19:40.827936 SherLocking-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-07-18 04:42:39.000000 SherLocking-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      558 2023-07-18 21:19:40.827936 SherLocking-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-18 04:42:44.000000 SherLocking-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 21:19:40.801928 SherLocking-0.0.4/SherLocking/
--rw-rw-rw-   0        0        0      102 2023-07-18 21:18:26.000000 SherLocking-0.0.4/SherLocking/__init__.py
--rw-rw-rw-   0        0        0     5218 2023-07-18 17:50:11.000000 SherLocking-0.0.4/SherLocking/activation.py
--rw-rw-rw-   0        0        0     1286 2023-07-18 06:53:24.000000 SherLocking-0.0.4/SherLocking/config.py
--rw-rw-rw-   0        0        0     1824 2023-07-18 17:58:37.000000 SherLocking-0.0.4/SherLocking/file.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:19:40.812265 SherLocking-0.0.4/SherLocking.egg-info/
--rw-rw-rw-   0        0        0      558 2023-07-18 21:19:40.000000 SherLocking-0.0.4/SherLocking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-07-18 21:19:40.000000 SherLocking-0.0.4/SherLocking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 21:19:40.000000 SherLocking-0.0.4/SherLocking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-18 21:19:40.000000 SherLocking-0.0.4/SherLocking.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-18 21:19:40.000000 SherLocking-0.0.4/SherLocking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 21:19:40.827936 SherLocking-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-07-18 21:19:37.000000 SherLocking-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:22:53.049213 SherLocking-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-07-18 04:42:39.000000 SherLocking-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      558 2023-07-18 21:22:53.049213 SherLocking-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-18 04:42:44.000000 SherLocking-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 21:22:53.023516 SherLocking-0.0.5/SherLocking/
+-rw-rw-rw-   0        0        0      102 2023-07-18 21:18:26.000000 SherLocking-0.0.5/SherLocking/__init__.py
+-rw-rw-rw-   0        0        0     5218 2023-07-18 17:50:11.000000 SherLocking-0.0.5/SherLocking/activation.py
+-rw-rw-rw-   0        0        0     1286 2023-07-18 06:53:24.000000 SherLocking-0.0.5/SherLocking/config.py
+-rw-rw-rw-   0        0        0     1836 2023-07-18 21:21:38.000000 SherLocking-0.0.5/SherLocking/file.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:22:53.049213 SherLocking-0.0.5/SherLocking.egg-info/
+-rw-rw-rw-   0        0        0      558 2023-07-18 21:22:52.000000 SherLocking-0.0.5/SherLocking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-18 21:22:52.000000 SherLocking-0.0.5/SherLocking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 21:22:52.000000 SherLocking-0.0.5/SherLocking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-18 21:22:52.000000 SherLocking-0.0.5/SherLocking.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 21:22:52.000000 SherLocking-0.0.5/SherLocking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 21:22:53.049213 SherLocking-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-07-18 21:22:07.000000 SherLocking-0.0.5/setup.py
```

### Comparing `SherLocking-0.0.4/PKG-INFO` & `SherLocking-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SherLocking
-Version: 0.0.4
+Version: 0.0.5
 Summary: Applies activation for any program.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python,locking,activation,trial,license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SherLocking-0.0.4/SherLocking/activation.py` & `SherLocking-0.0.5/SherLocking/activation.py`

 * *Files identical despite different names*

### Comparing `SherLocking-0.0.4/SherLocking/config.py` & `SherLocking-0.0.5/SherLocking/config.py`

 * *Files identical despite different names*

### Comparing `SherLocking-0.0.4/SherLocking/file.py` & `SherLocking-0.0.5/SherLocking/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import time
-from config import Config
+from SherLocking.config import Config
 
 
 class File:
     def __init__(self, path: str):
         
         # PROPERTIES
         self.path = path
```

### Comparing `SherLocking-0.0.4/SherLocking.egg-info/PKG-INFO` & `SherLocking-0.0.5/SherLocking.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SherLocking
-Version: 0.0.4
+Version: 0.0.5
 Summary: Applies activation for any program.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python,locking,activation,trial,license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SherLocking-0.0.4/setup.py` & `SherLocking-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Applies activation for any program.'
 LONG_DESCRIPTION = 'A package to apply activation required to run any program, like a license.'
 
 setup(
     name="SherLocking",
     version=VERSION,
     author="Armando Chaparro",
```

