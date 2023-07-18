# Comparing `tmp/lexset-4.0.6.tar.gz` & `tmp/lexset-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexset-4.0.6.tar", last modified: Tue Jul 18 19:19:42 2023, max compression
+gzip compressed data, was "lexset-4.0.7.tar", last modified: Tue Jul 18 19:32:56 2023, max compression
```

## Comparing `lexset-4.0.6.tar` & `lexset-4.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:19:42.786081 lexset-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 19:19:42.786081 lexset-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 19:19:25.000000 lexset-4.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:19:42.786081 lexset-4.0.6/lexset/
--rw-r--r--   0 runner    (1001) docker     (123)    30597 2023-07-18 19:19:25.000000 lexset-4.0.6/lexset/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 19:19:25.000000 lexset-4.0.6/lexset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 19:19:25.000000 lexset-4.0.6/lexset/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:19:42.786081 lexset-4.0.6/lexset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:19:42.786081 lexset-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 19:19:25.000000 lexset-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:56.552623 lexset-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 19:32:56.552623 lexset-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 19:32:34.000000 lexset-4.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:56.548623 lexset-4.0.7/lexset/
+-rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-07-18 19:32:34.000000 lexset-4.0.7/lexset/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 19:32:34.000000 lexset-4.0.7/lexset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 19:32:34.000000 lexset-4.0.7/lexset/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:32:56.552623 lexset-4.0.7/lexset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 19:32:56.000000 lexset-4.0.7/lexset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:32:56.552623 lexset-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 19:32:34.000000 lexset-4.0.7/setup.py
```

### Comparing `lexset-4.0.6/lexset/LexsetManager.py` & `lexset-4.0.7/lexset/LexsetManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
 
             response = requests.request("DELETE", url, headers=headers, data=payload)
 
             if response.status_code == 401:
                 print("\33[1;31;40mUnauthorized: " + str(response.status_code) + "\33[0m")
                 return("Unauthorized")
             if response.status_code == 200:
-                print("\n\33[1;32;40mSimulation ID "+ str(self.simulation_id) +" started successfully.\33[0m")
+                print("\n\33[1;32;40mSimulation ID "+ str(self.simulation_id) +" removed from queue.\33[0m")
                 #parseResponse = json.loads(response.text)
                 time.sleep(5)
                 return("success")
             if response.status_code == 400:
                 print("\n\33[1;32;40mSimulation ID "+ str(self.simulation_id) +" not in queue.\33[0m")
                 #parseResponse = json.loads(response.text)
                 time.sleep(5)
```

### Comparing `lexset-4.0.6/lexset/credentials.py` & `lexset-4.0.7/lexset/credentials.py`

 * *Files identical despite different names*

