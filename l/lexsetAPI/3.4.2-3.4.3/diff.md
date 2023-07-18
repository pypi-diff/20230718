# Comparing `tmp/lexsetAPI-3.4.2.tar.gz` & `tmp/lexsetAPI-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexsetAPI-3.4.2.tar", last modified: Fri Feb  3 21:45:22 2023, max compression
+gzip compressed data, was "lexsetAPI-3.4.3.tar", last modified: Tue Jul 18 16:59:50 2023, max compression
```

## Comparing `lexsetAPI-3.4.2.tar` & `lexsetAPI-3.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 21:45:22.569507 lexsetAPI-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-03 21:45:22.569507 lexsetAPI-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-03 21:45:06.000000 lexsetAPI-3.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 21:45:22.569507 lexsetAPI-3.4.2/lexsetAPI/
--rw-r--r--   0 runner    (1001) docker     (123)    26568 2023-02-03 21:45:06.000000 lexsetAPI-3.4.2/lexsetAPI/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-03 21:45:06.000000 lexsetAPI-3.4.2/lexsetAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-03 21:45:06.000000 lexsetAPI-3.4.2/lexsetAPI/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 21:45:22.569507 lexsetAPI-3.4.2/lexsetAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-03 21:45:22.000000 lexsetAPI-3.4.2/lexsetAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-03 21:45:22.000000 lexsetAPI-3.4.2/lexsetAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 21:45:22.000000 lexsetAPI-3.4.2/lexsetAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-03 21:45:22.000000 lexsetAPI-3.4.2/lexsetAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-03 21:45:22.000000 lexsetAPI-3.4.2/lexsetAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 21:45:22.569507 lexsetAPI-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-02-03 21:45:06.000000 lexsetAPI-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/lexsetAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)    27292 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/lexsetAPI/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/lexsetAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/lexsetAPI/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/lexsetAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 16:59:50.000000 lexsetAPI-3.4.3/lexsetAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 16:59:50.422264 lexsetAPI-3.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 16:59:33.000000 lexsetAPI-3.4.3/setup.py
```

### Comparing `lexsetAPI-3.4.2/lexsetAPI/LexsetManager.py` & `lexsetAPI-3.4.3/lexsetAPI/LexsetManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         #update simulation IDs
         self.simID = parseResponse["id"]
         self.dataID = parseResponse["datasetid"]
         self.userID = parseResponse["userid"]
 
     def startSimulation(self):
-        url = "https://lexsetapi.azurewebsites.net/api/Simulations/StartSimulation?id=" + str(self.simID)
+        url = "https://lexsetapi.azurewebsites.net/api/Simulations/QueueSimulation?id=" + str(self.simID)
 
         payload={}
         headers = {
         'Authorization': 'Bearer ' + self.token
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
@@ -270,15 +270,15 @@
         #parseResponse = json.loads(response.text)
         return("success")
     else:
         print("Error: " + str(getCode))
         return(getCode)
 
 def start(simulationID,token):
-    url = "https://lexsetapi.azurewebsites.net/api/Simulations/StartSimulation?id=" + str(simulationID)
+    url = "https://lexsetapi.azurewebsites.net/api/Simulations/QueueSimulation=" + str(simulationID)
 
     payload={}
     headers = {
     'Authorization': 'Bearer ' + token
     }
 
     response = requests.request("POST", url, headers=headers, data=payload)
@@ -404,15 +404,15 @@
         self.simulations = ""
         self.numSimulations = 0
         self.isComplete = False
         self.dataSetItems = ""
         self.numRendered = 0
 
     def startSimulation(self):
-        url = "https://lexsetapi.azurewebsites.net/api/Simulations/StartSimulation?id=" + str(self.simID)
+        url = "https://lexsetapi.azurewebsites.net/api/Simulations/QueueSimulation?id=" + str(self.simID)
 
         payload={}
         headers = {
         'Authorization': 'Bearer ' + self.token
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
@@ -555,61 +555,63 @@
     """
     percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
     filledLength = int(length * iteration // total)
     bar = fill * filledLength + '-' * (length - filledLength)
     print(f'{prefix} |{bar}| {percent}% {suffix}', end = printEnd)
 
 
-def batchSimulation(queue, allNodes, userID,token):
+# BATCH SIMULATION REMOVED WHEN SIMULATION QUEUE ADDED 7-18-2023
 
-    state = []
-    runningNodes = activeSimulationNodes(userID, token)
-    for item in range(len(queue)):
-        queue[item].updateStatus()
-        state.append(queue[item].hasStarted)
-        x = all(state)
-
-    while x == False:
-        #runningNodes = activeSimulationNodes(3,token)
-        for item in range(len(queue)):
-            if (queue[item].hasStarted == True and queue[item].isComplete == False):
-                print('\033[2KSimulation [' + str(queue[item].simID) + '] : ', end='')
-                printProgressBar(queue[item].getProgress(), 100, prefix='Running', length=50)
+# def batchSimulation(queue, allNodes, userID,token):
+
+#     state = []
+#     runningNodes = activeSimulationNodes(userID, token)
+#     for item in range(len(queue)):
+#         queue[item].updateStatus()
+#         state.append(queue[item].hasStarted)
+#         x = all(state)
+
+#     while x == False:
+#         #runningNodes = activeSimulationNodes(3,token)
+#         for item in range(len(queue)):
+#             if (queue[item].hasStarted == True and queue[item].isComplete == False):
+#                 print('\033[2KSimulation [' + str(queue[item].simID) + '] : ', end='')
+#                 printProgressBar(queue[item].getProgress(), 100, prefix='Running', length=50)
                     
-            if (queue[item].hasStarted == True and queue[item].isComplete == True):
-                print('\033[2KSimulation [' + str(queue[item].simID) + '] : Complete')
+#             if (queue[item].hasStarted == True and queue[item].isComplete == True):
+#                 print('\033[2KSimulation [' + str(queue[item].simID) + '] : Complete')
                     
-            if (queue[item].hasStarted == False and queue[item].isComplete == False):
-                print('\033[2KSimulation [' + str(queue[item].simID) + '] : Not yet started')
+#             if (queue[item].hasStarted == False and queue[item].isComplete == False):
+#                 print('\033[2KSimulation [' + str(queue[item].simID) + '] : Not yet started')
 
-        print('\033['+str(len(queue)+1)+'A')
+#         print('\033['+str(len(queue)+1)+'A')
 
-        for item in range(len(queue)):
-            time.sleep(5)
-            runningNodes = activeSimulationNodes(userID,token)
-            queue[item].updateStatus()
-            if (queue[item].nodeCount + runningNodes <= allNodes and queue[item].hasStarted == False) :
-                queue[item].startSimulation()
-                time.sleep(5)
+#         for item in range(len(queue)):
+#             time.sleep(5)
+#             runningNodes = activeSimulationNodes(userID,token)
+#             queue[item].updateStatus()
+#             if (queue[item].nodeCount + runningNodes <= allNodes and queue[item].hasStarted == False) :
+#                 queue[item].startSimulation()
+#                 time.sleep(5)
                 
-            state[item]=queue[item].hasStarted
-            x = all(state)
+#             state[item]=queue[item].hasStarted
+#             x = all(state)
 
-    for item in range(len(queue)):
-        if (queue[item].hasStarted == True and queue[item].isComplete == False):
-            print('\033[2KSimulation [' + str(queue[item].simID) + '] : ', end='')
-            printProgressBar(queue[item].getProgress(), 100, prefix='Running', length=50)
+#     for item in range(len(queue)):
+#         if (queue[item].hasStarted == True and queue[item].isComplete == False):
+#             print('\033[2KSimulation [' + str(queue[item].simID) + '] : ', end='')
+#             printProgressBar(queue[item].getProgress(), 100, prefix='Running', length=50)
                 
-        if (queue[item].hasStarted == True and queue[item].isComplete == True):
-            print('\033[2KSimulation [' + str(queue[item].simID) + '] : Complete')
+#         if (queue[item].hasStarted == True and queue[item].isComplete == True):
+#             print('\033[2KSimulation [' + str(queue[item].simID) + '] : Complete')
                 
-        if (queue[item].hasStarted == False and queue[item].isComplete == False):
-            print('\033[2KSimulation [' + str(queue[item].simID) + '] : Not yet started')
+#         if (queue[item].hasStarted == False and queue[item].isComplete == False):
+#             print('\033[2KSimulation [' + str(queue[item].simID) + '] : Not yet started')
 
-    print("All simulations in queue have been started.")
+#     print("All simulations in queue have been started.")
 
 def getOrganizationSimulations(orgID,state,token):
 
     # //Possible States
     # // RUNNING
     # // COMPLETED
     # // CREATED
@@ -738,14 +740,34 @@
     headers = {'Authorization': 'Bearer ' + str(token)}
     response = requests.delete(f'https://lexsetapi.lexset.ai/api/simulations/archivesimulation?id={id}', headers=headers)
     if response.status_code == 200:
         print("Simulation successfully deleted.")
     else:
         print(f"Error deleting simulation: {response.text}")
 
+def dequeue(simulationID,token):
+    url = "https://lexsetapi.azurewebsites.net/api/Simulations/RemoveSimulationFromQueue=" + str(simulationID)
+
+    payload={}
+    headers = {
+    'Authorization': 'Bearer ' + token
+    }
+
+    response = requests.request("POST", url, headers=headers, data=payload)
+    
+    getCode = response.status_code
+    if getCode == 401:
+        return("Unauthorized")
+    if getCode == 200:
+        #parseResponse = json.loads(response.text)
+        return("success")
+    else:
+        print("Error: " + str(getCode))
+        return(getCode)
+
 
 def gcp_transfer(id, userToken, bucketName, simulationId, token):
 
     url = "https://coreapi.lexset.ai/api/userdatamanagement/TransferDatasetToGcp?userid=" + str(id) + "&simulationId=" + str(simulationId) + "&bucketName=" + bucketName
     
     payload={}
     headers = {
```

### Comparing `lexsetAPI-3.4.2/lexsetAPI/credentials.py` & `lexsetAPI-3.4.3/lexsetAPI/credentials.py`

 * *Files identical despite different names*

