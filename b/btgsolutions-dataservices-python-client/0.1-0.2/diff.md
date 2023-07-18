# Comparing `tmp/btgsolutions-dataservices-python-client-0.1.tar.gz` & `tmp/btgsolutions-dataservices-python-client-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/btgsolutions-dataservices-python-client-0.1.tar", last modified: Fri Jul  7 12:19:52 2023, max compression
+gzip compressed data, was "dist/btgsolutions-dataservices-python-client-0.2.tar", last modified: Tue Jul 18 14:20:54 2023, max compression
```

## Comparing `btgsolutions-dataservices-python-client-0.1.tar` & `btgsolutions-dataservices-python-client-0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-07-06 19:30:06.000000 btgsolutions-dataservices-python-client-0.1/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2108 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1385 2023-07-07 12:14:25.000000 btgsolutions-dataservices-python-client-0.1/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1334 2023-07-06 19:33:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/config.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/exceptions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/rest/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      136 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/rest/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1297 2023-07-06 20:59:23.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/rest/authenticator.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3001 2023-07-06 20:55:43.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/rest/historical_candles.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5752 2023-07-06 19:56:51.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/rest/intraday_candles.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/websocket/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/websocket/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6667 2023-07-06 20:13:04.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/websocket/websocket_client.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/websocket/websocket_default_functions.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices_python_client.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2108 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices_python_client.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      841 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices_python_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       68 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices_python_client.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices_python_client.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       67 2023-07-06 19:30:06.000000 btgsolutions-dataservices-python-client-0.1/requirements.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-07 12:19:52.000000 btgsolutions-dataservices-python-client-0.1/setup.cfg
--rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-07-06 19:43:18.000000 btgsolutions-dataservices-python-client-0.1/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-07-06 19:30:06.000000 btgsolutions-dataservices-python-client-0.2/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2108 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1385 2023-07-07 12:14:25.000000 btgsolutions-dataservices-python-client-0.2/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       93 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1364 2023-07-17 22:13:34.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/config.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/exceptions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/rest/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      136 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/rest/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1297 2023-07-06 20:59:23.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/rest/authenticator.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3001 2023-07-06 20:55:43.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/rest/historical_candles.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5752 2023-07-06 19:56:51.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/rest/intraday_candles.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/websocket/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       45 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/websocket/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7354 2023-07-17 22:58:09.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/websocket/websocket_client.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      270 2023-07-06 19:30:05.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/websocket/websocket_default_functions.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices_python_client.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2108 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices_python_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      841 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices_python_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       68 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices_python_client.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices_python_client.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       67 2023-07-06 19:30:06.000000 btgsolutions-dataservices-python-client-0.2/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-18 14:20:54.000000 btgsolutions-dataservices-python-client-0.2/setup.cfg
+-rwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-07-18 14:20:17.000000 btgsolutions-dataservices-python-client-0.2/setup.py
```

### Comparing `btgsolutions-dataservices-python-client-0.1/PKG-INFO` & `btgsolutions-dataservices-python-client-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgsolutions-dataservices-python-client
-Version: 0.1
+Version: 0.2
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client
 Author: BTG Solutions Data Services powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # BTG Solutions - Data Service
         
         It's a Python library to get Brazilian Financial Market Data.
```

### Comparing `btgsolutions-dataservices-python-client-0.1/README.md` & `btgsolutions-dataservices-python-client-0.2/README.md`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/config.py` & `btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,10 +23,12 @@
 valid_delayed_options = list(set([i.split('_')[1] for i in keys_socket]))
 valid_feeds = list(set([i.split('_')[0] for i in keys_socket]))
 
 def valid_ws_options(feed, target):
     return list(set(socket_urls[f'{feed}_{target}']))
 
 
-### Rest
 
+MAX_WS_RECONNECT_RETRIES = 5
+
+### Rest
 url_apis = "https://dataservices.btgpactualsolutions.com/api/v2"
```

### Comparing `btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/exceptions.py` & `btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/exceptions.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/rest/authenticator.py` & `btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/rest/authenticator.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/rest/historical_candles.py` & `btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/rest/historical_candles.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/rest/intraday_candles.py` & `btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/rest/intraday_candles.py`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices/websocket/websocket_client.py` & `btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices/websocket/websocket_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 from typing import Optional, List
 from ..exceptions import WSTypeError, DelayedError, FeedError
 from ..rest import Authenticator
-from ..config import valid_feeds, valid_ws_options, valid_delayed_options, socket_urls
+from ..config import valid_feeds, valid_ws_options, valid_delayed_options, socket_urls, MAX_WS_RECONNECT_RETRIES
 from .websocket_default_functions import _on_open, _on_message, _on_error, _on_close
 import websocket 
 import json
 import ssl
 import threading
- 
+
 class WebSocketClient:
     """
     This class connects with BTG Solutions Data Services WebSocket, receiving trade and index data, in real time or delayed.
 
     * Main use case:
 
     >>> from btgsolutions_dataservices import WebSocketClient
@@ -66,19 +66,20 @@
         target:Optional[str] = 'realtime',
         ws_type:Optional[str] = 'trade',
         instruments:Optional[List[str]] = [],
         ssl:Optional[bool] = True,
         **kwargs,
     ):
         self.api_key = api_key
-        self.token = Authenticator(self.api_key).token
-        self.protocol_str = {"Sec-WebSocket-Protocol": self.token}
         self.instruments = instruments
         self.ssl = ssl
 
+        self.__authenticator = Authenticator(self.api_key)
+        self.__nro_reconnect_retries = 0
+
         if feed not in valid_feeds:
             raise FeedError(
                 f"Must provide a valid 'feed' parameter. Valid options are: {valid_feeds}"
             )
         if target not in valid_delayed_options:
             raise DelayedError(
                 f"Must provide a valid 'target' parameter. Valid options are: {valid_delayed_options}"
@@ -97,14 +98,15 @@
     
     def run(
         self,
         on_open = None,
         on_message = None,
         on_error = None,
         on_close = None,
+        reconnect=True
     ):
         """
         Initializes a connection to websocket and subscribes to the instruments, if it was passed in the class initialization.
 
         Parameters
         ----------
         on_open: function
@@ -129,45 +131,58 @@
         on_close: function
             - Called when connection is closed.
             - Arguments: 
                 1. close_status_code.
                 2. close_msg.
             - Field is not required. 
             - Default: prints a message that the connection was closed.
+        reconnect: bool
+            Try reconnect if connection is closed.
+            Field is not required.
+            Default: True.
         """
         if on_open is None:
             on_open = _on_open
         if on_message is None:
             on_message = _on_message
         if on_error is None:
             on_error = _on_error
         if on_close is None:
             on_close = _on_close
 
         def intermediary_on_open(ws):
             on_open()
             if self.instruments:
                 self.subscribe(self.instruments)
+            self.__nro_reconnect_retries = 0
 
         def intermediary_on_message(ws, data):
             on_message(data)
 
         def intermediary_on_error(ws, error):
             on_error(error)
 
         def intermediary_on_close(ws, close_status_code, close_msg):
             on_close(close_status_code, close_msg)
+            
+            if reconnect:
+                if self.__nro_reconnect_retries == MAX_WS_RECONNECT_RETRIES:
+                    print(f"### Fail retriyng reconnect")
+                    return
+                self.__nro_reconnect_retries +=1
+                print(f"### Reconnecting.... Attempts: {self.__nro_reconnect_retries}/{MAX_WS_RECONNECT_RETRIES}")
+                self.run(on_open, on_message, on_error, on_close, reconnect)
 
         self.ws = websocket.WebSocketApp(
             url=self.url,
             on_open=intermediary_on_open,
             on_message=intermediary_on_message,
             on_error=intermediary_on_error,
-            on_close=intermediary_on_close, 
-            header=self.protocol_str
+            on_close=intermediary_on_close,
+            header={"Sec-WebSocket-Protocol": self.__authenticator.token}
         )
 
         ssl_conf = {} if self.ssl else {"sslopt": {"cert_reqs": ssl.CERT_NONE}}
         wst = threading.Thread(target=self.ws.run_forever, kwargs=ssl_conf)
         wst.daemon = True
         wst.start()
```

### Comparing `btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices_python_client.egg-info/PKG-INFO` & `btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgsolutions-dataservices-python-client
-Version: 0.1
+Version: 0.2
 Summary: Python package containing several classes and data for extracting and manipulating market and trading data.
 Home-page: https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client
 Author: BTG Solutions Data Services powered by BTG Pactual Solutions
 License: UNKNOWN
 Description: # BTG Solutions - Data Service
         
         It's a Python library to get Brazilian Financial Market Data.
```

### Comparing `btgsolutions-dataservices-python-client-0.1/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt` & `btgsolutions-dataservices-python-client-0.2/btgsolutions_dataservices_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btgsolutions-dataservices-python-client-0.1/setup.py` & `btgsolutions-dataservices-python-client-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         with open(requirementPath) as f:
             install_requires = f.read().splitlines()
 
 description = "Python package containing several classes and data for extracting and manipulating market and trading data."
 
 setup(
     name='btgsolutions-dataservices-python-client',
-    version='0.1',
+    version='0.2',
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="BTG Solutions Data Services powered by BTG Pactual Solutions",
     packages=find_packages(),
     url="https://github.com/BTG-Pactual-Solutions/btgsolutions-dataservices-python-client",
     install_requires=install_requires,
```

