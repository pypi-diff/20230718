# Comparing `tmp/bs_python_utils-0.1.tar.gz` & `tmp/bs_python_utils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.1.tar", max compression
+gzip compressed data, was "bs_python_utils-0.2.tar", max compression
```

## Comparing `bs_python_utils-0.1.tar` & `bs_python_utils-0.2.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.1/LICENSE
--rw-r--r--   0        0        0     1490 2023-06-20 20:42:14.388128 bs_python_utils-0.1/README.md
--rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.1/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.1/bs_python_utils/__init__.py
--rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.1/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.1/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.1/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.1/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.1/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.1/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.1/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.1/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.1/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    32084 2023-06-20 20:51:26.724318 bs_python_utils-0.1/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.1/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.1/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.753098 bs_python_utils-0.1/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0    14016 2023-06-20 20:58:35.021722 bs_python_utils-0.1/bs_python_utils/chebyshev.py
--rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.1/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.1/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.1/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.1/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.1/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.1/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.1/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.1/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.1/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1455 2023-05-27 22:42:00.768780 bs_python_utils-0.1/bs_python_utils/tests
--rw-r--r--   0        0        0     1868 2023-06-20 20:59:29.194874 bs_python_utils-0.1/pyproject.toml
--rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 bs_python_utils-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.000000 bs_python_utils-0.2/LICENSE
+-rw-r--r--   0        0        0     1564 2023-07-17 22:10:49.909803 bs_python_utils-0.2/README.md
+-rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.000000 bs_python_utils-0.2/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.000000 bs_python_utils-0.2/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.000000 bs_python_utils-0.2/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    13890 2023-07-17 22:06:48.747455 bs_python_utils-0.2/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.000000 bs_python_utils-0.2/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.000000 bs_python_utils-0.2/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-04-24 19:42:58.000000 bs_python_utils-0.2/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    32084 2023-06-20 20:51:26.000000 bs_python_utils-0.2/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.000000 bs_python_utils-0.2/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.000000 bs_python_utils-0.2/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.000000 bs_python_utils-0.2/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0    14016 2023-06-20 20:58:35.000000 bs_python_utils-0.2/bs_python_utils/chebyshev.py
+-rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.000000 bs_python_utils-0.2/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.000000 bs_python_utils-0.2/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.000000 bs_python_utils-0.2/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.000000 bs_python_utils-0.2/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      552 2023-04-24 22:36:28.000000 bs_python_utils-0.2/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-04-24 21:45:53.000000 bs_python_utils-0.2/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      786 2023-04-24 22:36:28.000000 bs_python_utils-0.2/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.000000 bs_python_utils-0.2/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.000000 bs_python_utils-0.2/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1868 2023-07-17 22:09:47.445621 bs_python_utils-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bs_python_utils-0.2/PKG-INFO
```

### Comparing `bs_python_utils-0.1/LICENSE` & `bs_python_utils-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/README.md` & `bs_python_utils-0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+#### 0.2 (July 17, 2023)
+Fixed printing in accelerated gradient descent.
+
 #### 0.1 (June 20, 2023)
 Added `grid_function` and the `chebyshev` module. 
 
 #### 0.0.6 (May 9, 2023)
 
 Improved docs.
```

### Comparing `bs_python_utils-0.1/bs_python_utils/Timer.py` & `bs_python_utils-0.2/bs_python_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bs_altair.py` & `bs_python_utils-0.2/bs_python_utils/bs_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bs_logging.py` & `bs_python_utils-0.2/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.2/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bs_mem.py` & `bs_python_utils-0.2/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bs_opt.py` & `bs_python_utils-0.2/bs_python_utils/bs_opt.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,33 +214,34 @@
     verbose: bool = False,
     tol: float = 1e-9,
     alpha: float = 1.01,
     beta: float = 0.5,
     maxiter: int = 10000,
 ) -> tuple[np.ndarray, int]:
     """
-    minimizes `(f+h)` by Accelerated Gradient Descent
-     where `f` is smooth and convex  and `h` is convex.
+    minimizes `(f+h)` by Accelerated Gradient Descent where `f` is smooth and convex  and `h` is convex.
 
     By default `h` is zero.
+    The convergence criterion is that the largest component of the absolute value of the gradient must be smaller than `tol`.
+
 
     Args:
         grad_f: grad_f of `f`; should return an `(n)` array from an `(n)` array \
         and the `other_ params` object
         x_init: initial guess, shape `(n)`
         prox_h: proximal projector of `h`, if any
         other_params: an iterable with additional parameters
-        verbose: if `True`, print diagnosis
-        tol: convergence criterion on absolute grad_f
+        verbose: if `True`, print remaining gradient error every 10 iterations
+        tol: convergence criterion on grad_f
         alpha: ceiling on step multiplier
         beta: floor on step multiplier
         maxiter: max number of iterations
 
     Returns: 
-        the candidate solution, and 1 if converged/0 if not
+        the candidate solution, and a convergence code (0 if successful, 1 if not)
     """
 
     # no proximal projection if no h
     local_prox_h: ProximalFunction = prox_h if prox_h else lambda x, t, p: x
 
     x = x_init.copy()
     y = x_init.copy()
@@ -278,32 +279,32 @@
         g = grad_f(y, other_params)
         ndy = spla.norm(y - yi)
         t_hat = 0.5 * ndy * ndy / abs(np.dot(y - yi, gi - g))
         t = min(alpha * t, max(beta * t, t_hat))
 
         n_iter += 1
 
-        if verbose:
+        if verbose and n_iter % 10 == 0:
             print(f" AGD with grad_err = {grad_err} after {n_iter} iterations")
 
     x_conv = y
 
     ret_code = 0 if grad_err < tol else 1
 
     if verbose or print_result:
         if ret_code == 0:
             print_stars(
-                f" AGD converged with grad_err = {grad_err} after {iter} iterations"
+                f" AGD converged with grad_err = {grad_err} after {n_iter} iterations"
             )
         else:
             print_stars(
-                f" Problem in AGD: grad_err = {grad_err} after {iter} iterations"
+                f" Problem in AGD: grad_err = {grad_err} after {n_iter} iterations"
             )
 
-    return (x_conv, ret_code)
+    return x_conv, ret_code
 
 
 def _fix_some(
     obj: Callable, grad_obj: Callable, fixed_vars: list[int], fixed_vals: np.ndarray
 ) -> tuple[Callable, Callable]:
     """
     Takes in a function and its gradient, fixes the variables
```

### Comparing `bs_python_utils-0.1/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.2/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.2/bs_python_utils/bs_sparse_gaussian.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.2/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bsnputils.py` & `bs_python_utils-0.2/bs_python_utils/bsnputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bssputils.py` & `bs_python_utils-0.2/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bsstats.py` & `bs_python_utils-0.2/bs_python_utils/bsstats.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/bsutils.py` & `bs_python_utils-0.2/bs_python_utils/bsutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/chebyshev.py` & `bs_python_utils-0.2/bs_python_utils/chebyshev.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.2/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/example_opt.py` & `bs_python_utils-0.2/bs_python_utils/example_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/examples_altair.py` & `bs_python_utils-0.2/bs_python_utils/examples_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.2/bs_python_utils/examples_distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/examples_mem.py` & `bs_python_utils-0.2/bs_python_utils/examples_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.2/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.2/bs_python_utils/examples_sklearn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.2/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.2/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.1/pyproject.toml` & `bs_python_utils-0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.1"
+version = "0.2"
 description = "my Python utilities"
 authors = ["Bernard Salanie <bsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
```

### Comparing `bs_python_utils-0.1/PKG-INFO` & `bs_python_utils-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.1
+Version: 0.2
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
 Author-email: bsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -33,14 +33,17 @@
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+#### 0.2 (July 17, 2023)
+Fixed printing in accelerated gradient descent.
+
 #### 0.1 (June 20, 2023)
 Added `grid_function` and the `chebyshev` module. 
 
 #### 0.0.6 (May 9, 2023)
 
 Improved docs.
```

