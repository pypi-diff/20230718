# Comparing `tmp/lexsetAPI-3.4.5.tar.gz` & `tmp/lexsetAPI-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexsetAPI-3.4.5.tar", last modified: Tue Jul 18 18:11:11 2023, max compression
+gzip compressed data, was "lexsetAPI-3.4.6.tar", last modified: Tue Jul 18 18:15:02 2023, max compression
```

## Comparing `lexsetAPI-3.4.5.tar` & `lexsetAPI-3.4.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:11:11.669227 lexsetAPI-3.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 18:11:11.669227 lexsetAPI-3.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-18 18:10:51.000000 lexsetAPI-3.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:11:11.669227 lexsetAPI-3.4.5/lexsetAPI/
--rw-r--r--   0 runner    (1001) docker     (123)    27298 2023-07-18 18:10:51.000000 lexsetAPI-3.4.5/lexsetAPI/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 18:10:51.000000 lexsetAPI-3.4.5/lexsetAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 18:10:51.000000 lexsetAPI-3.4.5/lexsetAPI/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:11:11.669227 lexsetAPI-3.4.5/lexsetAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 18:11:11.000000 lexsetAPI-3.4.5/lexsetAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-18 18:11:11.000000 lexsetAPI-3.4.5/lexsetAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:11:11.000000 lexsetAPI-3.4.5/lexsetAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 18:11:11.000000 lexsetAPI-3.4.5/lexsetAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 18:11:11.000000 lexsetAPI-3.4.5/lexsetAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:11:11.669227 lexsetAPI-3.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 18:10:51.000000 lexsetAPI-3.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:15:02.264073 lexsetAPI-3.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 18:15:02.264073 lexsetAPI-3.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-18 18:14:45.000000 lexsetAPI-3.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:15:02.264073 lexsetAPI-3.4.6/lexsetAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)    27300 2023-07-18 18:14:45.000000 lexsetAPI-3.4.6/lexsetAPI/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 18:14:45.000000 lexsetAPI-3.4.6/lexsetAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 18:14:45.000000 lexsetAPI-3.4.6/lexsetAPI/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:15:02.264073 lexsetAPI-3.4.6/lexsetAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 18:15:02.000000 lexsetAPI-3.4.6/lexsetAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-18 18:15:02.000000 lexsetAPI-3.4.6/lexsetAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:15:02.000000 lexsetAPI-3.4.6/lexsetAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 18:15:02.000000 lexsetAPI-3.4.6/lexsetAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 18:15:02.000000 lexsetAPI-3.4.6/lexsetAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:15:02.264073 lexsetAPI-3.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 18:14:45.000000 lexsetAPI-3.4.6/setup.py
```

### Comparing `lexsetAPI-3.4.5/lexsetAPI/LexsetManager.py` & `lexsetAPI-3.4.6/lexsetAPI/LexsetManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         #parseResponse = json.loads(response.text)
         return("success")
     else:
         print("Error: " + str(getCode))
         return(getCode)
 
 def start(simulationID,token):
-    url = "https://lexsetapi.azurewebsites.net/api/Simulations/QueueSimulation=id" + str(simulationID)
+    url = "https://lexsetapi.azurewebsites.net/api/Simulations/QueueSimulation?id=" + str(simulationID)
 
     payload={}
     headers = {
     'Authorization': 'Bearer ' + token
     }
 
     response = requests.request("POST", url, headers=headers, data=payload)
@@ -741,15 +741,15 @@
     response = requests.delete(f'https://lexsetapi.lexset.ai/api/simulations/archivesimulation?id={id}', headers=headers)
     if response.status_code == 200:
         print("Simulation successfully deleted.")
     else:
         print(f"Error deleting simulation: {response.text}")
 
 def dequeue(simulationID,token):
-    url = "https://lexsetapi.azurewebsites.net/api/Simulations/RemoveSimulationFromQueue=id" + str(simulationID)
+    url = "https://lexsetapi.azurewebsites.net/api/Simulations/RemoveSimulationFromQueue?id=" + str(simulationID)
 
     payload={}
     headers = {
     'Authorization': 'Bearer ' + token
     }
 
     response = requests.request("DELETE", url, headers=headers, data=payload)
```

### Comparing `lexsetAPI-3.4.5/lexsetAPI/credentials.py` & `lexsetAPI-3.4.6/lexsetAPI/credentials.py`

 * *Files identical despite different names*

