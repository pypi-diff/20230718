# Comparing `tmp/sympde-0.9.8.tar.gz` & `tmp/sympde-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sympde-0.9.8.tar", last modified: Thu Mar 19 08:41:34 2020, max compression
+gzip compressed data, was "dist/sympde-0.9.9.tar", last modified: Thu Apr 16 08:32:39 2020, max compression
```

## Comparing `sympde-0.9.8.tar` & `sympde-0.9.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-03-19 08:41:34.000000 sympde-0.9.8/
-drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde.egg-info/
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)        1 2019-01-21 13:53:41.000000 sympde-0.9.8/sympde.egg-info/zip-safe
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)        1 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde.egg-info/dependency_links.txt
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1982 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde.egg-info/PKG-INFO
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)        7 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde.egg-info/top_level.txt
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       46 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde.egg-info/requires.txt
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      981 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde.egg-info/SOURCES.txt
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1384 2019-12-18 17:17:19.000000 sympde-0.9.8/setup.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       19 2019-01-15 16:22:47.000000 sympde-0.9.8/MANIFEST.in
-drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde/
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       22 2020-03-19 08:41:00.000000 sympde-0.9.8/sympde/version.py
-drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde/expr/
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    21646 2020-03-19 08:41:00.000000 sympde-0.9.8/sympde/expr/expr.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    36247 2020-03-19 08:41:00.000000 sympde-0.9.8/sympde/expr/evaluation.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      130 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/expr/__init__.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      443 2019-01-21 13:51:59.000000 sympde-0.9.8/sympde/expr/errors.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    11693 2019-12-18 10:21:23.000000 sympde-0.9.8/sympde/expr/equation.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     9211 2020-03-19 08:41:00.000000 sympde-0.9.8/sympde/expr/basic.py
-drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde/core/
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     5796 2019-10-02 11:30:33.000000 sympde-0.9.8/sympde/core/utils.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       84 2019-08-19 12:00:59.000000 sympde-0.9.8/sympde/core/__init__.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1351 2019-08-30 11:35:43.000000 sympde-0.9.8/sympde/core/basic.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     7626 2019-08-19 12:00:59.000000 sympde-0.9.8/sympde/core/algebra.py
-drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde/exterior/
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    19260 2019-11-19 17:08:05.000000 sympde-0.9.8/sympde/exterior/compiler.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1222 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/exterior/form.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     3895 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/exterior/datatype.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    15096 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/exterior/calculus.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     2268 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/exterior/inference.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      154 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/exterior/__init__.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      135 2019-08-30 16:38:07.000000 sympde-0.9.8/sympde/__init__.py
-drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde/topology/
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    26748 2019-11-19 17:08:05.000000 sympde-0.9.8/sympde/topology/derivatives.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     2868 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/topology/datatype.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    24892 2020-03-19 08:41:00.000000 sympde-0.9.8/sympde/topology/mapping.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      196 2019-08-19 12:00:59.000000 sympde-0.9.8/sympde/topology/__init__.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    21834 2019-12-18 17:17:19.000000 sympde-0.9.8/sympde/topology/domain.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1553 2019-01-15 16:22:47.000000 sympde-0.9.8/sympde/topology/measure.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    10350 2019-12-18 17:17:19.000000 sympde-0.9.8/sympde/topology/basic.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    24766 2019-11-19 17:08:05.000000 sympde-0.9.8/sympde/topology/space.py
-drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde/printing/
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    11319 2019-09-11 09:55:48.000000 sympde-0.9.8/sympde/printing/latex.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       22 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/printing/__init__.py
-drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-03-19 08:41:34.000000 sympde-0.9.8/sympde/calculus/
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    52305 2019-11-19 17:08:05.000000 sympde-0.9.8/sympde/calculus/core.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       44 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/calculus/__init__.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      186 2019-08-05 11:34:31.000000 sympde-0.9.8/sympde/calculus/errors.py
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1982 2020-03-19 08:41:34.000000 sympde-0.9.8/PKG-INFO
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1254 2019-08-21 15:17:13.000000 sympde-0.9.8/README.rst
--rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       38 2020-03-19 08:41:34.000000 sympde-0.9.8/setup.cfg
+drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-04-16 08:32:39.000000 sympde-0.9.9/
+drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-04-16 08:32:38.000000 sympde-0.9.9/sympde.egg-info/
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)        1 2019-01-21 13:53:41.000000 sympde-0.9.9/sympde.egg-info/zip-safe
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)        1 2020-04-16 08:32:37.000000 sympde-0.9.9/sympde.egg-info/dependency_links.txt
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1982 2020-04-16 08:32:37.000000 sympde-0.9.9/sympde.egg-info/PKG-INFO
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)        7 2020-04-16 08:32:37.000000 sympde-0.9.9/sympde.egg-info/top_level.txt
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       46 2020-04-16 08:32:37.000000 sympde-0.9.9/sympde.egg-info/requires.txt
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      981 2020-04-16 08:32:38.000000 sympde-0.9.9/sympde.egg-info/SOURCES.txt
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1384 2020-04-16 08:28:10.000000 sympde-0.9.9/setup.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       19 2019-01-15 16:22:47.000000 sympde-0.9.9/MANIFEST.in
+drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-04-16 08:32:38.000000 sympde-0.9.9/sympde/
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       22 2020-04-16 08:28:15.000000 sympde-0.9.9/sympde/version.py
+drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-04-16 08:32:38.000000 sympde-0.9.9/sympde/expr/
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    21646 2020-03-19 08:41:00.000000 sympde-0.9.9/sympde/expr/expr.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    32839 2020-04-16 08:28:15.000000 sympde-0.9.9/sympde/expr/evaluation.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      130 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/expr/__init__.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      443 2019-01-21 13:51:59.000000 sympde-0.9.9/sympde/expr/errors.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    11693 2019-12-18 10:21:23.000000 sympde-0.9.9/sympde/expr/equation.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     9211 2020-03-19 08:41:00.000000 sympde-0.9.9/sympde/expr/basic.py
+drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-04-16 08:32:38.000000 sympde-0.9.9/sympde/core/
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     5796 2019-10-02 11:30:33.000000 sympde-0.9.9/sympde/core/utils.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       84 2019-08-19 12:00:59.000000 sympde-0.9.9/sympde/core/__init__.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1351 2019-08-30 11:35:43.000000 sympde-0.9.9/sympde/core/basic.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     7626 2019-08-19 12:00:59.000000 sympde-0.9.9/sympde/core/algebra.py
+drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-04-16 08:32:39.000000 sympde-0.9.9/sympde/exterior/
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    19260 2019-11-19 17:08:05.000000 sympde-0.9.9/sympde/exterior/compiler.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1222 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/exterior/form.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     3895 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/exterior/datatype.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    15096 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/exterior/calculus.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     2268 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/exterior/inference.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      154 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/exterior/__init__.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      135 2019-08-30 16:38:07.000000 sympde-0.9.9/sympde/__init__.py
+drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-04-16 08:32:39.000000 sympde-0.9.9/sympde/topology/
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    26884 2020-04-16 08:28:15.000000 sympde-0.9.9/sympde/topology/derivatives.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     2868 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/topology/datatype.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    25107 2020-04-16 08:28:15.000000 sympde-0.9.9/sympde/topology/mapping.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      196 2019-08-19 12:00:59.000000 sympde-0.9.9/sympde/topology/__init__.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    22284 2020-04-16 08:28:15.000000 sympde-0.9.9/sympde/topology/domain.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1553 2019-01-15 16:22:47.000000 sympde-0.9.9/sympde/topology/measure.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    10598 2020-04-16 08:28:15.000000 sympde-0.9.9/sympde/topology/basic.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    24766 2019-11-19 17:08:05.000000 sympde-0.9.9/sympde/topology/space.py
+drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-04-16 08:32:39.000000 sympde-0.9.9/sympde/printing/
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    11319 2019-09-11 09:55:48.000000 sympde-0.9.9/sympde/printing/latex.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       22 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/printing/__init__.py
+drwxr-xr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2020-04-16 08:32:38.000000 sympde-0.9.9/sympde/calculus/
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)    52312 2020-04-16 08:28:15.000000 sympde-0.9.9/sympde/calculus/core.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       44 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/calculus/__init__.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)      186 2019-08-05 11:34:31.000000 sympde-0.9.9/sympde/calculus/errors.py
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1982 2020-04-16 08:32:39.000000 sympde-0.9.9/PKG-INFO
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)     1254 2019-08-21 15:17:13.000000 sympde-0.9.9/README.rst
+-rw-r--r--   0 yamanguc  (1000) yamanguc  (1000)       38 2020-04-16 08:32:39.000000 sympde-0.9.9/setup.cfg
```

### Comparing `sympde-0.9.8/sympde.egg-info/PKG-INFO` & `sympde-0.9.9/sympde.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: sympde
-Version: 0.9.8
+Version: 0.9.9
 Summary: Symbolic calculus for partial differential equations (and variational forms).
 Home-page: https://github.com/pyccel/sympde
 Author: Ahmed Ratnani
 Author-email: ratnaniahmed@gmail.com
 License: LICENSE
 Description: sympde
         ======
```

### Comparing `sympde-0.9.8/sympde.egg-info/SOURCES.txt` & `sympde-0.9.9/sympde.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/setup.py` & `sympde-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/expr/expr.py` & `sympde-0.9.9/sympde/expr/expr.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/expr/evaluation.py` & `sympde-0.9.9/sympde/expr/evaluation.py`

 * *Files 5% similar despite different names*

```diff
@@ -230,93 +230,14 @@
     if not(test_indices is None) and trial_indices is None:
         return _to_matrix_linear_form(expr, M, test_indices)
 
     if test_indices is None and trial_indices is None:
         return _to_matrix_functional_form(expr, M)
 
 #==============================================================================
-def _split_expr_over_subdomains(expr, interiors, tests=None, trials=None):
-    """
-    Splits an expression defined on a domain, having multiple interiors, into
-    expressions where the test and trial functions are defined on each side of
-    the subdomain.
-
-    Parameters:
-        expr: sympde expression
-
-        interiors: an interior or union of interiors
-
-        tests: tests functions as given from linear or bilinear forms
-
-        trials: trials functions as given from linear or bilinear forms
-
-    Returns: sympde expression
-    """
-    # ...
-    def _new_atom(v, interior):
-        new = '{v}_{domain}'.format( v      = v.name,
-                                     domain = interior.name )
-        return element_of(v.space, name=new)
-    # ...
-
-    # ...
-    is_bilinear = not( trials is None ) and not( tests is None )
-    is_linear   =    ( trials is None ) and not( tests is None )
-
-    if trials is None: trials = []
-    if tests  is None: tests  = []
-    # ...
-
-    # ...
-    d_expr = {}
-    for interior in interiors:
-        d_expr[interior] = 0
-    # ...
-
-    # ... create trial/test functions on each subdomain
-    d_trials = {}
-    d_tests  = {}
-    for interior in interiors:
-        # ...
-        news = []
-        for v in trials:
-            new = _new_atom(v, interior)
-            news.append(new)
-        d_trials[interior] = news
-        # ...
-
-        # ...
-        news = []
-        for v in tests:
-            new = _new_atom(v, interior)
-            news.append(new)
-        d_tests[interior] = news
-        # ...
-    # ...
-
-    # ...
-    for interior in interiors:
-        d_expr[interior] = expr
-
-        # use trial functions on each subdomain
-        olds = trials
-        news = d_trials[interior]
-        for old,new in zip(olds, news):
-            d_expr[interior] = d_expr[interior].subs({old: new})
-
-        # use test functions on each subdomain
-        olds = tests
-        news = d_tests[interior]
-        for old,new in zip(olds, news):
-            d_expr[interior] = d_expr[interior].subs({old: new})
-    # ...
-
-    return d_expr
-
-#==============================================================================
 def _split_expr_over_interface(expr, interface, tests=None, trials=None):
     """
     Splits an expression defined on an interface, into
     expressions where the test and trial functions are defined on each side of
     the interface.
 
     Parameters:
@@ -327,35 +248,21 @@
         tests: tests functions as given from linear or bilinear forms
 
         trials: trials functions as given from linear or bilinear forms
 
     Returns: sympde expression
     """
     # ...
-    def _new_atom(v, label):
-        new = '{v}_{label}'.format( v     = v.name,
-                                    label = label )
-        return element_of(v.space, name=new)
-    # ...
-
-    # ...
     is_bilinear = not( trials is None ) and not( tests is None )
     is_linear   =    ( trials is None ) and not( tests is None )
 
     if trials is None: trials = []
     if tests  is None: tests  = []
     # ...
 
-    # ...
-    B_minus = interface.minus
-    B_plus  = interface.plus
-    boundaries = (B_minus, B_plus)
-    labels     = ('minus', 'plus')
-    # ...
-
     int_expressions = []
     bnd_expressions = {}
 
     # ...
     # we replace all jumps
     jumps = expr.atoms(Jump)
     args = [j._args[0] for j in jumps]
@@ -402,85 +309,69 @@
 
     # ...
     def _nullify(expr, u, us):
         """nullifies all symbols in us except u."""
         others = list(set(us) - set([u]))
         for other in others:
             expr = expr.subs({other: 0})
-
         return expr
     # ...
-
-    # ...
-    def _not_zero_matrix(M):
-        n,m = expr.shape
-        return any([M[i,j] != 0 for i,j in product(range(n), range(m))])
-    # ...
-
-    # ...
     if is_bilinear:
         for u in d_trials.keys():
             u_minus = d_trials[u]['-']
             u_plus  = d_trials[u]['+']
             for v in d_tests.keys():
                 v_minus = d_tests[v]['-']
                 v_plus  = d_tests[v]['+']
 
                 # ...
                 newexpr = _nullify(expr, u_minus, trials)
                 newexpr = _nullify(newexpr, v_minus, tests)
                 newexpr = newexpr.subs({u_minus: u, v_minus: v})
-                if _not_zero_matrix(newexpr):
+                if not newexpr.is_zero:
                     bnd_expressions[interface.minus] = newexpr
                 # ...
-
-                # ...
                 # TODO must call InterfaceExpression afterward
                 newexpr = _nullify(expr, u_minus, trials)
                 newexpr = _nullify(newexpr, v_plus, tests)
-                if _not_zero_matrix(newexpr):
-                    int_expressions += [InterfaceExpression(interface, newexpr)]
-                # ...
-
+                if not newexpr.is_zero:
+                    int_expressions += [InterfaceExpression(interface, u_minus, v_plus, newexpr)]
                 # ...
                 # TODO must call InterfaceExpression afterward
                 newexpr = _nullify(expr, u_plus, trials)
                 newexpr = _nullify(newexpr, v_minus, tests)
-                if _not_zero_matrix(newexpr):
-                    int_expressions += [InterfaceExpression(interface, newexpr)]
-                # ...
 
+                if not newexpr.is_zero:
+                    int_expressions += [InterfaceExpression(interface, u_plus, v_minus, newexpr)]
                 # ...
                 newexpr = _nullify(expr, u_plus, trials)
                 newexpr = _nullify(newexpr, v_plus, tests)
                 newexpr = newexpr.subs({u_plus: u, v_plus: v})
-                if _not_zero_matrix(newexpr):
+                if not newexpr.is_zero:
                     bnd_expressions[interface.plus] = newexpr
                 # ...
 
     elif is_linear:
         for v in d_tests.keys():
             v_minus = d_tests[v]['-']
             v_plus  = d_tests[v]['+']
 
             # ...
             newexpr = _nullify(expr, v_minus, tests)
             newexpr = newexpr.subs({v_minus: v})
-            if _not_zero_matrix(newexpr):
+            if not newexpr.is_zero:
                 bnd_expressions[interface.minus] = newexpr
             # ...
 
             # ...
             newexpr = _nullify(expr, v_plus, tests)
             newexpr = newexpr.subs({v_plus: v})
-            if _not_zero_matrix(newexpr):
+            if not newexpr.is_zero:
                 bnd_expressions[interface.plus] = newexpr
             # ...
-    # ...
-
     return int_expressions, bnd_expressions
 
 
 #==============================================================================
 class KernelExpression(Basic):
     def __new__(cls, target, expr):
         assert(isinstance(expr, (Matrix, ImmutableDenseMatrix)))
@@ -503,16 +394,27 @@
 
 #==============================================================================
 class BoundaryExpression(KernelExpression):
     pass
 
 #==============================================================================
 class InterfaceExpression(KernelExpression):
-    pass
+    def __new__(cls, target, u, v, expr):
+        obj = KernelExpression.__new__(cls, target, expr)
+        obj._trial = u
+        obj._test  = v
+        return obj
 
+    @property
+    def test(self):
+        return self._test
+
+    @property
+    def trial(self):
+        return self._trial
 
 #==============================================================================
 class TerminalExpr(CalculusFunction):
 
     def __new__(cls, *args, **options):
         # (Try to) sympify args first
 
@@ -601,15 +503,14 @@
             # ...
 
             # ...
             d_expr = {}
             for d in domain:
                 d_expr[d] = S.Zero
             # ...
-
             if isinstance(expr.expr, Add):
                 for a in expr.expr.args:
                     newexpr = cls.eval(a, dim=dim)
                     newexpr = expand(newexpr)
 
                     # ...
                     try:
@@ -667,17 +568,14 @@
 
                     d_new[domain] = M
             # ...
 
             # ...
             ls = []
             d_all = {}
-            # ...
-#            print(d_new)
-#            print([type(i) for i in d_new.keys()])
 
             # ... treating interfaces
             keys = [k for k in d_new.keys() if isinstance(k, Interface)]
             for interface in keys:
                 # ...
                 trials = None
                 tests  = None
@@ -687,104 +585,71 @@
 
                 elif expr.is_linear:
                     tests  = list(expr.variables)
                 # ...
 
                 # ...
                 newexpr = d_new[interface]
-                ls_int, d = _split_expr_over_interface(newexpr, interface,
+                ls_int, d_bnd = _split_expr_over_interface(newexpr, interface,
                                                        tests=tests,
                                                        trials=trials)
                 # ...
 
-                # ...
                 ls += ls_int
                 # ...
-
-                # ...
-                for k, v in d.items():
+                for k, v in d_bnd.items():
                     if k in d_all.keys():
                         d_all[k] += v
 
                     else:
                         d_all[k] = v
-                # ...
             # ...
 
             # ... treating subdomains
             keys = [k for k in d_new.keys() if isinstance(k, Union)]
             for domain in keys:
-                # ...
-                trials = None
-                tests  = None
-                if expr.is_bilinear:
-                    trials = list(expr.variables[0])
-                    tests  = list(expr.variables[1])
-
-                elif expr.is_linear:
-                    tests  = list(expr.variables)
-
-                else:
-                    raise NotImplementedError('Only Bilinear and Linear forms are available')
-                # ...
 
-                # ...
                 newexpr = d_new[domain]
-                d = _split_expr_over_subdomains(newexpr, domain.as_tuple(),
-                                                tests=tests, trials=trials)
-                # ...
-
-                # ...
+                d       = {interior : newexpr for interior in domain.as_tuple()}
+                            # ...
                 for k, v in d.items():
                     if k in d_all.keys():
                         d_all[k] += v
 
                     else:
                         d_all[k] = v
-                # ...
-            # ...
 
-            # ...
             d = {}
 
             for k, v in d_new.items():
-                if not isinstance( k, (Interface, Union) ):
+                if not isinstance( k, (Interface, Union)):
                     d[k] = d_new[k]
 
             for k, v in d_all.items():
                 if k in d.keys():
                     d[k] += v
-
                 else:
                     d[k] = v
 
             d_new = d
             # ...
-
-            # ...
             for domain, newexpr in d_new.items():
                 if isinstance(domain, Boundary):
                     ls += [BoundaryExpression(domain, newexpr)]
 
-                elif isinstance(domain, Interface):
-                    ls += [InterfaceExpression(domain, newexpr)]
-
                 elif isinstance(domain, BasicDomain):
                     ls += [DomainExpression(domain, newexpr)]
 
                 else:
                     raise TypeError('not implemented for {}'.format(type(domain)))
             # ...
             return ls
 
         elif isinstance(expr, (DomainIntegral, BoundaryIntegral, InterfaceIntegral)):
-            if dim is None:
-                domain = expr.domain
-                dim = domain.dim
-
+            dim = expr.domain.dim if dim is None else dim
             return cls.eval(expr._args[0], dim=dim)
 
         elif isinstance(expr, NormalVector):
             lines = [[expr[i] for i in range(dim)]]
             return Matrix(lines)
 
         elif isinstance(expr, TangentVector):
@@ -1174,17 +1039,16 @@
             # ...
 
             # ...
             logical = False
             if not(mapping is None):
                 logical = True
                 terminal_expr = LogicalExpr(mapping, terminal_expr.expr)
-
-                det_M = DetJacobian(mapping)
-                det   = SymbolicDeterminant(mapping)
+                det_M         = DetJacobian(mapping)
+                det           = SymbolicDeterminant(mapping)
                 terminal_expr = terminal_expr.subs(det_M, det)
                 terminal_expr = expand(terminal_expr)
             # ...
 
             # ...
             expr = cls.eval(terminal_expr, d_atoms=d_atoms, mapping=mapping)
             # ...
```

### Comparing `sympde-0.9.8/sympde/expr/equation.py` & `sympde-0.9.9/sympde/expr/equation.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/expr/basic.py` & `sympde-0.9.9/sympde/expr/basic.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/core/utils.py` & `sympde-0.9.9/sympde/core/utils.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/core/basic.py` & `sympde-0.9.9/sympde/core/basic.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/core/algebra.py` & `sympde-0.9.9/sympde/core/algebra.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/exterior/compiler.py` & `sympde-0.9.9/sympde/exterior/compiler.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/exterior/form.py` & `sympde-0.9.9/sympde/exterior/form.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/exterior/datatype.py` & `sympde-0.9.9/sympde/exterior/datatype.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/exterior/calculus.py` & `sympde-0.9.9/sympde/exterior/calculus.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/exterior/inference.py` & `sympde-0.9.9/sympde/exterior/inference.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/topology/derivatives.py` & `sympde-0.9.9/sympde/topology/derivatives.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from sympde.core.basic import CalculusFunction
 from sympde.core.basic import _coeffs_registery
 from sympde.core.basic import BasicMapping
 from sympde.core.algebra import LinearOperator
 from .space import ScalarTestFunction, VectorTestFunction, IndexedTestTrial
 from .space import ScalarField, VectorField, IndexedVectorField
+from sympde.calculus.core import minus, plus
 
 #==============================================================================
 class DifferentialOperator(LinearOperator):
     """
     This class is a linear operator that applies the Leibniz formula
 
     """
@@ -44,21 +45,23 @@
         return self
 
     @classmethod
     def eval(cls, *_args):
         """."""
 
         expr = _args[0]
-
         if isinstance(expr, (IndexedTestTrial, IndexedVectorField, DifferentialOperator)):
             return cls(expr, evaluate=False)
 
         elif isinstance(expr, (ScalarField, ScalarTestFunction)):
             return cls(expr, evaluate=False)
 
+        elif isinstance(expr, (minus, plus)):
+            return cls(expr, evaluate=False)
+
         elif isinstance(expr, (VectorTestFunction, VectorField)):
             n = expr.shape[0]
             args = [cls(expr[i], evaluate=False) for i in range(0, n)]
             args = Tuple(*args)
             return Matrix([args])
 
         elif isinstance(expr, Indexed) and isinstance(expr.base, BasicMapping):
```

### Comparing `sympde-0.9.8/sympde/topology/datatype.py` & `sympde-0.9.9/sympde/topology/datatype.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/topology/mapping.py` & `sympde-0.9.9/sympde/topology/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from sympy.core import Basic
 from sympy.core import Symbol
 from sympy.core import Add, Mul, Pow
 from sympy.core.expr       import AtomicExpr
 from sympy.core.numbers    import ImaginaryUnit
 from sympy.core.containers import Tuple
 
+from sympde.calculus.core import PlusInterfaceOperator, MinusInterfaceOperator
+
 from sympde.core       import Constant
 from sympde.core.basic import BasicMapping
 from sympde.core.basic import CalculusFunction
 from sympde.core.basic import _coeffs_registery
 from sympde.topology   import NormalVector
 
 from .basic       import BasicDomain
@@ -791,14 +793,17 @@
             if code:
                 name = '{name}_{code}'.format(name=expr.name, code=code)
             else:
                 name = str(expr.name)
 
             return Symbol(name)
 
+        elif isinstance(expr, ( PlusInterfaceOperator, MinusInterfaceOperator)):
+            return cls.eval(expr.args[0], code=code)
+
         elif isinstance(expr, Indexed):
             base = expr.base
             if isinstance(base, Mapping):
                 if expr.indices[0] == 0:
                     name = 'x'
                 elif expr.indices[0] == 1:
                     name = 'y'
```

### Comparing `sympde-0.9.8/sympde/topology/domain.py` & `sympde-0.9.9/sympde/topology/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     A domain without a boundary is either infinite or periodic.
     A domain can also be constructed from a connectivity, in which case, only the
     name and connectivity need to be passed.
 
     """
 
     def __new__(cls, name, interiors=None, boundaries=None, dim=None,
-                connectivity=None, dtype=None):
+                connectivity=None):
         # ...
         if not isinstance(name, str):
             raise TypeError('> name must be a string')
         # ...
 
         # ...
         if ( ( interiors is None ) and ( connectivity is None ) and ( dim is None) ):
@@ -91,42 +91,41 @@
         if not( connectivity is None ):
             if not isinstance( connectivity, Connectivity ):
                 raise TypeError('> Expecting a Connectivity')
 
             # TODO check that patches appearing in connectivity are in interiors
         else:
             connectivity = Connectivity()
-        # ...
 
         # ...
-        if not dim is None:
-            assert(isinstance( dim, int ))
-
+        if interiors is None and dim:
             interiors = [InteriorDomain(name, dim=dim)]
-        # ...
 
-        # ...
-        if len(interiors) == 0:
+        if len(interiors) == 0 and dim is None:
             raise TypeError('No interior domain found')
 
         elif len(interiors) == 1:
             interiors = interiors[0]
+            dtype = interiors.dtype
+            dim   = interiors.dim
 
         elif len(interiors) > 1:
+            dtype = interiors[0].dtype
+            dim   = interiors[0].dim
             interiors = Union(*interiors)
-        # ...
 
         # ...
         if len(boundaries) > 1:
             boundaries = Union(*boundaries)
         # ...
 
         obj = Basic.__new__(cls, name, interiors, boundaries)
         obj._connectivity = connectivity
-        obj._dtype = dtype
+        obj._dtype        = dtype
+        obj._dim          = dim
 
         return obj
 
     @property
     def name(self):
         return self.args[0]
 
@@ -140,15 +139,15 @@
 
     @property
     def connectivity(self):
         return self._connectivity
 
     @property
     def dim(self):
-        return self.interior.dim
+        return self._dim
 
     @property
     def dtype(self):
         return self._dtype
 
     @property
     def interfaces(self):
@@ -350,31 +349,29 @@
         # ... interiors
         interiors = [self.interior, other.interior]
         # ...
 
         # ... connectivity
         connectivity = Connectivity()
         # TODO be careful with '|' in psydac
-        connectivity['{l}|{r}'.format(l=self.name, r=other.name)] = (bnd_minus, bnd_plus)
-
+        connectivity['{l}|{r}'.format(l=bnd_minus.domain.name, r=bnd_plus.domain.name)] = (bnd_minus, bnd_plus)
         for k,v in self.connectivity.items():
             connectivity[k] = v
 
         for k,v in other.connectivity.items():
             connectivity[k] = v
         # ...
 
         # ... boundary
         boundaries_minus = self.boundary.complement(bnd_minus)
         boundaries_plus  = other.boundary.complement(bnd_plus)
 
         boundaries = Union(boundaries_minus, boundaries_plus)
         boundaries = boundaries.as_tuple()
         # ...
-
         return Domain(name,
                       interiors=interiors,
                       boundaries=boundaries,
                       connectivity=connectivity)
 
 #==============================================================================
 class PeriodicDomain(BasicDomain):
@@ -417,14 +414,27 @@
     @property
     def coordinates(self):
         return self.domain.coordinates
 
     def __hash__(self):
         return self.domain.__hash__() + self._periods.__hash__()
 
+
+#==============================================================================
+class NCubeInterior(InteriorDomain):
+    _min_coords = None
+    _max_coords = None
+    @property
+    def min_coords(self):
+        return self._min_coords
+
+    @property
+    def max_coords(self):
+        return self._max_coords
+
 #==============================================================================
 # Ncube's properties (in addition to Domain's properties):
 #   . min_coords (default value is tuple of zeros)
 #   . max_coords (default value is tuple of ones)
 #
 class NCube(Domain):
 
@@ -450,32 +460,17 @@
         # Choose coordinate names. TODO: use unique convention
         if dim <= 3:
             coord_names = ('x', 'y', 'z')[:dim]
         else:
             coord_names = 'x1:{}'.format(dim + 1)
 
         coordinates = symbols(coord_names)
-        intervals   = [Interval('I_{}'.format(c.name), coordinate=c, bounds=(xmin, xmax))
+        intervals   = [Interval('{}_{}'.format(name, c.name), coordinate=c, bounds=(xmin, xmax))
                        for c, xmin, xmax in zip(coordinates, min_coords, max_coords)]
 
-        if len(intervals) == 1:
-            interior = intervals[0]
-        else:
-            interior = ProductDomain(*intervals, name=name)
-            interior = InteriorDomain(interior)
-
-        boundaries = []
-        i = 1
-        for axis in range(interior.dim):
-            for ext in [-1, 1]:
-                bnd_name = r'\Gamma_{}'.format(i)
-                Gamma = Boundary(bnd_name, interior, axis=axis, ext=ext)
-                boundaries += [Gamma]
-                i += 1
-
         # Choose which type to use:
         #   a) if dim <= 3, use Line, Square or Cube;
         #   b) if dim <= 4, use a generic 'NCube' type.
         #
         # Moreover, store all initialization parameters in a 'dtype' dictionary.
         # This dictionary will be written to file when exporting the geometry,
         # and it must contain all information necessary for building a new object
@@ -501,39 +496,54 @@
                                     'bounds3': [min_coords[2], max_coords[2]]}}
         else:
             dtype = {'type': 'NCube',
                      'parameters': {'dim'       : dim,
                                     'min_coords': [*min_coords],
                                     'max_coords': [*max_coords]}}
 
+        if len(intervals) == 1:
+            interior = intervals[0]
+        else:
+            interior = ProductDomain(*intervals, name=name)
+
+        interior             = NCubeInterior(interior, dtype=dtype)
+        interior._min_coords = tuple(min_coords)
+        interior._max_coords = tuple(max_coords)
+
+        boundaries = []
+        i = 1
+        for axis in range(dim):
+            for ext in [-1, 1]:
+                bnd_name = r'\Gamma_{}'.format(i)
+                Gamma = Boundary(bnd_name, interior, axis=axis, ext=ext)
+                boundaries += [Gamma]
+                i += 1
+
         # Create instance of given type
         obj = super().__new__(cls, name, interiors=[interior],
-                boundaries=boundaries, dtype=dtype)
+                boundaries=boundaries)
 
         # Store attributes in object
         obj._coordinates = tuple(coordinates)
-        obj._min_coords  = tuple(min_coords)
-        obj._max_coords  = tuple(max_coords)
 
         # Return object
         return obj
 
     @classmethod
     def from_file(cls, filename):
         msg = "Class method 'from_file' must be called on 'Domain' base class"
         raise TypeError(msg)
 
     @property
     def min_coords(self):
-        return self._min_coords
+        return self.interior.min_coords
 
     @property
     def max_coords(self):
-        return self._max_coords
-
+        return self.interior.max_coords
 #==============================================================================
 class Line(NCube):
 
     def __new__(cls, name='Line', bounds=(0, 1)):
         dim = 1
         min_coords = (bounds[0],)
         max_coords = (bounds[1],)
```

### Comparing `sympde-0.9.8/sympde/topology/measure.py` & `sympde-0.9.9/sympde/topology/measure.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/topology/basic.py` & `sympde-0.9.9/sympde/topology/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,39 +39,47 @@
 class InteriorDomain(BasicDomain):
     """
     Represents an undefined interior domain.
 
     Examples
 
     """
-    def __new__(cls, name, dim=None):
+    def __new__(cls, name, dim=None, dtype=None):
         target = None
         if not isinstance(name, str):
             target = name
             name   = name.name
 
         if not( target is None ):
-            if isinstance(target, ProductDomain):
-                dim = target.dim
+            dim = target.dim
 
         obj = Basic.__new__(cls, name)
 
         obj._dim    = dim
         obj._target = target
+        obj._dtype  = dtype
 
         return obj
 
     @property
     def name(self):
         return self.args[0]
 
     @property
     def target(self):
         return self._target
 
+    @property
+    def dtype(self):
+        return self._dtype
+
+    @property
+    def dim(self):
+        return self._dim
+
     def _sympystr(self, printer):
         sstr = printer.doprint
         return '{}'.format(sstr(self.name))
 
     def todict(self):
         name   = str(self.name)
         d = {'name': name}
@@ -172,15 +180,17 @@
 class Interval(InteriorDomain):
     """
     Represents a 1D interval.
 
     Examples
 
     """
+
     _dim = 1
+
     def __new__(cls, name=None, coordinate=None, bounds=None):
         if name is None:
             name = 'Interval'
 
         if bounds is None:
             bounds = (0, 1)
 
@@ -196,14 +206,15 @@
     def name(self):
         return self.args[0]
 
     @property
     def bounds(self):
         return self._bounds
 
+
 #==============================================================================
 class Boundary(BasicDomain):
     """
     Represents an undefined boundary over a domain.
 
     Examples
 
@@ -238,15 +249,15 @@
 
     @property
     def dim(self):
         return self.domain.dim
 
     def _sympystr(self, printer):
         sstr = printer.doprint
-        return '{}'.format(sstr(self.name))
+        return '{}_{}'.format(sstr(self.domain.name),sstr(self.name))
 
     def __add__(self, other):
         if isinstance(other, ComplementBoundary):
             raise TypeError('> Cannot add complement of boundary')
 
         return Union(self, other)
 
@@ -276,15 +287,15 @@
         if not isinstance(edge     , Edge    ): raise TypeError(edge)
         if not isinstance(bnd_minus, Boundary): raise TypeError(bnd_minus)
         if not isinstance(bnd_plus , Boundary): raise TypeError(bnd_plus)
 
         if bnd_minus.dim != bnd_plus.dim:
             raise TypeError('Dimension mismatch: {} != {}'.format(
                 bnd_minus.dim, bnd_plus.dim))
-
+        assert bnd_minus.axis == bnd_plus.axis
         return Basic.__new__(cls, edge.name, bnd_minus, bnd_plus)
 
     @property
     def dim(self):
         return self.minus.dim
 
     @property
@@ -295,14 +306,18 @@
     def minus(self):
         return self.args[1]
 
     @property
     def plus(self):
         return self.args[2]
 
+    @property
+    def axis(self):
+        return self.plus.axis
+
     def _sympystr(self, printer):
         sstr = printer.doprint
 
 #        name  = self.name
 #        minus = self.minus
 #        plus  = self.plus
 #        minus = '{domain}.{bnd}'.format( domain = sstr(minus.domain),
```

### Comparing `sympde-0.9.8/sympde/topology/space.py` & `sympde-0.9.9/sympde/topology/space.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/printing/latex.py` & `sympde-0.9.9/sympde/printing/latex.py`

 * *Files identical despite different names*

### Comparing `sympde-0.9.8/sympde/calculus/core.py` & `sympde-0.9.9/sympde/calculus/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 from sympde.core.basic import CalculusFunction
 from sympde.core.basic import _coeffs_registery
 
 from sympde.topology.space import ScalarTestFunction, VectorTestFunction, IndexedTestTrial
 from sympde.topology.space import ScalarField, VectorField, IndexedVectorField
 from sympde.topology.space import _is_sympde_atom
-from sympde.topology import NormalVector, MinusNormalVector, PlusNormalVector
+from sympde.topology.domain import NormalVector, MinusNormalVector, PlusNormalVector
 from sympde.topology.datatype import H1SpaceType, HcurlSpaceType
 from sympde.topology.datatype import HdivSpaceType, L2SpaceType, UndefinedSpaceType
 
 from .errors import ArgumentTypeError
 
 
 #==============================================================================
```

### Comparing `sympde-0.9.8/PKG-INFO` & `sympde-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: sympde
-Version: 0.9.8
+Version: 0.9.9
 Summary: Symbolic calculus for partial differential equations (and variational forms).
 Home-page: https://github.com/pyccel/sympde
 Author: Ahmed Ratnani
 Author-email: ratnaniahmed@gmail.com
 License: LICENSE
 Description: sympde
         ======
```

### Comparing `sympde-0.9.8/README.rst` & `sympde-0.9.9/README.rst`

 * *Files identical despite different names*

