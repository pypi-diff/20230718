# Comparing `tmp/metaplanet_room_chat-0.0.1.tar.gz` & `tmp/metaplanet_room_chat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaplanet_room_chat-0.0.1.tar", last modified: Wed Jul 12 11:03:56 2023, max compression
+gzip compressed data, was "metaplanet_room_chat-0.0.3.tar", last modified: Tue Jul 18 03:32:18 2023, max compression
```

## Comparing `metaplanet_room_chat-0.0.1.tar` & `metaplanet_room_chat-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 chishijie   (501) staff       (20)        0 2023-07-12 11:03:56.942175 metaplanet_room_chat-0.0.1/
--rw-r--r--   0 chishijie   (501) staff       (20)      223 2023-07-12 11:03:56.941967 metaplanet_room_chat-0.0.1/PKG-INFO
--rw-r--r--   0 chishijie   (501) staff       (20)       29 2023-07-12 10:26:20.000000 metaplanet_room_chat-0.0.1/README.md
--rw-r--r--   0 chishijie   (501) staff       (20)      636 2023-07-12 11:03:16.000000 metaplanet_room_chat-0.0.1/pyproject.toml
--rw-r--r--   0 chishijie   (501) staff       (20)       38 2023-07-12 11:03:56.942225 metaplanet_room_chat-0.0.1/setup.cfg
-drwxr-xr-x   0 chishijie   (501) staff       (20)        0 2023-07-12 11:03:56.939708 metaplanet_room_chat-0.0.1/src/
-drwxr-xr-x   0 chishijie   (501) staff       (20)        0 2023-07-12 11:03:56.940782 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat/
--rw-r--r--   0 chishijie   (501) staff       (20)        0 2023-07-12 10:20:47.000000 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat/__init__.py
--rw-r--r--   0 chishijie   (501) staff       (20)      831 2023-07-12 10:20:02.000000 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat/client.py
--rw-r--r--   0 chishijie   (501) staff       (20)      144 2023-07-12 10:21:57.000000 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat/config.py
--rw-r--r--   0 chishijie   (501) staff       (20)     1488 2023-07-12 10:21:56.000000 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat/handlers.py
-drwxr-xr-x   0 chishijie   (501) staff       (20)        0 2023-07-12 11:03:56.941714 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat.egg-info/
--rw-r--r--   0 chishijie   (501) staff       (20)      223 2023-07-12 11:03:56.000000 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat.egg-info/PKG-INFO
--rw-r--r--   0 chishijie   (501) staff       (20)      407 2023-07-12 11:03:56.000000 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat.egg-info/SOURCES.txt
--rw-r--r--   0 chishijie   (501) staff       (20)        1 2023-07-12 11:03:56.000000 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat.egg-info/dependency_links.txt
--rw-r--r--   0 chishijie   (501) staff       (20)       24 2023-07-12 11:03:56.000000 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat.egg-info/requires.txt
--rw-r--r--   0 chishijie   (501) staff       (20)       21 2023-07-12 11:03:56.000000 metaplanet_room_chat-0.0.1/src/metaplanet_room_chat.egg-info/top_level.txt
+drwxr-xr-x   0 chishijie   (501) staff       (20)        0 2023-07-18 03:32:18.905208 metaplanet_room_chat-0.0.3/
+-rw-r--r--   0 chishijie   (501) staff       (20)      915 2023-07-18 03:29:51.000000 metaplanet_room_chat-0.0.3/GUIDE.MD
+-rw-r--r--   0 chishijie   (501) staff       (20)     1109 2023-07-18 03:32:18.905015 metaplanet_room_chat-0.0.3/PKG-INFO
+-rw-r--r--   0 chishijie   (501) staff       (20)      106 2023-07-18 03:29:54.000000 metaplanet_room_chat-0.0.3/README.md
+-rw-r--r--   0 chishijie   (501) staff       (20)      634 2023-07-18 03:30:06.000000 metaplanet_room_chat-0.0.3/pyproject.toml
+-rw-r--r--   0 chishijie   (501) staff       (20)       38 2023-07-18 03:32:18.905260 metaplanet_room_chat-0.0.3/setup.cfg
+drwxr-xr-x   0 chishijie   (501) staff       (20)        0 2023-07-18 03:32:18.902003 metaplanet_room_chat-0.0.3/src/
+drwxr-xr-x   0 chishijie   (501) staff       (20)        0 2023-07-18 03:32:18.903621 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat/
+-rw-r--r--   0 chishijie   (501) staff       (20)        0 2023-07-12 10:20:47.000000 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat/__init__.py
+-rw-r--r--   0 chishijie   (501) staff       (20)     1101 2023-07-18 03:22:15.000000 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat/client.py
+-rw-r--r--   0 chishijie   (501) staff       (20)       28 2023-07-12 11:15:49.000000 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat/config.py
+-rw-r--r--   0 chishijie   (501) staff       (20)     1502 2023-07-12 11:16:55.000000 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat/handlers.py
+drwxr-xr-x   0 chishijie   (501) staff       (20)        0 2023-07-18 03:32:18.904764 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat.egg-info/
+-rw-r--r--   0 chishijie   (501) staff       (20)     1109 2023-07-18 03:32:18.000000 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat.egg-info/PKG-INFO
+-rw-r--r--   0 chishijie   (501) staff       (20)      416 2023-07-18 03:32:18.000000 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 chishijie   (501) staff       (20)        1 2023-07-18 03:32:18.000000 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 chishijie   (501) staff       (20)       24 2023-07-18 03:32:18.000000 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat.egg-info/requires.txt
+-rw-r--r--   0 chishijie   (501) staff       (20)       21 2023-07-18 03:32:18.000000 metaplanet_room_chat-0.0.3/src/metaplanet_room_chat.egg-info/top_level.txt
```

### Comparing `metaplanet_room_chat-0.0.1/pyproject.toml` & `metaplanet_room_chat-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metaplanet_room_chat"
-version = "0.0.1"
+version = "0.0.3"
 authors = [
   { name="Charles Meow", email="chishijie85@gmail.com" },
 ]
 description = "metaplanet room chat client"
-readme = "README.md"
+readme = "GUIDE.MD"
 dependencies = [
     "websocket_client>=1.6.0"
 ]
 
 
-
 # OR
 # [tool.setuptools.packages.find]
 # All the following settings are optional:
 # where = ["src"]  # ["."] by default
 #include = ["mypackage*"]  # ["*"] by default
 #exclude = ["mypackage.tests*"]  # empty by default
 #namespaces = false  # true by default
```

### Comparing `metaplanet_room_chat-0.0.1/src/metaplanet_room_chat/client.py` & `metaplanet_room_chat-0.0.3/src/metaplanet_room_chat/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import websocket
 import socket
 import json 
-from .config import DEBUG, WS_URL
+from .config import DEBUG
 from .handlers import Cmds, Handlers, decodePacket, encodePacket
 
 if DEBUG:
 	websocket.enableTrace(True) 
 
-def doConnect():
+def doConnect(ws: str, token: str, uid: int, roomId: int, on_receive = None):
+	config={
+		"token":token,
+		"uid":uid,
+		"roomId":roomId
+	}
 	def on_message(wsapp, message):
 		"""
 		接收消息处理函数
 		"""
 		print(f"on_message, packet: {message}")
 		packet = decodePacket(message)
 		cmd = packet["cmd"]
 		# 根据cmd获取处理器
 		handler = Handlers[cmd]
+		if(cmd == Cmds["ROOM_MSG_RECEIVE_S"]):
+			handler = on_receive	
 		if handler is None:
 			print(f"cmd: {cmd}对应的handler不存在")
-		handler(packet, wsapp)
+		handler(packet, wsapp, config)
 		
 	def on_connect(wsapp):
 		"""
 		连接事件处理函数
 		"""
 		print(f"on_open")
 		#发起第一个指令
 		wsapp.send(encodePacket(Cmds["CONNECT_C"]));
 		
-	wsapp = websocket.WebSocketApp(WS_URL, on_message=on_message, on_open=on_connect)
-	wsapp.run_forever() 
+	wsapp = websocket.WebSocketApp(ws, on_message=on_message, on_open=on_connect)
+	wsapp.run_forever(ping_interval=20, ping_timeout=10, ping_payload="This is an optional ping payload") 
 
-if __name__ == "__main__":
-	doConnect()
+# if __name__ == "__main__":
+# 	doConnect()
```

### Comparing `metaplanet_room_chat-0.0.1/src/metaplanet_room_chat/handlers.py` & `metaplanet_room_chat-0.0.3/src/metaplanet_room_chat/handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 
 import json
 
-from . config import ROOM_ID, TOKEN
-
 
 Cmds={
     "CONNECT_C": 100,
     "CONNECT_S": 101,
     "LOGIN_C": 102,
     "LOGIN_S": 103,
     "ENTER_ROOM_C": 104,
@@ -27,39 +25,39 @@
 def decodePacket(jsonData: str):
 	"""
 	报文解码
 	"""
 	packet= json.loads(jsonData)
 	return packet 
 
-def connect_handler(packet: dict, client):
+def connect_handler(packet: dict, client, config):
     """
 	connnect_s处理函数
 	"""
     print(f"connect handler")
-    sendPacket = encodePacket(Cmds["LOGIN_C"], data={"token": TOKEN})                
+    sendPacket = encodePacket(Cmds["LOGIN_C"], data={"token": config["token"]})                
     client.send(sendPacket)
     
-def login_handler(packet: dict, client):
+def login_handler(packet: dict, client, config):
     """
 	login_s处理函数
 	"""
     print(f"login handler")
-    sendPacket = encodePacket(Cmds["ENTER_ROOM_C"], data={"roomId": ROOM_ID})                
+    sendPacket = encodePacket(Cmds["ENTER_ROOM_C"], data={"roomId": config["roomId"]})                
     client.send(sendPacket)
     
-def room_enter_handler(packet: dict, client):
+def room_enter_handler(packet: dict, client, config):
 	"""
 	room_enter_s处理函数
 	"""
 	print(f"room enter handler")
 	if packet["data"]["roomId"] is None:
 		print(f"[ERROR]房间登录失败")
 	
-def msg_receive_handler(packet: dict, client):
+def msg_receive_handler(packet: dict, client, config):
 	"""
 	房间消息接收处理器
 	"""
 	print(f"收到房间消息:{packet}")
 
 Handlers={
     Cmds["CONNECT_S"]: connect_handler,
```

