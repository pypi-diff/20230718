# Comparing `tmp/alpaka-job-coverage-1.3.2.tar.gz` & `tmp/alpaka-job-coverage-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.3.2.tar", last modified: Mon Jul 17 11:29:01 2023, max compression
+gzip compressed data, was "alpaka-job-coverage-1.3.3.tar", last modified: Tue Jul 18 15:24:52 2023, max compression
```

## Comparing `alpaka-job-coverage-1.3.2.tar` & `alpaka-job-coverage-1.3.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.502150 alpaka-job-coverage-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 11:29:01.000000 alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:29:01.506150 alpaka-job-coverage-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/tests/test_compiler_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/tests/test_cuda_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 11:28:44.000000 alpaka-job-coverage-1.3.2/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:24:52.842141 alpaka-job-coverage-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-18 15:24:52.842141 alpaka-job-coverage-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:24:52.842141 alpaka-job-coverage-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:24:52.838141 alpaka-job-coverage-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:24:52.838141 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:24:52.842141 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-18 15:24:52.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-18 15:24:52.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:24:52.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-18 15:24:52.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 15:24:52.000000 alpaka-job-coverage-1.3.3/src/alpaka_job_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:24:52.842141 alpaka-job-coverage-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/tests/test_compiler_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/tests/test_cuda_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/tests/test_hipcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/tests/test_single_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:24:35.000000 alpaka-job-coverage-1.3.3/version.txt
```

### Comparing `alpaka-job-coverage-1.3.2/LICENSE` & `alpaka-job-coverage-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/PKG-INFO` & `alpaka-job-coverage-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.2
+Version: 1.3.3
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.3.2/README.md` & `alpaka-job-coverage-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/setup.py` & `alpaka-job-coverage-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_backend_version.py` & `alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,18 +110,14 @@
 
     ###########################
     ## hipcc device compiler
     ###########################
 
     # the HIP backend needs to be enabled and has the same version number
     if row_check_name(row, DEVICE_COMPILER, "==", HIPCC):
-        # the HIP backend needs to be defined
-        if backend_is_not_in_row(row, ALPAKA_ACC_GPU_HIP_ENABLE):
-            return False
-
         if row_check_backend_version(
             row,
             ALPAKA_ACC_GPU_HIP_ENABLE,
             "!=",
             row[param_map[DEVICE_COMPILER]][VERSION],
         ):
             return False
```

### Comparing `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_compiler_name.py` & `alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/filter_compiler_name.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_compiler_version.py` & `alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/filter_compiler_version.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/filter_software_dependency.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,8 +120,20 @@
     # a bug in CMAKE 3.18 avoids the correct usage of the variable CMAKE_CUDA_ARCHITECTURE if the
     # CUDA compiler is Clang++
     if row_check_name(row, DEVICE_COMPILER, "==", CLANG_CUDA) and row_check_version(
         row, CMAKE, "<", "3.19"
     ):
         return False
 
+    # disable nvcc 11.3 + gcc 10 + Ubuntu 20.04
+    # Ubuntu 20.04 provides only gcc 10.3 and not 10.4 or 10.5
+    # this combination does not work: https://github.com/alpaka-group/alpaka/issues/1297
+    if (
+        row_check_name(row, DEVICE_COMPILER, "==", NVCC)
+        and row_check_version(row, DEVICE_COMPILER, "==", "11.3")
+        and row_check_name(row, HOST_COMPILER, "==", GCC)
+        and row_check_version(row, HOST_COMPILER, "==", "10")
+        and row_check_version(row, UBUNTU, "==", "20.04")
+    ):
+        return False
+
     return True
```

### Comparing `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/globals.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.3.3/src/alpaka_job_coverage/util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.3.3/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.2
+Version: 1.3.3
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.3.2/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.3.3/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,8 +15,10 @@
 src/alpaka_job_coverage.egg-info/PKG-INFO
 src/alpaka_job_coverage.egg-info/SOURCES.txt
 src/alpaka_job_coverage.egg-info/dependency_links.txt
 src/alpaka_job_coverage.egg-info/requires.txt
 src/alpaka_job_coverage.egg-info/top_level.txt
 tests/test_compiler_names.py
 tests/test_cuda_sdk.py
+tests/test_hipcc.py
+tests/test_single_rules.py
 tests/test_util.py
```

### Comparing `alpaka-job-coverage-1.3.2/tests/test_compiler_names.py` & `alpaka-job-coverage-1.3.3/tests/test_compiler_names.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/tests/test_cuda_sdk.py` & `alpaka-job-coverage-1.3.3/tests/test_cuda_sdk.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.2/tests/test_util.py` & `alpaka-job-coverage-1.3.3/tests/test_util.py`

 * *Files identical despite different names*

