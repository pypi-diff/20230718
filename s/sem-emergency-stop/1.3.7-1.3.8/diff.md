# Comparing `tmp/sem-emergency-stop-1.3.7.tar.gz` & `tmp/sem-emergency-stop-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sem-emergency-stop-1.3.7.tar", last modified: Wed Apr  5 09:44:15 2023, max compression
+gzip compressed data, was "sem-emergency-stop-1.3.8.tar", last modified: Wed Apr  5 10:27:41 2023, max compression
```

## Comparing `sem-emergency-stop-1.3.7.tar` & `sem-emergency-stop-1.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pb        (1000) users      (100)        0 2023-04-05 09:44:15.167593 sem-emergency-stop-1.3.7/
--rw-r--r--   0 pb        (1000) users      (100)    11358 2021-09-02 13:10:54.000000 sem-emergency-stop-1.3.7/LICENSE
--rw-r--r--   0 pb        (1000) users      (100)     3203 2023-04-05 09:44:15.166593 sem-emergency-stop-1.3.7/PKG-INFO
--rw-r--r--   0 pb        (1000) users      (100)     2881 2021-09-02 13:10:54.000000 sem-emergency-stop-1.3.7/README.md
--rw-r--r--   0 pb        (1000) users      (100)      100 2022-04-04 13:56:44.000000 sem-emergency-stop-1.3.7/pyproject.toml
-drwxr-xr-x   0 pb        (1000) users      (100)        0 2023-04-05 09:44:15.166593 sem-emergency-stop-1.3.7/sem_emergency_stop.egg-info/
--rw-r--r--   0 pb        (1000) users      (100)     3203 2023-04-05 09:44:15.000000 sem-emergency-stop-1.3.7/sem_emergency_stop.egg-info/PKG-INFO
--rw-r--r--   0 pb        (1000) users      (100)      349 2023-04-05 09:44:15.000000 sem-emergency-stop-1.3.7/sem_emergency_stop.egg-info/SOURCES.txt
--rw-r--r--   0 pb        (1000) users      (100)        1 2023-04-05 09:44:15.000000 sem-emergency-stop-1.3.7/sem_emergency_stop.egg-info/dependency_links.txt
--rw-r--r--   0 pb        (1000) users      (100)      138 2023-04-05 09:44:15.000000 sem-emergency-stop-1.3.7/sem_emergency_stop.egg-info/entry_points.txt
--rw-r--r--   0 pb        (1000) users      (100)       19 2023-04-05 09:44:15.000000 sem-emergency-stop-1.3.7/sem_emergency_stop.egg-info/requires.txt
--rw-r--r--   0 pb        (1000) users      (100)        4 2023-04-05 09:44:15.000000 sem-emergency-stop-1.3.7/sem_emergency_stop.egg-info/top_level.txt
-drwxr-xr-x   0 pb        (1000) users      (100)        0 2023-04-05 09:44:15.166593 sem-emergency-stop-1.3.7/ses/
--rw-r--r--   0 pb        (1000) users      (100)        0 2021-09-02 13:10:54.000000 sem-emergency-stop-1.3.7/ses/__init__.py
--rw-r--r--   0 pb        (1000) users      (100)     4995 2021-09-02 13:10:54.000000 sem-emergency-stop-1.3.7/ses/auth.py
--rw-r--r--   0 pb        (1000) users      (100)    30674 2021-09-02 13:10:54.000000 sem-emergency-stop-1.3.7/ses/banner.py
--rw-r--r--   0 pb        (1000) users      (100)    11825 2022-07-06 08:11:45.000000 sem-emergency-stop-1.3.7/ses/main.py
--rw-r--r--   0 pb        (1000) users      (100)       38 2023-04-05 09:44:15.167593 sem-emergency-stop-1.3.7/setup.cfg
--rw-r--r--   0 pb        (1000) users      (100)      809 2023-04-05 09:43:15.000000 sem-emergency-stop-1.3.7/setup.py
+drwxr-xr-x   0 pb        (1000) users      (100)        0 2023-04-05 10:27:41.158643 sem-emergency-stop-1.3.8/
+-rw-r--r--   0 pb        (1000) users      (100)    11358 2021-09-02 13:10:54.000000 sem-emergency-stop-1.3.8/LICENSE
+-rw-r--r--   0 pb        (1000) users      (100)     3203 2023-04-05 10:27:41.158643 sem-emergency-stop-1.3.8/PKG-INFO
+-rw-r--r--   0 pb        (1000) users      (100)     2881 2021-09-02 13:10:54.000000 sem-emergency-stop-1.3.8/README.md
+-rw-r--r--   0 pb        (1000) users      (100)      100 2022-04-04 13:56:44.000000 sem-emergency-stop-1.3.8/pyproject.toml
+drwxr-xr-x   0 pb        (1000) users      (100)        0 2023-04-05 10:27:41.158643 sem-emergency-stop-1.3.8/sem_emergency_stop.egg-info/
+-rw-r--r--   0 pb        (1000) users      (100)     3203 2023-04-05 10:27:41.000000 sem-emergency-stop-1.3.8/sem_emergency_stop.egg-info/PKG-INFO
+-rw-r--r--   0 pb        (1000) users      (100)      349 2023-04-05 10:27:41.000000 sem-emergency-stop-1.3.8/sem_emergency_stop.egg-info/SOURCES.txt
+-rw-r--r--   0 pb        (1000) users      (100)        1 2023-04-05 10:27:41.000000 sem-emergency-stop-1.3.8/sem_emergency_stop.egg-info/dependency_links.txt
+-rw-r--r--   0 pb        (1000) users      (100)      138 2023-04-05 10:27:41.000000 sem-emergency-stop-1.3.8/sem_emergency_stop.egg-info/entry_points.txt
+-rw-r--r--   0 pb        (1000) users      (100)       19 2023-04-05 10:27:41.000000 sem-emergency-stop-1.3.8/sem_emergency_stop.egg-info/requires.txt
+-rw-r--r--   0 pb        (1000) users      (100)        4 2023-04-05 10:27:41.000000 sem-emergency-stop-1.3.8/sem_emergency_stop.egg-info/top_level.txt
+drwxr-xr-x   0 pb        (1000) users      (100)        0 2023-04-05 10:27:41.158643 sem-emergency-stop-1.3.8/ses/
+-rw-r--r--   0 pb        (1000) users      (100)        0 2021-09-02 13:10:54.000000 sem-emergency-stop-1.3.8/ses/__init__.py
+-rw-r--r--   0 pb        (1000) users      (100)     7063 2023-04-05 10:25:30.000000 sem-emergency-stop-1.3.8/ses/auth.py
+-rw-r--r--   0 pb        (1000) users      (100)    30674 2021-09-02 13:10:54.000000 sem-emergency-stop-1.3.8/ses/banner.py
+-rw-r--r--   0 pb        (1000) users      (100)    11825 2023-04-05 09:54:37.000000 sem-emergency-stop-1.3.8/ses/main.py
+-rw-r--r--   0 pb        (1000) users      (100)       38 2023-04-05 10:27:41.158643 sem-emergency-stop-1.3.8/setup.cfg
+-rw-r--r--   0 pb        (1000) users      (100)      809 2023-04-05 10:26:48.000000 sem-emergency-stop-1.3.8/setup.py
```

### Comparing `sem-emergency-stop-1.3.7/LICENSE` & `sem-emergency-stop-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sem-emergency-stop-1.3.7/PKG-INFO` & `sem-emergency-stop-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sem-emergency-stop
-Version: 1.3.7
+Version: 1.3.8
 Summary: Quickly stop all Google Ads advertising
 Home-page: https://github.com/getyourguide/sem-emergency-stop
 Author: GetYourGuide GmbH
 License: Apache License, Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sem-emergency-stop-1.3.7/README.md` & `sem-emergency-stop-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `sem-emergency-stop-1.3.7/sem_emergency_stop.egg-info/PKG-INFO` & `sem-emergency-stop-1.3.8/sem_emergency_stop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sem-emergency-stop
-Version: 1.3.7
+Version: 1.3.8
 Summary: Quickly stop all Google Ads advertising
 Home-page: https://github.com/getyourguide/sem-emergency-stop
 Author: GetYourGuide GmbH
 License: Apache License, Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sem-emergency-stop-1.3.7/ses/auth.py` & `sem-emergency-stop-1.3.8/ses/auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import os
+import re
+import sys
 import base64
 import json
+import hashlib
+import socket
 from base64 import b64decode
+from urllib.parse import unquote
 
-from google_auth_oauthlib.flow import InstalledAppFlow
+from google_auth_oauthlib.flow import Flow
 
 
 app_directory = os.path.join(
     os.getenv('HOME'), '.config', 'sem-emergency-stop'
 )
 user_auth_file = os.path.join(app_directory, 'user-auth.json')
 client_auth_file = os.path.join(app_directory, 'client-auth.json')
@@ -127,24 +132,85 @@
         return json.load(open(user_auth_file))
     except FileNotFoundError:
         oauth_flow()
         return load_user_auth()
 
 
 def oauth_flow():
-    flow = InstalledAppFlow.from_client_secrets_file(
-        client_auth_file, scopes=[auth_scope]
+    host = '127.0.0.1'
+    port = 14711
+    redirect_uri = f'http://{host}:{port}'
+    flow = Flow.from_client_secrets_file(client_auth_file, scopes=[auth_scope])
+    flow.redirect_uri = redirect_uri
+
+    passthrough_val = hashlib.sha256(os.urandom(1024)).hexdigest()
+    authorization_url, state = flow.authorization_url(
+        access_type='offline',
+        state=passthrough_val,
+        prompt='consent',
+        include_granted_scopes='true',
     )
 
-    flow.run_console()
+    print('Paste this URL into your browser: ')
+    print(authorization_url)
+    print(f'\nWaiting for authorization and callback to: {redirect_uri}')
+
+    code = unquote(get_authorization_code(passthrough_val, host, port))
+
+    flow.fetch_token(code=code)
+    refresh_token = flow.credentials.refresh_token
+
+    json.dump({'refresh_token': refresh_token}, open(user_auth_file, 'w'))
+
+
+def get_authorization_code(passthrough_val, host, port):
+    sock = socket.socket()
+    sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+    sock.bind((host, port))
+    sock.listen(1)
+    connection, address = sock.accept()
+    data = connection.recv(1024)
+    params = parse_raw_query_params(data)
 
-    json.dump(
-        {'refresh_token': flow.credentials.refresh_token},
-        open(user_auth_file, 'w'),
-    )
+    try:
+        if not params.get('code'):
+            error = params.get('error')
+            message = f'Failed to retrieve authorization code. Error: {error}'
+            raise ValueError(message)
+        elif params.get('state') != passthrough_val:
+            message = 'State token does not match the expected state.'
+            raise ValueError(message)
+        else:
+            message = 'Authorization code was successfully retrieved.'
+    except ValueError as error:
+        print(error)
+        sys.exit(1)
+    finally:
+        response = (
+            'HTTP/1.1 200 OK\n'
+            'Content-Type: text/html\n\n'
+            f'<b>{message}</b>'
+            '<p>Please check the console output.</p>\n'
+        )
+
+        connection.sendall(response.encode())
+        connection.close()
+
+    return params.get('code')
+
+
+def parse_raw_query_params(data):
+    decoded = data.decode('utf-8')
+
+    match = re.search('GET\\s\\/\\?(.*) ', decoded)
+    params = match.group(1)
+
+    pairs = [pair.split('=') for pair in params.split('&')]
+
+    return {key: val for key, val in pairs}
 
 
 def organization_token_reader():
     for arg in (
         'login_customer_id',
         'developer_token',
         'client_id',
```

### Comparing `sem-emergency-stop-1.3.7/ses/banner.py` & `sem-emergency-stop-1.3.8/ses/banner.py`

 * *Files identical despite different names*

### Comparing `sem-emergency-stop-1.3.7/ses/main.py` & `sem-emergency-stop-1.3.8/ses/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 def query(service, customer_id, query):
     return service.search_stream(customer_id=str(customer_id), query=query)
 
 
 def collect_customer_ids(client):
-    service = client.get_service('GoogleAdsService', version='v11')
+    service = client.get_service('GoogleAdsService', version='v13')
     return [
         parse_customer_id(row.customer_client.resource_name)
         for response in query(
             service,
             client.login_customer_id,
             """
                 SELECT customer.id
@@ -86,15 +86,15 @@
         {
             'campaign_sets': sorted(campaign_sets),
         }
     )
 
 
 def collect_campaign_ids(client, customer_id):
-    service = client.get_service('GoogleAdsService', version='v11')
+    service = client.get_service('GoogleAdsService', version='v13')
     return [
         row.campaign.id
         for response in query(
             service,
             customer_id,
             """
                 SELECT campaign.id
@@ -123,18 +123,18 @@
         campaign_sets.put(campaign_set)
         progress_queue.put_nowait(('customers', 1))
         progress_queue.put_nowait(('campaigns', len(ids)))
         customer_ids.task_done()
 
 
 def get_operation(client, service, customer_id, campaign_id, is_pause):
-    operation = client.get_type('CampaignOperation', version='v11')
+    operation = client.get_type('CampaignOperation', version='v13')
     campaign = operation.update
     campaign.resource_name = service.campaign_path(customer_id, campaign_id)
-    enum = client.get_type('CampaignStatusEnum', version='v11')
+    enum = client.get_type('CampaignStatusEnum', version='v13')
     campaign.status = enum.PAUSED if is_pause else enum.ENABLED
     operation.update_mask.CopyFrom(protobuf_helpers.field_mask(None, campaign))
 
     return operation
 
 
 def mutate_campaigns(
@@ -173,15 +173,15 @@
 
     progress_queue.put(('customers', 1))
 
 
 def mutate_worker(
     client, verbose, no_dry_run, is_pause, campaign_set_queue, progress_queue
 ):
-    service = client.get_service('CampaignService', version='v11')
+    service = client.get_service('CampaignService', version='v13')
 
     while True:
         try:
             sha1_hash = campaign_set_queue.get_nowait()
         except Empty:
             return
```

### Comparing `sem-emergency-stop-1.3.7/setup.py` & `sem-emergency-stop-1.3.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='sem-emergency-stop',
-    version='1.3.7',
+    version='1.3.8',
     author='GetYourGuide GmbH',
     description='Quickly stop all Google Ads advertising',
     license='Apache License, Version 2.0',
     license_file='LICENSE',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/getyourguide/sem-emergency-stop',
```

