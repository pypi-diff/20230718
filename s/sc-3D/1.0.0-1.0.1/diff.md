# Comparing `tmp/sc-3D-1.0.0.tar.gz` & `tmp/sc-3D-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-3D-1.0.0.tar", last modified: Thu Jul  6 10:35:50 2023, max compression
+gzip compressed data, was "sc-3D-1.0.1.tar", last modified: Tue Jul 18 08:48:08 2023, max compression
```

## Comparing `sc-3D-1.0.0.tar` & `sc-3D-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.547548 sc-3D-1.0.0/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-03-29 13:52:28.000000 sc-3D-1.0.0/LICENSE
--rw-r--r--   0 leo.guignard   (501) staff       (20)     7789 2023-07-06 10:35:50.547608 sc-3D-1.0.0/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)     6629 2023-06-21 13:19:01.000000 sc-3D-1.0.0/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      634 2022-08-10 13:34:47.000000 sc-3D-1.0.0/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1562 2023-07-06 10:35:50.547921 sc-3D-1.0.0/setup.cfg
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.544983 sc-3D-1.0.0/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.546246 sc-3D-1.0.0/src/sc3D/
--rw-r--r--   0 leo.guignard   (501) staff       (20)       93 2023-07-06 10:35:39.000000 sc-3D-1.0.0/src/sc3D/__init__.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.546689 sc-3D-1.0.0/src/sc3D/_tests/
--rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-08-10 13:38:51.000000 sc-3D-1.0.0/src/sc3D/_tests/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)      989 2023-02-07 16:44:08.000000 sc-3D-1.0.0/src/sc3D/_tests/test_sc3D.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    94208 2023-07-06 10:16:44.000000 sc-3D-1.0.0/src/sc3D/sc3D.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    11161 2023-07-06 10:21:28.000000 sc-3D-1.0.0/src/sc3D/transformations.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.547447 sc-3D-1.0.0/src/sc_3D.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     7789 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)      329 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       92 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        5 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 08:48:08.743708 sc-3D-1.0.1/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-03-29 13:52:28.000000 sc-3D-1.0.1/LICENSE
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     7843 2023-07-18 08:48:08.743773 sc-3D-1.0.1/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     6683 2023-07-18 08:43:48.000000 sc-3D-1.0.1/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      634 2022-08-10 13:34:47.000000 sc-3D-1.0.1/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1562 2023-07-18 08:48:08.744081 sc-3D-1.0.1/setup.cfg
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 08:48:08.741696 sc-3D-1.0.1/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 08:48:08.742793 sc-3D-1.0.1/src/sc3D/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       93 2023-07-18 08:45:55.000000 sc-3D-1.0.1/src/sc3D/__init__.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 08:48:08.742991 sc-3D-1.0.1/src/sc3D/_tests/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-08-10 13:38:51.000000 sc-3D-1.0.1/src/sc3D/_tests/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      989 2023-02-07 16:44:08.000000 sc-3D-1.0.1/src/sc3D/_tests/test_sc3D.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    94421 2023-07-18 08:42:57.000000 sc-3D-1.0.1/src/sc3D/sc3D.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    11169 2023-07-18 08:42:42.000000 sc-3D-1.0.1/src/sc3D/transformations.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-18 08:48:08.743625 sc-3D-1.0.1/src/sc_3D.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     7843 2023-07-18 08:48:08.000000 sc-3D-1.0.1/src/sc_3D.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      329 2023-07-18 08:48:08.000000 sc-3D-1.0.1/src/sc_3D.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-07-18 08:48:08.000000 sc-3D-1.0.1/src/sc_3D.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       92 2023-07-18 08:48:08.000000 sc-3D-1.0.1/src/sc_3D.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        5 2023-07-18 08:48:08.000000 sc-3D-1.0.1/src/sc_3D.egg-info/top_level.txt
```

### Comparing `sc-3D-1.0.0/LICENSE` & `sc-3D-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sc-3D-1.0.0/PKG-INFO` & `sc-3D-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-3D
-Version: 1.0.0
+Version: 1.0.1
 Summary: Array alignment and 3D differential expression for 3D sc omics
 Home-page: https://github.com/GuignardLab/sc3D
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/sc3D/issues
 Project-URL: Documentation, https://github.com/GuignardLab/sc3D#README.md
@@ -39,15 +39,15 @@
 
 __To access the 3D viewer for sc3D datasets, you can go to the following link: [GuignardLab/napari-sc3D-viewer](https://github.com/GuignardLab/napari-sc3D-viewer)__
 
 You can find it on the Guignard Lab GitHub page: [GuignardLab/sc3D](https://github.com/GuignardLab/sc3D). In there you will be able to find jupyter notebooks giving examples about how to use the datasets.
 
 This code was developed in the context of the following study:
 
-**Spatial transcriptomic maps of whole mouse embryos.** *Abhishek Sampath Kumar, Luyi Tian, Adriano Bolondi et al.*
+[**Spatial transcriptomic maps of whole mouse embryos.**](https://www.nature.com/articles/s41588-023-01435-6) *Abhishek Sampath Kumar, Luyi Tian, Adriano Bolondi et al.*
 
 The __sc3D__ code is based on the [anndata](https://anndata.readthedocs.io/en/latest/) and [Scanpy](https://scanpy.readthedocs.io/en/stable/) libraries and allows to read, register arrays and compute 3D differential expression.
 
 The dataset necessary to run the tests and look at the results can be downloaded [there](https://figshare.com/s/9c73df7fd39e3ca5422d) for the unregistered dataset (and test the provided algorithms) and [there](https://figshare.com/s/1c29d867bc8b90d754d2) for the already registered atlas to browse with our visualiser. You can find the visualiser [there](https://www.github.com/guignardlab/napari-sc3d-viewer).
 
 ## Description of the GitHub repository
```

### Comparing `sc-3D-1.0.0/README.md` & `sc-3D-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 __To access the 3D viewer for sc3D datasets, you can go to the following link: [GuignardLab/napari-sc3D-viewer](https://github.com/GuignardLab/napari-sc3D-viewer)__
 
 You can find it on the Guignard Lab GitHub page: [GuignardLab/sc3D](https://github.com/GuignardLab/sc3D). In there you will be able to find jupyter notebooks giving examples about how to use the datasets.
 
 This code was developed in the context of the following study:
 
-**Spatial transcriptomic maps of whole mouse embryos.** *Abhishek Sampath Kumar, Luyi Tian, Adriano Bolondi et al.*
+[**Spatial transcriptomic maps of whole mouse embryos.**](https://www.nature.com/articles/s41588-023-01435-6) *Abhishek Sampath Kumar, Luyi Tian, Adriano Bolondi et al.*
 
 The __sc3D__ code is based on the [anndata](https://anndata.readthedocs.io/en/latest/) and [Scanpy](https://scanpy.readthedocs.io/en/stable/) libraries and allows to read, register arrays and compute 3D differential expression.
 
 The dataset necessary to run the tests and look at the results can be downloaded [there](https://figshare.com/s/9c73df7fd39e3ca5422d) for the unregistered dataset (and test the provided algorithms) and [there](https://figshare.com/s/1c29d867bc8b90d754d2) for the already registered atlas to browse with our visualiser. You can find the visualiser [there](https://www.github.com/guignardlab/napari-sc3d-viewer).
 
 ## Description of the GitHub repository
```

### Comparing `sc-3D-1.0.0/pyproject.toml` & `sc-3D-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sc-3D-1.0.0/setup.cfg` & `sc-3D-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sc-3D
-version = 1.0.0
+version = 1.0.1
 author = Leo Guignard
 author_email = leo.guignard@univ-amu.fr
 url = https://github.com/GuignardLab/sc3D
 license = MIT
 description = Array alignment and 3D differential expression for 3D sc omics
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `sc-3D-1.0.0/src/sc3D/_tests/test_sc3D.py` & `sc-3D-1.0.1/src/sc3D/_tests/test_sc3D.py`

 * *Files identical despite different names*

### Comparing `sc-3D-1.0.0/src/sc3D/sc3D.py` & `sc-3D-1.0.1/src/sc3D/sc3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from seaborn import scatterplot
 import json
 from pathlib import Path
 
 import anndata
 from sc3D.transformations import transformations as tr
 
+
 class Embryo:
     """
     Embryo class to handle samples from 3D spatial
     single cell omics. It was initially designed with
     a specific dataset in mind but it should work
     for other kinds of datasets.
     """
@@ -989,22 +990,27 @@
                 else:
                     M_raw_filtered = raw_data.copy()
             else:
                 M_raw_filtered = raw_data.copy()
 
             all_cs_names = sorted(self.anndata.obs[self.array_id].unique())
             exp = re.compile("[0-9]+")
-            init_cs_numbers = [int(exp.findall(x)[self.array_id_num_pos]) for x in all_cs_names]
+            init_cs_numbers = [
+                int(exp.findall(x)[self.array_id_num_pos])
+                for x in all_cs_names
+            ]
             num_to_name = dict(zip(init_cs_numbers, all_cs_names))
-            M_raw_filtered.obsm['spatial'] = M_raw_filtered.obsm[self.pos_id]
+            M_raw_filtered.obsm["spatial"] = M_raw_filtered.obsm[self.pos_id]
             slices_id = sorted(cs_to_treat)
             slices = []
             for s_id in slices_id:
                 slices.append(
-                    M_raw_filtered[M_raw_filtered.obs[self.array_id] == num_to_name[s_id]]
+                    M_raw_filtered[
+                        M_raw_filtered.obs[self.array_id] == num_to_name[s_id]
+                    ]
                 )
             if timing:
                 start = time()
             times = []
             pis = []
             if timing:
                 current_time = time()
@@ -2318,15 +2324,18 @@
         self.diff_expressed_3D = {}
         self.tissues_diff_expre_processed = None
         self.umap_id = umap_id
         self.array_id = array_id
         self.pos_id = pos_id
         self.__diff_expr_processed = {}
 
-        if Path(data_path).suffix in [".h5ad", ".h5", ".csv"]:
+        if Path(data_path).suffix in [".h5ad", ".h5", ".csv"] or (
+            0 < len(sample_list)
+            and Path(sample_list[0]).suffix in [".h5ad", ".h5", ".csv"]
+        ):
             self.read_anndata(
                 data_path,
                 xy_resolution=xy_resolution,
                 genes_of_interest=genes_of_interest,
                 store_anndata=store_anndata,
                 tissue_id=tissue_id,
                 array_id=array_id,
```

### Comparing `sc-3D-1.0.0/src/sc3D/transformations.py` & `sc-3D-1.0.1/src/sc3D/transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Léo
 """
 
 import numpy as np
 import math
 
+
 class transformations:
     _EPS = np.finfo(float).eps * 4.0
 
     @classmethod
     def unit_vector(clf, data, axis=None, out=None):
         """Return ndarray normalized by length, i.e. Euclidean norm, along axis.
 
@@ -56,15 +57,15 @@
         np.sqrt(length, length)
         if axis is not None:
             length = np.expand_dims(length, axis)
         data /= length
         if out is None:
             return data
         return None
-    
+
     @classmethod
     def rotation_matrix(clf, angle, direction, point=None):
         """Return matrix to rotate about axis defined by point and direction.
 
         >>> R = rotation_matrix(math.pi/2, [0, 0, 1], [1, 0, 0])
         >>> numpy.allclose(numpy.dot(R, [0, 0, 0, 1]), [1, -1, 0, 1])
         True
@@ -84,14 +85,15 @@
         True
         >>> numpy.allclose(2, numpy.trace(rotation_matrix(math.pi/2,
         ...                                               direc, point)))
         True
 
         """
         import math
+
         sina = math.sin(angle)
         cosa = math.cos(angle)
         direction = clf.unit_vector(direction[:3])
         # rotation matrix around unit vector
         R = np.diag([cosa, cosa, cosa])
         R += np.outer(direction, direction) * (1.0 - cosa)
         direction *= sina
@@ -105,15 +107,15 @@
         M = np.identity(4)
         M[:3, :3] = R
         if point is not None:
             # rotation not around origin
             point = np.array(point[:3], dtype=np.float64, copy=False)
             M[:3, 3] = point - np.dot(R, point)
         return M
-    
+
     @classmethod
     def vector_norm(clf, data, axis=None, out=None):
         """Return length, i.e. Euclidean norm, of ndarray along axis.
 
         >>> v = numpy.random.random(3)
         >>> n = vector_norm(v)
         >>> numpy.allclose(n, numpy.linalg.norm(v))
@@ -191,15 +193,17 @@
                     0.0,
                 ],
                 [0.0, 0.0, 0.0, 1.0],
             ]
         )
 
     @classmethod
-    def affine_matrix_from_points(clf, v0, v1, shear=True, scale=True, usesvd=True):
+    def affine_matrix_from_points(
+        clf, v0, v1, shear=True, scale=True, usesvd=True
+    ):
         """Return affine transform matrix to register two point sets.
 
         v0 and v1 are shape (ndims, -1) arrays of at least ndims non-homogeneous
         coordinates, where ndims is the dimensionality of the coordinate space.
 
         If shear is False, a similarity transformation matrix is returned.
         If also scale is False, a rigid/Euclidean transformation matrix
@@ -237,27 +241,26 @@
 
         """
         v0 = np.array(v0, dtype=np.float64, copy=True)
         v1 = np.array(v1, dtype=np.float64, copy=True)
 
         ndims = v0.shape[0]
         if ndims < 2 or v0.shape[1] < ndims or v0.shape != v1.shape:
-            raise ValueError('input arrays are of wrong shape or type')
+            raise ValueError("input arrays are of wrong shape or type")
 
         # move centroids to origin
         t0 = -np.mean(v0, axis=1)
         M0 = np.identity(ndims + 1)
         M0[:ndims, ndims] = t0
         v0 += t0.reshape(ndims, 1)
         t1 = -np.mean(v1, axis=1)
         M1 = np.identity(ndims + 1)
         M1[:ndims, ndims] = t1
         v1 += t1.reshape(ndims, 1)
 
-
         if shear:
             # Affine transformation
             A = np.concatenate((v0, v1), axis=0)
             u, s, vh = np.linalg.svd(A.T)
             vh = vh[:ndims].T
             B = vh[:ndims]
             C = vh[ndims : 2 * ndims]
@@ -300,8 +303,8 @@
             v0 *= v0
             v1 *= v1
             M[:ndims, :ndims] *= math.sqrt(np.sum(v1) / np.sum(v0))
 
         # move centroids back
         M = np.dot(np.linalg.inv(M1), np.dot(M, M0))
         M /= M[ndims, ndims]
-        return M
+        return M
```

### Comparing `sc-3D-1.0.0/src/sc_3D.egg-info/PKG-INFO` & `sc-3D-1.0.1/src/sc_3D.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-3D
-Version: 1.0.0
+Version: 1.0.1
 Summary: Array alignment and 3D differential expression for 3D sc omics
 Home-page: https://github.com/GuignardLab/sc3D
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/sc3D/issues
 Project-URL: Documentation, https://github.com/GuignardLab/sc3D#README.md
@@ -39,15 +39,15 @@
 
 __To access the 3D viewer for sc3D datasets, you can go to the following link: [GuignardLab/napari-sc3D-viewer](https://github.com/GuignardLab/napari-sc3D-viewer)__
 
 You can find it on the Guignard Lab GitHub page: [GuignardLab/sc3D](https://github.com/GuignardLab/sc3D). In there you will be able to find jupyter notebooks giving examples about how to use the datasets.
 
 This code was developed in the context of the following study:
 
-**Spatial transcriptomic maps of whole mouse embryos.** *Abhishek Sampath Kumar, Luyi Tian, Adriano Bolondi et al.*
+[**Spatial transcriptomic maps of whole mouse embryos.**](https://www.nature.com/articles/s41588-023-01435-6) *Abhishek Sampath Kumar, Luyi Tian, Adriano Bolondi et al.*
 
 The __sc3D__ code is based on the [anndata](https://anndata.readthedocs.io/en/latest/) and [Scanpy](https://scanpy.readthedocs.io/en/stable/) libraries and allows to read, register arrays and compute 3D differential expression.
 
 The dataset necessary to run the tests and look at the results can be downloaded [there](https://figshare.com/s/9c73df7fd39e3ca5422d) for the unregistered dataset (and test the provided algorithms) and [there](https://figshare.com/s/1c29d867bc8b90d754d2) for the already registered atlas to browse with our visualiser. You can find the visualiser [there](https://www.github.com/guignardlab/napari-sc3d-viewer).
 
 ## Description of the GitHub repository
```

