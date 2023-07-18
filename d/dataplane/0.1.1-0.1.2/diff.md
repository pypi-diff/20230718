# Comparing `tmp/dataplane-0.1.1.tar.gz` & `tmp/dataplane-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataplane-0.1.1.tar", last modified: Wed Jul  5 20:20:23 2023, max compression
+gzip compressed data, was "dataplane-0.1.2.tar", last modified: Tue Jul 18 15:53:35 2023, max compression
```

## Comparing `dataplane-0.1.1.tar` & `dataplane-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-05 20:19:36.000000 dataplane-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-05 20:20:23.345730 dataplane-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-05 20:19:36.000000 dataplane-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-05 20:20:04.000000 dataplane-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 20:20:23.345730 dataplane-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.341730 dataplane-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.341730 dataplane-0.1.1/src/dataplane/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.341730 dataplane-0.1.1/src/dataplane/DataStorage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/DataStorage/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/s3_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/DataStorage/s3/test_s3_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/Microsoft/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/sharepoint_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/sharepoint_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint_nonroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/Microsoft/Teams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Teams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Teams/test_webhook_send.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/Teams/webhook_send.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/Microsoft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/pipelinerun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/pandas_redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/pandas_s3_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/redis_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_pandas_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-05 20:19:36.000000 dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_s3_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:20:23.345730 dataplane-0.1.1/src/dataplane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-05 20:20:23.000000 dataplane-0.1.1/src/dataplane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-05 20:20:23.000000 dataplane-0.1.1/src/dataplane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:20:23.000000 dataplane-0.1.1/src/dataplane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 20:20:23.000000 dataplane-0.1.1/src/dataplane.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.886285 dataplane-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-18 15:52:32.000000 dataplane-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-18 15:53:35.886285 dataplane-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-18 15:52:32.000000 dataplane-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-18 15:53:11.000000 dataplane-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:53:35.886285 dataplane-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.874285 dataplane-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.878285 dataplane-0.1.2/src/dataplane/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.874285 dataplane-0.1.2/src/dataplane/DataStorage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.882285 dataplane-0.1.2/src/dataplane/DataStorage/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/DataStorage/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/DataStorage/s3/s3_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/DataStorage/s3/s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/DataStorage/s3/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/DataStorage/s3/test_s3_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.882285 dataplane-0.1.2/src/dataplane/Microsoft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.886285 dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/sharepoint_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/sharepoint_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/test_sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/test_sharepoint_nonroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/test_sharepoint_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.886285 dataplane-0.1.2/src/dataplane/Microsoft/Teams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/Teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/Teams/test_webhook_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/Teams/webhook_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/Microsoft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.886285 dataplane-0.1.2/src/dataplane/pipelinerun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/pipelinerun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.886285 dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/pandas_redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/pandas_s3_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/redis_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/test_pandas_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-18 15:52:32.000000 dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/test_s3_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:53:35.882285 dataplane-0.1.2/src/dataplane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-18 15:53:35.000000 dataplane-0.1.2/src/dataplane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-18 15:53:35.000000 dataplane-0.1.2/src/dataplane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:53:35.000000 dataplane-0.1.2/src/dataplane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:53:35.000000 dataplane-0.1.2/src/dataplane.egg-info/top_level.txt
```

### Comparing `dataplane-0.1.1/LICENSE` & `dataplane-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/PKG-INFO` & `dataplane-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataplane
-Version: 0.1.1
+Version: 0.1.2
 Summary: The data engineering library to build robust, reliable and on time data pipelines in Python.
 Author: Saul Frank, Dataplane, Inc.
 Project-URL: Homepage, https://dataplane.app
 Project-URL: Github, https://github.com/dataplane-app/dataplane-python-package
 Project-URL: Issues, https://github.com/dataplane-app/dataplane/issues
 Project-URL: Feedback, https://github.com/dataplane-app/dataplane/discussions
 Keywords: workflow,data-science,data,airflow,etl,dataplane,data-engineering,data-pipelines,datawarehouse,automation,data-analysis,scheduler
```

### Comparing `dataplane-0.1.1/README.md` & `dataplane-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/pyproject.toml` & `dataplane-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0", "redis>=1.0.0", "pandas>1.0.0", "requests>1.0.0", "boto3>1.0.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataplane"
-version = "0.1.1"
+version = "0.1.2"
 description = "The data engineering library to build robust, reliable and on time data pipelines in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: BSD License", "Operating System :: OS Independent",]
 keywords = [ "workflow", "data-science", "data", "airflow", "etl", "dataplane", "data-engineering", "data-pipelines", "datawarehouse", "automation", "data-analysis", "scheduler",]
 [[project.authors]]
 name = "Saul Frank"
```

### Comparing `dataplane-0.1.1/src/dataplane/DataStorage/s3/s3_download.py` & `dataplane-0.1.2/src/dataplane/DataStorage/s3/s3_download.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/DataStorage/s3/s3_upload.py` & `dataplane-0.1.2/src/dataplane/DataStorage/s3/s3_upload.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/DataStorage/s3/test_s3.py` & `dataplane-0.1.2/src/dataplane/DataStorage/s3/test_s3.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/DataStorage/s3/test_s3_object.py` & `dataplane-0.1.2/src/dataplane/DataStorage/s3/test_s3_object.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/sharepoint_download.py` & `dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/sharepoint_download.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Secret: Azure secret for client ID.
 SiteName: Name of the site to be looked up <- in url e.g https://{name}.sharepoint.com/sites/DataplanePython
 FilePath: /General/hello.xlxs
 ProxyUse: Whether to use a proxy, true or false
 ProxyUrl: Proxy endpoint to use
 ProxyMethod: https or http, default https
 """
-def sharepoint_download(Host, TenantID, ClientID, Secret, SiteName,  SharepointFilePath, DownloadMethod="Object", LocalFilePath="", Library="root", ProxyUse=False, ProxyUrl="", ProxyMethod="https"):
+def sharepoint_download(Host, TenantID, ClientID, Secret, SiteName,  SharepointFilePath, DownloadMethod="Object", LocalFilePath="", Library="root", ProxyUse=False, ProxyUrl="", ProxyMethod="https", SSLVerify=True):
 
     import requests
     from datetime import datetime
     import json
 
     # Start the timer
     start  = datetime.now()
@@ -33,15 +33,15 @@
     }
 
     if ProxyUse==True:
         proxies = {ProxyMethod: ProxyUrl}
     else:
         proxies = {}
 
-    auth = requests.request("POST", url, headers=headers, data=payload, proxies=proxies)
+    auth = requests.request("POST", url, headers=headers, data=payload, proxies=proxies, verify=SSLVerify)
     
     if auth.status_code != 200:
         duration = datetime.now() - start
         return {"result":"Fail", "reason":"Auth fail", "duration": str(duration), "status": auth.status_code, "error": auth.json()} 
 
 
     auth = auth.json()
@@ -49,15 +49,15 @@
     headers = {
         "Content-Type": "application/json",
         "Authorization": "Bearer " + auth["access_token"]
     }
 
     # ======= Get Site ID from Site name ====
     SiteName = SiteName.replace(" ", "")
-    SiteID = requests.request("GET", f"https://graph.microsoft.com/v1.0/sites/{Host}:/sites/{SiteName}?$select=id", headers=headers, json=payload, proxies=proxies)
+    SiteID = requests.request("GET", f"https://graph.microsoft.com/v1.0/sites/{Host}:/sites/{SiteName}?$select=id", headers=headers, json=payload, proxies=proxies, verify=SSLVerify)
     
     if SiteID.status_code != 200:
         duration = datetime.now() - start
         return {"result":"Fail", "reason":"Get site ID", "duration": str(duration), "status": SiteID.status_code, "error": SiteID.json()} 
 
     SiteID = SiteID.json()
 
@@ -67,15 +67,15 @@
     drive = "root"
     if Library == "root":
         # ====== Create an upload session =====
         url = f"https://graph.microsoft.com/v1.0/sites/{SiteID['id']}/drive/root:{SharepointFilePath}"
     else:
 
         drive = ""
-        driveID = requests.request("GET", f"https://graph.microsoft.com/v1.0/sites/{SiteID['id']}/drives?$select=name,id", headers=headers, json=payload, proxies=proxies)
+        driveID = requests.request("GET", f"https://graph.microsoft.com/v1.0/sites/{SiteID['id']}/drives?$select=name,id", headers=headers, json=payload, proxies=proxies, verify=SSLVerify)
         if driveID.status_code != 200:
             duration = datetime.now() - start
             return {"result":"Fail", "reason":"Sharepoint get drives", "duration": str(duration), "status": driveID.status_code, "error": driveID.json()} 
         
         driveID = driveID.json()
         for x in driveID["value"]:
             if x["name"] == Library:
@@ -87,25 +87,25 @@
             return {"result":"Fail", "reason":"Sharepoint no drove found fpr library "+Library, "duration": str(duration)} 
         
         url = f"https://graph.microsoft.com/v1.0/sites/{SiteID['id']}/drives/{drive}/root:{SharepointFilePath}"
 
     # ====== Get Item ID =====
 
     
-    ItemID = requests.request("GET", url, headers=headers, json=payload, proxies=proxies)
+    ItemID = requests.request("GET", url, headers=headers, json=payload, proxies=proxies, verify=SSLVerify)
     
     if ItemID.status_code != 200:
         duration = datetime.now() - start
         return {"result":"Fail", "reason":"Get download session", "duration": str(duration), "status": ItemID.status_code, "error": ItemID.json(), "payload": json.dumps(payload), "url": url} 
     
     ItemID = ItemID.json()
 
 
     # ====== Download file using link =====
-    r = requests.get(ItemID["@microsoft.graph.downloadUrl"], proxies=proxies)  
+    r = requests.get(ItemID["@microsoft.graph.downloadUrl"], proxies=proxies, verify=SSLVerify)  
 
     if DownloadMethod == "File":
         with open(LocalFilePath, 'wb') as f:
             f.write(r.content)
         duration = datetime.now() - start
         return {"result":"OK", "duration": str(duration), "status": r.status_code, "FilePath": LocalFilePath}
```

### Comparing `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/sharepoint_upload.py` & `dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/sharepoint_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 UploadMethod
 ProxyUse: Whether to use a proxy, true or false
 ProxyUrl: Proxy endpoint to use
 ProxyMethod: https or http, default https
 FileConflict: "fail (default) | replace | rename"
 FileDescription: Sharepoint description for the file
 """
-def sharepoint_upload(Host, TenantID, ClientID, Secret, SiteName, TargetFilePath, SourceFilePath="/tmp/default.txt", Library="root", UploadMethod="Object", UploadObject="", ProxyUse=False, ProxyUrl="", ProxyMethod="https", FileConflict="fail"):
+def sharepoint_upload(Host, TenantID, ClientID, Secret, SiteName, TargetFilePath, SourceFilePath="/tmp/default.txt", Library="root", UploadMethod="Object", UploadObject="", ProxyUse=False, ProxyUrl="", ProxyMethod="https", FileConflict="fail", SSLVerify=True):
 
 
     import requests
     import os
     from datetime import datetime
     import json
     import sys
@@ -40,15 +40,15 @@
     }
 
     if ProxyUse==True:
         proxies = {ProxyMethod: ProxyUrl}
     else:
         proxies = {}
 
-    auth = requests.request("POST", url, headers=headers, data=payload, proxies=proxies)
+    auth = requests.request("POST", url, headers=headers, data=payload, proxies=proxies, verify=SSLVerify)
     
     if auth.status_code != 200:
         duration = datetime.now() - start
         return {"result":"Fail", "reason":"Auth fail", "duration": str(duration), "status": auth.status_code, "error": auth.json()} 
 
 
     auth = auth.json()
@@ -56,15 +56,15 @@
     headers = {
         "Content-Type": "application/json",
         "Authorization": "Bearer " + auth["access_token"]
     }
 
     # ======= Get Site ID from Site name ====
     SiteName = SiteName.replace(" ", "")
-    SiteID = requests.request("GET", f"https://graph.microsoft.com/v1.0/sites/{Host}:/sites/{SiteName}?$select=id", headers=headers, json=payload, proxies=proxies)
+    SiteID = requests.request("GET", f"https://graph.microsoft.com/v1.0/sites/{Host}:/sites/{SiteName}?$select=id", headers=headers, json=payload, proxies=proxies, verify=SSLVerify)
     
     if SiteID.status_code != 200:
         duration = datetime.now() - start
         return {"result":"Fail", "reason":"Get site ID", "duration": str(duration), "status": SiteID.status_code, "error": SiteID.json()} 
 
     SiteID = SiteID.json()
 
@@ -76,15 +76,15 @@
     drive = "root"
     if Library == "root":
         # ====== Create an upload session =====
         url = f"https://graph.microsoft.com/v1.0/sites/{SiteID['id']}/drive/root:{TargetFilePath}:/createUploadSession"
     else:
 
         drive = ""
-        driveID = requests.request("GET", f"https://graph.microsoft.com/v1.0/sites/{SiteID['id']}/drives?$select=name,id", headers=headers, json=payload, proxies=proxies)
+        driveID = requests.request("GET", f"https://graph.microsoft.com/v1.0/sites/{SiteID['id']}/drives?$select=name,id", headers=headers, json=payload, proxies=proxies, verify=SSLVerify)
         if driveID.status_code != 200:
             duration = datetime.now() - start
             return {"result":"Fail", "reason":"Sharepoint get drives", "duration": str(duration), "status": driveID.status_code, "error": driveID.json()} 
         
         driveID = driveID.json()
         for x in driveID["value"]:
             if x["name"] == Library:
@@ -107,15 +107,15 @@
         print("File size:", FileSize)
 
     payload = {
         "@microsoft.graph.conflictBehavior": FileConflict,
         "fileSize": FileSize,
         "name": TargetFilePath
     }
-    UploadUrl = requests.request("POST", url, headers=headers, json=payload, proxies=proxies)
+    UploadUrl = requests.request("POST", url, headers=headers, json=payload, proxies=proxies, verify=SSLVerify)
     
     if UploadUrl.status_code != 200:
         duration = datetime.now() - start
         return {"result":"Fail", "reason":"Get upload session", "duration": str(duration), "status": UploadUrl.status_code, "error": UploadUrl.json(), "payload": json.dumps(payload), "url": url} 
     
     UploadUrl = UploadUrl.json()
 
@@ -128,15 +128,15 @@
     headers = {
         "Content-Type": "application/octet-stream",
         "Content-Length": str(FileSize),
         "Content-Range": f"bytes 0-{FileSize-1}/{FileSize}",
         # "Authorization": "Bearer " + auth["access_token"]
     }
 
-    upload = requests.put(UploadUrl["uploadUrl"], data=UploadObject, headers=headers, proxies=proxies)
+    upload = requests.put(UploadUrl["uploadUrl"], data=UploadObject, headers=headers, proxies=proxies, verify=SSLVerify)
     if upload.status_code != 201:
         duration = datetime.now() - start
         return {"result":"non 201", "reason":"Upload file", "duration": str(duration), "status": upload.status_code, "response": upload.json()}
 
     duration = datetime.now() - start
 
     return {"result":"OK", "duration": str(duration), "status": upload.status_code, "response": upload.json()}
```

### Comparing `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint.py` & `dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/test_sharepoint.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint_nonroot.py` & `dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/test_sharepoint_nonroot.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/Microsoft/Sharepoint/test_sharepoint_object.py` & `dataplane-0.1.2/src/dataplane/Microsoft/Sharepoint/test_sharepoint_object.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/Microsoft/Teams/test_webhook_send.py` & `dataplane-0.1.2/src/dataplane/Microsoft/Teams/test_webhook_send.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/Microsoft/Teams/webhook_send.py` & `dataplane-0.1.2/src/dataplane/Microsoft/Teams/webhook_send.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/__init__.py` & `dataplane-0.1.2/src/dataplane/__init__.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/pandas_redis_store.py` & `dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/pandas_redis_store.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/pandas_s3_store.py` & `dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/pandas_s3_store.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/redis_store.py` & `dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/redis_store.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_pandas_redis.py` & `dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/test_pandas_redis.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_redis.py` & `dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/test_redis.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane/pipelinerun/data_persist/test_s3_store.py` & `dataplane-0.1.2/src/dataplane/pipelinerun/data_persist/test_s3_store.py`

 * *Files identical despite different names*

### Comparing `dataplane-0.1.1/src/dataplane.egg-info/PKG-INFO` & `dataplane-0.1.2/src/dataplane.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataplane
-Version: 0.1.1
+Version: 0.1.2
 Summary: The data engineering library to build robust, reliable and on time data pipelines in Python.
 Author: Saul Frank, Dataplane, Inc.
 Project-URL: Homepage, https://dataplane.app
 Project-URL: Github, https://github.com/dataplane-app/dataplane-python-package
 Project-URL: Issues, https://github.com/dataplane-app/dataplane/issues
 Project-URL: Feedback, https://github.com/dataplane-app/dataplane/discussions
 Keywords: workflow,data-science,data,airflow,etl,dataplane,data-engineering,data-pipelines,datawarehouse,automation,data-analysis,scheduler
```

### Comparing `dataplane-0.1.1/src/dataplane.egg-info/SOURCES.txt` & `dataplane-0.1.2/src/dataplane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

