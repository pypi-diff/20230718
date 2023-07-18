# Comparing `tmp/flytekitplugins-pandera-1.8.0.tar.gz` & `tmp/flytekitplugins-pandera-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-pandera-1.8.0.tar", last modified: Tue Jul 11 22:07:23 2023, max compression
+gzip compressed data, was "flytekitplugins-pandera-1.8.1.tar", last modified: Tue Jul 18 18:01:41 2023, max compression
```

## Comparing `flytekitplugins-pandera-1.8.0.tar` & `flytekitplugins-pandera-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-11 22:06:52.000000 flytekitplugins-pandera-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.411742 flytekitplugins-pandera-1.8.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/flytekitplugins/pandera/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 22:06:52.000000 flytekitplugins-pandera-1.8.0/flytekitplugins/pandera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-11 22:06:52.000000 flytekitplugins-pandera-1.8.0/flytekitplugins/pandera/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-11 22:07:11.000000 flytekitplugins-pandera-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:41.815022 flytekitplugins-pandera-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-18 18:01:41.815022 flytekitplugins-pandera-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-18 18:01:17.000000 flytekitplugins-pandera-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:41.815022 flytekitplugins-pandera-1.8.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:41.815022 flytekitplugins-pandera-1.8.1/flytekitplugins/pandera/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-18 18:01:17.000000 flytekitplugins-pandera-1.8.1/flytekitplugins/pandera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-18 18:01:17.000000 flytekitplugins-pandera-1.8.1/flytekitplugins/pandera/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:41.815022 flytekitplugins-pandera-1.8.1/flytekitplugins_pandera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-18 18:01:41.000000 flytekitplugins-pandera-1.8.1/flytekitplugins_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-18 18:01:41.000000 flytekitplugins-pandera-1.8.1/flytekitplugins_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:41.000000 flytekitplugins-pandera-1.8.1/flytekitplugins_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:41.000000 flytekitplugins-pandera-1.8.1/flytekitplugins_pandera.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 18:01:41.000000 flytekitplugins-pandera-1.8.1/flytekitplugins_pandera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:41.000000 flytekitplugins-pandera-1.8.1/flytekitplugins_pandera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:41.815022 flytekitplugins-pandera-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-18 18:01:33.000000 flytekitplugins-pandera-1.8.1/setup.py
```

### Comparing `flytekitplugins-pandera-1.8.0/PKG-INFO` & `flytekitplugins-pandera-1.8.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pandera
-Version: 1.8.0
+Version: 1.8.1
 Summary: Pandera plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pandera-1.8.0/README.md` & `flytekitplugins-pandera-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pandera-1.8.0/flytekitplugins/pandera/schema.py` & `flytekitplugins-pandera-1.8.1/flytekitplugins/pandera/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/PKG-INFO` & `flytekitplugins-pandera-1.8.1/flytekitplugins_pandera.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pandera
-Version: 1.8.0
+Version: 1.8.1
 Summary: Pandera plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pandera-1.8.0/setup.py` & `flytekitplugins-pandera-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "pandera"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "pandera>=0.7.1"]
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Pandera plugin for flytekit",
```

