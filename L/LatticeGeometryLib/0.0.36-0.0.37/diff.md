# Comparing `tmp/LatticeGeometryLib-0.0.36.tar.gz` & `tmp/LatticeGeometryLib-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LatticeGeometryLib-0.0.36.tar", last modified: Tue Jul 18 14:32:21 2023, max compression
+gzip compressed data, was "LatticeGeometryLib-0.0.37.tar", last modified: Tue Jul 18 15:24:00 2023, max compression
```

## Comparing `LatticeGeometryLib-0.0.36.tar` & `LatticeGeometryLib-0.0.37.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 14:32:21.989502 LatticeGeometryLib-0.0.36/
-drwxrwxrwx   0        0        0        0 2023-07-18 14:32:21.984519 LatticeGeometryLib-0.0.36/LatticeGeometryLib/
--rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib/CellConfiguration.py
--rw-rw-rw-   0        0        0     4577 2023-07-18 13:52:46.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib/Geometry.py
--rw-rw-rw-   0        0        0     3568 2023-07-18 13:53:41.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib/Lattice.py
--rw-rw-rw-   0        0        0     6952 2023-07-18 13:53:41.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib/LatticeGeometryLib.py
--rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib/LatticeGeometryUI.py
--rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib/Miscellaneous.py
--rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib/UnitaryCell.py
--rw-rw-rw-   0        0        0    10595 2023-07-18 10:29:10.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib/View.py
--rw-rw-rw-   0        0        0      168 2023-07-18 14:31:30.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:32:21.987511 LatticeGeometryLib-0.0.36/LatticeGeometryLib.egg-info/
--rw-rw-rw-   0        0        0      482 2023-07-18 14:32:21.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-07-18 14:32:21.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 14:32:21.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 14:32:21.000000 LatticeGeometryLib-0.0.36/LatticeGeometryLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      482 2023-07-18 14:32:21.988507 LatticeGeometryLib-0.0.36/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 14:32:21.989502 LatticeGeometryLib-0.0.36/setup.cfg
--rw-rw-rw-   0        0        0      919 2023-07-18 14:31:37.000000 LatticeGeometryLib-0.0.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:24:00.873688 LatticeGeometryLib-0.0.37/
+drwxrwxrwx   0        0        0        0 2023-07-18 15:24:00.858797 LatticeGeometryLib-0.0.37/LatticeGeometryLib/
+-rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib/CellConfiguration.py
+-rw-rw-rw-   0        0        0     4577 2023-07-18 13:52:46.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib/Geometry.py
+-rw-rw-rw-   0        0        0     3568 2023-07-18 13:53:41.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib/Lattice.py
+-rw-rw-rw-   0        0        0     6952 2023-07-18 13:53:41.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib/LatticeGeometryLib.py
+-rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib/LatticeGeometryUI.py
+-rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib/Miscellaneous.py
+-rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib/UnitaryCell.py
+-rw-rw-rw-   0        0        0    10595 2023-07-18 10:29:10.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib/View.py
+-rw-rw-rw-   0        0        0      168 2023-07-18 14:31:30.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:24:00.873072 LatticeGeometryLib-0.0.37/LatticeGeometryLib.egg-info/
+-rw-rw-rw-   0        0        0      482 2023-07-18 15:23:59.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-07-18 15:24:00.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 15:23:59.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 15:23:59.000000 LatticeGeometryLib-0.0.37/LatticeGeometryLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      482 2023-07-18 15:24:00.873688 LatticeGeometryLib-0.0.37/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 15:24:00.873688 LatticeGeometryLib-0.0.37/setup.cfg
+-rw-rw-rw-   0        0        0      919 2023-07-18 15:23:56.000000 LatticeGeometryLib-0.0.37/setup.py
```

### Comparing `LatticeGeometryLib-0.0.36/LatticeGeometryLib/CellConfiguration.py` & `LatticeGeometryLib-0.0.37/LatticeGeometryLib/CellConfiguration.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.36/LatticeGeometryLib/Geometry.py` & `LatticeGeometryLib-0.0.37/LatticeGeometryLib/Geometry.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.36/LatticeGeometryLib/Lattice.py` & `LatticeGeometryLib-0.0.37/LatticeGeometryLib/Lattice.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.36/LatticeGeometryLib/LatticeGeometryLib.py` & `LatticeGeometryLib-0.0.37/LatticeGeometryLib/LatticeGeometryLib.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.36/LatticeGeometryLib/LatticeGeometryUI.py` & `LatticeGeometryLib-0.0.37/LatticeGeometryLib/LatticeGeometryUI.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.36/LatticeGeometryLib/Miscellaneous.py` & `LatticeGeometryLib-0.0.37/LatticeGeometryLib/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.36/LatticeGeometryLib/UnitaryCell.py` & `LatticeGeometryLib-0.0.37/LatticeGeometryLib/UnitaryCell.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.36/LatticeGeometryLib/View.py` & `LatticeGeometryLib-0.0.37/LatticeGeometryLib/View.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.36/setup.py` & `LatticeGeometryLib-0.0.37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.36'
+VERSION = '0.0.37'
 DESCRIPTION = 'Package for LatticeGeometryLib'
 LONG_DESCRIPTION = 'Package for LatticeGeometryLib'
 
 # Setting up
 setup(
     # the name must match the folder name 'LatticeGeometryLib'
     name="LatticeGeometryLib",
```

