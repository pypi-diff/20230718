# Comparing `tmp/SherLocking-0.0.1.tar.gz` & `tmp/SherLocking-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SherLocking-0.0.1.tar", last modified: Tue Jul 18 04:59:16 2023, max compression
+gzip compressed data, was "SherLocking-0.0.2.tar", last modified: Tue Jul 18 17:39:28 2023, max compression
```

## Comparing `SherLocking-0.0.1.tar` & `SherLocking-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 04:59:16.826159 SherLocking-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-07-18 04:42:39.000000 SherLocking-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      558 2023-07-18 04:59:16.825081 SherLocking-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-18 04:42:44.000000 SherLocking-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 04:59:16.790080 SherLocking-0.0.1/SherLocking/
--rw-rw-rw-   0        0        0       18 2023-07-18 04:50:34.000000 SherLocking-0.0.1/SherLocking/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-18 04:47:54.000000 SherLocking-0.0.1/SherLocking/main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 04:59:16.823083 SherLocking-0.0.1/SherLocking.egg-info/
--rw-rw-rw-   0        0        0      558 2023-07-18 04:59:16.000000 SherLocking-0.0.1/SherLocking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-18 04:59:16.000000 SherLocking-0.0.1/SherLocking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 04:59:16.000000 SherLocking-0.0.1/SherLocking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-18 04:59:16.000000 SherLocking-0.0.1/SherLocking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 04:59:16.826159 SherLocking-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      853 2023-07-18 04:54:49.000000 SherLocking-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:39:28.304547 SherLocking-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-07-18 04:42:39.000000 SherLocking-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      558 2023-07-18 17:39:28.304547 SherLocking-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-18 04:42:44.000000 SherLocking-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 17:39:28.237273 SherLocking-0.0.2/SherLocking/
+-rw-rw-rw-   0        0        0       24 2023-07-18 05:28:28.000000 SherLocking-0.0.2/SherLocking/__init__.py
+-rw-rw-rw-   0        0        0     5154 2023-07-18 17:37:47.000000 SherLocking-0.0.2/SherLocking/activation.py
+-rw-rw-rw-   0        0        0     1286 2023-07-18 06:53:24.000000 SherLocking-0.0.2/SherLocking/config.py
+-rw-rw-rw-   0        0        0     2140 2023-07-18 17:36:22.000000 SherLocking-0.0.2/SherLocking/file.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:39:28.304547 SherLocking-0.0.2/SherLocking.egg-info/
+-rw-rw-rw-   0        0        0      558 2023-07-18 17:39:27.000000 SherLocking-0.0.2/SherLocking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-18 17:39:28.000000 SherLocking-0.0.2/SherLocking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:39:27.000000 SherLocking-0.0.2/SherLocking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-18 17:39:27.000000 SherLocking-0.0.2/SherLocking.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 17:39:27.000000 SherLocking-0.0.2/SherLocking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:39:28.314688 SherLocking-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-07-18 17:38:28.000000 SherLocking-0.0.2/setup.py
```

### Comparing `SherLocking-0.0.1/PKG-INFO` & `SherLocking-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SherLocking
-Version: 0.0.1
+Version: 0.0.2
 Summary: Applies activation for any program.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python,locking,activation,trial,license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SherLocking-0.0.1/SherLocking.egg-info/PKG-INFO` & `SherLocking-0.0.2/SherLocking.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SherLocking
-Version: 0.0.1
+Version: 0.0.2
 Summary: Applies activation for any program.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python,locking,activation,trial,license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SherLocking-0.0.1/setup.py` & `SherLocking-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from setuptools import setup, find_packages
-import codecs
-import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Applies activation for any program.'
 LONG_DESCRIPTION = 'A package to apply activation required to run any program, like a license.'
 
 setup(
     name="SherLocking",
     version=VERSION,
     author="Armando Chaparro",
     author_email="<pylejandria@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[
-
+        'ttkbootstrap'
     ],
     keywords=['python', 'locking', 'activation', 'trial', 'license'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
```

