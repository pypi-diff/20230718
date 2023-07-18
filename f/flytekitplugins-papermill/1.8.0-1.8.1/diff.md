# Comparing `tmp/flytekitplugins-papermill-1.8.0.tar.gz` & `tmp/flytekitplugins-papermill-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-papermill-1.8.0.tar", last modified: Tue Jul 11 22:07:23 2023, max compression
+gzip compressed data, was "flytekitplugins-papermill-1.8.1.tar", last modified: Tue Jul 18 18:01:42 2023, max compression
```

## Comparing `flytekitplugins-papermill-1.8.0.tar` & `flytekitplugins-papermill-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.955747 flytekitplugins-papermill-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-11 22:07:23.951747 flytekitplugins-papermill-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-11 22:06:52.000000 flytekitplugins-papermill-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.951747 flytekitplugins-papermill-1.8.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.951747 flytekitplugins-papermill-1.8.0/flytekitplugins/papermill/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 22:06:52.000000 flytekitplugins-papermill-1.8.0/flytekitplugins/papermill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-07-11 22:06:52.000000 flytekitplugins-papermill-1.8.0/flytekitplugins/papermill/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.951747 flytekitplugins-papermill-1.8.0/flytekitplugins_papermill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-11 22:07:23.000000 flytekitplugins-papermill-1.8.0/flytekitplugins_papermill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 22:07:23.000000 flytekitplugins-papermill-1.8.0/flytekitplugins_papermill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:23.000000 flytekitplugins-papermill-1.8.0/flytekitplugins_papermill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:23.000000 flytekitplugins-papermill-1.8.0/flytekitplugins_papermill.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 22:07:23.000000 flytekitplugins-papermill-1.8.0/flytekitplugins_papermill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:23.000000 flytekitplugins-papermill-1.8.0/flytekitplugins_papermill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:23.955747 flytekitplugins-papermill-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-11 22:07:11.000000 flytekitplugins-papermill-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:42.179022 flytekitplugins-papermill-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-18 18:01:42.179022 flytekitplugins-papermill-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 18:01:17.000000 flytekitplugins-papermill-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:42.179022 flytekitplugins-papermill-1.8.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:42.179022 flytekitplugins-papermill-1.8.1/flytekitplugins/papermill/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 18:01:17.000000 flytekitplugins-papermill-1.8.1/flytekitplugins/papermill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-07-18 18:01:17.000000 flytekitplugins-papermill-1.8.1/flytekitplugins/papermill/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:42.179022 flytekitplugins-papermill-1.8.1/flytekitplugins_papermill.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-18 18:01:42.000000 flytekitplugins-papermill-1.8.1/flytekitplugins_papermill.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 18:01:42.000000 flytekitplugins-papermill-1.8.1/flytekitplugins_papermill.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:42.000000 flytekitplugins-papermill-1.8.1/flytekitplugins_papermill.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:42.000000 flytekitplugins-papermill-1.8.1/flytekitplugins_papermill.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 18:01:42.000000 flytekitplugins-papermill-1.8.1/flytekitplugins_papermill.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:42.000000 flytekitplugins-papermill-1.8.1/flytekitplugins_papermill.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:42.179022 flytekitplugins-papermill-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-18 18:01:33.000000 flytekitplugins-papermill-1.8.1/setup.py
```

### Comparing `flytekitplugins-papermill-1.8.0/PKG-INFO` & `flytekitplugins-papermill-1.8.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.8.0
+Version: 1.8.1
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.8.0/README.md` & `flytekitplugins-papermill-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.8.0/flytekitplugins/papermill/task.py` & `flytekitplugins-papermill-1.8.1/flytekitplugins/papermill/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.8.0/flytekitplugins_papermill.egg-info/PKG-INFO` & `flytekitplugins-papermill-1.8.1/flytekitplugins_papermill.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.8.0
+Version: 1.8.1
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.8.0/setup.py` & `flytekitplugins-papermill-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit",
     "papermill>=1.2.0",
     "nbconvert>=6.0.7",
     "ipykernel>=5.0.0",
 ]
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is the flytekit papermill plugin",
```

