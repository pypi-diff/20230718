# Comparing `tmp/prophecy-libs-1.5.9.dev1.tar.gz` & `tmp/prophecy-libs-1.5.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.5.9.dev1.tar", last modified: Fri Jul 14 08:43:28 2023, max compression
+gzip compressed data, was "prophecy-libs-1.5.9.dev2.tar", last modified: Tue Jul 18 10:07:24 2023, max compression
```

## Comparing `prophecy-libs-1.5.9.dev1.tar` & `prophecy-libs-1.5.9.dev2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.496794 prophecy-libs-1.5.9.dev1/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      318 2023-07-14 08:43:28.496794 prophecy-libs-1.5.9.dev1/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.492794 prophecy-libs-1.5.9.dev1/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.492794 prophecy-libs-1.5.9.dev1/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.5.9.dev1/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.492794 prophecy-libs-1.5.9.dev1/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev1/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.492794 prophecy-libs-1.5.9.dev1/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.492794 prophecy-libs-1.5.9.dev1/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.496794 prophecy-libs-1.5.9.dev1/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.9.dev1/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.9.dev1/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.496794 prophecy-libs-1.5.9.dev1/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev1/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.9.dev1/prophecy/udfs/scala_udf_wrapper.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.496794 prophecy-libs-1.5.9.dev1/prophecy/utils/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       46 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev1/prophecy/utils/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.496794 prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      143 2023-07-14 08:43:27.000000 prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/abi_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    22828 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/abi_core_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1591 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/abi_fcn_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6521 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/dataframe_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      399 2023-07-14 08:43:27.000000 prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/dml_schema.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/fixed_file_schema.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    18113 2023-07-12 14:13:52.000000 prophecy-libs-1.5.9.dev1/prophecy/utils/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-14 08:43:28.496794 prophecy-libs-1.5.9.dev1/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      318 2023-07-14 08:43:28.000000 prophecy-libs-1.5.9.dev1/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1101 2023-07-14 08:43:28.000000 prophecy-libs-1.5.9.dev1/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-07-14 08:43:28.000000 prophecy-libs-1.5.9.dev1/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.9.dev1/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-07-14 08:43:28.000000 prophecy-libs-1.5.9.dev1/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-07-14 08:43:28.000000 prophecy-libs-1.5.9.dev1/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-07-14 08:43:28.496794 prophecy-libs-1.5.9.dev1/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      479 2023-07-14 08:43:27.000000 prophecy-libs-1.5.9.dev1/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.980995 prophecy-libs-1.5.9.dev2/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      318 2023-07-18 10:07:24.980995 prophecy-libs-1.5.9.dev2/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.968994 prophecy-libs-1.5.9.dev2/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.968994 prophecy-libs-1.5.9.dev2/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.5.9.dev2/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.968994 prophecy-libs-1.5.9.dev2/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev2/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.968994 prophecy-libs-1.5.9.dev2/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.972995 prophecy-libs-1.5.9.dev2/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.972995 prophecy-libs-1.5.9.dev2/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.9.dev2/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.9.dev2/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.976995 prophecy-libs-1.5.9.dev2/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev2/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.9.dev2/prophecy/udfs/scala_udf_wrapper.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.976995 prophecy-libs-1.5.9.dev2/prophecy/utils/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       46 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev2/prophecy/utils/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.980995 prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      143 2023-07-18 10:07:22.000000 prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/abi_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    22828 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/abi_core_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1591 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/abi_fcn_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6521 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/dataframe_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      286 2023-07-18 10:07:22.000000 prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/dml_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/fixed_file_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    18113 2023-07-12 14:13:52.000000 prophecy-libs-1.5.9.dev2/prophecy/utils/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-18 10:07:24.980995 prophecy-libs-1.5.9.dev2/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      318 2023-07-18 10:07:24.000000 prophecy-libs-1.5.9.dev2/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1101 2023-07-18 10:07:24.000000 prophecy-libs-1.5.9.dev2/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-07-18 10:07:24.000000 prophecy-libs-1.5.9.dev2/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.9.dev2/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-07-18 10:07:24.000000 prophecy-libs-1.5.9.dev2/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-07-18 10:07:24.000000 prophecy-libs-1.5.9.dev2/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-07-18 10:07:24.980995 prophecy-libs-1.5.9.dev2/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      479 2023-07-18 10:07:22.000000 prophecy-libs-1.5.9.dev2/setup.py
```

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/config/config_base.py` & `prophecy-libs-1.5.9.dev2/prophecy/config/config_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/config/utils.py` & `prophecy-libs-1.5.9.dev2/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/libs/utils.py` & `prophecy-libs-1.5.9.dev2/prophecy/libs/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.5.9.dev2/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/random_data_creator.py` & `prophecy-libs-1.5.9.dev2/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.5.9.dev2/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/test/base_test_case.py` & `prophecy-libs-1.5.9.dev2/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/test/utils.py` & `prophecy-libs-1.5.9.dev2/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.5.9.dev2/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.5.9.dev2/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/abi_base.py` & `prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/abi_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/abi_core_fcns.py` & `prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/abi_core_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/abi_fcn_wrapper.py` & `prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/abi_fcn_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/dataframe_fcns.py` & `prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/dataframe_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/utils/transpiler/fixed_file_schema.py` & `prophecy-libs-1.5.9.dev2/prophecy/utils/transpiler/fixed_file_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy/utils/utils.py` & `prophecy-libs-1.5.9.dev2/prophecy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.9.dev1/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.5.9.dev2/prophecy_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

