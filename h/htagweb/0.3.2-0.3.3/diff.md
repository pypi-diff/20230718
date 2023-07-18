# Comparing `tmp/htagweb-0.3.2.tar.gz` & `tmp/htagweb-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.3.2.tar", max compression
+gzip compressed data, was "htagweb-0.3.3.tar", max compression
```

## Comparing `htagweb-0.3.2.tar` & `htagweb-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-07-17 13:00:40.710421 htagweb-0.3.2/LICENSE
--rw-r--r--   0        0        0     3148 2023-07-17 13:00:40.710421 htagweb-0.3.2/README.md
--rw-r--r--   0        0        0     9938 2023-07-17 13:00:41.018432 htagweb-0.3.2/htagweb/__init__.py
--rw-r--r--   0        0        0     2225 2023-07-17 13:00:40.710421 htagweb-0.3.2/htagweb/crypto.py
--rw-r--r--   0        0        0     3732 2023-07-17 13:00:40.710421 htagweb-0.3.2/htagweb/manager.py
--rw-r--r--   0        0        0     5541 2023-07-17 13:00:40.710421 htagweb-0.3.2/htagweb/uidprocess.py
--rw-r--r--   0        0        0     1124 2023-07-17 13:00:41.018432 htagweb-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 htagweb-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-18 07:00:12.071597 htagweb-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3148 2023-07-18 07:00:12.071597 htagweb-0.3.3/README.md
+-rw-r--r--   0        0        0     9938 2023-07-18 07:00:12.351596 htagweb-0.3.3/htagweb/__init__.py
+-rw-r--r--   0        0        0     2225 2023-07-18 07:00:12.071597 htagweb-0.3.3/htagweb/crypto.py
+-rw-r--r--   0        0        0     3794 2023-07-18 07:00:12.071597 htagweb-0.3.3/htagweb/manager.py
+-rw-r--r--   0        0        0     5541 2023-07-18 07:00:12.071597 htagweb-0.3.3/htagweb/uidprocess.py
+-rw-r--r--   0        0        0     1124 2023-07-18 07:00:12.351596 htagweb-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 htagweb-0.3.3/PKG-INFO
```

### Comparing `htagweb-0.3.2/LICENSE` & `htagweb-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.2/README.md` & `htagweb-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.2/htagweb/__init__.py` & `htagweb-0.3.3/htagweb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.3.2" # auto updated
+__version__ = "0.3.3" # auto updated
 
 """
 WebServer & WebServerWS
 ~~~~~~~~~~~~~~~~~~~~~~~~
 - new versions of oldest WebHTTP & WebWS (nearly compatibles)
 - concept of an htag app application server (manager), which communicate with child process, with queue
 - Htag Apps runned in a process, per user (real isolation!)
```

### Comparing `htagweb-0.3.2/htagweb/crypto.py` & `htagweb-0.3.3/htagweb/crypto.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.2/htagweb/manager.py` & `htagweb-0.3.3/htagweb/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,48 +63,49 @@
     writer.close()
     await writer.wait_closed()
 
 
 class Manager:
     def __init__(self,port=17788):
         self.port=port
-        self._srv=None
+        self._task=None
 
     def is_server(self):
-        return self._srv!=None
+        return self._task!=None
 
     async def __aenter__(self):
         await self.start()
         return self
 
     async def __aexit__(self, *args):
         await self.stop()
 
     async def start(self):
         """ start server part """
-        if self._srv==None:
+        if self._task==None:
             try:
-                self._srv = await asyncio.start_server( manager_server, '127.0.0.1', self.port)
+                self._server = asyncio.start_server( manager_server, '127.0.0.1', self.port)
+                self._task=await asyncio.create_task( self._server )
                 return True
             except:
-                self._srv=None
+                self._task=None
                 return False
         else:
             raise Exception("Already started")
-            
+
     async def stop(self):
-        if self._srv:
+        if self._task:
             try:
                 await self.killall()
             except:
                 pass
             await asyncio.sleep(0.1)
-            self._srv.close()
-            await self._srv.wait_closed()
-            self._srv=None
+            self._task.close()
+            await self._task.wait_closed()
+            self._task=None
 
     def __getattr__(self,name:str):
         async def _(*a,**k):
             reader, writer = await asyncio.open_connection("127.0.0.1", self.port)
             question = pickle.dumps( (name,a,k) )
             # logger.debug('Sending data of size: %s',len(question))
             writer.write(question)
```

### Comparing `htagweb-0.3.2/htagweb/uidprocess.py` & `htagweb-0.3.3/htagweb/uidprocess.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.2/pyproject.toml` & `htagweb-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.3.2" # auto-updated
+version = "0.3.3" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
```

### Comparing `htagweb-0.3.2/PKG-INFO` & `htagweb-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.3.2
+Version: 0.3.3
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
```

