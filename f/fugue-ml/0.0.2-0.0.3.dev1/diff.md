# Comparing `tmp/fugue-ml-0.0.2.tar.gz` & `tmp/fugue-ml-0.0.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-ml-0.0.2.tar", last modified: Wed May 24 07:55:17 2023, max compression
+gzip compressed data, was "fugue-ml-0.0.3.dev1.tar", last modified: Tue Jul 18 07:29:40 2023, max compression
```

## Comparing `fugue-ml-0.0.2.tar` & `fugue-ml-0.0.3.dev1.tar`

### file list

```diff
@@ -1,25 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:55:17.886147 fugue-ml-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-24 07:55:17.886147 fugue-ml-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:55:17.882146 fugue-ml-0.0.2/fugue_ml/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/fugue_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:55:17.882146 fugue-ml-0.0.2/fugue_ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/fugue_ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/fugue_ml/utils/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:55:17.882146 fugue-ml-0.0.2/fugue_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-24 07:55:17.000000 fugue-ml-0.0.2/fugue_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-24 07:55:17.000000 fugue-ml-0.0.2/fugue_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:55:17.000000 fugue-ml-0.0.2/fugue_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 07:55:17.000000 fugue-ml-0.0.2/fugue_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 07:55:17.000000 fugue-ml-0.0.2/fugue_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 07:55:17.000000 fugue-ml-0.0.2/fugue_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:55:17.886147 fugue-ml-0.0.2/fugue_ml_version/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/fugue_ml_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-24 07:55:17.886147 fugue-ml-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:55:17.886147 fugue-ml-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:55:17.886147 fugue-ml-0.0.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-24 07:54:10.000000 fugue-ml-0.0.2/tests/utils/test_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/fugue_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/fugue_ml/ann/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/ann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/ann/indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/fugue_ml/ann/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/ann/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/ann/integrations/nmslib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/embedding/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/embedding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/embedding/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/sentence_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/cred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/knn/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/knn/brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19100 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/knn/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/test/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/test/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/test/embedding/cache_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/fugue_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/utils/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/numpy/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/fugue_ml_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/tests/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/tests/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/tests/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/tests/knn/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/integrations/test_brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/test_api_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/test_indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/tests/utils/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/numpy/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/test_fugue_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/test_schema.py
```

### Comparing `fugue-ml-0.0.2/LICENSE` & `fugue-ml-0.0.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.2/PKG-INFO` & `fugue-ml-0.0.3.dev1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue-ml
-Version: 0.0.2
+Version: 0.0.3.dev1
 Summary: Fugue ML
 Home-page: http://github.com/fugue-project/fugue-ml
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue Machine Learning Library
         
@@ -20,7 +20,9 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: openai
+Provides-Extra: huggingface
```

### Comparing `fugue-ml-0.0.2/fugue_ml.egg-info/PKG-INFO` & `fugue-ml-0.0.3.dev1/fugue_ml.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue-ml
-Version: 0.0.2
+Version: 0.0.3.dev1
 Summary: Fugue ML
 Home-page: http://github.com/fugue-project/fugue-ml
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue Machine Learning Library
         
@@ -20,7 +20,9 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: openai
+Provides-Extra: huggingface
```

### Comparing `fugue-ml-0.0.2/setup.py` & `fugue-ml-0.0.3.dev1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,35 +16,42 @@
         assert tag == __version__, "release tag and version mismatch"
     return __version__
 
 
 setup(
     name="fugue-ml",
     version=get_version(),
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests"]),
     description="Fugue ML",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     author="The Fugue Development Team",
     author_email="hello@fugue.ai",
     keywords="fugue machine learning ai",
     url="http://github.com/fugue-project/fugue-ml",
-    install_requires=["fugue>=0.8.4"],
-    extras_require={},
+    package_data={"fugue_ml": ["py.typed"]},
+    install_requires=["fugue>=0.8.5", "fsspec>=2023.1.0"],
+    extras_require={
+        "openai": ["openai", "tiktoken"],
+        "huggingface": ["transformers", "sentence-transformers"],
+    },
     classifiers=[
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     python_requires=">=3.7",
     entry_points={
-        "fugue.plugins": [],
+        "fugue_ml.plugins": [
+            "openai = fugue_ml.integrations.openai.registry[openai]",
+            "huggingface = fugue_ml.integrations.huggingface.registry[huggingface]",
+        ],
     },
 )
```

### Comparing `fugue-ml-0.0.2/tests/utils/test_numpy.py` & `fugue-ml-0.0.3.dev1/tests/utils/numpy/test_distance.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,86 @@
 import numpy as np
 from pytest import raises
 
-from fugue_ml.utils.numpy import (
-    compute_cos_matrix,
-    compute_l2_square_matrix,
-    find_best_n_matches,
+from fugue_ml.utils.numpy.distance import (
+    compute_distance_matrix,
+    knn,
 )
 
 
 def test_compute_l2_square_matrix():
     v1 = np.array([[1, 2, 3], [4, 5, 6]])
     v2 = np.array([[0, 1, 0], [3, 2, 1], [6, 5, 4]])
     res = np.zeros((2, 3))
     for i in range(2):
         for j in range(3):
-            res[i, j] = np.sum(np.square(v1[i] - v2[j]))
-    assert np.allclose(res, compute_l2_square_matrix(v1, v2))
+            res[i, j] = np.sqrt(np.sum(np.square(v1[i] - v2[j])))
+    assert np.allclose(res, compute_distance_matrix(v1, v2, metric="l2"))
+
+
+def test_compute_dot_matrix():
+    v1 = np.array([[1, 2, 3], [4, 5, 6]])
+    v2 = np.array([[0, 1, 0], [3, 2, 1], [6, 5, 4]])
+    res = np.zeros((2, 3))
+    for i in range(2):
+        for j in range(3):
+            a, b = v1[i], v2[j]
+            res[i, j] = -np.dot(a, b)
+    assert np.allclose(res, compute_distance_matrix(v1, v2, metric="dot"))
 
 
 def test_compute_cos_matrix():
     v1 = np.array([[1, 2, 3], [4, 5, 6]])
     v2 = np.array([[0, 1, 0], [3, 2, 1], [6, 5, 4]])
     res = np.zeros((2, 3))
     for i in range(2):
         for j in range(3):
             a, b = v1[i], v2[j]
             res[i, j] = 1 - np.dot(a, b) / (np.linalg.norm(a, 2) * np.linalg.norm(b, 2))
-    assert np.allclose(res, compute_cos_matrix(v1, v2))
+    assert np.allclose(res, compute_distance_matrix(v1, v2, metric="cos"))
 
 
-def test_find_best_n_matches():
+def test_knn_matches():
     v1 = np.array([[1, 2, 3], [4, 5, 6]])
     v2 = np.array([[4.1, 5.1, 6.1], [3, 3, 3], [1.1, 2.1, 3.1]])
     res = np.zeros((2, 3))
-    idx, res = find_best_n_matches(v1, v2, metric="l2", n=1)
+    idx, res = knn(v2, v1, metric="l2", k=1)
     assert np.allclose(idx, np.array([[2], [0]]))
     assert np.allclose(
         res,
         np.array(
             [[np.linalg.norm(v2[2] - v1[0], 2)], [np.linalg.norm(v2[0] - v1[1], 2)]]
         ),
     )
-    idx, res = find_best_n_matches(v1, v2, metric="l2", n=2)
+    idx, res = knn(v2, v1, metric="l2", k=2)
     assert np.allclose(idx, np.array([[2, 1], [0, 1]]))
     assert np.allclose(
         res,
         np.array(
             [
                 [np.linalg.norm(v2[2] - v1[0], 2), np.linalg.norm(v2[1] - v1[0], 2)],
                 [np.linalg.norm(v2[0] - v1[1], 2), np.linalg.norm(v2[1] - v1[1], 2)],
             ]
         ),
     )
-    idx, res = find_best_n_matches(v1, v2, metric="cos", n=3)
-    assert np.allclose(idx, np.array([[0, 1, 2], [0, 1, 2]]))
-    assert np.allclose(res, compute_cos_matrix(v1, v2))
+    idx, res = knn(v2, v1, metric="l2", k=3)
+    assert np.allclose(idx, np.array([[2, 1, 0], [0, 1, 2]]))
+    assert np.allclose(
+        res,
+        np.array(
+            [
+                [
+                    np.linalg.norm(v2[2] - v1[0], 2),
+                    np.linalg.norm(v2[1] - v1[0], 2),
+                    np.linalg.norm(v2[0] - v1[0], 2),
+                ],
+                [
+                    np.linalg.norm(v2[0] - v1[1], 2),
+                    np.linalg.norm(v2[1] - v1[1], 2),
+                    np.linalg.norm(v2[2] - v1[1], 2),
+                ],
+            ]
+        ),
+    )
 
     with raises(ValueError):
-        find_best_n_matches(v1, v2, metric="unknown", n=1)
+        knn(v1, v2, metric="unknown", k=1)
```

