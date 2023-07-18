# Comparing `tmp/parrottools-0.2.8.tar.gz` & `tmp/parrottools-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parrottools-0.2.8.tar", last modified: Fri Sep 23 12:29:27 2022, max compression
+gzip compressed data, was "parrottools-0.2.9.tar", last modified: Mon Mar 27 14:41:26 2023, max compression
```

## Comparing `parrottools-0.2.8.tar` & `parrottools-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 12:29:27.172308 parrottools-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (116)      902 2022-09-23 12:29:27.172308 parrottools-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      265 2022-09-23 12:29:13.000000 parrottools-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      221 2022-09-23 12:29:13.000000 parrottools-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-09-23 12:29:27.172308 parrottools-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1524 2022-09-23 12:29:13.000000 parrottools-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 12:29:27.164308 parrottools-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 12:29:27.168308 parrottools-0.2.8/src/parrottools/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-23 12:29:13.000000 parrottools-0.2.8/src/parrottools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       48 2022-09-23 12:29:13.000000 parrottools-0.2.8/src/parrottools/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 12:29:27.172308 parrottools-0.2.8/src/parrottools/events/
--rw-r--r--   0 runner    (1001) docker     (116)      125 2022-09-23 12:29:13.000000 parrottools-0.2.8/src/parrottools/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2655 2022-09-23 12:29:13.000000 parrottools-0.2.8/src/parrottools/events/publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 12:29:27.172308 parrottools-0.2.8/src/parrottools/logging/
--rw-r--r--   0 runner    (1001) docker     (116)      289 2022-09-23 12:29:13.000000 parrottools-0.2.8/src/parrottools/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7773 2022-09-23 12:29:13.000000 parrottools-0.2.8/src/parrottools/logging/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-23 12:29:27.172308 parrottools-0.2.8/src/parrottools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      902 2022-09-23 12:29:27.000000 parrottools-0.2.8/src/parrottools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      430 2022-09-23 12:29:27.000000 parrottools-0.2.8/src/parrottools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-23 12:29:27.000000 parrottools-0.2.8/src/parrottools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      210 2022-09-23 12:29:27.000000 parrottools-0.2.8/src/parrottools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-09-23 12:29:27.000000 parrottools-0.2.8/src/parrottools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 14:41:26.851249 parrottools-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      902 2023-03-27 14:41:26.851249 parrottools-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      265 2023-03-27 14:41:18.000000 parrottools-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      261 2023-03-27 14:41:18.000000 parrottools-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-27 14:41:26.851249 parrottools-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1524 2023-03-27 14:41:18.000000 parrottools-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 14:41:26.843249 parrottools-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 14:41:26.847249 parrottools-0.2.9/src/parrottools/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-27 14:41:18.000000 parrottools-0.2.9/src/parrottools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       48 2023-03-27 14:41:18.000000 parrottools-0.2.9/src/parrottools/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 14:41:26.851249 parrottools-0.2.9/src/parrottools/events/
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2023-03-27 14:41:18.000000 parrottools-0.2.9/src/parrottools/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2655 2023-03-27 14:41:18.000000 parrottools-0.2.9/src/parrottools/events/publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 14:41:26.851249 parrottools-0.2.9/src/parrottools/logging/
+-rw-r--r--   0 runner    (1001) docker     (116)      289 2023-03-27 14:41:18.000000 parrottools-0.2.9/src/parrottools/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7772 2023-03-27 14:41:18.000000 parrottools-0.2.9/src/parrottools/logging/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-27 14:41:26.847249 parrottools-0.2.9/src/parrottools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      902 2023-03-27 14:41:26.000000 parrottools-0.2.9/src/parrottools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2023-03-27 14:41:26.000000 parrottools-0.2.9/src/parrottools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-27 14:41:26.000000 parrottools-0.2.9/src/parrottools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      210 2023-03-27 14:41:26.000000 parrottools-0.2.9/src/parrottools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2023-03-27 14:41:26.000000 parrottools-0.2.9/src/parrottools.egg-info/top_level.txt
```

### Comparing `parrottools-0.2.8/PKG-INFO` & `parrottools-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parrottools
-Version: 0.2.8
+Version: 0.2.9
 Summary: Collection of common utilities.
 Home-page: https://github.com/parrot-com/parrottools
 Author: Parrot
 Maintainer: Parrot
 Project-URL: Source Code, https://github.com/parrot-com/parrottools
 Keywords: observability,logging
 Classifier: Programming Language :: Python :: 3
```

### Comparing `parrottools-0.2.8/setup.py` & `parrottools-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `parrottools-0.2.8/src/parrottools/events/publisher.py` & `parrottools-0.2.9/src/parrottools/events/publisher.py`

 * *Files identical despite different names*

### Comparing `parrottools-0.2.8/src/parrottools/logging/configure.py` & `parrottools-0.2.9/src/parrottools/logging/configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     def __init__(
         self,
         service_name: Optional[str] = None,
         service_version: Optional[str] = None,
         deployment_env: Optional[str] = None,
         sentry_enabled: bool = False,
     ) -> None:
-
         # Application can specify this parameters when configuring the module.
         # If not present, fallback to environment variables that should be present from
         # Kubernetes deployment downward API from deployment metadata.
         if service_name is None:
             service_name = os.environ.get("DEPLOYMENT_NAME", f"unknown_service:{__file__}")
         if service_version is None:
             service_version = os.environ.get("DEPLOYMENT_VERSION", None)
```

### Comparing `parrottools-0.2.8/src/parrottools.egg-info/PKG-INFO` & `parrottools-0.2.9/src/parrottools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parrottools
-Version: 0.2.8
+Version: 0.2.9
 Summary: Collection of common utilities.
 Home-page: https://github.com/parrot-com/parrottools
 Author: Parrot
 Maintainer: Parrot
 Project-URL: Source Code, https://github.com/parrot-com/parrottools
 Keywords: observability,logging
 Classifier: Programming Language :: Python :: 3
```

