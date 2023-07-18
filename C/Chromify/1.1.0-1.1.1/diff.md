# Comparing `tmp/Chromify-1.1.0.tar.gz` & `tmp/Chromify-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chromify-1.1.0.tar", last modified: Tue Jul 18 12:47:04 2023, max compression
+gzip compressed data, was "Chromify-1.1.1.tar", last modified: Tue Jul 18 12:48:47 2023, max compression
```

## Comparing `Chromify-1.1.0.tar` & `Chromify-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 12:47:04.825023 Chromify-1.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-18 12:47:04.810896 Chromify-1.1.0/Chromify/
--rw-rw-rw-   0        0        0     6544 2023-07-18 12:34:11.000000 Chromify-1.1.0/Chromify/Chromify.py
--rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.1.0/Chromify/Color.py
--rw-rw-rw-   0        0        0     7866 2023-07-18 12:34:17.000000 Chromify-1.1.0/Chromify/Converter.py
--rw-rw-rw-   0        0        0      148 2023-07-18 12:46:47.000000 Chromify-1.1.0/Chromify/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:47:04.822023 Chromify-1.1.0/Chromify.egg-info/
--rw-rw-rw-   0        0        0     8637 2023-07-18 12:47:04.000000 Chromify-1.1.0/Chromify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-18 12:47:04.000000 Chromify-1.1.0/Chromify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 12:47:04.000000 Chromify-1.1.0/Chromify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 12:47:04.000000 Chromify-1.1.0/Chromify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1292 2023-07-17 19:51:25.000000 Chromify-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     8637 2023-07-18 12:47:04.825023 Chromify-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7915 2023-07-18 12:45:47.000000 Chromify-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 12:47:04.826023 Chromify-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-07-18 12:46:59.000000 Chromify-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:48:47.123782 Chromify-1.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-18 12:48:47.113650 Chromify-1.1.1/Chromify/
+-rw-rw-rw-   0        0        0     6544 2023-07-18 12:34:11.000000 Chromify-1.1.1/Chromify/Chromify.py
+-rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.1.1/Chromify/Color.py
+-rw-rw-rw-   0        0        0     7866 2023-07-18 12:34:17.000000 Chromify-1.1.1/Chromify/Converter.py
+-rw-rw-rw-   0        0        0      148 2023-07-18 12:48:36.000000 Chromify-1.1.1/Chromify/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:48:47.120781 Chromify-1.1.1/Chromify.egg-info/
+-rw-rw-rw-   0        0        0     8643 2023-07-18 12:48:47.000000 Chromify-1.1.1/Chromify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-18 12:48:47.000000 Chromify-1.1.1/Chromify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 12:48:47.000000 Chromify-1.1.1/Chromify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 12:48:47.000000 Chromify-1.1.1/Chromify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1292 2023-07-17 19:51:25.000000 Chromify-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     8643 2023-07-18 12:48:47.122799 Chromify-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7918 2023-07-18 12:48:26.000000 Chromify-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 12:48:47.123782 Chromify-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-18 12:48:42.000000 Chromify-1.1.1/setup.py
```

### Comparing `Chromify-1.1.0/Chromify/Chromify.py` & `Chromify-1.1.1/Chromify/Chromify.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.1.0/Chromify/Color.py` & `Chromify-1.1.1/Chromify/Color.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.1.0/Chromify/Converter.py` & `Chromify-1.1.1/Chromify/Converter.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.1.0/Chromify.egg-info/PKG-INFO` & `Chromify-1.1.1/Chromify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.1.0
+Version: 1.1.1
 Summary: Colorful Terminal Prints
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -189,16 +189,19 @@
 {myArray[5].FORE}#############################
 """
 print(myString)
 ```
 
 #### Steps Return Values
 `"rgb"`: Returns the array with rgb touples that are compatible with Color class (Default).
+
 `"fore_esc"`: Returns the array with escape strings to color the foreground.
+
 `"back_esc"`: Returns the array with escape strings to color the background.
+
 `"color"`: Returns the array with Color objects that are compatible with Color class (Default if an invalid value is given). 
 
 # License
 
 MIT License
 
 Copyright (c) 2023 Plaraje
```

### Comparing `Chromify-1.1.0/LICENSE` & `Chromify-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Chromify-1.1.0/PKG-INFO` & `Chromify-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.1.0
+Version: 1.1.1
 Summary: Colorful Terminal Prints
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -189,16 +189,19 @@
 {myArray[5].FORE}#############################
 """
 print(myString)
 ```
 
 #### Steps Return Values
 `"rgb"`: Returns the array with rgb touples that are compatible with Color class (Default).
+
 `"fore_esc"`: Returns the array with escape strings to color the foreground.
+
 `"back_esc"`: Returns the array with escape strings to color the background.
+
 `"color"`: Returns the array with Color objects that are compatible with Color class (Default if an invalid value is given). 
 
 # License
 
 MIT License
 
 Copyright (c) 2023 Plaraje
```

### Comparing `Chromify-1.1.0/README.md` & `Chromify-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -174,16 +174,19 @@
 {myArray[5].FORE}#############################
 """
 print(myString)
 ```
 
 #### Steps Return Values
 `"rgb"`: Returns the array with rgb touples that are compatible with Color class (Default).
+
 `"fore_esc"`: Returns the array with escape strings to color the foreground.
+
 `"back_esc"`: Returns the array with escape strings to color the background.
+
 `"color"`: Returns the array with Color objects that are compatible with Color class (Default if an invalid value is given). 
 
 # License
 
 MIT License
 
 Copyright (c) 2023 Plaraje
```

### Comparing `Chromify-1.1.0/setup.py` & `Chromify-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Chromify',
-    version='1.1.0',
+    version='1.1.1',
     author='Plaraje',
     author_email='mat.demoya@gmail.com',
     description='Colorful Terminal Prints',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

