# Comparing `tmp/storey-1.4.4.tar.gz` & `tmp/storey-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-zb0_k6rx/storey-1.4.4.tar", last modified: Mon Jul 10 06:23:46 2023, max compression
+gzip compressed data, was "/home/runner/work/storey/storey/dist/.tmp-y_domb5g/storey-1.5.0.tar", last modified: Tue Jul 18 09:46:40 2023, max compression
```

## Comparing `storey-1.4.4.tar` & `storey-1.5.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 06:15:48.000000 storey-1.4.4/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 06:15:48.000000 storey-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-10 06:15:48.000000 storey-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-10 06:23:46.000000 storey-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-10 06:15:48.000000 storey-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-10 06:15:48.000000 storey-1.4.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-10 06:15:48.000000 storey-1.4.4/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-10 06:15:48.000000 storey-1.4.4/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-10 06:15:48.000000 storey-1.4.4/integration/integration_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_aggregation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_azure_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_filesystems_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_flow_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_kafka_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_redis_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-07-10 06:15:48.000000 storey-1.4.4/integration/test_s3_filesystem_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-10 06:15:48.000000 storey-1.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 06:23:46.000000 storey-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-10 06:15:48.000000 storey-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/storey/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-10 06:23:40.000000 storey-1.4.4/storey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-10 06:15:48.000000 storey-1.4.4/storey/aggregation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-07-10 06:15:48.000000 storey-1.4.4/storey/aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-10 06:15:48.000000 storey-1.4.4/storey/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-07-10 06:15:48.000000 storey-1.4.4/storey/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-07-10 06:15:48.000000 storey-1.4.4/storey/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    50622 2023-07-10 06:15:48.000000 storey-1.4.4/storey/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-10 06:15:48.000000 storey-1.4.4/storey/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    27610 2023-07-10 06:15:48.000000 storey-1.4.4/storey/redis_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    37793 2023-07-10 06:15:48.000000 storey-1.4.4/storey/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-10 06:15:48.000000 storey-1.4.4/storey/sql_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/storey/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-10 06:15:48.000000 storey-1.4.4/storey/steps/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    79910 2023-07-10 06:15:48.000000 storey-1.4.4/storey/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    51037 2023-07-10 06:15:48.000000 storey-1.4.4/storey/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/storey/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-10 06:15:48.000000 storey-1.4.4/storey/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-10 06:15:48.000000 storey-1.4.4/storey/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-10 06:15:48.000000 storey-1.4.4/storey/windowed_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 06:23:46.000000 storey-1.4.4/storey.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 06:23:46.000000 storey-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-10 06:15:48.000000 storey-1.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_aggregate_by_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_aggregate_store.py
--rw-r--r--   0 runner    (1001) docker     (123)   125240 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_v3io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-10 06:15:48.000000 storey-1.4.4/tests/test_windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:40.000000 storey-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 09:43:39.000000 storey-1.5.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 09:43:39.000000 storey-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-18 09:43:39.000000 storey-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-18 09:46:40.000000 storey-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-18 09:43:39.000000 storey-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-18 09:43:39.000000 storey-1.5.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:40.000000 storey-1.5.0/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-18 09:43:39.000000 storey-1.5.0/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-18 09:43:39.000000 storey-1.5.0/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-18 09:43:39.000000 storey-1.5.0/integration/integration_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170272 2023-07-18 09:43:39.000000 storey-1.5.0/integration/test_aggregation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-07-18 09:43:39.000000 storey-1.5.0/integration/test_azure_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21737 2023-07-18 09:43:39.000000 storey-1.5.0/integration/test_filesystems_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42755 2023-07-18 09:43:39.000000 storey-1.5.0/integration/test_flow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-18 09:43:39.000000 storey-1.5.0/integration/test_kafka_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-18 09:43:39.000000 storey-1.5.0/integration/test_redis_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-07-18 09:43:39.000000 storey-1.5.0/integration/test_s3_filesystem_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-18 09:43:39.000000 storey-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 09:46:40.000000 storey-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-18 09:43:39.000000 storey-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:40.000000 storey-1.5.0/storey/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-18 09:46:35.000000 storey-1.5.0/storey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-18 09:43:39.000000 storey-1.5.0/storey/aggregation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-07-18 09:43:39.000000 storey-1.5.0/storey/aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-18 09:43:39.000000 storey-1.5.0/storey/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-07-18 09:43:39.000000 storey-1.5.0/storey/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-07-18 09:43:39.000000 storey-1.5.0/storey/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51518 2023-07-18 09:43:39.000000 storey-1.5.0/storey/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-18 09:43:39.000000 storey-1.5.0/storey/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27610 2023-07-18 09:43:39.000000 storey-1.5.0/storey/redis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43777 2023-07-18 09:43:39.000000 storey-1.5.0/storey/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-18 09:43:39.000000 storey-1.5.0/storey/sql_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:40.000000 storey-1.5.0/storey/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-18 09:43:39.000000 storey-1.5.0/storey/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-18 09:43:39.000000 storey-1.5.0/storey/steps/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-18 09:43:39.000000 storey-1.5.0/storey/steps/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-18 09:43:39.000000 storey-1.5.0/storey/steps/foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-18 09:43:39.000000 storey-1.5.0/storey/steps/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-18 09:43:39.000000 storey-1.5.0/storey/steps/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80029 2023-07-18 09:43:39.000000 storey-1.5.0/storey/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52048 2023-07-18 09:43:39.000000 storey-1.5.0/storey/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:40.000000 storey-1.5.0/storey/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-18 09:43:39.000000 storey-1.5.0/storey/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-18 09:43:39.000000 storey-1.5.0/storey/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-18 09:43:39.000000 storey-1.5.0/storey/windowed_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:40.000000 storey-1.5.0/storey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-18 09:46:40.000000 storey-1.5.0/storey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-18 09:46:40.000000 storey-1.5.0/storey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:46:40.000000 storey-1.5.0/storey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-18 09:46:40.000000 storey-1.5.0/storey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 09:46:40.000000 storey-1.5.0/storey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:40.000000 storey-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-18 09:43:39.000000 storey-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-07-18 09:43:39.000000 storey-1.5.0/tests/test_aggregate_by_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-18 09:43:39.000000 storey-1.5.0/tests/test_aggregate_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131843 2023-07-18 09:43:39.000000 storey-1.5.0/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-07-18 09:43:39.000000 storey-1.5.0/tests/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-18 09:43:39.000000 storey-1.5.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-18 09:43:39.000000 storey-1.5.0/tests/test_v3io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-18 09:43:39.000000 storey-1.5.0/tests/test_windowed_store.py
```

### Comparing `storey-1.4.4/LICENSE` & `storey-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/PKG-INFO` & `storey-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.4.4
+Version: 1.5.0
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.4.4/README.md` & `storey-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/__init__.py` & `storey-1.5.0/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/conftest.py` & `storey-1.5.0/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/integration_test_utils.py` & `storey-1.5.0/integration/integration_test_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/test_aggregation_integration.py` & `storey-1.5.0/integration/test_aggregation_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/test_azure_filesystem_integration.py` & `storey-1.5.0/integration/test_azure_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/test_filesystems_integration.py` & `storey-1.5.0/integration/test_filesystems_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/test_flow_integration.py` & `storey-1.5.0/integration/test_flow_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/test_kafka_integration.py` & `storey-1.5.0/integration/test_kafka_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/test_redis_specific.py` & `storey-1.5.0/integration/test_redis_specific.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/integration/test_s3_filesystem_integration.py` & `storey-1.5.0/integration/test_s3_filesystem_integration.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/setup.py` & `storey-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/__init__.py` & `storey-1.5.0/storey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.4.4"
+__version__ = "1.5.0"
 
 # Importing supported filesystems explicitly so that they will get registered as an fsspec filesystem
 import v3iofs  # noqa: F401
 
 from .aggregations import AggregateByKey, QueryByKey  # noqa: F401
 from .dataframe import ReduceToDataFrame, ToDataFrame  # noqa: F401
 from .drivers import Driver, NoopDriver, V3ioDriver  # noqa: F401
```

### Comparing `storey-1.4.4/storey/aggregation_utils.py` & `storey-1.5.0/storey/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/aggregations.py` & `storey-1.5.0/storey/aggregations.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             if self._key_extractor:
                 key = self._key_extractor(element)
 
             event_timestamp = self._get_timestamp(event)
 
             safe_key = stringify_key(key)
             await self._table._lazy_load_key_with_aggregates(safe_key, event_timestamp)
-            await self._table._aggregate(safe_key, element, event_timestamp)
+            await self._table._aggregate(safe_key, event, element, event_timestamp)
 
             if isinstance(self._emit_policy, EmitEveryEvent):
                 await self._emit_event(key, event)
             elif isinstance(self._emit_policy, EmitAfterMaxEvent):
                 if safe_key in self._events_in_batch:
                     self._events_in_batch[safe_key]["counter"] += 1
                 else:
```

### Comparing `storey-1.4.4/storey/dataframe.py` & `storey-1.5.0/storey/dataframe.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/drivers.py` & `storey-1.5.0/storey/drivers.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/dtypes.py` & `storey-1.5.0/storey/dtypes.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/flow.py` & `storey-1.5.0/storey/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,18 +265,24 @@
                     )
             return self._termination_result
         # If there is more than one outlet, allow concurrent execution.
         tasks = []
         if len(self._outlets) > 1:
             awaitable_result = event._awaitable_result
             event._awaitable_result = None
+            original_events = getattr(event, "_original_events", None)
+            # Temporarily delete self-reference to avoid deepcopy getting stuck in an infinite loop
+            event._original_events = None
             for i in range(1, len(self._outlets)):
                 event_copy = copy.deepcopy(event)
                 event_copy._awaitable_result = awaitable_result
+                event_copy._original_events = original_events
                 tasks.append(asyncio.get_running_loop().create_task(self._outlets[i]._do_and_recover(event_copy)))
+            # Set self-reference back after deepcopy
+            event._original_events = original_events
             event._awaitable_result = awaitable_result
         if self.verbose and self.logger:
             step_name = self.name
             event_string = self._event_string(event)
             self.logger.debug(f"{step_name} -> {self._outlets[0].name} | {event_string}")
         await self._outlets[0]._do_and_recover(event)  # Optimization - avoids creating a task for the first outlet.
         for i, task in enumerate(tasks, start=1):
@@ -546,14 +552,15 @@
             if isinstance(self._state, Table):
                 key_data = await self._state._get_or_load_static_attributes_by_key(safe_key)
             else:
                 key_data = self._state[event.key]
             res, new_state = self._fn(element, key_data)
             async with self._state._get_lock(safe_key):
                 self._state._update_static_attrs(safe_key, new_state)
+                self._state._pending_events.append(event)
             self._state._init_flush_task()
         else:
             res, self._state = self._fn(element, self._state)
         if self._is_async:
             res = await res
         return res
 
@@ -972,14 +979,16 @@
             raise ValueError("flush_after_seconds cannot be negative")
 
         self._extract_key: Optional[Callable[[Event], str]] = self._create_key_extractor(key_field)
 
     def _init(self):
         super()._init()
         self._batch: Dict[Optional[str], List[Any]] = defaultdict(list)
+        # Keep the original events that make up each batch
+        self._batch_events: Dict[Optional[str], List[Any]] = defaultdict(list)
         self._batch_first_event_time: Dict[Optional[str], datetime.datetime] = {}
         self._batch_last_event_time: Dict[Optional[str], datetime.datetime] = {}
         self._batch_start_time: Dict[Optional[str], float] = {}
         self._timeout_task: Optional[Task] = None
 
     @staticmethod
     def _create_key_extractor(key_field) -> Callable:
@@ -991,15 +1000,15 @@
             if key_field == "$key":
                 return lambda event: event.key
             else:
                 return lambda event: event.body[key_field]
         else:
             raise ValueError(f"Unsupported key_field type {type(key_field)}")
 
-    async def _emit(self, batch, batch_key, batch_time, last_event_time=None):
+    async def _emit(self, batch, batch_key, batch_time, batch_events, last_event_time=None):
         raise NotImplementedError
 
     async def _terminate(self):
         pass
 
     async def _do(self, event):
         if event is _termination_obj:
@@ -1021,14 +1030,15 @@
         elif self._batch_last_event_time[key] < event_time:
             self._batch_last_event_time[key] = event_time
 
         if self._flush_after_seconds is not None and self._timeout_task is None:
             self._timeout_task = asyncio.get_running_loop().create_task(self._sleep_and_emit())
 
         self._batch[key].append(self._event_to_batch_entry(event))
+        self._batch_events[key].append(event)
 
         if len(self._batch[key]) == self._max_events:
             await self._emit_batch(key)
 
         if self._do_downstream_per_event:
             await self._do_downstream(event)
 
@@ -1053,15 +1063,16 @@
     async def _emit_batch(self, batch_key: Optional[str] = None):
         batch_to_emit = self._batch.pop(batch_key, None)
         if batch_to_emit is None:
             return
         batch_time = self._batch_first_event_time.pop(batch_key)
         last_event_time = self._batch_last_event_time.pop(batch_key)
         del self._batch_start_time[batch_key]
-        await self._emit(batch_to_emit, batch_key, batch_time, last_event_time)
+        await self._emit(batch_to_emit, batch_key, batch_time, self._batch_events[batch_key], last_event_time)
+        del self._batch_events[batch_key]
 
     async def _emit_all(self):
         for key in list(self._batch.keys()):
             await self._emit_batch(key)
 
 
 class Batch(_Batching):
@@ -1077,16 +1088,19 @@
         Set a '$key' to group events by the Event.key property.
         set a 'str' key to group events by Event.body[str].
         set a Callable[Any, Any] to group events by a a custom key extractor.
     """
 
     _do_downstream_per_event = False
 
-    async def _emit(self, batch, batch_key, batch_time, last_event_time=None):
+    async def _emit(self, batch, batch_key, batch_time, batch_events, last_event_time=None):
         event = Event(batch)
+        if not self._full_event:
+            # Preserve reference to the original events to avoid early commit of offsets
+            event._original_events = batch_events
         return await self._do_downstream(event)
 
 
 class JoinWithV3IOTable(_ConcurrentJobExecution):
     """Joins each event with a V3IO table. Used for event augmentation.
 
     :param storage: Database driver.
```

### Comparing `storey-1.4.4/storey/queue.py` & `storey-1.5.0/storey/queue.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/redis_driver.py` & `storey-1.5.0/storey/redis_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/sources.py` & `storey-1.5.0/storey/sources.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,25 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import asyncio
 import copy
+import gc
 import queue
 import threading
 import uuid
 import warnings
+import weakref
+from collections import defaultdict
 from datetime import datetime, timezone
 from typing import Callable, Coroutine, Iterable, List, Optional, Union
 
 import pandas
 import pandas as pd
 import pyarrow
 import pytz
+from nuclio_sdk import QualifiedOffset
 
 from .dtypes import Event, _termination_obj
 from .flow import Complete, Flow
 from .utils import find_filters, find_partitions, url_to_file_system
 
 
 class AwaitableResult:
@@ -195,14 +199,15 @@
             )
 
         event = self._build_event(element, key)
         awaitable_result = None
         if self._return_awaitable_result:
             awaitable_result = AwaitableResult(expected_number_of_results=expected_number_of_results or 1)
         event._awaitable_result = awaitable_result
+        event._original_events = [event]
         self._emit_fn(event)
         return awaitable_result
 
     def terminate(self):
         """Terminates the associated flow."""
         self._emit_fn(_termination_obj)
 
@@ -221,62 +226,109 @@
         self._await_termination_fn = await_termination_fn
 
     def await_termination(self):
         """ "waits for the flow to terminate and returns the result"""
         return self._await_termination_fn()
 
 
+class _EventOffset:
+    def __init__(self, event):
+        self.event_weakref = weakref.ref(event)
+        self.offset = event.offset
+
+    def is_ready_to_commit(self):
+        return self.event_weakref() is None
+
+    def __repr__(self):
+        return f"_EventOffset({self.offset})"
+
+
 class SyncEmitSource(Flow):
     """Synchronous entry point into a flow. Produces a FlowController when run, for use from inside a synchronous
     context. See AsyncEmitSource for use from inside an async context.
 
     :param buffer_size: size of the incoming event buffer. Defaults to 8.
     :param key_field: Field to extract and use as the key. Optional.
+    :param max_events_before_commit: Maximum number of events to be processed before committing offsets.
+    :param explicit_ack: Whether to explicitly commit offsets. Defaults to False.
     :param name: Name of this step, as it should appear in logs. Defaults to class name (SyncEmitSource).
     :type name: string
 
     for additional params, see documentation of  :class:`storey.flow.Flow`
     """
 
     _legal_first_step = True
 
     def __init__(
         self,
         buffer_size: Optional[int] = None,
         key_field: Union[list, str, int, None] = None,
+        max_events_before_commit=None,
+        explicit_ack=False,
         **kwargs,
     ):
         if buffer_size is None:
             buffer_size = 8
         else:
             kwargs["buffer_size"] = buffer_size
         if key_field is not None:
             kwargs["key_field"] = key_field
         super().__init__(**kwargs)
         if buffer_size <= 0:
             raise ValueError("Buffer size must be positive")
         self._q = queue.Queue(buffer_size)
         self._key_field = key_field
+        self._max_events_before_commit = max_events_before_commit or 1000
+        self._explicit_ack = explicit_ack
         self._termination_q = queue.Queue(1)
         self._ex = None
         self._closeables = []
 
     def _init(self):
         super()._init()
         self._is_terminated = False
+        self._outstanding_offsets = defaultdict(list)
 
     async def _run_loop(self):
         loop = asyncio.get_running_loop()
-        self._termination_future = asyncio.get_running_loop().create_future()
-
+        self._termination_future = loop.create_future()
+        committer = None
+        num_events_handled_without_commit = 0
+        if self._explicit_ack and hasattr(self.context, "platform") and hasattr(self.context.platform, "explicit_ack"):
+            committer = self.context.platform.explicit_ack
         while True:
-            event = await loop.run_in_executor(None, self._q.get)
+            event = None
+            if (
+                num_events_handled_without_commit > 0
+                and self._q.empty()
+                or num_events_handled_without_commit >= self._max_events_before_commit
+            ):
+                num_events_handled_without_commit = 0
+                can_block = await _commit_handled_events(self._outstanding_offsets, committer)
+                # In case we can't block because there are outstanding events
+                while not can_block:
+                    if self._q.qsize() > 0:
+                        event = self._q.get_nowait()
+                        if event:
+                            break
+                    await asyncio.sleep(1)
+                    can_block = await _commit_handled_events(self._outstanding_offsets, committer)
+            if not event:
+                event = await loop.run_in_executor(None, self._q.get)
+            if committer and hasattr(event, "path") and hasattr(event, "shard_id") and hasattr(event, "offset"):
+                qualified_shard = (event.path, event.shard_id)
+                offsets = self._outstanding_offsets[qualified_shard]
+                offsets.append(_EventOffset(event))
+                num_events_handled_without_commit += 1
             try:
                 termination_result = await self._do_downstream(event)
                 if event is _termination_obj:
+                    # We can commit all at this point because termination of
+                    # all downstream steps completed successfully.
+                    await _commit_handled_events(self._outstanding_offsets, committer, commit_all=True)
                     self._termination_future.set_result(termination_result)
             except BaseException as ex:
                 if event is not _termination_obj and event._awaitable_result:
                     event._awaitable_result._set_error(ex)
                 self._ex = ex
                 if not self._q.empty():
                     event = self._q.get()
@@ -426,14 +478,15 @@
             )
 
         event = self._build_event(element, key)
         awaitable = None
         if self._await_result:
             awaitable = AsyncAwaitableResult()
         event._awaitable_result = awaitable
+        event._original_events = [event]
         await self._emit_fn(event)
         if self._await_result:
             result = await awaitable.await_result()
             if isinstance(result, BaseException):
                 raise result
             return result
 
@@ -445,56 +498,120 @@
         """
         Awaits the termination of the flow. To be called after terminate. Returns the termination result of the
         flow (if any).
         """
         return await self._loop_task
 
 
+async def _commit_handled_events(outstanding_offsets_by_qualified_shard, committer, commit_all=False):
+    all_offsets_handled = True
+    for qualified_shard, offsets in outstanding_offsets_by_qualified_shard.items():
+        if commit_all and offsets:
+            last_handled_offset = offsets[-1].offset
+            num_to_clear = len(offsets)
+        else:
+            num_to_clear = 0
+            last_handled_offset = None
+            gc.collect()
+            # go over offsets in the qualified shard by arrival order until we reach an unhandled offset
+            for offset in offsets:
+                if not offset.is_ready_to_commit():
+                    all_offsets_handled = False
+                    break
+                last_handled_offset = offset.offset
+                num_to_clear += 1
+        if last_handled_offset is not None:
+            path, shard_id = qualified_shard
+            await committer(QualifiedOffset(path, shard_id, last_handled_offset))
+            outstanding_offsets_by_qualified_shard[qualified_shard] = offsets[num_to_clear:]
+    return all_offsets_handled
+
+
 class AsyncEmitSource(Flow):
     """
     Asynchronous entry point into a flow. Produces an AsyncFlowController when run, for use from inside an async def.
     See SyncEmitSource for use from inside a synchronous context.
 
     :param buffer_size: size of the incoming event buffer. Defaults to 8.
+    :param key_field: Field to extract and use as the key. Optional.
+    :param max_events_before_commit: Maximum number of events to be processed before committing offsets.
+    :param explicit_ack: Whether to explicitly commit offsets. Defaults to False.
     :param name: Name of this step, as it should appear in logs. Defaults to class name (AsyncEmitSource).
     :type name: string
 
     for additional params, see documentation of  :class:`~storey.flow.Flow`
     """
 
     _legal_first_step = True
 
     def __init__(
         self,
         buffer_size: int = None,
         key_field: Union[list, str, None] = None,
+        max_events_before_commit=None,
+        explicit_ack=False,
         **kwargs,
     ):
         super().__init__(**kwargs)
         if buffer_size is None:
             buffer_size = 8
         elif buffer_size <= 0:
             raise ValueError("Buffer size must be positive")
         else:
             kwargs["buffer_size"] = buffer_size
         self._q = asyncio.Queue(buffer_size)
         self._key_field = key_field
+        self._max_events_before_commit = max_events_before_commit or 1000
+        self._explicit_ack = explicit_ack
         self._ex = None
         self._closeables = []
 
     def _init(self):
         super()._init()
         self._is_terminated = False
+        self._outstanding_offsets = defaultdict(list)
 
     async def _run_loop(self):
+        committer = None
+        num_events_handled_without_commit = 0
+        if self._explicit_ack and hasattr(self.context, "platform") and hasattr(self.context.platform, "explicit_ack"):
+            committer = self.context.platform.explicit_ack
         while True:
-            event = await self._q.get()
+            event = None
+            if (
+                num_events_handled_without_commit > 0
+                and self._q.empty()
+                or num_events_handled_without_commit >= self._max_events_before_commit
+            ):
+                num_events_handled_without_commit = 0
+                can_block = await _commit_handled_events(self._outstanding_offsets, committer)
+                # In case we can't block because there are outstanding events
+                while not can_block:
+                    # Yield to allow the queue to fill if possible
+                    await asyncio.sleep(0)
+                    if not self._q.empty():
+                        event = self._q.get_nowait()
+                    if event:
+                        break
+                    # Wait to avoid busy-wait
+                    await asyncio.sleep(0.2)
+                    can_block = await _commit_handled_events(self._outstanding_offsets, committer)
+            if not event:
+                event = await self._q.get()
+            if committer and hasattr(event, "path") and hasattr(event, "shard_id") and hasattr(event, "offset"):
+                qualified_shard = (event.path, event.shard_id)
+                offsets = self._outstanding_offsets[qualified_shard]
+                offsets.append(_EventOffset(event))
+                num_events_handled_without_commit += 1
             try:
                 termination_result = await self._do_downstream(event)
                 if event is _termination_obj:
+                    # We can commit all at this point because termination of
+                    # all downstream steps completed successfully.
+                    await _commit_handled_events(self._outstanding_offsets, committer, commit_all=True)
                     return termination_result
             except BaseException as ex:
                 self._ex = ex
                 if event is not _termination_obj and event._awaitable_result:
                     awaitable = event._awaitable_result._set_error(ex)
                     if awaitable:
                         await awaitable
```

### Comparing `storey-1.4.4/storey/sql_driver.py` & `storey-1.5.0/storey/sql_driver.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/steps/__init__.py` & `storey-1.5.0/storey/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/steps/assertion.py` & `storey-1.5.0/storey/steps/assertion.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/steps/flatten.py` & `storey-1.5.0/storey/steps/flatten.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/steps/foreach.py` & `storey-1.5.0/storey/steps/foreach.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/steps/partition.py` & `storey-1.5.0/storey/steps/partition.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/steps/sample.py` & `storey-1.5.0/storey/steps/sample.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/table.py` & `storey-1.5.0/storey/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         self._max_updates_in_flight = max_updates_in_flight
         self._pending_by_key = {}
         self._flush_interval_secs = flush_interval_secs
         self._flush_task = None
         self._terminated = False
         self._flush_exception = None
         self._changed_keys = set()
+        self._pending_events = []
         self.fixed_window_type = None
 
     def __str__(self):
         return f"{self._container}/{self._table_path}"
 
     def supports_aggregations(self):
         return self._storage.supports_aggregations()
@@ -176,23 +177,24 @@
     def _init_flush_task(self):
         if not self._flush_task and self._flush_interval_secs:
             self._flush_task = asyncio.get_running_loop().create_task(self._flush_worker())
 
     async def close(self):
         await self._storage.close()
 
-    async def _aggregate(self, key, data, timestamp):
+    async def _aggregate(self, key, event, data, timestamp):
         if self._flush_exception is not None:
             raise self._flush_exception
         if not self._schema:
             await self._load_and_update_schema()
         async with self._get_lock(key):
             cache_item = self._get_aggregations_attrs(key)
             await cache_item.aggregate(data, timestamp)
             self._changed_keys.add(key)
+        self._pending_events.append(event)
 
     async def _get_features(self, key, timestamp):
         if self._flush_exception is not None:
             raise self._flush_exception
         if not self._schema:
             await self._load_and_update_schema()
 
@@ -386,14 +388,16 @@
                         await self._persist(_PersistJob(key, None, None))
                         self._changed_keys.discard(key)
 
         except BaseException as ex:
             if not isinstance(ex, asyncio.CancelledError):
                 self._flush_exception = ex
 
+        self._pending_events = []
+
     async def _persist_worker(self):
         task = None
         received_job_count = 0
         self_sent_jobs = {}
         try:
             while True:
                 jobs = self_sent_jobs.pop(received_job_count, None)
```

### Comparing `storey-1.4.4/storey/targets.py` & `storey-1.5.0/storey/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -470,15 +470,15 @@
             raise TypeError(f"CSV writer does not support event body of type {type(event.body)}.")
         return writer_entry
 
     async def _terminate(self):
         asyncio.get_running_loop().run_in_executor(None, lambda: self._data_buffer.put(_termination_obj))
         await self._blocking_io_loop_future
 
-    async def _emit(self, batch, batch_key, batch_time, last_event_time=None):
+    async def _emit(self, batch, batch_key, batch_time, batch_events, last_event_time=None):
         if not self._blocking_io_loop_future:
             self._blocking_io_loop_future = asyncio.get_running_loop().run_in_executor(None, self._blocking_io_loop)
 
         if self._blocking_io_loop_failed:
             await self._blocking_io_loop_future
         else:
             await asyncio.get_running_loop().run_in_executor(None, lambda: self._data_buffer.put(batch))
@@ -594,15 +594,15 @@
     def _init(self):
         _Batching._init(self)
         _Writer._init(self)
 
     def _event_to_batch_entry(self, event):
         return self._event_to_writer_entry(event)
 
-    async def _emit(self, batch, batch_key, batch_time, last_event_time=None):
+    async def _emit(self, batch, batch_key, batch_time, batch_events, last_event_time=None):
         df_columns = []
         if self._non_partition_columns:
             if self._index_cols:
                 df_columns.extend(self._index_cols)
             df_columns.extend(self._non_partition_columns)
         if not df_columns:
             df_columns = None
@@ -745,15 +745,15 @@
     def _init(self):
         _Batching._init(self)
         _Writer._init(self)
 
     def _event_to_batch_entry(self, event):
         return self._event_to_writer_entry(event)
 
-    async def _emit(self, batch, batch_key, batch_time, last_event_time=None):
+    async def _emit(self, batch, batch_key, batch_time, batch_events, last_event_time=None):
         df_columns = []
         if self._index_cols:
             df_columns.extend(self._index_cols)
         df_columns.extend(self._columns)
         df = pd.DataFrame(batch, columns=df_columns)
         df[self._time_col] = pd.to_datetime(df[self._time_col], format=self._time_format)
         df.set_index(keys=self._index_cols, inplace=True)
@@ -858,43 +858,55 @@
         for record in records:
             if isinstance(record, dict):
                 record = json.dumps(record, default=str).encode("utf-8")
             record_list_for_json.append({"shard_id": shard_id, "data": record})
 
         return record_list_for_json
 
-    def _send_batch(self, buffers, in_flight_reqs, shard_id):
+    def _send_batch(self, buffers, in_flight_reqs, buffer_events, in_flight_events, shard_id):
         buffer = buffers[shard_id]
+        if not buffer:
+            return
         buffers[shard_id] = []
+        in_flight_events[shard_id] = buffer_events[shard_id]
+        buffer_events[shard_id] = []
         request_body = self._build_request_put_records(shard_id, buffer)
         request = self._storage._put_records(self._container, self._stream_path, request_body)
         in_flight_reqs[shard_id] = asyncio.get_running_loop().create_task(request)
 
     async def _worker(self):
         try:
             buffers = []
             in_flight_reqs = []
+
+            # We keep the original events before sending and then while in flight, to avoid them being marked as
+            # completed and ready to commit at the source
+            buffer_events = []
+            in_flight_events = []
+
             for _ in range(self._shards):
                 buffers.append([])
+                buffer_events.append([])
                 in_flight_reqs.append(None)
+                in_flight_events.append(None)
             while True:
                 try:
                     for shard_id in range(self._shards):
                         if self._q.empty():
                             req = in_flight_reqs[shard_id]
                             in_flight_reqs[shard_id] = None
                             await self._handle_response(req)
-                            self._send_batch(buffers, in_flight_reqs, shard_id)
+                            in_flight_events[shard_id] = None
+                            self._send_batch(buffers, in_flight_reqs, buffer_events, in_flight_events, shard_id)
                     event = await self._q.get()
                     if event is _termination_obj:  # handle outstanding batches and in flight requests on termination
                         for req in in_flight_reqs:
                             await self._handle_response(req)
                         for shard_id in range(self._shards):
-                            if buffers[shard_id]:
-                                self._send_batch(buffers, in_flight_reqs, shard_id)
+                            self._send_batch(buffers, in_flight_reqs, buffer_events, in_flight_events, shard_id)
                         for req in in_flight_reqs:
                             await self._handle_response(req)
                         break
                     sharding_func_result = self._sharding_func(event)
                     if isinstance(sharding_func_result, int):
                         shard_id = sharding_func_result
                     else:
@@ -902,20 +914,22 @@
                         h.update(sharding_func_result)
                         shard_id = h.intdigest()
                     shard_id %= self._shards
                     record = self._event_to_writer_entry(event)
                     if self._full_event:
                         record = Event.wrap_for_serialization(event, record)
                     buffers[shard_id].append(record)
+                    buffer_events[shard_id].append(event)
                     if len(buffers[shard_id]) >= self._batch_size:
                         if in_flight_reqs[shard_id]:
                             req = in_flight_reqs[shard_id]
                             in_flight_reqs[shard_id] = None
                             await self._handle_response(req)
-                        self._send_batch(buffers, in_flight_reqs, shard_id)
+                            in_flight_events[shard_id] = None
+                        self._send_batch(buffers, in_flight_reqs, buffer_events, in_flight_events, shard_id)
                 except BaseException as ex:
                     ex._raised_by_storey_step = self
                     if self.context and hasattr(self.context, "push_error"):
                         message = traceback.format_exc()
                         if self.logger:
                             self.logger.error(f"Pushing error to error stream: {ex}\n{message}")
                         self.context.push_error(event, f"{ex}\n{message}", source=self.name)
@@ -984,15 +998,15 @@
         appended to the provided list. If header is True and columns is not provided, infer_columns_from_data=True is
         implied. Optional. Default to False if columns is provided, True otherwise.
     :param full_event: Enable metadata wrapper for serialized event. Defaults to False.
     """
 
     def __init__(
         self,
-        bootstrap_servers: str,
+        bootstrap_servers: Union[str, List[str]],
         topic: str,
         producer_options: Optional[dict] = None,
         sharding_func: Union[None, int, str, Callable[[Event], Any]] = None,
         columns: Optional[List[str]] = None,
         infer_columns_from_data: Optional[bool] = None,
         full_event: Optional[bool] = None,
         **kwargs,
@@ -1039,14 +1053,15 @@
             self._producer = KafkaProducer(bootstrap_servers=self._bootstrap_servers, **kwargs)
             self._initialized = True
 
     async def _do(self, event):
         await self._lazy_init()
 
         if event is _termination_obj:
+            self._producer.flush()
             self._producer.close()
             return await self._do_downstream(_termination_obj)
         else:
             key = None
             if event.key is not None:
                 key = stringify_key(event.key).encode("UTF-8")
             record = self._event_to_writer_entry(event)
@@ -1056,15 +1071,17 @@
             partition = None
             if self._sharding_func:
                 sharding_func_result = self._sharding_func(event)
                 if isinstance(sharding_func_result, int):
                     partition = sharding_func_result
                 else:
                     key = sharding_func_result
-            self._producer.send(self._topic, record, key, partition=partition)
+            future = self._producer.send(self._topic, record, key, partition=partition)
+            # Prevent garbage collection of event until persisted to kafka
+            future.add_callback(lambda x: event)
 
 
 class NoSqlTarget(_Writer, Flow):
     """
     Persists the data in `table` to its associated storage by key.
 
     :param table: A Table object or name to persist. If a table name is provided, it will be looked up in the context.
@@ -1125,9 +1142,10 @@
         if not self._table._flush_interval_secs:
             data_to_persist = self._event_to_writer_entry(event)
             await self._table._persist(_PersistJob(key, data_to_persist, self._handle_completed, event))
         else:
             data_to_persist = self._event_to_writer_entry(event)
             async with self._table._get_lock(key):
                 self._table._update_static_attrs(key, data_to_persist)
+                self._table._pending_events.append(event)
             self._table._init_flush_task()
             await self._do_downstream(event)
```

### Comparing `storey-1.4.4/storey/transformations/__init__.py` & `storey-1.5.0/storey/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/utils.py` & `storey-1.5.0/storey/utils.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey/windowed_store.py` & `storey-1.5.0/storey/windowed_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/storey.egg-info/PKG-INFO` & `storey-1.5.0/storey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storey
-Version: 1.4.4
+Version: 1.5.0
 Summary: Async flows
 Home-page: https://github.com/mlrun/storey
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `storey-1.4.4/storey.egg-info/SOURCES.txt` & `storey-1.5.0/storey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/tests/__init__.py` & `storey-1.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/tests/test_aggregate_by_key.py` & `storey-1.5.0/tests/test_aggregate_by_key.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/tests/test_aggregate_store.py` & `storey-1.5.0/tests/test_aggregate_store.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/tests/test_flow.py` & `storey-1.5.0/tests/test_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import asyncio
 import copy
+import gc
 import math
 import os
 import queue
 import time
 import traceback
 import uuid
 from datetime import datetime
@@ -103,14 +104,230 @@
         for i in range(10):
             controller.emit(i)
     controller.terminate()
     termination_result = controller.await_termination()
     assert termination_result == 3300
 
 
+class Committer:
+    def __init__(self):
+        self.offsets = {}
+
+    async def explicit_ack(self, qualified_offset):
+        qualified_shard = (qualified_offset.topic, qualified_offset.partition)
+        offset = qualified_offset.offset
+        current_offset = self.offsets.get(qualified_shard, 0)
+        assert current_offset < offset
+        self.offsets[qualified_shard] = offset
+
+
+class CommitterContext:
+    def __init__(self, platform):
+        self.platform = platform
+
+
+class EventHoarder(storey.Flow):
+    events = []
+
+    async def _do(self, event):
+        if event is storey.dtypes._termination_obj:
+            self.events = []
+            print("Hoarder terminated")
+        else:
+            self.events.append(event)
+            print("Hoarder hoards!")
+        return await self._do_downstream(event)
+
+
+def test_offset_commit():
+    platform = Committer()
+    context = CommitterContext(platform)
+
+    controller = build_flow(
+        [
+            SyncEmitSource(context=context, explicit_ack=True),
+            Map(lambda x: x + 1),
+            Filter(lambda x: x < 3),
+            FlatMap(lambda x: [x, x * 10]),
+            Reduce(0, lambda acc, x: acc + x),
+        ]
+    ).run()
+
+    num_shards = 10
+    num_records_per_shard = 10
+
+    for offset in range(1, num_records_per_shard + 1):
+        for shard in range(num_shards):
+            event = Event(shard)
+            event.shard_id = shard
+            event.offset = offset
+            controller.emit(event)
+    controller.terminate()
+    termination_result = controller.await_termination()
+    assert termination_result == 330
+
+    offsets = copy.copy(platform.offsets)
+    assert offsets == {("/", i): num_records_per_shard for i in range(num_shards)}
+
+
+async def async_offset_commit():
+    platform = Committer()
+    context = CommitterContext(platform)
+
+    controller = build_flow(
+        [
+            AsyncEmitSource(context=context, explicit_ack=True),
+            Map(lambda x: x + 1),
+            Filter(lambda x: x < 3),
+            FlatMap(lambda x: [x, x * 10]),
+            Reduce(0, lambda acc, x: acc + x),
+        ]
+    ).run()
+
+    num_shards = 10
+    num_records_per_shard = 10
+
+    for offset in range(1, num_records_per_shard + 1):
+        for shard in range(num_shards):
+            event = Event(shard)
+            event.shard_id = shard
+            event.offset = offset
+            await controller.emit(event)
+    print()
+    await controller.terminate()
+    termination_result = await controller.await_termination()
+    assert termination_result == 330
+
+    offsets = copy.copy(platform.offsets)
+    assert offsets == {("/", i): num_records_per_shard for i in range(num_shards)}
+
+
+def test_async_offset_commit():
+    asyncio.run(async_offset_commit())
+
+
+def test_offset_commit_before_termination():
+    platform = Committer()
+    context = CommitterContext(platform)
+
+    controller = build_flow(
+        [
+            SyncEmitSource(context=context, explicit_ack=True),
+            Map(lambda x: x + 1),
+            Filter(lambda x: x < 3),
+            FlatMap(lambda x: [x, x * 10]),
+            Reduce(0, lambda acc, x: acc + x),
+        ]
+    ).run()
+
+    num_shards = 10
+    num_records_per_shard = 10
+
+    for offset in range(1, num_records_per_shard + 1):
+        for shard in range(num_shards):
+            event = Event(shard)
+            event.shard_id = shard
+            event.offset = offset
+            controller.emit(event)
+
+    time.sleep(1)
+    gc.collect()
+    time.sleep(1)
+
+    expected_offsets = {("/", i): num_records_per_shard for i in range(num_shards)}
+    # TODO: Remove when commit of last record is fixed
+    expected_offsets[("/", 9)] = 9
+
+    try:
+        offsets = copy.copy(platform.offsets)
+        assert offsets == expected_offsets
+    finally:
+        controller.terminate()
+    termination_result = controller.await_termination()
+    assert termination_result == 330
+
+
+async def async_offset_commit_before_termination():
+    platform = Committer()
+    context = CommitterContext(platform)
+
+    controller = build_flow(
+        [
+            AsyncEmitSource(context=context, explicit_ack=True),
+            Map(lambda x: x + 1),
+            Filter(lambda x: x < 3),
+            FlatMap(lambda x: [x, x * 10]),
+            Reduce(0, lambda acc, x: acc + x),
+        ]
+    ).run()
+
+    num_shards = 10
+    num_records_per_shard = 10
+
+    for offset in range(1, num_records_per_shard + 1):
+        for shard in range(num_shards):
+            event = Event(shard)
+            event.shard_id = shard
+            event.offset = offset
+            await controller.emit(event)
+
+    del event
+
+    await asyncio.sleep(1)
+    gc.collect()
+    await asyncio.sleep(1)
+
+    try:
+        offsets = copy.copy(platform.offsets)
+        assert offsets == {("/", i): num_records_per_shard for i in range(num_shards)}
+    finally:
+        await controller.terminate()
+    termination_result = await controller.await_termination()
+    assert termination_result == 330
+
+
+def test_async_offset_commit_before_termination():
+    asyncio.run(async_offset_commit_before_termination())
+
+
+def test_offset_not_committed_prematurely():
+    platform = Committer()
+    context = CommitterContext(platform)
+
+    controller = build_flow(
+        [
+            SyncEmitSource(context=context, explicit_ack=True),
+            EventHoarder(),
+            Reduce(0, lambda acc, x: acc + x),
+        ]
+    ).run()
+
+    num_shards = 10
+    num_records_per_shard = 10
+
+    for offset in range(1, num_records_per_shard + 1):
+        for shard in range(num_shards):
+            event = Event(shard)
+            event.shard_id = shard
+            event.offset = offset
+            controller.emit(event)
+
+    time.sleep(1)
+
+    try:
+        offsets = copy.copy(platform.offsets)
+        assert offsets == {}
+    finally:
+        controller.terminate()
+    termination_result = controller.await_termination()
+    assert termination_result == 450
+    offsets = copy.copy(platform.offsets)
+    assert offsets == {("/", i): num_records_per_shard for i in range(num_shards)}
+
+
 def test_multiple_upstreams():
     source = SyncEmitSource()
     map1 = Map(lambda x: x + 1)
     map2 = Map(lambda x: x * 10)
     reduce = Reduce(0, lambda x, y: x + y)
     source.to(map1)
     source.to(map2)
@@ -121,14 +338,29 @@
     for i in range(10):
         controller.emit(i)
     controller.terminate()
     termination_result = controller.await_termination()
     assert termination_result == 55 + 450
 
 
+def test_multiple_upstreams_csv_source():
+    source = CSVSource("tests/test.csv")
+    map1 = Map(lambda x: append_and_return(x, "map1"))
+    map2 = Map(lambda x: append_and_return(x, "map2"))
+    reduce = Reduce([], append_and_return)
+    source.to(map1)
+    source.to(map2)
+    map1.to(reduce)
+    map2.to(reduce)
+    controller = source.run()
+
+    termination_result = controller.await_termination()
+    assert termination_result == [[1, 2, 3, "map1"], [1, 2, 3, "map2"], [4, 5, 6, "map1"], [4, 5, 6, "map2"]]
+
+
 def test_multiple_upstreams_completion():
     source = SyncEmitSource()
     map1 = Map(lambda x: x + 1)
     map2 = Map(lambda x: x * 10)
     complete = Complete()
     source.to(map1)
     source.to(map2)
```

### Comparing `storey-1.4.4/tests/test_steps.py` & `storey-1.5.0/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/tests/test_types.py` & `storey-1.5.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/tests/test_v3io.py` & `storey-1.5.0/tests/test_v3io.py`

 * *Files identical despite different names*

### Comparing `storey-1.4.4/tests/test_windowed_store.py` & `storey-1.5.0/tests/test_windowed_store.py`

 * *Files identical despite different names*

