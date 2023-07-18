# Comparing `tmp/pewlib-0.7.3.tar.gz` & `tmp/pewlib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pewlib-0.7.3.tar", last modified: Wed Dec  8 05:04:11 2021, max compression
+gzip compressed data, was "pewlib-0.8.0.tar", last modified: Tue Jul 18 06:13:28 2023, max compression
```

## Comparing `pewlib-0.7.3.tar` & `pewlib-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 05:04:11.261598 pewlib-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-12-08 05:03:56.000000 pewlib-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      873 2021-12-08 05:04:11.261598 pewlib-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      443 2021-12-08 05:03:56.000000 pewlib-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 05:04:11.249598 pewlib-0.7.3/pewlib/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8129 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 05:04:11.257598 pewlib-0.7.3/pewlib/io/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21986 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/io/agilent.py
--rw-r--r--   0 runner    (1001) docker     (121)     7494 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     3604 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/io/npz.py
--rw-r--r--   0 runner    (1001) docker     (121)     2945 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/io/perkinelmer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/io/textimage.py
--rw-r--r--   0 runner    (1001) docker     (121)     7640 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/io/thermo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/io/vtk.py
--rw-r--r--   0 runner    (1001) docker     (121)     4905 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/laser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 05:04:11.261598 pewlib-0.7.3/pewlib/process/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5990 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/process/calc.py
--rw-r--r--   0 runner    (1001) docker     (121)     6651 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/process/colocal.py
--rw-r--r--   0 runner    (1001) docker     (121)    11597 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/process/convolve.py
--rw-r--r--   0 runner    (1001) docker     (121)     5017 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/process/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    14612 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/process/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (121)     6984 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/process/register.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/process/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 05:04:11.261598 pewlib-0.7.3/pewlib/srr/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/srr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5276 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/srr/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     9088 2021-12-08 05:03:56.000000 pewlib-0.7.3/pewlib/srr/srr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 05:04:11.249598 pewlib-0.7.3/pewlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      873 2021-12-08 05:04:10.000000 pewlib-0.7.3/pewlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      687 2021-12-08 05:04:11.000000 pewlib-0.7.3/pewlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-08 05:04:10.000000 pewlib-0.7.3/pewlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-08 05:04:10.000000 pewlib-0.7.3/pewlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-12-08 05:04:10.000000 pewlib-0.7.3/pewlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-08 05:04:11.261598 pewlib-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      924 2021-12-08 05:03:56.000000 pewlib-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.666656 pewlib-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 06:13:08.000000 pewlib-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-18 06:13:28.666656 pewlib-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-18 06:13:08.000000 pewlib-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.658655 pewlib-0.8.0/pewlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.658655 pewlib-0.8.0/pewlib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/agilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/npz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/perkinelmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/textimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/io/vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/laser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.662655 pewlib-0.8.0/pewlib/process/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/colocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/process/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.662655 pewlib-0.8.0/pewlib/srr/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/srr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/srr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-07-18 06:13:08.000000 pewlib-0.8.0/pewlib/srr/srr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.658655 pewlib-0.8.0/pewlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 06:13:28.000000 pewlib-0.8.0/pewlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:13:28.666656 pewlib-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-18 06:13:08.000000 pewlib-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:13:28.662655 pewlib-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_colocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_io_agilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_io_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_laser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_srr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-18 06:13:08.000000 pewlib-0.8.0/tests/test_threshold.py
```

### Comparing `pewlib-0.7.3/LICENSE` & `pewlib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pewlib-0.7.3/PKG-INFO` & `pewlib-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pewlib
-Version: 0.7.3
+Version: 0.8.0
 Summary: Import, processing and export library for LA-ICP-MS data.
 Home-page: https://github.com/djdt/pewlib
 Author: T. Lockwood
 Author-email: thomas.lockwood@uts.edu.au
-License: UNKNOWN
 Project-URL: Documentation, https://djdt.github.io/pewlib
 Project-URL: Source, https://gtihub.com/djdt/pewlib
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pewlib
 
 ![Build](https://github.com/djdt/pewlib/workflows/Build/badge.svg)
 
@@ -24,9 +22,7 @@
 Pewlib is availble on PyPI and installable via pip.
 
 ```pip install pewlib```
 
 ## Documentation
 
 Documenation is available at <https://djdt.github.io/pewlib>.
-
-
```

### Comparing `pewlib-0.7.3/pewlib/calibration.py` & `pewlib-0.8.0/pewlib/calibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import numpy as np
-
 from typing import Tuple, Union
 
+import numpy as np
+
 
 def weights_from_weighting(
     x: np.ndarray, weighting: str, safe: bool = True
 ) -> np.ndarray:
     """Get weighting for `x`.
 
     Conveience function for calculating simple weightings. If `safe` then any
@@ -31,20 +31,20 @@
     if weighting == "Equal":
         return np.ones_like(x)
     elif weighting == "x":
         return x
     elif weighting == "1/x":
         return 1.0 / x
     elif weighting == "1/(x^2)":
-        return 1.0 / (x ** 2.0)
+        return 1.0 / (x**2.0)
     else:
         raise ValueError(f"Unknown weighting {weighting}.")
 
 
-def weighted_rsq(x: np.ndarray, y: np.ndarray, w: np.ndarray = None) -> float:
+def weighted_rsq(x: np.ndarray, y: np.ndarray, w: np.ndarray | None = None) -> float:
     """Calculate r² for weighted linear regression.
 
     Args:
         x: 1d-array
         y: array, same size as `x`
         w: weights, same size as `x`
     """
@@ -58,15 +58,15 @@
     if np.iscomplexobj(c):  # pragma: no cover
         np.clip(c.imag, -1, 1, out=c.imag)
 
     return c[0, 1] ** 2.0
 
 
 def weighted_linreg(
-    x: np.ndarray, y: np.ndarray, w: np.ndarray = None
+    x: np.ndarray, y: np.ndarray, w: np.ndarray | None = None
 ) -> Tuple[float, float, float, float]:
     """Weighted linear regression.
 
     Uses polyfit with sqrt(weights) for intercept and gradient.
 
     Args:
         x: 1d-array
@@ -111,17 +111,17 @@
     KNOWN_WEIGHTING = ["Equal", "x", "1/x", "1/(x^2)", "y", "1/y", "1/(y^2)"]
 
     def __init__(
         self,
         intercept: float = 0.0,
         gradient: float = 1.0,
         unit: str = "",
-        rsq: float = None,
-        error: float = None,
-        points: np.ndarray = None,
+        rsq: float | None = None,
+        error: float | None = None,
+        points: np.ndarray | None = None,
         weights: Union[str, Tuple[str, np.ndarray]] = "Equal",
     ):
         self.intercept = intercept
         self.gradient = gradient
         self.unit = unit
 
         self.rsq = rsq
@@ -130,15 +130,16 @@
         self._points: np.ndarray = np.empty((0, 2), dtype=np.float64)
         self._weights: np.ndarray = np.empty(0, dtype=np.float64)
         self.weighting: str = ""
 
         if points is not None:
             self.points = points
 
-        self.weights = weights
+        # Set weights via property
+        self.weights = weights  # type: ignore
 
     @property
     def x(self) -> np.ndarray:
         return self._points[:, 0]
 
     @property
     def y(self) -> np.ndarray:
@@ -201,55 +202,61 @@
                 )
             else:
                 x, y, w = self.x[no_nans], self.y[no_nans], self.weights[no_nans]
                 self.gradient, self.intercept, self.rsq, self.error = weighted_linreg(
                     x, y, w
                 )
 
-    def to_array(self) -> np.ndarray:
-        points = self.points
-        unit = np.array(self.unit)
-        weights = np.array(self.weights)
-        weighting = np.array(self.weighting)
+    def to_array(self, size: int | None = None) -> np.ndarray:
+        """Convert to a Numpy array. Points and weights are trimmed or padded with nan to 'size' if passed."""
+        if size is None:
+            size = self.x.shape[0]
+
+        points = np.full((size, 2), np.nan)
+        points[: self.points.shape[0]] = self.points
+        weights = np.full(size, np.nan)
+        weights[: self.weights.shape[0]] = self.weights
+
         return np.array(
             (
                 self.intercept,
                 self.gradient,
-                unit,
+                self.unit,
                 self.rsq,
                 self.error,
                 points,
                 weights,
-                weighting,
+                self.weighting,
             ),
             dtype=[
                 ("intercept", np.float64),
                 ("gradient", np.float64),
-                ("unit", unit.dtype),
+                ("unit", "U32"),
                 ("rsq", np.float64),
                 ("error", np.float64),
-                ("points", points.dtype, points.shape),
-                ("weights", weights.dtype, weights.shape),
-                ("weighting", weighting.dtype),
+                ("points", np.float64, points.shape),
+                ("weights", np.float64, weights.shape),
+                ("weighting", "U32"),
             ],
         )
 
     @classmethod
     def from_array(cls, array: np.ndarray) -> "Calibration":
+        nans = np.isnan(array["weights"]) & np.all(np.isnan(array["points"]), axis=1)
         if array["weighting"] in Calibration.KNOWN_WEIGHTING:
             weights = str(array["weighting"])
         else:
-            weights = (str(array["weighting"]), array["weights"])  # type: ignore
+            weights = (str(array["weighting"]), array["weights"][~nans])  # type: ignore
         return cls(
             intercept=float(array["intercept"]),
             gradient=float(array["gradient"]),
             unit=str(array["unit"]),
             rsq=None if np.isnan(array["rsq"]) else float(array["rsq"]),
             error=None if np.isnan(array["error"]) else float(array["error"]),
-            points=array["points"],
+            points=array["points"][~nans],
             weights=weights,
         )
 
     @classmethod
     def from_points(
         cls,
         points: np.ndarray,
```

### Comparing `pewlib-0.7.3/pewlib/config.py` & `pewlib-0.8.0/pewlib/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import numpy as np
-
 from typing import Tuple
 
+import numpy as np
+
 
 class Config(object):
     """Class for the rastered parameters of image.
 
     Args:
         spotsize: laser-spot diameter, μm
         speed: laser movement speed, μm/s
@@ -58,15 +58,15 @@
 
     Args:
         spotsize: x, y distance between laser-spots, μm
     """
 
     _class = "Spot"
 
-    def __init__(self, spotsize: float = 100.0, spotsize_y: float = None):
+    def __init__(self, spotsize: float = 100.0, spotsize_y: float | None = None):
         super().__init__(spotsize=spotsize, speed=0.0, scantime=0.0)
         if spotsize_y is None:
             spotsize_y = spotsize
         self.spotsize_y = spotsize_y
 
     def to_array(self) -> np.ndarray:
         return np.array(
```

### Comparing `pewlib-0.7.3/pewlib/io/agilent.py` & `pewlib-0.8.0/pewlib/io/agilent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """
 Import of line-by-line collected Agilent '.b' batches.
 Both raw binaries and the '.csv' exports are supported.
 Tested with Agilent 7500, 7700 and 8900 ICPs.
 """
 import logging
-from xml.etree import ElementTree
 from pathlib import Path
+from typing import Callable, Dict, Generator, List, Tuple, Union
+from xml.etree import ElementTree
 
 import numpy as np
 import numpy.lib.recfunctions as rfn
 
-from typing import Callable, Dict, Generator, List, Tuple, Union
-
 logger = logging.getLogger(__name__)
 
 acq_method_xml_path = Path("Method", "AcqMethod.xml")
 batch_csv_path = Path("BatchLog.csv")
 batch_xml_path = Path("Method", "BatchLog.xml")
 
 
 class XSpecificMass(object):
-    def __init__(self, id: int, name: str, acctime: float, mz: int, mz2: int = None):
+    def __init__(
+        self, id: int, name: str, acctime: float, mz: int, mz2: int | None = None
+    ):
         self.id = id
         self.name = name
         self.acctime = acctime
         self.mz = mz
         self.mz2 = mz2
 
     def __str__(self) -> str:
@@ -158,15 +159,18 @@
     offsets = (
         msscan["SpectrumParamValues"]["SpectrumOffset"]
         // msscan["SpectrumParamValues"]["ByteCount"]
     )
     dtype = [(str(mass), np.float64) for mass in masses] + [("Time", np.float64)]
     data = np.empty(offsets.size, dtype=dtype)
     for mass in masses:
-        data[str(mass)] = msprofile[(offsets * len(masses)) + (mass.id - 1)]["Analog"]
+        size = np.minimum(
+            (offsets * len(masses)) + (mass.id - 1), msprofile.shape[0] - 1
+        )
+        data[str(mass)] = msprofile[size]["Analog"]
 
     data["Time"] = msscan["ScanTime"] * 60.0  # ScanTime in minutes
     return data
 
 
 def binary_read_msscan(path: Path):
     msscan_magic_number = 257
@@ -317,17 +321,17 @@
             product = int(msts_index.findtext("ProductIonMZ") or 0)
             xdict[index] = (precursor, product)
     return xdict, scan_type
 
 
 def load_binary(
     path: Union[str, Path],
-    collection_methods: List[str] = None,
+    collection_methods: List[str] | None = None,
     counts_per_second: bool = False,
-    drop_names: List[str] = None,
+    drop_names: List[str] | None = None,
     full: bool = False,
 ) -> Union[np.ndarray, Tuple[np.ndarray, dict]]:
     """Imports an Agilent '.b' batch.
 
     Import is performed using the 'MSScan.bin', 'MSProfile.bin' binaries and
     'MSTS_XSpecific.xml' document.
     By default `drop_names` drops the 'Time' field.
@@ -450,17 +454,17 @@
                 dtype=np.float64,
                 deletechars="",
             )
 
 
 def load_csv(
     path: Union[str, Path],
-    collection_methods: List[str] = None,
+    collection_methods: List[str] | None = None,
     use_acq_for_names: bool = True,
-    drop_names: List[str] = None,
+    drop_names: List[str] | None = None,
     full: bool = False,
 ) -> Union[np.ndarray, Tuple[np.ndarray, dict]]:
     """Imports an Agilent '.b' batch.
 
     Import is performed using the '.csv' files found in each '.d' datafile.
     If a '.csv' can not be found then all data in the line is set to 0.
     To load properly formatted element names use `use_acq_for_names`.
@@ -588,37 +592,35 @@
 
     if isinstance(path, str):  # pragma: no cover
         path = Path(path)
 
     try:
         device_xml = path.glob("*.d/AcqData/Devices.xml")
         info = device_xml_read_info(next(device_xml))
-    except (
-        StopIteration,
-        FileNotFoundError,
-        ElementTree.ParseError,
-    ):  # pragma: no cover
+    except (StopIteration, ElementTree.ParseError):  # pragma: no cover
         logger.warning("Unable to read info from Devices.xml.")
         info = {}
 
     try:
         batch_xml = path.joinpath(batch_xml_path)
+        if not batch_xml.exists():
+            raise FileNotFoundError
         info.update(batch_xml_read_info(batch_xml))
     except (FileNotFoundError, ElementTree.ParseError):  # pragma: no cover
         logger.warning("Unable to read info from BatchLog.xml.")
 
     return {k: v for k, v in sorted(info.items()) if v is not None}
 
 
 def load(
     path: Union[str, Path],
-    collection_methods: List[str] = None,
+    collection_methods: List[str] | None = None,
     use_acq_for_names: bool = True,
     counts_per_second: bool = False,
-    drop_names: List[str] = None,
+    drop_names: List[str] | None = None,
     full: bool = False,
 ) -> Union[np.ndarray, Tuple[np.ndarray, dict]]:
     """Imports an Agilent '.b' batch.
 
     First attempts a binary import, falling back to importing any '.csv' files.
 
     Args:
```

### Comparing `pewlib-0.7.3/pewlib/io/csv.py` & `pewlib-0.8.0/pewlib/io/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
 Import of line-by-line data stored as a series of .csv files.
 """
 
-from concurrent.futures import ProcessPoolExecutor
 import logging
-from pathlib import Path
-import time
 import re
+import time
+from concurrent.futures import ProcessPoolExecutor
+from pathlib import Path
+from typing import Any, List, Tuple, Union
 
 import numpy as np
 import numpy.lib.recfunctions as rfn
 
-from typing import Any, List, Tuple, Union
-
-
 logger = logging.getLogger(__name__)
 
 
 class GenericOption(object):
     """Options for instrument specific csv imports.
 
     Options are used by :func:`pewlib.io.csv.load` to filter and sort paths,
@@ -28,15 +26,15 @@
         kw_genfromtxt: kwargs for numpy.genfromtxt
         regex: regex string for matching filenames
     """
 
     def __init__(
         self,
         drop_names: List[str] = [],
-        kw_genfromtxt: dict = None,
+        kw_genfromtxt: dict | None = None,
         regex: str = r".*\.csv",
         drop_nan_rows: bool = False,
         drop_nan_columns: bool = False,
         transposed: bool = False,
     ):
         self.drop_names = drop_names
         self.kw_genfromtxt = kw_genfromtxt
@@ -160,15 +158,15 @@
         (op for op in options if op.validForPath(path)),
         GenericOption(),
     )
 
 
 def load(
     path: Union[str, Path],
-    option: GenericOption = None,
+    option: GenericOption | None = None,
     full: bool = False,
 ) -> Union[np.ndarray, Tuple[np.ndarray, dict]]:
     """Load a directory where lines are stored in separate .csv files.
 
     Paths are filtered and sorted according to the `option` used, defaulting
     to the value of :func:`pewlib.io.csv.option_for_path`.
```

### Comparing `pewlib-0.7.3/pewlib/io/perkinelmer.py` & `pewlib-0.8.0/pewlib/io/perkinelmer.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.7.3/pewlib/io/textimage.py` & `pewlib-0.8.0/pewlib/io/textimage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Import and export of text-images, files where data is stored as delimited text values.
 Data is read in order from the first line.
 """
-import numpy as np
 from pathlib import Path
-
 from typing import Union
 
+import numpy as np
+
 
 def load(
-    path: Union[str, Path], delimiter: str = None, comments: str = "#", name: str = None
+    path: Union[str, Path],
+    delimiter: str | None = None,
+    comments: str = "#",
+    name: str = None,
 ) -> np.ndarray:
     """Load text-image.
 
     Loads 2d data from file. If `delimiter` is specified then all tab and ';'
     are converted to ',' before import. If `name` is specified then a single
     field structured array is returned.
 
@@ -50,8 +53,10 @@
     See :func:`numpy.savetxt`
 
     Args:
         path: path to file
         data: unstructured array
         header: file header
     """
+    if isinstance(path, str):  # pragma: no cover
+        path = Path(path)
     np.savetxt(path, data, delimiter=",", comments="#", header=header, fmt="%.18g")
```

### Comparing `pewlib-0.7.3/pewlib/io/thermo.py` & `pewlib-0.8.0/pewlib/io/thermo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """
 Import of line-by-line data exported from Qtegra using the '.csv' export function.
 Both column and row formats are supported.
 Tested with Thermo iCAP RQ ICP-MS.
 """
-import numpy as np
 import logging
 from pathlib import Path
-
 from typing import Generator, TextIO, Tuple, Union
 
+import numpy as np
+
 logger = logging.getLogger(__name__)
 
 
 def _icap_csv_columns_read(
-    path: Path, line_type: str, delimiter: str = None, comma_decimal: bool = False
+    path: Path,
+    line_type: str,
+    delimiter: str | None = None,
+    comma_decimal: bool = False,
 ) -> np.ndarray:
     def _read_lines(
         fp: TextIO, line_type: str, replace_decimal: bool = False
     ) -> Generator[str, None, None]:
         for line in fp:
             if line.startswith("MainRuns") and line_type in line:
                 yield line.replace(",", ".") if replace_decimal else line
@@ -58,15 +61,15 @@
             structured[name] = data[data["name"] == name]["data"].T
 
         return structured
 
 
 def icap_csv_columns_read_data(
     path: Union[str, Path],
-    delimiter: str = None,
+    delimiter: str | None = None,
     comma_decimal: bool = False,
     use_analog: bool = False,
 ) -> np.ndarray:
     if isinstance(path, str):  # pragma: no cover
         path = Path(path)
 
     return _icap_csv_columns_read(
@@ -75,15 +78,15 @@
         delimiter=delimiter,
         comma_decimal=comma_decimal,
     )
 
 
 def icap_csv_columns_read_params(
     path: Union[str, Path],
-    delimiter: str = None,
+    delimiter: str | None = None,
     comma_decimal: bool = False,
 ) -> dict:
     if isinstance(path, str):  # pragma: no cover
         path = Path(path)
 
     data = _icap_csv_columns_read(
         path, line_type="Time", delimiter=delimiter, comma_decimal=comma_decimal
@@ -93,15 +96,15 @@
 
     return dict(scantime=scantime)
 
 
 def _icap_csv_rows_read(
     path: Union[str, Path],
     col_type: str,
-    delimiter: str = None,
+    delimiter: str | None = None,
     comma_decimal: bool = False,
 ) -> np.ndarray:
     def _read_lines(
         fp: TextIO, replace_decimal: bool = False
     ) -> Generator[str, None, None]:
         for line in fp:
             yield line.replace(",", ".") if replace_decimal else line
@@ -141,36 +144,34 @@
             structured[name] = data[:, names == name]
 
         return structured
 
 
 def icap_csv_rows_read_data(
     path: Union[str, Path],
-    delimiter: str = None,
+    delimiter: str | None = None,
     comma_decimal: bool = False,
     use_analog: bool = False,
 ) -> np.ndarray:
-
     if isinstance(path, str):  # pragma: no cover
         path = Path(path)
 
     return _icap_csv_rows_read(
         path,
         "Analog" if use_analog else "Counter",
         delimiter=delimiter,
         comma_decimal=comma_decimal,
     )
 
 
 def icap_csv_rows_read_params(
     path: Union[str, Path],
-    delimiter: str = None,
+    delimiter: str | None = None,
     comma_decimal: bool = False,
 ) -> dict:
-
     if isinstance(path, str):  # pragma: no cover
         path = Path(path)
 
     data = _icap_csv_rows_read(
         path,
         "Time",
         delimiter=delimiter,
```

### Comparing `pewlib-0.7.3/pewlib/io/vtk.py` & `pewlib-0.8.0/pewlib/io/vtk.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.7.3/pewlib/laser.py` & `pewlib-0.8.0/pewlib/laser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Class for data collected line-by-line.
 Line-by-line data is collected in multiple lines, with each line performed as a
 continuous ablation in one direction. The lines are then stacked to form an image.
 """
+import copy
+from typing import Dict, List, Tuple, Union
+
 import numpy as np
 import numpy.lib.recfunctions as rfn
-import copy
 
 from pewlib.calibration import Calibration
 from pewlib.config import Config
 
-from typing import Dict, List, Tuple, Union
-
 
 class Laser(object):
     """Class for line-by-line laser data.
 
     Args:
         data: structured array of elemental data
         calibration: dict mapping elements to calibrations, optional
@@ -24,17 +24,17 @@
     Todo:
         Support rastered collection.
     """
 
     def __init__(
         self,
         data: np.ndarray,
-        calibration: Dict[str, Calibration] = None,
-        config: Config = None,
-        info: Dict[str, str] = None,
+        calibration: Dict[str, Calibration] | None = None,
+        config: Config | None = None,
+        info: Dict[str, str] | None = None,
     ):
         self.data: np.ndarray = data
         self.calibration = {name: Calibration() for name in self.elements}
         if calibration is not None:
             self.calibration.update(copy.deepcopy(calibration))
 
         if config is None:
@@ -59,15 +59,15 @@
         return self.data.shape
 
     @property
     def layers(self) -> int:
         return 1
 
     def add(
-        self, element: str, data: np.ndarray, calibration: Calibration = None
+        self, element: str, data: np.ndarray, calibration: Calibration | None = None
     ) -> None:
         """Adds a new element.
 
         Args:
             element: element name
             data: array
             calibration: calibration for data, optional
@@ -101,17 +101,17 @@
         """
         self.data = rfn.rename_fields(self.data, names)
         for old, new in names.items():
             self.calibration[new] = self.calibration.pop(old)
 
     def get(
         self,
-        element: str = None,
-        calibrate: bool = False,
-        extent: Tuple[float, float, float, float] = None,
+        element: str | None = None,
+        calibrate: bool | None = False,
+        extent: Tuple[float, float, float, float] | None = None,
         **kwargs,
     ) -> np.ndarray:
         """Get elemental data.
 
         If `element` is None then all elements are returned in a structured array.
 
         Args:
@@ -144,15 +144,15 @@
         return data
 
     @classmethod
     def from_list(
         cls,
         elements: List[str],
         datas: List[np.ndarray],
-        config: Config = None,
+        config: Config | None = None,
         info: Dict[str, str] = {},
     ) -> "Laser":
         """Creates class from a list of names and unstructured arrays."""
         assert len(elements) == len(datas)
         dtype = [(element, float) for element in elements]
 
         structured = np.empty(datas[0].shape, dtype=dtype)
```

### Comparing `pewlib-0.7.3/pewlib/process/calc.py` & `pewlib-0.8.0/pewlib/process/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """This module contains functions used by other processing modules."""
 
-import numpy as np
+from typing import List, Optional, Tuple
 
-from typing import List, Tuple
+import numpy as np
 
 
 def local_maxima(x: np.ndarray) -> np.ndarray:
     """Indicies of local maxima.
 
     Maxima are values greater than the 2 values surrounding them.
 
@@ -52,15 +52,15 @@
     oc = np.maximum.accumulate(c * n)
     return c - oc
 
 
 def shuffle_blocks(
     x: np.ndarray,
     block: Tuple[int, ...],
-    mask: np.ndarray = None,
+    mask: Optional[np.ndarray] | None = None,
     mode: str = "pad",
     shuffle_partial: bool = False,
 ) -> np.ndarray:
     """Shuffle an ndim array as tiles of a certain size.
 
     If a `mask` is passed then only the region within the mask is shuffled.
     If `shuffle_partial` then partially masked blocks will be shuffled otherwise
@@ -171,15 +171,15 @@
     See Also:
         :func:`pewlib.process.calc.subpixel_offset`
     """
     return subpixel_offset(x, [(o, o) for o in offsets], (pixelsize, pixelsize))
 
 
 def view_as_blocks(
-    x: np.ndarray, block: Tuple[int, ...], step: Tuple[int, ...] = None
+    x: np.ndarray, block: Tuple[int, ...], step: Optional[Tuple[int, ...]] | None = None
 ) -> np.ndarray:
     """Block view of array
 
     Can be overlapping if `step` < `block`.
 
     Args:
         x: array
```

### Comparing `pewlib-0.7.3/pewlib/process/colocal.py` & `pewlib-0.8.0/pewlib/process/colocal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Colcalisation can be used to quantify the spacial relationship between
 elements. A few ofthe many available algorithms are implemented in this file.
 
 """
 
+from typing import Tuple
+
 import numpy as np
 
 from pewlib.process.calc import normalise, shuffle_blocks
 
-from typing import Tuple
-
 
 def li_icq(x: np.ndarray, y: np.ndarray) -> float:
     """Calculates Li's ICQ.
 
     The intenisty correlation quotient calculates the number of pixels where both
     x and y are above or below their means. A value of 0 indicates no correlation,
     below 0 segregation and above 0 colocalisation.
@@ -49,15 +49,15 @@
     return (np.mean(x * y) - (np.mean(x) * np.mean(y))) / (np.std(x) * np.std(y))
 
 
 def pearsonr_probablity(
     x: np.ndarray,
     y: np.ndarray,
     block: int = 3,
-    mask: np.ndarray = None,
+    mask: np.ndarray | None = None,
     shuffle_partial: bool = False,
     n: int = 500,
 ) -> Tuple[float, float]:
     """Evalulates Probability of Pearson's coefficient.
 
     Calculates Pearson's R of `x` and `y` then shuffles `y` `n` times, retesting
     Pearson's R. The probability is defined as the ratio of R's produced by the
@@ -103,15 +103,15 @@
         )
         rs[i] = pearsonr(x[mask], shuffled[mask])
 
     return r, (rs < r).sum() / n
 
 
 def manders(
-    x: np.ndarray, y: np.ndarray, tx: float = None, ty: float = None
+    x: np.ndarray, y: np.ndarray, tx: float | None = None, ty: float | None = None
 ) -> Tuple[float, float]:
     """Manders' correlation coefficients.
 
     Args:
         x: array
         y: array, same shape as `x`
         tx: threshold for `x`, defaults to x.min()
```

### Comparing `pewlib-0.7.3/pewlib/process/convolve.py` & `pewlib-0.8.0/pewlib/process/convolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,36 +58,35 @@
         return rec
     elif mode == "same":
         return np.hstack((rec, x[rec.size :]))
     else:  # pragma: no cover
         raise ValueError("Valid modes are 'valid', 'same'.")
 
 
-def erf(x: float) -> float:
+def erf(x: float | np.ndarray) -> float | np.ndarray:
     """Error function approximation.
 
-    The maximum error is 5e-4 [1].
+    The maximum error is 1.5e-7 [1].
 
     Args:
         x: value
 
     Returns:
         approximation of error function
 
     References:
-
-    .. [1] Abramowitz, Milton, and Irene A. Stegun, eds. Handbook of mathematical
-        functions with formulas, graphs, and mathematical tables.
-        Vol. 55. US Government printing office, 1970.
+        .. [1] Abramowitz, Milton, and Irene A. Stegun, eds. Handbook of mathematical
+            functions with formulas, graphs, and mathematical tables.
+            Vol. 55. US Government printing office, 1970.
     """
-    assert x >= 0.0
-    # Maximum error: 2.5e-5
+    sign = np.sign(x)
     a = np.array([0.278393, 0.230389, 0.000972, 0.078108])
-
-    return 1.0 - 1.0 / (1.0 + np.sum(a * np.power(x, [1, 2, 3, 4]))) ** 4
+    p = np.array([[1, 2, 3, 4]]).T
+    sum = np.sum(a * np.power(x, p).T, axis=1)
+    return sign * (1.0 - 1.0 / (1.0 + sum) ** 4)
 
 
 def erfinv(x: float) -> float:
     """Inverse error function approximation.
 
     The maximum error is 6e-3 [2].
 
@@ -209,15 +208,15 @@
     """
     x = np.linspace(shift, size * scale + shift, size)
     y = exponential_pdf(x, _lambda)
     return np.stack((x, y / y.sum()), axis=1)
 
 
 def inversegamma_pdf(x: np.ndarray, alpha: float, beta: float) -> np.ndarray:
-    return ((beta ** alpha) / gamma(alpha)) * x ** (-alpha - 1.0) * np.exp(-beta / x)
+    return ((beta**alpha) / gamma(alpha)) * x ** (-alpha - 1.0) * np.exp(-beta / x)
 
 
 def inversegamma(
     size: int, alpha: float, beta: float, scale: float = 1.0, shift: float = 1e-6
 ) -> np.ndarray:
     """Inverse Gamma distribution.
```

### Comparing `pewlib-0.7.3/pewlib/process/filters.py` & `pewlib-0.8.0/pewlib/process/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 
 def rolling_mean(
     x: np.ndarray, block: Union[int, Tuple[int, ...]], threshold: float = 3.0
 ) -> np.ndarray:
     """Filter an array using rolling mean.
 
     Each value of `x` is compared to the mean of its `block`, the values arround it.
-    If it is `threshold` times the standard deviation *without the central value* then
-    it is considered an outlier. This prevents the value from impacting the stddev.
-    The mean of each block is recalculated outliers set to the new local mean.
+    If it is `threshold` times the standard deviation *with the central value* then
+    it is considered an outlier. Outliers are set to the local mean *without the central value*.
 
     Args:
         x: array
         block: size of window, int or same dims as `x`
         threshold: number of stddevs away from mean to consider outlier
 
     Returns:
@@ -32,75 +31,74 @@
 
     Removing spikes from 1d data.
 
     >>> import numpy as np
     >>> from pewlib.process import filters
     >>> a = np.sin(np.linspace(0, 1, 50))
     >>> a[5::10] +=np.random.choice([-1, 1], size=10)
-    >>> b = filters.rolling_mean(a, 3, threshold=3.0)
+    >>> b = filters.rolling_mean(a, 3, threshold=1.0)
 
     .. plot::
 
         import matplotlib.pyplot as plt
         import numpy as np
         from pewlib.process import filters
         a = np.sin(np.linspace(0, 10, 50))
         a[5::10] +=np.random.choice([-1, 1], size=5)
-        b = filters.rolling_mean(a, 3, threshold=3.0)
+        b = filters.rolling_mean(a, 3, threshold=1.0)
 
         plt.plot(a, c="black")
         plt.plot(b, ls=":", c="red", label="filtered")
         plt.legend()
         plt.show()
     """
     if isinstance(block, int):
-        block = tuple([block])
+        block = tuple([block] * x.ndim)
     assert len(block) == x.ndim
 
     # Prepare array by padding with nan
     pads = [(b // 2, b // 2) for b in block]
-    x_pad = np.pad(x, pads, constant_values=np.nan)
+    x_pad = np.pad(x, pads, mode="mean", stat_length=pads)  # type: ignore
 
-    blocks = view_as_blocks(x_pad, block, tuple([1 for b in block]))
+    blocks = view_as_blocks(x_pad, block, tuple([1] * x.ndim))
 
     # Calculate means and stds
     axes = tuple(np.arange(x.ndim, x.ndim * 2))
-    means = np.nanmean(blocks, axis=axes)
 
-    # Don't include the central point in the std calculation
-    nancenter = np.ones(block, dtype=np.float64)
-    nancenter[np.array(nancenter.shape) // 2] = np.nan
-    stds = np.nanstd(blocks * nancenter, axis=axes)
+    means = np.mean(blocks, axis=axes)
 
-    # Check for outlying values and set as nan
-    outliers = np.abs(x - means) > threshold * stds
+    mask = np.ones(block, dtype=bool)
+    mask[tuple(np.array(block) // 2)] = False
 
-    unpads = tuple([slice(p[0], -p[1]) for p in pads])
-    x_pad[unpads][outliers] = np.nan
+    # Mask out central (tested) value when calculating stddev
+    masked_stds = np.std(blocks, axis=axes, where=mask)
+    # Recalc means without central value
+    masked_means = np.mean(blocks, axis=axes, where=mask)
 
-    # As the mean is sensitive to outliers reclaculate it
-    means = np.nanmean(blocks, axis=axes)
+    # Check for outlying values and set as nan
+    outliers = np.abs(x - means) > threshold * masked_stds
 
-    return np.where(np.logical_and(outliers, ~np.isnan(means)), means, x)
+    return np.where(outliers, masked_means, x)
 
 
 def rolling_median(
-    x: np.ndarray, block: Union[int, Tuple[int, ...]], threshold: float = 3.0
+    x: np.ndarray,
+    block: Union[int, Tuple[int, ...]],
+    threshold: float = 3.0,
 ) -> np.ndarray:
     """Filter an array using rolling median.
 
     Each value of `x` is compared to the median of its `block`, the values arround it.
-    If it is `threshold` times the median distance from the median then
-    it is considered an outlier.
-    The mean of each block is recalculated outliers set to the local median.
+    If it is `threshold` times the stdev from the median then it is considered an outlier.
+    Outliers are set to the local median.
 
     Args:
         x: array
         block: size of window, int or same dims as `x`
-        threshold: number of median distances away from medians to consider outlier
+        threshold: number of SDs (via MAD) away from median to consider outlier
 
     Returns:
         array with outliers set to local means
 
     Example
     -------
 
@@ -126,31 +124,32 @@
         ax[0].set_title("raw image 'a'")
         ax[1].imshow(b, vmax=1.0)
         ax[1].set_title("filtered image 'b'")
         plt.show()
 
     """
     if isinstance(block, int):  # pragma: no cover
-        block = tuple([block])
+        block = tuple([block] * x.ndim)
     assert len(block) == x.ndim
 
     # Prepare array by padding with nan
     pads = [(b // 2, b // 2) for b in block]
-    x_pad = np.pad(x, pads, constant_values=np.nan)
+    y = np.pad(x, pads, mode="median", stat_length=pads)  # type: ignore
 
-    blocks = view_as_blocks(x_pad, block, tuple([1 for b in block]))
+    blocks = view_as_blocks(y, block, tuple([1] * x.ndim))
 
     # Calculate median and differences
     axes = tuple(np.arange(x.ndim, x.ndim * 2))
-    medians = np.nanmedian(blocks, axis=axes)
+    medians = np.median(blocks, axis=axes)
 
-    # Remove padding
-    unpads = tuple([slice(p[0], -p[1]) for p in pads])
-    x_pad[unpads] = np.abs(x - medians)
+    # Remove padding and set to differences
+    diff = np.abs(x - medians)
+    diff_pad = np.pad(diff, pads, mode="median", stat_length=pads)  # type: ignore
+    diff_blocks = view_as_blocks(diff_pad, block, tuple([1] * x.ndim))
 
     # Median of differences
-    median_medians = np.nanmedian(blocks, axis=axes)
+    mad = np.median(diff_blocks, axis=axes) * 1.4826  # estimate stddev
 
     # Outliers are n medians from data
-    outliers = x_pad[unpads] > threshold * median_medians
+    outliers = diff > threshold * mad
 
-    return np.where(np.logical_and(outliers, ~np.isnan(medians)), medians, x)
+    return np.where(outliers, medians, x)
```

### Comparing `pewlib-0.7.3/pewlib/process/peakfinding.py` & `pewlib-0.8.0/pewlib/process/peakfinding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+from typing import Callable
+
 import numpy as np
 
 from pewlib.process.calc import local_maxima, reset_cumsum, view_as_blocks
 
-from typing import Callable
-
-
 PEAK_DTYPE = np.dtype(
     {
         "names": ["height", "width", "area", "base", "top", "bottom", "left", "right"],
         "formats": [float, float, float, float, int, int, int, int],
     }
 )
 
@@ -31,20 +30,20 @@
         cwt[i] = np.convolve(x, wavelet(n, windows[i]), mode="same")
     return cwt
 
 
 def ricker_wavelet(size: int, sigma: float) -> np.ndarray:
     """The Ricker wavelet. For use with cwt."""
     x = np.linspace(-size / 2.0, size / 2.0, size)
-    a = 2.0 / (np.sqrt(3.0 * sigma) * np.pi ** 0.25)
-    return a * (1.0 - (x / sigma) ** 2) * np.exp(-(x ** 2 / (2.0 * sigma ** 2)))
+    a = 2.0 / (np.sqrt(3.0 * sigma) * np.pi**0.25)
+    return a * (1.0 - (x / sigma) ** 2) * np.exp(-(x**2 / (2.0 * sigma**2)))
 
 
 def _cwt_identify_ridges(
-    cwt_coef: np.ndarray, windows: np.ndarray, gap_threshold: int = None
+    cwt_coef: np.ndarray, windows: np.ndarray, gap_threshold: int | None = None
 ) -> np.ndarray:
     if gap_threshold is None:
         gap_threshold = len(windows) // 4
 
     maxima = local_maxima(cwt_coef[-1])
     ridges = np.full((cwt_coef.shape[0], maxima.size), -1, dtype=int)
     ridges[-1] = maxima
@@ -78,17 +77,17 @@
 
     return ridges
 
 
 def _cwt_filter_ridges(
     ridges: np.ndarray,
     cwt_coef: np.ndarray,
-    min_length: int = None,
+    min_length: int | None = None,
     noise_window: int = 100,
-    min_noise: float = None,
+    min_noise: float | None = None,
     min_snr: float = 10.0,
 ) -> np.ndarray:
     if min_noise is None:
         min_noise = np.amax(np.abs(cwt_coef[0])) / 100.0
     if min_length is None:
         min_length = ridges.shape[0] // 2
 
@@ -145,16 +144,16 @@
 #     return signal, filtered, means, stds
 
 
 def find_peaks_cwt(
     x: np.ndarray,
     min_midth: int,
     max_width: int,
-    ridge_gap_threshold: int = None,
-    ridget_min_length: int = None,
+    ridge_gap_threshold: int | None = None,
+    ridget_min_length: int | None = None,
     ridge_min_snr: float = 9.0,
     width_factor: float = 2.5,
     peak_base_method: str = "baseline",
     peak_height_method: str = "maxima",
     peak_min_area: float = 0.0,
     peak_min_height: float = 0.0,
     peak_min_width: float = 0.0,
@@ -327,15 +326,15 @@
 #     )
 
 #     return peaks
 
 
 def insert_missing_peaks(
     peaks: np.ndarray,
-    distance: float = None,
+    distance: float | None = None,
     param: str = "top",
     missing_peak_area: float = 0.0,
 ) -> np.ndarray:
     """Inserts missing peaks in a regularly spaced aquisition.
 
     If a gap in `param` greater than `distance` exists then peaks are inserted
     until no gap remains.
@@ -388,15 +387,15 @@
 
 def peaks_from_edges(
     x: np.ndarray,
     lefts: np.ndarray,
     rights: np.ndarray,
     base_method: str = "baseline",
     height_method: str = "maxima",
-    baseline: np.ndarray = None,
+    baseline: np.ndarray | None = None,
 ) -> np.ndarray:
     """Creates a peak array from left and right indicies.
 
     Args:
         x: array
         lefts: left indices of peaks
         right: right indices of peaks
```

### Comparing `pewlib-0.7.3/pewlib/process/register.py` & `pewlib-0.8.0/pewlib/process/register.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,45 @@
 """Module for registering and merging images."""
 
 import numpy as np
 
-from pewlib.laser import Laser
+from typing import Iterable, Tuple
 
-from typing import Iterable, Union, Tuple
 
+def anchor_offset(a: np.ndarray, b: np.ndarray, anchor: str) -> Tuple[int, int]:
+    """Return offset of `b` from `a` given a common achor point.
 
-def fft_register_images(a: np.ndarray, b: np.ndarray) -> Tuple[int, ...]:
+    Both `a` and `b` must be 2d arrays.
+    Valid anchors are 'top left', 'top right', 'bottom left', 'bottom right' or 'center'.
+
+    Args:
+        anchor: anchor poisition
+        a: nd array
+        b: nd array
+
+    Returns:
+        offset of 'b' from 'a' in pixels
+    """
+    assert a.ndim == 2 and b.ndim == 2
+
+    if anchor == "top left":
+        return (0, 0)
+    elif anchor == "top right":
+        return (0, a.shape[1] - b.shape[1])
+    elif anchor == "bottom left":
+        return (a.shape[0] - b.shape[0], 0)
+    elif anchor == "bottom right":
+        return (a.shape[0] - b.shape[0], a.shape[1] - b.shape[1])
+    elif anchor == "center":
+        return tuple((np.array(a.shape, dtype=int) + b.shape) // 2 - b.shape)
+    else:  # pragma: no cover
+        raise ValueError("Unknown anchor string.")
+
+
+def fft_register_offset(a: np.ndarray, b: np.ndarray) -> Tuple[int, ...]:
     """Register two images using FFT correlation.
 
     Arrays are zero-padded to `a.shape` + `b.shape` - 1
 
     Args:
         a: nd array
         b: nd array
@@ -94,31 +122,34 @@
     # offsets for each array
     aoffset = np.where(offset < 0, -offset, 0)
     boffset = np.where(offset >= 0, offset, 0)
     aslice = tuple(slice(o, o + s) for o, s in zip(aoffset, a.shape))
     bslice = tuple(slice(o, o + s) for o, s in zip(boffset, b.shape))
 
     # size and slice of overlapping area
-    abslice = tuple(slice(max(a.start, b.start), min(a.stop, b.stop), None) for a, b in zip(aslice, bslice))
+    abslice = tuple(
+        slice(max(a.start, b.start), min(a.stop, b.stop), None)
+        for a, b in zip(aslice, bslice)
+    )
     absize = tuple(s.stop - s.start for s in abslice)
     hasoverlap = all(x > 0 for x in absize)
 
     # sections of overlap from a, b
     asec = tuple(slice(o, o + s) for o, s in zip(aoffset, absize))
     bsec = tuple(slice(o, o + s) for o, s in zip(boffset, absize))
 
     c[aslice] = a
     c[bslice] = b
 
     if mode == "replace":
         pass
     elif mode == "mean" and hasoverlap:
-        c[abslice] = np.mean([a[asec], b[bsec]], axis=0)
+        c[abslice] = np.nanmean([a[asec], b[bsec]], axis=0)
     elif mode == "sum" and hasoverlap:
-        c[abslice] = np.sum([a[asec], b[bsec]], axis=0)
+        c[abslice] = np.nansum([a[asec], b[bsec]], axis=0)
 
     return c
 
 
 def overlap_structured_arrays(
     a: np.ndarray,
     b: np.ndarray,
@@ -146,72 +177,34 @@
     """
     offset = np.array(offset, dtype=int)
     if offset.size != a.ndim:  # pragma: no cover
         raise ValueError("Anchor must have same dimensions as arrays.")
 
     # find the max / min extents of the new array
     new_shape = np.maximum(a.shape, offset + b.shape) - np.minimum(0, offset)
-    new_dtype = list(set(a.dtype.descr + b.dtype.descr))
+    new_dtype = list(a.dtype.descr)
+    new_dtype.extend([x for x in b.dtype.descr if x not in new_dtype])
     c = np.empty(new_shape, dtype=new_dtype)
 
     for name in c.dtype.names:
         if name not in b.dtype.names:
             c[name] = overlap_arrays(
-                np.full(b.shape, fill), a[name], offset=-offset, fill=fill, mode=mode
+                np.full(b.shape, fill),
+                a[name],
+                offset=-offset,
+                fill=fill,
+                mode="replace",
             )
         elif name not in a.dtype.names:
             c[name] = overlap_arrays(
-                np.full(a.shape, fill), b[name], offset=offset, fill=fill, mode=mode
+                np.full(a.shape, fill),
+                b[name],
+                offset=offset,
+                fill=fill,
+                mode="replace",
             )
         else:
             c[name] = overlap_arrays(
                 a[name], b[name], offset=offset, fill=fill, mode=mode
             )
 
     return c
-
-
-def overlap_lasers(
-    a: Laser, b: Laser, anchor: Union[str, Tuple[int, int]] = "top left"
-) -> Laser:
-    """Merges two arrays by enlarging.
-
-    Coordinates (0, 0) of array 'b' will be at 'anchor' in the new array.
-    Shared names and calibrations in 'a' are overwritten by 'b' where overlap occurs.
-    Valid anchors are 'top left', 'top right', 'bottom left', 'bottom right', 'center' or
-    a tuple of ints sepcififying the coordinates of overlap.
-
-    Args:
-        a: Laser
-        b: Laser
-        anchor: offset
-
-    Returns:
-        new overlapped array
-    """
-    if isinstance(anchor, str):
-        if anchor == "top left":
-            anchor = (0, 0)
-        elif anchor == "top right":
-            anchor = (0, a.shape[1] - b.shape[1])
-        elif anchor == "bottom left":
-            anchor = (a.shape[0] - b.shape[0], 0)
-        elif anchor == "bottom right":
-            anchor = (a.shape[0] - b.shape[0], a.shape[1] - b.shape[1])
-        elif anchor == "center":
-            anchor = (np.array(a.shape, dtype=int) + b.shape) // 2 - b.shape
-        else:
-            raise ValueError("Unknown anchor string.")
-
-    data = overlap_structured_arrays(a.data, b.data, anchor=anchor)
-
-    calibration = {}
-    for name in data.dtype.names:
-        if name in b.elements:
-            calibration[name] = b.calibration[name]
-        elif name in a.elements:
-            calibration[name] = a.calibration[name]
-
-    info = {"Overlap": f"{a.info['Name']}:{b.info['Name']}@{anchor[0],anchor[1]}"}
-    info.update(a.info)
-
-    return Laser(data=data, calibration=calibration, config=a.config, info=info)
```

### Comparing `pewlib-0.7.3/pewlib/process/threshold.py` & `pewlib-0.8.0/pewlib/process/threshold.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.7.3/pewlib/srr/config.py` & `pewlib-0.8.0/pewlib/srr/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from typing import Iterable, List, Tuple
+
 import numpy as np
 
 from pewlib.config import Config
 
-from typing import Iterable, Tuple, List
-
 
 class SRRConfig(Config):
     """Class for the super-resolution-reconstruction image parameters.
 
     Args:
         spotsize: laser-spot diameter, μm
         speed: laser movement speed, μm/s
@@ -75,28 +75,28 @@
         mag = np.round(mag).astype(int)
         return np.lcm(self._subpixel_size, mag) // mag
 
     def set_equal_subpixel_offsets(self, width: int) -> None:
         self._subpixel_offsets = np.arange(0, width, dtype=int)
         self._subpixel_size = width
 
-    def get_pixel_width(self, layer: int = None) -> float:
+    def get_pixel_width(self, layer: int | None = None) -> float:
         """Pixel width in μm.
 
         Args:
             layer: limit to layer
         """
         if layer is None:
             return super().get_pixel_width() / self.subpixels_per_pixel
         elif layer % 2 == 0:
             return super().get_pixel_width()
         else:
             return super().get_pixel_height()
 
-    def get_pixel_height(self, layer: int = None) -> float:
+    def get_pixel_height(self, layer: int | None = None) -> float:
         """Pixel height in μm.
 
         Args:
             layer: limit to layer
         """
         if layer is None:
             return super().get_pixel_width() / self.subpixels_per_pixel
@@ -105,15 +105,15 @@
         else:
             return super().get_pixel_width()
 
     # Return without the washout included
     def data_extent(
         self,
         shape: Tuple[int, ...],
-        layer: int = None,
+        layer: int | None = None,
     ) -> Tuple[float, float, float, float]:
         """Extent of data in μm.
 
         Args:
             shape: data shape
             layer: limit calculation to layer
         """
```

### Comparing `pewlib-0.7.3/pewlib/srr/srr.py` & `pewlib-0.8.0/pewlib/srr/srr.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 The resulting image is 3d, but can be flattened to a higher resolution 2d image.
 
 References:
     Westerhausen, M. T.; Bishop, D. P.; Dowd, A.; Wanagat, J.; Cole, N.
     & Doble, P. A. Super-Resolution Reconstruction for Two- and Three-Dimensional
     LA-ICP-MS Bioimaging Analytical Chemistry, American Chemical Society (ACS), 2019
 """
+import copy
+from typing import Dict, List, Tuple, Union
+
 import numpy as np
 import numpy.lib.recfunctions as rfn
-import copy
 
-from pewlib.laser import Laser
 from pewlib.calibration import Calibration
-
+from pewlib.laser import Laser
 from pewlib.process.calc import subpixel_offset_equal
-
 from pewlib.srr.config import SRRConfig
 
-from typing import Dict, List, Tuple, Union
-
 
 class SRRLaser(Laser):
     """Class for SRR laser data.
 
     Args:
         data: list of structured arrays
         calibration: dict mapping elements to calibrations, optional
@@ -35,17 +33,17 @@
     See Also:
         :class:`pewlib.laser.Laser`
     """
 
     def __init__(
         self,
         data: List[np.ndarray],
-        calibration: Dict[str, Calibration] = None,
-        config: SRRConfig = None,
-        info: Dict[str, str] = None,
+        calibration: Dict[str, Calibration] | None = None,
+        config: SRRConfig | None = None,
+        info: Dict[str, str] | None = None,
     ):
         assert len(data) > 1
         self.data: List[np.ndarray] = data
         self.calibration = {name: Calibration() for name in self.elements}
         if calibration is not None:
             self.calibration.update(copy.deepcopy(calibration))
 
@@ -77,15 +75,18 @@
         return len(self.data)
 
     @property
     def shape(self) -> Tuple[int, ...]:
         return (self.data[1].shape[0], self.data[0].shape[0], len(self.data))
 
     def add(
-        self, element: str, data: List[np.ndarray], calibration: Calibration = None
+        self,
+        element: str,
+        data: List[np.ndarray],
+        calibration: Calibration | None = None,
     ) -> None:
         """Add an element."""
         assert len(data) == len(self.data)
         for i in range(0, len(self.data)):
             assert data[i].shape == self.data[i].shape
             dtype = self.data[i].dtype
             new_dtype = dtype.descr + [(element, data[i].dtype.str)]
@@ -118,19 +119,19 @@
         for i in range(len(self.data)):
             self.data[i] = rfn.rename_fields(self.data[i], names)
         for old, new in names.items():
             self.calibration[(new)] = self.calibration.pop(old)
 
     def get(
         self,
-        element: str = None,
+        element: str | None = None,
         calibrate: bool = False,
-        extent: Tuple[float, float, float, float] = None,
+        extent: Tuple[float, float, float, float] | None = None,
         flat: bool = False,
-        layer: int = None,
+        layer: int | None = None,
         **kwargs,
     ) -> np.ndarray:
         """Get elemental data.
 
         If `element` is None then all elements are returned in a structured array.
         If a 2d array is required then `flat` will flatten the array by calculating
         the mean across the 2nd axis. If a `layer` is given then the layer is extracted
@@ -222,16 +223,16 @@
         )
 
     @classmethod
     def from_list(
         cls,
         elements: List[str],
         layers: List[List[np.ndarray]],
-        config: SRRConfig = None,
-        info: Dict[str, str] = None,
+        config: SRRConfig | None = None,
+        info: Dict[str, str] | None = None,
     ) -> "SRRLaser":
         """Creates class from a list of names and lists of unstructured arrays."""
         dtype = [(element, float) for element in elements]
 
         structured_layers = []
         for datas in layers:
             assert len(elements) == len(datas)
```

### Comparing `pewlib-0.7.3/pewlib.egg-info/PKG-INFO` & `pewlib-0.8.0/pewlib.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pewlib
-Version: 0.7.3
+Version: 0.8.0
 Summary: Import, processing and export library for LA-ICP-MS data.
 Home-page: https://github.com/djdt/pewlib
 Author: T. Lockwood
 Author-email: thomas.lockwood@uts.edu.au
-License: UNKNOWN
 Project-URL: Documentation, https://djdt.github.io/pewlib
 Project-URL: Source, https://gtihub.com/djdt/pewlib
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pewlib
 
 ![Build](https://github.com/djdt/pewlib/workflows/Build/badge.svg)
 
@@ -24,9 +22,7 @@
 Pewlib is availble on PyPI and installable via pip.
 
 ```pip install pewlib```
 
 ## Documentation
 
 Documenation is available at <https://djdt.github.io/pewlib>.
-
-
```

### Comparing `pewlib-0.7.3/setup.py` & `pewlib-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,10 +19,11 @@
     author_email="thomas.lockwood@uts.edu.au",
     url="https://github.com/djdt/pewlib",
     project_urls={
         "Documentation": "https://djdt.github.io/pewlib",
         "Source": "https://gtihub.com/djdt/pewlib",
     },
     packages=find_packages(include=["pewlib", "pewlib.*"]),
+    entry_points={"console_scripts": ["pewlib=pewlib.__main__:main"]},
     install_requires=["numpy"],
     tests_require=["pytest"],
 )
```

