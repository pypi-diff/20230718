# Comparing `tmp/Giraffe_View-0.0.6.tar.gz` & `tmp/Giraffe_View-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.0.6.tar", last modified: Tue Jul 18 12:00:43 2023, max compression
+gzip compressed data, was "Giraffe_View-0.0.7.tar", last modified: Tue Jul 18 12:03:51 2023, max compression
```

## Comparing `Giraffe_View-0.0.6.tar` & `Giraffe_View-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 12:00:43.039044 Giraffe_View-0.0.6/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 12:00:43.039044 Giraffe_View-0.0.6/Giraffe_View/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3288 2023-07-18 11:57:08.000000 Giraffe_View-0.0.6/Giraffe_View/GC_bias.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3663 2023-07-18 11:50:42.000000 Giraffe_View-0.0.6/Giraffe_View/Giraffe
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-18 11:47:04.000000 Giraffe_View-0.0.6/Giraffe_View/__init__.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.6/Giraffe_View/estimated_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.6/Giraffe_View/function.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4721 2023-07-18 11:57:22.000000 Giraffe_View-0.0.6/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.6/Giraffe_View/observed_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5319 2023-07-18 10:42:50.000000 Giraffe_View-0.0.6/Giraffe_View/plot.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.6/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 12:00:43.039044 Giraffe_View-0.0.6/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 12:00:42.000000 Giraffe_View-0.0.6/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-18 12:00:43.000000 Giraffe_View-0.0.6/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-18 12:00:42.000000 Giraffe_View-0.0.6/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       65 2023-07-18 12:00:42.000000 Giraffe_View-0.0.6/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-18 12:00:42.000000 Giraffe_View-0.0.6/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.6/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 12:00:43.039044 Giraffe_View-0.0.6/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4774 2023-07-18 10:39:38.000000 Giraffe_View-0.0.6/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-18 12:00:43.039044 Giraffe_View-0.0.6/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      930 2023-07-18 12:00:27.000000 Giraffe_View-0.0.6/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 12:03:51.210467 Giraffe_View-0.0.7/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 12:03:51.206467 Giraffe_View-0.0.7/Giraffe_View/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3288 2023-07-18 11:57:08.000000 Giraffe_View-0.0.7/Giraffe_View/GC_bias.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3663 2023-07-18 11:50:42.000000 Giraffe_View-0.0.7/Giraffe_View/Giraffe
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-18 11:47:04.000000 Giraffe_View-0.0.7/Giraffe_View/__init__.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.7/Giraffe_View/estimated_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.7/Giraffe_View/function.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4721 2023-07-18 12:03:26.000000 Giraffe_View-0.0.7/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.7/Giraffe_View/observed_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5319 2023-07-18 10:42:50.000000 Giraffe_View-0.0.7/Giraffe_View/plot.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.7/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 12:03:51.206467 Giraffe_View-0.0.7/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 12:03:51.000000 Giraffe_View-0.0.7/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-18 12:03:51.000000 Giraffe_View-0.0.7/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-18 12:03:51.000000 Giraffe_View-0.0.7/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       65 2023-07-18 12:03:51.000000 Giraffe_View-0.0.7/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-18 12:03:51.000000 Giraffe_View-0.0.7/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.7/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 12:03:51.206467 Giraffe_View-0.0.7/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4774 2023-07-18 10:39:38.000000 Giraffe_View-0.0.7/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-18 12:03:51.210467 Giraffe_View-0.0.7/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      930 2023-07-18 12:03:44.000000 Giraffe_View-0.0.7/setup.py
```

### Comparing `Giraffe_View-0.0.6/Giraffe_View/GC_bias.py` & `Giraffe_View-0.0.7/Giraffe_View/GC_bias.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.6/Giraffe_View/Giraffe` & `Giraffe_View-0.0.7/Giraffe_View/Giraffe`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.6/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.0.7/Giraffe_View/estimated_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.6/Giraffe_View/function.py` & `Giraffe_View-0.0.7/Giraffe_View/function.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.6/Giraffe_View/homopolymer.py` & `Giraffe_View-0.0.7/Giraffe_View/homopolymer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import pysam
 import re
-from fGiraffe_View.unction import *
+from Giraffe_View.function import *
 import multiprocessing
 
 
 def homopolymer_from_bam(input_bamfile):
 	bamfile = pysam.AlignmentFile(input_bamfile, threads=4)
 	dir_polymer = {}
```

### Comparing `Giraffe_View-0.0.6/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.0.7/Giraffe_View/observed_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.6/Giraffe_View/plot.py` & `Giraffe_View-0.0.7/Giraffe_View/plot.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.6/Giraffe_View/regional_modification.py` & `Giraffe_View-0.0.7/Giraffe_View/regional_modification.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.6/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.0.7/Giraffe_View.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe-View
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.0.6/LICENSE` & `Giraffe_View-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.6/PKG-INFO` & `Giraffe_View-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe_View
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.0.6/README.md` & `Giraffe_View-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.6/setup.py` & `Giraffe_View-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.0.6",
+  version="0.0.7",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="A small tool help assess and visualize the accuracy of a sequencing dataset, \
   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
```

