# Comparing `tmp/nids_datasets-0.0.4.tar.gz` & `tmp/nids_datasets-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nids_datasets-0.0.4.tar", last modified: Tue Jul 18 17:23:11 2023, max compression
+gzip compressed data, was "nids_datasets-0.0.5.tar", last modified: Tue Jul 18 17:26:24 2023, max compression
```

## Comparing `nids_datasets-0.0.4.tar` & `nids_datasets-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:23:11.229047 nids_datasets-0.0.4/
--rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-18 17:23:11.228784 nids_datasets-0.0.4/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-17 06:06:29.000000 nids_datasets-0.0.4/README.md
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:23:11.227259 nids_datasets-0.0.4/nids_datasets/
--rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.0.4/nids_datasets/__init__.py
--rw-r--r--   0 rdp        (501) staff       (20)    12810 2023-07-18 17:19:50.000000 nids_datasets-0.0.4/nids_datasets/dataset.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:23:11.228550 nids_datasets-0.0.4/nids_datasets.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-18 17:23:11.000000 nids_datasets-0.0.4/nids_datasets.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      253 2023-07-18 17:23:11.000000 nids_datasets-0.0.4/nids_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 17:23:11.000000 nids_datasets-0.0.4/nids_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      117 2023-07-18 17:23:11.000000 nids_datasets-0.0.4/nids_datasets.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       14 2023-07-18 17:23:11.000000 nids_datasets-0.0.4/nids_datasets.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 17:23:11.229210 nids_datasets-0.0.4/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      889 2023-07-18 17:23:08.000000 nids_datasets-0.0.4/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:26:24.867790 nids_datasets-0.0.5/
+-rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-18 17:26:24.867555 nids_datasets-0.0.5/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-17 06:06:29.000000 nids_datasets-0.0.5/README.md
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:26:24.866478 nids_datasets-0.0.5/nids_datasets/
+-rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.0.5/nids_datasets/__init__.py
+-rw-r--r--   0 rdp        (501) staff       (20)    12810 2023-07-18 17:19:50.000000 nids_datasets-0.0.5/nids_datasets/dataset.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:26:24.867348 nids_datasets-0.0.5/nids_datasets.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      253 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      117 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       14 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 17:26:24.867840 nids_datasets-0.0.5/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      889 2023-07-18 17:26:11.000000 nids_datasets-0.0.5/setup.py
```

### Comparing `nids_datasets-0.0.4/PKG-INFO` & `nids_datasets-0.0.5/nids_datasets.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nids_datasets
-Version: 0.0.4
+Name: nids-datasets
+Version: 0.0.5
 Summary: Download UNSW-NB15 and CIC-IDS2017 Datasets for Network Intrusion Detection (NIDS)
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: Dataset NIDS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_datasets-0.0.4/nids_datasets/dataset.py` & `nids_datasets-0.0.5/nids_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `nids_datasets-0.0.4/nids_datasets.egg-info/PKG-INFO` & `nids_datasets-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nids-datasets
-Version: 0.0.4
+Name: nids_datasets
+Version: 0.0.5
 Summary: Download UNSW-NB15 and CIC-IDS2017 Datasets for Network Intrusion Detection (NIDS)
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: Dataset NIDS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_datasets-0.0.4/setup.py` & `nids_datasets-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='nids_datasets',
-    version='0.0.4',
+    version='0.0.5',
     description="Download UNSW-NB15 and CIC-IDS2017 Datasets for Network Intrusion Detection (NIDS)",
     keywords="Dataset NIDS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

