# Comparing `tmp/flytekitplugins-ray-1.8.0.tar.gz` & `tmp/flytekitplugins-ray-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-ray-1.8.0.tar", last modified: Tue Jul 11 22:07:24 2023, max compression
+gzip compressed data, was "flytekitplugins-ray-1.8.1.tar", last modified: Tue Jul 18 18:01:42 2023, max compression
```

## Comparing `flytekitplugins-ray-1.8.0.tar` & `flytekitplugins-ray-1.8.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:24.963756 flytekitplugins-ray-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-11 22:07:24.963756 flytekitplugins-ray-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-11 22:06:52.000000 flytekitplugins-ray-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:24.959756 flytekitplugins-ray-1.8.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:24.959756 flytekitplugins-ray-1.8.0/flytekitplugins/ray/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-11 22:06:52.000000 flytekitplugins-ray-1.8.0/flytekitplugins/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-11 22:06:52.000000 flytekitplugins-ray-1.8.0/flytekitplugins/ray/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-11 22:06:52.000000 flytekitplugins-ray-1.8.0/flytekitplugins/ray/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:24.963756 flytekitplugins-ray-1.8.0/flytekitplugins_ray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-11 22:07:24.000000 flytekitplugins-ray-1.8.0/flytekitplugins_ray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 22:07:24.000000 flytekitplugins-ray-1.8.0/flytekitplugins_ray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:24.000000 flytekitplugins-ray-1.8.0/flytekitplugins_ray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:24.000000 flytekitplugins-ray-1.8.0/flytekitplugins_ray.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 22:07:24.000000 flytekitplugins-ray-1.8.0/flytekitplugins_ray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:24.000000 flytekitplugins-ray-1.8.0/flytekitplugins_ray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:24.963756 flytekitplugins-ray-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-11 22:07:11.000000 flytekitplugins-ray-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:42.919022 flytekitplugins-ray-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-18 18:01:42.915022 flytekitplugins-ray-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-18 18:01:17.000000 flytekitplugins-ray-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:42.915022 flytekitplugins-ray-1.8.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:42.915022 flytekitplugins-ray-1.8.1/flytekitplugins/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-18 18:01:17.000000 flytekitplugins-ray-1.8.1/flytekitplugins/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-18 18:01:17.000000 flytekitplugins-ray-1.8.1/flytekitplugins/ray/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-18 18:01:17.000000 flytekitplugins-ray-1.8.1/flytekitplugins/ray/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:42.915022 flytekitplugins-ray-1.8.1/flytekitplugins_ray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-18 18:01:42.000000 flytekitplugins-ray-1.8.1/flytekitplugins_ray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-18 18:01:42.000000 flytekitplugins-ray-1.8.1/flytekitplugins_ray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:42.000000 flytekitplugins-ray-1.8.1/flytekitplugins_ray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:42.000000 flytekitplugins-ray-1.8.1/flytekitplugins_ray.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 18:01:42.000000 flytekitplugins-ray-1.8.1/flytekitplugins_ray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:42.000000 flytekitplugins-ray-1.8.1/flytekitplugins_ray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:42.919022 flytekitplugins-ray-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-18 18:01:33.000000 flytekitplugins-ray-1.8.1/setup.py
```

### Comparing `flytekitplugins-ray-1.8.0/PKG-INFO` & `flytekitplugins-ray-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-ray
-Version: 1.8.0
+Version: 1.8.1
 Summary: This package holds the Ray plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-ray-1.8.0/flytekitplugins/ray/models.py` & `flytekitplugins-ray-1.8.1/flytekitplugins/ray/models.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-ray-1.8.0/flytekitplugins/ray/task.py` & `flytekitplugins-ray-1.8.1/flytekitplugins/ray/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-ray-1.8.0/flytekitplugins_ray.egg-info/PKG-INFO` & `flytekitplugins-ray-1.8.1/flytekitplugins_ray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-ray
-Version: 1.8.0
+Version: 1.8.1
 Summary: This package holds the Ray plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-ray-1.8.0/setup.py` & `flytekitplugins-ray-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "ray"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["ray[default]", "flytekit>=1.3.0b2,<2.0.0", "flyteidl>=1.1.10"]
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Ray plugins for flytekit",
```

