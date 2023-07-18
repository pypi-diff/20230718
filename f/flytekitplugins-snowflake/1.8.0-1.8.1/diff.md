# Comparing `tmp/flytekitplugins-snowflake-1.8.0.tar.gz` & `tmp/flytekitplugins-snowflake-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-snowflake-1.8.0.tar", last modified: Tue Jul 11 22:07:25 2023, max compression
+gzip compressed data, was "flytekitplugins-snowflake-1.8.1.tar", last modified: Tue Jul 18 18:01:43 2023, max compression
```

## Comparing `flytekitplugins-snowflake-1.8.0.tar` & `flytekitplugins-snowflake-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:25.459760 flytekitplugins-snowflake-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-11 22:07:25.455760 flytekitplugins-snowflake-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-11 22:06:52.000000 flytekitplugins-snowflake-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:25.451760 flytekitplugins-snowflake-1.8.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:25.455760 flytekitplugins-snowflake-1.8.0/flytekitplugins/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 22:06:52.000000 flytekitplugins-snowflake-1.8.0/flytekitplugins/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-11 22:06:52.000000 flytekitplugins-snowflake-1.8.0/flytekitplugins/snowflake/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:25.455760 flytekitplugins-snowflake-1.8.0/flytekitplugins_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-11 22:07:25.000000 flytekitplugins-snowflake-1.8.0/flytekitplugins_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 22:07:25.000000 flytekitplugins-snowflake-1.8.0/flytekitplugins_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:25.000000 flytekitplugins-snowflake-1.8.0/flytekitplugins_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:25.000000 flytekitplugins-snowflake-1.8.0/flytekitplugins_snowflake.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 22:07:25.000000 flytekitplugins-snowflake-1.8.0/flytekitplugins_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:25.000000 flytekitplugins-snowflake-1.8.0/flytekitplugins_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:25.459760 flytekitplugins-snowflake-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-11 22:07:11.000000 flytekitplugins-snowflake-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:43.283022 flytekitplugins-snowflake-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-18 18:01:43.283022 flytekitplugins-snowflake-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-18 18:01:17.000000 flytekitplugins-snowflake-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:43.283022 flytekitplugins-snowflake-1.8.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:43.283022 flytekitplugins-snowflake-1.8.1/flytekitplugins/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-18 18:01:17.000000 flytekitplugins-snowflake-1.8.1/flytekitplugins/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-18 18:01:17.000000 flytekitplugins-snowflake-1.8.1/flytekitplugins/snowflake/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:43.283022 flytekitplugins-snowflake-1.8.1/flytekitplugins_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-18 18:01:43.000000 flytekitplugins-snowflake-1.8.1/flytekitplugins_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 18:01:43.000000 flytekitplugins-snowflake-1.8.1/flytekitplugins_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:43.000000 flytekitplugins-snowflake-1.8.1/flytekitplugins_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:43.000000 flytekitplugins-snowflake-1.8.1/flytekitplugins_snowflake.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 18:01:43.000000 flytekitplugins-snowflake-1.8.1/flytekitplugins_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:43.000000 flytekitplugins-snowflake-1.8.1/flytekitplugins_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:43.283022 flytekitplugins-snowflake-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-18 18:01:33.000000 flytekitplugins-snowflake-1.8.1/setup.py
```

### Comparing `flytekitplugins-snowflake-1.8.0/PKG-INFO` & `flytekitplugins-snowflake-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-snowflake
-Version: 1.8.0
+Version: 1.8.1
 Summary: This package holds the Snowflake plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-snowflake-1.8.0/README.md` & `flytekitplugins-snowflake-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-snowflake-1.8.0/flytekitplugins/snowflake/task.py` & `flytekitplugins-snowflake-1.8.1/flytekitplugins/snowflake/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-snowflake-1.8.0/flytekitplugins_snowflake.egg-info/PKG-INFO` & `flytekitplugins-snowflake-1.8.1/flytekitplugins_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-snowflake
-Version: 1.8.0
+Version: 1.8.1
 Summary: This package holds the Snowflake plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-snowflake-1.8.0/setup.py` & `flytekitplugins-snowflake-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "snowflake"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Snowflake plugins for flytekit",
```

