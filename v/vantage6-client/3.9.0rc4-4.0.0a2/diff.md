# Comparing `tmp/vantage6-client-3.9.0rc4.tar.gz` & `tmp/vantage6-client-4.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-client-3.9.0rc4.tar", last modified: Wed May 24 09:34:09 2023, max compression
+gzip compressed data, was "vantage6-client-4.0.0a2.tar", last modified: Tue Jul 18 13:32:08 2023, max compression
```

## Comparing `vantage6-client-3.9.0rc4.tar` & `vantage6-client-4.0.0a2.tar`

### file list

```diff
@@ -1,38 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.073726 vantage6-client-3.9.0rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.073726 vantage6-client-3.9.0rc4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/vantage6/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    83916 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/algorithm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/vantage6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/dispatch_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-05-24 09:33:56.000000 vantage6-client-3.9.0rc4/vantage6/tools/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:09.077726 vantage6-client-3.9.0rc4/vantage6_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 09:34:09.000000 vantage6-client-3.9.0rc4/vantage6_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.112671 vantage6-client-4.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 13:32:08.112671 vantage6-client-4.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:32:08.112671 vantage6-client-4.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.108671 vantage6-client-4.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/tests/algorithm_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/tests/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/tests/test_docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.108671 vantage6-client-4.0.0a2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.108671 vantage6-client-4.0.0a2/vantage6/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/client/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    58214 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/client/algorithm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.112671 vantage6-client-4.0.0a2/vantage6/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/tools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/tools/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/tools/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-18 13:31:55.000000 vantage6-client-4.0.0a2/vantage6/tools/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:08.112671 vantage6-client-4.0.0a2/vantage6_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 13:32:08.000000 vantage6-client-4.0.0a2/vantage6_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-18 13:32:08.000000 vantage6-client-4.0.0a2/vantage6_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:32:08.000000 vantage6-client-4.0.0a2/vantage6_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 13:32:08.000000 vantage6-client-4.0.0a2/vantage6_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 13:32:08.000000 vantage6-client-4.0.0a2/vantage6_client.egg-info/top_level.txt
```

### Comparing `vantage6-client-3.9.0rc4/PKG-INFO` & `vantage6-client-4.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.9.0rc4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a2 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.9.0rc4/setup.py` & `vantage6-client-4.0.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'pandas==1.5.3',
         'PyJWT==2.6.0',
         'pyfiglet==0.8.post1',
-        'requests==2.31.0',
         'SPARQLWrapper==2.0.0',
         'qrcode==7.3.1',
         f'vantage6-common=={version_ns["__version__"]}',
     ],
     tests_require=["pytest"],
     package_data={
         'vantage6.client': [
```

### Comparing `vantage6-client-3.9.0rc4/tests/test_client.py` & `vantage6-client-4.0.0a2/tests/test_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import json
-import pickle
+
 from unittest import TestCase
 from unittest.mock import patch, MagicMock
 
-from vantage6.client import Client
+from vantage6.client import UserClient
 from vantage6.common.globals import STRING_ENCODING
 
 # Mock server
 HOST = 'mock_server'
 PORT = 1234
 
 # Mock credentials
@@ -22,69 +22,46 @@
 ORGANIZATION_IDS = [1]
 SAMPLE_INPUT = {'method': 'test-task'}
 FAKE_NAME = 'john doe'
 
 
 class TestClient(TestCase):
 
-    def test_post_task_legacy_method(self):
-        post_input = TestClient.post_task_on_mock_client(SAMPLE_INPUT, 'legacy')
-        decoded_input = base64.b64decode(post_input)
-        decoded_input = pickle.loads(decoded_input)
-        assert {'method': 'test-task'} == decoded_input
-
-    def test_post_json_task(self):
-        post_input = TestClient.post_task_on_mock_client(SAMPLE_INPUT, 'json')
-        decoded_input = base64.b64decode(post_input)
-        assert b'json.{"method": "test-task"}' == decoded_input
-
-    def test_post_pickle_task(self):
-        post_input = TestClient.post_task_on_mock_client(SAMPLE_INPUT, 'pickle')
+    def test_post_task(self):
+        post_input = TestClient.post_task_on_mock_client(SAMPLE_INPUT)
         decoded_input = base64.b64decode(post_input)
+        assert b'{"method": "test-task"}' == decoded_input
 
-        assert b'pickle.' == decoded_input[0:7]
-
-        assert {'method': 'test-task'} == pickle.loads(decoded_input[7:])
-
-    def test_get_legacy_results(self):
-        mock_result = pickle.dumps(1)
-
-        results = TestClient._receive_results_on_mock_client(mock_result)
-
-        assert results == [{'result': 1}]
-
-    def test_get_json_results(self):
-        mock_result = b'json.' + json.dumps({'some_key': 'some_value'}).encode()
+    def test_get_results(self):
+        mock_result = json.dumps({'some_key': 'some_value'}).encode()
 
         results = TestClient._receive_results_on_mock_client(mock_result)
 
         assert results == [{'result': {'some_key': 'some_value'}}]
 
-    def test_get_pickle_results(self):
-        mock_result = b'pickle.' + pickle.dumps([1, 2, 3, 4, 5])
-
-        results = TestClient._receive_results_on_mock_client(mock_result)
-
-        assert results == [{'result': [1, 2, 3, 4, 5]}]
-
     @staticmethod
-    def post_task_on_mock_client(input_, serialization: str) -> dict[str, any]:
+    def post_task_on_mock_client(input_) -> dict[str, any]:
         mock_requests = MagicMock()
         mock_requests.get.return_value.status_code = 200
         mock_requests.post.return_value.status_code = 200
 
         mock_jwt = TestClient._create_mock_jwt()
-        with patch.multiple('vantage6.client', requests=mock_requests, jwt=mock_jwt):
+        with patch.multiple('vantage6.client', requests=mock_requests,
+                            jwt=mock_jwt):
             client = TestClient.setup_client()
 
-            client.post_task(name=TASK_NAME, image=TASK_IMAGE, collaboration_id=COLLABORATION_ID,
-                             organization_ids=ORGANIZATION_IDS, input_=input_, data_format=serialization)
-
-            # In a request.post call, json is provided with the keyword argument 'json'
-            # call_args provides a tuple with positional arguments followed by a dict with positional arguments
+            client.task.create(
+                name=TASK_NAME, image=TASK_IMAGE,
+                collaboration_id=COLLABORATION_ID,
+                organization_ids=ORGANIZATION_IDS, input_=input_
+            )
+
+            # In a request.post call, json is provided with the keyword
+            # argument 'json'. call_args provides a tuple with positional
+            # arguments followed by a dict with positional arguments
             post_content = mock_requests.post.call_args[1]['json']
 
             post_input = post_content['organizations'][0]['input']
 
         return post_input
 
     @staticmethod
@@ -93,30 +70,36 @@
         mock_result_response = [{'result': mock_result}]
         mock_jwt = TestClient._create_mock_jwt()
 
         mock_requests = MagicMock()
         mock_requests.get.return_value.status_code = 200
         mock_requests.post.return_value.status_code = 200
 
-        user = {'id': FAKE_ID, 'firstname': 'naam', 'organization': {'id': FAKE_ID}}
+        user = {
+            'id': FAKE_ID, 'firstname': 'naam',
+            'organization': {'id': FAKE_ID}
+        }
         organization = {'id': FAKE_ID, 'name': FAKE_NAME}
 
-        # The client will first send a post request for authentication, then for retrieving results.
-        mock_requests.get.return_value.json.side_effect = [user, organization, mock_result_response]
+        # The client will first send a post request for authentication, then
+        # for retrieving results.
+        mock_requests.get.return_value.json.side_effect = \
+            [user, organization, mock_result_response]
 
-        with patch.multiple('vantage6.client', requests=mock_requests, jwt=mock_jwt):
+        with patch.multiple('vantage6.client', requests=mock_requests,
+                            jwt=mock_jwt):
             client = TestClient.setup_client()
 
             results = client.result.from_task(task_id=FAKE_ID)
 
             return results
 
     @staticmethod
-    def setup_client() -> Client:
-        client = Client(HOST, PORT)
+    def setup_client() -> UserClient:
+        client = UserClient(HOST, PORT)
         client.authenticate(FAKE_USERNAME, FAKE_PASSWORD)
         client.setup_encryption(None)
         return client
 
     @staticmethod
     def _create_mock_jwt() -> MagicMock:
         mock_jwt = MagicMock()
```

### Comparing `vantage6-client-3.9.0rc4/vantage6/client/__init__.py` & `vantage6-client-4.0.0a2/vantage6/client/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,679 +1,66 @@
 """
 vantage6 clients
 
 This module is contains a base client. From this base client the container
 client (client used by master algorithms) and the user client are derived.
 """
+from __future__ import annotations
+
 import logging
-import pickle
 import time
 import typing
 import jwt
-import requests
 import pyfiglet
-import json as json_lib
 import itertools
 import sys
 import traceback
 
 from pathlib import Path
 
-from vantage6.common.exceptions import AuthenticationException
-from vantage6.common import bytes_to_base64s, base64s_to_bytes
 from vantage6.common.globals import APPNAME
-from vantage6.common.encryption import RSACryptor, DummyCryptor
+from vantage6.common.encryption import RSACryptor
 from vantage6.common import WhoAmI
-from vantage6.client import serialization, deserialization
+from vantage6.tools import serialization
 from vantage6.client.filter import post_filtering
-from vantage6.client.utils import print_qr_code, LogLevel
+from vantage6.common.client.utils import print_qr_code
+from vantage6.client.utils import LogLevel
+from vantage6.common.task_status import TaskStatus
+from vantage6.common.client.client_base import ClientBase
 
 
 module_name = __name__.split('.')[1]
 
 LEGACY = 'legacy'
 
 
-class ServerInfo(typing.NamedTuple):
-    """
-    Data-class to store the server info.
-
-    Attributes
-    ----------
-    host : str
-        Adress (including protocol, e.g. `https://`) of the vantage6 server
-    port : int
-        Port numer to which the server listens
-    path : str
-        Path of the api, e.g. '/api'
-    """
-    host: str
-    port: int
-    path: str
-
-
-class ClientBase(object):
-    """Common interface to the central server.
-
-    Contains the basis for all other clients, e.g. UserClient, NodeClient and
-    AlgorithmClient. This includes a basic interface to authenticate, send
-    generic requests, create tasks and retrieve results.
-    """
-
-    def __init__(self, host: str, port: int, path: str = '/api') -> None:
-        """Basic setup for the client
-
-        Parameters
-        ----------
-        host : str
-            Adress (including protocol, e.g. `https://`) of the vantage6 server
-        port : int
-            port numer to which the server listens
-        path : str, optional
-            path of the api, by default '/api'
-        """
-
-        self.log = logging.getLogger(module_name)
-
-        # server settings
-        self.__host = host
-        self.__port = port
-        self.__api_path = path
-
-        # tokens
-        self._access_token = None
-        self.__refresh_token = None
-        self.__refresh_url = None
-
-        self.cryptor = None
-        self.whoami = None
-
-    @property
-    def name(self) -> str:
-        """
-        Return the node's/client's name
-
-        Returns
-        -------
-        str
-            Name of the user or node
-        """
-        return self.whoami.name
-
-    @property
-    def headers(self) -> dict:
-        """
-        Defines headers that are sent with each request. This includes the
-        authorization token.
-
-        Returns
-        -------
-        dict
-            Headers
-        """
-        if self._access_token:
-            return {'Authorization': 'Bearer ' + self._access_token}
-        else:
-            return {}
-
-    @property
-    def token(self) -> str:
-        """
-        JWT Authorization token
-
-        Returns
-        -------
-        str
-            JWT token
-        """
-        return self._access_token
-
-    @property
-    def host(self) -> str:
-        """
-        Host including protocol (HTTP/HTTPS)
-
-        Returns
-        -------
-        str
-            Host address of the vantage6 server
-        """
-        return self.__host
-
-    @property
-    def port(self) -> int:
-        """
-        Port on which vantage6 server listens
-
-        Returns
-        -------
-        int
-            Port number
-        """
-        return self.__port
-
-    @property
-    def path(self) -> str:
-        """
-        Path/endpoint at the server where the api resides
-
-        Returns
-        -------
-        str
-            Path to the api
-        """
-        return self.__api_path
-
-    @property
-    def base_path(self) -> str:
-        """
-        Full path to the server URL. Combination of host, port and api-path
-
-        Returns
-        -------
-        str
-            Server URL
-        """
-        if self.__port:
-            return f"{self.host}:{self.port}{self.__api_path}"
-
-        return f"{self.host}{self.__api_path}"
-
-    def generate_path_to(self, endpoint: str) -> str:
-        """Generate URL to endpoint using host, port and endpoint
-
-        Parameters
-        ----------
-        endpoint : str
-            endpoint to which a fullpath needs to be generated
-
-        Returns
-        -------
-        str
-            URL to the endpoint
-        """
-        if endpoint.startswith('/'):
-            path = self.base_path + endpoint
-        else:
-            path = self.base_path + '/' + endpoint
-
-        return path
-
-    def request(self, endpoint: str, json: dict = None, method: str = 'get',
-                params: dict = None, first_try: bool = True,
-                retry: bool = True) -> dict:
-        """Create http(s) request to the vantage6 server
-
-        Parameters
-        ----------
-        endpoint : str
-            Endpoint of the server
-        json : dict, optional
-            payload, by default None
-        method : str, optional
-            Http verb, by default 'get'
-        params : dict, optional
-            URL parameters, by default None
-        first_try : bool, optional
-            Whether this is the first attempt of this request. Default True.
-        retry: bool, optional
-            Try request again after refreshing the token. Default True.
-
-        Returns
-        -------
-        dict
-            Response of the server
-        """
-
-        # get appropiate method
-        rest_method = {
-            'get': requests.get,
-            'post': requests.post,
-            'put': requests.put,
-            'patch': requests.patch,
-            'delete': requests.delete
-        }.get(method.lower(), requests.get)
-
-        # send request to server
-        url = self.generate_path_to(endpoint)
-        self.log.debug(f'Making request: {method.upper()} | {url} | {params}')
-
-        try:
-            response = rest_method(url, json=json, headers=self.headers,
-                                   params=params)
-        except requests.exceptions.ConnectionError as e:
-            # we can safely retry as this is a connection error. And we
-            # keep trying!
-            self.log.error('Connection error... Retrying')
-            self.log.debug(e)
-            time.sleep(1)
-            return self.request(endpoint, json, method, params)
-
-        # TODO: should check for a non 2xx response
-        if response.status_code > 210:
-            self.log.error(
-                f'Server responded with error code: {response.status_code}')
-            try:
-                self.log.error("msg:"+response.json().get("msg", ""))
-            except json_lib.JSONDecodeError:
-                self.log.error('Did not find a message from the server')
-                self.log.debug(response.content)
-
-            if retry:
-                if first_try:
-                    self.refresh_token()
-                    return self.request(endpoint, json, method, params,
-                                        first_try=False)
-                else:
-                    self.log.error("Nope, refreshing the token didn't fix it.")
-
-        return response.json()
-
-    def setup_encryption(self, private_key_file: str) -> None:
-        """Enable the encryption module fot the communication
-
-        This will attach a Crypter object to the client. It will also
-        verify that the public key at the server matches the local
-        private key. In case they differ, the local public key is uploaded
-        to the server.
-
-        Parameters
-        ----------
-        private_key_file : str
-            File path of the private key file
-
-        Raises
-        ------
-        AssertionError
-            If the client is not authenticated
-        """
-        assert self._access_token, \
-            "Encryption can only be setup after authentication"
-        assert self.whoami.organization_id, \
-            "Organization unknown... Did you authenticate?"
-
-        if private_key_file is None:
-            self.cryptor = DummyCryptor()
-            return
-
-        if isinstance(private_key_file, str):
-            private_key_file = Path(private_key_file)
-
-        cryptor = RSACryptor(private_key_file)
-
-        # check if the public-key is the same on the server. If this is
-        # not the case, this node will not be able to read any messages
-        # that are send to him! If this is the case, the new public_key
-        # will be uploaded to the central server
-        organization = self.request(
-            f"organization/{self.whoami.organization_id}")
-        pub_key = organization.get("public_key")
-        upload_pub_key = False
-
-        if pub_key:
-            if cryptor.verify_public_key(pub_key):
-                self.log.info("Public key matches the server key! Good to go!")
-
-            else:
-                self.log.critical(
-                    "Local public key does not match server public key. "
-                    "You will not able to read any messages that are intended "
-                    "for you!"
-                )
-                upload_pub_key = True
-        else:
-            upload_pub_key = True
-
-        # upload public key if required
-        if upload_pub_key:
-            self.request(
-                f"organization/{self.whoami.organization_id}",
-                method="patch",
-                json={"public_key": cryptor.public_key_str}
-            )
-            self.log.info("The public key on the server is updated!")
-
-        self.cryptor = cryptor
-
-    def authenticate(self, credentials: dict,
-                     path: str = "token/user") -> bool:
-        """Authenticate to the vantage6-server
-
-        It allows users, nodes and containers to sign in. Credentials can
-        either be a username/password combination or a JWT authorization
-        token.
-
-        Parameters
-        ----------
-        credentials : dict
-            Credentials used to authenticate
-        path : str, optional
-            Endpoint used for authentication. This differs for users, nodes and
-            containers, by default "token/user"
-
-        Raises
-        ------
-        Exception
-            Failed to authenticate
-
-        Returns
-        -------
-        Bool
-            Whether or not user is authenticated. Alternative is that user is
-            redirected to set up two-factor authentication
-        """
-        if 'username' in credentials:
-            self.log.debug(
-                f"Authenticating user {credentials['username']}...")
-        elif 'api_key' in credentials:
-            self.log.debug('Authenticating node...')
-
-        # authenticate to the central server
-        url = self.generate_path_to(path)
-        response = requests.post(url, json=credentials)
-        data = response.json()
-
-        # handle negative responses
-        if response.status_code > 200:
-            self.log.critical(f"Failed to authenticate: {data.get('msg')}")
-            if response.status_code == 401:
-                raise AuthenticationException("Failed to authenticate")
-            else:
-                raise Exception("Failed to authenticate")
-
-        if 'qr_uri' in data:
-            print_qr_code(data)
-            return False
-        else:
-            # Check if there is an access token. If not, there is a problem
-            # with authenticating
-            if 'access_token' not in data:
-                if 'msg' in data:
-                    raise Exception(data['msg'])
-                else:
-                    raise Exception(
-                        "No access token in authentication response!")
-
-            # store tokens in object
-            self.log.info("Successfully authenticated")
-            self._access_token = data.get("access_token")
-            self.__refresh_token = data.get("refresh_token")
-            self.__refresh_url = data.get("refresh_url")
-            return True
-
-    def refresh_token(self) -> None:
-        """Refresh an expired token using the refresh token
-
-        Raises
-        ------
-        Exception
-            Authentication Error!
-        AssertionError
-            Refresh URL not found
-        """
-        self.log.info("Refreshing token")
-        assert self.__refresh_url, \
-            "Refresh URL not found, did you authenticate?"
-
-        # if no port is specified explicit, then it should be omit the
-        # colon : in the path. Similar (but different) to the property
-        # base_path
-        if self.__port:
-            url = f"{self.__host}:{self.__port}{self.__refresh_url}"
-        else:
-            url = f"{self.__host}{self.__refresh_url}"
-
-        # send request to server
-        response = requests.post(url, headers={
-            'Authorization': 'Bearer ' + self.__refresh_token
-        })
-
-        # server says no!
-        if response.status_code != 200:
-            self.log.critical("Could not refresh token")
-            raise Exception("Authentication Error!")
-
-        self._access_token = response.json()["access_token"]
-        self.__refresh_token = response.json()["refresh_token"]
-
-    # TODO BvB 23-01-23 remove this method in v4+. It is only here for
-    # backwards compatibility
-    def post_task(self, name: str, image: str, collaboration_id: int,
-                  input_='', description='',
-                  organization_ids: list = None,
-                  data_format=LEGACY, database: str = 'default') -> dict:
-        """Post a new task at the server
-
-        It will also encrypt `input_` for each receiving organization.
-
-        Parameters
-        ----------
-        name : str
-            Human readable name for the task
-        image : str
-            Docker image name containing the algorithm
-        collaboration_id : int
-            Collaboration `id` of the collaboration for which the task is
-            intended
-        input_ : str, optional
-            Task input, by default ''
-        description : str, optional
-            Human readable description of the task, by default ''
-        organization_ids : list, optional
-            Ids of organizations (within the collaboration) that need to
-            execute this task, by default None
-        data_format : str, optional
-            Type of data format to use to send and receive
-            data. possible values: 'json', 'pickle', 'legacy'. 'legacy'
-            will use pickle serialization. Default is 'legacy'., by default
-            LEGACY
-        database : str, optional
-            Database label to use for the task, by default 'default'
-
-        Returns
-        -------
-        dict
-            Containing the task meta-data
-
-        Raises
-        ------
-        AssertionError
-            Encryption has not yet been setup.
-        """
-        assert self.cryptor, "Encryption has not yet been setup!"
-
-        if organization_ids is None:
-            organization_ids = []
-
-        if data_format == LEGACY:
-            serialized_input = pickle.dumps(input_)
-        else:
-            # Data will be serialized to bytes in the specified data format.
-            # It will be prepended with 'DATA_FORMAT.' in unicode.
-            serialized_input = data_format.encode() + b'.' \
-                + serialization.serialize(input_, data_format)
-
-        organization_json_list = []
-        for org_id in organization_ids:
-            pub_key = self.request(f"organization/{org_id}").get("public_key")
-            # pub_key = base64s_to_bytes(pub_key)
-            # self.log.debug(pub_key)
-
-            organization_json_list.append({
-                "id": org_id,
-                "input": self.cryptor.encrypt_bytes_to_str(serialized_input,
-                                                           pub_key)
-            })
-
-        return self.request('task', method='post', json={
-            "name": name,
-            "image": image,
-            "collaboration_id": collaboration_id,
-            "description": description,
-            "organizations": organization_json_list,
-            'database': database
-        })
-
-    # TODO BvB 23-01-23 remove this method in v4+ (or make it private?). It is
-    # only here for backwards compatibility.
-    def get_results(self, id_: int = None, state: str = None,
-                    include_task: bool = False, task_id: int = None,
-                    node_id: int = None, params: dict = {}) -> dict:
-        """Get task result(s) from the central server
-
-        Depending if a `id` is specified or not, either a single or a
-        list of results is returned. The input and result field of the
-        result are attempted te be decrypted. This fails if the public
-        key at the server is not derived from the currently private key
-        or when the result is not from your organization.
-
-        Parameters
-        ----------
-        id : int, optional
-            Id of the result, by default None
-        state : str, optional
-            The state of the task (e.g. `open`), by default None
-        include_task : bool, optional
-            Whenever to include the originating task, by default False
-        task_id : int, optional
-            The id of the originating task, this will return all results
-            belonging to this task, by default None
-        node_id : int, optional
-            The id of the node at which this result has been produced,
-            this will return all results from this node, by default None
-        params : dict, optional
-            Additional query parameters, by default {}
-
-        Returns
-        -------
-        dict
-            Containing the result(s)
-        """
-        # Determine endpoint and create dict with query parameters
-        endpoint = 'result' if not id_ else f'result/{id_}'
-
-        extended_params = params.copy()
-        if state:
-            extended_params['state'] = state
-        if include_task:
-            extended_params['include'] = 'task'
-        if task_id:
-            extended_params['task_id'] = task_id
-        if node_id:
-            extended_params['node_id'] = node_id
-
-        # self.log.debug(f"Retrieving results using query parameters:{params}")
-        results = self.request(endpoint=endpoint, params=extended_params)
-
-        if isinstance(results, str):
-            self.log.warn("Requesting results failed")
-            self.log.debug(f"Results message: {results}")
-            return {}
-
-        # hack: in the case that the pagination metadata is included we
-        # need to strip that for decrypting
-        if isinstance(results, dict) and 'data' in results:
-            wrapper = results
-            results = results['data']
-
-        if id_:
-            # Single result
-            self._decrypt_result(results)
-
-        else:
-            # Multiple results
-            for result in results:
-                self._decrypt_result(result)
-
-        if 'wrapper' in locals():
-            wrapper['data'] = results
-            results = wrapper
-
-        return results
-
-    def _decrypt_result(self, result: dict) -> None:
-        """
-        Helper to decrypt the keys 'input' and 'result' in dict.
-
-        Keys are replaced, but object reference remains intact: changes are
-        made *in-place*.
-
-        Parameters
-        ----------
-        result : dict
-            The result dict to decrypt
-
-        Raises
-        ------
-        AssertionError
-            Encryption has not been initialized
-        """
-        assert self.cryptor, "Encryption has not been initialized"
-        cryptor = self.cryptor
-        try:
-            self.log.info('Decrypting input')
-            # TODO this only works when the results belong to the
-            # same organization... We should make different implementation
-            # of get_results
-            result["input"] = cryptor.decrypt_str_to_bytes(result["input"])
-
-        except Exception as e:
-            self.log.debug(e)
-
-        try:
-            if result["result"]:
-                self.log.info('Decrypting result')
-                result["result"] = \
-                    cryptor.decrypt_str_to_bytes(result["result"])
-
-        except ValueError as e:
-            self.log.error("Could not decrypt/decode input or result.")
-            self.log.error(e)
-            # raise
-
-    class SubClient:
-        """
-        Create sub groups of commands using this SubClient
-
-        Parameters
-        ----------
-        parent : UserClient
-            The parent client
-        """
-        def __init__(self, parent) -> None:
-            self.parent: UserClient = parent
-
-
 class UserClient(ClientBase):
     """User interface to the vantage6-server"""
 
-    def __init__(self, *args, verbose=False, log_level='debug',
-                 **kwargs) -> None:
+    def __init__(self, *args, log_level='debug', **kwargs) -> None:
         """Create user client
 
         All paramters from `ClientBase` can be used here.
 
         Parameters
         ----------
-        verbose : bool, optional
-            Whenever to print (info) messages, by default False
         log_level : str, optional
             The log level to use, by default 'debug'
         """
         super(UserClient, self).__init__(*args, **kwargs)
 
         # Replace logger by print logger
-        # TODO in v4+, remove the verbose option and only keep log_level
-        self.log = self._get_logger(verbose, log_level)
+        self.log = self._get_logger(log_level)
 
         # attach sub-clients
         self.util = self.Util(self)
         self.collaboration = self.Collaboration(self)
         self.organization = self.Organization(self)
         self.user = self.User(self)
+        self.run = self.Run(self)
         self.result = self.Result(self)
         self.task = self.Task(self)
         self.role = self.Role(self)
         self.node = self.Node(self)
         self.rule = self.Rule(self)
 
         # Display welcome message
@@ -687,22 +74,20 @@
         self.log.info("Cite us!")
         self.log.info("If you publish your findings obtained using vantage6, ")
         self.log.info("please cite the proper sources as mentioned in:")
         self.log.info("https://vantage6.ai/vantage6/references")
         self.log.info("-" * 60)
 
     @staticmethod
-    def _get_logger(enabled: bool, level: str) -> logging.Logger:
+    def _get_logger(level: str) -> logging.Logger:
         """
         Create print-logger
 
         Parameters
         ----------
-        enabled: bool
-            If true, logging at most detailed level
         level: str
             Desired logging level
 
         Returns
         -------
         logging.Logger
             Logger object
@@ -710,17 +95,15 @@
         # get logger that prints to console
         logger = logging.getLogger()
         logger.handlers.clear()
         logger.addHandler(logging.StreamHandler(sys.stdout))
 
         # set log level
         level = level.upper()
-        if enabled:
-            logger.setLevel(LogLevel.DEBUG.value)
-        elif level not in [lvl.value for lvl in LogLevel]:
+        if level not in [lvl.value for lvl in LogLevel]:
             default_lvl = LogLevel.DEBUG.value
             logger.setLevel(default_lvl)
             logger.warn(
                 f"You set unknown log level {level}. Available levels are: "
                 f"{', '.join([lvl.value for lvl in LogLevel])}. ")
             logger.warn(f"Log level now set to {default_lvl}.")
         else:
@@ -755,23 +138,16 @@
             # printing useful output
             return
 
         # identify the user and the organization to which this user
         # belongs. This is usefull for some client side checks
         try:
             type_ = "user"
-            jwt_payload = jwt.decode(self.token,
-                                     options={"verify_signature": False})
-
-            # FIXME: 'identity' is no longer needed in version 4+. So this if
-            # statement can be removed
-            if 'sub' in jwt_payload:
-                id_ = jwt_payload['sub']
-            elif 'identity' in jwt_payload:
-                id_ = jwt_payload['identity']
+            id_ = jwt.decode(
+                self.token, options={"verify_signature": False})['sub']
 
             user = self.request(f"user/{id_}")
             name = user.get("firstname")
             organization_id = user.get("organization").get("id")
             organization = self.request(f"organization/{organization_id}")
             organization_name = organization.get("name")
 
@@ -787,24 +163,24 @@
             self.log.info(f" --> Name: {name} (id={id_})")
             self.log.info(f" --> Organization: {organization_name} "
                           f"(id={organization_id})")
         except Exception:
             self.log.info('--> Retrieving additional user info failed!')
             self.log.error(traceback.format_exc())
 
-    def wait_for_results(self, task_id: int, sleep: float = 1) -> dict:
+    def wait_for_results(self, task_id: int, interval: float = 1) -> dict:
         """
         Polls the server to check when results are ready, and returns the
         results when the task is completed.
 
         Parameters
         ----------
         task_id: int
             ID of the task that you are waiting for
-        sleep: float
+        interval: float
             Interval in seconds between checks if task is finished. Default 1.
 
         Returns
         -------
         dict
             A dictionary with the results of the task, after it has completed.
         """
@@ -816,30 +192,32 @@
         elif isinstance(self.log, UserClient.Log):
             prev_level = self.log.enabled
             self.log.enabled = False
 
         animation = itertools.cycle(['|', '/', '-', '\\'])
         t = time.time()
 
-        while not self.task.get(task_id)['complete']:
+        while self.task.get(task_id)['status'] != TaskStatus.COMPLETED:
             frame = next(animation)
             sys.stdout.write(
                 f'\r{frame} Waiting for task {task_id} ({int(time.time()-t)}s)'
             )
             sys.stdout.flush()
-            time.sleep(sleep)
+            time.sleep(interval)
         sys.stdout.write('\rDone!                  ')
 
         # Re-enable logging
         if isinstance(self.log, logging.Logger):
             self.log.setLevel(prev_level)
         elif isinstance(self.log, UserClient.Log):
             self.log.enabled = prev_level
 
-        return self.get_results(task_id=task_id)
+        result = self.request('result', params={'task_id': task_id})
+        result = self.result._decrypt_result(result, is_single_result=False)
+        return result
 
     class Util(ClientBase.SubClient):
         """Collection of general utilities"""
 
         def get_server_version(self) -> dict:
             """View the version number of the vantage6-server
 
@@ -1780,53 +1158,57 @@
                 Containing the task data
             """
             params = {}
             params['include'] = 'results' if include_results else None
             return self.parent.request(f'task/{id_}', params=params)
 
         @post_filtering()
-        def list(self, initiator: int = None, initiating_user: int = None,
-                 collaboration: int = None, image: str = None,
-                 parent: int = None, run: int = None,
-                 name: str = None, include_results: bool = False,
-                 description: str = None, database: str = None,
-                 result: int = None, status: str = None, page: int = 1,
-                 per_page: int = 20, include_metadata: bool = True) -> dict:
+        def list(
+            self, initiating_org: int = None, initiating_user: int = None,
+            collaboration: int = None, image: str = None, parent: int = None,
+            job: int = None, name: str = None, include_results: bool = False,
+            description: str = None, database: str = None, run: int = None,
+            status: str = None, user_created: bool = None, page: int = 1,
+            per_page: int = 20, include_metadata: bool = True
+        ) -> dict:
             """List tasks
 
             Parameters
             ----------
             name: str, optional
                 Filter by the name of the task. It will match with a
                 Like operator. I.e. E% will search for task names that
                 start with an 'E'.
-            initiator: int, optional
+            initiating_org: int, optional
                 Filter by initiating organization
             initiating_user: int, optional
                 Filter by initiating user
             collaboration: int, optional
                 Filter by collaboration
             image: str, optional
                 Filter by Docker image name (with LIKE operator)
             parent: int, optional
                 Filter by parent task
-            run: int, optional
-                Filter by run
+            job: int, optional
+                Filter by job id
             include_results : bool, optional
                 Whenever to include the results in the tasks, by default
                 False
             description: str, optional
                 Filter by description (with LIKE operator)
             database: str, optional
                 Filter by database (with LIKE operator)
-            result: int, optional
-                Only show task that contains this result id
+            run: int, optional
+                Only show task that contains this run id
             status: str, optional
                 Filter by task status (e.g. 'active', 'pending', 'completed',
                 'crashed')
+            user_created: bool, optional
+                If True, show only top-level tasks created by users. If False,
+                show only subtasks created by algorithm containers.
             page: int, optional
                 Pagination page, by default 1
             per_page: int, optional
                 Number of items on a single page, by default 20
             include_metadata: bool, optional
                 Whenever to include the pagination metadata. If this is
                 set to False the output is no longer wrapped in a
@@ -1844,39 +1226,37 @@
             list
                 when 'include_metadata' is set to false, it removes the
                 metadata wrapper. I.e. directly returning the 'data'
                 key.
             """
             # if the param is None, it will not be passed on to the
             # request
-            # TODO in v4+, we should change the 'initiator' argument to
-            # a name that distinguishes it better from the initiating user.
-            # Then, we should also change it in the server
             params = {
-                'initiator_id': initiator, 'init_user_id': initiating_user,
+                'init_org_id': initiating_org, 'init_user_id': initiating_user,
                 'collaboration_id': collaboration,
-                'image': image, 'parent_id': parent, 'run_id': run,
+                'image': image, 'parent_id': parent, 'job_id': job,
                 'name': name, 'page': page, 'per_page': per_page,
                 'description': description, 'database': database,
-                'result_id': result, 'status': status,
+                'run_id': run, 'status': status,
             }
             includes = []
             if include_results:
                 includes.append('results')
             if include_metadata:
                 includes.append('metadata')
             params['include'] = includes
+            if user_created is not None:
+                params['is_user_created'] = 1 if user_created else 0
 
             return self.parent.request('task', params=params)
 
         @post_filtering(iterable=False)
         def create(self, collaboration: int, organizations: list, name: str,
-                   image: str, description: str, input: dict,
-                   data_format: str = LEGACY,
-                   database: str = 'default') -> dict:
+                   image: str, description: str, input_: dict,
+                   databases: list[str] = None) -> dict:
             """Create a new task
 
             Parameters
             ----------
             collaboration : int
                 Id of the collaboration to which this task belongs
             organizations : list
@@ -1884,34 +1264,64 @@
                 to execute this task
             name : str
                 Human readable name
             image : str
                 Docker image name which contains the algorithm
             description : str
                 Human readable description
-            input : dict
+            input_ : dict
                 Algorithm input
-            data_format : str, optional
-                IO data format used, by default LEGACY
-            database: str, optional
-                Database name to be used at the node
+            databases: list[str], optional
+                Database names to be used at the node
 
             Returns
             -------
             dict
-                [description]
+                A dictionairy containing data on the created task, or a message
+                from the server if the task could not be created
             """
-            return self.parent.post_task(name, image, collaboration, input,
-                                         description, organizations,
-                                         data_format, database)
+            assert self.parent.cryptor, "Encryption has not yet been setup!"
+
+            if organizations is None:
+                organizations = []
+            if databases is None:
+                databases = ['default']
+            elif isinstance(databases, str):
+                # it is not unlikely that users specify a single database as a
+                # str, in that case we convert it to a list
+                databases = [databases]
+
+            # Data will be serialized in JSON.
+            serialized_input = serialization.serialize(input_)
+
+            # Encrypt the input per organization using that organization's
+            # public key.
+            organization_json_list = []
+            for org_id in organizations:
+                pub_key = self.parent.request(f"organization/{org_id}")\
+                    .get("public_key")
+                organization_json_list.append({
+                    "id": org_id,
+                    "input": self.parent.cryptor.encrypt_bytes_to_str(
+                        serialized_input, pub_key)
+                })
+
+            return self.parent.request('task', method='post', json={
+                "name": name,
+                "image": image,
+                "collaboration_id": collaboration,
+                "description": description,
+                "organizations": organization_json_list,
+                'databases': databases
+            })
 
         def delete(self, id_: int) -> dict:
             """Delete a task
 
-            Also removes the related results.
+            Also removes the related runs.
 
             Parameters
             ----------
             id_ : int
                 Id of the task to be removed
 
             Returns
@@ -1939,56 +1349,52 @@
                 Message from the server
             """
             msg = self.parent.request('/kill/task', method='post', json={
                 'id': id_
             })
             self.parent.log.info(f'--> {msg}')
 
-    class Result(ClientBase.SubClient):
+    class Run(ClientBase.SubClient):
 
         @post_filtering(iterable=False)
         def get(self, id_: int, include_task: bool = False) -> dict:
-            """View a specific result
+            """View a specific run
 
             Parameters
             ----------
             id_ : int
-                id of the result you want to inspect
+                id of the run you want to inspect
             include_task : bool, optional
                 Whenever to include the task or not, by default False
 
             Returns
             -------
             dict
-                Containing the result data
+                Containing the run data
             """
             self.parent.log.info('--> Attempting to decrypt results!')
 
-            # get_results also handles decryption
-            result = self.parent.get_results(id_=id_,
-                                             include_task=include_task)
-            result_data = result.get('result')
-            if result_data:
-                try:
-                    result['result'] = deserialization.load_data(result_data)
-                except Exception as e:
-                    self.parent.log.warn('--> Failed to deserialize')
-                    self.parent.log.debug(e)
+            # get run from the API
+            params = {'include': 'task'} if include_task else {}
+            run = self.parent.request(endpoint=f'run/{id_}', params=params)
 
-            return result
+            # decrypt input
+            run = self._decrypt_input(run_data=run, is_single_run=True)
+
+            return run
 
         @post_filtering()
         def list(self, task: int = None, organization: int = None,
                  state: str = None, node: int = None,
                  include_task: bool = False, started: tuple[str, str] = None,
                  assigned: tuple[str, str] = None,
                  finished: tuple[str, str] = None, port: int = None,
                  page: int = None, per_page: int = None,
                  include_metadata: bool = True) -> dict | list[dict]:
-            """List results
+            """List runs
 
             Parameters
             ----------
             task: int, optional
                 Filter by task id
             organization: int, optional
                 Filter by organization id
@@ -2001,32 +1407,32 @@
             started: tuple[str, str], optional
                 Filter on a range of start times (format: yyyy-mm-dd)
             assigned: tuple[str, str], optional
                 Filter on a range of assign times (format: yyyy-mm-dd)
             finished: tuple[str, str], optional
                 Filter on a range of finished times (format: yyyy-mm-dd)
             port: int, optional
-                Port on which result was computed
+                Port on which run was computed
             page: int, optional
                 Pagination page number, defaults to 1
             per_page: int, optional
                 Number of items per page, defaults to 20
             include_metedata: bool, optional
                 Whenevet to include pagination metadata, defaults to
                 True
 
             Returns
             -------
             dict | list[dict]
                 If include_metadata is True, a dictionary is returned
                 containing the key 'data' which contains a list of
-                results, and a key 'links' which contains the pagination
+                runs, and a key 'links' which contains the pagination
                 metadata.
                 When include_metadata is False, the metadata wrapper
-                is stripped and only a list of results is returned
+                is stripped and only a list of runs is returned
             """
             includes = []
             if include_metadata:
                 includes.append('metadata')
             if include_task:
                 includes.append('task')
 
@@ -2040,47 +1446,27 @@
                 'per_page': per_page, 'include': includes,
                 'started_from': s_from, 'started_till': s_till,
                 'assigned_from': a_from, 'assigned_till': a_till,
                 'finished_from': f_from, 'finished_till': f_till,
                 'port': port
             }
 
-            results = self.parent.get_results(params=params)
+            # get runs from the API
+            runs = self.parent.request(endpoint='run', params=params)
 
-            if isinstance(results, dict):
-                wrapper = results
-                results = results['data']
-
-            cleaned_results = []
-            for result in results:
-                if result.get('result'):
-                    try:
-                        des_res = deserialization.load_data(
-                            result.get('result')
-                        )
-                    except Exception as e:
-                        id_ = result.get('id')
-                        self.parent.log.warn('Could not deserialize result id='
-                                             f'{id_}')
-                        self.parent.log.debug(e)
-                        continue
-                    result['result'] = des_res
-                cleaned_results.append(result)
-
-            if 'wrapper' in locals():
-                wrapper['data'] = cleaned_results
-                cleaned_results = wrapper
+            # decrypt input data
+            runs = self._decrypt_input(run_data=runs, is_single_run=False)
 
-            return cleaned_results
+            return runs
 
         def from_task(
             self, task_id: int, include_task: bool = False
         ) -> typing.List[dict]:
             """
-            Get all results from a specific task
+            Get all algorithm runs from a specific task
 
             Parameters
             ----------
             task_id : int
                 Id of the task to get results from
             include_task : bool, optional
                 Whenever to include the task or not, by default False
@@ -2088,25 +1474,104 @@
             Returns
             -------
             list[dict]
                 Containing the results
             """
             self.parent.log.info('--> Attempting to decrypt results!')
 
-            # get_results also handles decryption
-            results = self.parent.get_results(task_id=task_id,
-                                              include_task=include_task)
-            cleaned_results = []
-            for result in results:
-                if result.get('result'):
-                    des_res = deserialization.load_data(result.get('result'))
-                    result['result'] = des_res
-                cleaned_results.append(result)
+            # get all algorithm runs from a specific task
+            params = {}
+            if include_task:
+                params['include'] = 'task'
+            if task_id:
+                params['task_id'] = task_id
+            runs = self.parent.request(endpoint='run', params=params)
+
+            # decrypt input data
+            runs = self._decrypt_input(run_data=runs, is_single_run=False)
+
+            return runs
+
+        def _decrypt_input(self, run_data: dict, is_single_run: bool) -> dict:
+            """
+            Wrapper function to decrypt and deserialize the input of one or
+            more runs
+
+            Parameters
+            ----------
+            run_data : dict
+                The data of the run(s) to decrypt
+            is_single_run : bool
+                Whether the run_data is a single run or a list of runs
+
+            Returns
+            -------
+            dict
+                Data on the algorithm run(s) with decrypted input
+            """
+            return self.parent._decrypt_field(
+                data=run_data, field='input', is_single_resource=is_single_run
+            )
+
+    class Result(ClientBase.SubClient):
+        """
+        Client to get the results of one or multiple algorithm runs
+        """
+        @post_filtering(iterable=False)
+        def get(self, id_: int) -> dict:
+            """View a specific result
+
+            Parameters
+            ----------
+            id_ : int
+                id of the run you want to inspect
+
+            Returns
+            -------
+            dict
+                Containing the run data
+            """
+            self.parent.log.info('--> Attempting to decrypt results!')
+
+            result = self.parent.request(endpoint=f'result/{id_}')
+            result = self._decrypt_result(
+                result_data=result, is_single_result=True
+            )
+
+            return result['result']
+
+        def from_task(self, task_id: int):
+            self.parent.log.info('--> Attempting to decrypt results!')
+
+            results = self.parent.request('result', {'task_id': task_id})
+            results = self._decrypt_result(results, False)
+            return results
+
+        def _decrypt_result(self, result_data: dict,
+                            is_single_result: bool) -> dict:
+            """
+            Wrapper function to decrypt and deserialize the input of one or
+            more runs
+
+            Parameters
+            ----------
+            result_data : dict
+                The data of the run(s) to decrypt
+            is_single_result : bool
+                Whether the result_data is a single result or a list of results
 
-            return cleaned_results
+            Returns
+            -------
+            dict
+                Data on the algorithm run(s) with decrypted input
+            """
+            return self.parent._decrypt_field(
+                data=result_data, field='result',
+                is_single_resource=is_single_result
+            )
 
     class Rule(ClientBase.SubClient):
 
         @post_filtering(iterable=False)
         def get(self, id_: int) -> dict:
             """View specific rule
 
@@ -2155,222 +1620,7 @@
             includes = ['metadata'] if include_metadata else []
             params = {
                 'page': page, 'per_page': per_page, 'include': includes,
                 'name': name, 'operation': operation, 'scope': scope,
                 'role_id': role
             }
             return self.parent.request('rule', params=params)
-
-
-# TODO remove in v4+ (deprecated for AlgorithmClient but still kept for
-# backwards compatibility)
-class ContainerClient(ClientBase):
-    """ Container interface to the local proxy server (central server).
-
-        An algorithm container should never communicate directly to the
-        central server. Therefore the algorithm container has no
-        internet connection. The algorithm can, however, talk to a local
-        proxy server which has interface to the central server. This way
-        we make sure that the algorithm container does not share stuff
-        with others, and we also can encrypt the results for a specific
-        receiver. Thus this not a interface to the central server but to
-        the local proxy server. However the interface is identical thus
-        we are happy that we can ignore this detail.
-    """
-
-    def __init__(self, token: str, *args, **kwargs):
-        """Container client.
-        A client which can be used by algorithms. All permissions of the
-        container are derived from the token.
-
-        Parameters
-        ----------
-        token : str
-            JWT (container) token, generated by the node
-                the algorithm container runs on
-        """
-        super().__init__(*args, **kwargs)
-
-        # obtain the identity from the token
-        jwt_payload = jwt.decode(
-            token, options={"verify_signature": False})
-
-        # FIXME: 'identity' is no longer needed in version 4+. So this if
-        # statement can be removed
-        if 'sub' in jwt_payload:
-            container_identity = jwt_payload['sub']
-        elif 'identity' in jwt_payload:
-            container_identity = jwt_payload['identity']
-
-        self.image = container_identity.get("image")
-        self.database = container_identity.get('database')
-        self.host_node_id = container_identity.get("node_id")
-        self.collaboration_id = container_identity.get("collaboration_id")
-        self.log.info(
-            f"Container in collaboration_id={self.collaboration_id} \n"
-            f"Key created by node_id {self.host_node_id} \n"
-            f"Can only use image={self.image}"
-        )
-
-        self._access_token = token
-        self.log.debug(f"Access token={self._access_token}")
-
-    def authenticate(self):
-        """ Containers obtain their key via their host Node."""
-        self.log.warn("Containers do not authenticate?!")
-        return
-
-    def refresh_token(self):
-        """ Containers cannot refresh their token.
-
-            TODO we might want to notify node/server about this...
-            TODO make a more usefull exception
-        """
-        raise Exception("Containers cannot refresh!")
-
-    def get_results(self, task_id: int):
-        """ Obtain results from a specific task at the server
-
-            Containers are allowed to obtain the results of their
-            children (having the same run_id at the server). The
-            permissions are checked at te central server.
-
-            :param task_id: id of the task from which you want to obtain
-                the results
-        """
-        results = self.request(
-            f"task/{task_id}/result"
-        )
-
-        res = []
-        # Encryption is not done at the client level for the container.
-        # Although I am not completely sure that the format is always
-        # a pickle.
-        # for result in results:
-        #     self._decrypt_result(result)
-        #     res.append(result.get("result"))
-        #
-        try:
-            res = [pickle.loads(base64s_to_bytes(result.get("result")))
-                   for result in results if result.get("result")]
-        except Exception as e:
-            self.log.error('Unable to unpickle result')
-            self.log.debug(e)
-
-        return res
-
-    def get_algorithm_addresses(self, task_id: int):
-        """
-        Return IP address and port number of other algorithm containers
-        involved in a task so that VPN can be used for communication
-        """
-        results = self.request(f"task/{task_id}/result")
-
-        algorithm_addresses = []
-        for result in results:
-            for port in result['ports']:
-                algorithm_addresses.append({
-                    'ip': result['node']['ip'],
-                    'port': port['port'],
-                    'label': port['label']
-                })
-        return algorithm_addresses
-
-    def get_algorithm_address_by_label(self, task_id: int, label: str) -> str:
-        """
-        Return the IP address plus port number of a given port label
-        """
-        algorithm_addresses = self.get_algorithm_addresses(task_id=task_id)
-        for address in algorithm_addresses:
-            if address['label'] == label:
-                return f"{address['ip']}:{address['port']}"
-        return None
-
-    def get_task(self, task_id: int):
-        return self.request(
-            f"task/{task_id}"
-        )
-
-    def create_new_task(self, input_, organization_ids=[]):
-        """ Create a new (child) task at the central server.
-
-            Containers are allowed to create child tasks (having the
-            same run_id) at the central server. The docker image must
-            be the same as the docker image of this container self.
-
-            :param input_: input to the task
-            :param organization_ids: organization ids which need to
-                execute this task
-        """
-        self.log.debug(f"create new task for {organization_ids}")
-
-        return self.post_task(
-            name="subtask",
-            description=f"task from container on node_id={self.host_node_id}",
-            collaboration_id=self.collaboration_id,
-            organization_ids=organization_ids,
-            input_=input_,
-            image=self.image,
-            database=self.database
-        )
-
-    def get_organizations_in_my_collaboration(self):
-        """ Obtain all organization in the collaboration.
-
-            The container runs in a Node which is part of a single
-            collaboration. This method retrieves all organization data
-            that are within that collaboration. This can be used to
-            target specific organizations in a collaboration.
-        """
-        organizations = self.request(
-            f"collaboration/{self.collaboration_id}/organization")
-        return organizations
-
-    def post_task(self, name: str, image: str, collaboration_id: int,
-                  input_: str = '', description='',
-                  organization_ids: list = [], database='default') -> dict:
-        """ Post a new task at the central server.
-
-            ! To create a new task from the algorithm container you
-            should use the `create_new_task` function !
-
-            Creating a task from a container does need to be encrypted.
-            This is done because the container should never have access
-            to the private key of this organization. The encryption
-            takes place in the local proxy server to which the algorithm
-            communicates (indirectly to the central server). Therefore
-            we needed to overload the post_task function.
-
-            :param name: human-readable name
-            :param image: docker image name of the task
-            :param collaboration_id: id of the collaboration in which
-                the task should run
-            :param input_: input to the task
-            :param description: human-readable description
-            :param organization_ids: ids of the organizations where this
-                task should run
-        """
-        self.log.debug("post task without encryption (is handled by proxy)")
-
-        serialized_input = bytes_to_base64s(pickle.dumps(input_))
-
-        organization_json_list = []
-        for org_id in organization_ids:
-            organization_json_list.append(
-                {
-                    "id": org_id,
-                    "input": serialized_input
-                }
-            )
-
-        return self.request('task', method='post', json={
-            "name": name,
-            "image": image,
-            "collaboration_id": collaboration_id,
-            "description": description,
-            "organizations": organization_json_list,
-            "database": database
-        })
-
-
-# For backwards compatibility
-Client = UserClient
```

### Comparing `vantage6-client-3.9.0rc4/vantage6/client/_version.py` & `vantage6-client-4.0.0a2/vantage6/client/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (3, 9, 0, 'candidate', __build__, 0)
+version_info = (4, 0, 0, 'alpha', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = '' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = '' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-client-3.9.0rc4/vantage6/client/algorithm_client.py` & `vantage6-client-4.0.0a2/vantage6/client/algorithm_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import jwt
-import pickle
+import json as json_lib
+import time
 
-from vantage6.client import ClientBase
-from vantage6.client import base64s_to_bytes, bytes_to_base64s
+from typing import Any
+
+from vantage6.common.client.client_base import ClientBase
+from vantage6.common import base64s_to_bytes, bytes_to_base64s
+from vantage6.common.task_status import TaskStatus
+from vantage6.tools.serialization import serialize
+from vantage6.tools.util import info
 
 
 class AlgorithmClient(ClientBase):
     """
     Interface to communicate between the algorithm container and the central
     server via a local proxy server.
 
@@ -31,32 +37,29 @@
     def __init__(self, token: str, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         # obtain the identity from the token
         jwt_payload = jwt.decode(
             token, options={"verify_signature": False})
 
-        # FIXME: 'identity' is no longer needed in version 4+. So this if
-        # statement can be removed
-        if 'sub' in jwt_payload:
-            container_identity = jwt_payload['sub']
-        elif 'identity' in jwt_payload:
-            container_identity = jwt_payload['identity']
+        container_identity = jwt_payload['sub']
 
         self.image = container_identity.get("image")
-        self.database = container_identity.get('database')
-        self.host_node_id = container_identity.get("node_id")
+        self.databases = container_identity.get('databases', [])
+        self.node_id = container_identity.get("node_id")
         self.collaboration_id = container_identity.get("collaboration_id")
+        self.organization_id = container_identity.get("organization_id")
         self.log.info(
             f"Container in collaboration_id={self.collaboration_id} \n"
-            f"Key created by node_id {self.host_node_id} \n"
+            f"Key created by node_id {self.node_id} \n"
             f"Can only use image={self.image}"
         )
 
         # attach sub-clients
+        self.run = self.Run(self)
         self.result = self.Result(self)
         self.task = self.Task(self)
         self.vpn = self.VPN(self)
         self.organization = self.Organization(self)
         self.collaboration = self.Collaboration(self)
         self.node = self.Node(self)
 
@@ -76,59 +79,195 @@
         Returns
         -------
         dict
             Response from the central server.
         """
         return super().request(*args, **kwargs, retry=False)
 
+    def wait_for_results(self, task_id: int, interval: float = 1) -> list:
+        """
+        Poll the central server until results are available and then return
+        them.
+
+        Parameters
+        ----------
+        task_id: int
+            ID of the task for which the results should be obtained.
+        interval: float
+            Interval in seconds to wait between checking server for results.
+
+        Returns
+        -------
+        list
+            List of task results.
+        """
+        while self.task.get(task_id)['status'] != TaskStatus.COMPLETED:
+            info(f"Waiting for results of task {task_id}...")
+            time.sleep(interval)
+        info("Done!")
+
+        return self.result.from_task(task_id)
+
+    def _multi_page_request(self, endpoint: str, params: dict = None) -> dict:
+        """
+        Make multiple requests to the central server to get all pages of a list
+        of results.
+
+        Parameters
+        ----------
+        endpoint: str
+            Endpoint to which the request should be made.
+        params: dict
+            Parameters to be passed to the request.
+
+        Returns
+        -------
+        dict
+            Response from the central server.
+        """
+        if params is None:
+            params = {}
+        # get first page
+        page = 1
+        params["page"] = page
+        response = self.request(endpoint, params=params)
+
+        # append next pages (if any)
+        links = response.get("links")
+        while links and links.get("next"):
+            page += 1
+            params["page"] = page
+            response["data"] += self.request(endpoint, params=params)["data"]
+            links = response.get("links")
+
+        return response['data']
+
+    class Run(ClientBase.SubClient):
+        """
+        Algorithm Run client for the algorithm container.
+
+        This client is used to obtain algorithm runs of tasks with the same
+        job_id from the central server.
+        """
+
+        def get(self, id_) -> dict:
+            """
+            Obtain a specific algorithm run from the central server.
+
+            Parameters
+            ----------
+            id_: int
+                ID of the algorithm run that should be obtained.
+
+            Returns
+            -------
+            dict
+                Algorithm run data.
+            """
+            return self.parent.request(f"run/{id_}")
+
+        def from_task(self, task_id: int) -> list:
+            """
+            Obtain algorithm runs from a specific task at the server.
+
+            Containers are allowed to obtain the runs of their children
+            (having the same job_id at the server). The permissions are checked
+            at te central server.
+
+            Note that the returned results are not decrypted. The algorithm is
+            responsible for decrypting the results.
+
+            Parameters
+            ----------
+            task_id: int
+                ID of the task from which you want to obtain the algorithm runs
+
+            Returns
+            -------
+            list
+                List of algorithm run data. The type of the results depends on
+                the algorithm.
+            """
+            # TODO do we need this function? It may be used to collect data
+            # on subtasks but usually only the results are accessed, which is
+            # done with the function below.
+            return self.parent._multi_page_request(
+                "run", params={"task_id": task_id}
+            )
+
     class Result(ClientBase.SubClient):
         """
         Result client for the algorithm container.
 
-        This client is used to obtain results of tasks with the same run_id
-        from the central server.
+        This client is used to get results from the central server.
         """
+        def get(self, id_: int) -> Any:
+            """
+            Obtain a specific result from the central server.
+
+            Parameters
+            ----------
+            id_: int
+                ID of the algorithm run of which the result should be obtained.
 
-        def get(self, task_id: int) -> list:
+            Returns
+            -------
+            Any
+                Result of the algorithm run.
+            """
+            response = self.parent.request(f"result/{id_}")
+
+            # Encryption is not done at the client level for the container. The
+            # algorithm developer is responsible for decrypting the results.
+            self.parent.log.info('--> Attempting to decode results!')
+            result = None
+            if response.get('result'):
+                result = json_lib.loads(
+                    base64s_to_bytes(response.get('result')).decode()
+                )
+            return result
+
+        def from_task(self, task_id: int) -> list[Any]:
             """
             Obtain results from a specific task at the server.
 
             Containers are allowed to obtain the results of their children
-            (having the same run_id at the server). The permissions are checked
+            (having the same job_id at the server). The permissions are checked
             at te central server.
 
-            Note that the returned results are not decrypted. The algorithm is
-            responisble for decrypting the results.
+            Results are decrypted by the proxy server and decoded here before
+            returning them to the algorithm.
 
             Parameters
             ----------
             task_id: int
                 ID of the task from which you want to obtain the results
 
             Returns
             -------
-            list
+            list[Any]
                 List of results. The type of the results depends on the
                 algorithm.
             """
-            results = self.parent.request(
-                f"task/{task_id}/result"
+            results = self.parent._multi_page_request(
+                "result", params={"task_id": task_id}
             )
 
-            decoded_results = []
             # Encryption is not done at the client level for the container. The
             # algorithm developer is responsible for decrypting the results.
-            # FIXME Are we completely sure that the format is always a pickle?
+            decoded_results = []
             try:
                 decoded_results = [
-                    pickle.loads(base64s_to_bytes(result.get("result")))
+                    json_lib.loads(
+                        base64s_to_bytes(result.get("result")).decode()
+                    )
                     for result in results if result.get("result")
                 ]
             except Exception as e:
-                self.parent.log.error('Unable to unpickle result')
+                self.parent.log.error('Unable to load results')
                 self.parent.log.debug(e)
 
             return decoded_results
 
     class Task(ClientBase.SubClient):
         """
         A task client for the algorithm container.
@@ -150,69 +289,68 @@
                 Dictionary containing the task information
             """
             return self.parent.request(
                 f"task/{task_id}"
             )
 
         def create(
-            self, input_: bytes, organization_ids: list[int] = None,
+            self, input_: bytes, organizations: list[int] = None,
             name: str = "subtask", description: str = None
         ) -> dict:
             """
             Create a new (child) task at the central server.
 
             Containers are allowed to create child tasks (having the
-            same run_id) at the central server. The docker image must
+            same job_id) at the central server. The docker image must
             be the same as the docker image of this container self.
 
             Parameters
             ----------
             input_ : bytes
                 Input to the task. Should be b64 encoded.
-            organization_ids : list[int]
+            organizations : list[int]
                 List of organization IDs that should execute the task.
             name: str, optional
                 Name of the subtask
             description : str, optional
                 Description of the subtask
 
             Returns
             -------
             dict
                 Dictionary containing information on the created task
             """
-            if organization_ids is None:
-                organization_ids = []
-            self.parent.log.debug(
-                f"Creating new subtask for {organization_ids}")
+            if not organizations:
+                organizations = []
+            self.parent.log.debug(f"Creating new subtask for {organizations}")
 
             description = (
                 description or
-                f"task from container on node_id={self.parent.host_node_id}"
+                f"task from container on node_id={self.parent.node_id}"
             )
 
             # serializing input. Note that the input is not encrypted here, but
             # in the proxy server (self.parent.request())
-            serialized_input = bytes_to_base64s(pickle.dumps(input_))
+            serialized_input = bytes_to_base64s(serialize(input_))
             organization_json_list = []
-            for org_id in organization_ids:
+            for org_id in organizations:
                 organization_json_list.append(
                     {
                         "id": org_id,
                         "input": serialized_input
                     }
                 )
 
             return self.parent.request('task', method='post', json={
                 "name": name,
                 "image": self.parent.image,
                 "collaboration_id": self.parent.collaboration_id,
                 "description": description,
                 "organizations": organization_json_list,
-                "database": self.parent.database
+                "databases": self.parent.databases
             })
 
     class VPN(ClientBase.SubClient):
         """
         A VPN client for the algorithm container.
 
         It provides functions to obtain the IP addresses of other containers.
@@ -329,19 +467,19 @@
             organizations in a collaboration.
 
             Returns
             -------
             list[dict]
                 List of organizations in the collaboration.
             """
-            organizations = self.parent.request(
-                "organization",
-                params={"collaboration_id": self.parent.collaboration_id}
+            return self.parent._multi_page_request(
+                endpoint="organization", params={
+                    "collaboration_id": self.parent.collaboration_id
+                }
             )
-            return organizations
 
     class Collaboration(ClientBase.SubClient):
         """
         Get information about the collaboration.
         """
         def get(self) -> dict:
             """
@@ -365,8 +503,8 @@
 
             Returns
             -------
             dict
                 Dictionary containing data on the node this algorithm is
                 running on.
             """
-            return self.parent.request(f"node/{self.parent.host_node_id}")
+            return self.parent.request(f"node/{self.parent.node_id}")
```

### Comparing `vantage6-client-3.9.0rc4/vantage6/client/filter.py` & `vantage6-client-4.0.0a2/vantage6/client/filter.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc4/vantage6/tools/util.py` & `vantage6-client-4.0.0a2/vantage6/tools/util.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.9.0rc4/vantage6_client.egg-info/PKG-INFO` & `vantage6-client-4.0.0a2/vantage6_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.9.0rc4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 4.0.0a2 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.9.0rc4/vantage6_client.egg-info/SOURCES.txt` & `vantage6-client-4.0.0a2/vantage6_client.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,23 @@
 tests/test_deserialization.py
 tests/test_docker_wrapper.py
 tests/test_serialization.py
 vantage6/client/__build__
 vantage6/client/__init__.py
 vantage6/client/_version.py
 vantage6/client/algorithm_client.py
-vantage6/client/deserialization.py
 vantage6/client/exceptions.py
 vantage6/client/filter.py
-vantage6/client/serialization.py
 vantage6/client/utils.py
 vantage6/tools/__init__.py
-vantage6/tools/data_format.py
-vantage6/tools/deserialization.py
-vantage6/tools/dispatch_rpc.py
-vantage6/tools/docker_wrapper.py
+vantage6/tools/decorators.py
 vantage6/tools/exceptions.py
 vantage6/tools/mock_client.py
 vantage6/tools/serialization.py
 vantage6/tools/util.py
-vantage6/tools/wrapper.py
+vantage6/tools/wrap.py
+vantage6/tools/wrappers.py
 vantage6_client.egg-info/PKG-INFO
 vantage6_client.egg-info/SOURCES.txt
 vantage6_client.egg-info/dependency_links.txt
 vantage6_client.egg-info/requires.txt
 vantage6_client.egg-info/top_level.txt
```

