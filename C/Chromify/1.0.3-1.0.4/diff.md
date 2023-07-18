# Comparing `tmp/Chromify-1.0.3.tar.gz` & `tmp/Chromify-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chromify-1.0.3.tar", last modified: Tue Jul 18 12:15:51 2023, max compression
+gzip compressed data, was "Chromify-1.0.4.tar", last modified: Tue Jul 18 12:31:22 2023, max compression
```

## Comparing `Chromify-1.0.3.tar` & `Chromify-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 12:15:51.481371 Chromify-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-18 12:15:51.469263 Chromify-1.0.3/Chromify.egg-info/
--rw-rw-rw-   0        0        0     5118 2023-07-18 12:15:51.000000 Chromify-1.0.3/Chromify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-18 12:15:51.000000 Chromify-1.0.3/Chromify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 12:15:51.000000 Chromify-1.0.3/Chromify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-18 12:15:51.000000 Chromify-1.0.3/Chromify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5118 2023-07-18 12:15:51.480373 Chromify-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 12:15:51.478377 Chromify-1.0.3/lib/
--rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.0.3/lib/Color.py
--rw-rw-rw-   0        0        0     7865 2023-07-18 10:07:14.000000 Chromify-1.0.3/lib/Converter.py
--rw-rw-rw-   0        0        0      144 2023-07-18 12:15:40.000000 Chromify-1.0.3/lib/__init__.py
--rw-rw-rw-   0        0        0     6542 2023-07-18 10:22:00.000000 Chromify-1.0.3/lib/main.py
--rw-rw-rw-   0        0        0       42 2023-07-18 12:15:51.481371 Chromify-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-07-18 12:15:32.000000 Chromify-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:31:22.409989 Chromify-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-18 12:31:22.398876 Chromify-1.0.4/Chromify/
+-rw-rw-rw-   0        0        0     6542 2023-07-18 10:22:00.000000 Chromify-1.0.4/Chromify/Chromify.py
+-rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.0.4/Chromify/Color.py
+-rw-rw-rw-   0        0        0     7865 2023-07-18 10:07:14.000000 Chromify-1.0.4/Chromify/Converter.py
+-rw-rw-rw-   0        0        0      148 2023-07-18 12:31:16.000000 Chromify-1.0.4/Chromify/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:31:22.405901 Chromify-1.0.4/Chromify.egg-info/
+-rw-rw-rw-   0        0        0     5141 2023-07-18 12:31:22.000000 Chromify-1.0.4/Chromify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-18 12:31:22.000000 Chromify-1.0.4/Chromify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 12:31:22.000000 Chromify-1.0.4/Chromify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 12:31:22.000000 Chromify-1.0.4/Chromify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1292 2023-07-17 19:51:25.000000 Chromify-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5141 2023-07-18 12:31:22.408016 Chromify-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4489 2023-07-17 23:18:42.000000 Chromify-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 12:31:22.409989 Chromify-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-18 12:31:02.000000 Chromify-1.0.4/setup.py
```

### Comparing `Chromify-1.0.3/Chromify.egg-info/PKG-INFO` & `Chromify-1.0.4/Chromify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.0.3
+Version: 1.0.4
 Summary: Colorful Terminal Prints
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Chromify - Python Library Documentation
 
 Chromify is a Python library that provides functionalities for color manipulation and conversion. It allows you to convert between different color representations such as RGB, HEX, HSL, CMYK, and HSV, and perform various color operations.
 
 ![BANNER](https://github.com/plaraje/chromify/assets/61209614/e4906631-4315-4923-83de-df161fcc1bae)
```

### Comparing `Chromify-1.0.3/PKG-INFO` & `Chromify-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.0.3
+Version: 1.0.4
 Summary: Colorful Terminal Prints
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Chromify - Python Library Documentation
 
 Chromify is a Python library that provides functionalities for color manipulation and conversion. It allows you to convert between different color representations such as RGB, HEX, HSL, CMYK, and HSV, and perform various color operations.
 
 ![BANNER](https://github.com/plaraje/chromify/assets/61209614/e4906631-4315-4923-83de-df161fcc1bae)
```

### Comparing `Chromify-1.0.3/lib/Color.py` & `Chromify-1.0.4/Chromify/Color.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.3/lib/Converter.py` & `Chromify-1.0.4/Chromify/Converter.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.3/lib/main.py` & `Chromify-1.0.4/Chromify/Chromify.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.3/setup.py` & `Chromify-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
-with open('docs/README.md', 'r', encoding='utf-8') as f:
+with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Chromify',
-    version='1.0.3',
+    version='1.0.4',
     author='Plaraje',
     author_email='mat.demoya@gmail.com',
     description='Colorful Terminal Prints',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

