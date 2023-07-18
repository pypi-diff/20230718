# Comparing `tmp/timing-asgi-0.3.0b0.tar.gz` & `tmp/timing_asgi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timing-asgi-0.3.0b0.tar", max compression
+gzip compressed data, was "timing_asgi-0.3.1.tar", max compression
```

## Comparing `timing-asgi-0.3.0b0.tar` & `timing_asgi-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      588 2022-07-13 23:38:52.717017 timing-asgi-0.3.0b0/pyproject.toml
--rw-r--r--   0        0        0      174 2020-11-13 11:36:19.015514 timing-asgi-0.3.0b0/timing_asgi/__init__.py
--rw-r--r--   0        0        0       78 2020-11-13 11:36:19.015683 timing-asgi-0.3.0b0/timing_asgi/integrations/__init__.py
--rw-r--r--   0        0        0     1103 2022-07-13 23:32:12.435889 timing-asgi-0.3.0b0/timing_asgi/integrations/starlette.py
--rw-r--r--   0        0        0      392 2022-07-13 23:32:12.436686 timing-asgi-0.3.0b0/timing_asgi/interfaces.py
--rw-r--r--   0        0        0     2568 2022-07-13 23:32:12.437396 timing-asgi-0.3.0b0/timing_asgi/middleware.py
--rw-r--r--   0        0        0     1385 2022-07-13 23:37:39.900578 timing-asgi-0.3.0b0/timing_asgi/utils.py
--rw-r--r--   0        0        0      701 2022-07-13 23:58:20.744370 timing-asgi-0.3.0b0/setup.py
--rw-r--r--   0        0        0      632 2022-07-13 23:58:20.744601 timing-asgi-0.3.0b0/PKG-INFO
+-rw-r--r--   0        0        0     2973 2023-07-18 10:16:30.736838 timing_asgi-0.3.1/README.md
+-rw-r--r--   0        0        0      660 2023-07-18 10:18:21.190648 timing_asgi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      174 2020-11-13 11:36:19.015514 timing_asgi-0.3.1/timing_asgi/__init__.py
+-rw-r--r--   0        0        0       78 2020-11-13 11:36:19.015683 timing_asgi-0.3.1/timing_asgi/integrations/__init__.py
+-rw-r--r--   0        0        0     1103 2022-07-13 23:32:12.435889 timing_asgi-0.3.1/timing_asgi/integrations/starlette.py
+-rw-r--r--   0        0        0      392 2022-07-13 23:32:12.436686 timing_asgi-0.3.1/timing_asgi/interfaces.py
+-rw-r--r--   0        0        0     2603 2023-07-18 10:16:30.737885 timing_asgi-0.3.1/timing_asgi/middleware.py
+-rw-r--r--   0        0        0     1385 2022-07-13 23:37:39.900578 timing_asgi-0.3.1/timing_asgi/utils.py
+-rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 timing_asgi-0.3.1/setup.py
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 timing_asgi-0.3.1/PKG-INFO
```

### Comparing `timing-asgi-0.3.0b0/pyproject.toml` & `timing_asgi-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [tool.poetry]
 name = "timing-asgi"
-version = "0.3.0b"
+version = "0.3.1"
 description = "ASGI middleware to emit timing metrics with something like statsd"
 authors = ["Steinn Eldjárn Sigurðarson <steinnes@gmail.com>"]
+readme = "README.md"
 license = "MIT"
 
+[project.urls]
+"Source" = "https://github.com/steinnes/timing-asgi"
+
 [tool.poetry.dependencies]
 python = "^3.6"
-alog = "^0.9.13"
 
 [tool.poetry.dev-dependencies]
 starlette = "^0.12.0"
 pytest = "^4.3"
 pytest-cov = "^2.6"
 requests = "^2.21"
 pytest-asyncio = "^0.10.0"
```

### Comparing `timing-asgi-0.3.0b0/timing_asgi/integrations/starlette.py` & `timing_asgi-0.3.1/timing_asgi/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `timing-asgi-0.3.0b0/timing_asgi/middleware.py` & `timing_asgi-0.3.1/timing_asgi/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import alog
+import logging
 
 from .utils import PathToName, TimingStats
 
+log = logging.getLogger(__name__)
+
 
 class TimingMiddleware:
     """Timing middleware for ASGI applications
 
     Args:
       app (ASGI application): ASGI application
       client (TimingClient): the client used to emit instrumentation metrics
@@ -33,25 +35,25 @@
 
         def send_wrapper(response):
             if response["type"] == "http.response.start":
                 instance["http_status_code"] = response["status"]
             return send(response)
 
         if scope["type"] != "http":
-            alog.debug(f"ASGI scope of type {scope['type']} is not supported yet")
+            log.debug(f"ASGI scope of type {scope['type']} is not supported yet")
             await self.app(scope, receive, send)
             return
 
         try:
             metric_name = self.metric_namer(scope)
         except AttributeError as e:
-            alog.error(
+            log.error(
                 f"Unable to extract metric name from asgi scope: {scope}, skipping statsd timing"
             )
-            alog.error(f" -> exception: {e}")
+            log.error(f" -> exception: {e}")
             await self.app(scope, receive, send)
             return
 
         def emit(stats):
             statsd_tags = [
                 f"http_status:{instance['http_status_code']}",
                 f"http_method:{scope['method']}",
```

### Comparing `timing-asgi-0.3.0b0/timing_asgi/utils.py` & `timing_asgi-0.3.1/timing_asgi/utils.py`

 * *Files identical despite different names*

