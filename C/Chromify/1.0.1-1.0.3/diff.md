# Comparing `tmp/Chromify-1.0.1.tar.gz` & `tmp/Chromify-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chromify-1.0.1.tar", last modified: Tue Jul 18 11:28:55 2023, max compression
+gzip compressed data, was "Chromify-1.0.3.tar", last modified: Tue Jul 18 12:15:51 2023, max compression
```

## Comparing `Chromify-1.0.1.tar` & `Chromify-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 11:28:55.057359 Chromify-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-18 11:28:55.036574 Chromify-1.0.1/Chromify.egg-info/
--rw-rw-rw-   0        0        0     5118 2023-07-18 11:28:54.000000 Chromify-1.0.1/Chromify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-07-18 11:28:54.000000 Chromify-1.0.1/Chromify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 11:28:54.000000 Chromify-1.0.1/Chromify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-18 11:28:54.000000 Chromify-1.0.1/Chromify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5118 2023-07-18 11:28:55.055226 Chromify-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 11:28:55.048153 Chromify-1.0.1/lib/
--rw-rw-rw-   0        0        0     6542 2023-07-18 10:22:00.000000 Chromify-1.0.1/lib/Chromify.py
--rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.0.1/lib/Color.py
--rw-rw-rw-   0        0        0     7865 2023-07-18 10:07:14.000000 Chromify-1.0.1/lib/Converter.py
--rw-rw-rw-   0        0        0      148 2023-07-18 11:28:38.000000 Chromify-1.0.1/lib/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-18 11:28:55.058357 Chromify-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-07-18 11:28:16.000000 Chromify-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:15:51.481371 Chromify-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-18 12:15:51.469263 Chromify-1.0.3/Chromify.egg-info/
+-rw-rw-rw-   0        0        0     5118 2023-07-18 12:15:51.000000 Chromify-1.0.3/Chromify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-18 12:15:51.000000 Chromify-1.0.3/Chromify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 12:15:51.000000 Chromify-1.0.3/Chromify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-18 12:15:51.000000 Chromify-1.0.3/Chromify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5118 2023-07-18 12:15:51.480373 Chromify-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 12:15:51.478377 Chromify-1.0.3/lib/
+-rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.0.3/lib/Color.py
+-rw-rw-rw-   0        0        0     7865 2023-07-18 10:07:14.000000 Chromify-1.0.3/lib/Converter.py
+-rw-rw-rw-   0        0        0      144 2023-07-18 12:15:40.000000 Chromify-1.0.3/lib/__init__.py
+-rw-rw-rw-   0        0        0     6542 2023-07-18 10:22:00.000000 Chromify-1.0.3/lib/main.py
+-rw-rw-rw-   0        0        0       42 2023-07-18 12:15:51.481371 Chromify-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-07-18 12:15:32.000000 Chromify-1.0.3/setup.py
```

### Comparing `Chromify-1.0.1/Chromify.egg-info/PKG-INFO` & `Chromify-1.0.3/Chromify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.0.1
+Version: 1.0.3
 Summary: Colorful Terminal Prints
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Chromify-1.0.1/PKG-INFO` & `Chromify-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.0.1
+Version: 1.0.3
 Summary: Colorful Terminal Prints
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Chromify-1.0.1/lib/Chromify.py` & `Chromify-1.0.3/lib/main.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.1/lib/Color.py` & `Chromify-1.0.3/lib/Color.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.1/lib/Converter.py` & `Chromify-1.0.3/lib/Converter.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.1/setup.py` & `Chromify-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('docs/README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Chromify',
-    version='1.0.1',
+    version='1.0.3',
     author='Plaraje',
     author_email='mat.demoya@gmail.com',
     description='Colorful Terminal Prints',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

