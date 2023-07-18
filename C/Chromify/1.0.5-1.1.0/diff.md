# Comparing `tmp/Chromify-1.0.5.tar.gz` & `tmp/Chromify-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chromify-1.0.5.tar", last modified: Tue Jul 18 12:34:45 2023, max compression
+gzip compressed data, was "Chromify-1.1.0.tar", last modified: Tue Jul 18 12:47:04 2023, max compression
```

## Comparing `Chromify-1.0.5.tar` & `Chromify-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 12:34:45.236430 Chromify-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-18 12:34:45.227324 Chromify-1.0.5/Chromify/
--rw-rw-rw-   0        0        0     6544 2023-07-18 12:34:11.000000 Chromify-1.0.5/Chromify/Chromify.py
--rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.0.5/Chromify/Color.py
--rw-rw-rw-   0        0        0     7866 2023-07-18 12:34:17.000000 Chromify-1.0.5/Chromify/Converter.py
--rw-rw-rw-   0        0        0      148 2023-07-18 12:34:24.000000 Chromify-1.0.5/Chromify/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:34:45.234431 Chromify-1.0.5/Chromify.egg-info/
--rw-rw-rw-   0        0        0     5141 2023-07-18 12:34:45.000000 Chromify-1.0.5/Chromify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-18 12:34:45.000000 Chromify-1.0.5/Chromify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 12:34:45.000000 Chromify-1.0.5/Chromify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 12:34:45.000000 Chromify-1.0.5/Chromify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1292 2023-07-17 19:51:25.000000 Chromify-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     5141 2023-07-18 12:34:45.236430 Chromify-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4489 2023-07-17 23:18:42.000000 Chromify-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 12:34:45.237430 Chromify-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-07-18 12:34:38.000000 Chromify-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:47:04.825023 Chromify-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-07-18 12:47:04.810896 Chromify-1.1.0/Chromify/
+-rw-rw-rw-   0        0        0     6544 2023-07-18 12:34:11.000000 Chromify-1.1.0/Chromify/Chromify.py
+-rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.1.0/Chromify/Color.py
+-rw-rw-rw-   0        0        0     7866 2023-07-18 12:34:17.000000 Chromify-1.1.0/Chromify/Converter.py
+-rw-rw-rw-   0        0        0      148 2023-07-18 12:46:47.000000 Chromify-1.1.0/Chromify/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:47:04.822023 Chromify-1.1.0/Chromify.egg-info/
+-rw-rw-rw-   0        0        0     8637 2023-07-18 12:47:04.000000 Chromify-1.1.0/Chromify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-18 12:47:04.000000 Chromify-1.1.0/Chromify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 12:47:04.000000 Chromify-1.1.0/Chromify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 12:47:04.000000 Chromify-1.1.0/Chromify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1292 2023-07-17 19:51:25.000000 Chromify-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8637 2023-07-18 12:47:04.825023 Chromify-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7915 2023-07-18 12:45:47.000000 Chromify-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 12:47:04.826023 Chromify-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-18 12:46:59.000000 Chromify-1.1.0/setup.py
```

### Comparing `Chromify-1.0.5/Chromify/Chromify.py` & `Chromify-1.1.0/Chromify/Chromify.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.5/Chromify/Color.py` & `Chromify-1.1.0/Chromify/Color.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.5/Chromify/Converter.py` & `Chromify-1.1.0/Chromify/Converter.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.5/LICENSE` & `Chromify-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.5/setup.py` & `Chromify-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Chromify',
-    version='1.0.5',
+    version='1.1.0',
     author='Plaraje',
     author_email='mat.demoya@gmail.com',
     description='Colorful Terminal Prints',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

