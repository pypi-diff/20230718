# Comparing `tmp/LatticeGeometryLib-0.0.5.tar.gz` & `tmp/LatticeGeometryLib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LatticeGeometryLib-0.0.5.tar", last modified: Tue Jul 18 10:17:52 2023, max compression
+gzip compressed data, was "LatticeGeometryLib-0.0.6.tar", last modified: Tue Jul 18 10:22:59 2023, max compression
```

## Comparing `LatticeGeometryLib-0.0.5.tar` & `LatticeGeometryLib-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 10:17:52.264875 LatticeGeometryLib-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-07-18 10:17:52.243951 LatticeGeometryLib-0.0.5/.idea/
--rw-rw-rw-   0        0        0       50 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.5/.idea/.gitignore
--rw-rw-rw-   0        0        0      291 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.5/.idea/Bachelorarbeit.iml
-drwxrwxrwx   0        0        0        0 2023-07-18 10:17:52.246937 LatticeGeometryLib-0.0.5/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      410 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0        0        0      174 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      189 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.5/.idea/misc.xml
--rw-rw-rw-   0        0        0      287 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.5/.idea/modules.xml
--rw-rw-rw-   0        0        0      185 2023-02-13 07:47:18.000000 LatticeGeometryLib-0.0.5/.idea/vcs.xml
-drwxrwxrwx   0        0        0        0 2023-07-18 10:17:52.250922 LatticeGeometryLib-0.0.5/LatticeGeometryLib/
--rw-rw-rw-   0        0        0     6668 2023-07-18 10:12:04.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/LatticeGeometryLib.py
--rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/LatticeGeometryUI.py
--rw-rw-rw-   0        0        0    10659 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/View.py
--rw-rw-rw-   0        0        0      113 2023-07-18 10:17:17.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 10:17:52.262882 LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/
--rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/CellConfiguration.py
--rw-rw-rw-   0        0        0     4537 2023-07-17 21:25:19.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/Geometry.py
--rw-rw-rw-   0        0        0     3438 2023-07-17 20:10:54.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/Lattice.py
--rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/Miscellaneous.py
--rw-rw-rw-   0        0        0     5015 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/UnitaryCell.py
--rw-rw-rw-   0        0        0      101 2023-07-18 10:04:34.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 10:17:52.256909 LatticeGeometryLib-0.0.5/LatticeGeometryLib.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-18 10:17:51.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      746 2023-07-18 10:17:52.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 10:17:51.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 10:17:51.000000 LatticeGeometryLib-0.0.5/LatticeGeometryLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      481 2023-07-18 10:17:52.263879 LatticeGeometryLib-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 10:17:52.264875 LatticeGeometryLib-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-07-18 10:17:35.000000 LatticeGeometryLib-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:22:59.499532 LatticeGeometryLib-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-07-18 10:22:59.479600 LatticeGeometryLib-0.0.6/.idea/
+-rw-rw-rw-   0        0        0       50 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.6/.idea/.gitignore
+-rw-rw-rw-   0        0        0      291 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.6/.idea/Bachelorarbeit.iml
+drwxrwxrwx   0        0        0        0 2023-07-18 10:22:59.481592 LatticeGeometryLib-0.0.6/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      410 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      174 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      189 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.6/.idea/misc.xml
+-rw-rw-rw-   0        0        0      287 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.6/.idea/modules.xml
+-rw-rw-rw-   0        0        0      185 2023-02-13 07:47:18.000000 LatticeGeometryLib-0.0.6/.idea/vcs.xml
+drwxrwxrwx   0        0        0        0 2023-07-18 10:22:59.491563 LatticeGeometryLib-0.0.6/LatticeGeometryLib/
+-rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib/CellConfiguration.py
+-rw-rw-rw-   0        0        0     4537 2023-07-17 21:25:19.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib/Geometry.py
+-rw-rw-rw-   0        0        0     3438 2023-07-17 20:10:54.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib/Lattice.py
+-rw-rw-rw-   0        0        0     6684 2023-07-18 10:22:47.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib/LatticeGeometryLib.py
+-rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib/LatticeGeometryUI.py
+-rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib/Miscellaneous.py
+-rw-rw-rw-   0        0        0     5015 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib/UnitaryCell.py
+-rw-rw-rw-   0        0        0    10659 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib/View.py
+-rw-rw-rw-   0        0        0       94 2023-07-18 10:22:47.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:22:59.497544 LatticeGeometryLib-0.0.6/LatticeGeometryLib.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-18 10:22:58.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2023-07-18 10:22:59.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:22:58.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 10:22:58.000000 LatticeGeometryLib-0.0.6/LatticeGeometryLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      481 2023-07-18 10:22:59.498536 LatticeGeometryLib-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:22:59.499532 LatticeGeometryLib-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-07-18 10:22:55.000000 LatticeGeometryLib-0.0.6/setup.py
```

### Comparing `LatticeGeometryLib-0.0.5/LatticeGeometryLib/LatticeGeometryLib.py` & `LatticeGeometryLib-0.0.6/LatticeGeometryLib/LatticeGeometryLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cadquery import Workplane, importers, exporters
 from modules.Geometry import Geometry
 from modules.Miscellaneous import Size, Switch
-from modules.UnitaryCell import UnitaryCell
+from Code.LatticeGeometryLib.UnitaryCell import UnitaryCell
 from modules.Lattice import Lattice
 from modules.CellConfiguration import Entity, CellConfiguration
 
 
 class LatticeGeometryLib:
     def __init__( self ):
         self.config = CellConfiguration()
```

### Comparing `LatticeGeometryLib-0.0.5/LatticeGeometryLib/LatticeGeometryUI.py` & `LatticeGeometryLib-0.0.6/LatticeGeometryLib/LatticeGeometryUI.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.5/LatticeGeometryLib/View.py` & `LatticeGeometryLib-0.0.6/LatticeGeometryLib/View.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/CellConfiguration.py` & `LatticeGeometryLib-0.0.6/LatticeGeometryLib/CellConfiguration.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/Geometry.py` & `LatticeGeometryLib-0.0.6/LatticeGeometryLib/Geometry.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/Lattice.py` & `LatticeGeometryLib-0.0.6/LatticeGeometryLib/Lattice.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/Miscellaneous.py` & `LatticeGeometryLib-0.0.6/LatticeGeometryLib/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.5/LatticeGeometryLib/modules/UnitaryCell.py` & `LatticeGeometryLib-0.0.6/LatticeGeometryLib/UnitaryCell.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.5/LatticeGeometryLib.egg-info/SOURCES.txt` & `LatticeGeometryLib-0.0.6/LatticeGeometryLib.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 .idea/.gitignore
 .idea/Bachelorarbeit.iml
 .idea/misc.xml
 .idea/modules.xml
 .idea/vcs.xml
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
+LatticeGeometryLib/CellConfiguration.py
+LatticeGeometryLib/Geometry.py
+LatticeGeometryLib/Lattice.py
 LatticeGeometryLib/LatticeGeometryLib.py
 LatticeGeometryLib/LatticeGeometryUI.py
+LatticeGeometryLib/Miscellaneous.py
+LatticeGeometryLib/UnitaryCell.py
 LatticeGeometryLib/View.py
 LatticeGeometryLib/__init__.py
 LatticeGeometryLib.egg-info/PKG-INFO
 LatticeGeometryLib.egg-info/SOURCES.txt
 LatticeGeometryLib.egg-info/dependency_links.txt
-LatticeGeometryLib.egg-info/top_level.txt
-LatticeGeometryLib/modules/CellConfiguration.py
-LatticeGeometryLib/modules/Geometry.py
-LatticeGeometryLib/modules/Lattice.py
-LatticeGeometryLib/modules/Miscellaneous.py
-LatticeGeometryLib/modules/UnitaryCell.py
-LatticeGeometryLib/modules/__init__.py
+LatticeGeometryLib.egg-info/top_level.txt
```

### Comparing `LatticeGeometryLib-0.0.5/setup.py` & `LatticeGeometryLib-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' \
+VERSION = '0.0.6' \
           ''
 DESCRIPTION = 'Package for LatticeGeometryLib'
 LONG_DESCRIPTION = 'Package for LatticeGeometryLib'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
```

