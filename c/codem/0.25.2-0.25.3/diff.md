# Comparing `tmp/codem-0.25.2.tar.gz` & `tmp/codem-0.25.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codem-0.25.2.tar", last modified: Tue Jul 11 17:45:55 2023, max compression
+gzip compressed data, was "codem-0.25.3.tar", last modified: Mon Jul 17 22:38:37 2023, max compression
```

## Comparing `codem-0.25.2.tar` & `codem-0.25.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.871037 codem-0.25.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 17:45:37.000000 codem-0.25.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-11 17:45:55.871037 codem-0.25.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-11 17:45:38.000000 codem-0.25.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-11 17:45:38.000000 codem-0.25.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:45:55.871037 codem-0.25.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.863037 codem-0.25.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/lib/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32538 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/preprocessing/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem/registration/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/registration/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)    24882 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/registration/dsm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-07-11 17:45:38.000000 codem-0.25.2/src/codem/registration/icp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/codem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 17:45:55.000000 codem-0.25.2/src/codem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/vcd/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/vcd/meshing/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/meshing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/meshing/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.867037 codem-0.25.2/src/vcd/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-07-11 17:45:38.000000 codem-0.25.2/src/vcd/preprocessing/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:55.871037 codem-0.25.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-11 17:45:38.000000 codem-0.25.2/tests/test_registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.470859 codem-0.25.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 22:38:18.000000 codem-0.25.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-17 22:38:37.470859 codem-0.25.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-17 22:38:18.000000 codem-0.25.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-17 22:38:18.000000 codem-0.25.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:38:37.474860 codem-0.25.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.466859 codem-0.25.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.466859 codem-0.25.3/src/codem/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.470859 codem-0.25.3/src/codem/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/lib/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.470859 codem-0.25.3/src/codem/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32560 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/preprocessing/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.470859 codem-0.25.3/src/codem/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/registration/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25113 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/registration/dsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-17 22:38:18.000000 codem-0.25.3/src/codem/registration/icp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.470859 codem-0.25.3/src/codem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-17 22:38:37.000000 codem-0.25.3/src/codem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 22:38:37.000000 codem-0.25.3/src/codem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:38:37.000000 codem-0.25.3/src/codem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 22:38:37.000000 codem-0.25.3/src/codem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:38:37.000000 codem-0.25.3/src/codem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 22:38:37.000000 codem-0.25.3/src/codem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 22:38:37.000000 codem-0.25.3/src/codem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.470859 codem-0.25.3/src/vcd/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-17 22:38:18.000000 codem-0.25.3/src/vcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-07-17 22:38:18.000000 codem-0.25.3/src/vcd/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.470859 codem-0.25.3/src/vcd/meshing/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 22:38:18.000000 codem-0.25.3/src/vcd/meshing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-17 22:38:18.000000 codem-0.25.3/src/vcd/meshing/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.470859 codem-0.25.3/src/vcd/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-17 22:38:18.000000 codem-0.25.3/src/vcd/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-07-17 22:38:18.000000 codem-0.25.3/src/vcd/preprocessing/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:38:37.470859 codem-0.25.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-17 22:38:18.000000 codem-0.25.3/tests/test_registration.py
```

### Comparing `codem-0.25.2/LICENSE` & `codem-0.25.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codem-0.25.2/PKG-INFO` & `codem-0.25.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codem
-Version: 0.25.2
+Version: 0.25.3
 Summary: A package for co-registering geospatial data
 Author: Jesse Shanahan, Bahirah Adewunmi
 Author-email: Preston Hartzell <pjhartzell@uh.edu>
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/NCALM-UH/CODEM
 Project-URL: repository, https://github.com/NCALM-UH/CODEM
```

### Comparing `codem-0.25.2/pyproject.toml` & `codem-0.25.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codem-0.25.2/readme.md` & `codem-0.25.3/readme.md`

 * *Files identical despite different names*

### Comparing `codem-0.25.2/src/codem/lib/log.py` & `codem-0.25.3/src/codem/lib/log.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.2/src/codem/main.py` & `codem-0.25.3/src/codem/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import yaml
+from codem import __version__
 from codem.lib.log import Log
 from codem.preprocessing.preprocess import clip_data
 from codem.preprocessing.preprocess import GeoData
 from codem.preprocessing.preprocess import instantiate
 from codem.registration import ApplyRegistration
 from codem.registration import DsmRegistration
 from codem.registration import IcpRegistration
@@ -299,14 +300,20 @@
         "-ts",
         action="store_true",
         help=(
             "Limits the registration search to the region of overlap. Both datasets "
             "must have the same CRS defined."
         ),
     )
+    ap.add_argument(
+        "--version",
+        action="version",
+        version=f"{__version__}",
+        help="Display codem version information",
+    )
     return ap.parse_args()
 
 
 def create_config(args: argparse.Namespace) -> Dict[str, Any]:
     config = CodemRunConfig(
         os.fsdecode(os.path.abspath(args.foundation_file)),
         os.fsdecode(os.path.abspath(args.aoi_file)),
```

### Comparing `codem-0.25.2/src/codem/preprocessing/preprocess.py` & `codem-0.25.3/src/codem/preprocessing/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,16 @@
         """
         dsm_array = np.array(self.dsm)
         if self.nodata is not None:
             empty_array = np.full(dsm_array.shape, self.nodata)
         else:
             empty_array = np.empty_like(dsm_array)
 
-        assert not np.array_equal(dsm_array, empty_array), "DSM array is empty."
+        if np.array_equal(dsm_array, empty_array):
+            raise ValueError("DSM array is empty.")
 
         infilled = np.copy(self.dsm)
         mask = self._get_nodata_mask(infilled)
         infill_mask = np.copy(mask)
 
         while np.sum(infill_mask) < infill_mask.size:
             infilled = rasterio.fill.fillnodata(infilled, mask=infill_mask)
```

### Comparing `codem-0.25.2/src/codem/registration/apply.py` & `codem-0.25.3/src/codem/registration/apply.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.2/src/codem/registration/dsm.py` & `codem-0.25.3/src/codem/registration/dsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
   transformation (no scale factor) between two sets of 3D points.
 * Scaled3dSimilarityTransform: a class for solving the 7-parameter
   transformation (includes a scale factor) between two sets of 3D points.
 """
 import logging
 import math
 import os
+import warnings
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Tuple
 
 import cv2
 import numpy as np
@@ -247,21 +248,29 @@
             )
         if model is None:
             raise ValueError(
                 "ransac model not fitted, no inliers found. Consider tuning "
                 "DSM_RANSAC_THRESHOLD or DSM_RANSAC_MAX_ITER"
             )
         self.logger.info(f"{np.sum(inliers)} keypoint matches found.")
-        assert np.sum(inliers) >= 4, "Less than four keypoint matches found."
+
+        if np.sum(inliers) < 4:
+            raise RuntimeError("Less than 4 keypoint matches found.")
 
         T: np.ndarray = model.transform
         c = np.linalg.norm(T[:, 0])
-        assert (
-            c > 0.67 and c < 1.5
-        ), "Solved scale difference between foundation and AOI data exceeds 50%"
+        if c < 0.67 or c > 1.5:
+            warnings.warn(
+                (
+                    "Coarse regsistration solved scale between datasets exceeds 50%. "
+                    "Registration is likely to fail"
+                ),
+                category=RuntimeWarning,
+                stacklevel=2,
+            )
 
         self.transformation = T
         self.inliers = inliers
         self.fnd_inliers_xyz = fnd_xyz[inliers]
         self.aoi_inliers_xyz = aoi_xyz[inliers]
 
     def _save_match_img(self) -> None:
```

### Comparing `codem-0.25.2/src/codem/registration/icp.py` & `codem-0.25.3/src/codem/registration/icp.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 * IcpRegistration: a class for point cloud to point cloud registration
 """
 from __future__ import annotations
 
 import logging
 import math
 import os
+import warnings
 from typing import Any
 from typing import Dict
 from typing import Tuple
 from typing import TYPE_CHECKING
 
 import numpy as np
 from codem.preprocessing.preprocess import GeoData
@@ -71,25 +72,32 @@
         self.resolution = aoi_obj.resolution
         self.initial_transform = dsm_reg.registration_parameters["matrix"]
         self.outlier_thresh = dsm_reg.registration_parameters["rmse_3d"]
         self.config = config
         self.residual_origins: np.ndarray = np.empty((0, 0), np.double)
         self.residual_vectors: np.ndarray = np.empty((0, 0), np.double)
 
-        assert (
-            self.fixed.shape[1] == 3
-            and self.moving.shape[1] == 3
-            and self.normals.shape[1] == 3
-        ), "Point and normal vector data must be 3D."
-        assert (
-            self.fixed.shape[0] >= 7 and self.moving.shape[0] >= 7
-        ), "At least 7 points required for the point to plane ICP algorithm."
-        assert (
-            self.normals.shape == self.fixed.shape
-        ), "Normal vector array must be same size as fixed points array."
+        if not all(
+            [
+                self.fixed.shape[1] == 3,
+                self.moving.shape[1] == 3,
+                self.normals.shape[1] == 3,
+            ]
+        ):
+            raise ValueError("Point and Normal Vector Must be 3D")
+
+        if self.fixed.shape[0] < 7 or self.moving.shape[0] < 7:
+            raise ValueError(
+                "At least 7 points required for hte point to plane ICP algorithm."
+            )
+
+        if self.normals.shape != self.fixed.shape:
+            raise ValueError(
+                "Normal vector array must be same size as fixed points array."
+            )
 
     def register(self) -> None:
         """
         Executes ICP by minimizing point-to-plane distances:
         * Find fixed point closest to each moving point
         * Find the transform that minimizes the projected distance between each
         paired fixed and moving point, where the projection is to the fixed
@@ -127,17 +135,18 @@
 
             include_fixed = idx[idx < fixed.shape[0]]
             include_moving = idx < fixed.shape[0]
             temp_fixed = fixed[include_fixed]
             temp_normals = self.normals[include_fixed]
             temp_moving_transformed = moving_transformed[include_moving]
 
-            assert (
-                temp_fixed.shape[0] >= 7
-            ), "At least 7 points within the ICP outlier threshold are required."
+            if temp_fixed.shape[0] < 7:
+                raise RuntimeError(
+                    "At least 7 points within the ICP outlier threshold are required."
+                )
 
             weights = self._get_weights(
                 temp_fixed, temp_normals, temp_moving_transformed, alpha, beta
             )
             alpha -= tau
 
             if self.config["ICP_SOLVE_SCALE"]:
@@ -187,17 +196,23 @@
         pre_transform[:3, 3] = -fixed_mean
         post_transform = np.eye(4)
         post_transform[:3, 3] = fixed_mean
         icp_transform = post_transform @ cumulative_transform @ pre_transform
 
         T = icp_transform @ self.initial_transform
         c = np.sqrt(T[0, 0] ** 2 + T[1, 0] ** 2 + T[2, 0] ** 2)
-        assert (
-            c > 0.67 and c < 1.5
-        ), "Solved scale difference between foundation and AOI data exceeds 50%."
+        if c < 0.67 or c > 1.5:
+            warnings.warn(
+                (
+                    "Coarse regsistration solved scale between datasets exceeds 50%. "
+                    "Registration is likely to fail"
+                ),
+                category=RuntimeWarning,
+                stacklevel=2,
+            )
         if self.config["ICP_SAVE_RESIDUALS"]:
             self.residual_origins = self._apply_transform(self.moving, T)
             self.residual_vectors = self._residuals(
                 fixed_tree, fixed, self.normals, moving_transformed
             )
 
         self.transformation = T
@@ -281,15 +296,18 @@
             4x4 transformation matrix to apply to points
 
         Returns
         -------
         transformed_points: np.array
             Array of transformed 3D points
         """
-        assert transform.shape == (4, 4), "Transformation matrix is an invalid shape"
+        if transform.shape != (4, 4):
+            raise ValueError(
+                f"Transformation matrix is an invalid shape: {transform.shape}"
+            )
         points = np.hstack((points, np.ones((points.shape[0], 1))))
         transformed_points: np.ndarray = np.transpose(transform @ points.T)[:, 0:3]
         return transformed_points
 
     def _scaled(
         self, fixed: np.ndarray, normals: np.ndarray, moving: np.ndarray, weights: diags
     ) -> Tuple[np.ndarray, float, float]:
```

### Comparing `codem-0.25.2/src/codem.egg-info/PKG-INFO` & `codem-0.25.3/src/codem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codem
-Version: 0.25.2
+Version: 0.25.3
 Summary: A package for co-registering geospatial data
 Author: Jesse Shanahan, Bahirah Adewunmi
 Author-email: Preston Hartzell <pjhartzell@uh.edu>
 Maintainer-email: Ognyan Moore <ogi@hobu.co>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/NCALM-UH/CODEM
 Project-URL: repository, https://github.com/NCALM-UH/CODEM
```

### Comparing `codem-0.25.2/src/codem.egg-info/SOURCES.txt` & `codem-0.25.3/src/codem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codem-0.25.2/src/vcd/main.py` & `codem-0.25.3/src/vcd/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import yaml
+from codem import __version__
 from codem.lib.log import Log
 from distutils.util import strtobool
 from vcd.meshing.mesh import Mesh
 from vcd.preprocessing.preprocess import PointCloud
 from vcd.preprocessing.preprocess import VCD
 from vcd.preprocessing.preprocess import VCDParameters
 
@@ -205,14 +206,20 @@
         "--compute_hag",
         action="store_true",
         help=(
             "Compute height above ground between after scan (non-ground) and before "
             "scan (ground), otherwise compute to nearest neighbor from after to before."
         ),
     )
+    ap.add_argument(
+        "--version",
+        action="version",
+        version=f"{__version__}",
+        help="Display codem version information",
+    )
     args = ap.parse_args()
     return args
 
 
 def create_config(args: argparse.Namespace) -> Dict[str, Any]:
     config = VcdRunConfig(
         os.fsdecode(os.path.abspath(args.before)),
```

### Comparing `codem-0.25.2/src/vcd/meshing/mesh.py` & `codem-0.25.3/src/vcd/meshing/mesh.py`

 * *Files identical despite different names*

### Comparing `codem-0.25.2/src/vcd/preprocessing/preprocess.py` & `codem-0.25.3/src/vcd/preprocessing/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             filters |= pdal.Filter.outlier(where="Classification!=7")
             filters |= pdal.Filter.range(limits="Classification![7:7]")
             filters |= pdal.Filter.assign(assignment="Classification[:]=1")
             filters |= pdal.Filter.smrf()
 
         else:
             filters |= pdal.Filter.returns(groups="only")
-        
+
         filters.execute()
         self.pipeline = filters
         return filters
 
 
 class VCD:
     def __init__(self, before: PointCloud, after: PointCloud) -> None:
@@ -188,64 +188,73 @@
 
     def compute_indexes(self) -> None:
         after = self.after.df
         before = self.before.df
 
         # Compute height as delta Z between nearest point in before cloud from the after cloud -- original workflow.
         if not self.before.config["COMPUTE_HAG"]:
-            tree3d = cKDTree(before[["X", "Y", "Z"]])
-            _, i3d = tree3d.query(after[["X", "Y", "Z"]], k=1)
+            tree3d = cKDTree(before[["X", "Y", "Z"]].to_numpy())
+            _, i3d = tree3d.query(after[["X", "Y", "Z"]].to_numpy(), k=1)
             after["dZ3d"] = after.Z - before.iloc[i3d].Z.values
-        
+
         # Compute height as HAG, treating after as non-ground and before as ground -- new workflow.
         else:
             # Assing after non-ground, before ground.
             after["TempClassification"] = 1
             before["TempClassification"] = 2
 
             # Merge clouds.
             allpoints = pd.concat([after, before])
 
             # Stash original classifications, then compute HAG using TempClassification. Pop the original classifications.
             pipeline = pdal.Pipeline(dataframes=[allpoints])
-            pipeline |= pdal.Filter.ferry(dimensions="TempClassification=>Classification")
+            pipeline |= pdal.Filter.ferry(
+                dimensions="TempClassification=>Classification"
+            )
             pipeline |= pdal.Filter.hag_delaunay()
             pipeline.execute()
 
             # Assign HAG as dZ3d and d3 in keeping with the original approach.
             result = pipeline.get_dataframe(0)
             after["dZ3d"] = result["HeightAboveGround"]
 
-
     def cluster(self) -> None:
         after = self.after.df
         gh = self.gh
 
         thresholdFilter = pdal.Filter.range(limits="dZ3d![-{gh}:{gh}]".format(gh=gh))
 
-        conditions = [f"Classification=={id}" for id in self.after.config["CLASS_LABELS"]]
+        conditions = [
+            f"Classification=={id}" for id in self.after.config["CLASS_LABELS"]
+        ]
         expression = " || ".join(conditions)
         rangeFilter = pdal.Filter.expression(expression=expression)
 
         clusterFilter = pdal.Filter.cluster(
             min_points=self.after.config["MIN_POINTS"],
             tolerance=self.after.config["CLUSTER_TOLERANCE"],
         )
 
-        conditions = [f"ClusterID!={id}" for id in self.after.config["CULL_CLUSTER_IDS"]]
+        conditions = [
+            f"ClusterID!={id}" for id in self.after.config["CULL_CLUSTER_IDS"]
+        ]
         expression = " && ".join(conditions)
         clusterIdFilter = pdal.Filter.expression(expression=expression)
 
         array = after.to_records()
-        self.clusters = pdal.Pipeline([thresholdFilter, rangeFilter, clusterFilter, clusterIdFilter], [array])
+        self.clusters = pdal.Pipeline(
+            [thresholdFilter, rangeFilter, clusterFilter, clusterIdFilter], [array]
+        )
         self.clusters.execute()
         cluster_df = pd.DataFrame(self.clusters.arrays[0])
 
         # Encode the size of each cluster as a new dimension for analysis.
-        cluster_df['ClusterSize'] = cluster_df.groupby(['ClusterID'])['ClusterID'].transform('count')
+        cluster_df["ClusterSize"] = cluster_df.groupby(["ClusterID"])[
+            "ClusterID"
+        ].transform("count")
         self.cluster_sizes = cluster_df["ClusterSize"].to_numpy()
 
         p = self.make_product(
             cluster_df.X,
             cluster_df.Y,
             cluster_df.ClusterID,
             description=f"Clusters greater than +/-{gh:.2f} height",
@@ -340,15 +349,17 @@
                 colors.to_rgba_array(colormap(divnorm(array["dZ3d"])))
                 * np.iinfo(np.uint16).max
             ],
             dtype=np.uint16,
         )[0, :, :-1]
 
         array = rfn.append_fields(
-            array, ["Red", "Green", "Blue", "ClusterSize"], [rgb[:, 0], rgb[:, 1], rgb[:, 2], sizes]
+            array,
+            ["Red", "Green", "Blue", "ClusterSize"],
+            [rgb[:, 0], rgb[:, 1], rgb[:, 2], sizes],
         )
 
         crs = self.after.crs
         pipeline = pdal.Writer.las(
             filename=filename,
             extra_dims="all",
             a_srs=crs.to_string() if crs is not None else crs,
```

### Comparing `codem-0.25.2/tests/test_registration.py` & `codem-0.25.3/tests/test_registration.py`

 * *Files identical despite different names*

