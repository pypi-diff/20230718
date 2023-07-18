# Comparing `tmp/eventix-0.8.0.tar.gz` & `tmp/eventix-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventix-0.8.0.tar", max compression
+gzip compressed data, was "eventix-0.8.1.tar", max compression
```

## Comparing `eventix-0.8.0.tar` & `eventix-0.8.1.tar`

### file list

```diff
@@ -1,55 +1,30 @@
--rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/__init__.py
--rw-r--r--   0        0        0     1577 2023-07-06 06:33:36.740790 eventix-0.8.0/eventix/contexts/__init__.py
--rw-r--r--   0        0        0     2796 2023-07-06 07:02:50.296411 eventix-0.8.0/eventix/contexts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/depends/__init__.py
--rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.8.0/eventix/exceptions/__init__.py
--rw-r--r--   0        0        0     2396 2023-07-03 12:34:47.194805 eventix-0.8.0/eventix/exceptions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/functions/__init__.py
--rw-r--r--   0        0        0      176 2023-07-03 12:30:27.428538 eventix-0.8.0/eventix/functions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6492 2023-07-06 14:41:10.892197 eventix-0.8.0/eventix/functions/__pycache__/core.cpython-311.pyc
--rw-r--r--   0        0        0     1833 2023-07-13 10:40:02.600612 eventix-0.8.0/eventix/functions/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0     2546 2023-07-07 07:11:23.559241 eventix-0.8.0/eventix/functions/__pycache__/eventix_client.cpython-311.pyc
--rw-r--r--   0        0        0     5466 2023-07-04 08:25:54.680135 eventix-0.8.0/eventix/functions/__pycache__/fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     2013 2023-07-12 07:19:14.246636 eventix-0.8.0/eventix/functions/__pycache__/metrics.cpython-311.pyc
--rw-r--r--   0        0        0      942 2023-07-06 14:41:10.948196 eventix-0.8.0/eventix/functions/__pycache__/schedule.cpython-311.pyc
--rw-r--r--   0        0        0     8220 2023-07-13 11:00:24.001119 eventix-0.8.0/eventix/functions/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     3107 2023-07-04 20:37:50.771263 eventix-0.8.0/eventix/functions/__pycache__/task_scheduler.cpython-311.pyc
--rw-r--r--   0        0        0    15277 2023-07-12 07:19:14.218636 eventix-0.8.0/eventix/functions/__pycache__/task_worker.cpython-311.pyc
--rw-r--r--   0        0        0     2089 2023-07-12 07:19:14.222636 eventix-0.8.0/eventix/functions/__pycache__/tools.cpython-311.pyc
--rw-r--r--   0        0        0     4036 2023-07-06 14:36:57.587160 eventix-0.8.0/eventix/functions/core.py
--rw-r--r--   0        0        0      950 2023-07-13 10:39:48.044793 eventix-0.8.0/eventix/functions/errors.py
--rw-r--r--   0        0        0     1676 2023-07-07 07:11:22.071252 eventix-0.8.0/eventix/functions/eventix_client.py
--rw-r--r--   0        0        0     2815 2023-07-04 08:25:54.140139 eventix-0.8.0/eventix/functions/fastapi.py
--rw-r--r--   0        0        0      858 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/functions/metrics.py
--rw-r--r--   0        0        0      426 2023-07-06 14:36:57.671160 eventix-0.8.0/eventix/functions/schedule.py
--rw-r--r--   0        0        0     7507 2023-07-13 11:00:20.373143 eventix-0.8.0/eventix/functions/task.py
--rw-r--r--   0        0        0     1155 2023-07-04 15:24:17.145091 eventix-0.8.0/eventix/functions/task_scheduler.py
--rw-r--r--   0        0        0     7605 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/functions/task_worker.py
--rw-r--r--   0        0        0      790 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/functions/tools.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/pydantic/__init__.py
--rw-r--r--   0        0        0      175 2023-07-03 12:30:27.464538 eventix-0.8.0/eventix/pydantic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1024 2023-07-03 12:35:27.342561 eventix-0.8.0/eventix/pydantic/__pycache__/event.cpython-311.pyc
--rw-r--r--   0        0        0     1670 2023-07-12 07:19:14.222636 eventix-0.8.0/eventix/pydantic/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0        0        0     1666 2023-07-06 19:19:55.403553 eventix-0.8.0/eventix/pydantic/__pycache__/schedule.cpython-311.pyc
--rw-r--r--   0        0        0     3075 2023-07-13 11:01:55.584489 eventix-0.8.0/eventix/pydantic/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/pydantic/event.py
--rw-r--r--   0        0        0      615 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/pydantic/pagination.py
--rw-r--r--   0        0        0      634 2023-07-06 19:19:42.803712 eventix-0.8.0/eventix/pydantic/schedule.py
--rw-r--r--   0        0        0     2063 2023-07-13 11:01:52.956508 eventix-0.8.0/eventix/pydantic/task.py
--rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.0/eventix/router/__init__.py
--rw-r--r--   0        0        0      173 2023-07-03 12:35:27.342561 eventix-0.8.0/eventix/router/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      989 2023-07-12 07:19:14.258636 eventix-0.8.0/eventix/router/__pycache__/default.cpython-311.pyc
--rw-r--r--   0        0        0      748 2023-07-12 07:19:14.246636 eventix-0.8.0/eventix/router/__pycache__/metrics.cpython-311.pyc
--rw-r--r--   0        0        0     2068 2023-07-12 07:19:14.250636 eventix-0.8.0/eventix/router/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     2577 2023-07-12 07:19:14.258636 eventix-0.8.0/eventix/router/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0      340 2023-07-12 07:18:50.098891 eventix-0.8.0/eventix/router/default.py
--rw-r--r--   0        0        0      243 2023-07-12 07:18:50.102891 eventix-0.8.0/eventix/router/metrics.py
--rw-r--r--   0        0        0      913 2023-07-12 07:18:50.102891 eventix-0.8.0/eventix/router/task.py
--rw-r--r--   0        0        0     1386 2023-07-12 07:18:50.102891 eventix-0.8.0/eventix/router/tasks.py
--rw-r--r--   0        0        0        0 2023-07-04 19:28:16.696215 eventix-0.8.0/eventix/tasks/__init__.py
--rw-r--r--   0        0        0      172 2023-07-04 20:38:18.799048 eventix-0.8.0/eventix/tasks/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1107 2023-07-06 20:58:27.178748 eventix-0.8.0/eventix/tasks/__pycache__/cleanup.cpython-311.pyc
--rw-r--r--   0        0        0      396 2023-07-06 20:57:49.171190 eventix-0.8.0/eventix/tasks/cleanup.py
--rw-r--r--   0        0        0     1025 2023-07-14 10:59:43.151255 eventix-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 eventix-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/__init__.py
+-rw-r--r--   0        0        0     1577 2023-07-06 06:33:36.740790 eventix-0.8.1/eventix/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/depends/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.8.1/eventix/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/functions/__init__.py
+-rw-r--r--   0        0        0     4036 2023-07-06 14:36:57.587160 eventix-0.8.1/eventix/functions/core.py
+-rw-r--r--   0        0        0      950 2023-07-13 10:39:48.044793 eventix-0.8.1/eventix/functions/errors.py
+-rw-r--r--   0        0        0     1676 2023-07-07 07:11:22.071252 eventix-0.8.1/eventix/functions/eventix_client.py
+-rw-r--r--   0        0        0     2815 2023-07-04 08:25:54.140139 eventix-0.8.1/eventix/functions/fastapi.py
+-rw-r--r--   0        0        0      858 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/functions/metrics.py
+-rw-r--r--   0        0        0      426 2023-07-06 14:36:57.671160 eventix-0.8.1/eventix/functions/schedule.py
+-rw-r--r--   0        0        0     7507 2023-07-13 11:00:20.373143 eventix-0.8.1/eventix/functions/task.py
+-rw-r--r--   0        0        0     1155 2023-07-04 15:24:17.145091 eventix-0.8.1/eventix/functions/task_scheduler.py
+-rw-r--r--   0        0        0     7605 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/functions/task_worker.py
+-rw-r--r--   0        0        0      790 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/functions/tools.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/pydantic/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/pydantic/event.py
+-rw-r--r--   0        0        0      615 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/pydantic/pagination.py
+-rw-r--r--   0        0        0      634 2023-07-06 19:19:42.803712 eventix-0.8.1/eventix/pydantic/schedule.py
+-rw-r--r--   0        0        0     2063 2023-07-13 11:01:52.956508 eventix-0.8.1/eventix/pydantic/task.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.8.1/eventix/router/__init__.py
+-rw-r--r--   0        0        0      340 2023-07-12 07:18:50.098891 eventix-0.8.1/eventix/router/default.py
+-rw-r--r--   0        0        0      243 2023-07-12 07:18:50.102891 eventix-0.8.1/eventix/router/metrics.py
+-rw-r--r--   0        0        0      913 2023-07-12 07:18:50.102891 eventix-0.8.1/eventix/router/task.py
+-rw-r--r--   0        0        0     1386 2023-07-12 07:18:50.102891 eventix-0.8.1/eventix/router/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-04 19:28:16.696215 eventix-0.8.1/eventix/tasks/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-06 20:57:49.171190 eventix-0.8.1/eventix/tasks/cleanup.py
+-rw-r--r--   0        0        0     1024 2023-07-18 07:02:31.282246 eventix-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 eventix-0.8.1/PKG-INFO
```

### Comparing `eventix-0.8.0/eventix/contexts/__init__.py` & `eventix-0.8.1/eventix/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/exceptions/__init__.py` & `eventix-0.8.1/eventix/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/functions/core.py` & `eventix-0.8.1/eventix/functions/core.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/functions/errors.py` & `eventix-0.8.1/eventix/functions/errors.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/functions/eventix_client.py` & `eventix-0.8.1/eventix/functions/eventix_client.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/functions/fastapi.py` & `eventix-0.8.1/eventix/functions/fastapi.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/functions/metrics.py` & `eventix-0.8.1/eventix/functions/metrics.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/functions/task.py` & `eventix-0.8.1/eventix/functions/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/functions/task_scheduler.py` & `eventix-0.8.1/eventix/functions/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/functions/task_worker.py` & `eventix-0.8.1/eventix/functions/task_worker.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/functions/tools.py` & `eventix-0.8.1/eventix/functions/tools.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/pydantic/pagination.py` & `eventix-0.8.1/eventix/pydantic/pagination.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/pydantic/schedule.py` & `eventix-0.8.1/eventix/pydantic/schedule.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/pydantic/task.py` & `eventix-0.8.1/eventix/pydantic/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/router/task.py` & `eventix-0.8.1/eventix/router/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/eventix/router/tasks.py` & `eventix-0.8.1/eventix/router/tasks.py`

 * *Files identical despite different names*

### Comparing `eventix-0.8.0/pyproject.toml` & `eventix-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "eventix"
-version = "0.8.0"
+version = "0.8.1"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.99.1"
-uvicorn = "^0.21.0"
+uvicorn = "^0.22.0"
 python-dotenv = "^0.15.0"
 pydash = "*"
 pydantic-db-backend = {version = "^0.6.0", extras = ["couchdb"]}
 psutil = "^5.9.5"
 requests = "^2.31.0"
 toml = "^0.10.2"
 webexception = "^1.0.2"
 croniter = "^1.4.1"
 supervisor = "^4.2.5"
 
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 httpx = "^0.24.1"
 freezegun = "^1.2.2"
 coverage = "^7.2.7"
 pytest-mock = "^3.11.1"
 semantic-version = "^2.10.0"
```

### Comparing `eventix-0.8.0/PKG-INFO` & `eventix-0.8.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventix
-Version: 0.8.0
+Version: 0.8.1
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: croniter (>=1.4.1,<2.0.0)
@@ -12,15 +12,15 @@
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pydantic-db-backend[couchdb] (>=0.6.0,<0.7.0)
 Requires-Dist: pydash
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: supervisor (>=4.2.5,<5.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: webexception (>=1.0.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Eventix
 
 ## Database
```

