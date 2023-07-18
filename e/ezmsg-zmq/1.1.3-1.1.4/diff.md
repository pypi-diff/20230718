# Comparing `tmp/ezmsg-zmq-1.1.3.tar.gz` & `tmp/ezmsg-zmq-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmsg-zmq-1.1.3.tar", last modified: Thu Jul 13 15:38:22 2023, max compression
+gzip compressed data, was "ezmsg-zmq-1.1.4.tar", last modified: Tue Jul 18 00:37:02 2023, max compression
```

## Comparing `ezmsg-zmq-1.1.3.tar` & `ezmsg-zmq-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/ezmsg/zmq/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/ezmsg/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/ezmsg/zmq/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/ezmsg/zmq/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:38:22.774459 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 15:38:22.000000 ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-13 15:38:22.778459 ezmsg-zmq-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 15:38:11.000000 ezmsg-zmq-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:37:02.344862 ezmsg-zmq-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-18 00:36:48.000000 ezmsg-zmq-1.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-18 00:37:02.344862 ezmsg-zmq-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-18 00:36:48.000000 ezmsg-zmq-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:37:02.340862 ezmsg-zmq-1.1.4/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:37:02.344862 ezmsg-zmq-1.1.4/ezmsg/zmq/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 00:36:48.000000 ezmsg-zmq-1.1.4/ezmsg/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 00:36:48.000000 ezmsg-zmq-1.1.4/ezmsg/zmq/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-18 00:36:48.000000 ezmsg-zmq-1.1.4/ezmsg/zmq/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:37:02.344862 ezmsg-zmq-1.1.4/ezmsg_zmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-18 00:37:02.000000 ezmsg-zmq-1.1.4/ezmsg_zmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-18 00:37:02.000000 ezmsg-zmq-1.1.4/ezmsg_zmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:37:02.000000 ezmsg-zmq-1.1.4/ezmsg_zmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:37:02.000000 ezmsg-zmq-1.1.4/ezmsg_zmq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 00:37:02.000000 ezmsg-zmq-1.1.4/ezmsg_zmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 00:37:02.000000 ezmsg-zmq-1.1.4/ezmsg_zmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-18 00:36:48.000000 ezmsg-zmq-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-18 00:37:02.344862 ezmsg-zmq-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-18 00:36:48.000000 ezmsg-zmq-1.1.4/setup.py
```

### Comparing `ezmsg-zmq-1.1.3/LICENSE.txt` & `ezmsg-zmq-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezmsg-zmq-1.1.3/PKG-INFO` & `ezmsg-zmq-1.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg-zmq
-Version: 1.1.3
+Version: 1.1.4
 Summary: ZeroMQ units for ezmsg
 Home-page: https://github.com/iscoe/ezmsg
 Author: Preston Peranich
 Author-email: pperanich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-zmq-1.1.3/ezmsg/zmq/units.py` & `ezmsg-zmq-1.1.4/ezmsg/zmq/units.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,46 +43,55 @@
 
 class ZMQSenderSettings(ez.Settings):
     write_addr: str
     zmq_topic: str
     multipart: bool = False
 
 
+class ZMQSenderState(ez.State):
+    context: zmq.asyncio.Context
+    socket: zmq.asyncio.Socket
+    monitor: zmq.asyncio.Socket
+    poller: zmq.Poller
+
+
 class ZMQSenderUnit(ez.Unit):
     """
     Represents a node in a Labgraph graph that subscribes to messages in a
     Labgraph topic and forwards them by writing to a ZMQ socket.
 
     Args:
         write_addr: The address to which ZMQ data should be written.
         zmq_topic: The ZMQ topic being sent.
     """
 
     INPUT = ez.InputStream(ZMQMessage)
 
     SETTINGS: ZMQSenderSettings
+    STATE: ZMQSenderState
 
     def initialize(self) -> None:
-        self.context = zmq.asyncio.Context()
-        self.socket = self.context.socket(zmq.PUB)
-        self.monitor = self.socket.get_monitor_socket()
+        self.STATE.context = zmq.asyncio.Context()
+        self.STATE.socket = self.STATE.context.socket(zmq.PUB)
+        self.STATE.monitor = self.STATE.socket.get_monitor_socket()
         ez.logger.debug(f"{self}:binding to {self.SETTINGS.write_addr}")
-        self.socket.bind(self.SETTINGS.write_addr)
+        self.STATE.socket.bind(self.SETTINGS.write_addr)
         self.has_subscribers = False
 
     def shutdown(self) -> None:
-        self.monitor.close()
-        self.socket.close()
+        self.STATE.monitor.close()
+        self.STATE.socket.close()
+        self.STATE.context.term()
 
     @ez.task
     async def _socket_monitor(self) -> None:
         while True:
-            monitor_result = await self.monitor.poll(100, zmq.POLLIN)
+            monitor_result = await self.STATE.monitor.poll(100, zmq.POLLIN)
             if monitor_result:
-                data = await self.monitor.recv_multipart()
+                data = await self.STATE.monitor.recv_multipart()
                 evt = parse_monitor_message(data)
 
                 event = evt["event"]
 
                 if event == zmq.EVENT_ACCEPTED:
                     ez.logger.debug(f"{self}:subscriber joined")
                     self.has_subscribers = True
@@ -94,32 +103,39 @@
                     break
 
     @ez.subscriber(INPUT)
     async def zmq_subscriber(self, message: ZMQMessage) -> None:
         while not self.has_subscribers:
             await asyncio.sleep(STARTUP_WAIT_TIME)
         if self.SETTINGS.multipart is True:
-            await self.socket.send_multipart(
+            await self.STATE.socket.send_multipart(
                 (bytes(self.SETTINGS.zmq_topic, "UTF-8"), message.data),
                 flags=zmq.NOBLOCK,
             )
         else:
-            await self.socket.send(
+            await self.STATE.socket.send(
                 b"".join((bytes(self.SETTINGS.zmq_topic, "UTF-8"), message.data)),
                 flags=zmq.NOBLOCK,
             )
 
 
 class ZMQPollerSettings(ez.Settings):
     read_addr: str
     zmq_topic: str
     poll_time: float = POLL_TIME
     multipart: bool = False
 
 
+class ZMQPollerState(ez.State):
+    context: zmq.asyncio.Context
+    socket: zmq.asyncio.Socket
+    monitor: zmq.asyncio.Socket
+    poller: zmq.Poller
+
+
 class ZMQPollerUnit(ez.Unit):
     """
     Represents a node in the graph which polls data from ZMQ.
     Data polled from ZMQ are subsequently pushed to the rest of the
     graph as a ZMQMessage.
 
     Args:
@@ -133,37 +149,39 @@
             An optional ZMQ event code specifying the event which,
             if encountered by the monitor, should signal the termination
             of this particular node's activity.
     """
 
     OUTPUT = ez.OutputStream(ZMQMessage)
     SETTINGS: ZMQPollerSettings
+    STATE: ZMQPollerState
 
     def initialize(self) -> None:
-        self.context = zmq.asyncio.Context()
-        self.socket = self.context.socket(zmq.SUB)
-        self.monitor = self.socket.get_monitor_socket()
-        self.socket.connect(self.SETTINGS.read_addr)
-        self.socket.subscribe(self.SETTINGS.zmq_topic)
+        self.STATE.context = zmq.asyncio.Context()
+        self.STATE.socket = self.STATE.context.socket(zmq.SUB)
+        self.STATE.monitor = self.STATE.socket.get_monitor_socket()
+        self.STATE.socket.connect(self.SETTINGS.read_addr)
+        self.STATE.socket.subscribe(self.SETTINGS.zmq_topic)
 
-        self.poller = zmq.Poller()
-        self.poller.register(self.socket, zmq.POLLIN)
+        self.STATE.poller = zmq.Poller()
+        self.STATE.poller.register(self.STATE.socket, zmq.POLLIN)
 
         self.socket_open = False
 
     def shutdown(self) -> None:
-        self.monitor.close()
-        self.socket.close()
+        self.STATE.monitor.close()
+        self.STATE.socket.close()
+        self.STATE.context.term()
 
     @ez.task
     async def socket_monitor(self) -> None:
         while True:
-            monitor_result = await self.monitor.poll(100, zmq.POLLIN)
+            monitor_result = await self.STATE.monitor.poll(100, zmq.POLLIN)
             if monitor_result:
-                data = await self.monitor.recv_multipart()
+                data = await self.STATE.monitor.recv_multipart()
                 evt = parse_monitor_message(data)
 
                 event = evt["event"]
 
                 if event == zmq.EVENT_CONNECTED:
                     self.socket_open = True
                 elif event == zmq.EVENT_CLOSED:
@@ -185,16 +203,16 @@
     @ez.publisher(OUTPUT)
     async def zmq_publisher(self) -> AsyncGenerator:
         # Wait for socket connection
         while not self.socket_open:
             await asyncio.sleep(POLL_TIME)
 
         while self.socket_open:
-            poll_result = await self.socket.poll(
+            poll_result = await self.STATE.socket.poll(
                 self.SETTINGS.poll_time * 1000, zmq.POLLIN
             )
             if poll_result:
                 if self.SETTINGS.multipart is True:
-                    _, data = await self.socket.recv_multipart()
+                    _, data = await self.STATE.socket.recv_multipart()
                 else:
-                    data = await self.socket.recv()
+                    data = await self.STATE.socket.recv()
                 yield self.OUTPUT, ZMQMessage(data)
```

### Comparing `ezmsg-zmq-1.1.3/ezmsg_zmq.egg-info/PKG-INFO` & `ezmsg-zmq-1.1.4/ezmsg_zmq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg-zmq
-Version: 1.1.3
+Version: 1.1.4
 Summary: ZeroMQ units for ezmsg
 Home-page: https://github.com/iscoe/ezmsg
 Author: Preston Peranich
 Author-email: pperanich@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-zmq-1.1.3/setup.cfg` & `ezmsg-zmq-1.1.4/setup.cfg`

 * *Files identical despite different names*

