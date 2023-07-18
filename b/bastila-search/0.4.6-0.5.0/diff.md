# Comparing `tmp/bastila_search-0.4.6.tar.gz` & `tmp/bastila_search-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastila_search-0.4.6.tar", last modified: Fri Jul 14 19:42:45 2023, max compression
+gzip compressed data, was "bastila_search-0.5.0.tar", last modified: Mon Jul 17 23:59:16 2023, max compression
```

## Comparing `bastila_search-0.4.6.tar` & `bastila_search-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:42:45.723913 bastila_search-0.4.6/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.4.6/LICENSE
--rw-rw-r--   0 joe       (1000) joe       (1000)     1103 2023-07-14 19:42:45.723913 bastila_search-0.4.6/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      775 2023-07-14 19:30:52.000000 bastila_search-0.4.6/README.md
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:42:45.723913 bastila_search-0.4.6/bastila_search/
--rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.4.6/bastila_search/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     5331 2023-07-14 19:42:22.000000 bastila_search-0.4.6/bastila_search/bastila_search.py
--rw-rw-r--   0 joe       (1000) joe       (1000)      444 2023-07-14 19:12:46.000000 bastila_search-0.4.6/bastila_search/setup_config.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-14 19:42:45.723913 bastila_search-0.4.6/bastila_search.egg-info/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1103 2023-07-14 19:42:45.000000 bastila_search-0.4.6/bastila_search.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      384 2023-07-14 19:42:45.000000 bastila_search-0.4.6/bastila_search.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-14 19:42:45.000000 bastila_search-0.4.6/bastila_search.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)      116 2023-07-14 19:42:45.000000 bastila_search-0.4.6/bastila_search.egg-info/entry_points.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.4.6/bastila_search.egg-info/not-zip-safe
--rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-14 19:42:45.000000 bastila_search-0.4.6/bastila_search.egg-info/requires.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-14 19:42:45.000000 bastila_search-0.4.6/bastila_search.egg-info/top_level.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-14 19:42:45.723913 bastila_search-0.4.6/setup.cfg
--rw-rw-r--   0 joe       (1000) joe       (1000)      789 2023-07-14 19:42:29.000000 bastila_search-0.4.6/setup.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-17 23:59:16.518382 bastila_search-0.5.0/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.5.0/LICENSE
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1103 2023-07-17 23:59:16.518382 bastila_search-0.5.0/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      775 2023-07-14 19:30:52.000000 bastila_search-0.5.0/README.md
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-17 23:59:16.518382 bastila_search-0.5.0/bastila_search/
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.5.0/bastila_search/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     4418 2023-07-17 23:57:20.000000 bastila_search-0.5.0/bastila_search/bastila_search.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)      444 2023-07-14 19:12:46.000000 bastila_search-0.5.0/bastila_search/setup_config.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-17 23:59:16.518382 bastila_search-0.5.0/bastila_search.egg-info/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1103 2023-07-17 23:59:16.000000 bastila_search-0.5.0/bastila_search.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      384 2023-07-17 23:59:16.000000 bastila_search-0.5.0/bastila_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-17 23:59:16.000000 bastila_search-0.5.0/bastila_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)      116 2023-07-17 23:59:16.000000 bastila_search-0.5.0/bastila_search.egg-info/entry_points.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.5.0/bastila_search.egg-info/not-zip-safe
+-rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-17 23:59:16.000000 bastila_search-0.5.0/bastila_search.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-17 23:59:16.000000 bastila_search-0.5.0/bastila_search.egg-info/top_level.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-17 23:59:16.518382 bastila_search-0.5.0/setup.cfg
+-rw-rw-r--   0 joe       (1000) joe       (1000)      789 2023-07-17 23:59:06.000000 bastila_search-0.5.0/setup.py
```

### Comparing `bastila_search-0.4.6/LICENSE` & `bastila_search-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bastila_search-0.4.6/PKG-INFO` & `bastila_search-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastila_search
-Version: 0.4.6
+Version: 0.5.0
 Summary: A python script that catches commits that introduce predefined deprecated patterns
 Home-page: https://github.com/GetBastila/bastila-hook
 Author: Bastila
 Author-email: hello@bastila.app
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bastila_search-0.4.6/README.md` & `bastila_search-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bastila_search-0.4.6/bastila_search/bastila_search.py` & `bastila_search-0.5.0/bastila_search/bastila_search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import requests
 import json
 import re
 import sys
-import os
 import fnmatch
 
 from pathlib import Path
 
 base_url = 'https://bastila.dev'
 
 
@@ -14,20 +13,14 @@
     try:
         with open("config.json", "r") as file:
             return json.load(file)
     except FileNotFoundError:
         return None
 
 
-def handle_exception(error, prevent_regression):
-    print(error)
-    if prevent_regression:
-        sys.exit(1)
-
-
 def fetch_patterns(session):
     response = session.get(f'{base_url}/api/check/standard-changes/')
     response.raise_for_status()
     standards = response.json()
 
     return standards['results']
 
@@ -111,63 +104,49 @@
     response.raise_for_status()
     return response.json()
 
 
 def main():
     config = load_config()
 
-    BASTILA_KEY = os.getenv("BASTILA_KEY", None)
-    POST_RESULTS = os.getenv('POST_RESULTS', 'false').lower() == 'true'
-    PREVENT_REGRESSION = os.getenv("PREVENT_REGRESSION", 'false').lower() == 'true'
-
-    if config is None and BASTILA_KEY is None:
-        print("Configuration not found. Please run the command bastila_setup or setup an environment file to set up the necessary parameters.")
-        handle_exception('Configuration not setup', PREVENT_REGRESSION)
-    elif config is not None:
+    if config is None:
+        print("Configuration not found. Please run the command bastila_setup to set up the necessary parameters.")
+        sys.exit(1)
+    else:
         BASTILA_KEY = config["BASTILA_KEY"]
         PREVENT_REGRESSION = config["PREVENT_REGRESSION"]
 
     session = requests.Session()
     session.headers.update({
         'Authorization': f'Api-Key {BASTILA_KEY}',
         'Content-Type': 'application/json'
     })
     print('Starting Bastila Search')
 
     try:
         print('Starting check')
-        check = create_check(session)
+        create_check(session)
     except Exception as e:
-        print('Create check failed')
-        handle_exception(e, PREVENT_REGRESSION)
+        print(e)
+        sys.exit(1)
 
     try:
         print('Fetching patterns')
         patterns = fetch_patterns(session)
     except Exception as e:
-        print('Fetch patterns failed')
-        handle_exception(e, PREVENT_REGRESSION)
+        print(e)
+        sys.exit(1)
 
+    results = []
     try:
         print('Searching files')
         results = search_files(patterns)
     except Exception as e:
-        print('Fetch patterns failed')
-        handle_exception(e, PREVENT_REGRESSION)
-
-    if POST_RESULTS:
-        try:
-            print('Posting results')
-            post_results(session, {
-              'check': check['id'],
-              'results': results
-            })
-        except Exception as e:
-            print('Posting results failed')
-            handle_exception(e, PREVENT_REGRESSION)
+        print(e)
+        sys.exit(1)
 
     is_regression = False
     for result in results:
         if not result['is_successful']:
             print(result['fix_recommendation'])
             is_regression = True
```

### Comparing `bastila_search-0.4.6/bastila_search.egg-info/PKG-INFO` & `bastila_search-0.5.0/bastila_search.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastila-search
-Version: 0.4.6
+Version: 0.5.0
 Summary: A python script that catches commits that introduce predefined deprecated patterns
 Home-page: https://github.com/GetBastila/bastila-hook
 Author: Bastila
 Author-email: hello@bastila.app
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bastila_search-0.4.6/setup.py` & `bastila_search-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='bastila_search',
-    version='0.4.6',
+    version='0.5.0',
     description='A python script that catches commits that introduce predefined deprecated patterns',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/GetBastila/bastila-hook',
     author='Bastila',
     author_email='hello@bastila.app',
     license='MIT',
```

