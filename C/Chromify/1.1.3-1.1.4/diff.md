# Comparing `tmp/Chromify-1.1.3.tar.gz` & `tmp/Chromify-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chromify-1.1.3.tar", last modified: Tue Jul 18 14:17:20 2023, max compression
+gzip compressed data, was "Chromify-1.1.4.tar", last modified: Tue Jul 18 14:39:12 2023, max compression
```

## Comparing `Chromify-1.1.3.tar` & `Chromify-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 14:17:20.091568 Chromify-1.1.3/
-drwxrwxrwx   0        0        0        0 2023-07-18 14:17:19.767131 Chromify-1.1.3/Chromify/
--rw-rw-rw-   0        0        0     6544 2023-07-18 13:26:56.000000 Chromify-1.1.3/Chromify/Chromify.py
--rw-rw-rw-   0        0        0    16090 2023-07-18 13:26:56.000000 Chromify-1.1.3/Chromify/Color.py
--rw-rw-rw-   0        0        0     7866 2023-07-18 13:37:52.000000 Chromify-1.1.3/Chromify/Converter.py
--rw-rw-rw-   0        0        0      148 2023-07-18 14:17:04.000000 Chromify-1.1.3/Chromify/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:17:20.012303 Chromify-1.1.3/Chromify.egg-info/
--rw-rw-rw-   0        0        0     8627 2023-07-18 14:17:19.000000 Chromify-1.1.3/Chromify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-18 14:17:19.000000 Chromify-1.1.3/Chromify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 14:17:19.000000 Chromify-1.1.3/Chromify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 14:17:19.000000 Chromify-1.1.3/Chromify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1314 2023-07-18 13:26:56.000000 Chromify-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     8627 2023-07-18 14:17:20.089573 Chromify-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     8065 2023-07-18 13:42:14.000000 Chromify-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 14:17:20.091568 Chromify-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-07-18 14:17:04.000000 Chromify-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:39:12.563789 Chromify-1.1.4/
+drwxrwxrwx   0        0        0        0 2023-07-18 14:39:12.243109 Chromify-1.1.4/Chromify/
+-rw-rw-rw-   0        0        0     6544 2023-07-18 13:26:56.000000 Chromify-1.1.4/Chromify/Chromify.py
+-rw-rw-rw-   0        0        0    16090 2023-07-18 13:26:56.000000 Chromify-1.1.4/Chromify/Color.py
+-rw-rw-rw-   0        0        0     7866 2023-07-18 13:37:52.000000 Chromify-1.1.4/Chromify/Converter.py
+-rw-rw-rw-   0        0        0      148 2023-07-18 14:38:46.000000 Chromify-1.1.4/Chromify/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:39:12.483154 Chromify-1.1.4/Chromify.egg-info/
+-rw-rw-rw-   0        0        0     8627 2023-07-18 14:39:11.000000 Chromify-1.1.4/Chromify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-18 14:39:12.000000 Chromify-1.1.4/Chromify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 14:39:11.000000 Chromify-1.1.4/Chromify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 14:39:12.000000 Chromify-1.1.4/Chromify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1314 2023-07-18 13:26:56.000000 Chromify-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     8627 2023-07-18 14:39:12.561805 Chromify-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8065 2023-07-18 13:42:14.000000 Chromify-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 14:39:12.563789 Chromify-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-07-18 14:38:46.000000 Chromify-1.1.4/setup.py
```

### Comparing `Chromify-1.1.3/Chromify/Chromify.py` & `Chromify-1.1.4/Chromify/Chromify.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.1.3/Chromify/Color.py` & `Chromify-1.1.4/Chromify/Color.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.1.3/Chromify/Converter.py` & `Chromify-1.1.4/Chromify/Converter.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.1.3/Chromify.egg-info/PKG-INFO` & `Chromify-1.1.4/Chromify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.1.3
+Version: 1.1.4
 Summary: Colorful Terminal Prints
 Home-page: https://github.com/plaraje/Chromify
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Chromify-1.1.3/LICENSE` & `Chromify-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Chromify-1.1.3/PKG-INFO` & `Chromify-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.1.3
+Version: 1.1.4
 Summary: Colorful Terminal Prints
 Home-page: https://github.com/plaraje/Chromify
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Chromify-1.1.3/README.md` & `Chromify-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `Chromify-1.1.3/setup.py` & `Chromify-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Chromify',
-    version='1.1.3',
+    version='1.1.4',
     author='Plaraje',
     author_email='mat.demoya@gmail.com',
     description='Colorful Terminal Prints',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

