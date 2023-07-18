# Comparing `tmp/lugo4py-0.0.3.tar.gz` & `tmp/lugo4py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lugo4py-0.0.3.tar", last modified: Mon Jun 26 21:20:02 2023, max compression
+gzip compressed data, was "lugo4py-0.0.4.tar", last modified: Tue Jul 18 01:21:16 2023, max compression
```

## Comparing `lugo4py-0.0.3.tar` & `lugo4py-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.184534 lugo4py-0.0.3/
--rw-rw-r--   0 aquer     (1000) aquer     (1000)    35147 2023-06-26 21:12:44.000000 lugo4py-0.0.3/LICENSE.txt
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     8030 2023-06-26 21:20:02.184534 lugo4py-0.0.3/PKG-INFO
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     7634 2023-06-26 21:12:44.000000 lugo4py-0.0.3/README.md
--rw-rw-r--   0 aquer     (1000) aquer     (1000)      373 2023-06-26 21:15:07.000000 lugo4py-0.0.3/pyproject.toml
--rw-rw-r--   0 aquer     (1000) aquer     (1000)      551 2023-06-26 21:20:02.184534 lugo4py-0.0.3/setup.cfg
-drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.180534 lugo4py-0.0.3/src/
-drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.180534 lugo4py-0.0.3/src/lugo4py/
--rw-rw-r--   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/__init__.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     6886 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/client.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     1343 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/geo.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)      629 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/goal.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     1004 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/interface.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     1604 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/loader.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     6826 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/lugo.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     3697 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/mapper.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     1012 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/orientation.py
-drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.184534 lugo4py-0.0.3/src/lugo4py/protos/
--rw-rw-r--   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/__init__.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)    10066 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/broadcast_pb2.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     5946 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/broadcast_pb2_grpc.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     2672 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/health_pb2.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     3893 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/health_pb2_grpc.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     2157 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/physics_pb2.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)      159 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/physics_pb2_grpc.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     7104 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/remote_pb2.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)    12109 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/remote_pb2_grpc.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     8935 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/server_pb2.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     3897 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/protos/server_pb2_grpc.py
-drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.184534 lugo4py-0.0.3/src/lugo4py/rl/
--rw-rw-r--   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/__init__.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     3457 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/gym.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     2398 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/helper_bots.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     3741 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/interfaces.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     2473 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/remote_control.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     5510 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/rl/training_controller.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     8136 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/snapshot.py
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     3821 2023-06-26 21:12:44.000000 lugo4py-0.0.3/src/lugo4py/specs.py
-drwxrwxr-x   0 aquer     (1000) aquer     (1000)        0 2023-06-26 21:20:02.180534 lugo4py-0.0.3/src/lugo4py.egg-info/
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     8030 2023-06-26 21:20:02.000000 lugo4py-0.0.3/src/lugo4py.egg-info/PKG-INFO
--rw-rw-r--   0 aquer     (1000) aquer     (1000)     1005 2023-06-26 21:20:02.000000 lugo4py-0.0.3/src/lugo4py.egg-info/SOURCES.txt
--rw-rw-r--   0 aquer     (1000) aquer     (1000)        1 2023-06-26 21:20:02.000000 lugo4py-0.0.3/src/lugo4py.egg-info/dependency_links.txt
--rw-rw-r--   0 aquer     (1000) aquer     (1000)        8 2023-06-26 21:20:02.000000 lugo4py-0.0.3/src/lugo4py.egg-info/top_level.txt
+drwxrwxr-x   0 rubens    (1000) rubens    (1000)        0 2023-07-18 01:21:16.724131 lugo4py-0.0.4/
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)    35147 2023-02-22 23:28:00.000000 lugo4py-0.0.4/LICENSE.txt
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     8030 2023-07-18 01:21:16.724131 lugo4py-0.0.4/PKG-INFO
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     7634 2023-07-04 01:39:39.000000 lugo4py-0.0.4/README.md
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)      373 2023-07-18 01:18:53.000000 lugo4py-0.0.4/pyproject.toml
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)      551 2023-07-18 01:21:16.728132 lugo4py-0.0.4/setup.cfg
+drwxrwxr-x   0 rubens    (1000) rubens    (1000)        0 2023-07-18 01:21:16.720131 lugo4py-0.0.4/src/
+drwxrwxr-x   0 rubens    (1000) rubens    (1000)        0 2023-07-18 01:21:16.720131 lugo4py-0.0.4/src/lugo4py/
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)        0 2023-05-02 03:10:54.000000 lugo4py-0.0.4/src/lugo4py/__init__.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     6886 2023-07-14 00:57:30.000000 lugo4py-0.0.4/src/lugo4py/client.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     1343 2023-07-04 01:39:39.000000 lugo4py-0.0.4/src/lugo4py/geo.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)      629 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/goal.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     1004 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/interface.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     1604 2023-07-04 01:39:39.000000 lugo4py-0.0.4/src/lugo4py/loader.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     6826 2023-07-04 01:39:39.000000 lugo4py-0.0.4/src/lugo4py/lugo.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     3697 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/mapper.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     1012 2023-02-15 02:24:56.000000 lugo4py-0.0.4/src/lugo4py/orientation.py
+drwxrwxr-x   0 rubens    (1000) rubens    (1000)        0 2023-07-18 01:21:16.724131 lugo4py-0.0.4/src/lugo4py/protos/
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)        0 2023-03-30 22:28:08.000000 lugo4py-0.0.4/src/lugo4py/protos/__init__.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)    10066 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/protos/broadcast_pb2.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     5946 2023-04-05 22:00:41.000000 lugo4py-0.0.4/src/lugo4py/protos/broadcast_pb2_grpc.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     2672 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/protos/health_pb2.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     3893 2023-04-05 22:00:41.000000 lugo4py-0.0.4/src/lugo4py/protos/health_pb2_grpc.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     2157 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/protos/physics_pb2.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)      159 2023-02-15 02:24:56.000000 lugo4py-0.0.4/src/lugo4py/protos/physics_pb2_grpc.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     7104 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/protos/remote_pb2.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)    12109 2023-04-05 22:00:41.000000 lugo4py-0.0.4/src/lugo4py/protos/remote_pb2_grpc.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     8935 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/protos/server_pb2.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     3897 2023-04-05 22:00:41.000000 lugo4py-0.0.4/src/lugo4py/protos/server_pb2_grpc.py
+drwxrwxr-x   0 rubens    (1000) rubens    (1000)        0 2023-07-18 01:21:16.724131 lugo4py-0.0.4/src/lugo4py/rl/
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)        0 2023-02-15 02:24:56.000000 lugo4py-0.0.4/src/lugo4py/rl/__init__.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     3457 2023-07-14 00:57:17.000000 lugo4py-0.0.4/src/lugo4py/rl/gym.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     2398 2023-07-04 01:39:39.000000 lugo4py-0.0.4/src/lugo4py/rl/helper_bots.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     3741 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/rl/interfaces.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     2473 2023-05-03 03:34:13.000000 lugo4py-0.0.4/src/lugo4py/rl/remote_control.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     5510 2023-07-04 01:39:39.000000 lugo4py-0.0.4/src/lugo4py/rl/training_controller.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     8136 2023-07-04 01:39:39.000000 lugo4py-0.0.4/src/lugo4py/snapshot.py
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     3822 2023-07-14 03:02:17.000000 lugo4py-0.0.4/src/lugo4py/specs.py
+drwxrwxr-x   0 rubens    (1000) rubens    (1000)        0 2023-07-18 01:21:16.720131 lugo4py-0.0.4/src/lugo4py.egg-info/
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     8030 2023-07-18 01:21:16.000000 lugo4py-0.0.4/src/lugo4py.egg-info/PKG-INFO
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)     1005 2023-07-18 01:21:16.000000 lugo4py-0.0.4/src/lugo4py.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)        1 2023-07-18 01:21:16.000000 lugo4py-0.0.4/src/lugo4py.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubens    (1000) rubens    (1000)        8 2023-07-18 01:21:16.000000 lugo4py-0.0.4/src/lugo4py.egg-info/top_level.txt
```

### Comparing `lugo4py-0.0.3/LICENSE.txt` & `lugo4py-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/PKG-INFO` & `lugo4py-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lugo4py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Lugo4Py is a Python3 implementation of a client player for Lugo game.
 Home-page: https://lugobots.dev/
 Author: "Rubens Silva, Lucas Coelho"
 Project-URL: Homepage, https://lugobots.dev/
 Project-URL: Repository, https://github.com/lugobots/lugo4py
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `lugo4py-0.0.3/README.md` & `lugo4py-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/setup.cfg` & `lugo4py-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lugo4py
-version = 0.0.1
+version = 0.0.3
 author = "Rubens Silva, Lucas Coelho"
 description = "Client to connect to Lugo Game Server",
 long_description = file: README.md
 description-file = README.md
 url = https://lugobots.dev/
 project_urls = 
 	Source = https://github.com/CodeSolid/python-package-example-setuptools https://github.com/lugobots/lugo4py
```

### Comparing `lugo4py-0.0.3/src/lugo4py/client.py` & `lugo4py-0.0.4/src/lugo4py/client.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/geo.py` & `lugo4py-0.0.4/src/lugo4py/geo.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/goal.py` & `lugo4py-0.0.4/src/lugo4py/goal.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/interface.py` & `lugo4py-0.0.4/src/lugo4py/interface.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/loader.py` & `lugo4py-0.0.4/src/lugo4py/loader.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/lugo.py` & `lugo4py-0.0.4/src/lugo4py/lugo.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/mapper.py` & `lugo4py-0.0.4/src/lugo4py/mapper.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/orientation.py` & `lugo4py-0.0.4/src/lugo4py/orientation.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/protos/broadcast_pb2.py` & `lugo4py-0.0.4/src/lugo4py/protos/broadcast_pb2.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/protos/broadcast_pb2_grpc.py` & `lugo4py-0.0.4/src/lugo4py/protos/broadcast_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/protos/health_pb2.py` & `lugo4py-0.0.4/src/lugo4py/protos/health_pb2.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/protos/health_pb2_grpc.py` & `lugo4py-0.0.4/src/lugo4py/protos/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/protos/physics_pb2.py` & `lugo4py-0.0.4/src/lugo4py/protos/physics_pb2.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/protos/remote_pb2.py` & `lugo4py-0.0.4/src/lugo4py/protos/remote_pb2.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/protos/remote_pb2_grpc.py` & `lugo4py-0.0.4/src/lugo4py/protos/remote_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/protos/server_pb2.py` & `lugo4py-0.0.4/src/lugo4py/protos/server_pb2.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/protos/server_pb2_grpc.py` & `lugo4py-0.0.4/src/lugo4py/protos/server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/rl/gym.py` & `lugo4py-0.0.4/src/lugo4py/rl/gym.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/rl/helper_bots.py` & `lugo4py-0.0.4/src/lugo4py/rl/helper_bots.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/rl/interfaces.py` & `lugo4py-0.0.4/src/lugo4py/rl/interfaces.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/rl/remote_control.py` & `lugo4py-0.0.4/src/lugo4py/rl/remote_control.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/rl/training_controller.py` & `lugo4py-0.0.4/src/lugo4py/rl/training_controller.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/snapshot.py` & `lugo4py-0.0.4/src/lugo4py/snapshot.py`

 * *Files identical despite different names*

### Comparing `lugo4py-0.0.3/src/lugo4py/specs.py` & `lugo4py-0.0.4/src/lugo4py/specs.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
 # FIELD_HEIGHT is the height of the field (horizontal view)
 # This value must be an odd number because we cant to a coordinate at the perfect middle of the field
 # e.g. If the field height is 10, and the coordinates go from 0 to 9, there is no precise middle.
 # Thus, the field height would have to be 11, so the coordinate 5 is at the precise center
 FIELD_HEIGHT = max_y_coordinate + 1
 
-# FIELD_NEUTRAL_CENTER is the radius of the neutral circle on the center of the field
-FIELD_NEUTRAL_CENTER = 100
+# FIELD_NEUTRAL_CENTER is the radius of the neutral circle in the center of the field
+FIELD_NEUTRAL_CENTER = 1000
 
 # BALL_SIZE size of the element ball
 BALL_SIZE = 2 * BASE_UNIT
 
 # BALL_DECELERATION is the deceleration rate of the ball speed  by frame
 BALL_DECELERATION = 10.0
```

### Comparing `lugo4py-0.0.3/src/lugo4py.egg-info/PKG-INFO` & `lugo4py-0.0.4/src/lugo4py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lugo4py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Lugo4Py is a Python3 implementation of a client player for Lugo game.
 Home-page: https://lugobots.dev/
 Author: "Rubens Silva, Lucas Coelho"
 Project-URL: Homepage, https://lugobots.dev/
 Project-URL: Repository, https://github.com/lugobots/lugo4py
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `lugo4py-0.0.3/src/lugo4py.egg-info/SOURCES.txt` & `lugo4py-0.0.4/src/lugo4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

