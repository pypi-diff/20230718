# Comparing `tmp/summerepi2-1.2.7.tar.gz` & `tmp/summerepi2-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summerepi2-1.2.7.tar", max compression
+gzip compressed data, was "summerepi2-1.2.8.tar", max compression
```

## Comparing `summerepi2-1.2.7.tar` & `summerepi2-1.2.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1512 2022-09-01 20:25:00.648111 summerepi2-1.2.7/LICENSE.txt
--rw-r--r--   0        0        0     1930 2023-07-18 01:38:03.872027 summerepi2-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     4428 2023-07-18 01:38:31.525826 summerepi2-1.2.7/README.md
--rw-r--r--   0        0        0      280 2022-09-01 05:32:07.966265 summerepi2-1.2.7/summer2/__init__.py
--rw-r--r--   0        0        0     4095 2022-09-01 05:32:07.967266 summerepi2-1.2.7/summer2/adjust.py
--rw-r--r--   0        0        0     4782 2022-09-01 05:32:07.967769 summerepi2-1.2.7/summer2/compartment.py
--rw-r--r--   0        0        0      137 2022-08-26 06:17:31.101047 summerepi2-1.2.7/summer2/compute_bak/__init__.py
--rw-r--r--   0        0        0     2151 2022-08-27 21:20:06.649159 summerepi2-1.2.7/summer2/compute_bak/compute_jax.py
--rw-r--r--   0        0        0    11683 2022-09-01 05:32:07.968765 summerepi2-1.2.7/summer2/derived_outputs.py
--rw-r--r--   0        0        0    10490 2023-04-05 00:33:04.716810 summerepi2-1.2.7/summer2/experimental/model_builder.py
--rw-r--r--   0        0        0     2603 2023-04-19 22:25:13.644705 summerepi2-1.2.7/summer2/extras/test_models.py
--rw-r--r--   0        0        0    19144 2022-09-01 05:32:07.970266 summerepi2-1.2.7/summer2/flows.py
--rw-r--r--   0        0        0      203 2023-02-10 00:07:02.891606 summerepi2-1.2.7/summer2/functions/__init__.py
--rw-r--r--   0        0        0     4640 2023-07-17 21:39:16.749238 summerepi2-1.2.7/summer2/functions/interpolate.py
--rw-r--r--   0        0        0     4620 2023-01-17 01:08:37.545738 summerepi2-1.2.7/summer2/functions/interpolate_old.py
--rw-r--r--   0        0        0     4106 2023-07-18 01:31:47.511898 summerepi2-1.2.7/summer2/functions/time.py
--rw-r--r--   0        0        0     4176 2023-07-17 22:41:45.501478 summerepi2-1.2.7/summer2/functions/util.py
--rw-r--r--   0        0        0     6019 2022-10-11 00:26:22.994134 summerepi2-1.2.7/summer2/inspect.py
--rw-r--r--   0        0        0    53972 2023-07-04 01:20:03.692135 summerepi2-1.2.7/summer2/model.py
--rw-r--r--   0        0        0       22 2022-10-11 01:49:59.803947 summerepi2-1.2.7/summer2/parameters/__init__.py
--rw-r--r--   0        0        0    10987 2023-04-18 23:12:23.096368 summerepi2-1.2.7/summer2/parameters/param_impl.py
--rw-r--r--   0        0        0     4255 2023-04-05 00:33:04.747809 summerepi2-1.2.7/summer2/parameters/params.py
--rw-r--r--   0        0        0     4804 2022-09-01 05:32:07.974766 summerepi2-1.2.7/summer2/population.py
--rw-r--r--   0        0        0       40 2022-09-01 05:32:07.975265 summerepi2-1.2.7/summer2/runner/__init__.py
--rw-r--r--   0        0        0        0 2022-09-01 05:32:07.975767 summerepi2-1.2.7/summer2/runner/jax/__init__.py
--rw-r--r--   0        0        0     5240 2023-05-02 00:15:48.813286 summerepi2-1.2.7/summer2/runner/jax/derived_outputs.py
--rw-r--r--   0        0        0    25732 2023-07-04 01:18:52.606131 summerepi2-1.2.7/summer2/runner/jax/model_impl.py
--rw-r--r--   0        0        0    11588 2023-04-05 00:33:04.765810 summerepi2-1.2.7/summer2/runner/jax/ode.py
--rw-r--r--   0        0        0    11222 2022-10-12 17:29:54.983503 summerepi2-1.2.7/summer2/runner/jax/ode2.py
--rw-r--r--   0        0        0     2736 2022-11-30 22:02:39.159369 summerepi2-1.2.7/summer2/runner/jax/solvers.py
--rw-r--r--   0        0        0     5111 2022-09-01 05:32:08.044494 summerepi2-1.2.7/summer2/runner/jax/stratify.py
--rw-r--r--   0        0        0     8170 2022-12-02 02:13:10.114800 summerepi2-1.2.7/summer2/runner/model_runner.py
--rw-r--r--   0        0        0     6277 2022-10-11 01:50:00.034457 summerepi2-1.2.7/summer2/solver.py
--rw-r--r--   0        0        0    17065 2023-04-18 23:09:58.702374 summerepi2-1.2.7/summer2/stratification.py
--rw-r--r--   0        0        0      472 2022-09-01 05:32:08.049501 summerepi2-1.2.7/summer2/tracker.py
--rw-r--r--   0        0        0     3760 2023-05-11 02:02:50.793367 summerepi2-1.2.7/summer2/utils.py
--rw-r--r--   0        0        0     5949 1970-01-01 00:00:00.000000 summerepi2-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1512 2022-09-01 20:25:00.648111 summerepi2-1.2.8/LICENSE.txt
+-rw-r--r--   0        0        0     1930 2023-07-18 01:41:52.364946 summerepi2-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4428 2023-07-18 01:41:57.110446 summerepi2-1.2.8/README.md
+-rw-r--r--   0        0        0      280 2022-09-01 05:32:07.966265 summerepi2-1.2.8/summer2/__init__.py
+-rw-r--r--   0        0        0     4095 2022-09-01 05:32:07.967266 summerepi2-1.2.8/summer2/adjust.py
+-rw-r--r--   0        0        0     4782 2022-09-01 05:32:07.967769 summerepi2-1.2.8/summer2/compartment.py
+-rw-r--r--   0        0        0      137 2022-08-26 06:17:31.101047 summerepi2-1.2.8/summer2/compute_bak/__init__.py
+-rw-r--r--   0        0        0     2151 2022-08-27 21:20:06.649159 summerepi2-1.2.8/summer2/compute_bak/compute_jax.py
+-rw-r--r--   0        0        0    11683 2022-09-01 05:32:07.968765 summerepi2-1.2.8/summer2/derived_outputs.py
+-rw-r--r--   0        0        0    10490 2023-04-05 00:33:04.716810 summerepi2-1.2.8/summer2/experimental/model_builder.py
+-rw-r--r--   0        0        0     2603 2023-04-19 22:25:13.644705 summerepi2-1.2.8/summer2/extras/test_models.py
+-rw-r--r--   0        0        0    19144 2022-09-01 05:32:07.970266 summerepi2-1.2.8/summer2/flows.py
+-rw-r--r--   0        0        0      203 2023-02-10 00:07:02.891606 summerepi2-1.2.8/summer2/functions/__init__.py
+-rw-r--r--   0        0        0     4640 2023-07-17 21:39:16.749238 summerepi2-1.2.8/summer2/functions/interpolate.py
+-rw-r--r--   0        0        0     4620 2023-01-17 01:08:37.545738 summerepi2-1.2.8/summer2/functions/interpolate_old.py
+-rw-r--r--   0        0        0     4106 2023-07-18 01:31:47.511898 summerepi2-1.2.8/summer2/functions/time.py
+-rw-r--r--   0        0        0     4176 2023-07-17 22:41:45.501478 summerepi2-1.2.8/summer2/functions/util.py
+-rw-r--r--   0        0        0     6019 2022-10-11 00:26:22.994134 summerepi2-1.2.8/summer2/inspect.py
+-rw-r--r--   0        0        0    53972 2023-07-04 01:20:03.692135 summerepi2-1.2.8/summer2/model.py
+-rw-r--r--   0        0        0       22 2022-10-11 01:49:59.803947 summerepi2-1.2.8/summer2/parameters/__init__.py
+-rw-r--r--   0        0        0    10987 2023-04-18 23:12:23.096368 summerepi2-1.2.8/summer2/parameters/param_impl.py
+-rw-r--r--   0        0        0     4255 2023-04-05 00:33:04.747809 summerepi2-1.2.8/summer2/parameters/params.py
+-rw-r--r--   0        0        0     4804 2022-09-01 05:32:07.974766 summerepi2-1.2.8/summer2/population.py
+-rw-r--r--   0        0        0       40 2022-09-01 05:32:07.975265 summerepi2-1.2.8/summer2/runner/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-01 05:32:07.975767 summerepi2-1.2.8/summer2/runner/jax/__init__.py
+-rw-r--r--   0        0        0     5240 2023-05-02 00:15:48.813286 summerepi2-1.2.8/summer2/runner/jax/derived_outputs.py
+-rw-r--r--   0        0        0    25732 2023-07-04 01:18:52.606131 summerepi2-1.2.8/summer2/runner/jax/model_impl.py
+-rw-r--r--   0        0        0    11588 2023-04-05 00:33:04.765810 summerepi2-1.2.8/summer2/runner/jax/ode.py
+-rw-r--r--   0        0        0    11222 2022-10-12 17:29:54.983503 summerepi2-1.2.8/summer2/runner/jax/ode2.py
+-rw-r--r--   0        0        0     2736 2022-11-30 22:02:39.159369 summerepi2-1.2.8/summer2/runner/jax/solvers.py
+-rw-r--r--   0        0        0     5111 2022-09-01 05:32:08.044494 summerepi2-1.2.8/summer2/runner/jax/stratify.py
+-rw-r--r--   0        0        0     8170 2022-12-02 02:13:10.114800 summerepi2-1.2.8/summer2/runner/model_runner.py
+-rw-r--r--   0        0        0     6277 2022-10-11 01:50:00.034457 summerepi2-1.2.8/summer2/solver.py
+-rw-r--r--   0        0        0    17065 2023-04-18 23:09:58.702374 summerepi2-1.2.8/summer2/stratification.py
+-rw-r--r--   0        0        0      472 2022-09-01 05:32:08.049501 summerepi2-1.2.8/summer2/tracker.py
+-rw-r--r--   0        0        0     3760 2023-05-11 02:02:50.793367 summerepi2-1.2.8/summer2/utils.py
+-rw-r--r--   0        0        0     5949 1970-01-01 00:00:00.000000 summerepi2-1.2.8/PKG-INFO
```

### Comparing `summerepi2-1.2.7/LICENSE.txt` & `summerepi2-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/pyproject.toml` & `summerepi2-1.2.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "summerepi2"
-version = "1.2.7"
+version = "1.2.8"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "http://summerepi.com/"
 documentation = "http://summerepi.com/"
 repository = "https://github.com/monash-emu/summer2"
 keywords = [
     "epidemiology",
@@ -20,15 +20,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.0"
 numpy = ">=1.20.3"
 networkx = ">=2.6.2"
 pandas = ">=1.3.2"
 plotly = ">=5.5.0"
-computegraph = "==0.4.2"
+computegraph = "==0.4.3"
 jax =  [
     {extras = ["cpu"], version = ">=0.4", platform = "linux"},
     {extras = ["cpu"], version = ">=0.4", platform = "darwin"},
 ]
 sphinx-rtd-theme = {version = "^0.5.1", optional = true}
 recommonmark = {version = "^0.7.1", optional = true}
 nbsphinx = {version = "^0.8.2", optional = true}
```

### Comparing `summerepi2-1.2.7/README.md` & `summerepi2-1.2.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
   - Removed inner jit in model building to improve debugging
 - 1.2.4
   - CompartmentValues not functioning previously; include more comprehensive check in graph split
 - 1.2.5
   - Previous issue was not resolved correctly; bugfix-bugfix release
 - 1.2.6
   - Make full (comparment) outputs optional for jax runners
-- 1.2.7
+- 1.2.8
   - Improve time varying functions (allow GraphObjects in x values)
 
 ## Release process
 
 To do a release:
 
 - Commit any code changes and push them to GitHub
```

### Comparing `summerepi2-1.2.7/summer2/adjust.py` & `summerepi2-1.2.8/summer2/adjust.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/compartment.py` & `summerepi2-1.2.8/summer2/compartment.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/compute_bak/compute_jax.py` & `summerepi2-1.2.8/summer2/compute_bak/compute_jax.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/derived_outputs.py` & `summerepi2-1.2.8/summer2/derived_outputs.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/experimental/model_builder.py` & `summerepi2-1.2.8/summer2/experimental/model_builder.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/extras/test_models.py` & `summerepi2-1.2.8/summer2/extras/test_models.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/flows.py` & `summerepi2-1.2.8/summer2/flows.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/functions/interpolate.py` & `summerepi2-1.2.8/summer2/functions/interpolate.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/functions/interpolate_old.py` & `summerepi2-1.2.8/summer2/functions/interpolate_old.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/functions/time.py` & `summerepi2-1.2.8/summer2/functions/time.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/functions/util.py` & `summerepi2-1.2.8/summer2/functions/util.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/inspect.py` & `summerepi2-1.2.8/summer2/inspect.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/model.py` & `summerepi2-1.2.8/summer2/model.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/parameters/param_impl.py` & `summerepi2-1.2.8/summer2/parameters/param_impl.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/parameters/params.py` & `summerepi2-1.2.8/summer2/parameters/params.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/population.py` & `summerepi2-1.2.8/summer2/population.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/runner/jax/derived_outputs.py` & `summerepi2-1.2.8/summer2/runner/jax/derived_outputs.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/runner/jax/model_impl.py` & `summerepi2-1.2.8/summer2/runner/jax/model_impl.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/runner/jax/ode.py` & `summerepi2-1.2.8/summer2/runner/jax/ode.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/runner/jax/ode2.py` & `summerepi2-1.2.8/summer2/runner/jax/ode2.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/runner/jax/solvers.py` & `summerepi2-1.2.8/summer2/runner/jax/solvers.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/runner/jax/stratify.py` & `summerepi2-1.2.8/summer2/runner/jax/stratify.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/runner/model_runner.py` & `summerepi2-1.2.8/summer2/runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/solver.py` & `summerepi2-1.2.8/summer2/solver.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/stratification.py` & `summerepi2-1.2.8/summer2/stratification.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/summer2/utils.py` & `summerepi2-1.2.8/summer2/utils.py`

 * *Files identical despite different names*

### Comparing `summerepi2-1.2.7/PKG-INFO` & `summerepi2-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: summerepi2
-Version: 1.2.7
+Version: 1.2.8
 Summary: Summer is a compartmental disease modelling framework, written in Python. It provides a high-level API to build and run models.
 Home-page: http://summerepi.com/
 License: BSD-2-Clause
 Keywords: epidemiology,disease,compartmental,infectious
 Author: James Trauer
 Author-email: james.trauer@monash.edu
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: computegraph (==0.4.2)
+Requires-Dist: computegraph (==0.4.3)
 Requires-Dist: ipykernel (>=6.15.1,<7.0.0) ; extra == "docs"
 Requires-Dist: jax[cpu] (>=0.4) ; sys_platform == "darwin"
 Requires-Dist: jax[cpu] (>=0.4) ; sys_platform == "linux"
 Requires-Dist: matplotlib (>=3.4.3) ; extra == "docs"
 Requires-Dist: nbsphinx (>=0.8.2,<0.9.0) ; extra == "docs"
 Requires-Dist: networkx (>=2.6.2)
 Requires-Dist: numpy (>=1.20.3)
@@ -132,15 +132,15 @@
   - Removed inner jit in model building to improve debugging
 - 1.2.4
   - CompartmentValues not functioning previously; include more comprehensive check in graph split
 - 1.2.5
   - Previous issue was not resolved correctly; bugfix-bugfix release
 - 1.2.6
   - Make full (comparment) outputs optional for jax runners
-- 1.2.7
+- 1.2.8
   - Improve time varying functions (allow GraphObjects in x values)
 
 ## Release process
 
 To do a release:
 
 - Commit any code changes and push them to GitHub
```

