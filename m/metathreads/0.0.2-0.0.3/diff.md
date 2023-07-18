# Comparing `tmp/metathreads-0.0.2.tar.gz` & `tmp/metathreads-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metathreads-0.0.2.tar", last modified: Sun Jul 16 14:42:55 2023, max compression
+gzip compressed data, was "metathreads-0.0.3.tar", last modified: Tue Jul 18 08:21:52 2023, max compression
```

## Comparing `metathreads-0.0.2.tar` & `metathreads-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 14:42:55.196747 metathreads-0.0.2/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 metathreads-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       24 2023-07-13 14:53:51.000000 metathreads-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4742 2023-07-16 14:42:55.196747 metathreads-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3554 2023-07-13 14:54:38.000000 metathreads-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 14:42:55.177610 metathreads-0.0.2/metathreads/
--rw-rw-rw-   0        0        0       38 2023-07-13 14:53:20.000000 metathreads-0.0.2/metathreads/__init__.py
--rw-rw-rw-   0        0        0      408 2023-07-13 09:42:18.000000 metathreads-0.0.2/metathreads/config.py
--rw-rw-rw-   0        0        0     1378 2023-07-13 12:19:15.000000 metathreads-0.0.2/metathreads/constants.py
--rw-rw-rw-   0        0        0    14495 2023-07-13 14:51:30.000000 metathreads-0.0.2/metathreads/metathreads.py
--rw-rw-rw-   0        0        0     7848 2023-07-16 14:39:41.000000 metathreads-0.0.2/metathreads/request_util.py
--rw-rw-rw-   0        0        0     3800 2023-07-13 12:32:50.000000 metathreads-0.0.2/metathreads/util.py
-drwxrwxrwx   0        0        0        0 2023-07-16 14:42:55.193234 metathreads-0.0.2/metathreads.egg-info/
--rw-rw-rw-   0        0        0     4742 2023-07-16 14:42:54.000000 metathreads-0.0.2/metathreads.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-07-16 14:42:54.000000 metathreads-0.0.2/metathreads.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 14:42:54.000000 metathreads-0.0.2/metathreads.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      184 2023-07-16 14:42:54.000000 metathreads-0.0.2/metathreads.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 14:42:54.000000 metathreads-0.0.2/metathreads.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 14:42:55.196747 metathreads-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1636 2023-07-16 14:42:40.000000 metathreads-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:21:52.039972 metathreads-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 metathreads-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-07-13 14:53:51.000000 metathreads-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4742 2023-07-18 08:21:52.039972 metathreads-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3554 2023-07-13 14:54:38.000000 metathreads-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 08:21:52.024350 metathreads-0.0.3/metathreads/
+-rw-rw-rw-   0        0        0       38 2023-07-13 14:53:20.000000 metathreads-0.0.3/metathreads/__init__.py
+-rw-rw-rw-   0        0        0      414 2023-07-18 08:17:20.000000 metathreads-0.0.3/metathreads/config.py
+-rw-rw-rw-   0        0        0     1378 2023-07-13 12:19:15.000000 metathreads-0.0.3/metathreads/constants.py
+-rw-rw-rw-   0        0        0    14529 2023-07-18 07:20:15.000000 metathreads-0.0.3/metathreads/metathreads.py
+-rw-rw-rw-   0        0        0     8072 2023-07-18 08:16:10.000000 metathreads-0.0.3/metathreads/request_util.py
+-rw-rw-rw-   0        0        0     3800 2023-07-13 12:32:50.000000 metathreads-0.0.3/metathreads/util.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:21:52.039972 metathreads-0.0.3/metathreads.egg-info/
+-rw-rw-rw-   0        0        0     4742 2023-07-18 08:21:51.000000 metathreads-0.0.3/metathreads.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-07-18 08:21:51.000000 metathreads-0.0.3/metathreads.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:21:51.000000 metathreads-0.0.3/metathreads.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      184 2023-07-18 08:21:51.000000 metathreads-0.0.3/metathreads.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 08:21:51.000000 metathreads-0.0.3/metathreads.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 08:21:52.039972 metathreads-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1636 2023-07-18 08:20:54.000000 metathreads-0.0.3/setup.py
```

### Comparing `metathreads-0.0.2/LICENSE` & `metathreads-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metathreads-0.0.2/PKG-INFO` & `metathreads-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metathreads
-Version: 0.0.2
+Version: 0.0.3
 Summary: MetaThreads is Meta Threads-API to interact with Instagram threads app, extract data and perform actions. The library is written in python. MetaThreads API lets you fetch user's threads, thread replies, user's data, user's friends. Actions like posting a thread, like/unlike threads etc. can easily be perfomed with the api.
 Home-page: https://github.com/iSarabjitDhiman/MetaThreads
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: metathreads,threads-api,threadsapi,meta threads api,threads api,instagram threads,threads-api-python,insta-threads
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metathreads Version: 0.0.2 Summary: MetaThreads is
+Metadata-Version: 2.1 Name: metathreads Version: 0.0.3 Summary: MetaThreads is
 Meta Threads-API to interact with Instagram threads app, extract data and
 perform actions. The library is written in python. MetaThreads API lets you
 fetch user's threads, thread replies, user's data, user's friends. Actions like
 posting a thread, like/unlike threads etc. can easily be perfomed with the api.
 Home-page: https://github.com/iSarabjitDhiman/MetaThreads Author: Sarabjit
 Dhiman Author-email: hello@sarabjitdhiman.com License: MIT Keywords:
 metathreads,threads-api,threadsapi,meta threads api,threads api,instagram
```

### Comparing `metathreads-0.0.2/README.md` & `metathreads-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `metathreads-0.0.2/metathreads/constants.py` & `metathreads-0.0.3/metathreads/constants.py`

 * *Files identical despite different names*

### Comparing `metathreads-0.0.2/metathreads/metathreads.py` & `metathreads-0.0.3/metathreads/metathreads.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,17 @@
         Args:
             thread_id (str/int): Thread ID or URL.
             cursor (str, optional): Last endcursor point. (To start from where you left off the last time). Defaults to None.
 
         Returns:
             dict: Thread replies dataset. i.e. people who replied to the thread and replied content.
         """
-        pagination_data = {"paging_token'": cursor, "count": 100}
-        return generate_request_data(Path.THREAD_ENDPOINT, thread_id, pagination=pagination_data)
+        params = {"count": 100}
+        pagination_data = {"paging_token'": cursor}
+        return generate_request_data(Path.THREAD_ENDPOINT, thread_id, params=params, pagination=pagination_data)
 
     @thread_id_decorator
     def get_thread_likes(self, thread_id):
         """Get thread likes.
 
         Args:
             thread_id (str/int): Thread ID or URL.
```

### Comparing `metathreads-0.0.2/metathreads/request_util.py` & `metathreads-0.0.3/metathreads/request_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import httpx
 import asyncio
 import bs4
 import json
+import hashlib
 from . import util
 from . import config
 from .constants import Path
 
 
 def make_request(url=None, method=None, params=None, request_payload=None, session=None, timeout=None, **kwargs):
-    global data_placeholder
+    global data_container
     # fmt: off - Turns off formatting for this block of code. Just for the readability purpose.
     def make_regular_request(request_payload):
         return validate_response(session.request(**request_payload))
 
     async def make_async_request(request_payload):
         pagination_data = request_payload.pop("pagination_data",None)
         if not pagination_data:
@@ -28,14 +29,15 @@
             if not isinstance(query_params,list):
                 return await make_async_request({"params":query_params} | request_payload) 
             if not query_params:
                 return await make_async_request(request_payload)  
             tasks_list = [asyncio.create_task(make_async_request({"params":query} | request_payload)) for query in query_params]
         return await asyncio.gather(*tasks_list, return_exceptions=True)
 
+    data_container = {}
     method = method or "GET"
     timeout = timeout or config.TIMEOUT or 10
     proxies = config.PROXY or None
     ssl_verify = False if proxies else True
     concurrent_requests = False
     session = session or config._DEFAULT_SESSION or httpx.Client(follow_redirects=True, timeout=timeout, proxies=proxies, verify=ssl_verify)
     if request_payload:
@@ -44,18 +46,18 @@
             connection_limits = httpx.Limits(max_connections=100, max_keepalive_connections=10, keepalive_expiry=5)
             headers,cookies = session.headers,session.cookies
             session = httpx.AsyncClient(limits=connection_limits,headers=headers,cookies=cookies,follow_redirects=True,timeout=timeout,proxies=proxies,verify=ssl_verify)
             try:
                 return asyncio.run(make_concurrent_requests(request_payload))
             except KeyboardInterrupt:
                 print("Interuppted..")
-                return data_placeholder
+                return list(data_container.values())
             except Exception as error:
                 print(error)
-                return data_placeholder
+                return list(data_container.values())
     else:
         request_payload = {"method":method,"url":url,"params":params} | kwargs
     return make_regular_request(request_payload)
 
 
 def generate_request_data(endpoint, placeholder=None, params=None, additional_payload=None, pagination=None, return_payload=False, **kwargs):
         # fmt: off - Turns off formatting for this block of code. Just for the readability purpose.
@@ -88,33 +90,35 @@
     if pagination:
         request_payload.update({"pagination_data": pagination}) if isinstance(request_payload, dict) else [
             item.update({"pagination_data": pagination}) for item in request_payload]
     return make_request(request_payload=request_payload)
 
 
 async def _handle_pagination(url=None, request_payload=None, session=None, end_cursor=None, **kwargs):
-    global data_placeholder
         # fmt: off  - Turns off formatting for this block of code. Just for the readability purpose.
+    unique_key = hashlib.sha1(json.dumps(request_payload, sort_keys=True).encode()).hexdigest()
     data_placeholder = {"data": [],"cursor_endpoint": None, "has_next_page": True}
     request_payload = request_payload or {"url": url} | kwargs
-    cursor_key,end_cursor = end_cursor.popitem()
+    cursor_key = next(iter(end_cursor))
+    end_cursor = end_cursor[cursor_key]
     while data_placeholder["has_next_page"]:
         try:
             if end_cursor:
                 query_params = request_payload["params"] or json.dumps({cursor_key:""})
                 query_params = json.loads(query_params)
                 query_params[cursor_key] = end_cursor
                 request_payload["params"] = json.dumps(query_params)
             response = await session.request(**request_payload)
             response = validate_response(response)
             end_cursor = util.find_nested_key(response,"next_max_id") or util.find_nested_key(response,"paging_tokens")
             end_cursor = end_cursor[0] if (end_cursor and isinstance(end_cursor[0],str)) else end_cursor[0].get("downwards",None) if (end_cursor and isinstance(end_cursor[0],dict)) else None
             more_threads =  util.find_nested_key(response,"downwards_thread_will_continue")
             more_threads = more_threads[0] if more_threads else True
             data_placeholder['data'].append(response)
+            data_container[unique_key] = data_placeholder
             print(f"Page: {len(data_placeholder['data'])}", end="\r")
             if end_cursor:
                 data_placeholder['cursor_endpoint'] = end_cursor
             else:
                 data_placeholder["has_next_page"] = False
 
             if not data_placeholder["has_next_page"] or not more_threads:
```

### Comparing `metathreads-0.0.2/metathreads/util.py` & `metathreads-0.0.3/metathreads/util.py`

 * *Files identical despite different names*

### Comparing `metathreads-0.0.2/metathreads.egg-info/PKG-INFO` & `metathreads-0.0.3/metathreads.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metathreads
-Version: 0.0.2
+Version: 0.0.3
 Summary: MetaThreads is Meta Threads-API to interact with Instagram threads app, extract data and perform actions. The library is written in python. MetaThreads API lets you fetch user's threads, thread replies, user's data, user's friends. Actions like posting a thread, like/unlike threads etc. can easily be perfomed with the api.
 Home-page: https://github.com/iSarabjitDhiman/MetaThreads
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: metathreads,threads-api,threadsapi,meta threads api,threads api,instagram threads,threads-api-python,insta-threads
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metathreads Version: 0.0.2 Summary: MetaThreads is
+Metadata-Version: 2.1 Name: metathreads Version: 0.0.3 Summary: MetaThreads is
 Meta Threads-API to interact with Instagram threads app, extract data and
 perform actions. The library is written in python. MetaThreads API lets you
 fetch user's threads, thread replies, user's data, user's friends. Actions like
 posting a thread, like/unlike threads etc. can easily be perfomed with the api.
 Home-page: https://github.com/iSarabjitDhiman/MetaThreads Author: Sarabjit
 Dhiman Author-email: hello@sarabjitdhiman.com License: MIT Keywords:
 metathreads,threads-api,threadsapi,meta threads api,threads api,instagram
```

### Comparing `metathreads-0.0.2/setup.py` & `metathreads-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 SHORT_DESCRIPTION = "MetaThreads is Meta Threads-API to interact with Instagram threads app, extract data and perform actions. The library is written in python. MetaThreads API lets you fetch user's threads, thread replies, user's data, user's friends. Actions like posting a thread, like/unlike threads etc. can easily be perfomed with the api."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

