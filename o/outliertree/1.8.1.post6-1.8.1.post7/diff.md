# Comparing `tmp/outliertree-1.8.1.post6.tar.gz` & `tmp/outliertree-1.8.1.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outliertree-1.8.1.post6.tar", last modified: Sat Mar 25 16:58:22 2023, max compression
+gzip compressed data, was "outliertree-1.8.1.post7.tar", last modified: Tue Jul 18 18:46:30 2023, max compression
```

## Comparing `outliertree-1.8.1.post6.tar` & `outliertree-1.8.1.post7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:58:22.082233 outliertree-1.8.1.post6/
--rw-r--r--   0 david     (1000) david     (1000)    35149 2019-07-14 14:58:06.000000 outliertree-1.8.1.post6/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      682 2021-08-23 00:10:59.000000 outliertree-1.8.1.post6/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      273 2023-03-25 16:58:22.082233 outliertree-1.8.1.post6/PKG-INFO
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:58:22.082233 outliertree-1.8.1.post6/outliertree/
--rw-r--r--   0 david     (1000) david     (1000)    62848 2022-05-30 20:05:04.000000 outliertree-1.8.1.post6/outliertree/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)    51998 2023-03-19 18:00:27.000000 outliertree-1.8.1.post6/outliertree/outlier_cpp_interface.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:58:22.082233 outliertree-1.8.1.post6/outliertree.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      273 2023-03-25 16:58:22.000000 outliertree-1.8.1.post6/outliertree.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      381 2023-03-25 16:58:22.000000 outliertree-1.8.1.post6/outliertree.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-03-25 16:58:22.000000 outliertree-1.8.1.post6/outliertree.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       12 2023-03-25 16:58:22.000000 outliertree-1.8.1.post6/outliertree.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       86 2021-04-15 16:07:15.000000 outliertree-1.8.1.post6/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)       28 2020-04-28 17:04:55.000000 outliertree-1.8.1.post6/requirements.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-03-25 16:58:22.082233 outliertree-1.8.1.post6/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    13688 2023-03-25 16:57:54.000000 outliertree-1.8.1.post6/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-03-25 16:58:22.082233 outliertree-1.8.1.post6/src/
--rw-r--r--   0 david     (1000) david     (1000)    14620 2021-10-14 17:47:05.000000 outliertree-1.8.1.post6/src/cat_outlier.cpp
--rw-r--r--   0 david     (1000) david     (1000)    47798 2021-12-15 00:27:15.000000 outliertree-1.8.1.post6/src/clusters.cpp
--rw-r--r--   0 david     (1000) david     (1000)   133408 2022-02-17 15:09:38.000000 outliertree-1.8.1.post6/src/fit_model.cpp
--rw-r--r--   0 david     (1000) david     (1000)    31965 2022-02-17 15:09:25.000000 outliertree-1.8.1.post6/src/misc.cpp
--rw-r--r--   0 david     (1000) david     (1000)    46846 2022-02-17 15:09:30.000000 outliertree-1.8.1.post6/src/outlier_tree.hpp
--rw-r--r--   0 david     (1000) david     (1000)    37668 2021-10-14 17:47:05.000000 outliertree-1.8.1.post6/src/predict.cpp
--rw-r--r--   0 david     (1000) david     (1000)    50701 2022-02-17 14:25:53.000000 outliertree-1.8.1.post6/src/split.cpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 18:46:30.101287 outliertree-1.8.1.post7/
+-rw-r--r--   0 david     (1000) david     (1000)    35149 2019-07-14 14:58:06.000000 outliertree-1.8.1.post7/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      682 2021-08-23 00:10:59.000000 outliertree-1.8.1.post7/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      273 2023-07-18 18:46:30.101287 outliertree-1.8.1.post7/PKG-INFO
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 18:46:30.101287 outliertree-1.8.1.post7/outliertree/
+-rw-r--r--   0 david     (1000) david     (1000)    62848 2022-05-30 20:05:04.000000 outliertree-1.8.1.post7/outliertree/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)    51998 2023-07-18 18:44:09.000000 outliertree-1.8.1.post7/outliertree/outlier_cpp_interface.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 18:46:30.101287 outliertree-1.8.1.post7/outliertree.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      273 2023-07-18 18:46:30.000000 outliertree-1.8.1.post7/outliertree.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      414 2023-07-18 18:46:30.000000 outliertree-1.8.1.post7/outliertree.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-18 18:46:30.000000 outliertree-1.8.1.post7/outliertree.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       12 2023-07-18 18:46:30.000000 outliertree-1.8.1.post7/outliertree.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       69 2023-07-18 18:45:20.000000 outliertree-1.8.1.post7/outliertree_compiler_testing.cpp
+-rw-r--r--   0 david     (1000) david     (1000)       82 2023-07-18 18:45:07.000000 outliertree-1.8.1.post7/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)       41 2023-07-18 18:45:16.000000 outliertree-1.8.1.post7/requirements.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-18 18:46:30.101287 outliertree-1.8.1.post7/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    13774 2023-07-18 18:44:39.000000 outliertree-1.8.1.post7/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 18:46:30.101287 outliertree-1.8.1.post7/src/
+-rw-r--r--   0 david     (1000) david     (1000)    14620 2021-10-14 17:47:05.000000 outliertree-1.8.1.post7/src/cat_outlier.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    47798 2021-12-15 00:27:15.000000 outliertree-1.8.1.post7/src/clusters.cpp
+-rw-r--r--   0 david     (1000) david     (1000)   133408 2022-02-17 15:09:38.000000 outliertree-1.8.1.post7/src/fit_model.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    31965 2022-02-17 15:09:25.000000 outliertree-1.8.1.post7/src/misc.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    46846 2022-02-17 15:09:30.000000 outliertree-1.8.1.post7/src/outlier_tree.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    37668 2021-10-14 17:47:05.000000 outliertree-1.8.1.post7/src/predict.cpp
+-rw-r--r--   0 david     (1000) david     (1000)    50701 2022-02-17 14:25:53.000000 outliertree-1.8.1.post7/src/split.cpp
```

### Comparing `outliertree-1.8.1.post6/LICENSE` & `outliertree-1.8.1.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `outliertree-1.8.1.post6/MANIFEST.in` & `outliertree-1.8.1.post7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `outliertree-1.8.1.post6/outliertree/__init__.py` & `outliertree-1.8.1.post7/outliertree/__init__.py`

 * *Files identical despite different names*

### Comparing `outliertree-1.8.1.post6/outliertree/outlier_cpp_interface.pyx` & `outliertree-1.8.1.post7/outliertree/outlier_cpp_interface.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -99,29 +99,29 @@
         size_t ncols_categ
         size_t ncols_ord
         vector[double] min_outlier_any_cl
         vector[double] max_outlier_any_cl
         vector[vector[bool_t]] cat_outlier_any_cl
         size_t max_depth
 
-    bool_t get_has_openmp() nogil except +
+    bool_t get_has_openmp() except + nogil
 
     bool_t fit_outliers_models(ModelOutputs &model_outputs,
                                double *numeric_data,     size_t ncols_numeric,
                                int    *categorical_data, size_t ncols_categ,   int *ncat,
                                int    *ordinal_data,     size_t ncols_ord,     int *ncat_ord,
                                size_t nrows, char *cols_ignore, int nthreads,
                                bool_t categ_as_bin, bool_t ord_as_bin, bool_t cat_bruteforce_subset, bool_t categ_from_maj, bool_t take_mid,
                                size_t max_conditions, double max_perc_outliers, size_t min_size_numeric, size_t min_size_categ,
-                               double min_gain, bool_t gain_as_pct, bool_t follow_all, double z_norm, double z_outlier) nogil except +
+                               double min_gain, bool_t gain_as_pct, bool_t follow_all, double z_norm, double z_outlier) except + nogil
 
     bool_t find_new_outliers(double *numeric_data,
                              int    *categorical_data,
                              int    *ordinal_data,
-                             size_t nrows, int nthreads, ModelOutputs &model_outputs) nogil except +
+                             size_t nrows, int nthreads, ModelOutputs &model_outputs) except + nogil
 
     void forget_row_outputs(ModelOutputs &model_outputs)
 
     void check_more_two_values(double *arr_num, size_t nrows, size_t ncols, int nthreads, char *too_few_values)
 
     void dealloc_ModelOutputs(ModelOutputs &model_outputs)
```

### Comparing `outliertree-1.8.1.post6/setup.py` & `outliertree-1.8.1.post7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,28 +277,29 @@
             for e in self.extensions:
                 e.define_macros += [("SUPPORTS_RESTRICT", "1")]
 
 
 setup(
     name  = "outliertree",
     packages = ["outliertree"],
-    version = '1.8.1-6',
+    version = '1.8.1-7',
     description = 'Explainable outlier detection through smart decision tree conditioning',
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/outliertree',
     keywords = ['outlier', 'anomaly', 'gritbot'],
     cmdclass = {'build_ext': build_ext_subclass},
     ext_modules = [Extension(
                                 "outliertree._outlier_cpp_interface",
                                 sources=["outliertree/outlier_cpp_interface.pyx", "src/split.cpp", "src/cat_outlier.cpp",
                                          "src/fit_model.cpp", "src/clusters.cpp", "src/misc.cpp", "src/predict.cpp"],
                                 include_dirs=[np.get_include(), ".", "./src"],
                                 define_macros=[
                                     ("_FOR_PYTHON", None),
-                                    ("NDEBUG", None)
+                                    ("NDEBUG", None),
+                                    ("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")
                                 ],
                                 language="c++",
                             )]
     ) 
 
 if not found_omp:
     omp_msg  = "\n\n\nCould not detect OpenMP. Package will be built without multi-threading capabilities. "
```

### Comparing `outliertree-1.8.1.post6/src/cat_outlier.cpp` & `outliertree-1.8.1.post7/src/cat_outlier.cpp`

 * *Files identical despite different names*

### Comparing `outliertree-1.8.1.post6/src/clusters.cpp` & `outliertree-1.8.1.post7/src/clusters.cpp`

 * *Files identical despite different names*

### Comparing `outliertree-1.8.1.post6/src/fit_model.cpp` & `outliertree-1.8.1.post7/src/fit_model.cpp`

 * *Files identical despite different names*

### Comparing `outliertree-1.8.1.post6/src/misc.cpp` & `outliertree-1.8.1.post7/src/misc.cpp`

 * *Files identical despite different names*

### Comparing `outliertree-1.8.1.post6/src/outlier_tree.hpp` & `outliertree-1.8.1.post7/src/outlier_tree.hpp`

 * *Files identical despite different names*

### Comparing `outliertree-1.8.1.post6/src/predict.cpp` & `outliertree-1.8.1.post7/src/predict.cpp`

 * *Files identical despite different names*

### Comparing `outliertree-1.8.1.post6/src/split.cpp` & `outliertree-1.8.1.post7/src/split.cpp`

 * *Files identical despite different names*

