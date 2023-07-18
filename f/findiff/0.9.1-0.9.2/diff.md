# Comparing `tmp/findiff-0.9.1.tar.gz` & `tmp/findiff-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/findiff-0.9.1.tar", last modified: Wed Aug 10 18:46:46 2022, max compression
+gzip compressed data, was "dist/findiff-0.9.2.tar", last modified: Thu Aug 11 06:01:34 2022, max compression
```

## Comparing `findiff-0.9.1.tar` & `findiff-0.9.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-08-10 18:46:46.075480 findiff-0.9.1/
--rw-r--r--   0 mbaer    (671849960) 579947404     1063 2020-07-10 12:52:17.000000 findiff-0.9.1/LICENSE
--rw-r--r--   0 mbaer    (671849960) 579947404     1926 2022-08-10 18:46:46.075601 findiff-0.9.1/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404     9610 2022-08-10 16:36:45.000000 findiff-0.9.1/README.md
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-08-10 18:46:46.069681 findiff-0.9.1/findiff/
--rw-r--r--   0 mbaer    (671849960) 579947404     1148 2022-08-10 18:46:18.000000 findiff-0.9.1/findiff/__init__.py
--rw-r--r--   0 mbaer    (671849960) 579947404     6534 2021-02-01 15:31:23.000000 findiff-0.9.1/findiff/coefs.py
--rw-r--r--   0 mbaer    (671849960) 579947404    17139 2022-07-29 05:45:37.000000 findiff-0.9.1/findiff/diff.py
--rw-r--r--   0 mbaer    (671849960) 579947404      664 2021-01-16 17:41:31.000000 findiff-0.9.1/findiff/grids.py
--rw-r--r--   0 mbaer    (671849960) 579947404     5530 2022-07-28 14:03:47.000000 findiff-0.9.1/findiff/operators.py
--rw-r--r--   0 mbaer    (671849960) 579947404     3538 2021-02-01 06:44:55.000000 findiff-0.9.1/findiff/pde.py
--rw-r--r--   0 mbaer    (671849960) 579947404    10415 2022-08-10 18:18:33.000000 findiff-0.9.1/findiff/stencils.py
--rw-r--r--   0 mbaer    (671849960) 579947404      918 2022-07-29 05:46:17.000000 findiff-0.9.1/findiff/utils.py
--rw-r--r--   0 mbaer    (671849960) 579947404     8379 2021-01-16 17:41:31.000000 findiff-0.9.1/findiff/vector.py
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-08-10 18:46:46.071417 findiff-0.9.1/findiff.egg-info/
--rw-r--r--   0 mbaer    (671849960) 579947404     1926 2022-08-10 18:46:46.000000 findiff-0.9.1/findiff.egg-info/PKG-INFO
--rw-r--r--   0 mbaer    (671849960) 579947404      562 2022-08-10 18:46:46.000000 findiff-0.9.1/findiff.egg-info/SOURCES.txt
--rw-r--r--   0 mbaer    (671849960) 579947404        1 2022-08-10 18:46:46.000000 findiff-0.9.1/findiff.egg-info/dependency_links.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       18 2022-08-10 18:46:46.000000 findiff-0.9.1/findiff.egg-info/requires.txt
--rw-r--r--   0 mbaer    (671849960) 579947404       13 2022-08-10 18:46:46.000000 findiff-0.9.1/findiff.egg-info/top_level.txt
--rw-r--r--   0 mbaer    (671849960) 579947404      104 2022-08-10 18:46:46.076086 findiff-0.9.1/setup.cfg
--rw-r--r--   0 mbaer    (671849960) 579947404     2718 2022-07-29 12:01:08.000000 findiff-0.9.1/setup.py
-drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-08-10 18:46:46.075240 findiff-0.9.1/test/
--rw-r--r--   0 mbaer    (671849960) 579947404        1 2022-07-28 16:07:31.000000 findiff-0.9.1/test/__init__.py
--rw-r--r--   0 mbaer    (671849960) 579947404     4161 2021-01-16 18:09:56.000000 findiff-0.9.1/test/test_bugs.py
--rw-r--r--   0 mbaer    (671849960) 579947404     6198 2021-02-01 15:33:51.000000 findiff-0.9.1/test/test_coefs.py
--rw-r--r--   0 mbaer    (671849960) 579947404     4645 2021-01-17 17:21:38.000000 findiff-0.9.1/test/test_diff.py
--rw-r--r--   0 mbaer    (671849960) 579947404    14335 2021-01-17 17:24:34.000000 findiff-0.9.1/test/test_findiff.py
--rw-r--r--   0 mbaer    (671849960) 579947404      539 2021-01-16 17:41:31.000000 findiff-0.9.1/test/test_grids.py
--rw-r--r--   0 mbaer    (671849960) 579947404     8301 2020-07-10 12:52:17.000000 findiff-0.9.1/test/test_pde.py
--rw-r--r--   0 mbaer    (671849960) 579947404     2004 2020-07-10 13:04:57.000000 findiff-0.9.1/test/test_scaling.py
--rw-r--r--   0 mbaer    (671849960) 579947404     5530 2022-07-29 11:57:45.000000 findiff-0.9.1/test/test_stencils.py
--rw-r--r--   0 mbaer    (671849960) 579947404     1394 2022-07-29 05:46:05.000000 findiff-0.9.1/test/test_utils.py
--rw-r--r--   0 mbaer    (671849960) 579947404     4342 2021-01-16 17:41:31.000000 findiff-0.9.1/test/test_vector.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-08-11 06:01:34.368267 findiff-0.9.2/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1063 2020-07-10 12:52:17.000000 findiff-0.9.2/LICENSE
+-rw-r--r--   0 mbaer    (671849960) 579947404     1926 2022-08-11 06:01:34.368439 findiff-0.9.2/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404     9604 2022-08-11 05:38:35.000000 findiff-0.9.2/README.md
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-08-11 06:01:34.361312 findiff-0.9.2/findiff/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1148 2022-08-11 06:01:08.000000 findiff-0.9.2/findiff/__init__.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     6534 2021-02-01 15:31:23.000000 findiff-0.9.2/findiff/coefs.py
+-rw-r--r--   0 mbaer    (671849960) 579947404    17120 2022-08-11 06:00:49.000000 findiff-0.9.2/findiff/diff.py
+-rw-r--r--   0 mbaer    (671849960) 579947404      664 2021-01-16 17:41:31.000000 findiff-0.9.2/findiff/grids.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     5435 2022-08-11 06:00:49.000000 findiff-0.9.2/findiff/operators.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     3538 2021-02-01 06:44:55.000000 findiff-0.9.2/findiff/pde.py
+-rw-r--r--   0 mbaer    (671849960) 579947404    10314 2022-08-11 06:00:49.000000 findiff-0.9.2/findiff/stencils.py
+-rw-r--r--   0 mbaer    (671849960) 579947404      918 2022-07-29 05:46:17.000000 findiff-0.9.2/findiff/utils.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     8379 2021-01-16 17:41:31.000000 findiff-0.9.2/findiff/vector.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-08-11 06:01:34.362716 findiff-0.9.2/findiff.egg-info/
+-rw-r--r--   0 mbaer    (671849960) 579947404     1926 2022-08-11 06:01:34.000000 findiff-0.9.2/findiff.egg-info/PKG-INFO
+-rw-r--r--   0 mbaer    (671849960) 579947404      562 2022-08-11 06:01:34.000000 findiff-0.9.2/findiff.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404        1 2022-08-11 06:01:34.000000 findiff-0.9.2/findiff.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       18 2022-08-11 06:01:34.000000 findiff-0.9.2/findiff.egg-info/requires.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404       13 2022-08-11 06:01:34.000000 findiff-0.9.2/findiff.egg-info/top_level.txt
+-rw-r--r--   0 mbaer    (671849960) 579947404      104 2022-08-11 06:01:34.369047 findiff-0.9.2/setup.cfg
+-rw-r--r--   0 mbaer    (671849960) 579947404     2718 2022-07-29 12:01:08.000000 findiff-0.9.2/setup.py
+drwxr-xr-x   0 mbaer    (671849960) 579947404        0 2022-08-11 06:01:34.367872 findiff-0.9.2/test/
+-rw-r--r--   0 mbaer    (671849960) 579947404        1 2022-07-28 16:07:31.000000 findiff-0.9.2/test/__init__.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     4161 2022-08-11 06:00:49.000000 findiff-0.9.2/test/test_bugs.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     6198 2021-02-01 15:33:51.000000 findiff-0.9.2/test/test_coefs.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     4645 2021-01-17 17:21:38.000000 findiff-0.9.2/test/test_diff.py
+-rw-r--r--   0 mbaer    (671849960) 579947404    14335 2021-01-17 17:24:34.000000 findiff-0.9.2/test/test_findiff.py
+-rw-r--r--   0 mbaer    (671849960) 579947404      539 2021-01-16 17:41:31.000000 findiff-0.9.2/test/test_grids.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     8301 2020-07-10 12:52:17.000000 findiff-0.9.2/test/test_pde.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     2004 2020-07-10 13:04:57.000000 findiff-0.9.2/test/test_scaling.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     6399 2022-08-11 06:00:49.000000 findiff-0.9.2/test/test_stencils.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     1394 2022-07-29 05:46:05.000000 findiff-0.9.2/test/test_utils.py
+-rw-r--r--   0 mbaer    (671849960) 579947404     4342 2021-01-16 17:41:31.000000 findiff-0.9.2/test/test_vector.py
```

### Comparing `findiff-0.9.1/LICENSE` & `findiff-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/PKG-INFO` & `findiff-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findiff
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python package for finite difference derivatives in any number of dimensions.
 Home-page: https://github.com/maroba/findiff
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Keywords: finite-differences,numerical-derivatives,scientific-computing
 Platform: ALL
```

### Comparing `findiff-0.9.1/README.md` & `findiff-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 ```
 import numpy as np
 
 x = np.linspace(0, 1, 100)
 f = np.sin(x)  # as an example
 
 # Define the derivative:
-d2_dx2 = FinDiff(0, dx, 1)
+d_dx = FinDiff(0, dx, 1)
 
 # Apply it:
-d2f_dx2 = d2_dx2(f) 
+df_dx = d_dx(f) 
 ```
 
 Similary, you can define partial derivative operators along different axes or of higher degree, for example:
 
 | Math                                                  | *findiff*                             |                                        |
 |-------------------------------------------------------|---------------------------------------|----------------------------------------|
 | <img src="docs/frontpage/d_dy.png" height="50px">     | ```FinDiff(1, dy, 1)```               | same as ``` FinDiff(1, dy)```          |
```

### Comparing `findiff-0.9.1/findiff/__init__.py` & `findiff-0.9.2/findiff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 - Fully vectorized for speed
 - Calculate raw finite difference coefficients for any order and accuracy for uniform and non-uniform grids
 - New in version 0.7: Generate matrix representations of arbitrary linear differential operators
 - New in version 0.8: Solve partial differential equations with Dirichlet or Neumann boundary conditions
 - New in version 0.9: Generate differential operators for generic stencils
 """
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 
 from .coefs import coefficients
 from .operators import FinDiff, Coef, Identity, Coefficient
 from .vector import Gradient, Divergence, Curl, Laplacian
 from .pde import PDE, BoundaryConditions
```

### Comparing `findiff-0.9.1/findiff/coefs.py` & `findiff-0.9.2/findiff/coefs.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/findiff/diff.py` & `findiff-0.9.2/findiff/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
     def apply(self, rhs, *args, **kwargs):
         raise NotImplementedError
 
     def __call__(self, rhs, *args, **kwargs):
         return self.apply(rhs, *args, **kwargs)
 
-    def stencil(self, shape, acc=None):
-        return StencilSet(self, shape, acc=acc)
+    def stencil(self, shape):
+        return StencilSet(self, shape)
 
 
 class Plus(BinaryOperator):
     """ A class to add two differential operators """
 
     def __init__(self, left, right):
         super().__init__(left, right)
```

### Comparing `findiff-0.9.1/findiff/grids.py` & `findiff-0.9.2/findiff/grids.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/findiff/operators.py` & `findiff-0.9.2/findiff/operators.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,18 +89,16 @@
         if len(args) == 0 and 'h' not in kwargs:
             if self.uniform:
                 args = self.spac,
             else:
                 args = self.coords,
         return self.pds(rhs, *args, **kwargs)
 
-    def stencil(self, shape, acc=None):
-        if acc is None and self.acc is not None:
-            acc = self.acc
-        return StencilSet(self, shape, acc=acc)
+    def stencil(self, shape):
+        return StencilSet(self, shape)
 
     def matrix(self, shape, h=None, acc=None):
         if acc is None:
             if self.acc is None:
                 acc = DEFAULT_ACC
             else:
                 acc = self.acc
```

### Comparing `findiff-0.9.1/findiff/pde.py` & `findiff-0.9.2/findiff/pde.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/findiff/stencils.py` & `findiff-0.9.2/findiff/stencils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class StencilSet(object):
     """
     Represent the finite difference stencil for a given differential operator.
     """
 
-    def __init__(self, diff_op, shape, old_stl=None, acc=None):
+    def __init__(self, diff_op, shape, old_stl=None):
         """
         Constructor for Stencil objects.
 
         :param shape: tuple of ints
             Shape of the grid on which the stencil should be applied.
 
         :param axis: int >= 0
@@ -23,25 +23,19 @@
 
         :param order: int > 0
             The order of the derivative.
 
         :param h: float
             The spacing of the (equidistant) grid
 
-        :param acc: (even) int > 0
-            The desired accuracy order of the finite difference scheme.
-
         """
 
         self.shape = shape
         self.diff_op = diff_op
         self.char_pts = self._det_characteristic_points()
-        self.acc = None
-        if acc is not None:
-            self.acc = acc
 
         self.data = {}
 
         self._create_stencil()
 
     def __str__(self):
         return str(self.data)
@@ -59,15 +53,15 @@
             The index of the grid point where to differentiate the function.
 
         :return:
             The derivative at the given point.
         """
 
         if not hasattr(idx0, '__len__'):
-            idx0 = (idx0, )
+            idx0 = (idx0,)
 
         typ = []
         for axis in range(len(self.shape)):
             if idx0[axis] == 0:
                 typ.append('L')
             elif idx0[axis] == self.shape[axis] - 1:
                 typ.append('H')
@@ -113,15 +107,15 @@
         for idx in indices:
             du[idx] = self.apply(u, idx)
 
         return du
 
     def _create_stencil(self):
 
-        matrix = self.diff_op.matrix(self.shape, acc=self.acc)
+        matrix = self.diff_op.matrix(self.shape)
 
         for pt in self.char_pts:
 
             char_point_stencil = {}
             self.data[pt] = char_point_stencil
 
             index_tuple_for_char_pt = self._typical_index_tuple_for_char_point(pt)
@@ -145,15 +139,15 @@
             else:
                 index_tuple_for_char_pt.append(self.shape[axis] - 1)
         return tuple(index_tuple_for_char_pt)
 
     def _det_characteristic_points(self):
         shape = self.shape
         ndim = len(shape)
-        typ = [("L", "C", "H")]*ndim
+        typ = [("L", "C", "H")] * ndim
         return product(*typ)
 
 
 class Stencil:
 
     def __init__(self, offsets, partials, spacings=None):
 
@@ -181,14 +175,20 @@
         if at is None and on is not None:
             if isinstance(on[0], slice):
                 return self._apply_on_multi_slice(f, on)
             else:
                 return self._apply_on_mask(f, on)
         raise Exception('Cannot specify both *at* and *on* parameters.')
 
+    def __str__(self):
+        return str(self.values)
+
+    def __repr__(self):
+        return str(self.values)
+
     def _apply_on_mask(self, f, mask):
         result = np.zeros_like(f)
         for offset, coeff in self.values.items():
             offset_mask = self._make_offset_mask(mask, offset)
             result[mask] += coeff * f[offset_mask]
         return result
 
@@ -230,17 +230,14 @@
                 sl_off = slice(None, off_)
                 sl_base = slice(-off_, None)
             mslice_off.append(sl_off)
             mslice_base.append(sl_base)
         offset_mask[tuple(mslice_base)] = mask[tuple(mslice_off)]
         return offset_mask
 
-
-
-
     def _canonic_slice(self, sl, length):
         start = sl.start
         if start is None:
             start = 0
         if start < 0:
             start = length - start
         stop = sl.stop
@@ -317,8 +314,7 @@
         all_combs = list(product(range(the_sum + 1), repeat=self.ndims))
         return list(filter(lambda tpl: sum(tpl) == the_sum, all_combs))
 
     def _rows_are_linearly_independent(self, matrix):
         """Checks the linear independence of the rows of a matrix."""
         matrix = np.array(matrix).astype(float)
         return np.linalg.matrix_rank(matrix) == len(matrix)
-
```

### Comparing `findiff-0.9.1/findiff/utils.py` & `findiff-0.9.2/findiff/utils.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/findiff/vector.py` & `findiff-0.9.2/findiff/vector.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/findiff.egg-info/PKG-INFO` & `findiff-0.9.2/findiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findiff
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python package for finite difference derivatives in any number of dimensions.
 Home-page: https://github.com/maroba/findiff
 Author: Matthias Baer
 Author-email: matthias.r.baer@googlemail.com
 License: MIT
 Keywords: finite-differences,numerical-derivatives,scientific-computing
 Platform: ALL
```

### Comparing `findiff-0.9.1/findiff.egg-info/SOURCES.txt` & `findiff-0.9.2/findiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/setup.py` & `findiff-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/test/test_bugs.py` & `findiff-0.9.2/test/test_bugs.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
                          (-1, 0): -3.999999999999996, (0, 0): 2.0833333333333317},
         }
 
         for char_pt in stencil1.data:
             stl = stencil1.data[char_pt]
             self.assert_dict_almost_equal(expected[char_pt], stl)
 
-        d1x = FinDiff(0, dx, 1)
-        stencil1 = d1x.stencil(shape, acc=4)
+        d1x = FinDiff(0, dx, 1, acc=4)
+        stencil1 = d1x.stencil(shape)
         for char_pt in stencil1.data:
             stl = stencil1.data[char_pt]
             self.assert_dict_almost_equal(expected[char_pt], stl)
 
     def test_order_as_numpy_integer(self):
 
         order = np.ones(3, dtype=np.int32)[0]
```

### Comparing `findiff-0.9.1/test/test_coefs.py` & `findiff-0.9.2/test/test_coefs.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/test/test_diff.py` & `findiff-0.9.2/test/test_diff.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/test/test_findiff.py` & `findiff-0.9.2/test/test_findiff.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/test/test_grids.py` & `findiff-0.9.2/test/test_grids.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/test/test_pde.py` & `findiff-0.9.2/test/test_pde.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/test/test_scaling.py` & `findiff-0.9.2/test/test_scaling.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/test/test_stencils.py` & `findiff-0.9.2/test/test_stencils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 
 import numpy as np
 
+from findiff import Identity, FinDiff
 from findiff.stencils import Stencil
 
 
 class TestStencilOperations(unittest.TestCase):
 
     def test_solve_laplace_2d_with_5_points(self):
         offsets = [(-1, 0), (0, 0), (1, 0), (0, 1), (0, -1)]
@@ -132,15 +133,14 @@
         f = x**3
         expected = 6*x
         offsets = list(range(-4, 5))
         stencil = Stencil(offsets, partials={(2,): 1}, spacings=(x[1]-x[0],))
         at = 8,
         actual = stencil(f, at)
         self.assertAlmostEqual(expected[at], actual, places=5)
-        print(stencil.values, stencil.accuracy)
 
     def tests_apply_stencil_on_multislice(self):
         x = y = np.linspace(0, 1, 21)
         dx = dy = x[1] - x[0]
         X, Y = np.meshgrid(x, y, indexing='ij')
 
         f = X ** 3 + Y ** 3
@@ -164,7 +164,28 @@
         offsets = [(-1, 0), (0, 0), (1, 0), (0, 1), (0, -1)]
         stencil = Stencil(offsets, {(2, 0): 1, (0, 2): 1}, spacings=(dx, dy))
 
         mask = np.full_like(f, fill_value=False, dtype=bool)
         mask[1:-1, 1:-1] = True
         actual = stencil(f, on=mask)
         np.testing.assert_array_almost_equal(expected[mask], actual[mask])
+
+    def test_helmholtz_stencil_issue_60(self):
+        # This is a regression test for issue #60.
+
+        H = Identity() - FinDiff(0, 1, 2)
+
+        stencil_set = H.stencil((10,))
+
+        expected = {('L',): {(0,): -1.0, (1,): 5.0, (2,): -4.0, (3,): 1.0}, ('C',): {(-1,): -1.0, (0,): 3.0, (1,): -1.0},
+         ('H',): {(-3,): 1.0, (-2,): -4.0, (-1,): 5.0, (0,): -1.0}}
+
+        actual = stencil_set.data
+        self.assertEqual(len(expected), len(actual))
+        self.assertEqual(expected.keys(), actual.keys())
+        for key, expected_stencil in expected.items():
+            actual_stencil = actual[key]
+
+            self.assertEqual(expected_stencil.keys(), actual_stencil.keys())
+            for offset, expected_coef in expected_stencil.items():
+                actual_coef = actual_stencil[offset]
+                self.assertAlmostEqual(expected_coef, actual_coef)
```

### Comparing `findiff-0.9.1/test/test_utils.py` & `findiff-0.9.2/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `findiff-0.9.1/test/test_vector.py` & `findiff-0.9.2/test/test_vector.py`

 * *Files identical despite different names*

