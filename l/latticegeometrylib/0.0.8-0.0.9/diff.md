# Comparing `tmp/latticegeometrylib-0.0.8.tar.gz` & `tmp/latticegeometrylib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latticegeometrylib-0.0.8.tar", last modified: Tue Jul 18 18:18:13 2023, max compression
+gzip compressed data, was "latticegeometrylib-0.0.9.tar", last modified: Tue Jul 18 18:21:49 2023, max compression
```

## Comparing `latticegeometrylib-0.0.8.tar` & `latticegeometrylib-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 18:18:13.793587 latticegeometrylib-0.0.8/
--rw-rw-rw-   0        0        0     2938 2023-07-18 18:18:13.792590 latticegeometrylib-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2465 2023-07-18 18:18:02.000000 latticegeometrylib-0.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-18 18:18:13.786610 latticegeometrylib-0.0.8/latticegeometrylib/
--rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 latticegeometrylib-0.0.8/latticegeometrylib/CellConfiguration.py
--rw-rw-rw-   0        0        0     6898 2023-07-18 16:31:33.000000 latticegeometrylib-0.0.8/latticegeometrylib/Generator.py
--rw-rw-rw-   0        0        0     4617 2023-07-18 16:13:19.000000 latticegeometrylib-0.0.8/latticegeometrylib/Geometry.py
--rw-rw-rw-   0        0        0     3570 2023-07-18 15:26:00.000000 latticegeometrylib-0.0.8/latticegeometrylib/Lattice.py
--rw-rw-rw-   0        0        0     6118 2023-07-18 17:08:37.000000 latticegeometrylib-0.0.8/latticegeometrylib/Miscellaneous.py
--rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 latticegeometrylib-0.0.8/latticegeometrylib/UnitaryCell.py
--rw-rw-rw-   0        0        0      161 2023-07-18 16:31:50.000000 latticegeometrylib-0.0.8/latticegeometrylib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:18:13.791593 latticegeometrylib-0.0.8/latticegeometrylib.egg-info/
--rw-rw-rw-   0        0        0     2938 2023-07-18 18:18:13.000000 latticegeometrylib-0.0.8/latticegeometrylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-07-18 18:18:13.000000 latticegeometrylib-0.0.8/latticegeometrylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 18:18:13.000000 latticegeometrylib-0.0.8/latticegeometrylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 18:18:13.000000 latticegeometrylib-0.0.8/latticegeometrylib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 18:18:13.793587 latticegeometrylib-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-07-18 18:18:08.000000 latticegeometrylib-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:21:49.052186 latticegeometrylib-0.0.9/
+-rw-rw-rw-   0        0        0     2956 2023-07-18 18:21:49.052186 latticegeometrylib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2483 2023-07-18 18:21:26.000000 latticegeometrylib-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-18 18:21:49.045004 latticegeometrylib-0.0.9/latticegeometrylib/
+-rw-rw-rw-   0        0        0    11680 2023-07-17 14:54:21.000000 latticegeometrylib-0.0.9/latticegeometrylib/CellConfiguration.py
+-rw-rw-rw-   0        0        0     6898 2023-07-18 16:31:33.000000 latticegeometrylib-0.0.9/latticegeometrylib/Generator.py
+-rw-rw-rw-   0        0        0     4617 2023-07-18 16:13:19.000000 latticegeometrylib-0.0.9/latticegeometrylib/Geometry.py
+-rw-rw-rw-   0        0        0     3570 2023-07-18 15:26:00.000000 latticegeometrylib-0.0.9/latticegeometrylib/Lattice.py
+-rw-rw-rw-   0        0        0     6118 2023-07-18 17:08:37.000000 latticegeometrylib-0.0.9/latticegeometrylib/Miscellaneous.py
+-rw-rw-rw-   0        0        0     5048 2023-07-18 13:53:06.000000 latticegeometrylib-0.0.9/latticegeometrylib/UnitaryCell.py
+-rw-rw-rw-   0        0        0      161 2023-07-18 16:31:50.000000 latticegeometrylib-0.0.9/latticegeometrylib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:21:49.051187 latticegeometrylib-0.0.9/latticegeometrylib.egg-info/
+-rw-rw-rw-   0        0        0     2956 2023-07-18 18:21:48.000000 latticegeometrylib-0.0.9/latticegeometrylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-07-18 18:21:48.000000 latticegeometrylib-0.0.9/latticegeometrylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:21:48.000000 latticegeometrylib-0.0.9/latticegeometrylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 18:21:48.000000 latticegeometrylib-0.0.9/latticegeometrylib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 18:21:49.052186 latticegeometrylib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-18 18:21:43.000000 latticegeometrylib-0.0.9/setup.py
```

### Comparing `latticegeometrylib-0.0.8/PKG-INFO` & `latticegeometrylib-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latticegeometrylib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for generating periodic truss based lattices
 Author: Dennis Schulz
 Keywords: python,cadquery
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 LatticeGeometryLib is a python library for creating spacial lattice structures which
 consist of an interconnected network of nodes struts and plates. These individual entities
 are combined into a unitary cell which periodic repetition creates the lattice. Furthermore
 this lattice can be inserted into any shell-like CAD geometry. This library is based on the CADQuery library.
 
 .. image:: images/latticegeometrylib.png
+    :height: 500
 
 Requirements
 ============
 
 .. list-table::
    :widths: 50 50
    :header-rows: 1
```

### Comparing `latticegeometrylib-0.0.8/README.rst` & `latticegeometrylib-0.0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 LatticeGeometryLib is a python library for creating spacial lattice structures which
 consist of an interconnected network of nodes struts and plates. These individual entities
 are combined into a unitary cell which periodic repetition creates the lattice. Furthermore
 this lattice can be inserted into any shell-like CAD geometry. This library is based on the CADQuery library.
 
 .. image:: images/latticegeometrylib.png
+    :height: 500
 
 Requirements
 ============
 
 .. list-table::
    :widths: 50 50
    :header-rows: 1
```

### Comparing `latticegeometrylib-0.0.8/latticegeometrylib/CellConfiguration.py` & `latticegeometrylib-0.0.9/latticegeometrylib/CellConfiguration.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.8/latticegeometrylib/Generator.py` & `latticegeometrylib-0.0.9/latticegeometrylib/Generator.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.8/latticegeometrylib/Geometry.py` & `latticegeometrylib-0.0.9/latticegeometrylib/Geometry.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.8/latticegeometrylib/Lattice.py` & `latticegeometrylib-0.0.9/latticegeometrylib/Lattice.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.8/latticegeometrylib/Miscellaneous.py` & `latticegeometrylib-0.0.9/latticegeometrylib/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.8/latticegeometrylib/UnitaryCell.py` & `latticegeometrylib-0.0.9/latticegeometrylib/UnitaryCell.py`

 * *Files identical despite different names*

### Comparing `latticegeometrylib-0.0.8/latticegeometrylib.egg-info/PKG-INFO` & `latticegeometrylib-0.0.9/latticegeometrylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latticegeometrylib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for generating periodic truss based lattices
 Author: Dennis Schulz
 Keywords: python,cadquery
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,15 @@
 
 LatticeGeometryLib is a python library for creating spacial lattice structures which
 consist of an interconnected network of nodes struts and plates. These individual entities
 are combined into a unitary cell which periodic repetition creates the lattice. Furthermore
 this lattice can be inserted into any shell-like CAD geometry. This library is based on the CADQuery library.
 
 .. image:: images/latticegeometrylib.png
+    :height: 500
 
 Requirements
 ============
 
 .. list-table::
    :widths: 50 50
    :header-rows: 1
```

### Comparing `latticegeometrylib-0.0.8/setup.py` & `latticegeometrylib-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DESCRIPTION = 'Package for generating periodic truss based lattices'
 
 # Setting up
 setup(
     # the name must match the folder name 'latticegeometrylib'
     name="latticegeometrylib",
     author="Dennis Schulz",
-    version='0.0.8',
+    version='0.0.9',
     description=DESCRIPTION,
     long_description=open('README.rst').read(),
     packages=find_packages(),
     install_requires=[],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
 
     keywords=['python', 'cadquery'],
```

