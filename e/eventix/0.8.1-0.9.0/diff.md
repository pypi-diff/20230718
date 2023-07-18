# Comparing `tmp/eventix-0.8.1.tar.gz` & `tmp/eventix-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventix-0.8.1.tar", max compression
+gzip compressed data, was "eventix-0.9.0.tar", max compression
```

## Comparing `eventix-0.8.1.tar` & `eventix-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/__init__.py
--rw-r--r--   0        0        0     1577 2023-07-06 06:33:36.740790 eventix-0.8.1/eventix/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/depends/__init__.py
--rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.8.1/eventix/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/functions/__init__.py
--rw-r--r--   0        0        0     4036 2023-07-06 14:36:57.587160 eventix-0.8.1/eventix/functions/core.py
--rw-r--r--   0        0        0      950 2023-07-13 10:39:48.044793 eventix-0.8.1/eventix/functions/errors.py
--rw-r--r--   0        0        0     1676 2023-07-07 07:11:22.071252 eventix-0.8.1/eventix/functions/eventix_client.py
--rw-r--r--   0        0        0     2815 2023-07-04 08:25:54.140139 eventix-0.8.1/eventix/functions/fastapi.py
--rw-r--r--   0        0        0      858 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/functions/metrics.py
--rw-r--r--   0        0        0      426 2023-07-06 14:36:57.671160 eventix-0.8.1/eventix/functions/schedule.py
--rw-r--r--   0        0        0     7507 2023-07-13 11:00:20.373143 eventix-0.8.1/eventix/functions/task.py
--rw-r--r--   0        0        0     1155 2023-07-04 15:24:17.145091 eventix-0.8.1/eventix/functions/task_scheduler.py
--rw-r--r--   0        0        0     7605 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/functions/task_worker.py
--rw-r--r--   0        0        0      790 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/functions/tools.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/pydantic/__init__.py
--rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/pydantic/event.py
--rw-r--r--   0        0        0      615 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/pydantic/pagination.py
--rw-r--r--   0        0        0      634 2023-07-06 19:19:42.803712 eventix-0.8.1/eventix/pydantic/schedule.py
--rw-r--r--   0        0        0     2063 2023-07-13 11:01:52.956508 eventix-0.8.1/eventix/pydantic/task.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/router/__init__.py
--rw-r--r--   0        0        0      340 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/router/default.py
--rw-r--r--   0        0        0      243 2023-07-12 07:18:50.102891 eventix-0.8.1/eventix/router/metrics.py
--rw-r--r--   0        0        0      913 2023-07-12 07:18:50.102891 eventix-0.8.1/eventix/router/task.py
--rw-r--r--   0        0        0     1386 2023-07-12 07:18:50.102891 eventix-0.8.1/eventix/router/tasks.py
--rw-r--r--   0        0        0        0 2023-07-04 19:28:16.696215 eventix-0.8.1/eventix/tasks/__init__.py
--rw-r--r--   0        0        0      396 2023-07-06 20:57:49.171190 eventix-0.8.1/eventix/tasks/cleanup.py
--rw-r--r--   0        0        0     1024 2023-07-18 07:02:31.282246 eventix-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 eventix-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.9.0/eventix/__init__.py
+-rw-r--r--   0        0        0     1577 2023-07-06 06:33:36.740790 eventix-0.9.0/eventix/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:18:50.098891 eventix-0.9.0/eventix/depends/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.9.0/eventix/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.9.0/eventix/functions/__init__.py
+-rw-r--r--   0        0        0     4036 2023-07-06 14:36:57.587160 eventix-0.9.0/eventix/functions/core.py
+-rw-r--r--   0        0        0      950 2023-07-13 10:39:48.044793 eventix-0.9.0/eventix/functions/errors.py
+-rw-r--r--   0        0        0     1676 2023-07-07 07:11:22.071252 eventix-0.9.0/eventix/functions/eventix_client.py
+-rw-r--r--   0        0        0     2815 2023-07-04 08:25:54.140139 eventix-0.9.0/eventix/functions/fastapi.py
+-rw-r--r--   0        0        0      858 2023-07-12 07:18:50.098891 eventix-0.9.0/eventix/functions/metrics.py
+-rw-r--r--   0        0        0      426 2023-07-06 14:36:57.671160 eventix-0.9.0/eventix/functions/schedule.py
+-rw-r--r--   0        0        0     7507 2023-07-13 11:00:20.373143 eventix-0.9.0/eventix/functions/task.py
+-rw-r--r--   0        0        0     1908 2023-07-18 07:40:01.741108 eventix-0.9.0/eventix/functions/task_scheduler.py
+-rw-r--r--   0        0        0     7605 2023-07-12 07:18:50.098891 eventix-0.9.0/eventix/functions/task_worker.py
+-rw-r--r--   0        0        0      790 2023-07-12 07:18:50.098891 eventix-0.9.0/eventix/functions/tools.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.9.0/eventix/pydantic/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.9.0/eventix/pydantic/event.py
+-rw-r--r--   0        0        0      615 2023-07-12 07:18:50.098891 eventix-0.9.0/eventix/pydantic/pagination.py
+-rw-r--r--   0        0        0      634 2023-07-06 19:19:42.803712 eventix-0.9.0/eventix/pydantic/schedule.py
+-rw-r--r--   0        0        0     2063 2023-07-13 11:01:52.956508 eventix-0.9.0/eventix/pydantic/task.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.9.0/eventix/router/__init__.py
+-rw-r--r--   0        0        0      340 2023-07-12 07:18:50.098891 eventix-0.9.0/eventix/router/default.py
+-rw-r--r--   0        0        0      243 2023-07-12 07:18:50.102891 eventix-0.9.0/eventix/router/metrics.py
+-rw-r--r--   0        0        0      913 2023-07-12 07:18:50.102891 eventix-0.9.0/eventix/router/task.py
+-rw-r--r--   0        0        0     1386 2023-07-12 07:18:50.102891 eventix-0.9.0/eventix/router/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:28:16.696215 eventix-0.9.0/eventix/tasks/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-06 20:57:49.171190 eventix-0.9.0/eventix/tasks/cleanup.py
+-rw-r--r--   0        0        0     1024 2023-07-18 07:48:13.064214 eventix-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 eventix-0.9.0/PKG-INFO
```

### Comparing `eventix-0.8.1/eventix/contexts/__init__.py` & `eventix-0.9.0/eventix/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/exceptions/__init__.py` & `eventix-0.9.0/eventix/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/functions/core.py` & `eventix-0.9.0/eventix/functions/core.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/functions/errors.py` & `eventix-0.9.0/eventix/functions/errors.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/functions/eventix_client.py` & `eventix-0.9.0/eventix/functions/eventix_client.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/functions/fastapi.py` & `eventix-0.9.0/eventix/functions/fastapi.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/functions/metrics.py` & `eventix-0.9.0/eventix/functions/metrics.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/functions/task.py` & `eventix-0.9.0/eventix/functions/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/functions/task_scheduler.py` & `eventix-0.9.0/eventix/functions/task_scheduler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
+import os
+import sys
 
-from eventix.contexts import namespace_context
+from eventix.contexts import namespace_context, namespace_context_var
 from eventix.exceptions import backend_exceptions
 from eventix.functions.errors import raise_errors
 from eventix.functions.eventix_client import EventixClient
 from eventix.pydantic.task import TaskModel
 
 log = logging.getLogger(__name__)
 
@@ -26,7 +28,35 @@
             return TaskModel.parse_raw(r.content)
 
     @classmethod
     def task_post(cls, task: TaskModel) -> TaskModel:
         r = cls.interface.post('/task', data=task.json())
         with raise_errors(r, backend_exceptions):
             return TaskModel.parse_raw(r.content)
+
+    @classmethod
+    def config(cls, config: dict):
+        # Be aware that the namespace context is set direct through
+        # the context variable.... so no reset possible
+
+        base_url = os.environ.get("EVENTIX_URL", "")
+        if base_url == "":
+            log.error("No EVENTIX_URL set.")
+            sys.exit()
+
+        cls.set_base_url(base_url)
+
+        namespace = ""
+        if "namespace" in config:
+            namespace = config['namespace']
+
+        if namespace == "":
+            namespace = os.environ.get("EVENTIX_NAMESPACE", "")
+
+
+        if namespace == "":
+            log.error("No EVENTIX_NAMESPACE set.")
+            sys.exit()
+
+        namespace_context_var.set(namespace)
+
+
```

### Comparing `eventix-0.8.1/eventix/functions/task_worker.py` & `eventix-0.9.0/eventix/functions/task_worker.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/functions/tools.py` & `eventix-0.9.0/eventix/functions/tools.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/pydantic/pagination.py` & `eventix-0.9.0/eventix/pydantic/pagination.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/pydantic/schedule.py` & `eventix-0.9.0/eventix/pydantic/schedule.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/pydantic/task.py` & `eventix-0.9.0/eventix/pydantic/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/router/task.py` & `eventix-0.9.0/eventix/router/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/eventix/router/tasks.py` & `eventix-0.9.0/eventix/router/tasks.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.1/pyproject.toml` & `eventix-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventix"
-version = "0.8.1"
+version = "0.9.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.99.1"
```

### Comparing `eventix-0.8.1/PKG-INFO` & `eventix-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventix
-Version: 0.8.1
+Version: 0.9.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: croniter (>=1.4.1,<2.0.0)
```

