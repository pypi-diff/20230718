# Comparing `tmp/LatticeGeometryLib-0.0.7.tar.gz` & `tmp/LatticeGeometryLib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LatticeGeometryLib-0.0.7.tar", last modified: Tue Jul 18 10:25:58 2023, max compression
+gzip compressed data, was "LatticeGeometryLib-0.0.9.tar", last modified: Tue Jul 18 10:31:32 2023, max compression
```

## Comparing `LatticeGeometryLib-0.0.7.tar` & `LatticeGeometryLib-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 10:25:58.830525 LatticeGeometryLib-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-07-18 10:25:58.816571 LatticeGeometryLib-0.0.7/.idea/
--rw-rw-rw-   0        0        0       50 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.7/.idea/.gitignore
--rw-rw-rw-   0        0        0      291 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.7/.idea/Bachelorarbeit.iml
-drwxrwxrwx   0        0        0        0 2023-07-18 10:25:58.817577 LatticeGeometryLib-0.0.7/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      410 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.7/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0        0        0      174 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      189 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.7/.idea/misc.xml
--rw-rw-rw-   0        0        0      287 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.7/.idea/modules.xml
--rw-rw-rw-   0        0        0      185 2023-02-13 07:47:18.000000 LatticeGeometryLib-0.0.7/.idea/vcs.xml
-drwxrwxrwx   0        0        0        0 2023-07-18 10:25:58.824548 LatticeGeometryLib-0.0.7/LatticeGeometryLib/
--rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib/CellConfiguration.py
--rw-rw-rw-   0        0        0     4537 2023-07-17 21:25:19.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib/Geometry.py
--rw-rw-rw-   0        0        0     3438 2023-07-17 20:10:54.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib/Lattice.py
--rw-rw-rw-   0        0        0     6684 2023-07-18 10:22:47.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib/LatticeGeometryLib.py
--rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib/LatticeGeometryUI.py
--rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib/Miscellaneous.py
--rw-rw-rw-   0        0        0     5015 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib/UnitaryCell.py
--rw-rw-rw-   0        0        0    10659 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib/View.py
--rw-rw-rw-   0        0        0       94 2023-07-18 10:22:47.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 10:25:58.828531 LatticeGeometryLib-0.0.7/LatticeGeometryLib.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-18 10:25:58.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2023-07-18 10:25:58.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 10:25:58.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 10:25:58.000000 LatticeGeometryLib-0.0.7/LatticeGeometryLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      481 2023-07-18 10:25:58.829528 LatticeGeometryLib-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 10:25:58.830525 LatticeGeometryLib-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-07-18 10:25:56.000000 LatticeGeometryLib-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:31:32.874272 LatticeGeometryLib-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-07-18 10:31:32.859322 LatticeGeometryLib-0.0.9/.idea/
+-rw-rw-rw-   0        0        0       50 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.9/.idea/.gitignore
+-rw-rw-rw-   0        0        0      291 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.9/.idea/Bachelorarbeit.iml
+drwxrwxrwx   0        0        0        0 2023-07-18 10:31:32.861316 LatticeGeometryLib-0.0.9/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      410 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      174 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      189 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.9/.idea/misc.xml
+-rw-rw-rw-   0        0        0      287 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.9/.idea/modules.xml
+-rw-rw-rw-   0        0        0      185 2023-02-13 07:47:18.000000 LatticeGeometryLib-0.0.9/.idea/vcs.xml
+drwxrwxrwx   0        0        0        0 2023-07-18 10:31:32.870286 LatticeGeometryLib-0.0.9/LatticeGeometryLib/
+-rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib/CellConfiguration.py
+-rw-rw-rw-   0        0        0     4537 2023-07-17 21:25:19.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib/Geometry.py
+-rw-rw-rw-   0        0        0     3438 2023-07-17 20:10:54.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib/Lattice.py
+-rw-rw-rw-   0        0        0     6652 2023-07-18 10:28:32.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib/LatticeGeometryLib.py
+-rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib/LatticeGeometryUI.py
+-rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib/Miscellaneous.py
+-rw-rw-rw-   0        0        0     4983 2023-07-18 10:28:54.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib/UnitaryCell.py
+-rw-rw-rw-   0        0        0    10595 2023-07-18 10:29:10.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib/View.py
+-rw-rw-rw-   0        0        0       94 2023-07-18 10:22:47.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:31:32.873276 LatticeGeometryLib-0.0.9/LatticeGeometryLib.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-18 10:31:32.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2023-07-18 10:31:32.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:31:32.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 10:31:32.000000 LatticeGeometryLib-0.0.9/LatticeGeometryLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      481 2023-07-18 10:31:32.874272 LatticeGeometryLib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:31:32.875269 LatticeGeometryLib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      916 2023-07-18 10:31:00.000000 LatticeGeometryLib-0.0.9/setup.py
```

### Comparing `LatticeGeometryLib-0.0.7/LatticeGeometryLib/CellConfiguration.py` & `LatticeGeometryLib-0.0.9/LatticeGeometryLib/CellConfiguration.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.7/LatticeGeometryLib/Geometry.py` & `LatticeGeometryLib-0.0.9/LatticeGeometryLib/Geometry.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.7/LatticeGeometryLib/Lattice.py` & `LatticeGeometryLib-0.0.9/LatticeGeometryLib/Lattice.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.7/LatticeGeometryLib/LatticeGeometryLib.py` & `LatticeGeometryLib-0.0.9/LatticeGeometryLib/LatticeGeometryLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from cadquery import Workplane, importers, exporters
-from modules.Geometry import Geometry
-from modules.Miscellaneous import Size, Switch
+from Geometry import Geometry
+from Miscellaneous import Size, Switch
 from Code.LatticeGeometryLib.UnitaryCell import UnitaryCell
-from modules.Lattice import Lattice
-from modules.CellConfiguration import Entity, CellConfiguration
+from Lattice import Lattice
+from CellConfiguration import Entity, CellConfiguration
 
 
 class LatticeGeometryLib:
     def __init__( self ):
         self.config = CellConfiguration()
         self.geometry = Geometry()
         self.lattice: Lattice = Lattice()
```

### Comparing `LatticeGeometryLib-0.0.7/LatticeGeometryLib/LatticeGeometryUI.py` & `LatticeGeometryLib-0.0.9/LatticeGeometryLib/LatticeGeometryUI.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.7/LatticeGeometryLib/Miscellaneous.py` & `LatticeGeometryLib-0.0.9/LatticeGeometryLib/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.7/LatticeGeometryLib/UnitaryCell.py` & `LatticeGeometryLib-0.0.9/LatticeGeometryLib/UnitaryCell.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from Miscellaneous import Size
-from Code.LatticeGeometryLib.modules.CellConfiguration import CellConfiguration
+from CellConfiguration import CellConfiguration
 from cadquery import Workplane, Plane, Location, Vector
 from cadquery.selectors import BoxSelector
 
 
 class UnitaryCell:
     """
     Geometrische Repräsentation der Elementarzelle
```

### Comparing `LatticeGeometryLib-0.0.7/LatticeGeometryLib/View.py` & `LatticeGeometryLib-0.0.9/LatticeGeometryLib/View.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from matplotlib import pyplot
 from mpl_toolkits.mplot3d import art3d
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from typing import (List)
-from Code.LatticeGeometryLib.modules.Miscellaneous import Size, Periodicity
+from Miscellaneous import Size, Periodicity
 from ctypes import windll
 import cadquery as cq
-from Code.LatticeGeometryLib.modules.CellConfiguration import CellConfiguration
+from CellConfiguration import CellConfiguration
 
 
 class CellViewer(FigureCanvasTkAgg):
     def __init__(self, widget, width, height):
         self.dpi = get_ppi()
         self.figure, self.axes = pyplot.subplots(nrows=2, ncols=1, figsize=(width / self.dpi, height / self.dpi),
                                                  dpi=self.dpi, subplot_kw={'projection': '3d'},
```

### Comparing `LatticeGeometryLib-0.0.7/LatticeGeometryLib.egg-info/SOURCES.txt` & `LatticeGeometryLib-0.0.9/LatticeGeometryLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.7/setup.py` & `LatticeGeometryLib-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.9'
 DESCRIPTION = 'Package for LatticeGeometryLib'
 LONG_DESCRIPTION = 'Package for LatticeGeometryLib'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="LatticeGeometryLib",
```

