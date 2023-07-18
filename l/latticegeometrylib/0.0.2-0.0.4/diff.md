# Comparing `tmp/latticegeometrylib-0.0.2.tar.gz` & `tmp/latticegeometrylib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latticegeometrylib-0.0.2.tar", last modified: Tue Jul 18 16:47:05 2023, max compression
+gzip compressed data, was "latticegeometrylib-0.0.4.tar", last modified: Tue Jul 18 17:11:03 2023, max compression
```

## Comparing `latticegeometrylib-0.0.2.tar` & `latticegeometrylib-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 16:47:05.475649 latticegeometrylib-0.0.2/
--rw-rw-rw-   0        0        0      525 2023-07-18 16:47:05.475649 latticegeometrylib-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 16:47:05.462742 latticegeometrylib-0.0.2/latticegeometrylib/
--rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 latticegeometrylib-0.0.2/latticegeometrylib/CellConfiguration.py
--rw-rw-rw-   0        0        0     6898 2023-07-18 16:31:33.000000 latticegeometrylib-0.0.2/latticegeometrylib/Generator.py
--rw-rw-rw-   0        0        0     4617 2023-07-18 16:13:19.000000 latticegeometrylib-0.0.2/latticegeometrylib/Geometry.py
--rw-rw-rw-   0        0        0     3570 2023-07-18 15:26:00.000000 latticegeometrylib-0.0.2/latticegeometrylib/Lattice.py
--rw-rw-rw-   0        0        0     6175 2023-07-17 13:40:13.000000 latticegeometrylib-0.0.2/latticegeometrylib/Miscellaneous.py
--rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 latticegeometrylib-0.0.2/latticegeometrylib/UnitaryCell.py
--rw-rw-rw-   0        0        0      161 2023-07-18 16:31:50.000000 latticegeometrylib-0.0.2/latticegeometrylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 16:47:05.471644 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/
--rw-rw-rw-   0        0        0      525 2023-07-18 16:47:04.000000 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-07-18 16:47:05.000000 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 16:47:04.000000 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 16:47:04.000000 latticegeometrylib-0.0.2/latticegeometrylib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 16:47:05.475649 latticegeometrylib-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      900 2023-07-18 16:47:01.000000 latticegeometrylib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:11:03.697414 latticegeometrylib-0.0.4/
+-rw-rw-rw-   0        0        0     1096 2023-07-18 17:11:03.697414 latticegeometrylib-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-07-18 17:09:30.000000 latticegeometrylib-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-18 17:11:03.685788 latticegeometrylib-0.0.4/latticegeometrylib/
+-rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 latticegeometrylib-0.0.4/latticegeometrylib/CellConfiguration.py
+-rw-rw-rw-   0        0        0     6898 2023-07-18 16:31:33.000000 latticegeometrylib-0.0.4/latticegeometrylib/Generator.py
+-rw-rw-rw-   0        0        0     4617 2023-07-18 16:13:19.000000 latticegeometrylib-0.0.4/latticegeometrylib/Geometry.py
+-rw-rw-rw-   0        0        0     3570 2023-07-18 15:26:00.000000 latticegeometrylib-0.0.4/latticegeometrylib/Lattice.py
+-rw-rw-rw-   0        0        0     6118 2023-07-18 17:08:37.000000 latticegeometrylib-0.0.4/latticegeometrylib/Miscellaneous.py
+-rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 latticegeometrylib-0.0.4/latticegeometrylib/UnitaryCell.py
+-rw-rw-rw-   0        0        0      161 2023-07-18 16:31:50.000000 latticegeometrylib-0.0.4/latticegeometrylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:11:03.697414 latticegeometrylib-0.0.4/latticegeometrylib.egg-info/
+-rw-rw-rw-   0        0        0     1096 2023-07-18 17:11:02.000000 latticegeometrylib-0.0.4/latticegeometrylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-07-18 17:11:03.000000 latticegeometrylib-0.0.4/latticegeometrylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:11:02.000000 latticegeometrylib-0.0.4/latticegeometrylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 17:11:02.000000 latticegeometrylib-0.0.4/latticegeometrylib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:11:03.697414 latticegeometrylib-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-18 17:10:59.000000 latticegeometrylib-0.0.4/setup.py
```

### Comparing `latticegeometrylib-0.0.2/latticegeometrylib/CellConfiguration.py` & `latticegeometrylib-0.0.4/latticegeometrylib/CellConfiguration.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.2/latticegeometrylib/Generator.py` & `latticegeometrylib-0.0.4/latticegeometrylib/Generator.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.2/latticegeometrylib/Geometry.py` & `latticegeometrylib-0.0.4/latticegeometrylib/Geometry.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.2/latticegeometrylib/Lattice.py` & `latticegeometrylib-0.0.4/latticegeometrylib/Lattice.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.2/latticegeometrylib/Miscellaneous.py` & `latticegeometrylib-0.0.4/latticegeometrylib/Miscellaneous.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 
-from stl.mesh import Mesh
-from cqmore import Workplane
 import cadquery as cq
 from typing import (Tuple, List, Any, AnyStr, Union)
 
 
 def boundingBox(model: cq.Workplane) -> List[ List[ float ]]:
 
     bbInfo = model.val().BoundingBox()
```

### Comparing `latticegeometrylib-0.0.2/latticegeometrylib/UnitaryCell.py` & `latticegeometrylib-0.0.4/latticegeometrylib/UnitaryCell.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.2/setup.py` & `latticegeometrylib-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = 'Package for generating periodic truss based lattices'
-LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     # the name must match the folder name 'latticegeometrylib'
     name="latticegeometrylib",
     author="Dennis Schulz",
-    version='0.0.2',
+    version='0.0.4',
     description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
+    long_description=open('README.rst').read(),
     packages=find_packages(),
     install_requires=[],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
     keywords=['python', 'cadquery'],
     classifiers=[
         "Development Status :: 3 - Alpha",
```

