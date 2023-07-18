# Comparing `tmp/spender-0.2.1.tar.gz` & `tmp/spender-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spender-0.2.1.tar", last modified: Tue Jul 18 02:28:43 2023, max compression
+gzip compressed data, was "spender-0.2.2.tar", last modified: Tue Jul 18 02:55:16 2023, max compression
```

## Comparing `spender-0.2.1.tar` & `spender-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:28:43.585621 spender-0.2.1/
--rw-r--r--   0 pmelchior   (501) staff       (20)     1082 2022-08-08 22:13:56.000000 spender-0.2.1/LICENSE
--rw-r--r--   0 pmelchior   (501) staff       (20)     5145 2023-07-18 02:28:43.585412 spender-0.2.1/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)     4455 2023-07-18 02:15:37.000000 spender-0.2.1/README.md
--rw-r--r--   0 pmelchior   (501) staff       (20)       38 2023-07-18 02:28:43.585670 spender-0.2.1/setup.cfg
--rw-r--r--   0 pmelchior   (501) staff       (20)     1051 2023-07-18 02:21:54.000000 spender-0.2.1/setup.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:28:43.580327 spender-0.2.1/spender/
--rw-r--r--   0 pmelchior   (501) staff       (20)     2995 2023-07-17 20:35:16.000000 spender-0.2.1/spender/__init__.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:28:43.584739 spender-0.2.1/spender/data/
--rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.2.1/spender/data/__init__.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    23672 2023-07-17 17:44:22.000000 spender-0.2.1/spender/data/desi.py
--rwxr-xr-x   0 pmelchior   (501) staff       (20)     1082 2023-05-17 22:05:49.000000 spender-0.2.1/spender/data/emission_lines.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    19391 2023-05-17 22:05:49.000000 spender-0.2.1/spender/data/sdss.py
--rwxr-xr-x   0 pmelchior   (501) staff       (20)     7570 2023-07-17 21:35:41.000000 spender-0.2.1/spender/flow.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3933 2023-05-17 22:05:49.000000 spender-0.2.1/spender/instrument.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    16440 2023-07-17 20:05:39.000000 spender-0.2.1/spender/model.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3569 2023-05-17 22:05:49.000000 spender-0.2.1/spender/util.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:28:43.581108 spender-0.2.1/spender.egg-info/
--rw-r--r--   0 pmelchior   (501) staff       (20)     5145 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)      369 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/SOURCES.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        1 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/dependency_links.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)       68 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/requires.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        8 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/top_level.txt
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:55:16.247034 spender-0.2.2/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1082 2022-08-08 22:13:56.000000 spender-0.2.2/LICENSE
+-rw-r--r--   0 pmelchior   (501) staff       (20)     5145 2023-07-18 02:55:16.246860 spender-0.2.2/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4455 2023-07-18 02:15:37.000000 spender-0.2.2/README.md
+-rw-r--r--   0 pmelchior   (501) staff       (20)       38 2023-07-18 02:55:16.247082 spender-0.2.2/setup.cfg
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1051 2023-07-18 02:50:30.000000 spender-0.2.2/setup.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:55:16.244194 spender-0.2.2/spender/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     2995 2023-07-18 02:39:17.000000 spender-0.2.2/spender/__init__.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:55:16.246208 spender-0.2.2/spender/data/
+-rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.2.2/spender/data/__init__.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    23672 2023-07-17 17:44:22.000000 spender-0.2.2/spender/data/desi.py
+-rwxr-xr-x   0 pmelchior   (501) staff       (20)     1082 2023-05-17 22:05:49.000000 spender-0.2.2/spender/data/emission_lines.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    19391 2023-05-17 22:05:49.000000 spender-0.2.2/spender/data/sdss.py
+-rwxr-xr-x   0 pmelchior   (501) staff       (20)     7570 2023-07-17 21:35:41.000000 spender-0.2.2/spender/flow.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3933 2023-05-17 22:05:49.000000 spender-0.2.2/spender/instrument.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    16440 2023-07-17 20:05:39.000000 spender-0.2.2/spender/model.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3569 2023-05-17 22:05:49.000000 spender-0.2.2/spender/util.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:55:16.245042 spender-0.2.2/spender.egg-info/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     5145 2023-07-18 02:55:16.000000 spender-0.2.2/spender.egg-info/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)      369 2023-07-18 02:55:16.000000 spender-0.2.2/spender.egg-info/SOURCES.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        1 2023-07-18 02:55:16.000000 spender-0.2.2/spender.egg-info/dependency_links.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)       68 2023-07-18 02:55:16.000000 spender-0.2.2/spender.egg-info/requires.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        8 2023-07-18 02:55:16.000000 spender-0.2.2/spender.egg-info/top_level.txt
```

### Comparing `spender-0.2.1/LICENSE` & `spender-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/PKG-INFO` & `spender-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spender
-Version: 0.2.1
+Version: 0.2.2
 Summary: Spectrum encoder and decoder
 Home-page: https://github.com/pmelchior/spender
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: spectroscopy,autoencoder
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spender-0.2.1/README.md` & `spender-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/setup.py` & `spender-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 long_description = open('README.md').read()
 
 setup(
     name="spender",
     description="Spectrum encoder and decoder",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="0.2.1",
+    version="0.2.2",
     license="MIT",
     author="Peter Melchior",
     author_email="peter.m.melchior@gmail.com",
     url="https://github.com/pmelchior/spender",
     packages=["spender", "spender.data"],
     package_data={"skymapper.data": ['*.txt']},
     classifiers=[
```

### Comparing `spender-0.2.1/spender/__init__.py` & `spender-0.2.2/spender/__init__.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/spender/data/desi.py` & `spender-0.2.2/spender/data/desi.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/spender/data/emission_lines.py` & `spender-0.2.2/spender/data/emission_lines.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/spender/data/sdss.py` & `spender-0.2.2/spender/data/sdss.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/spender/flow.py` & `spender-0.2.2/spender/flow.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/spender/instrument.py` & `spender-0.2.2/spender/instrument.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/spender/model.py` & `spender-0.2.2/spender/model.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/spender/util.py` & `spender-0.2.2/spender/util.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.1/spender.egg-info/PKG-INFO` & `spender-0.2.2/spender.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spender
-Version: 0.2.1
+Version: 0.2.2
 Summary: Spectrum encoder and decoder
 Home-page: https://github.com/pmelchior/spender
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: spectroscopy,autoencoder
 Classifier: Development Status :: 4 - Beta
```

