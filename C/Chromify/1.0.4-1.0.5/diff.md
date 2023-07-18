# Comparing `tmp/Chromify-1.0.4.tar.gz` & `tmp/Chromify-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chromify-1.0.4.tar", last modified: Tue Jul 18 12:31:22 2023, max compression
+gzip compressed data, was "Chromify-1.0.5.tar", last modified: Tue Jul 18 12:34:45 2023, max compression
```

## Comparing `Chromify-1.0.4.tar` & `Chromify-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 12:31:22.409989 Chromify-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-18 12:31:22.398876 Chromify-1.0.4/Chromify/
--rw-rw-rw-   0        0        0     6542 2023-07-18 10:22:00.000000 Chromify-1.0.4/Chromify/Chromify.py
--rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.0.4/Chromify/Color.py
--rw-rw-rw-   0        0        0     7865 2023-07-18 10:07:14.000000 Chromify-1.0.4/Chromify/Converter.py
--rw-rw-rw-   0        0        0      148 2023-07-18 12:31:16.000000 Chromify-1.0.4/Chromify/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:31:22.405901 Chromify-1.0.4/Chromify.egg-info/
--rw-rw-rw-   0        0        0     5141 2023-07-18 12:31:22.000000 Chromify-1.0.4/Chromify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-18 12:31:22.000000 Chromify-1.0.4/Chromify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 12:31:22.000000 Chromify-1.0.4/Chromify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 12:31:22.000000 Chromify-1.0.4/Chromify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1292 2023-07-17 19:51:25.000000 Chromify-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     5141 2023-07-18 12:31:22.408016 Chromify-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4489 2023-07-17 23:18:42.000000 Chromify-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 12:31:22.409989 Chromify-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-07-18 12:31:02.000000 Chromify-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:34:45.236430 Chromify-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-18 12:34:45.227324 Chromify-1.0.5/Chromify/
+-rw-rw-rw-   0        0        0     6544 2023-07-18 12:34:11.000000 Chromify-1.0.5/Chromify/Chromify.py
+-rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.0.5/Chromify/Color.py
+-rw-rw-rw-   0        0        0     7866 2023-07-18 12:34:17.000000 Chromify-1.0.5/Chromify/Converter.py
+-rw-rw-rw-   0        0        0      148 2023-07-18 12:34:24.000000 Chromify-1.0.5/Chromify/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:34:45.234431 Chromify-1.0.5/Chromify.egg-info/
+-rw-rw-rw-   0        0        0     5141 2023-07-18 12:34:45.000000 Chromify-1.0.5/Chromify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-18 12:34:45.000000 Chromify-1.0.5/Chromify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 12:34:45.000000 Chromify-1.0.5/Chromify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 12:34:45.000000 Chromify-1.0.5/Chromify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1292 2023-07-17 19:51:25.000000 Chromify-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5141 2023-07-18 12:34:45.236430 Chromify-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4489 2023-07-17 23:18:42.000000 Chromify-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 12:34:45.237430 Chromify-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-07-18 12:34:38.000000 Chromify-1.0.5/setup.py
```

### Comparing `Chromify-1.0.4/Chromify/Chromify.py` & `Chromify-1.0.5/Chromify/Chromify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-from Color import Color
-from Converter import Converter
+from .Color import Color
+from .Converter import Converter
 
 def init():
     if os.name == 'nt':
         os.system('color')
     else:
         if not os.getenv('TERM') or os.getenv('TERM') == 'dumb':
             os.environ['TERM'] = 'xterm'
```

### Comparing `Chromify-1.0.4/Chromify/Color.py` & `Chromify-1.0.5/Chromify/Color.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.4/Chromify/Converter.py` & `Chromify-1.0.5/Chromify/Converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from Color import Color
+from .Color import Color
 
 class Converter:
     def __init__(self, r=None, g=None, b=None):
         if isinstance(r, str):
             if r.startswith("#"):
                 self._from_hex(r)
             elif r.startswith("hsl"):
```

### Comparing `Chromify-1.0.4/Chromify.egg-info/PKG-INFO` & `Chromify-1.0.5/Chromify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.0.4
+Version: 1.0.5
 Summary: Colorful Terminal Prints
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Chromify-1.0.4/LICENSE` & `Chromify-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.4/PKG-INFO` & `Chromify-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chromify
-Version: 1.0.4
+Version: 1.0.5
 Summary: Colorful Terminal Prints
 Author: Plaraje
 Author-email: mat.demoya@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Chromify-1.0.4/README.md` & `Chromify-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.4/setup.py` & `Chromify-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='Chromify',
-    version='1.0.4',
+    version='1.0.5',
     author='Plaraje',
     author_email='mat.demoya@gmail.com',
     description='Colorful Terminal Prints',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

