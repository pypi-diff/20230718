# Comparing `tmp/uvicorn-0.9.0.tar.gz` & `tmp/uvicorn-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uvicorn-0.9.0.tar", last modified: Fri Sep  6 16:04:25 2019, max compression
+gzip compressed data, was "dist/uvicorn-0.9.1.tar", last modified: Mon Oct 21 14:27:01 2019, max compression
```

## Comparing `uvicorn-0.9.0.tar` & `uvicorn-0.9.1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/
--rw-r--r--   0 tomchristie   (501) staff       (20)     1525 2018-11-23 14:21:54.000000 uvicorn-0.9.0/LICENSE.md
--rw-r--r--   0 tomchristie   (501) staff       (20)     3498 2019-09-06 16:04:25.000000 uvicorn-0.9.0/PKG-INFO
--rw-r--r--   0 tomchristie   (501) staff       (20)     2117 2019-09-06 16:04:22.000000 uvicorn-0.9.0/README.md
--rw-r--r--   0 tomchristie   (501) staff       (20)       38 2019-09-06 16:04:25.000000 uvicorn-0.9.0/setup.cfg
--rwxr-xr-x   0 tomchristie   (501) staff       (20)     2190 2019-09-06 16:04:22.000000 uvicorn-0.9.0/setup.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn/
--rw-r--r--   0 tomchristie   (501) staff       (20)      146 2019-09-06 16:04:22.000000 uvicorn-0.9.0/uvicorn/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     7747 2019-09-04 14:52:58.000000 uvicorn-0.9.0/uvicorn/config.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     1138 2018-11-23 14:21:54.000000 uvicorn-0.9.0/uvicorn/importer.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn/lifespan/
--rw-r--r--   0 tomchristie   (501) staff       (20)        0 2019-02-05 12:05:11.000000 uvicorn-0.9.0/uvicorn/lifespan/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      171 2019-03-20 13:13:12.000000 uvicorn-0.9.0/uvicorn/lifespan/off.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     3115 2019-08-01 16:41:50.000000 uvicorn-0.9.0/uvicorn/lifespan/on.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn/loops/
--rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.0/uvicorn/loops/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      107 2019-02-14 09:17:49.000000 uvicorn-0.9.0/uvicorn/loops/asyncio.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      274 2019-02-14 09:17:49.000000 uvicorn-0.9.0/uvicorn/loops/auto.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      112 2019-02-14 09:17:49.000000 uvicorn-0.9.0/uvicorn/loops/uvloop.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    13700 2019-06-28 11:40:47.000000 uvicorn-0.9.0/uvicorn/main.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn/middleware/
--rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.0/uvicorn/middleware/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      201 2019-03-20 13:13:12.000000 uvicorn-0.9.0/uvicorn/middleware/asgi2.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2709 2019-03-20 13:13:12.000000 uvicorn-0.9.0/uvicorn/middleware/debug.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2083 2019-03-20 13:13:12.000000 uvicorn-0.9.0/uvicorn/middleware/message_logger.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     1561 2019-03-20 13:13:12.000000 uvicorn-0.9.0/uvicorn/middleware/proxy_headers.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     4938 2019-09-04 14:52:58.000000 uvicorn-0.9.0/uvicorn/middleware/wsgi.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn/protocols/
--rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.0/uvicorn/protocols/__init__.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn/protocols/http/
--rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.0/uvicorn/protocols/http/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      289 2018-11-23 14:21:54.000000 uvicorn-0.9.0/uvicorn/protocols/http/auto.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    17457 2019-07-29 13:59:53.000000 uvicorn-0.9.0/uvicorn/protocols/http/h11_impl.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    18190 2019-07-29 13:59:53.000000 uvicorn-0.9.0/uvicorn/protocols/http/httptools_impl.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     1420 2019-07-29 13:59:53.000000 uvicorn-0.9.0/uvicorn/protocols/utils.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn/protocols/websockets/
--rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.0/uvicorn/protocols/websockets/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      436 2018-11-23 14:21:54.000000 uvicorn-0.9.0/uvicorn/protocols/websockets/auto.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     8401 2019-09-06 15:15:37.000000 uvicorn-0.9.0/uvicorn/protocols/websockets/websockets_impl.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    11085 2019-06-18 14:17:39.000000 uvicorn-0.9.0/uvicorn/protocols/websockets/wsproto_impl.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn/supervisors/
--rw-r--r--   0 tomchristie   (501) staff       (20)      154 2019-03-04 13:39:29.000000 uvicorn-0.9.0/uvicorn/supervisors/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     1114 2019-03-05 10:27:29.000000 uvicorn-0.9.0/uvicorn/supervisors/multiprocess.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2941 2019-09-04 14:52:58.000000 uvicorn-0.9.0/uvicorn/supervisors/statreload.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     1939 2019-03-20 13:13:12.000000 uvicorn-0.9.0/uvicorn/workers.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn.egg-info/
--rw-r--r--   0 tomchristie   (501) staff       (20)     3498 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn.egg-info/PKG-INFO
--rw-r--r--   0 tomchristie   (501) staff       (20)     1142 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn.egg-info/SOURCES.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)        1 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn.egg-info/dependency_links.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)       57 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn.egg-info/entry_points.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)      170 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn.egg-info/requires.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)      148 2019-09-06 16:04:25.000000 uvicorn-0.9.0/uvicorn.egg-info/top_level.txt
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1525 2018-11-23 14:21:54.000000 uvicorn-0.9.1/LICENSE.md
+-rw-r--r--   0 tomchristie   (501) staff       (20)     3498 2019-10-21 14:27:01.000000 uvicorn-0.9.1/PKG-INFO
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2117 2019-09-06 16:04:22.000000 uvicorn-0.9.1/README.md
+-rw-r--r--   0 tomchristie   (501) staff       (20)       38 2019-10-21 14:27:01.000000 uvicorn-0.9.1/setup.cfg
+-rwxr-xr-x   0 tomchristie   (501) staff       (20)     2190 2019-09-06 16:04:22.000000 uvicorn-0.9.1/setup.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn/
+-rw-r--r--   0 tomchristie   (501) staff       (20)      146 2019-10-21 14:26:30.000000 uvicorn-0.9.1/uvicorn/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)       63 2019-10-21 14:26:20.000000 uvicorn-0.9.1/uvicorn/__main__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     7792 2019-10-21 14:26:20.000000 uvicorn-0.9.1/uvicorn/config.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1138 2018-11-23 14:21:54.000000 uvicorn-0.9.1/uvicorn/importer.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn/lifespan/
+-rw-r--r--   0 tomchristie   (501) staff       (20)        0 2019-02-05 12:05:11.000000 uvicorn-0.9.1/uvicorn/lifespan/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      171 2019-03-20 13:13:12.000000 uvicorn-0.9.1/uvicorn/lifespan/off.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     3115 2019-08-01 16:41:50.000000 uvicorn-0.9.1/uvicorn/lifespan/on.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn/loops/
+-rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.1/uvicorn/loops/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      107 2019-02-14 09:17:49.000000 uvicorn-0.9.1/uvicorn/loops/asyncio.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      420 2019-10-21 14:26:20.000000 uvicorn-0.9.1/uvicorn/loops/auto.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      264 2019-10-21 14:26:20.000000 uvicorn-0.9.1/uvicorn/loops/iocp.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      112 2019-02-14 09:17:49.000000 uvicorn-0.9.1/uvicorn/loops/uvloop.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)    13700 2019-06-28 11:40:47.000000 uvicorn-0.9.1/uvicorn/main.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn/middleware/
+-rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.1/uvicorn/middleware/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      201 2019-03-20 13:13:12.000000 uvicorn-0.9.1/uvicorn/middleware/asgi2.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2709 2019-03-20 13:13:12.000000 uvicorn-0.9.1/uvicorn/middleware/debug.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2083 2019-03-20 13:13:12.000000 uvicorn-0.9.1/uvicorn/middleware/message_logger.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1561 2019-03-20 13:13:12.000000 uvicorn-0.9.1/uvicorn/middleware/proxy_headers.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     4938 2019-09-04 14:52:58.000000 uvicorn-0.9.1/uvicorn/middleware/wsgi.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn/protocols/
+-rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.1/uvicorn/protocols/__init__.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn/protocols/http/
+-rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.1/uvicorn/protocols/http/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      289 2018-11-23 14:21:54.000000 uvicorn-0.9.1/uvicorn/protocols/http/auto.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)    17534 2019-10-21 14:26:20.000000 uvicorn-0.9.1/uvicorn/protocols/http/h11_impl.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)    18305 2019-10-21 14:26:20.000000 uvicorn-0.9.1/uvicorn/protocols/http/httptools_impl.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1420 2019-07-29 13:59:53.000000 uvicorn-0.9.1/uvicorn/protocols/utils.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn/protocols/websockets/
+-rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 14:21:54.000000 uvicorn-0.9.1/uvicorn/protocols/websockets/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      436 2018-11-23 14:21:54.000000 uvicorn-0.9.1/uvicorn/protocols/websockets/auto.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     8401 2019-09-06 15:15:37.000000 uvicorn-0.9.1/uvicorn/protocols/websockets/websockets_impl.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)    11085 2019-06-18 14:17:39.000000 uvicorn-0.9.1/uvicorn/protocols/websockets/wsproto_impl.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn/supervisors/
+-rw-r--r--   0 tomchristie   (501) staff       (20)      154 2019-03-04 13:39:29.000000 uvicorn-0.9.1/uvicorn/supervisors/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1114 2019-03-05 10:27:29.000000 uvicorn-0.9.1/uvicorn/supervisors/multiprocess.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2941 2019-09-04 14:52:58.000000 uvicorn-0.9.1/uvicorn/supervisors/statreload.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1991 2019-10-21 14:26:20.000000 uvicorn-0.9.1/uvicorn/workers.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn.egg-info/
+-rw-r--r--   0 tomchristie   (501) staff       (20)     3498 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn.egg-info/PKG-INFO
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1184 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn.egg-info/SOURCES.txt
+-rw-r--r--   0 tomchristie   (501) staff       (20)        1 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn.egg-info/dependency_links.txt
+-rw-r--r--   0 tomchristie   (501) staff       (20)       57 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn.egg-info/entry_points.txt
+-rw-r--r--   0 tomchristie   (501) staff       (20)      170 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn.egg-info/requires.txt
+-rw-r--r--   0 tomchristie   (501) staff       (20)      148 2019-10-21 14:27:01.000000 uvicorn-0.9.1/uvicorn.egg-info/top_level.txt
```

### Comparing `uvicorn-0.9.0/LICENSE.md` & `uvicorn-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/PKG-INFO` & `uvicorn-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvicorn
-Version: 0.9.0
+Version: 0.9.1
 Summary: The lightning-fast ASGI server.
 Home-page: https://github.com/encode/uvicorn
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Description: <p align="center">
           <img width="320" height="320" src="https://raw.githubusercontent.com/tomchristie/uvicorn/master/docs/uvicorn.png" alt='uvicorn'>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uvicorn Version: 0.9.0 Summary: The lightning-fast
+Metadata-Version: 2.1 Name: uvicorn Version: 0.9.1 Summary: The lightning-fast
 ASGI server. Home-page: https://github.com/encode/uvicorn Author: Tom Christie
 Author-email: tom@tomchristie.com License: BSD Description:
                                    [uvicorn]
                         The lightning-fast ASGI server.
 --- [![Build Status](https://travis-ci.org/encode/uvicorn.svg?branch=master)]
 (https://travis-ci.org/encode/uvicorn) [![Coverage](https://codecov.io/gh/
 encode/uvicorn/branch/master/graph/badge.svg)](https://codecov.io/gh/encode/
```

### Comparing `uvicorn-0.9.0/README.md` & `uvicorn-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/setup.py` & `uvicorn-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/config.py` & `uvicorn-0.9.1/uvicorn/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "on": "uvicorn.lifespan.on:LifespanOn",
     "off": "uvicorn.lifespan.off:LifespanOff",
 }
 LOOP_SETUPS = {
     "auto": "uvicorn.loops.auto:auto_loop_setup",
     "asyncio": "uvicorn.loops.asyncio:asyncio_setup",
     "uvloop": "uvicorn.loops.uvloop:uvloop_setup",
+    "iocp": "uvicorn.loops.iocp:iocp_setup",
 }
 INTERFACES = ["auto", "asgi3", "asgi2", "wsgi"]
 
 # Fallback to 'ssl.PROTOCOL_SSLv23' in order to support Python < 3.5.3.
 SSL_PROTOCOL_VERSION = getattr(ssl, "PROTOCOL_TLS", ssl.PROTOCOL_SSLv23)
```

### Comparing `uvicorn-0.9.0/uvicorn/importer.py` & `uvicorn-0.9.1/uvicorn/importer.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/lifespan/on.py` & `uvicorn-0.9.1/uvicorn/lifespan/on.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/main.py` & `uvicorn-0.9.1/uvicorn/main.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/middleware/debug.py` & `uvicorn-0.9.1/uvicorn/middleware/debug.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/middleware/message_logger.py` & `uvicorn-0.9.1/uvicorn/middleware/message_logger.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/middleware/proxy_headers.py` & `uvicorn-0.9.1/uvicorn/middleware/proxy_headers.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/middleware/wsgi.py` & `uvicorn-0.9.1/uvicorn/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/protocols/http/h11_impl.py` & `uvicorn-0.9.1/uvicorn/protocols/http/h11_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import logging
 from urllib.parse import unquote
 
 import h11
 
 from uvicorn.protocols.utils import (
     get_local_addr,
+    get_path_with_query_string,
     get_remote_addr,
     is_ssl,
-    get_path_with_query_string,
 )
 
 
 def _get_status_phrase(status_code):
     try:
         return http.HTTPStatus(status_code).phrase.encode()
     except ValueError as exc:
@@ -437,14 +437,15 @@
                 self.logger.info(
                     '%s - "%s %s HTTP/%s" %d',
                     self.scope["client"],
                     self.scope["method"],
                     get_path_with_query_string(self.scope),
                     self.scope["http_version"],
                     status_code,
+                    extra={"status_code": status_code, "scope": self.scope},
                 )
 
             # Write response status line and headers
             reason = STATUS_PHRASES[status_code]
             event = h11.Response(
                 status_code=status_code, headers=headers, reason=reason
             )
```

### Comparing `uvicorn-0.9.0/uvicorn/protocols/http/httptools_impl.py` & `uvicorn-0.9.1/uvicorn/protocols/http/httptools_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import logging
 import urllib
 
 import httptools
 
 from uvicorn.protocols.utils import (
     get_local_addr,
+    get_path_with_query_string,
     get_remote_addr,
     is_ssl,
-    get_path_with_query_string,
 )
 
 
 def _get_status_line(status_code):
     try:
         phrase = http.HTTPStatus(status_code).phrase.encode()
     except ValueError as exc:
@@ -133,15 +133,16 @@
 
         if self.logger.level <= logging.DEBUG:
             self.logger.debug("%s - Disconnected", self.client)
 
         if self.cycle and not self.cycle.response_complete:
             self.cycle.disconnected = True
         self.message_event.set()
-        self.flow.resume_writing()
+        if self.flow is not None:
+            self.flow.resume_writing()
 
     def eof_received(self):
         pass
 
     def data_received(self, data):
         if self.timeout_keep_alive_task is not None:
             self.timeout_keep_alive_task.cancel()
@@ -437,14 +438,15 @@
                 self.logger.info(
                     '%s - "%s %s HTTP/%s" %d',
                     self.scope["client"],
                     self.scope["method"],
                     get_path_with_query_string(self.scope),
                     self.scope["http_version"],
                     status_code,
+                    extra={"status_code": status_code, "scope": self.scope},
                 )
 
             # Write response status line and headers
             content = [STATUS_LINE[status_code]]
 
             for name, value in headers:
                 name = name.lower()
```

### Comparing `uvicorn-0.9.0/uvicorn/protocols/utils.py` & `uvicorn-0.9.1/uvicorn/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/protocols/websockets/websockets_impl.py` & `uvicorn-0.9.1/uvicorn/protocols/websockets/websockets_impl.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/protocols/websockets/wsproto_impl.py` & `uvicorn-0.9.1/uvicorn/protocols/websockets/wsproto_impl.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/supervisors/multiprocess.py` & `uvicorn-0.9.1/uvicorn/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/supervisors/statreload.py` & `uvicorn-0.9.1/uvicorn/supervisors/statreload.py`

 * *Files identical despite different names*

### Comparing `uvicorn-0.9.0/uvicorn/workers.py` & `uvicorn-0.9.1/uvicorn/workers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 
 from gunicorn.workers.base import Worker
-
 from uvicorn.config import Config
 from uvicorn.main import Server
 
 
 class UvicornWorker(Worker):
     """
     A worker class for Gunicorn that interfaces with an ASGI consumer callable,
@@ -21,14 +20,15 @@
 
         config_kwargs = {
             "app": None,
             "logger": self.log,
             "timeout_keep_alive": self.cfg.keepalive,
             "timeout_notify": self.timeout,
             "callback_notify": self.callback_notify,
+            "limit_max_requests": self.max_requests,
         }
 
         if self.cfg.is_ssl:
             ssl_kwargs = {
                 "ssl_keyfile": self.cfg.ssl_options.get("keyfile"),
                 "ssl_certfile": self.cfg.ssl_options.get("certfile"),
                 "ssl_version": self.cfg.ssl_options.get("ssl_version"),
```

### Comparing `uvicorn-0.9.0/uvicorn.egg-info/PKG-INFO` & `uvicorn-0.9.1/uvicorn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvicorn
-Version: 0.9.0
+Version: 0.9.1
 Summary: The lightning-fast ASGI server.
 Home-page: https://github.com/encode/uvicorn
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Description: <p align="center">
           <img width="320" height="320" src="https://raw.githubusercontent.com/tomchristie/uvicorn/master/docs/uvicorn.png" alt='uvicorn'>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uvicorn Version: 0.9.0 Summary: The lightning-fast
+Metadata-Version: 2.1 Name: uvicorn Version: 0.9.1 Summary: The lightning-fast
 ASGI server. Home-page: https://github.com/encode/uvicorn Author: Tom Christie
 Author-email: tom@tomchristie.com License: BSD Description:
                                    [uvicorn]
                         The lightning-fast ASGI server.
 --- [![Build Status](https://travis-ci.org/encode/uvicorn.svg?branch=master)]
 (https://travis-ci.org/encode/uvicorn) [![Coverage](https://codecov.io/gh/
 encode/uvicorn/branch/master/graph/badge.svg)](https://codecov.io/gh/encode/
```

### Comparing `uvicorn-0.9.0/uvicorn.egg-info/SOURCES.txt` & `uvicorn-0.9.1/uvicorn.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.md
 README.md
 setup.py
 uvicorn/__init__.py
+uvicorn/__main__.py
 uvicorn/config.py
 uvicorn/importer.py
 uvicorn/main.py
 uvicorn/workers.py
 uvicorn.egg-info/PKG-INFO
 uvicorn.egg-info/SOURCES.txt
 uvicorn.egg-info/dependency_links.txt
@@ -14,14 +15,15 @@
 uvicorn.egg-info/top_level.txt
 uvicorn/lifespan/__init__.py
 uvicorn/lifespan/off.py
 uvicorn/lifespan/on.py
 uvicorn/loops/__init__.py
 uvicorn/loops/asyncio.py
 uvicorn/loops/auto.py
+uvicorn/loops/iocp.py
 uvicorn/loops/uvloop.py
 uvicorn/middleware/__init__.py
 uvicorn/middleware/asgi2.py
 uvicorn/middleware/debug.py
 uvicorn/middleware/message_logger.py
 uvicorn/middleware/proxy_headers.py
 uvicorn/middleware/wsgi.py
```

