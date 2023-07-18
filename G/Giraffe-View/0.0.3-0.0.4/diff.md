# Comparing `tmp/Giraffe_View-0.0.3.tar.gz` & `tmp/Giraffe_View-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.0.3.tar", last modified: Tue Jul 18 11:10:51 2023, max compression
+gzip compressed data, was "Giraffe_View-0.0.4.tar", last modified: Tue Jul 18 11:39:02 2023, max compression
```

## Comparing `Giraffe_View-0.0.3.tar` & `Giraffe_View-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/Giraffe_View/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3274 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/GC_bias.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3572 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/Giraffe_View.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       22 2023-07-18 10:43:47.000000 Giraffe_View-0.0.3/Giraffe_View/__init__.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/estimated_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/function.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4707 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/observed_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5319 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/plot.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      474 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       65 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.3/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4774 2023-07-18 10:39:38.000000 Giraffe_View-0.0.3/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      938 2023-07-18 11:10:45.000000 Giraffe_View-0.0.3/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:39:02.837392 Giraffe_View-0.0.4/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:39:02.837392 Giraffe_View-0.0.4/Giraffe_View/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3274 2023-07-18 10:42:50.000000 Giraffe_View-0.0.4/Giraffe_View/GC_bias.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3572 2023-07-18 11:28:54.000000 Giraffe_View-0.0.4/Giraffe_View/Giraffe
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       57 2023-07-18 11:25:53.000000 Giraffe_View-0.0.4/Giraffe_View/__init__.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.4/Giraffe_View/estimated_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.4/Giraffe_View/function.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4707 2023-07-18 10:42:50.000000 Giraffe_View-0.0.4/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.4/Giraffe_View/observed_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5319 2023-07-18 10:42:50.000000 Giraffe_View-0.0.4/Giraffe_View/plot.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.4/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:39:02.837392 Giraffe_View-0.0.4/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 11:39:02.000000 Giraffe_View-0.0.4/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2023-07-18 11:39:02.000000 Giraffe_View-0.0.4/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-18 11:39:02.000000 Giraffe_View-0.0.4/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       65 2023-07-18 11:39:02.000000 Giraffe_View-0.0.4/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-18 11:39:02.000000 Giraffe_View-0.0.4/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.4/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 11:39:02.837392 Giraffe_View-0.0.4/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4774 2023-07-18 10:39:38.000000 Giraffe_View-0.0.4/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-18 11:39:02.837392 Giraffe_View-0.0.4/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      930 2023-07-18 11:38:28.000000 Giraffe_View-0.0.4/setup.py
```

### Comparing `Giraffe_View-0.0.3/Giraffe_View/GC_bias.py` & `Giraffe_View-0.0.4/Giraffe_View/GC_bias.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/Giraffe_View/Giraffe_View.py` & `Giraffe_View-0.0.4/Giraffe_View/Giraffe`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.0.4/Giraffe_View/estimated_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/Giraffe_View/function.py` & `Giraffe_View-0.0.4/Giraffe_View/function.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/Giraffe_View/homopolymer.py` & `Giraffe_View-0.0.4/Giraffe_View/homopolymer.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.0.4/Giraffe_View/observed_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/Giraffe_View/plot.py` & `Giraffe_View-0.0.4/Giraffe_View/plot.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/Giraffe_View/regional_modification.py` & `Giraffe_View-0.0.4/Giraffe_View/regional_modification.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.0.4/Giraffe_View.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe-View
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.0.3/LICENSE` & `Giraffe_View-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/PKG-INFO` & `Giraffe_View-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe_View
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.0.3/README.md` & `Giraffe_View-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.3/setup.py` & `Giraffe_View-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.0.3",
+  version="0.0.4",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="A small tool help assess and visualize the accuracy of a sequencing dataset, \
   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
@@ -23,9 +23,9 @@
   install_requires=[
   'pysam == 0.21.0',
   'rpy2==3.0',
   'numpy == 1.25.1',
   'pandas == 2.0.3',
   'tqdm == 4.64.0'
   ],
-  scripts = ["Giraffe_View/Giraffe_View.py"]
+  scripts = ["Giraffe_View/Giraffe"]
 )
```

