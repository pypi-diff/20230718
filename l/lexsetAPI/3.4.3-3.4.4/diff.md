# Comparing `tmp/lexsetAPI-3.4.3.tar.gz` & `tmp/lexsetAPI-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexsetAPI-3.4.3.tar", last modified: Tue Jul 18 16:59:50 2023, max compression
+gzip compressed data, was "lexsetAPI-3.4.4.tar", last modified: Tue Jul 18 17:24:50 2023, max compression
```

## Comparing `lexsetAPI-3.4.3.tar` & `lexsetAPI-3.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/lexsetAPI/
--rw-r--r--   0 runner    (1001) docker     (123)    27292 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/lexsetAPI/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/lexsetAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/lexsetAPI/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/lexsetAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:24:50.949558 lexsetAPI-3.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 17:24:50.945558 lexsetAPI-3.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-18 17:24:33.000000 lexsetAPI-3.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:24:50.945558 lexsetAPI-3.4.4/lexsetAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)    27294 2023-07-18 17:24:33.000000 lexsetAPI-3.4.4/lexsetAPI/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 17:24:33.000000 lexsetAPI-3.4.4/lexsetAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 17:24:33.000000 lexsetAPI-3.4.4/lexsetAPI/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:24:50.945558 lexsetAPI-3.4.4/lexsetAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 17:24:50.000000 lexsetAPI-3.4.4/lexsetAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-18 17:24:50.000000 lexsetAPI-3.4.4/lexsetAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:24:50.000000 lexsetAPI-3.4.4/lexsetAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 17:24:50.000000 lexsetAPI-3.4.4/lexsetAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 17:24:50.000000 lexsetAPI-3.4.4/lexsetAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:24:50.949558 lexsetAPI-3.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 17:24:33.000000 lexsetAPI-3.4.4/setup.py
```

### Comparing `lexsetAPI-3.4.3/lexsetAPI/LexsetManager.py` & `lexsetAPI-3.4.4/lexsetAPI/LexsetManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -748,15 +748,15 @@
     url = "https://lexsetapi.azurewebsites.net/api/Simulations/RemoveSimulationFromQueue=" + str(simulationID)
 
     payload={}
     headers = {
     'Authorization': 'Bearer ' + token
     }
 
-    response = requests.request("POST", url, headers=headers, data=payload)
+    response = requests.request("DELETE", url, headers=headers, data=payload)
     
     getCode = response.status_code
     if getCode == 401:
         return("Unauthorized")
     if getCode == 200:
         #parseResponse = json.loads(response.text)
         return("success")
```

### Comparing `lexsetAPI-3.4.3/lexsetAPI/credentials.py` & `lexsetAPI-3.4.4/lexsetAPI/credentials.py`

 * *Files identical despite different names*

