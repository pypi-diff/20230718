# Comparing `tmp/kn_flatten_json-0.0.8.tar.gz` & `tmp/kn_flatten_json-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kn_flatten_json-0.0.8.tar", last modified: Thu May 25 11:08:31 2023, max compression
+gzip compressed data, was "dist\kn_flatten_json-0.0.9.tar", last modified: Fri May 26 08:01:42 2023, max compression
```

## Comparing `kn_flatten_json-0.0.8.tar` & `kn_flatten_json-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 11:08:31.000000 kn_flatten_json-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-25 11:08:31.000000 kn_flatten_json-0.0.8/kn_flatten_json/
--rw-rw-rw-   0        0        0    10160 2023-05-25 11:08:01.000000 kn_flatten_json-0.0.8/kn_flatten_json/kn_flatten_json.py
--rw-rw-rw-   0        0        0       58 2023-05-22 08:36:10.000000 kn_flatten_json-0.0.8/kn_flatten_json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 11:08:31.000000 kn_flatten_json-0.0.8/kn_flatten_json.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-25 11:08:30.000000 kn_flatten_json-0.0.8/kn_flatten_json.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    10613 2023-05-25 11:08:30.000000 kn_flatten_json-0.0.8/kn_flatten_json.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-25 11:08:30.000000 kn_flatten_json-0.0.8/kn_flatten_json.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2023-05-25 11:08:30.000000 kn_flatten_json-0.0.8/kn_flatten_json.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10613 2023-05-25 11:08:31.000000 kn_flatten_json-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     7614 2023-05-25 08:16:55.000000 kn_flatten_json-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-25 11:08:31.000000 kn_flatten_json-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1006 2023-05-25 08:20:20.000000 kn_flatten_json-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:01:42.000000 kn_flatten_json-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-05-26 08:01:42.000000 kn_flatten_json-0.0.9/kn_flatten_json/
+-rw-rw-rw-   0        0        0    10130 2023-05-25 11:36:10.000000 kn_flatten_json-0.0.9/kn_flatten_json/kn_flatten_json.py
+-rw-rw-rw-   0        0        0       58 2023-05-25 11:36:15.000000 kn_flatten_json-0.0.9/kn_flatten_json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:01:42.000000 kn_flatten_json-0.0.9/kn_flatten_json.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-26 08:01:41.000000 kn_flatten_json-0.0.9/kn_flatten_json.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    10613 2023-05-26 08:01:41.000000 kn_flatten_json-0.0.9/kn_flatten_json.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-26 08:01:41.000000 kn_flatten_json-0.0.9/kn_flatten_json.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       16 2023-05-26 08:01:41.000000 kn_flatten_json-0.0.9/kn_flatten_json.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10613 2023-05-26 08:01:42.000000 kn_flatten_json-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7614 2023-05-25 08:16:55.000000 kn_flatten_json-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 08:01:42.000000 kn_flatten_json-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2023-05-25 11:36:41.000000 kn_flatten_json-0.0.9/setup.py
```

### Comparing `kn_flatten_json-0.0.8/kn_flatten_json/kn_flatten_json.py` & `kn_flatten_json-0.0.9/kn_flatten_json/kn_flatten_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from urllib.parse import urlparse
 import json
 import re
 from pyspark.sql.functions import *
 from pyspark.sql.types import *
 
 
-def flatten_api_valid(spark=None, url=None, method=None, body=None, authToken=None, username=None, password=None,
-                      sep="_"):
+def flatten_api(spark=None, url=None, method=None, body=None, authToken=None, username=None, password=None,sep="_"):
                       
     # replace unwanted characters from columns of api data
     def replace_dots_except_integers(string):
         pattern = r'\b\d+\.\d+\b|\b\d+\b'
 
         dots_within_integers = re.findall(pattern, string)
```

### Comparing `kn_flatten_json-0.0.8/kn_flatten_json.egg-info/PKG-INFO` & `kn_flatten_json-0.0.9/kn_flatten_json.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kn-flatten-json
-Version: 0.0.8
+Version: 0.0.9
 Summary: kn_flatten_json
 Home-page: UNKNOWN
 Author: Sukriti
 Author-email: sukriti.saluja@kockpit.in
 License: UNKNOWN
 Description: # Flatten Nested  API Data/Dataframe with kpt_flatten_json Package
```

### Comparing `kn_flatten_json-0.0.8/PKG-INFO` & `kn_flatten_json-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kn_flatten_json
-Version: 0.0.8
+Version: 0.0.9
 Summary: kn_flatten_json
 Home-page: UNKNOWN
 Author: Sukriti
 Author-email: sukriti.saluja@kockpit.in
 License: UNKNOWN
 Description: # Flatten Nested  API Data/Dataframe with kpt_flatten_json Package
```

### Comparing `kn_flatten_json-0.0.8/README.md` & `kn_flatten_json-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kn_flatten_json-0.0.8/setup.py` & `kn_flatten_json-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 from pathlib import Path
 this_directory = Path(__file__).parent
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'kn_flatten_json'
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
 
 # Setting up
 setup(
     name="kn_flatten_json",
```

