# Comparing `tmp/turtlemd-2023.2.dev1.tar.gz` & `tmp/turtlemd-2023.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turtlemd-2023.2.dev1.tar", max compression
+gzip compressed data, was "turtlemd-2023.2.dev2.tar", max compression
```

## Comparing `turtlemd-2023.2.dev1.tar` & `turtlemd-2023.2.dev2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1065 2023-04-14 09:18:44.791469 turtlemd-2023.2.dev1/LICENSE
--rw-r--r--   0        0        0      425 2023-07-17 12:41:01.376025 turtlemd-2023.2.dev1/README.md
--rw-r--r--   0        0        0      892 2023-07-18 09:53:50.409663 turtlemd-2023.2.dev1/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/__init__.py
--rw-r--r--   0        0        0    10436 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/integrators.py
--rw-r--r--   0        0        0      150 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/potentials/__init__.py
--rw-r--r--   0        0        0     3627 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/potentials/jax_bondedinteractions.py
--rw-r--r--   0        0        0    15670 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/potentials/lennardjones.py
--rw-r--r--   0        0        0     2071 2023-07-17 10:54:44.034273 turtlemd-2023.2.dev1/turtlemd/potentials/potential.py
--rw-r--r--   0        0        0     9804 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/potentials/well.py
--rw-r--r--   0        0        0       67 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/simulation/__init__.py
--rw-r--r--   0        0        0     2987 2023-07-17 10:54:44.034273 turtlemd-2023.2.dev1/turtlemd/simulation/mdsimulation.py
--rw-r--r--   0        0        0     1396 2023-07-17 10:54:44.034273 turtlemd-2023.2.dev1/turtlemd/simulation/stopping.py
--rw-r--r--   0        0        0      182 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/system/__init__.py
--rw-r--r--   0        0        0     5812 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/system/box.py
--rw-r--r--   0        0        0     8873 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/system/particles.py
--rw-r--r--   0        0        0     3835 2023-07-17 10:54:44.034273 turtlemd-2023.2.dev1/turtlemd/system/system.py
--rw-r--r--   0        0        0      168 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/tools/__init__.py
--rw-r--r--   0        0        0     2430 2023-07-10 10:53:00.136494 turtlemd-2023.2.dev1/turtlemd/tools/tools.py
--rw-r--r--   0        0        0     3083 2023-07-17 10:54:44.034273 turtlemd-2023.2.dev1/turtlemd/tools/xyz.py
--rw-r--r--   0        0        0      102 2023-06-09 08:44:04.880542 turtlemd-2023.2.dev1/turtlemd/version.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 turtlemd-2023.2.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-18 10:44:13.657090 turtlemd-2023.2.dev2/LICENSE
+-rw-r--r--   0        0        0      425 2023-07-18 10:44:13.657090 turtlemd-2023.2.dev2/README.md
+-rw-r--r--   0        0        0      892 2023-07-18 10:44:13.657090 turtlemd-2023.2.dev2/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/__init__.py
+-rw-r--r--   0        0        0    10436 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/integrators.py
+-rw-r--r--   0        0        0      150 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/potentials/__init__.py
+-rw-r--r--   0        0        0     3627 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/potentials/jax_bondedinteractions.py
+-rw-r--r--   0        0        0    15670 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/potentials/lennardjones.py
+-rw-r--r--   0        0        0     2071 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/potentials/potential.py
+-rw-r--r--   0        0        0     9804 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/potentials/well.py
+-rw-r--r--   0        0        0       67 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/simulation/__init__.py
+-rw-r--r--   0        0        0     2987 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/simulation/mdsimulation.py
+-rw-r--r--   0        0        0     1396 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/simulation/stopping.py
+-rw-r--r--   0        0        0      182 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/system/__init__.py
+-rw-r--r--   0        0        0     5812 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/system/box.py
+-rw-r--r--   0        0        0     8873 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/system/particles.py
+-rw-r--r--   0        0        0     3835 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/system/system.py
+-rw-r--r--   0        0        0      168 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/tools/__init__.py
+-rw-r--r--   0        0        0     2430 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/tools/tools.py
+-rw-r--r--   0        0        0     3083 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/tools/xyz.py
+-rw-r--r--   0        0        0      102 2023-07-18 10:44:13.661090 turtlemd-2023.2.dev2/turtlemd/version.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 turtlemd-2023.2.dev2/PKG-INFO
```

### Comparing `turtlemd-2023.2.dev1/LICENSE` & `turtlemd-2023.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/pyproject.toml` & `turtlemd-2023.2.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turtlemd"
-version = "2023.2.dev1"
+version = "2023.2.dev2"
 description = "A slow molecular dynamics library for testing"
 authors = ["Anders Lervik <andersle@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `turtlemd-2023.2.dev1/turtlemd/integrators.py` & `turtlemd-2023.2.dev2/turtlemd/integrators.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/potentials/jax_bondedinteractions.py` & `turtlemd-2023.2.dev2/turtlemd/potentials/jax_bondedinteractions.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/potentials/lennardjones.py` & `turtlemd-2023.2.dev2/turtlemd/potentials/lennardjones.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/potentials/potential.py` & `turtlemd-2023.2.dev2/turtlemd/potentials/potential.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/potentials/well.py` & `turtlemd-2023.2.dev2/turtlemd/potentials/well.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/simulation/mdsimulation.py` & `turtlemd-2023.2.dev2/turtlemd/simulation/mdsimulation.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/simulation/stopping.py` & `turtlemd-2023.2.dev2/turtlemd/simulation/stopping.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/system/box.py` & `turtlemd-2023.2.dev2/turtlemd/system/box.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/system/particles.py` & `turtlemd-2023.2.dev2/turtlemd/system/particles.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/system/system.py` & `turtlemd-2023.2.dev2/turtlemd/system/system.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/tools/tools.py` & `turtlemd-2023.2.dev2/turtlemd/tools/tools.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/turtlemd/tools/xyz.py` & `turtlemd-2023.2.dev2/turtlemd/tools/xyz.py`

 * *Files identical despite different names*

### Comparing `turtlemd-2023.2.dev1/PKG-INFO` & `turtlemd-2023.2.dev2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turtlemd
-Version: 2023.2.dev1
+Version: 2023.2.dev2
 Summary: A slow molecular dynamics library for testing
 License: MIT
 Author: Anders Lervik
 Author-email: andersle@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

