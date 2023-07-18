# Comparing `tmp/pupyl-0.9.8.tar.gz` & `tmp/pupyl-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pupyl-0.9.8.tar", last modified: Tue Oct  6 22:15:52 2020, max compression
+gzip compressed data, was "dist/pupyl-0.9.9.tar", last modified: Thu Oct  8 20:40:03 2020, max compression
```

## Comparing `pupyl-0.9.8.tar` & `pupyl-0.9.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:52.907281 pupyl-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (116)     3685 2020-10-06 22:15:52.907281 pupyl-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2020-10-06 22:15:45.000000 pupyl-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:52.903281 pupyl-0.9.8/pupyl/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:52.903281 pupyl-0.9.8/pupyl/addendum/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/addendum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      689 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/addendum/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:52.903281 pupyl-0.9.8/pupyl/duplex/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/duplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      404 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/duplex/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    14349 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/duplex/file_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     2875 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/duplex/file_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     5093 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/duplex/image.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:52.903281 pupyl-0.9.8/pupyl/embeddings/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      241 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/embeddings/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     6539 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/embeddings/features.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:52.903281 pupyl-0.9.8/pupyl/indexer/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/indexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      696 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/indexer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     7941 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/indexer/facets.py
--rw-r--r--   0 runner    (1001) docker     (116)     4568 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/search.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:52.903281 pupyl-0.9.8/pupyl/storage/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7103 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/storage/database.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:52.907281 pupyl-0.9.8/pupyl/web/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5558 2020-10-06 22:15:45.000000 pupyl-0.9.8/pupyl/web/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-06 22:15:52.903281 pupyl-0.9.8/pupyl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3685 2020-10-06 22:15:52.000000 pupyl-0.9.8/pupyl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      640 2020-10-06 22:15:52.000000 pupyl-0.9.8/pupyl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-06 22:15:52.000000 pupyl-0.9.8/pupyl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-10-06 22:15:52.000000 pupyl-0.9.8/pupyl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-10-06 22:15:52.000000 pupyl-0.9.8/pupyl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-06 22:15:52.907281 pupyl-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1099 2020-10-06 22:15:45.000000 pupyl-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-08 20:40:03.354344 pupyl-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     3723 2020-10-08 20:40:03.354344 pupyl-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2333 2020-10-08 20:39:55.000000 pupyl-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-08 20:40:03.346344 pupyl-0.9.9/pupyl/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-08 20:40:03.346344 pupyl-0.9.9/pupyl/addendum/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/addendum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      689 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/addendum/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-08 20:40:03.346344 pupyl-0.9.9/pupyl/duplex/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/duplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      404 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/duplex/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14671 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/duplex/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2875 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/duplex/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5093 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/duplex/image.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-08 20:40:03.346344 pupyl-0.9.9/pupyl/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      241 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/embeddings/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6539 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/embeddings/features.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-08 20:40:03.346344 pupyl-0.9.9/pupyl/indexer/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/indexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      696 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/indexer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7941 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/indexer/facets.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4568 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/search.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-08 20:40:03.346344 pupyl-0.9.9/pupyl/storage/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7103 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/storage/database.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-08 20:40:03.346344 pupyl-0.9.9/pupyl/web/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5558 2020-10-08 20:39:55.000000 pupyl-0.9.9/pupyl/web/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-08 20:40:03.346344 pupyl-0.9.9/pupyl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3723 2020-10-08 20:40:03.000000 pupyl-0.9.9/pupyl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      640 2020-10-08 20:40:03.000000 pupyl-0.9.9/pupyl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-08 20:40:03.000000 pupyl-0.9.9/pupyl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2020-10-08 20:40:03.000000 pupyl-0.9.9/pupyl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-10-08 20:40:03.000000 pupyl-0.9.9/pupyl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-08 20:40:03.354344 pupyl-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1099 2020-10-08 20:39:55.000000 pupyl-0.9.9/setup.py
```

### Comparing `pupyl-0.9.8/PKG-INFO` & `pupyl-0.9.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pupyl
-Version: 0.9.8
+Version: 0.9.9
 Summary: 🧿 Pupyl is a really fast image search library which you can index your own (millions of) images and find similar images in millisecond.
 Home-page: https://github.com/policratus/pupyl
 Author: Nelson Forte
 Author-email: policratus@gmail.com
 License: UNKNOWN
 Description: 
         ![pupyl](https://github.com/policratus/pupyl/raw/master/docs/pupyl.png)
@@ -34,24 +34,25 @@
         ```
         import tempfile
         
         from pupyl.search import PupylImageSearch
         from pupyl.web import interface
         
         
-        SAMPLES = 'https://github.com/policratus/pupyl' +
+        SAMPLES = 'https://github.com/policratus/pupyl' + \
             '/raw/master/samples/pupyl.txt.xz'
+        DATA_DIR = tempfile.gettempdir()
         
-        SEARCH = PupylImageSearch(data_dir=tempfile.gettempdir())
+        SEARCH = PupylImageSearch(data_dir=DATA_DIR)
         
         SEARCH.index(SAMPLES)
         
         🕐 Processed 12942 items
         
-        interface.serve()
+        interface.serve(DATA_DIR)
         ```
         
         ## 📌 Dependencies
         See all dependencies here: [dependencies](https://github.com/policratus/pupyl/network/dependencies).
         
         ### 🐧 Linux
         Some linux distros are packaged without some essential applications to built `pupyl` dependencies. If during the installation you face errors like this:
```

### Comparing `pupyl-0.9.8/README.md` & `pupyl-0.9.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,24 +26,25 @@
 ```
 import tempfile
 
 from pupyl.search import PupylImageSearch
 from pupyl.web import interface
 
 
-SAMPLES = 'https://github.com/policratus/pupyl' +
+SAMPLES = 'https://github.com/policratus/pupyl' + \
     '/raw/master/samples/pupyl.txt.xz'
+DATA_DIR = tempfile.gettempdir()
 
-SEARCH = PupylImageSearch(data_dir=tempfile.gettempdir())
+SEARCH = PupylImageSearch(data_dir=DATA_DIR)
 
 SEARCH.index(SAMPLES)
 
 🕐 Processed 12942 items
 
-interface.serve()
+interface.serve(DATA_DIR)
 ```
 
 ## 📌 Dependencies
 See all dependencies here: [dependencies](https://github.com/policratus/pupyl/network/dependencies).
 
 ### 🐧 Linux
 Some linux distros are packaged without some essential applications to built `pupyl` dependencies. If during the installation you face errors like this:
```

### Comparing `pupyl-0.9.8/pupyl/addendum/operators.py` & `pupyl-0.9.9/pupyl/addendum/operators.py`

 * *Files identical despite different names*

### Comparing `pupyl-0.9.8/pupyl/duplex/file_io.py` & `pupyl-0.9.9/pupyl/duplex/file_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import gzip
 import zipfile
 import bz2
 import lzma
 import tarfile
 from datetime import datetime
 from itertools import cycle
+from io import BytesIO
+
 import termcolor
 
 from pupyl.duplex.file_types import FileType
 from pupyl.duplex.exceptions import FileTypeNotSupportedYet, \
     FileScanNotPossible
 from pupyl.addendum.operators import intmul
 
@@ -241,15 +243,15 @@
             raise FileTypeNotSupportedYet
 
         csv_string = csv_string.decode('utf-8').splitlines()
 
         reader = csv.reader(csv_string)
 
         for row in reader:
-            yield row
+            yield row[0]
 
     @classmethod
     def scan_csv_gzip(cls, uri):
         """
         Scanner for CSV formatted text files, compressed with Gzip algorithm.
 
         Parameters
@@ -258,17 +260,22 @@
             Where csv file resides
 
         Returns
         -------
         generator of str:
             With the discovery file paths
         """
-        with gzip.open(uri, 'rt') as gzip_file:
-            for row in gzip_file:
-                yield row.replace('\n', '')
+        file_bytes = cls.get(uri)
+
+        gzip_file = gzip.decompress(
+            file_bytes
+        ).decode('utf-8').splitlines()
+
+        for row in gzip_file:
+            yield row.replace('\n', '')
 
     @staticmethod
     def safe_temp_file(**kwargs):
         """
         Create a secure temporary file name,
         which means a file with an unique name.
 
@@ -303,17 +310,22 @@
             Where csv file resides
 
         Returns
         -------
         generator of str:
             With the discovery file paths
         """
-        with bz2.open(uri, 'rt') as bz2_file:
-            for row in bz2_file:
-                yield row.replace('\n', '')
+        file_bytes = cls.get(uri)
+
+        bz2_file = bz2.decompress(
+            file_bytes
+        ).decode('utf-8').splitlines()
+
+        for row in bz2_file:
+            yield row.replace('\n', '')
 
     @classmethod
     def scan_csv_zip(cls, uri):
         """
         Scanner for CSV formatted text files, compressed with Zip algorithm.
 
         Parameters
@@ -322,16 +334,18 @@
             Where csv file resides
 
         Returns
         -------
         generator of str:
             With the discovery file paths
         """
-        for ffile in zipfile.ZipFile(uri).namelist():
-            with zipfile.ZipFile(uri).open(ffile) as ufile:
+        file_bytes = BytesIO(cls.get(uri))
+
+        for ffile in zipfile.ZipFile(file_bytes).namelist():
+            with zipfile.ZipFile(file_bytes).open(ffile) as ufile:
                 for row in ufile:
                     yield row.decode('utf-8').replace('\n', '')
 
     @classmethod
     def scan_csv_xz(cls, uri):
         """
         Scanner for CSV formatted text files, compressed with Lzma algorithm.
@@ -342,17 +356,22 @@
             Where csv file resides
 
         Returns
         -------
         generator of str:
             With the discovery file paths
         """
-        with lzma.open(uri, 'rt') as xz_file:
-            for row in xz_file:
-                yield row.replace('\n', '')
+        file_bytes = cls.get(uri)
+
+        xz_file = lzma.decompress(
+            file_bytes
+        ).decode('utf-8').splitlines()
+
+        for row in xz_file:
+            yield row.replace('\n', '')
 
     def scan(self, uri):
         """
         Return a validated uri, resolving several cases.
 
         It also choose the best discovery method.
```

### Comparing `pupyl-0.9.8/pupyl/duplex/file_types.py` & `pupyl-0.9.9/pupyl/duplex/file_types.py`

 * *Files identical despite different names*

### Comparing `pupyl-0.9.8/pupyl/duplex/image.py` & `pupyl-0.9.9/pupyl/duplex/image.py`

 * *Files identical despite different names*

### Comparing `pupyl-0.9.8/pupyl/embeddings/features.py` & `pupyl-0.9.9/pupyl/embeddings/features.py`

 * *Files identical despite different names*

### Comparing `pupyl-0.9.8/pupyl/indexer/exceptions.py` & `pupyl-0.9.9/pupyl/indexer/exceptions.py`

 * *Files identical despite different names*

### Comparing `pupyl-0.9.8/pupyl/indexer/facets.py` & `pupyl-0.9.9/pupyl/indexer/facets.py`

 * *Files identical despite different names*

### Comparing `pupyl-0.9.8/pupyl/search.py` & `pupyl-0.9.9/pupyl/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 🧿 pupyl
 
 Pupyl is a really fast image search library which you
 can index your own (millions of) images and find similar
 images in milliseconds.
 """
-__version__ = 'v0.9.8'
+__version__ = 'v0.9.9'
 
 
 import os
 import json
 import concurrent.futures
 
 from pupyl.embeddings.features import Extractors, Characteristics
```

### Comparing `pupyl-0.9.8/pupyl/storage/database.py` & `pupyl-0.9.9/pupyl/storage/database.py`

 * *Files identical despite different names*

### Comparing `pupyl-0.9.8/pupyl/web/interface.py` & `pupyl-0.9.9/pupyl/web/interface.py`

 * *Files identical despite different names*

### Comparing `pupyl-0.9.8/pupyl.egg-info/PKG-INFO` & `pupyl-0.9.9/pupyl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pupyl
-Version: 0.9.8
+Version: 0.9.9
 Summary: 🧿 Pupyl is a really fast image search library which you can index your own (millions of) images and find similar images in millisecond.
 Home-page: https://github.com/policratus/pupyl
 Author: Nelson Forte
 Author-email: policratus@gmail.com
 License: UNKNOWN
 Description: 
         ![pupyl](https://github.com/policratus/pupyl/raw/master/docs/pupyl.png)
@@ -34,24 +34,25 @@
         ```
         import tempfile
         
         from pupyl.search import PupylImageSearch
         from pupyl.web import interface
         
         
-        SAMPLES = 'https://github.com/policratus/pupyl' +
+        SAMPLES = 'https://github.com/policratus/pupyl' + \
             '/raw/master/samples/pupyl.txt.xz'
+        DATA_DIR = tempfile.gettempdir()
         
-        SEARCH = PupylImageSearch(data_dir=tempfile.gettempdir())
+        SEARCH = PupylImageSearch(data_dir=DATA_DIR)
         
         SEARCH.index(SAMPLES)
         
         🕐 Processed 12942 items
         
-        interface.serve()
+        interface.serve(DATA_DIR)
         ```
         
         ## 📌 Dependencies
         See all dependencies here: [dependencies](https://github.com/policratus/pupyl/network/dependencies).
         
         ### 🐧 Linux
         Some linux distros are packaged without some essential applications to built `pupyl` dependencies. If during the installation you face errors like this:
```

### Comparing `pupyl-0.9.8/pupyl.egg-info/SOURCES.txt` & `pupyl-0.9.9/pupyl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pupyl-0.9.8/setup.py` & `pupyl-0.9.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 
 setuptools.setup(
     name="pupyl",
-    version="0.9.8",
+    version="0.9.9",
     author="Nelson Forte",
     author_email="policratus@gmail.com",
     description="🧿 Pupyl is a really fast image search "
     "library which you can index your own (millions of) images "
     "and find similar images in millisecond.",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

