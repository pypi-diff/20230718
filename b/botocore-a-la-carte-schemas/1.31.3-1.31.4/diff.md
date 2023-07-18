# Comparing `tmp/botocore-a-la-carte-schemas-1.31.3.tar.gz` & `tmp/botocore-a-la-carte-schemas-1.31.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-schemas-1.31.3.tar", last modified: Fri Jul 14 01:46:43 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-schemas-1.31.4.tar", last modified: Tue Jul 18 01:55:37 2023, max compression
```

## Comparing `botocore-a-la-carte-schemas-1.31.3.tar` & `botocore-a-la-carte-schemas-1.31.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:43.383006 botocore-a-la-carte-schemas-1.31.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:46:43.000000 botocore-a-la-carte-schemas-1.31.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-14 01:46:43.383006 botocore-a-la-carte-schemas-1.31.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:43.383006 botocore-a-la-carte-schemas-1.31.3/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:43.383006 botocore-a-la-carte-schemas-1.31.3/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:43.383006 botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:43.383006 botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/2019-12-02/
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-07-14 01:45:45.000000 botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/2019-12-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-14 01:45:45.000000 botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/2019-12-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    99536 2023-07-14 01:45:45.000000 botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/2019-12-02/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-14 01:45:45.000000 botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/2019-12-02/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:43.383006 botocore-a-la-carte-schemas-1.31.3/botocore_a_la_carte_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-14 01:46:43.000000 botocore-a-la-carte-schemas-1.31.3/botocore_a_la_carte_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-14 01:46:43.000000 botocore-a-la-carte-schemas-1.31.3/botocore_a_la_carte_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:46:43.000000 botocore-a-la-carte-schemas-1.31.3/botocore_a_la_carte_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:46:43.000000 botocore-a-la-carte-schemas-1.31.3/botocore_a_la_carte_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:46:43.383006 botocore-a-la-carte-schemas-1.31.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 01:46:43.000000 botocore-a-la-carte-schemas-1.31.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:37.856338 botocore-a-la-carte-schemas-1.31.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 01:55:37.000000 botocore-a-la-carte-schemas-1.31.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-18 01:55:37.856338 botocore-a-la-carte-schemas-1.31.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:37.852338 botocore-a-la-carte-schemas-1.31.4/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:37.852338 botocore-a-la-carte-schemas-1.31.4/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:37.852338 botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:37.852338 botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/2019-12-02/
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-07-18 01:54:50.000000 botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/2019-12-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-18 01:54:50.000000 botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/2019-12-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    99536 2023-07-18 01:54:50.000000 botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/2019-12-02/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-18 01:54:50.000000 botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/2019-12-02/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:37.852338 botocore-a-la-carte-schemas-1.31.4/botocore_a_la_carte_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-18 01:55:37.000000 botocore-a-la-carte-schemas-1.31.4/botocore_a_la_carte_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-18 01:55:37.000000 botocore-a-la-carte-schemas-1.31.4/botocore_a_la_carte_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:55:37.000000 botocore-a-la-carte-schemas-1.31.4/botocore_a_la_carte_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 01:55:37.000000 botocore-a-la-carte-schemas-1.31.4/botocore_a_la_carte_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:55:37.856338 botocore-a-la-carte-schemas-1.31.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-18 01:55:37.000000 botocore-a-la-carte-schemas-1.31.4/setup.py
```

### Comparing `botocore-a-la-carte-schemas-1.31.3/LICENSE.txt` & `botocore-a-la-carte-schemas-1.31.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-schemas-1.31.3/PKG-INFO` & `botocore-a-la-carte-schemas-1.31.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-schemas
-Version: 1.31.3
+Version: 1.31.4
 Summary: schemas data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/2019-12-02/endpoint-rule-set-1.json` & `botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/2019-12-02/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/2019-12-02/paginators-1.json` & `botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/2019-12-02/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/2019-12-02/service-2.json` & `botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/2019-12-02/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-schemas-1.31.3/botocore/data/schemas/2019-12-02/waiters-2.json` & `botocore-a-la-carte-schemas-1.31.4/botocore/data/schemas/2019-12-02/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-schemas-1.31.3/botocore_a_la_carte_schemas.egg-info/PKG-INFO` & `botocore-a-la-carte-schemas-1.31.4/botocore_a_la_carte_schemas.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-schemas
-Version: 1.31.3
+Version: 1.31.4
 Summary: schemas data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-schemas-1.31.3/setup.py` & `botocore-a-la-carte-schemas-1.31.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-schemas',
-    version="1.31.3",
+    version="1.31.4",
     description='schemas data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/schemas/*/*.json'],
```

