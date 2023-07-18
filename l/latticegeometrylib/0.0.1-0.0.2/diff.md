# Comparing `tmp/latticegeometrylib-0.0.1.tar.gz` & `tmp/latticegeometrylib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latticegeometrylib-0.0.1.tar", last modified: Tue Jul 18 16:32:12 2023, max compression
+gzip compressed data, was "latticegeometrylib-0.0.2.tar", last modified: Tue Jul 18 16:47:05 2023, max compression
```

## Comparing `latticegeometrylib-0.0.1.tar` & `latticegeometrylib-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 16:32:12.049648 latticegeometrylib-0.0.1/
--rw-rw-rw-   0        0        0      525 2023-07-18 16:32:12.047927 latticegeometrylib-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 16:32:12.033940 latticegeometrylib-0.0.1/latticegeometrylib/
--rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 latticegeometrylib-0.0.1/latticegeometrylib/CellConfiguration.py
--rw-rw-rw-   0        0        0     6898 2023-07-18 16:31:33.000000 latticegeometrylib-0.0.1/latticegeometrylib/Generator.py
--rw-rw-rw-   0        0        0     4617 2023-07-18 16:13:19.000000 latticegeometrylib-0.0.1/latticegeometrylib/Geometry.py
--rw-rw-rw-   0        0        0     3570 2023-07-18 15:26:00.000000 latticegeometrylib-0.0.1/latticegeometrylib/Lattice.py
--rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 latticegeometrylib-0.0.1/latticegeometrylib/Miscellaneous.py
--rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 latticegeometrylib-0.0.1/latticegeometrylib/UnitaryCell.py
--rw-rw-rw-   0        0        0      161 2023-07-18 16:31:50.000000 latticegeometrylib-0.0.1/latticegeometrylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 16:32:12.043602 latticegeometrylib-0.0.1/latticegeometrylib.egg-info/
--rw-rw-rw-   0        0        0      525 2023-07-18 16:32:10.000000 latticegeometrylib-0.0.1/latticegeometrylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-07-18 16:32:11.000000 latticegeometrylib-0.0.1/latticegeometrylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 16:32:10.000000 latticegeometrylib-0.0.1/latticegeometrylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 16:32:10.000000 latticegeometrylib-0.0.1/latticegeometrylib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 16:32:12.049648 latticegeometrylib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      919 2023-07-18 16:31:33.000000 latticegeometrylib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:47:05.475649 latticegeometrylib-0.0.2/
+-rw-rw-rw-   0        0        0      525 2023-07-18 16:47:05.475649 latticegeometrylib-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 16:47:05.462742 latticegeometrylib-0.0.2/latticegeometrylib/
+-rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 latticegeometrylib-0.0.2/latticegeometrylib/CellConfiguration.py
+-rw-rw-rw-   0        0        0     6898 2023-07-18 16:31:33.000000 latticegeometrylib-0.0.2/latticegeometrylib/Generator.py
+-rw-rw-rw-   0        0        0     4617 2023-07-18 16:13:19.000000 latticegeometrylib-0.0.2/latticegeometrylib/Geometry.py
+-rw-rw-rw-   0        0        0     3570 2023-07-18 15:26:00.000000 latticegeometrylib-0.0.2/latticegeometrylib/Lattice.py
+-rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 latticegeometrylib-0.0.2/latticegeometrylib/Miscellaneous.py
+-rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 latticegeometrylib-0.0.2/latticegeometrylib/UnitaryCell.py
+-rw-rw-rw-   0        0        0      161 2023-07-18 16:31:50.000000 latticegeometrylib-0.0.2/latticegeometrylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:47:05.471644 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-07-18 16:47:04.000000 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-07-18 16:47:05.000000 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 16:47:04.000000 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 16:47:04.000000 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 16:47:05.475649 latticegeometrylib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      900 2023-07-18 16:47:01.000000 latticegeometrylib-0.0.2/setup.py
```

### Comparing `latticegeometrylib-0.0.1/PKG-INFO` & `latticegeometrylib-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latticegeometrylib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for generating periodic truss based lattices
 Author: Dennis Schulz
 Keywords: python,cadquery
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `latticegeometrylib-0.0.1/latticegeometrylib/CellConfiguration.py` & `latticegeometrylib-0.0.2/latticegeometrylib/CellConfiguration.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.1/latticegeometrylib/Generator.py` & `latticegeometrylib-0.0.2/latticegeometrylib/Generator.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.1/latticegeometrylib/Geometry.py` & `latticegeometrylib-0.0.2/latticegeometrylib/Geometry.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.1/latticegeometrylib/Lattice.py` & `latticegeometrylib-0.0.2/latticegeometrylib/Lattice.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.1/latticegeometrylib/Miscellaneous.py` & `latticegeometrylib-0.0.2/latticegeometrylib/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.1/latticegeometrylib/UnitaryCell.py` & `latticegeometrylib-0.0.2/latticegeometrylib/UnitaryCell.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.1/latticegeometrylib.egg-info/PKG-INFO` & `latticegeometrylib-0.0.2/latticegeometrylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latticegeometrylib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for generating periodic truss based lattices
 Author: Dennis Schulz
 Keywords: python,cadquery
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `latticegeometrylib-0.0.1/setup.py` & `latticegeometrylib-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
 DESCRIPTION = 'Package for generating periodic truss based lattices'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     # the name must match the folder name 'latticegeometrylib'
     name="latticegeometrylib",
     author="Dennis Schulz",
-    version=VERSION,
+    version='0.0.2',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
     keywords=['python', 'cadquery'],
```

