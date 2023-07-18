# Comparing `tmp/resotodata-0.1.0.tar.gz` & `tmp/resotodata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotodata-0.1.0.tar", last modified: Wed Mar 22 15:35:13 2023, max compression
+gzip compressed data, was "resotodata-0.2.0.tar", last modified: Tue Jul 18 17:59:21 2023, max compression
```

## Comparing `resotodata-0.1.0.tar` & `resotodata-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:35:13.413609 resotodata-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-22 15:34:45.000000 resotodata-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-22 15:35:13.413609 resotodata-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-22 15:34:45.000000 resotodata-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:35:13.413609 resotodata-0.1.0/resotodata/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-22 15:34:45.000000 resotodata-0.1.0/resotodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-03-22 15:34:45.000000 resotodata-0.1.0/resotodata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-22 15:34:45.000000 resotodata-0.1.0/resotodata/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-22 15:34:45.000000 resotodata-0.1.0/resotodata/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:35:13.413609 resotodata-0.1.0/resotodata/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-22 15:34:45.000000 resotodata-0.1.0/resotodata/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-03-22 15:34:45.000000 resotodata-0.1.0/resotodata/data/regions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:35:13.413609 resotodata-0.1.0/resotodata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-22 15:35:13.000000 resotodata-0.1.0/resotodata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-22 15:35:13.000000 resotodata-0.1.0/resotodata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 15:35:13.000000 resotodata-0.1.0/resotodata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-22 15:35:13.000000 resotodata-0.1.0/resotodata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 15:35:13.000000 resotodata-0.1.0/resotodata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-22 15:35:13.000000 resotodata-0.1.0/resotodata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 15:35:13.000000 resotodata-0.1.0/resotodata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-22 15:35:13.413609 resotodata-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-22 15:34:45.000000 resotodata-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:35:13.413609 resotodata-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-22 15:34:45.000000 resotodata-0.1.0/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:59:21.714568 resotodata-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 17:58:45.000000 resotodata-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 17:59:21.714568 resotodata-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-18 17:58:45.000000 resotodata-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:59:21.558568 resotodata-0.2.0/resotodata/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12753 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/co2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:59:21.682567 resotodata-0.2.0/resotodata/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/data/ccfdataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123) 101248560 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/data/instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/data/regions.json
+-rw-r--r--   0 runner    (1001) docker     (123) 21240137 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/data/stripped_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-18 17:58:45.000000 resotodata-0.2.0/resotodata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:59:21.558568 resotodata-0.2.0/resotodata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 17:59:21.000000 resotodata-0.2.0/resotodata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-18 17:59:21.000000 resotodata-0.2.0/resotodata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:59:21.000000 resotodata-0.2.0/resotodata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-18 17:59:21.000000 resotodata-0.2.0/resotodata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:59:21.000000 resotodata-0.2.0/resotodata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 17:59:21.000000 resotodata-0.2.0/resotodata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 17:59:21.000000 resotodata-0.2.0/resotodata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 17:59:21.714568 resotodata-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-18 17:58:45.000000 resotodata-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:59:21.714568 resotodata-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 17:58:45.000000 resotodata-0.2.0/test/test_args.py
```

### Comparing `resotodata-0.1.0/PKG-INFO` & `resotodata-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodata
-Version: 0.1.0
+Version: 0.2.0
 Summary: Miscellaneous Resoto data.
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,7 +18,9 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # `resotodata`
 Public Resoto Data
 
 Location data is open data, licensed under the [Open Data Commons Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/) by the [OpenStreetMap Foundation (OSMF)](https://wiki.osmfoundation.org/wiki/Main_Page).
+
+Carbon Emissions data is open source, licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0) by [Cloud Carbon Footprint](https://www.cloudcarbonfootprint.org/).
```

### Comparing `resotodata-0.1.0/resotodata/data/colors.json` & `resotodata-0.2.0/resotodata/data/colors.json`

 * *Files identical despite different names*

### Comparing `resotodata-0.1.0/resotodata/data/regions.json` & `resotodata-0.2.0/resotodata/data/regions.json`

 * *Files identical despite different names*

### Comparing `resotodata-0.1.0/resotodata.egg-info/PKG-INFO` & `resotodata-0.2.0/resotodata.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodata
-Version: 0.1.0
+Version: 0.2.0
 Summary: Miscellaneous Resoto data.
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,7 +18,9 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # `resotodata`
 Public Resoto Data
 
 Location data is open data, licensed under the [Open Data Commons Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/) by the [OpenStreetMap Foundation (OSMF)](https://wiki.osmfoundation.org/wiki/Main_Page).
+
+Carbon Emissions data is open source, licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0) by [Cloud Carbon Footprint](https://www.cloudcarbonfootprint.org/).
```

### Comparing `resotodata-0.1.0/setup.py` & `resotodata-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     packages=find_packages(),
     long_description=readme,
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
             "resotodata-update-regions = resotodata.__main__:update_regions",
             "resotodata-update-colors = resotodata.__main__:update_colors",
+            "resotodata-update-ccfdataset = resotodata.__main__:update_ccfdataset",
+            "resotodata-update-instances = resotodata.__main__:update_instances",
         ]
     },
     include_package_data=True,
     zip_safe=False,
     install_requires=requirements,
     extras_require={"dev": dev_required},
     setup_requires=["pytest-runner"],
```

