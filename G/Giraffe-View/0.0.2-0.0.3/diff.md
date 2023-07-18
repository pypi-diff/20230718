# Comparing `tmp/Giraffe_View-0.0.2.tar.gz` & `tmp/Giraffe_View-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.0.2.tar", last modified: Tue Jul 18 11:06:54 2023, max compression
+gzip compressed data, was "Giraffe_View-0.0.3.tar", last modified: Tue Jul 18 11:10:51 2023, max compression
```

## Comparing `Giraffe_View-0.0.2.tar` & `Giraffe_View-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:06:54.397913 Giraffe_View-0.0.2/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:06:54.393913 Giraffe_View-0.0.2/Giraffe_View/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3274 2023-07-18 10:42:50.000000 Giraffe_View-0.0.2/Giraffe_View/GC_bias.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3572 2023-07-18 10:42:50.000000 Giraffe_View-0.0.2/Giraffe_View/Giraffe_View.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       22 2023-07-18 10:43:47.000000 Giraffe_View-0.0.2/Giraffe_View/__init__.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.2/Giraffe_View/estimated_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.2/Giraffe_View/function.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4707 2023-07-18 10:42:50.000000 Giraffe_View-0.0.2/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.2/Giraffe_View/observed_read_accuracy.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5319 2023-07-18 10:42:50.000000 Giraffe_View-0.0.2/Giraffe_View/plot.py
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.2/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:06:54.393913 Giraffe_View-0.0.2/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5166 2023-07-18 11:06:54.000000 Giraffe_View-0.0.2/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      474 2023-07-18 11:06:54.000000 Giraffe_View-0.0.2/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-18 11:06:54.000000 Giraffe_View-0.0.2/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       65 2023-07-18 11:06:54.000000 Giraffe_View-0.0.2/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-18 11:06:54.000000 Giraffe_View-0.0.2/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.2/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5166 2023-07-18 11:06:54.393913 Giraffe_View-0.0.2/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4774 2023-07-18 10:39:38.000000 Giraffe_View-0.0.2/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-18 11:06:54.397913 Giraffe_View-0.0.2/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      937 2023-07-18 11:06:47.000000 Giraffe_View-0.0.2/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/Giraffe_View/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3274 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/GC_bias.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     3572 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/Giraffe_View.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       22 2023-07-18 10:43:47.000000 Giraffe_View-0.0.3/Giraffe_View/__init__.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2835 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/estimated_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4539 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/function.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     4707 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2944 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/observed_read_accuracy.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5319 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/plot.py
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     2156 2023-07-18 10:42:50.000000 Giraffe_View-0.0.3/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      474 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       65 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2023-07-18 11:10:51.000000 Giraffe_View-0.0.3/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2023-07-18 10:44:57.000000 Giraffe_View-0.0.3/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)     5167 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4774 2023-07-18 10:39:38.000000 Giraffe_View-0.0.3/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2023-07-18 11:10:51.848941 Giraffe_View-0.0.3/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      938 2023-07-18 11:10:45.000000 Giraffe_View-0.0.3/setup.py
```

### Comparing `Giraffe_View-0.0.2/Giraffe_View/GC_bias.py` & `Giraffe_View-0.0.3/Giraffe_View/GC_bias.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/Giraffe_View/Giraffe_View.py` & `Giraffe_View-0.0.3/Giraffe_View/Giraffe_View.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.0.3/Giraffe_View/estimated_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/Giraffe_View/function.py` & `Giraffe_View-0.0.3/Giraffe_View/function.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/Giraffe_View/homopolymer.py` & `Giraffe_View-0.0.3/Giraffe_View/homopolymer.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.0.3/Giraffe_View/observed_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/Giraffe_View/plot.py` & `Giraffe_View-0.0.3/Giraffe_View/plot.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/Giraffe_View/regional_modification.py` & `Giraffe_View-0.0.3/Giraffe_View/regional_modification.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: Giraffe-View
-Version: 0.0.2
+Name: Giraffe_View
+Version: 0.0.3
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <=3.9
+Requires-Python: >=3.7, <=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
```

### Comparing `Giraffe_View-0.0.2/LICENSE` & `Giraffe_View-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/PKG-INFO` & `Giraffe_View-0.0.3/Giraffe_View.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: Giraffe_View
-Version: 0.0.2
+Name: Giraffe-View
+Version: 0.0.3
 Summary: A small tool help assess and visualize the accuracy of a sequencing dataset,   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <=3.9
+Requires-Python: >=3.7, <=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Giraffe_View 
 
 **Giraffe_View** is designed to help assess and visualize the accuracy of a sequencing dataset, specifically for Oxford Nanopore Technologies (ONT) long-read sequencing including DNA and RNA data. There are four main functions to validate the read quality.
```

### Comparing `Giraffe_View-0.0.2/README.md` & `Giraffe_View-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.0.2/setup.py` & `Giraffe_View-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.0.2",
+  version="0.0.3",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="A small tool help assess and visualize the accuracy of a sequencing dataset, \
   	specifically for Oxford Nanopore Technologies (ONT) long-read sequencing.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
   packages=setuptools.find_packages(),
   classifiers=[
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   ],
-  python_requires = '>=3.7, <=3.9',
+  python_requires = '>=3.7, <=3.10',
   install_requires=[
   'pysam == 0.21.0',
   'rpy2==3.0',
   'numpy == 1.25.1',
   'pandas == 2.0.3',
   'tqdm == 4.64.0'
   ],
```

