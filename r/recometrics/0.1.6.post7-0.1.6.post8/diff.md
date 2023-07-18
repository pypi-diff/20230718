# Comparing `tmp/recometrics-0.1.6.post7.tar.gz` & `tmp/recometrics-0.1.6.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recometrics-0.1.6.post7.tar", last modified: Mon Jul  3 18:57:17 2023, max compression
+gzip compressed data, was "recometrics-0.1.6.post8.tar", last modified: Tue Jul 18 19:52:20 2023, max compression
```

## Comparing `recometrics-0.1.6.post7.tar` & `recometrics-0.1.6.post8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/
--rw-r--r--   0 david     (1000) david     (1000)     1317 2021-06-22 23:08:42.000000 recometrics-0.1.6.post7/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      700 2021-07-12 00:19:42.000000 recometrics-0.1.6.post7/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)       95 2022-01-20 17:22:42.000000 recometrics-0.1.6.post7/pyproject.toml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/recometrics/
--rw-r--r--   0 david     (1000) david     (1000)    38717 2023-07-03 18:56:28.000000 recometrics-0.1.6.post7/recometrics/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      951 2023-07-03 18:55:43.000000 recometrics-0.1.6.post7/recometrics/wrapper.h
--rw-r--r--   0 david     (1000) david     (1000)    27792 2023-07-03 18:53:43.000000 recometrics-0.1.6.post7/recometrics/wrapper.pyx
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/recometrics.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-03 18:57:16.000000 recometrics-0.1.6.post7/recometrics.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      371 2023-07-03 18:57:17.000000 recometrics-0.1.6.post7/recometrics.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-03 18:57:16.000000 recometrics-0.1.6.post7/recometrics.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       26 2023-07-03 18:57:16.000000 recometrics-0.1.6.post7/recometrics.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       12 2023-07-03 18:57:16.000000 recometrics-0.1.6.post7/recometrics.egg-info/top_level.txt
--rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)    13482 2023-07-03 18:49:26.000000 recometrics-0.1.6.post7/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-03 18:57:17.045452 recometrics-0.1.6.post7/src/
--rw-r--r--   0 david     (1000) david     (1000)    64977 2023-02-16 17:41:12.000000 recometrics-0.1.6.post7/src/recometrics.hpp
--rw-r--r--   0 david     (1000) david     (1000)    10477 2021-07-25 03:17:47.000000 recometrics-0.1.6.post7/src/recometrics_instantiated.cpp
--rw-r--r--   0 david     (1000) david     (1000)     7426 2021-07-25 03:17:28.000000 recometrics-0.1.6.post7/src/recometrics_signatures.hpp
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/
+-rw-r--r--   0 david     (1000) david     (1000)     1317 2021-06-22 23:08:42.000000 recometrics-0.1.6.post8/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)      700 2021-07-12 00:19:42.000000 recometrics-0.1.6.post8/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)       99 2023-07-18 19:49:29.000000 recometrics-0.1.6.post8/pyproject.toml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/recometrics/
+-rw-r--r--   0 david     (1000) david     (1000)    38717 2023-07-03 18:56:28.000000 recometrics-0.1.6.post8/recometrics/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     2269 2023-07-18 19:51:03.000000 recometrics-0.1.6.post8/recometrics/wrapper.h
+-rw-r--r--   0 david     (1000) david     (1000)    27792 2023-07-18 19:48:20.000000 recometrics-0.1.6.post8/recometrics/wrapper.pyx
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/recometrics.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)      248 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)      371 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       26 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       12 2023-07-18 19:52:20.000000 recometrics-0.1.6.post8/recometrics.egg-info/top_level.txt
+-rw-r--r--   0 david     (1000) david     (1000)       38 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)    13598 2023-07-18 19:48:02.000000 recometrics-0.1.6.post8/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-07-18 19:52:20.510808 recometrics-0.1.6.post8/src/
+-rw-r--r--   0 david     (1000) david     (1000)    64977 2023-02-16 17:41:12.000000 recometrics-0.1.6.post8/src/recometrics.hpp
+-rw-r--r--   0 david     (1000) david     (1000)    10477 2021-07-25 03:17:47.000000 recometrics-0.1.6.post8/src/recometrics_instantiated.cpp
+-rw-r--r--   0 david     (1000) david     (1000)     7426 2021-07-25 03:17:28.000000 recometrics-0.1.6.post8/src/recometrics_signatures.hpp
```

### Comparing `recometrics-0.1.6.post7/LICENSE` & `recometrics-0.1.6.post8/LICENSE`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post7/MANIFEST.in` & `recometrics-0.1.6.post8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post7/recometrics/__init__.py` & `recometrics-0.1.6.post8/recometrics/__init__.py`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post7/recometrics/wrapper.pyx` & `recometrics-0.1.6.post8/recometrics/wrapper.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 cdef public double ddot_(const int* n, const double* x, const int* incx, const double* y, const int* incy) nogil:
     return (<ddot__>ddot)(n, x, incx, y, incy)
 
 cdef public float sdot_(const int* n, const float* x, const int* incx, const float* y, const int* incy) nogil:
     return (<sdot__>sdot)(n, x, incx, y, incy)
 
 cdef extern from "recometrics_signatures.hpp":
-    c_bool get_has_openmp() nogil except +
+    c_bool get_has_openmp() except + nogil
 
     void calc_metrics_double(
         const double *A, const size_t lda, const double *B, const size_t ldb,
         const int32_t m, const int32_t n, const int32_t k,
         const int32_t *Xtrain_csr_p, const int32_t *Xtrain_csr_i,
         const int32_t *Xtest_csr_p, const int32_t *Xtest_csr_i, const double *Xtest_csr,
         const int32_t k_metrics,
@@ -55,30 +55,30 @@
         double *roc_auc,
         double *pr_auc,
         const c_bool consider_cold_start,
         int32_t min_items_pool,
         int32_t min_pos_test,
         int32_t nthreads,
         uint64_t seed
-    ) nogil except +
+    ) except + nogil
 
     void split_data_selected_users_double(
         const int32_t *X_csr_p,
         const int32_t *X_csr_i,
         const double *X_csr,
         const int32_t m, const int32_t n,
         vector[int32_t] &Xtrain_csr_p,
         vector[int32_t] &Xtrain_csr_i,
         vector[double] &Xtrain_csr,
         vector[int32_t] &Xtest_csr_p,
         vector[int32_t] &Xtest_csr_i,
         vector[double] &Xtest_csr,
         const double test_fraction,
         uint64_t seed
-    ) nogil except +
+    ) except + nogil
 
     void split_data_separate_users_double(
         const int32_t *X_csr_p,
         const int32_t *X_csr_i,
         const double *X_csr,
         int32_t m, int32_t n,
         vector[int32_t] &users_test,
@@ -93,15 +93,15 @@
         vector[double] &Xtest_csr,
         const int32_t n_users_test,
         const double test_fraction,
         const c_bool consider_cold_start,
         const int32_t min_items_pool,
         const int32_t min_pos_test,
         uint64_t seed
-    ) nogil except +
+    ) except + nogil
 
     void split_data_joined_users_double(
         const int32_t *X_csr_p,
         const int32_t *X_csr_i,
         const double *X_csr,
         int32_t m, int32_t n,
         vector[int32_t] &users_test,
@@ -113,15 +113,15 @@
         vector[double] &Xtest_csr,
         const int32_t n_users_test,
         const double test_fraction,
         const c_bool consider_cold_start,
         const int32_t min_items_pool,
         const int32_t min_pos_test,
         uint64_t seed
-    ) nogil except +
+    ) except + nogil
 
     void calc_metrics_float(
         const float *A, const size_t lda, const float *B, const size_t ldb,
         const int32_t m, const int32_t n, const int32_t k,
         const int32_t *Xtrain_csr_p, const int32_t *Xtrain_csr_i,
         const int32_t *Xtest_csr_p, const int32_t *Xtest_csr_i, const float *Xtest_csr,
         const int32_t k_metrics,
@@ -138,30 +138,30 @@
         float *roc_auc,
         float *pr_auc,
         const c_bool consider_cold_start,
         int32_t min_items_pool,
         int32_t min_pos_test,
         int32_t nthreads,
         uint64_t seed
-    ) nogil except +
+    ) except + nogil
 
     void split_data_selected_users_float(
         const int32_t *X_csr_p,
         const int32_t *X_csr_i,
         const float *X_csr,
         const int32_t m, const int32_t n,
         vector[int32_t] &Xtrain_csr_p,
         vector[int32_t] &Xtrain_csr_i,
         vector[float] &Xtrain_csr,
         vector[int32_t] &Xtest_csr_p,
         vector[int32_t] &Xtest_csr_i,
         vector[float] &Xtest_csr,
         const double test_fraction,
         uint64_t seed
-    ) nogil except +
+    ) except + nogil
 
     void split_data_separate_users_float(
         const int32_t *X_csr_p,
         const int32_t *X_csr_i,
         const float *X_csr,
         int32_t m, int32_t n,
         vector[int32_t] &users_test,
@@ -176,15 +176,15 @@
         vector[float] &Xtest_csr,
         const int32_t n_users_test,
         const double test_fraction,
         const c_bool consider_cold_start,
         const int32_t min_items_pool,
         const int32_t min_pos_test,
         uint64_t seed
-    ) nogil except +
+    ) except + nogil
 
     void split_data_joined_users_float(
         const int32_t *X_csr_p,
         const int32_t *X_csr_i,
         const float *X_csr,
         int32_t m, int32_t n,
         vector[int32_t] &users_test,
@@ -196,15 +196,15 @@
         vector[float] &Xtest_csr,
         const int32_t n_users_test,
         const double test_fraction,
         const c_bool consider_cold_start,
         const int32_t min_items_pool,
         const int32_t min_pos_test,
         uint64_t seed
-    ) nogil except +
+    ) except + nogil
 
 def _get_has_openmp():
     return get_has_openmp()
 
 cdef double* get_ptr_double(np.ndarray[double, ndim=1] a):
     if a.shape[0]:
         return &a[0]
```

### Comparing `recometrics-0.1.6.post7/setup.py` & `recometrics-0.1.6.post8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,28 +280,30 @@
                 e.define_macros += [("SUPPORTS_RESTRICT", "1")]
 
 
 
 setup(
     name  = "recometrics",
     packages = ["recometrics"],
-    version = '0.1.6-7',
+    version = '0.1.6-8',
     cmdclass = {'build_ext': build_ext_subclass},
     author = 'David Cortes',
     url = 'https://github.com/david-cortes/recometrics',
     install_requires = ['numpy', 'scipy', 'cython', 'pandas'],
     description = 'Library-agnostic evaluation framework for implicit-feedback recommender systems',
     ext_modules = [
         Extension("recometrics.cpp_funs",
             language="c++",
             sources=["recometrics/wrapper.pyx", "src/recometrics_instantiated.cpp"],
             include_dirs=[np.get_include(), "src"],
             define_macros=[
                 ("_FOR_PYTHON", None),
                 ("NDEBUG", None),
+                ("CYTHON_EXTERN_C", 'extern "C"'),
+                ("NPY_NO_DEPRECATED_API", "NPY_1_7_API_VERSION")
             ]
             )
         ]
 )
 
 if not found_omp:
     omp_msg  = "\n\n\nCould not detect OpenMP. Package will be built without multi-threading capabilities. "
```

### Comparing `recometrics-0.1.6.post7/src/recometrics.hpp` & `recometrics-0.1.6.post8/src/recometrics.hpp`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post7/src/recometrics_instantiated.cpp` & `recometrics-0.1.6.post8/src/recometrics_instantiated.cpp`

 * *Files identical despite different names*

### Comparing `recometrics-0.1.6.post7/src/recometrics_signatures.hpp` & `recometrics-0.1.6.post8/src/recometrics_signatures.hpp`

 * *Files identical despite different names*

