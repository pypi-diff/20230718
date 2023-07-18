# Comparing `tmp/LatticeGeometryLib-0.0.1.tar.gz` & `tmp/LatticeGeometryLib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LatticeGeometryLib-0.0.1.tar", last modified: Tue Jul 18 09:42:51 2023, max compression
+gzip compressed data, was "LatticeGeometryLib-0.0.2.tar", last modified: Tue Jul 18 09:52:57 2023, max compression
```

## Comparing `LatticeGeometryLib-0.0.1.tar` & `LatticeGeometryLib-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 09:42:51.036687 LatticeGeometryLib-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-18 09:42:50.999410 LatticeGeometryLib-0.0.1/.idea/
--rw-rw-rw-   0        0        0       50 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.1/.idea/.gitignore
--rw-rw-rw-   0        0        0      291 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.1/.idea/Bachelorarbeit.iml
-drwxrwxrwx   0        0        0        0 2023-07-18 09:42:51.006159 LatticeGeometryLib-0.0.1/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      410 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0        0        0      174 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      189 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.1/.idea/misc.xml
--rw-rw-rw-   0        0        0      287 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.1/.idea/modules.xml
--rw-rw-rw-   0        0        0      185 2023-02-13 07:47:18.000000 LatticeGeometryLib-0.0.1/.idea/vcs.xml
-drwxrwxrwx   0        0        0        0 2023-07-18 09:42:51.019107 LatticeGeometryLib-0.0.1/LatticeGeometryLib/
--rw-rw-rw-   0        0        0     6801 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/LatticeGeometryLib.py
--rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/LatticeGeometryUI.py
--rw-rw-rw-   0        0        0    10659 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/View.py
--rw-rw-rw-   0        0        0       64 2023-07-18 09:24:04.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:42:51.034442 LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/
--rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/CellConfiguration.py
--rw-rw-rw-   0        0        0     4537 2023-07-17 21:25:19.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/Geometry.py
--rw-rw-rw-   0        0        0     3438 2023-07-17 20:10:54.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/Lattice.py
--rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/Miscellaneous.py
--rw-rw-rw-   0        0        0     5015 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/UnitaryCell.py
--rw-rw-rw-   0        0        0       99 2023-07-18 09:22:42.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 09:42:51.025554 LatticeGeometryLib-0.0.1/LatticeGeometryLib.egg-info/
--rw-rw-rw-   0        0        0      486 2023-07-18 09:42:50.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      746 2023-07-18 09:42:50.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 09:42:50.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 09:42:50.000000 LatticeGeometryLib-0.0.1/LatticeGeometryLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      486 2023-07-18 09:42:51.035685 LatticeGeometryLib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 09:42:51.036832 LatticeGeometryLib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-07-18 09:29:57.000000 LatticeGeometryLib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.566417 LatticeGeometryLib-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.549469 LatticeGeometryLib-0.0.2/.idea/
+-rw-rw-rw-   0        0        0       50 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/.gitignore
+-rw-rw-rw-   0        0        0      291 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/Bachelorarbeit.iml
+drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.552459 LatticeGeometryLib-0.0.2/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      410 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      174 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      189 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/misc.xml
+-rw-rw-rw-   0        0        0      287 2023-02-09 09:53:28.000000 LatticeGeometryLib-0.0.2/.idea/modules.xml
+-rw-rw-rw-   0        0        0      185 2023-02-13 07:47:18.000000 LatticeGeometryLib-0.0.2/.idea/vcs.xml
+drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.556445 LatticeGeometryLib-0.0.2/LatticeGeometryLib/
+-rw-rw-rw-   0        0        0     6801 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/LatticeGeometryLib.py
+-rw-rw-rw-   0        0        0    66293 2023-07-18 07:06:37.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/LatticeGeometryUI.py
+-rw-rw-rw-   0        0        0    10659 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/View.py
+-rw-rw-rw-   0        0        0       64 2023-07-18 09:24:04.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.564419 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/
+-rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/CellConfiguration.py
+-rw-rw-rw-   0        0        0     4537 2023-07-17 21:25:19.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Geometry.py
+-rw-rw-rw-   0        0        0     3438 2023-07-17 20:10:54.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Lattice.py
+-rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Miscellaneous.py
+-rw-rw-rw-   0        0        0     5015 2023-07-18 09:27:04.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/UnitaryCell.py
+-rw-rw-rw-   0        0        0       99 2023-07-18 09:22:42.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:52:57.559436 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-18 09:52:56.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-07-18 09:52:57.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 09:52:56.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 09:52:56.000000 LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      481 2023-07-18 09:52:57.565415 LatticeGeometryLib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 09:52:57.566417 LatticeGeometryLib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      916 2023-07-18 09:52:46.000000 LatticeGeometryLib-0.0.2/setup.py
```

### Comparing `LatticeGeometryLib-0.0.1/LatticeGeometryLib/LatticeGeometryLib.py` & `LatticeGeometryLib-0.0.2/LatticeGeometryLib/LatticeGeometryLib.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.1/LatticeGeometryLib/LatticeGeometryUI.py` & `LatticeGeometryLib-0.0.2/LatticeGeometryLib/LatticeGeometryUI.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.1/LatticeGeometryLib/View.py` & `LatticeGeometryLib-0.0.2/LatticeGeometryLib/View.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/CellConfiguration.py` & `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/CellConfiguration.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/Geometry.py` & `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Geometry.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/Lattice.py` & `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Lattice.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/Miscellaneous.py` & `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.1/LatticeGeometryLib/modules/UnitaryCell.py` & `LatticeGeometryLib-0.0.2/LatticeGeometryLib/modules/UnitaryCell.py`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.1/LatticeGeometryLib.egg-info/SOURCES.txt` & `LatticeGeometryLib-0.0.2/LatticeGeometryLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LatticeGeometryLib-0.0.1/setup.py` & `LatticeGeometryLib-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Package for LatticeGeometryLib'
 LONG_DESCRIPTION = 'Package for LatticeGeometryLib'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="LatticeGeometryLib",
-    version=VERSION,
     author="Dennis Schulz",
+    version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
-    keywords=['python', 'first package'],
+    keywords=['python', 'cadquery'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

