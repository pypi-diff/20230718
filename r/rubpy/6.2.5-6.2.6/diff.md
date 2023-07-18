# Comparing `tmp/rubpy-6.2.5.tar.gz` & `tmp/rubpy-6.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.2.5.tar", last modified: Thu Jun 29 13:17:33 2023, max compression
+gzip compressed data, was "rubpy-6.2.6.tar", last modified: Tue Jul 18 01:20:09 2023, max compression
```

## Comparing `rubpy-6.2.5.tar` & `rubpy-6.2.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.295670 rubpy-6.2.5/
--rw-rw-rw-   0        0        0     3378 2023-06-29 13:17:33.295670 rubpy-6.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.256893 rubpy-6.2.5/rubpy/
--rw-rw-rw-   0        0        0      240 2023-06-29 13:16:44.000000 rubpy-6.2.5/rubpy/__init__.py
--rw-rw-rw-   0        0        0    44119 2023-06-29 13:13:18.000000 rubpy-6.2.5/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.278092 rubpy-6.2.5/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.5/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.288661 rubpy-6.2.5/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.2.5/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.5/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    27137 2023-06-15 19:36:00.000000 rubpy-6.2.5/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.5/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     6772 2023-06-29 12:36:38.000000 rubpy-6.2.5/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.288661 rubpy-6.2.5/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    12030 2023-06-16 08:31:13.000000 rubpy-6.2.5/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.288661 rubpy-6.2.5/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.5/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.295670 rubpy-6.2.5/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.5/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.278092 rubpy-6.2.5/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3378 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 13:17:33.295670 rubpy-6.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-06-29 13:16:58.000000 rubpy-6.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.777094 rubpy-6.2.6/
+-rw-rw-rw-   0        0        0     3378 2023-07-18 01:20:09.777094 rubpy-6.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.730214 rubpy-6.2.6/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-06-29 13:16:44.000000 rubpy-6.2.6/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    44856 2023-07-18 01:17:24.000000 rubpy-6.2.6/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.761471 rubpy-6.2.6/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.6/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.761471 rubpy-6.2.6/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.2.6/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.6/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    27137 2023-06-15 19:36:00.000000 rubpy-6.2.6/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.6/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     6772 2023-06-29 12:36:38.000000 rubpy-6.2.6/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.761471 rubpy-6.2.6/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    11464 2023-07-18 01:15:37.000000 rubpy-6.2.6/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.777094 rubpy-6.2.6/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.6/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.777094 rubpy-6.2.6/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.6/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.761471 rubpy-6.2.6/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 01:20:09.777094 rubpy-6.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-07-18 01:17:55.000000 rubpy-6.2.6/setup.py
```

### Comparing `rubpy-6.2.5/PKG-INFO` & `rubpy-6.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.5
+Version: 6.2.6
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.5 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.6 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.5/README.md` & `rubpy-6.2.6/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/client.py` & `rubpy-6.2.6/rubpy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         'package': 'web.rubika.ir',
         'platform': 'Web',
         'app_name': 'Main',
         'user_agent': ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
                        'AppleWebKit/537.36 (KHTML, like Gecko)'
                        'Chrome/102.0.0.0 Safari/537.36'),
         'api_version': '6',
-        'app_version': '4.3.3'
+        'app_version': '4.3.5'
     }
 
     def __init__(self,
         session,
         proxy=None,
         logger=None,
         timeout=20,
@@ -423,14 +423,37 @@
         return await self(methods.groups.GetGroupAdminAccessList(group_guid, member_guid))
 
     async def set_group_timer(self, group_guid: str, time: int):
         return await self(methods.groups.EditGroupInfo(group_guid, slow_mode=time, updated_parameters=['slow_mode']))
 
 # ---------------- Messages Methods ----------------
 
+    async def custom_send_message(self,
+        object_guid: str,
+        message=None,
+        reply_to_message_id: str = None,
+        file: bytes = None,
+        file_inline: dict = None,
+        *args, **kwargs
+    ) -> dict:
+        if object_guid.lower() in ['me', 'self', 'cloud']:
+            object_guid = self._guid
+
+        if file:
+            file = await self.upload(file, *args, **kwargs)
+            for key, value in file_inline.items():
+                file[key] = value
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=message,
+                file_inline=file,
+                reply_to_message_id=reply_to_message_id))
+
     async def send_message(self,
         object_guid: str,
         message=None,
         reply_to_message_id: str = None,
         file_inline=None,
         type: str = methods.messages.File,
         thumb: bool = True, *args, **kwargs
```

### Comparing `rubpy-6.2.5/rubpy/crypto/crypto.py` & `rubpy-6.2.6/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/gadgets/classino.py` & `rubpy-6.2.6/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/gadgets/exceptions.py` & `rubpy-6.2.6/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/gadgets/grouping.py` & `rubpy-6.2.6/rubpy/gadgets/grouping.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/gadgets/methods.py` & `rubpy-6.2.6/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/gadgets/thumbnail.py` & `rubpy-6.2.6/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/network/connection.py` & `rubpy-6.2.6/rubpy/network/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,16 @@
                     upload_url,
                     headers={
                         'auth': self._client._auth,
                         'file-id': id,
                         'total-part': str(total),
                         'part-number': str(index + 1),
                         'chunk-size': str(len(data)),
-                        'access-hash-send': access_hash_send
+                        'access-hash-send': access_hash_send,
+                        'User-Agent': self._client._user_agent
                     },
                     data=data
                 )
                 result = await result.json()
                 if callable(callback):
                     try:
                         await callback(len(file), index * chunk)
@@ -195,38 +196,19 @@
 
     async def download(self, dc_id, file_id,
                        access_hash, chunk=131072, callback=None):
         url = (await self._dcs()).storages[str(dc_id)]
         headers = {
             'file-id': str(file_id),
             'auth': self._client._auth,
-            'access-hash-rec': access_hash}
-        async with self._connection.post(url, headers=headers) as result:
-            if result.status != 200:
-                raise exceptions.InternalProblem(
-                    'the server is not responding')
-
-            data = b''
-            total = int(result.headers.get('total_length', None))
-
-            async for chunk in result.content.iter_chunked(chunk):
-                data += chunk
-                if callable(callback):
-                    try:
-                        await callback(total, len(data))
-
-                    except exceptions.CancelledError:
-                        self._client._logger.info(
-                            'download media cancelled (%s) (%s)', headers, url)
-                        return None
-
-                    except Exception:
-                        pass
-
-            return data
+            'access-hash-rec': access_hash,
+            'User-Agent': self._client._user_agent}
+        async with aiohttp.ClientSession() as connection:
+            async with connection.post(url, headers=headers) as result:
+                return await result.read()
 
     async def handel_update(self, name, update):
         handlers = self._client._handlers.copy()
         for func, handler in handlers.items():
             try:
                 # if handler is empty filters
                 if isinstance(handler, type):
```

### Comparing `rubpy-6.2.5/rubpy/network/proxies.py` & `rubpy-6.2.6/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/sessions/sqliteSession.py` & `rubpy-6.2.6/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/sessions/stringSession.py` & `rubpy-6.2.6/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/structs/handlers.py` & `rubpy-6.2.6/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/structs/models.py` & `rubpy-6.2.6/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/structs/results.py` & `rubpy-6.2.6/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy/structs/struct.py` & `rubpy-6.2.6/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/rubpy.egg-info/PKG-INFO` & `rubpy-6.2.6/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.5
+Version: 6.2.6
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.5 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.6 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.5/rubpy.egg-info/SOURCES.txt` & `rubpy-6.2.6/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.5/setup.py` & `rubpy-6.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.2.5',
+    version = '6.2.6',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

