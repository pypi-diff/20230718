# Comparing `tmp/cofi-0.2.1.tar.gz` & `tmp/cofi-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cofi-0.2.1.tar", last modified: Fri Jul  7 03:56:03 2023, max compression
+gzip compressed data, was "cofi-0.2.2.tar", last modified: Mon Jul 17 23:17:39 2023, max compression
```

## Comparing `cofi-0.2.1.tar` & `cofi-0.2.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.918507 cofi-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-07 03:55:49.000000 cofi-0.2.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-07 03:56:03.918507 cofi-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-07 03:55:49.000000 cofi-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-07 03:55:49.000000 cofi-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 03:56:03.918507 cofi-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.910507 cofi-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.914507 cofi-0.2.1/src/cofi/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67472 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/_base_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/_inversion_options.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.914507 cofi-0.2.1/src/cofi/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_base_inference_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_cofi_simple_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_emcee.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_pytorch_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_scipy_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_scipy_opt_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/tools/_scipy_opt_min.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.914507 cofi-0.2.1/src/cofi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/utils/_reg_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/utils/_reg_lp_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/utils/_reg_model_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 03:55:49.000000 cofi-0.2.1/src/cofi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.914507 cofi-0.2.1/src/cofi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 03:56:03.000000 cofi-0.2.1/src/cofi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 03:56:03.918507 cofi-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_base_problem_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_base_problem_for_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_base_problem_for_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_base_problem_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_inversion_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 03:55:49.000000 cofi-0.2.1/tests/test_inversion_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.906929 cofi-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-17 23:17:25.000000 cofi-0.2.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-17 23:17:39.906929 cofi-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-17 23:17:25.000000 cofi-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-17 23:17:26.000000 cofi-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:17:39.906929 cofi-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.898929 cofi-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.902929 cofi-0.2.2/src/cofi/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67334 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/_base_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22939 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/_inversion_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.902929 cofi-0.2.2/src/cofi/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_base_inference_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_cofi_simple_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_emcee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_pytorch_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_scipy_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_scipy_opt_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/tools/_scipy_opt_min.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.902929 cofi-0.2.2/src/cofi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/_multiple_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/_reg_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/_reg_lp_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/utils/_reg_model_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:17:26.000000 cofi-0.2.2/src/cofi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.902929 cofi-0.2.2/src/cofi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 23:17:39.000000 cofi-0.2.2/src/cofi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:17:39.906929 cofi-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_base_problem_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_base_problem_for_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_base_problem_for_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_base_problem_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_inversion_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-17 23:17:26.000000 cofi-0.2.2/tests/test_inversion_result.py
```

### Comparing `cofi-0.2.1/LICENCE` & `cofi-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/PKG-INFO` & `cofi-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Common Framework for Inference
 Author: InLab, CoFI development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `cofi-0.2.1/README.md` & `cofi-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/pyproject.toml` & `cofi-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/__init__.py` & `cofi-0.2.2/src/cofi/__init__.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/_base_problem.py` & `cofi-0.2.2/src/cofi/_base_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from numbers import Number
 from typing import Callable, Union, Tuple, Sequence
 import functools
 import json
 
 import numpy as np
 
-from .utils import BaseRegularization
 from ._exceptions import (
     DimensionMismatchError,
     InvalidOptionError,
     InvocationError,
     NotDefinedError,
 )
 
@@ -963,15 +962,15 @@
             self.data_misfit = _FunctionWrapper(
                 "data_misfit", data_misfit, args, kwargs
             )
         self._update_autogen("data_misfit")
 
     def set_regularization(
         self,
-        regularization: Union[Callable[[np.ndarray], Number], BaseRegularization],
+        regularization: Callable[[np.ndarray], Number],
         regularization_matrix: Union[
             np.ndarray, Callable[[np.ndarray], np.ndarray]
         ] = None,
         args: list = None,
         kwargs: dict = None,
     ):
         r"""Sets the function to compute the regularization
@@ -1023,17 +1022,15 @@
         >>> inv_problem.regularization([1,1])
         2
         """
         # preprocess regularization_matrix if there is one
         _reg_matrix = None
         if regularization_matrix is not None:
             _reg_matrix = regularization_matrix
-        elif isinstance(regularization, BaseRegularization) and hasattr(
-            regularization, "matrix"
-        ):
+        elif hasattr(regularization, "matrix"):
             _reg_matrix = regularization.matrix
         # wrap regularization_matrix as a function
         if _reg_matrix is not None and np.ndim(_reg_matrix) != 0:
             self.regularization_matrix = _FunctionWrapper(
                 "regularization_matrix", _matrix_to_func, args=[_reg_matrix]
             )
         elif _reg_matrix is not None and callable(_reg_matrix):
```

### Comparing `cofi-0.2.1/src/cofi/_exceptions.py` & `cofi-0.2.2/src/cofi/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/_inversion.py` & `cofi-0.2.2/src/cofi/_inversion.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/_inversion_options.py` & `cofi-0.2.2/src/cofi/_inversion_options.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/tools/__init__.py` & `cofi-0.2.2/src/cofi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/tools/_base_inference_tool.py` & `cofi-0.2.2/src/cofi/tools/_base_inference_tool.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/tools/_cofi_simple_newton.py` & `cofi-0.2.2/src/cofi/tools/_cofi_simple_newton.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/tools/_emcee.py` & `cofi-0.2.2/src/cofi/tools/_emcee.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/tools/_pytorch_optim.py` & `cofi-0.2.2/src/cofi/tools/_pytorch_optim.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/tools/_scipy_lstsq.py` & `cofi-0.2.2/src/cofi/tools/_scipy_lstsq.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/tools/_scipy_opt_lstsq.py` & `cofi-0.2.2/src/cofi/tools/_scipy_opt_lstsq.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/tools/_scipy_opt_min.py` & `cofi-0.2.2/src/cofi/tools/_scipy_opt_min.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/utils/__init__.py` & `cofi-0.2.2/src/cofi/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 
 """
 
 from ._reg_base import BaseRegularization
 from ._reg_lp_norm import LpNormRegularization, QuadraticReg
 from ._reg_model_cov import ModelCovariance, GaussianPrior
 
+from ._multiple_runs import run_multiple_inversions
+
 
 __all__ = [
     "BaseRegularization",
     "LpNormRegularization",
     "QuadraticReg",
     "ModelCovariance",
     "GaussianPrior",
+    "run_multiple_inversions",
 ]
```

### Comparing `cofi-0.2.1/src/cofi/utils/_reg_base.py` & `cofi-0.2.2/src/cofi/utils/_reg_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -130,34 +130,16 @@
         if self.model_size != other_reg.model_size:
             raise DimensionMismatchError(
                 entered_name="the second regularization term",
                 entered_dimension=other_reg.model_size,
                 expected_source="the first regularization term",
                 expected_dimension=self.model_size,
             )
-        tmp_model_shape = self.model_shape
-        tmp_reg = self.reg
-        tmp_grad = self.gradient
-        tmp_hess = self.hessian
-
-        class CompositeRegularization(BaseRegularization):
-            @property
-            def model_shape(self):
-                return tmp_model_shape
-
-            def reg(self, model):
-                return tmp_reg(model) + other_reg(model)
 
-            def gradient(self, model):
-                return tmp_grad(model) + other_reg.gradient(model)
-
-            def hessian(self, model):
-                return tmp_hess(model) + other_reg.hessian(model)
-
-        return CompositeRegularization()
+        return CompositeRegularization(self, other=other_reg)
 
     def __rmul__(self, coefficient):
         r"""Multiply a regularization term with a constant number
 
         Parameters
         ----------
         coefficient : Number
@@ -188,27 +170,37 @@
 
         """
         if not isinstance(coefficient, Number):
             raise TypeError(
                 f"unsupported operand type(s) for *: '{coefficient.__class__.__name__}'"
                 f" and '{self.__class__.__name__}"
             )
-        tmp_model_shape = self.model_shape
-        tmp_reg = self.reg
-        tmp_grad = self.gradient
-        tmp_hess = self.hessian
-
-        class CompositeRegularization(BaseRegularization):
-            @property
-            def model_shape(self):
-                return tmp_model_shape
-
-            def reg(self, model):
-                return coefficient * tmp_reg(model)
-
-            def gradient(self, model):
-                return coefficient * tmp_grad(model)
+        return CompositeRegularization(self, coefficient=coefficient)
 
-            def hessian(self, model):
-                return coefficient * tmp_hess(model)
 
-        return CompositeRegularization()
+class CompositeRegularization(BaseRegularization):
+    def __init__(self, base, other=None, coefficient=None):
+        self.base = base
+        self.other = other
+        self.coefficient = coefficient
+
+    @property
+    def model_shape(self):
+        return self.base.model_shape
+
+    def reg(self, model):
+        if self.other:
+            return self.base.reg(model) + self.other.reg(model)
+        elif self.coefficient is not None:
+            return self.coefficient * self.base.reg(model)
+
+    def gradient(self, model):
+        if self.other:
+            return self.base.gradient(model) + self.other.gradient(model)
+        elif self.coefficient is not None:
+            return self.coefficient * self.base.gradient(model)
+
+    def hessian(self, model):
+        if self.other:
+            return self.base.hessian(model) + self.other.hessian(model)
+        elif self.coefficient is not None:
+            return self.coefficient * self.base.hessian(model)
```

### Comparing `cofi-0.2.1/src/cofi/utils/_reg_lp_norm.py` & `cofi-0.2.2/src/cofi/utils/_reg_lp_norm.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi/utils/_reg_model_cov.py` & `cofi-0.2.2/src/cofi/utils/_reg_model_cov.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/src/cofi.egg-info/PKG-INFO` & `cofi-0.2.2/src/cofi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Common Framework for Inference
 Author: InLab, CoFI development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `cofi-0.2.1/src/cofi.egg-info/SOURCES.txt` & `cofi-0.2.2/src/cofi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/cofi/tools/_cofi_simple_newton.py
 src/cofi/tools/_emcee.py
 src/cofi/tools/_pytorch_optim.py
 src/cofi/tools/_scipy_lstsq.py
 src/cofi/tools/_scipy_opt_lstsq.py
 src/cofi/tools/_scipy_opt_min.py
 src/cofi/utils/__init__.py
+src/cofi/utils/_multiple_runs.py
 src/cofi/utils/_reg_base.py
 src/cofi/utils/_reg_lp_norm.py
 src/cofi/utils/_reg_model_cov.py
 tests/test_base_problem_basics.py
 tests/test_base_problem_for_optimization.py
 tests/test_base_problem_for_sampling.py
 tests/test_base_problem_misc.py
```

### Comparing `cofi-0.2.1/tests/test_base_problem_basics.py` & `cofi-0.2.2/tests/test_base_problem_basics.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/tests/test_base_problem_for_optimization.py` & `cofi-0.2.2/tests/test_base_problem_for_optimization.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/tests/test_base_problem_for_sampling.py` & `cofi-0.2.2/tests/test_base_problem_for_sampling.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/tests/test_base_problem_misc.py` & `cofi-0.2.2/tests/test_base_problem_misc.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/tests/test_inversion.py` & `cofi-0.2.2/tests/test_inversion.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/tests/test_inversion_options.py` & `cofi-0.2.2/tests/test_inversion_options.py`

 * *Files identical despite different names*

### Comparing `cofi-0.2.1/tests/test_inversion_result.py` & `cofi-0.2.2/tests/test_inversion_result.py`

 * *Files identical despite different names*

