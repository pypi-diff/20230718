# Comparing `tmp/autogluon.eda-0.8.3b20230717.tar.gz` & `tmp/autogluon.eda-0.8.3b20230718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.eda-0.8.3b20230717.tar", last modified: Mon Jul 17 09:04:31 2023, max compression
+gzip compressed data, was "autogluon.eda-0.8.3b20230718.tar", last modified: Tue Jul 18 09:04:30 2023, max compression
```

## Comparing `autogluon.eda-0.8.3b20230717.tar` & `autogluon.eda-0.8.3b20230718.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:31.595884 autogluon.eda-0.8.3b20230717/
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-07-17 09:04:31.595884 autogluon.eda-0.8.3b20230717/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-17 09:04:31.599884 autogluon.eda-0.8.3b20230717/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:31.591884 autogluon.eda-0.8.3b20230717/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:31.591884 autogluon.eda-0.8.3b20230717/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:31.595884 autogluon.eda-0.8.3b20230717/src/autogluon/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:31.595884 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:31.595884 autogluon.eda-0.8.3b20230717/src/autogluon/eda/auto/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77515 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/auto/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:31.595884 autogluon.eda-0.8.3b20230717/src/autogluon/eda/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 09:04:31.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:31.595884 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-17 09:03:42.000000 autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/shift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:31.595884 autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-07-17 09:04:31.000000 autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-17 09:04:31.000000 autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:04:31.000000 autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 09:04:31.000000 autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-17 09:04:31.000000 autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 09:04:31.000000 autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:04:31.000000 autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:30.125407 autogluon.eda-0.8.3b20230718/
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-07-18 09:04:30.125407 autogluon.eda-0.8.3b20230718/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-18 09:04:30.129407 autogluon.eda-0.8.3b20230718/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:30.121407 autogluon.eda-0.8.3b20230718/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:30.121407 autogluon.eda-0.8.3b20230718/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:30.125407 autogluon.eda-0.8.3b20230718/src/autogluon/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:30.125407 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:30.125407 autogluon.eda-0.8.3b20230718/src/autogluon/eda/auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77515 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/auto/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:30.125407 autogluon.eda-0.8.3b20230718/src/autogluon/eda/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 09:04:29.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:30.125407 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-18 09:03:47.000000 autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/shift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:30.125407 autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-07-18 09:04:30.000000 autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-18 09:04:30.000000 autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:04:30.000000 autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 09:04:30.000000 autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 09:04:30.000000 autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 09:04:30.000000 autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:04:30.000000 autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/zip-safe
```

### Comparing `autogluon.eda-0.8.3b20230717/PKG-INFO` & `autogluon.eda-0.8.3b20230718/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.eda
-Version: 0.8.3b20230717
+Version: 0.8.3b20230718
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.eda-0.8.3b20230717/setup.cfg` & `autogluon.eda-0.8.3b20230718/setup.cfg`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/setup.py` & `autogluon.eda-0.8.3b20230718/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/__init__.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/anomaly.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/anomaly.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,18 @@
         if detector_list is None:
             detector_list = AnomalyDetector._get_default_detector_list()
         self.detector_list = detector_list
 
         # Can't go beyond 4 - SUOD is throwing errors
         num_cpus = min(ResourceManager.get_cpu_count(), 4)
 
-        suod_defaults = dict(base_estimators=self.detector_list, n_jobs=num_cpus, combination="average", verbose=False)
+        # Don't use `bps_flag=True` - it's using pre-trained models which aren't loading in newer versions of sklearn
+        suod_defaults = dict(
+            base_estimators=self.detector_list, n_jobs=num_cpus, combination="average", bps_flag=False, verbose=False
+        )
         self._suod_kwargs = {**suod_defaults, **detector_kwargs}
         self._detectors: Optional[List[BaseDetector]] = None
         self._train_index_to_detector: Optional[Dict[int, Any]] = None
         self.original_features: Optional[List[str]] = None
 
     @staticmethod
     def _get_default_detector_list():
```

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/base.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/dataset.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/explain.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/interaction.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/interaction.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/missing.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/missing.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/model.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/shift.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/shift.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/analysis/transform.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/auto/simple.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/auto/simple.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/state.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/state.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/utils/common.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/utils/common.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/utils/defaults.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/__init__.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/anomaly.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/anomaly.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/base.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/dataset.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/explain.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/explain.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/interaction.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/interaction.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/jupyter.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/jupyter.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/layouts.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/layouts.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/missing.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/missing.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/model.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon/eda/visualization/shift.py` & `autogluon.eda-0.8.3b20230718/src/autogluon/eda/visualization/shift.py`

 * *Files identical despite different names*

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/PKG-INFO` & `autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.eda
-Version: 0.8.3b20230717
+Version: 0.8.3b20230718
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.eda-0.8.3b20230717/src/autogluon.eda.egg-info/SOURCES.txt` & `autogluon.eda-0.8.3b20230718/src/autogluon.eda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

