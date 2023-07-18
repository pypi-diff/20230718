# Comparing `tmp/lexset-4.0.5.tar.gz` & `tmp/lexset-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexset-4.0.5.tar", last modified: Wed May 10 23:29:39 2023, max compression
+gzip compressed data, was "lexset-4.0.6.tar", last modified: Tue Jul 18 19:19:42 2023, max compression
```

## Comparing `lexset-4.0.5.tar` & `lexset-4.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:29:39.169370 lexset-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:29:39.169370 lexset-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 23:29:18.000000 lexset-4.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:29:39.169370 lexset-4.0.5/lexset/
--rw-r--r--   0 runner    (1001) docker     (123)    28981 2023-05-10 23:29:18.000000 lexset-4.0.5/lexset/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 23:29:18.000000 lexset-4.0.5/lexset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 23:29:18.000000 lexset-4.0.5/lexset/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 23:29:39.169370 lexset-4.0.5/lexset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 23:29:39.000000 lexset-4.0.5/lexset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 23:29:39.169370 lexset-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 23:29:18.000000 lexset-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:19:42.786081 lexset-4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 19:19:42.786081 lexset-4.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 19:19:25.000000 lexset-4.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:19:42.786081 lexset-4.0.6/lexset/
+-rw-r--r--   0 runner    (1001) docker     (123)    30597 2023-07-18 19:19:25.000000 lexset-4.0.6/lexset/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 19:19:25.000000 lexset-4.0.6/lexset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 19:19:25.000000 lexset-4.0.6/lexset/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:19:42.786081 lexset-4.0.6/lexset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 19:19:42.000000 lexset-4.0.6/lexset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:19:42.786081 lexset-4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 19:19:25.000000 lexset-4.0.6/setup.py
```

### Comparing `lexset-4.0.5/lexset/LexsetManager.py` & `lexset-4.0.6/lexset/LexsetManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     def setSimulation_id(self, simulationID):
         self.simulation_id = simulationID
         print("\n\33[1;32;40mSimulation ID(s) set to: " + str(self.simulation_id) + "\n\33[0m")
 
     def get_organization_simulations(self,state, limit = 100):
 
         #CHECK REQUESTED STATE
-        if(state == "RUNNING" or state == "COMPLETED" or state == "CREATED"):
+        if(state == "RUNNING" or state == "COMPLETED" or state == "CREATED" or state == "QUEUED"):
             print("\33[3;37;40mGetting simulations for organizationID: " + str(self.organization_id) + "-->\33[0m")
         else:
             print("\33[1;31;40mInvalid State: " + state + "\33[0m")
             print("\33[3;37;40mValid States: RUNNING, COMPLETED, CREATED\33[0m")
             return
 
         url = "https://lexsetapi.lexset.ai/api/Simulations/GetSimulationsByOrganization?orgid=" + (str(self.organization_id)) +"&state=" + state
@@ -349,15 +349,15 @@
     def start(self):
         #convert simulation id into an array if not already
         if type(self.simulation_id) is not list:
             self.simulation_id = [self.simulation_id]
         
         for id in self.simulation_id:            
 
-            url = "https://lexsetapi.azurewebsites.net/api/Simulations/StartSimulation?id=" + str(id)
+            url = "https://lexsetapi.azurewebsites.net/api/Simulations/QueueSimulation?id=" + str(id)
 
             payload={}
             headers = {
             'Authorization': 'Bearer ' + self.token
             }
 
             response = requests.request("POST", url, headers=headers, data=payload)
@@ -370,14 +370,47 @@
                 #parseResponse = json.loads(response.text)
                 time.sleep(5)
                 return("success")
             else:
                 print("\33[1;31;40mstart() Error: " + str(response.status_code) + "\33[0m")
                 return(response.status_code)        
 
+    def dequeue(self):
+        #convert simulation id into an array if not already
+        if type(self.simulation_id) is not list:
+            self.simulation_id = [self.simulation_id]
+        
+        for id in self.simulation_id:            
+
+            url = "https://lexsetapi.azurewebsites.net/api/Simulations/RemoveSimulationFromQueue?id=" + str(id)
+
+            payload={}
+            headers = {
+            'Authorization': 'Bearer ' + self.token
+            }
+
+            response = requests.request("DELETE", url, headers=headers, data=payload)
+
+            if response.status_code == 401:
+                print("\33[1;31;40mUnauthorized: " + str(response.status_code) + "\33[0m")
+                return("Unauthorized")
+            if response.status_code == 200:
+                print("\n\33[1;32;40mSimulation ID "+ str(self.simulation_id) +" started successfully.\33[0m")
+                #parseResponse = json.loads(response.text)
+                time.sleep(5)
+                return("success")
+            if response.status_code == 400:
+                print("\n\33[1;32;40mSimulation ID "+ str(self.simulation_id) +" not in queue.\33[0m")
+                #parseResponse = json.loads(response.text)
+                time.sleep(5)
+                return("warning")
+            else:
+                print("\33[1;31;40mstart() Error: " + str(response.status_code) + "\33[0m")
+                return(response.status_code)        
+
     def stop(self):
 
         #convert simulation id into an array if not already
         if type(self.simulation_id) is not list:
             self.simulation_id = [self.simulation_id]
         
 
@@ -494,57 +527,58 @@
         if getCode == 200: 
             parseResponse = json.loads(response.text) 
             return(parseResponse) 
         else: 
             print("Error: " + str(getCode)) 
             return(getCode) 
 
+# BATCHING SIMUALTIONS DISABLED AS OF 7-18-23 NOT COMPATIBLE WITH QUEUE SYSTEM
 
-    def batch_start(self, allNodes):
-        #convert simulation id into an array if not already
-        if type(self.simulation_id) is not list:
-            self.simulation_id = [self.simulation_id]
+    # def batch_start(self, allNodes):
+    #     #convert simulation id into an array if not already
+    #     if type(self.simulation_id) is not list:
+    #         self.simulation_id = [self.simulation_id]
         
-        queue = self.simulation_id
-        def update_status():
-            #convert simulation id into an array if not already
-            if type(self.simulation_id) is not list:
-                self.simulation_id = [self.simulation_id]
-
-            #initilze status_list
-            self.status_list = []
-            for id in self.simulation_id:
-
-                url = "https://lexsetapi.azurewebsites.net/api/simulations/getsimulationstatus?id=" + str(id)
-
-                payload={}
-                headers = {
-                'Authorization': 'Bearer ' + self.token
-                }
+    #     queue = self.simulation_id
+    #     def update_status():
+    #         #convert simulation id into an array if not already
+    #         if type(self.simulation_id) is not list:
+    #             self.simulation_id = [self.simulation_id]
+
+    #         #initilze status_list
+    #         self.status_list = []
+    #         for id in self.simulation_id:
+
+    #             url = "https://lexsetapi.azurewebsites.net/api/simulations/getsimulationstatus?id=" + str(id)
+
+    #             payload={}
+    #             headers = {
+    #             'Authorization': 'Bearer ' + self.token
+    #             }
 
-                response = requests.request("GET", url, headers=headers, data=payload)
+    #             response = requests.request("GET", url, headers=headers, data=payload)
                 
-                if response.status_code == 401:
-                    print("\33[1;31;40mUnauthorized: " + str(response.status_code) + "\33[0m")
-                    return("Unauthorized")
-                if response.status_code == 200:
-                    #update if sim is complete or not complete
-                    parseResponse = json.loads(response.text)
+    #             if response.status_code == 401:
+    #                 print("\33[1;31;40mUnauthorized: " + str(response.status_code) + "\33[0m")
+    #                 return("Unauthorized")
+    #             if response.status_code == 200:
+    #                 #update if sim is complete or not complete
+    #                 parseResponse = json.loads(response.text)
                     
-                    if parseResponse == None:
-                        return False
-                    else:
-                        isComplete = parseResponse["isComplete"]
-                        hasStarted = parseResponse["hasStarted"]
-                        requestedNodes = parseResponse["requestedNodeCount"]
-                        status_tuple = (id, isComplete, hasStarted, requestedNodes)
-                        self.status_list.append(status_tuple)
-                else:
-                    print("\33[1;31;40mget_status() Error: " + str(response.status_code) + "\33[0m")
-                    return(response.status_code)
+    #                 if parseResponse == None:
+    #                     return False
+    #                 else:
+    #                     isComplete = parseResponse["isComplete"]
+    #                     hasStarted = parseResponse["hasStarted"]
+    #                     requestedNodes = parseResponse["requestedNodeCount"]
+    #                     status_tuple = (id, isComplete, hasStarted, requestedNodes)
+    #                     self.status_list.append(status_tuple)
+    #             else:
+    #                 print("\33[1;31;40mget_status() Error: " + str(response.status_code) + "\33[0m")
+    #                 return(response.status_code)
             
         def activeSimulationNodes(userID, token):
             url = "https://lexsetapi.azurewebsites.net/api/simulations/GetActiveSimulations/?userid=" + str(userID)
 
             payload={}
             headers = {
             'Authorization': 'Bearer ' + token
@@ -578,15 +612,15 @@
 
             response = requests.request("GET", url, headers=headers, data=payload)
             parseResponse = json.loads(response.text)
             return parseResponse['percentComplete']
 
 
         def startSimulation(simID):
-            url = "https://lexsetapi.azurewebsites.net/api/Simulations/StartSimulation?id=" + str(simID)
+            url = "https://lexsetapi.azurewebsites.net/api/Simulations/QueueSimulation?id=" + str(simID)
 
             payload={}
             headers = {
             'Authorization': 'Bearer ' + self.token
             }
 
             response = requests.request("POST", url, headers=headers, data=payload)
```

### Comparing `lexset-4.0.5/lexset/credentials.py` & `lexset-4.0.6/lexset/credentials.py`

 * *Files identical despite different names*

