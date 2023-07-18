# Comparing `tmp/argovisHelpers-0.0.8.tar.gz` & `tmp/argovisHelpers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argovisHelpers-0.0.8.tar", last modified: Tue Feb 28 04:54:26 2023, max compression
+gzip compressed data, was "argovisHelpers-0.0.9.tar", last modified: Wed Mar 22 16:12:00 2023, max compression
```

## Comparing `argovisHelpers-0.0.8.tar` & `argovisHelpers-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 04:54:26.226850 argovisHelpers-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1051 2022-05-10 16:05:19.000000 argovisHelpers-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2572 2023-02-28 04:54:26.223323 argovisHelpers-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      899 2023-01-12 19:25:14.000000 argovisHelpers-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 04:54:26.115525 argovisHelpers-0.0.8/argovisHelpers/
--rw-r--r--   0 root         (0) root         (0)       22 2022-09-16 00:52:29.000000 argovisHelpers-0.0.8/argovisHelpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5832 2023-02-28 04:16:37.000000 argovisHelpers-0.0.8/argovisHelpers/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 04:54:26.192469 argovisHelpers-0.0.8/argovisHelpers.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2572 2023-02-28 04:54:25.000000 argovisHelpers-0.0.8/argovisHelpers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2023-02-28 04:54:26.000000 argovisHelpers-0.0.8/argovisHelpers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 04:54:25.000000 argovisHelpers-0.0.8/argovisHelpers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-28 04:54:26.000000 argovisHelpers-0.0.8/argovisHelpers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-28 04:54:26.000000 argovisHelpers-0.0.8/argovisHelpers.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      615 2023-02-28 04:53:46.000000 argovisHelpers-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 04:54:26.229966 argovisHelpers-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 04:54:26.208649 argovisHelpers-0.0.8/tests/
--rw-r--r--   0 root         (0) root         (0)     4113 2023-02-15 17:43:39.000000 argovisHelpers-0.0.8/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:12:00.237415 argovisHelpers-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1051 2022-05-10 16:05:19.000000 argovisHelpers-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-03-22 16:12:00.233265 argovisHelpers-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      899 2023-01-12 19:25:14.000000 argovisHelpers-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:12:00.119568 argovisHelpers-0.0.9/argovisHelpers/
+-rw-r--r--   0 root         (0) root         (0)       22 2022-09-16 00:52:29.000000 argovisHelpers-0.0.9/argovisHelpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6264 2023-03-22 12:11:24.000000 argovisHelpers-0.0.9/argovisHelpers/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:12:00.199579 argovisHelpers-0.0.9/argovisHelpers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-03-22 16:11:59.000000 argovisHelpers-0.0.9/argovisHelpers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2023-03-22 16:12:00.000000 argovisHelpers-0.0.9/argovisHelpers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 16:11:59.000000 argovisHelpers-0.0.9/argovisHelpers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-03-22 16:12:00.000000 argovisHelpers-0.0.9/argovisHelpers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-03-22 16:12:00.000000 argovisHelpers-0.0.9/argovisHelpers.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      615 2023-03-22 16:11:35.000000 argovisHelpers-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-22 16:12:00.239331 argovisHelpers-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:12:00.220685 argovisHelpers-0.0.9/tests/
+-rw-r--r--   0 root         (0) root         (0)     4113 2023-03-21 17:56:43.000000 argovisHelpers-0.0.9/tests/tests.py
```

### Comparing `argovisHelpers-0.0.8/LICENSE` & `argovisHelpers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `argovisHelpers-0.0.8/PKG-INFO` & `argovisHelpers-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argovisHelpers
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper functions to consume and parse information from University of Colorado's Argovis API.
 Author: Bill Mills
 License: Copyright (c) 2022 Argovis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `argovisHelpers-0.0.8/README.md` & `argovisHelpers-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `argovisHelpers-0.0.8/argovisHelpers/helpers.py` & `argovisHelpers-0.0.9/argovisHelpers/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,33 @@
 
     o = copy.deepcopy(options)
     for option in ['polygon', 'multipolygon']:
         if option in options:
             options[option] = str(options[option])
 
     dl = requests.get(apiroot + route, params = options, headers={'x-argokey': apikey})
-    #url = dl.url
+    statuscode = dl.status_code
+    print(dl.url)
     dl = dl.json()
 
-    if 'code' in dl and dl['code'] == 429:
+    if statuscode==429:
         # user exceeded API limit, extract suggested wait and delay times, and try again
         wait = dl['delay'][0]
         latency = dl['delay'][1]
         time.sleep(wait*1.1)
         return argofetch(route, options=o, apikey=apikey, apiroot=apiroot, suggestedLatency=latency)
 
-    if 'code' in dl and dl['code'] != 404:
-        raise Exception(str(dl['code']) + ': ' + dl['message'])
+    if statuscode!=404 and statuscode!=200:
+        if statuscode == 413:
+            print('The temporospatial extent of your request is enormous! Consider using the `query` helper in this package to split it up into more manageable chunks.')
+        elif statuscode >= 500:
+            print("Argovis' servers experienced an error. Please try your request again, and email argovis@colorado.edu if this keeps happening; please include the full details of the the request you made so we can help address.")
+        raise Exception(statuscode)
 
-    if ('code' in dl and dl['code']==404) or (type(dl[0]) is dict and 'code' in dl[0] and dl[0]['code']==404):
+    if (statuscode==404) or (type(dl[0]) is dict and 'code' in dl[0] and dl[0]['code']==404):
         return [], suggestedLatency
 
     return dl, suggestedLatency
 
 def query(route, options={}, apikey='', apiroot='https://argovis-api.colorado.edu/'):
     # middleware function between the user and a call to argofetch to make sure individual requests are reasonably scoped and timed.
```

### Comparing `argovisHelpers-0.0.8/argovisHelpers.egg-info/PKG-INFO` & `argovisHelpers-0.0.9/argovisHelpers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argovisHelpers
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper functions to consume and parse information from University of Colorado's Argovis API.
 Author: Bill Mills
 License: Copyright (c) 2022 Argovis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `argovisHelpers-0.0.8/pyproject.toml` & `argovisHelpers-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "argovisHelpers"
-version = "0.0.8"
+version = "0.0.9"
 description = "Helper functions to consume and parse information from University of Colorado's Argovis API."
 readme = "README.md"
 authors = [{name = "Bill Mills" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `argovisHelpers-0.0.8/tests/tests.py` & `argovisHelpers-0.0.9/tests/tests.py`

 * *Files identical despite different names*

