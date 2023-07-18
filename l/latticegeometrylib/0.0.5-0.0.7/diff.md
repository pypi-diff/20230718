# Comparing `tmp/latticegeometrylib-0.0.5.tar.gz` & `tmp/latticegeometrylib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latticegeometrylib-0.0.5.tar", last modified: Tue Jul 18 17:46:39 2023, max compression
+gzip compressed data, was "latticegeometrylib-0.0.7.tar", last modified: Tue Jul 18 18:11:01 2023, max compression
```

## Comparing `latticegeometrylib-0.0.5.tar` & `latticegeometrylib-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:46:39.638814 latticegeometrylib-0.0.5/
--rw-rw-rw-   0        0        0     1361 2023-07-18 17:46:39.637817 latticegeometrylib-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      890 2023-07-18 17:45:47.000000 latticegeometrylib-0.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-18 17:46:39.633830 latticegeometrylib-0.0.5/latticegeometrylib/
--rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 latticegeometrylib-0.0.5/latticegeometrylib/CellConfiguration.py
--rw-rw-rw-   0        0        0     6898 2023-07-18 16:31:33.000000 latticegeometrylib-0.0.5/latticegeometrylib/Generator.py
--rw-rw-rw-   0        0        0     4617 2023-07-18 16:13:19.000000 latticegeometrylib-0.0.5/latticegeometrylib/Geometry.py
--rw-rw-rw-   0        0        0     3570 2023-07-18 15:26:00.000000 latticegeometrylib-0.0.5/latticegeometrylib/Lattice.py
--rw-rw-rw-   0        0        0     6118 2023-07-18 17:08:37.000000 latticegeometrylib-0.0.5/latticegeometrylib/Miscellaneous.py
--rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 latticegeometrylib-0.0.5/latticegeometrylib/UnitaryCell.py
--rw-rw-rw-   0        0        0      161 2023-07-18 16:31:50.000000 latticegeometrylib-0.0.5/latticegeometrylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:46:39.636821 latticegeometrylib-0.0.5/latticegeometrylib.egg-info/
--rw-rw-rw-   0        0        0     1361 2023-07-18 17:46:38.000000 latticegeometrylib-0.0.5/latticegeometrylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-07-18 17:46:39.000000 latticegeometrylib-0.0.5/latticegeometrylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:46:38.000000 latticegeometrylib-0.0.5/latticegeometrylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 17:46:38.000000 latticegeometrylib-0.0.5/latticegeometrylib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 17:46:39.638814 latticegeometrylib-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-07-18 17:46:05.000000 latticegeometrylib-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:11:01.809211 latticegeometrylib-0.0.7/
+-rw-rw-rw-   0        0        0     2894 2023-07-18 18:11:01.808261 latticegeometrylib-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2421 2023-07-18 18:10:55.000000 latticegeometrylib-0.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-18 18:11:01.803173 latticegeometrylib-0.0.7/latticegeometrylib/
+-rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 latticegeometrylib-0.0.7/latticegeometrylib/CellConfiguration.py
+-rw-rw-rw-   0        0        0     6898 2023-07-18 16:31:33.000000 latticegeometrylib-0.0.7/latticegeometrylib/Generator.py
+-rw-rw-rw-   0        0        0     4617 2023-07-18 16:13:19.000000 latticegeometrylib-0.0.7/latticegeometrylib/Geometry.py
+-rw-rw-rw-   0        0        0     3570 2023-07-18 15:26:00.000000 latticegeometrylib-0.0.7/latticegeometrylib/Lattice.py
+-rw-rw-rw-   0        0        0     6118 2023-07-18 17:08:37.000000 latticegeometrylib-0.0.7/latticegeometrylib/Miscellaneous.py
+-rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 latticegeometrylib-0.0.7/latticegeometrylib/UnitaryCell.py
+-rw-rw-rw-   0        0        0      161 2023-07-18 16:31:50.000000 latticegeometrylib-0.0.7/latticegeometrylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:11:01.807237 latticegeometrylib-0.0.7/latticegeometrylib.egg-info/
+-rw-rw-rw-   0        0        0     2894 2023-07-18 18:11:01.000000 latticegeometrylib-0.0.7/latticegeometrylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-07-18 18:11:01.000000 latticegeometrylib-0.0.7/latticegeometrylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:11:01.000000 latticegeometrylib-0.0.7/latticegeometrylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 18:11:01.000000 latticegeometrylib-0.0.7/latticegeometrylib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 18:11:01.809211 latticegeometrylib-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-18 18:08:44.000000 latticegeometrylib-0.0.7/setup.py
```

### Comparing `latticegeometrylib-0.0.5/latticegeometrylib/CellConfiguration.py` & `latticegeometrylib-0.0.7/latticegeometrylib/CellConfiguration.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.5/latticegeometrylib/Generator.py` & `latticegeometrylib-0.0.7/latticegeometrylib/Generator.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.5/latticegeometrylib/Geometry.py` & `latticegeometrylib-0.0.7/latticegeometrylib/Geometry.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.5/latticegeometrylib/Lattice.py` & `latticegeometrylib-0.0.7/latticegeometrylib/Lattice.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.5/latticegeometrylib/Miscellaneous.py` & `latticegeometrylib-0.0.7/latticegeometrylib/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.5/latticegeometrylib/UnitaryCell.py` & `latticegeometrylib-0.0.7/latticegeometrylib/UnitaryCell.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.5/setup.py` & `latticegeometrylib-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DESCRIPTION = 'Package for generating periodic truss based lattices'
 
 # Setting up
 setup(
     # the name must match the folder name 'latticegeometrylib'
     name="latticegeometrylib",
     author="Dennis Schulz",
-    version='0.0.5',
+    version='0.0.7',
     description=DESCRIPTION,
     long_description=open('README.rst').read(),
     packages=find_packages(),
     install_requires=[],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
     keywords=['python', 'cadquery'],
```

