# Comparing `tmp/botocore-a-la-carte-acm-pca-1.31.3.tar.gz` & `tmp/botocore-a-la-carte-acm-pca-1.31.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-acm-pca-1.31.3.tar", last modified: Fri Jul 14 01:45:51 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-acm-pca-1.31.4.tar", last modified: Tue Jul 18 01:54:55 2023, max compression
```

## Comparing `botocore-a-la-carte-acm-pca-1.31.3.tar` & `botocore-a-la-carte-acm-pca-1.31.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.454464 botocore-a-la-carte-acm-pca-1.31.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:45:51.000000 botocore-a-la-carte-acm-pca-1.31.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-14 01:45:51.454464 botocore-a-la-carte-acm-pca-1.31.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.454464 botocore-a-la-carte-acm-pca-1.31.3/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.454464 botocore-a-la-carte-acm-pca-1.31.3/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.454464 botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.454464 botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-07-14 01:45:44.000000 botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-14 01:45:44.000000 botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   136588 2023-07-14 01:45:44.000000 botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-14 01:45:44.000000 botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.454464 botocore-a-la-carte-acm-pca-1.31.3/botocore_a_la_carte_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-14 01:45:51.000000 botocore-a-la-carte-acm-pca-1.31.3/botocore_a_la_carte_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-14 01:45:51.000000 botocore-a-la-carte-acm-pca-1.31.3/botocore_a_la_carte_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:45:51.000000 botocore-a-la-carte-acm-pca-1.31.3/botocore_a_la_carte_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:45:51.000000 botocore-a-la-carte-acm-pca-1.31.3/botocore_a_la_carte_acm_pca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:45:51.454464 botocore-a-la-carte-acm-pca-1.31.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 01:45:51.000000 botocore-a-la-carte-acm-pca-1.31.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.220148 botocore-a-la-carte-acm-pca-1.31.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 01:54:55.000000 botocore-a-la-carte-acm-pca-1.31.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-18 01:54:55.220148 botocore-a-la-carte-acm-pca-1.31.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.216148 botocore-a-la-carte-acm-pca-1.31.4/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.216148 botocore-a-la-carte-acm-pca-1.31.4/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.216148 botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.216148 botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-07-18 01:54:49.000000 botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:49.000000 botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-18 01:54:49.000000 botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   136588 2023-07-18 01:54:49.000000 botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-18 01:54:49.000000 botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.220148 botocore-a-la-carte-acm-pca-1.31.4/botocore_a_la_carte_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-18 01:54:55.000000 botocore-a-la-carte-acm-pca-1.31.4/botocore_a_la_carte_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 01:54:55.000000 botocore-a-la-carte-acm-pca-1.31.4/botocore_a_la_carte_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:54:55.000000 botocore-a-la-carte-acm-pca-1.31.4/botocore_a_la_carte_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 01:54:55.000000 botocore-a-la-carte-acm-pca-1.31.4/botocore_a_la_carte_acm_pca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:54:55.220148 botocore-a-la-carte-acm-pca-1.31.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-18 01:54:55.000000 botocore-a-la-carte-acm-pca-1.31.4/setup.py
```

### Comparing `botocore-a-la-carte-acm-pca-1.31.3/LICENSE.txt` & `botocore-a-la-carte-acm-pca-1.31.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-acm-pca-1.31.3/PKG-INFO` & `botocore-a-la-carte-acm-pca-1.31.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-acm-pca
-Version: 1.31.3
+Version: 1.31.4
 Summary: acm-pca data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/endpoint-rule-set-1.json` & `botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/paginators-1.json` & `botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/service-2.json` & `botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-acm-pca-1.31.3/botocore/data/acm-pca/2017-08-22/waiters-2.json` & `botocore-a-la-carte-acm-pca-1.31.4/botocore/data/acm-pca/2017-08-22/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-acm-pca-1.31.3/botocore_a_la_carte_acm_pca.egg-info/PKG-INFO` & `botocore-a-la-carte-acm-pca-1.31.4/botocore_a_la_carte_acm_pca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-acm-pca
-Version: 1.31.3
+Version: 1.31.4
 Summary: acm-pca data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-acm-pca-1.31.3/setup.py` & `botocore-a-la-carte-acm-pca-1.31.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-acm-pca',
-    version="1.31.3",
+    version="1.31.4",
     description='acm-pca data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/acm-pca/*/*.json'],
```

