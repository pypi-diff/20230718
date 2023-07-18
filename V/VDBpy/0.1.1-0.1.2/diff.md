# Comparing `tmp/VDBpy-0.1.1.tar.gz` & `tmp/VDBpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VDBpy-0.1.1.tar", last modified: Tue Jul 18 16:41:23 2023, max compression
+gzip compressed data, was "VDBpy-0.1.2.tar", last modified: Tue Jul 18 16:45:52 2023, max compression
```

## Comparing `VDBpy-0.1.1.tar` & `VDBpy-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 16:41:23.951115 VDBpy-0.1.1/
--rw-rw-rw-   0        0        0      605 2023-07-18 16:41:23.951115 VDBpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-07-18 16:04:07.000000 VDBpy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 16:41:23.937579 VDBpy-0.1.1/VDBpy/
--rw-rw-rw-   0        0        0        0 2023-07-18 15:19:32.000000 VDBpy-0.1.1/VDBpy/__init__.py
--rw-rw-rw-   0        0        0     1303 2023-07-18 15:19:46.000000 VDBpy-0.1.1/VDBpy/indexing.py
--rw-rw-rw-   0        0        0      183 2023-07-18 13:37:09.000000 VDBpy-0.1.1/VDBpy/query.py
--rw-rw-rw-   0        0        0     1099 2023-07-18 15:19:43.000000 VDBpy-0.1.1/VDBpy/similarity.py
-drwxrwxrwx   0        0        0        0 2023-07-18 16:41:23.951115 VDBpy-0.1.1/VDBpy.egg-info/
--rw-rw-rw-   0        0        0      605 2023-07-18 16:41:23.000000 VDBpy-0.1.1/VDBpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-07-18 16:41:23.000000 VDBpy-0.1.1/VDBpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 16:41:23.000000 VDBpy-0.1.1/VDBpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 16:41:23.000000 VDBpy-0.1.1/VDBpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 16:41:23.951115 VDBpy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-07-18 16:40:56.000000 VDBpy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:45:52.247578 VDBpy-0.1.2/
+-rw-rw-rw-   0        0        0      605 2023-07-18 16:45:52.247578 VDBpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-07-18 16:04:07.000000 VDBpy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 16:45:52.205325 VDBpy-0.1.2/VDBpy/
+-rw-rw-rw-   0        0        0        0 2023-07-18 15:19:32.000000 VDBpy-0.1.2/VDBpy/__init__.py
+-rw-rw-rw-   0        0        0     1303 2023-07-18 15:19:46.000000 VDBpy-0.1.2/VDBpy/indexing.py
+-rw-rw-rw-   0        0        0      183 2023-07-18 13:37:09.000000 VDBpy-0.1.2/VDBpy/query.py
+-rw-rw-rw-   0        0        0     1099 2023-07-18 15:19:43.000000 VDBpy-0.1.2/VDBpy/similarity.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:45:52.244738 VDBpy-0.1.2/VDBpy.egg-info/
+-rw-rw-rw-   0        0        0      605 2023-07-18 16:45:52.000000 VDBpy-0.1.2/VDBpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-07-18 16:45:52.000000 VDBpy-0.1.2/VDBpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 16:45:52.000000 VDBpy-0.1.2/VDBpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 16:45:52.000000 VDBpy-0.1.2/VDBpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 16:45:52.251065 VDBpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      673 2023-07-18 16:45:47.000000 VDBpy-0.1.2/setup.py
```

### Comparing `VDBpy-0.1.1/PKG-INFO` & `VDBpy-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VDBpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple vector database allows difference search methods (consine similarity and euclidean distance ect.)
 Home-page: https://github.com/Ateee329/VDBpy
 Author: Justin He
 Author-email: justin.he814@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `VDBpy-0.1.1/VDBpy/indexing.py` & `VDBpy-0.1.2/VDBpy/indexing.py`

 * *Files identical despite different names*

### Comparing `VDBpy-0.1.1/VDBpy/similarity.py` & `VDBpy-0.1.2/VDBpy/similarity.py`

 * *Files identical despite different names*

### Comparing `VDBpy-0.1.1/VDBpy.egg-info/PKG-INFO` & `VDBpy-0.1.2/VDBpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VDBpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple vector database allows difference search methods (consine similarity and euclidean distance ect.)
 Home-page: https://github.com/Ateee329/VDBpy
 Author: Justin He
 Author-email: justin.he814@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `VDBpy-0.1.1/setup.py` & `VDBpy-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='VDBpy',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     description='A simple vector database allows difference search methods (consine similarity and euclidean distance ect.)',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Justin He',
     author_email='justin.he814@gmail.com',
     url='https://github.com/Ateee329/VDBpy',
```

