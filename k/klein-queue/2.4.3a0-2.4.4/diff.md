# Comparing `tmp/klein_queue-2.4.3a0.tar.gz` & `tmp/klein_queue-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klein_queue-2.4.3a0.tar", last modified: Tue Jun 21 14:24:47 2022, max compression
+gzip compressed data, was "dist/klein_queue-2.4.4.tar", last modified: Tue Jul 18 13:45:34 2023, max compression
```

## Comparing `klein_queue-2.4.3a0.tar` & `klein_queue-2.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 nick.etherington (1957169981) 1293359979        0 2022-06-21 14:24:47.078567 klein_queue-2.4.3a0/
--rw-r--r--   0 nick.etherington (1957169981) 1293359979     9136 2022-05-30 16:21:19.000000 klein_queue-2.4.3a0/LICENSE.txt
--rw-r--r--   0 nick.etherington (1957169981) 1293359979       40 2022-06-21 14:12:59.000000 klein_queue-2.4.3a0/MANIFEST.in
--rw-r--r--   0 nick.etherington (1957169981) 1293359979     2560 2022-06-21 14:24:47.078358 klein_queue-2.4.3a0/PKG-INFO
--rw-r--r--   0 nick.etherington (1957169981) 1293359979     2228 2022-05-30 16:21:19.000000 klein_queue-2.4.3a0/README.md
--rw-r--r--   0 nick.etherington (1957169981) 1293359979       38 2022-06-21 14:24:47.078611 klein_queue-2.4.3a0/setup.cfg
--rw-r--r--   0 nick.etherington (1957169981) 1293359979     1637 2022-06-21 14:12:59.000000 klein_queue-2.4.3a0/setup.py
-drwxr-xr-x   0 nick.etherington (1957169981) 1293359979        0 2022-06-21 14:24:47.071704 klein_queue-2.4.3a0/src/
-drwxr-xr-x   0 nick.etherington (1957169981) 1293359979        0 2022-06-21 14:24:47.072676 klein_queue-2.4.3a0/src/klein_queue/
--rw-r--r--   0 nick.etherington (1957169981) 1293359979       20 2022-05-26 13:41:11.000000 klein_queue-2.4.3a0/src/klein_queue/__init__.py
--rw-r--r--   0 nick.etherington (1957169981) 1293359979     1312 2022-05-30 16:21:19.000000 klein_queue-2.4.3a0/src/klein_queue/errors.py
-drwxr-xr-x   0 nick.etherington (1957169981) 1293359979        0 2022-06-21 14:24:47.078096 klein_queue-2.4.3a0/src/klein_queue/rabbitmq/
--rw-r--r--   0 nick.etherington (1957169981) 1293359979      267 2022-05-26 13:41:11.000000 klein_queue-2.4.3a0/src/klein_queue/rabbitmq/__init__.py
--rw-r--r--   0 nick.etherington (1957169981) 1293359979     2249 2022-05-30 16:21:19.000000 klein_queue-2.4.3a0/src/klein_queue/rabbitmq/api.py
--rw-r--r--   0 nick.etherington (1957169981) 1293359979    11730 2022-05-30 16:21:19.000000 klein_queue-2.4.3a0/src/klein_queue/rabbitmq/connect.py
--rw-r--r--   0 nick.etherington (1957169981) 1293359979    12391 2022-05-30 16:21:19.000000 klein_queue-2.4.3a0/src/klein_queue/rabbitmq/consumer.py
--rw-r--r--   0 nick.etherington (1957169981) 1293359979     4596 2022-05-30 16:21:19.000000 klein_queue-2.4.3a0/src/klein_queue/rabbitmq/exceptions.py
--rw-r--r--   0 nick.etherington (1957169981) 1293359979     7847 2022-05-30 16:21:19.000000 klein_queue-2.4.3a0/src/klein_queue/rabbitmq/publisher.py
-drwxr-xr-x   0 nick.etherington (1957169981) 1293359979        0 2022-06-21 14:24:47.074564 klein_queue-2.4.3a0/src/klein_queue.egg-info/
--rw-r--r--   0 nick.etherington (1957169981) 1293359979     2560 2022-06-21 14:24:46.000000 klein_queue-2.4.3a0/src/klein_queue.egg-info/PKG-INFO
--rw-r--r--   0 nick.etherington (1957169981) 1293359979      558 2022-06-21 14:24:47.000000 klein_queue-2.4.3a0/src/klein_queue.egg-info/SOURCES.txt
--rw-r--r--   0 nick.etherington (1957169981) 1293359979        1 2022-06-21 14:24:46.000000 klein_queue-2.4.3a0/src/klein_queue.egg-info/dependency_links.txt
--rw-r--r--   0 nick.etherington (1957169981) 1293359979       70 2022-06-21 14:24:46.000000 klein_queue-2.4.3a0/src/klein_queue.egg-info/requires.txt
--rw-r--r--   0 nick.etherington (1957169981) 1293359979       12 2022-06-21 14:24:46.000000 klein_queue-2.4.3a0/src/klein_queue.egg-info/top_level.txt
--rw-r--r--   0 nick.etherington (1957169981) 1293359979        1 2022-06-21 14:16:32.000000 klein_queue-2.4.3a0/src/klein_queue.egg-info/zip-safe
--rw-r--r--   0 nick.etherington (1957169981) 1293359979       45 2022-06-21 14:24:30.000000 klein_queue-2.4.3a0/src/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)     9136 2023-07-18 13:45:06.000000 klein_queue-2.4.4/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-18 13:45:06.000000 klein_queue-2.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-07-18 13:45:34.000000 klein_queue-2.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2023-07-18 13:45:06.000000 klein_queue-2.4.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 13:45:34.000000 klein_queue-2.4.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-18 13:45:06.000000 klein_queue-2.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2406 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11730 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/connect.py
+-rw-rw-rw-   0 root         (0) root         (0)    12614 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7847 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/klein_queue/rabbitmq/publisher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 13:45:34.000000 klein_queue-2.4.4/src/klein_queue.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-18 13:45:06.000000 klein_queue-2.4.4/src/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `klein_queue-2.4.3a0/LICENSE.txt` & `klein_queue-2.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.3a0/PKG-INFO` & `klein_queue-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klein_queue
-Version: 2.4.3a0
+Version: 2.4.4
 Summary: RabbitMQ integration
 Home-page: http://github.com/mdcatapult/py-queue
 Author: Medicines Discovery Catapult
 Author-email: SoftwareEngineering@md.catapult.org.uk
 License: Apache V2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `klein_queue-2.4.3a0/README.md` & `klein_queue-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.3a0/setup.py` & `klein_queue-2.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.3a0/src/klein_queue/errors.py` & `klein_queue-2.4.4/src/klein_queue/errors.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.3a0/src/klein_queue/rabbitmq/api.py` & `klein_queue-2.4.4/src/klein_queue/rabbitmq/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 
 class ApiClient:
 
     def __init__(self, config):
         self._config = config
         self._cache = {}
 
-    def list_queues(self, exchange, flush=False):
+    def list_queues(self, exchange, flush=False, timeout=None):
         """Utility to retrieve queues attached to exchange
         configured user for connection should have
         management permissions.
 
         `exchange`: `str` the exchange to query.
         `flush`: `bool` whether or not to flush the results cache.
+        `timeout`: `int` the time to wait for the request
         """
 
         if flush:
             del self._cache[exchange]
 
         if exchange in self._cache and "timestamp" in self._cache[exchange]:
             diff = time.time() - self._cache[exchange]["timestamp"]
@@ -47,18 +48,18 @@
         if isinstance(host, list):
             host = host[0]
 
         # TODO: Implement other vhosts than default.
         endpoint = f"/api/exchanges/%%2f/{exchange}/bindings/source"
         url = f'http://{host}:{self._config.get("rabbitmq.management_port")}{endpoint}'
 
-        response = requests.get(url, auth=(
-            self._config.get("rabbitmq.username"),
-            self._config.get("rabbitmq.password"))
-        )
+        response = requests.get(url,
+                                auth=(self._config.get("rabbitmq.username"),
+                                      self._config.get("rabbitmq.password")),
+                                timeout=timeout)
         queues = [q["destination"]
                   for q in response.json() if q["destination_type"] == "queue"]
 
         self._cache[exchange] = {
             "queues": queues,
             "timestamp": time.time()
         }
```

### Comparing `klein_queue-2.4.3a0/src/klein_queue/rabbitmq/connect.py` & `klein_queue-2.4.4/src/klein_queue/rabbitmq/connect.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.3a0/src/klein_queue/rabbitmq/consumer.py` & `klein_queue-2.4.4/src/klein_queue/rabbitmq/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # -*- coding: utf-8 -*-
+import functools
 import json
 import logging
-import functools
-import threading
 import queue
-from .connect import _Connection
+import threading
+import time
+
 from ..errors import KleinQueueError
+from .connect import _Connection
 
 LOGGER = logging.getLogger(__name__)
 
 
 class _MessageWorker(threading.Thread):
     """
     Message worker class
@@ -165,14 +167,20 @@
             LOGGER.info("Auto-acknowledged message # %s", basic_deliver.delivery_tag)
 
         # decode
         body = body.decode('utf-8')
 
         self._message_queue.put((body, properties, basic_deliver))
 
+    def on_channel_closed(self, channel, reason):
+        if not self._closing:
+            LOGGER.info('Channel closed, try and reconnect in 5 seconds')
+            time.sleep(5)
+            self.reconnect()
+
     def _stop_activity(self):
         if self._channel:
             LOGGER.debug('Sending a Basic.Cancel RPC command to RabbitMQ')
             self._channel.basic_cancel(self._consumer_tag, self.on_cancelok)
 
         # stop worker threads
         for worker in self._workers:
```

### Comparing `klein_queue-2.4.3a0/src/klein_queue/rabbitmq/exceptions.py` & `klein_queue-2.4.4/src/klein_queue/rabbitmq/exceptions.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.3a0/src/klein_queue/rabbitmq/publisher.py` & `klein_queue-2.4.4/src/klein_queue/rabbitmq/publisher.py`

 * *Files identical despite different names*

### Comparing `klein_queue-2.4.3a0/src/klein_queue.egg-info/PKG-INFO` & `klein_queue-2.4.4/src/klein_queue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klein-queue
-Version: 2.4.3a0
+Version: 2.4.4
 Summary: RabbitMQ integration
 Home-page: http://github.com/mdcatapult/py-queue
 Author: Medicines Discovery Catapult
 Author-email: SoftwareEngineering@md.catapult.org.uk
 License: Apache V2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `klein_queue-2.4.3a0/src/klein_queue.egg-info/SOURCES.txt` & `klein_queue-2.4.4/src/klein_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

