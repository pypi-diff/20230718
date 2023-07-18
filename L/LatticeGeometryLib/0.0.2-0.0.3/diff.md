# Comparing `tmp/LatticeGeometryLib-0.0.2.tar.gz` & `tmp/LatticeGeometryLib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LatticeGeometryLib-0.0.2.tar", last modified: Tue Jul 18 09:52:57 2023, max compression
+gzip compressed data, was "LatticeGeometryLib-0.0.3.tar", last modified: Tue Jul 18 10:04:43 2023, max compression
```

## Comparing `LatticeGeometryLib-0.0.2.tar` & `LatticeGeometryLib-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.566417 LatticeGeometryLib-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.549469 LatticeGeometryLib-0.0.2/.idea/
--rw-rw-rw-   0        0        0       50 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/.gitignore
--rw-rw-rw-   0        0        0      291 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/Bachelorarbeit.iml
-drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.552459 LatticeGeometryLib-0.0.2/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      410 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0        0        0      174 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      189 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/misc.xml
--rw-rw-rw-   0        0        0      287 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/modules.xml
--rw-rw-rw-   0        0        0      185 2023-02-13 07:47:18.000000 LatticeGeometryLib-0.0.2/.idea/vcs.xml
-drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.556445 LatticeGeometryLib-0.0.2/LatticeGeometryLib/
--rw-rw-rw-   0        0        0     6801 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/LatticeGeometryLib.py
--rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/LatticeGeometryUI.py
--rw-rw-rw-   0        0        0    10659 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/View.py
--rw-rw-rw-   0        0        0       64 2023-07-18 09:24:04.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.564419 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/
--rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/CellConfiguration.py
--rw-rw-rw-   0        0        0     4537 2023-07-17 21:25:19.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Geometry.py
--rw-rw-rw-   0        0        0     3438 2023-07-17 20:10:54.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Lattice.py
--rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Miscellaneous.py
--rw-rw-rw-   0        0        0     5015 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/UnitaryCell.py
--rw-rw-rw-   0        0        0       99 2023-07-18 09:22:42.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.559436 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-18 09:52:56.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      746 2023-07-18 09:52:57.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 09:52:56.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 09:52:56.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      481 2023-07-18 09:52:57.565415 LatticeGeometryLib-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 09:52:57.566417 LatticeGeometryLib-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-07-18 09:52:46.000000 LatticeGeometryLib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:04:43.703168 LatticeGeometryLib-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-18 10:04:43.686288 LatticeGeometryLib-0.0.3/.idea/
+-rw-rw-rw-   0        0        0       50 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.3/.idea/.gitignore
+-rw-rw-rw-   0        0        0      291 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.3/.idea/Bachelorarbeit.iml
+drwxrwxrwx   0        0        0        0 2023-07-18 10:04:43.688222 LatticeGeometryLib-0.0.3/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      410 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      174 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      189 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.3/.idea/misc.xml
+-rw-rw-rw-   0        0        0      287 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.3/.idea/modules.xml
+-rw-rw-rw-   0        0        0      185 2023-02-13 07:47:18.000000 LatticeGeometryLib-0.0.3/.idea/vcs.xml
+drwxrwxrwx   0        0        0        0 2023-07-18 10:04:43.692204 LatticeGeometryLib-0.0.3/LatticeGeometryLib/
+-rw-rw-rw-   0        0        0     6801 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/LatticeGeometryLib.py
+-rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/LatticeGeometryUI.py
+-rw-rw-rw-   0        0        0    10659 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/View.py
+-rw-rw-rw-   0        0        0       27 2023-07-18 10:04:34.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:04:43.701174 LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/
+-rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/CellConfiguration.py
+-rw-rw-rw-   0        0        0     4537 2023-07-17 21:25:19.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/Geometry.py
+-rw-rw-rw-   0        0        0     3438 2023-07-17 20:10:54.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/Lattice.py
+-rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/Miscellaneous.py
+-rw-rw-rw-   0        0        0     5015 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/UnitaryCell.py
+-rw-rw-rw-   0        0        0      101 2023-07-18 10:04:34.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:04:43.695198 LatticeGeometryLib-0.0.3/LatticeGeometryLib.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-18 10:04:43.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-07-18 10:04:43.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:04:43.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 10:04:43.000000 LatticeGeometryLib-0.0.3/LatticeGeometryLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      481 2023-07-18 10:04:43.702171 LatticeGeometryLib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:04:43.703168 LatticeGeometryLib-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      916 2023-07-18 10:04:34.000000 LatticeGeometryLib-0.0.3/setup.py
```

### Comparing `LatticeGeometryLib-0.0.2/LatticeGeometryLib/LatticeGeometryLib.py` & `LatticeGeometryLib-0.0.3/LatticeGeometryLib/LatticeGeometryLib.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.2/LatticeGeometryLib/LatticeGeometryUI.py` & `LatticeGeometryLib-0.0.3/LatticeGeometryLib/LatticeGeometryUI.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.2/LatticeGeometryLib/View.py` & `LatticeGeometryLib-0.0.3/LatticeGeometryLib/View.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/CellConfiguration.py` & `LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/CellConfiguration.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Geometry.py` & `LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/Geometry.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Lattice.py` & `LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/Lattice.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Miscellaneous.py` & `LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/UnitaryCell.py` & `LatticeGeometryLib-0.0.3/LatticeGeometryLib/modules/UnitaryCell.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/SOURCES.txt` & `LatticeGeometryLib-0.0.3/LatticeGeometryLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.2/setup.py` & `LatticeGeometryLib-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Package for LatticeGeometryLib'
 LONG_DESCRIPTION = 'Package for LatticeGeometryLib'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="LatticeGeometryLib",
```

