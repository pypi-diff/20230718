# Comparing `tmp/abm_shape_collection-0.7.0.tar.gz` & `tmp/abm_shape_collection-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abm_shape_collection-0.7.0.tar", max compression
+gzip compressed data, was "abm_shape_collection-0.7.1.tar", max compression
```

## Comparing `abm_shape_collection-0.7.0.tar` & `abm_shape_collection-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1540 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/LICENSE
--rw-r--r--   0        0        0     2573 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/README.md
--rw-r--r--   0        0        0     1933 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1347 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/__main__.py
--rw-r--r--   0        0        0     2898 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/calculate_shape_stats.py
--rw-r--r--   0        0        0     2765 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/calculate_size_stats.py
--rw-r--r--   0        0        0      777 2023-07-14 21:32:00.106938 abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_array.py
--rw-r--r--   0        0        0     1016 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_coeffs.py
--rw-r--r--   0        0        0      576 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_points.py
--rw-r--r--   0        0        0     2384 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/extract_mesh_projections.py
--rw-r--r--   0        0        0      582 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/extract_mesh_wireframe.py
--rw-r--r--   0        0        0     3058 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/extract_shape_modes.py
--rw-r--r--   0        0        0      508 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/fit_pca_model.py
--rw-r--r--   0        0        0      611 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/get_shape_coefficients.py
--rw-r--r--   0        0        0      352 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/get_shape_properties.py
--rw-r--r--   0        0        0     1228 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/make_voxels_array.py
--rw-r--r--   0        0        0        0 2023-07-14 21:32:00.110938 abm_shape_collection-0.7.0/src/abm_shape_collection/py.typed
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 abm_shape_collection-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1540 2023-07-18 18:27:20.195493 abm_shape_collection-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2573 2023-07-18 18:27:20.195493 abm_shape_collection-0.7.1/README.md
+-rw-r--r--   0        0        0     1933 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1347 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/__main__.py
+-rw-r--r--   0        0        0     2898 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/calculate_shape_stats.py
+-rw-r--r--   0        0        0     2765 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/calculate_size_stats.py
+-rw-r--r--   0        0        0      777 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/construct_mesh_from_array.py
+-rw-r--r--   0        0        0     1016 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/construct_mesh_from_coeffs.py
+-rw-r--r--   0        0        0      576 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/construct_mesh_from_points.py
+-rw-r--r--   0        0        0     2384 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/extract_mesh_projections.py
+-rw-r--r--   0        0        0      582 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/extract_mesh_wireframe.py
+-rw-r--r--   0        0        0     3058 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/extract_shape_modes.py
+-rw-r--r--   0        0        0      508 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/fit_pca_model.py
+-rw-r--r--   0        0        0      611 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/get_shape_coefficients.py
+-rw-r--r--   0        0        0      352 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/get_shape_properties.py
+-rw-r--r--   0        0        0     1228 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/make_voxels_array.py
+-rw-r--r--   0        0        0        0 2023-07-18 18:27:20.199493 abm_shape_collection-0.7.1/src/abm_shape_collection/py.typed
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 abm_shape_collection-0.7.1/PKG-INFO
```

### Comparing `abm_shape_collection-0.7.0/LICENSE` & `abm_shape_collection-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/README.md` & `abm_shape_collection-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/pyproject.toml` & `abm_shape_collection-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "abm-shape-collection"
-version = "0.7.0"
+version = "0.7.1"
 description = "Collection of tasks for analyzing cell shapes."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 prefect = "^2.8.2"
 numpy = "^1.24.2"
 pandas = "^1.5.3"
-aicsshparam = "^0.1.6"
+aicsshparam = "^0.1.7"
 vtk = "^9.2.5"
 trimesh = "^3.18.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
```

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/__init__.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/calculate_shape_stats.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/calculate_shape_stats.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/calculate_size_stats.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/calculate_size_stats.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_array.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/construct_mesh_from_array.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_coeffs.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/construct_mesh_from_coeffs.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/construct_mesh_from_points.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/construct_mesh_from_points.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/extract_mesh_projections.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/extract_mesh_projections.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/extract_mesh_wireframe.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/extract_mesh_wireframe.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/extract_shape_modes.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/extract_shape_modes.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/get_shape_coefficients.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/get_shape_coefficients.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/src/abm_shape_collection/make_voxels_array.py` & `abm_shape_collection-0.7.1/src/abm_shape_collection/make_voxels_array.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.7.0/PKG-INFO` & `abm_shape_collection-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: abm-shape-collection
-Version: 0.7.0
+Version: 0.7.1
 Summary: Collection of tasks for analyzing cell shapes.
 License: BSD-3-Clause
 Author: Jessica S. Yu
 Author-email: jesyu@uw.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aicsshparam (>=0.1.6,<0.2.0)
+Requires-Dist: aicsshparam (>=0.1.7,<0.2.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: prefect (>=2.8.2,<3.0.0)
 Requires-Dist: trimesh (>=3.18.3,<4.0.0)
 Requires-Dist: vtk (>=9.2.5,<10.0.0)
 Description-Content-Type: text/markdown
```

