# Comparing `tmp/fc-client-0.6.2.tar.gz` & `tmp/fc-client-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-client-0.6.2.tar", last modified: Thu Jul  6 08:49:04 2023, max compression
+gzip compressed data, was "dist/fc-client-0.6.3.tar", last modified: Tue Jul 18 04:27:05 2023, max compression
```

## Comparing `fc-client-0.6.2.tar` & `fc-client-0.6.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-06 08:48:52.000000 fc-client-0.6.2/LICENSE
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 08:49:04.000000 fc-client-0.6.2/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-06 08:48:52.000000 fc-client-0.6.2/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    14077 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_client/client.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      410 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/entry_points.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       92 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/requires.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client.egg-info/top_level.txt
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_client_daemon/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     7064 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_client_daemon/client_daemon.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-client-0.6.2/fc_common/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/VERSION
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/etcd.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/logger.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-06 08:48:52.000000 fc-client-0.6.2/fc_common/version.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-06 08:49:04.000000 fc-client-0.6.2/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-06 08:48:52.000000 fc-client-0.6.2/setup.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-18 04:26:21.000000 fc-client-0.6.3/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 04:27:05.000000 fc-client-0.6.3/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-18 04:26:21.000000 fc-client-0.6.3/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    14179 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_client/client.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      410 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       92 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/requires.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client_daemon/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     7064 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_client_daemon/client_daemon.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/version.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-18 04:27:05.000000 fc-client-0.6.3/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-18 04:26:21.000000 fc-client-0.6.3/setup.py
```

### Comparing `fc-client-0.6.2/LICENSE` & `fc-client-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.2/PKG-INFO` & `fc-client-0.6.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-client-0.6.2/README.rst` & `fc-client-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.2/fc_client/client.py` & `fc-client-0.6.3/fc_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import json
 import os
 import signal
 import socket
 import subprocess
 import sys
 import time
+import urllib.parse
 from getpass import getuser
 from socket import gethostname
 
 import aiohttp
 import prettytable
 import requests
 import yaml
@@ -173,28 +174,31 @@
 
     @staticmethod
     def status(args):
         async def get_status(fc_server):
             specified_resource = args.resource
             specified_farm_type = args.farm_type
             specified_device_type = args.device_type
+            specified_peripheral_info = args.peripheral_info
 
+            url = f"{fc_server}/resource"
             if specified_resource:
-                url = f"{fc_server}/resource/{specified_resource}"
-            elif specified_farm_type and specified_device_type:
-                url = (
-                    f"{fc_server}/resource"
-                    f"?farmtype={specified_farm_type}&devicetype={specified_device_type}"
-                )
-            elif specified_farm_type:
-                url = f"{fc_server}/resource?farmtype={specified_farm_type}"
-            elif specified_device_type:
-                url = f"{fc_server}/resource?devicetype={specified_device_type}"
-            else:
-                url = f"{fc_server}/resource"
+                url += f"/{specified_resource}"
+
+            query = {}
+            if specified_farm_type:
+                query["farmtype"] = specified_farm_type
+            if specified_device_type:
+                query["devicetype"] = specified_device_type
+            if specified_peripheral_info:
+                query["peripheralinfo"] = specified_peripheral_info
+            query_string = urllib.parse.urlencode(query)
+
+            if query_string:
+                url += f"?{query_string}"
 
             async with aiohttp.ClientSession() as session:
                 try:
                     async with session.get(url) as response:
                         output = await response.text()
                 except Exception:  # pylint: disable=broad-except
                     return []
@@ -340,14 +344,15 @@
     parser = argparse.ArgumentParser()
     parser.set_defaults(func=lambda args: parser.print_help())
     parser.add_argument(
         "-r", "--resource", "-p", "--place", type=str, help="resource name"
     )
     parser.add_argument("-f", "--farm-type", type=str, help="farm type")
     parser.add_argument("-d", "--device-type", type=str, help="device type")
+    parser.add_argument("-i", "--peripheral-info", type=str, help="peripheral info")
 
     args, extras = parser.parse_known_args()
 
     if (
         len(extras) > 0
         and extras[0]
         in [
```

### Comparing `fc-client-0.6.2/fc_client.egg-info/PKG-INFO` & `fc-client-0.6.3/fc_client.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-client-0.6.2/fc_client_daemon/client_daemon.py` & `fc-client-0.6.3/fc_client_daemon/client_daemon.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.2/fc_common/config.py` & `fc-client-0.6.3/fc_common/config.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.2/fc_common/etcd.py` & `fc-client-0.6.3/fc_common/etcd.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.2/fc_common/logger.py` & `fc-client-0.6.3/fc_common/logger.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.2/fc_common/version.py` & `fc-client-0.6.3/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.2/setup.cfg` & `fc-client-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.2/setup.py` & `fc-client-0.6.3/setup.py`

 * *Files identical despite different names*

