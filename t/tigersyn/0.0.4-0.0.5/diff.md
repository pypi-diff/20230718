# Comparing `tmp/tigersyn-0.0.4.tar.gz` & `tmp/tigersyn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigersyn-0.0.4.tar", last modified: Tue Jul 18 02:16:30 2023, max compression
+gzip compressed data, was "tigersyn-0.0.5.tar", last modified: Tue Jul 18 02:20:29 2023, max compression
```

## Comparing `tigersyn-0.0.4.tar` & `tigersyn-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 02:16:30.645455 tigersyn-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      948 2023-07-18 02:16:30.644458 tigersyn-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-07-18 02:14:57.000000 tigersyn-0.0.4/README.md
--rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 02:16:30.646463 tigersyn-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-07-18 02:08:42.000000 tigersyn-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:16:30.586833 tigersyn-0.0.4/tigersyn/
--rw-rw-rw-   0        0        0       28 2023-07-17 09:40:04.000000 tigersyn-0.0.4/tigersyn/__init__.py
--rw-rw-rw-   0        0        0     2275 2023-07-17 14:31:32.000000 tigersyn-0.0.4/tigersyn/syn.py
--rw-rw-rw-   0        0        0     3899 2023-07-18 02:00:16.000000 tigersyn-0.0.4/tigersyn/syn_tool.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:16:30.641456 tigersyn-0.0.4/tigersyn.egg-info/
--rw-rw-rw-   0        0        0      948 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 02:20:29.948144 tigersyn-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      987 2023-07-18 02:20:29.947141 tigersyn-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-07-18 02:14:57.000000 tigersyn-0.0.5/README.md
+-rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 02:20:29.948144 tigersyn-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-07-18 02:20:17.000000 tigersyn-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:20:29.903144 tigersyn-0.0.5/tigersyn/
+-rw-rw-rw-   0        0        0       28 2023-07-17 09:40:04.000000 tigersyn-0.0.5/tigersyn/__init__.py
+-rw-rw-rw-   0        0        0     2275 2023-07-17 14:31:32.000000 tigersyn-0.0.5/tigersyn/syn.py
+-rw-rw-rw-   0        0        0     3899 2023-07-18 02:00:16.000000 tigersyn-0.0.5/tigersyn/syn_tool.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:20:29.946242 tigersyn-0.0.5/tigersyn.egg-info/
+-rw-rw-rw-   0        0        0      987 2023-07-18 02:20:29.000000 tigersyn-0.0.5/tigersyn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-18 02:20:29.000000 tigersyn-0.0.5/tigersyn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:20:29.000000 tigersyn-0.0.5/tigersyn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-18 02:20:29.000000 tigersyn-0.0.5/tigersyn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 02:20:29.000000 tigersyn-0.0.5/tigersyn.egg-info/top_level.txt
```

### Comparing `tigersyn-0.0.4/LICENSE` & `tigersyn-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tigersyn-0.0.4/PKG-INFO` & `tigersyn-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: tigersyn
-Version: 0.0.4
+Version: 0.0.5
 Summary: Processing MRI images based on deep-learning
 Home-page: https://github.com/StanleyWangTW/tigersyn
 Author: X. S. Wang
 Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,7 +29,8 @@
 tigersyn.run('s', r'C:\T1w_dir\**\*.nii.gz') # storing output in the same dir
 tigersyn.run('sz', r'C:\T1w_dir') # Force storing nii.gz format
 ```
 ```
 s: Producing syntheseg mask
 z: Force storing nii.gz format
 ```
+
```

### Comparing `tigersyn-0.0.4/setup.py` & `tigersyn-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VESION = '0.0.4'
+VESION = '0.0.5'
 DESCRIPTION = 'Processing MRI images based on deep-learning'
 CLASSIFIERS = [
     'Intended Audience :: Developers',
     'Programming Language :: Python :: 3.9',
     'License :: OSI Approved :: MIT License',
     "Operating System :: Microsoft :: Windows"
 ]
```

### Comparing `tigersyn-0.0.4/tigersyn/syn.py` & `tigersyn-0.0.5/tigersyn/syn.py`

 * *Files identical despite different names*

### Comparing `tigersyn-0.0.4/tigersyn/syn_tool.py` & `tigersyn-0.0.5/tigersyn/syn_tool.py`

 * *Files identical despite different names*

### Comparing `tigersyn-0.0.4/tigersyn.egg-info/PKG-INFO` & `tigersyn-0.0.5/tigersyn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: tigersyn
-Version: 0.0.4
+Version: 0.0.5
 Summary: Processing MRI images based on deep-learning
 Home-page: https://github.com/StanleyWangTW/tigersyn
 Author: X. S. Wang
 Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -27,7 +29,8 @@
 tigersyn.run('s', r'C:\T1w_dir\**\*.nii.gz') # storing output in the same dir
 tigersyn.run('sz', r'C:\T1w_dir') # Force storing nii.gz format
 ```
 ```
 s: Producing syntheseg mask
 z: Force storing nii.gz format
 ```
+
```

