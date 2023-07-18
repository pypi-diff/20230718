# Comparing `tmp/flytekitplugins-kftensorflow-1.8.0.tar.gz` & `tmp/flytekitplugins-kftensorflow-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kftensorflow-1.8.0.tar", last modified: Tue Jul 11 22:07:20 2023, max compression
+gzip compressed data, was "flytekitplugins-kftensorflow-1.8.1.tar", last modified: Tue Jul 18 18:01:40 2023, max compression
```

## Comparing `flytekitplugins-kftensorflow-1.8.0.tar` & `flytekitplugins-kftensorflow-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:20.891719 flytekitplugins-kftensorflow-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-11 22:07:20.891719 flytekitplugins-kftensorflow-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-11 22:06:52.000000 flytekitplugins-kftensorflow-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:20.891719 flytekitplugins-kftensorflow-1.8.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:20.891719 flytekitplugins-kftensorflow-1.8.0/flytekitplugins/kftensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-11 22:06:52.000000 flytekitplugins-kftensorflow-1.8.0/flytekitplugins/kftensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-11 22:06:52.000000 flytekitplugins-kftensorflow-1.8.0/flytekitplugins/kftensorflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:20.891719 flytekitplugins-kftensorflow-1.8.0/flytekitplugins_kftensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-11 22:07:20.000000 flytekitplugins-kftensorflow-1.8.0/flytekitplugins_kftensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-11 22:07:20.000000 flytekitplugins-kftensorflow-1.8.0/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:20.000000 flytekitplugins-kftensorflow-1.8.0/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:20.000000 flytekitplugins-kftensorflow-1.8.0/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:20.000000 flytekitplugins-kftensorflow-1.8.0/flytekitplugins_kftensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:20.000000 flytekitplugins-kftensorflow-1.8.0/flytekitplugins_kftensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:20.891719 flytekitplugins-kftensorflow-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-11 22:07:11.000000 flytekitplugins-kftensorflow-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:40.015022 flytekitplugins-kftensorflow-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-18 18:01:40.015022 flytekitplugins-kftensorflow-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-18 18:01:17.000000 flytekitplugins-kftensorflow-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:40.015022 flytekitplugins-kftensorflow-1.8.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:40.015022 flytekitplugins-kftensorflow-1.8.1/flytekitplugins/kftensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 18:01:17.000000 flytekitplugins-kftensorflow-1.8.1/flytekitplugins/kftensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-18 18:01:17.000000 flytekitplugins-kftensorflow-1.8.1/flytekitplugins/kftensorflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:40.015022 flytekitplugins-kftensorflow-1.8.1/flytekitplugins_kftensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-18 18:01:39.000000 flytekitplugins-kftensorflow-1.8.1/flytekitplugins_kftensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-18 18:01:39.000000 flytekitplugins-kftensorflow-1.8.1/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:39.000000 flytekitplugins-kftensorflow-1.8.1/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:39.000000 flytekitplugins-kftensorflow-1.8.1/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:39.000000 flytekitplugins-kftensorflow-1.8.1/flytekitplugins_kftensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:39.000000 flytekitplugins-kftensorflow-1.8.1/flytekitplugins_kftensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:40.015022 flytekitplugins-kftensorflow-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 18:01:33.000000 flytekitplugins-kftensorflow-1.8.1/setup.py
```

### Comparing `flytekitplugins-kftensorflow-1.8.0/PKG-INFO` & `flytekitplugins-kftensorflow-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.8.0
+Version: 1.8.1
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.8.0/README.md` & `flytekitplugins-kftensorflow-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kftensorflow-1.8.0/flytekitplugins/kftensorflow/task.py` & `flytekitplugins-kftensorflow-1.8.1/flytekitplugins/kftensorflow/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kftensorflow-1.8.0/flytekitplugins_kftensorflow.egg-info/PKG-INFO` & `flytekitplugins-kftensorflow-1.8.1/flytekitplugins_kftensorflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.8.0
+Version: 1.8.1
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.8.0/setup.py` & `flytekitplugins-kftensorflow-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kftensorflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.6.1"]
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Tensorflow plugin for flytekit",
```

