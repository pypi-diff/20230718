# Comparing `tmp/locust-grasshopper-1.3.3.tar.gz` & `tmp/locust-grasshopper-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust-grasshopper-1.3.3.tar", last modified: Thu Jun  1 18:58:07 2023, max compression
+gzip compressed data, was "locust-grasshopper-1.3.4.tar", last modified: Tue Jul 18 16:25:34 2023, max compression
```

## Comparing `locust-grasshopper-1.3.3.tar` & `locust-grasshopper-1.3.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.179099 locust-grasshopper-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35142 2023-06-01 18:58:07.179099 locust-grasshopper-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    21193 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-01 18:57:52.000000 locust-grasshopper-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 18:58:07.179099 locust-grasshopper-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.175099 locust-grasshopper-1.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.175099 locust-grasshopper-1.3.3/src/grasshopper/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.175099 locust-grasshopper-1.3.3/src/grasshopper/lib/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.175099 locust-grasshopper-1.3.3/src/grasshopper/lib/configuration/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/configuration/gh_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.175099 locust-grasshopper-1.3.3/src/grasshopper/lib/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)    19255 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      870 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/fixtures/grasshopper_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/grasshopper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.175099 locust-grasshopper-1.3.3/src/grasshopper/lib/journeys/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/journeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7769 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/journeys/base_journey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.179099 locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/er_basic_console_reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/iextendedreporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/reporter_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/shared_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.179099 locust-grasshopper-1.3.3/src/grasshopper/lib/util/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      330 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/util/check_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/util/launch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/util/listeners.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/util/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/util/shapes.py
--rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-06-01 18:57:48.000000 locust-grasshopper-1.3.3/src/grasshopper/lib/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 18:58:07.179099 locust-grasshopper-1.3.3/src/locust_grasshopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    35142 2023-06-01 18:58:07.000000 locust-grasshopper-1.3.3/src/locust_grasshopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-06-01 18:58:07.000000 locust-grasshopper-1.3.3/src/locust_grasshopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 18:58:07.000000 locust-grasshopper-1.3.3/src/locust_grasshopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-01 18:58:07.000000 locust-grasshopper-1.3.3/src/locust_grasshopper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-01 18:58:07.000000 locust-grasshopper-1.3.3/src/locust_grasshopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-01 18:58:07.000000 locust-grasshopper-1.3.3/src/locust_grasshopper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.454905 locust-grasshopper-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35142 2023-07-18 16:25:34.454905 locust-grasshopper-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21193 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-07-18 16:25:19.000000 locust-grasshopper-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 16:25:34.454905 locust-grasshopper-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.450904 locust-grasshopper-1.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.450904 locust-grasshopper-1.3.4/src/grasshopper/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.450904 locust-grasshopper-1.3.4/src/grasshopper/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.450904 locust-grasshopper-1.3.4/src/grasshopper/lib/configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/configuration/gh_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.450904 locust-grasshopper-1.3.4/src/grasshopper/lib/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)    19255 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      870 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/fixtures/grasshopper_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/grasshopper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.454905 locust-grasshopper-1.3.4/src/grasshopper/lib/journeys/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/journeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7769 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/journeys/base_journey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.454905 locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/er_basic_console_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/iextendedreporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/reporter_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/shared_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.454905 locust-grasshopper-1.3.4/src/grasshopper/lib/util/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      330 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/util/check_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/util/launch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/util/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/util/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/util/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-07-18 16:25:16.000000 locust-grasshopper-1.3.4/src/grasshopper/lib/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 16:25:34.454905 locust-grasshopper-1.3.4/src/locust_grasshopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    35142 2023-07-18 16:25:34.000000 locust-grasshopper-1.3.4/src/locust_grasshopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-07-18 16:25:34.000000 locust-grasshopper-1.3.4/src/locust_grasshopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 16:25:34.000000 locust-grasshopper-1.3.4/src/locust_grasshopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-18 16:25:34.000000 locust-grasshopper-1.3.4/src/locust_grasshopper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-18 16:25:34.000000 locust-grasshopper-1.3.4/src/locust_grasshopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-18 16:25:34.000000 locust-grasshopper-1.3.4/src/locust_grasshopper.egg-info/top_level.txt
```

### Comparing `locust-grasshopper-1.3.3/LICENSE` & `locust-grasshopper-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/PKG-INFO` & `locust-grasshopper-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.3.3
+Version: 1.3.4
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `locust-grasshopper-1.3.3/README.md` & `locust-grasshopper-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/pyproject.toml` & `locust-grasshopper-1.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "cmake>=3.11.0,<4.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "locust-grasshopper"
-version = "1.3.3" # Managed by bump2version
+version = "1.3.4" # Managed by bump2version
 readme = {file = "README.md", content-type = "text/markdown"}
 description = "a load testing tool extended from locust"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
@@ -32,15 +32,15 @@
 dependencies = [
     "gevent ~=21.12.0",
     "influxdb ~= 5.3.1",
     "locust ~= 2.12.2",
     "locust-influxdb-listener ~= 0.0.9",
     "pytest ~= 6.2.5",
     "termcolor ~= 1.1.0",
-    "pyyaml ~= 5.4",
+    "pyyaml ~= 5.3.1",
     "tag-matcher ~= 0.0.5"
 ]
 
 [project.urls]
 "repository" = "https://github.com/alteryx/locust-grasshopper"
 
 [tool.setuptools.packages.find]
```

### Comparing `locust-grasshopper-1.3.3/setup.py` & `locust-grasshopper-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/configuration/gh_configuration.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/configuration/gh_configuration.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/fixtures/__init__.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/fixtures/grasshopper_constants.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/fixtures/grasshopper_constants.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/grasshopper.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/grasshopper.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/journeys/base_journey.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/journeys/base_journey.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/er_basic_console_reporter.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/er_basic_console_reporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/iextendedreporter.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/iextendedreporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/reporter_extensions.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/reporter_extensions.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/reporting/shared_reporting.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/reporting/shared_reporting.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/util/decorators.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/util/decorators.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/util/launch.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/util/launch.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/util/listeners.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/util/listeners.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/util/metrics.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/util/metrics.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/util/shapes.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/util/shapes.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/grasshopper/lib/util/utils.py` & `locust-grasshopper-1.3.4/src/grasshopper/lib/util/utils.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.3.3/src/locust_grasshopper.egg-info/PKG-INFO` & `locust-grasshopper-1.3.4/src/locust_grasshopper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.3.3
+Version: 1.3.4
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `locust-grasshopper-1.3.3/src/locust_grasshopper.egg-info/SOURCES.txt` & `locust-grasshopper-1.3.4/src/locust_grasshopper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

