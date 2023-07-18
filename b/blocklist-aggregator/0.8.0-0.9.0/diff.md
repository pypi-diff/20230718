# Comparing `tmp/blocklist_aggregator-0.8.0.tar.gz` & `tmp/blocklist_aggregator-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blocklist_aggregator-0.8.0.tar", last modified: Mon Sep 12 18:33:34 2022, max compression
+gzip compressed data, was "blocklist_aggregator-0.9.0.tar", last modified: Tue Jul 18 06:31:04 2023, max compression
```

## Comparing `blocklist_aggregator-0.8.0.tar` & `blocklist_aggregator-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-09-12 18:33:34.160976 blocklist_aggregator-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-09-12 18:33:22.000000 blocklist_aggregator-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       43 2022-09-12 18:33:22.000000 blocklist_aggregator-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3503 2022-09-12 18:33:34.160976 blocklist_aggregator-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2944 2022-09-12 18:33:22.000000 blocklist_aggregator-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-09-12 18:33:34.156976 blocklist_aggregator-0.8.0/blocklist_aggregator/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2022-09-12 18:33:22.000000 blocklist_aggregator-0.8.0/blocklist_aggregator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4438 2022-09-12 18:33:22.000000 blocklist_aggregator-0.8.0/blocklist_aggregator/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1842 2022-09-12 18:33:22.000000 blocklist_aggregator-0.8.0/blocklist_aggregator/blocklist.conf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-09-12 18:33:34.160976 blocklist_aggregator-0.8.0/blocklist_aggregator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3503 2022-09-12 18:33:34.000000 blocklist_aggregator-0.8.0/blocklist_aggregator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      361 2022-09-12 18:33:34.000000 blocklist_aggregator-0.8.0/blocklist_aggregator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-09-12 18:33:34.000000 blocklist_aggregator-0.8.0/blocklist_aggregator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-09-12 18:33:34.000000 blocklist_aggregator-0.8.0/blocklist_aggregator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2022-09-12 18:33:34.000000 blocklist_aggregator-0.8.0/blocklist_aggregator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-09-12 18:33:34.160976 blocklist_aggregator-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      942 2022-09-12 18:33:33.000000 blocklist_aggregator-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:31:04.199504 blocklist_aggregator-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 06:30:48.000000 blocklist_aggregator-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-18 06:30:48.000000 blocklist_aggregator-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-18 06:31:04.199504 blocklist_aggregator-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-18 06:30:48.000000 blocklist_aggregator-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:31:04.195503 blocklist_aggregator-0.9.0/blocklist_aggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-18 06:30:48.000000 blocklist_aggregator-0.9.0/blocklist_aggregator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-18 06:30:48.000000 blocklist_aggregator-0.9.0/blocklist_aggregator/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-18 06:30:48.000000 blocklist_aggregator-0.9.0/blocklist_aggregator/blocklist.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:31:04.199504 blocklist_aggregator-0.9.0/blocklist_aggregator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-18 06:31:04.000000 blocklist_aggregator-0.9.0/blocklist_aggregator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-18 06:31:04.000000 blocklist_aggregator-0.9.0/blocklist_aggregator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:31:04.000000 blocklist_aggregator-0.9.0/blocklist_aggregator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 06:31:04.000000 blocklist_aggregator-0.9.0/blocklist_aggregator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 06:31:04.000000 blocklist_aggregator-0.9.0/blocklist_aggregator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:31:04.199504 blocklist_aggregator-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-18 06:31:03.000000 blocklist_aggregator-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:31:04.199504 blocklist_aggregator-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-18 06:30:48.000000 blocklist_aggregator-0.9.0/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-18 06:30:48.000000 blocklist_aggregator-0.9.0/tests/test_save.py
```

### Comparing `blocklist_aggregator-0.8.0/LICENSE` & `blocklist_aggregator-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blocklist_aggregator-0.8.0/PKG-INFO` & `blocklist_aggregator-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blocklist_aggregator
-Version: 0.8.0
+Version: 0.9.0
 Summary: Domains blocklist aggregator
 Home-page: https://github.com/dmachard/blocklist-aggregator
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: blocklist aggregator domains dns blacklist whitelist
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `blocklist_aggregator-0.8.0/README.md` & `blocklist_aggregator-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `blocklist_aggregator-0.8.0/blocklist_aggregator/aggregator.py` & `blocklist_aggregator-0.9.0/blocklist_aggregator/aggregator.py`

 * *Files identical despite different names*

### Comparing `blocklist_aggregator-0.8.0/blocklist_aggregator/blocklist.conf` & `blocklist_aggregator-0.9.0/blocklist_aggregator/blocklist.conf`

 * *Files identical despite different names*

### Comparing `blocklist_aggregator-0.8.0/blocklist_aggregator.egg-info/PKG-INFO` & `blocklist_aggregator-0.9.0/blocklist_aggregator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blocklist-aggregator
-Version: 0.8.0
+Version: 0.9.0
 Summary: Domains blocklist aggregator
 Home-page: https://github.com/dmachard/blocklist-aggregator
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: blocklist aggregator domains dns blacklist whitelist
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `blocklist_aggregator-0.8.0/setup.py` & `blocklist_aggregator-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
     
 KEYWORDS = ('blocklist aggregator domains dns blacklist whitelist')
 
 setuptools.setup(
     name="blocklist_aggregator",
-    version="0.8.0",
+    version="0.9.0",
     author="Denis MACHARD",
     author_email="d.machard@gmail.com",
     description="Domains blocklist aggregator",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/dmachard/blocklist-aggregator",
     packages=['blocklist_aggregator'],
```

