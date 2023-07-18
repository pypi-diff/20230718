# Comparing `tmp/suanpan-sprt-0.6.2.tar.gz` & `tmp/suanpan-sprt-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.6.2.tar", last modified: Mon Jul 17 07:00:32 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.6.3.tar", last modified: Tue Jul 18 07:58:15 2023, max compression
```

## Comparing `suanpan-sprt-0.6.2.tar` & `suanpan-sprt-0.6.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4249 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5713 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.2/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2087 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.2/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6628 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.2/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.2/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-17 07:00:32.000000 suanpan-sprt-0.6.2/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4317 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5737 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2087 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.3/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6902 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.3/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.3/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.6.2/setup.py` & `suanpan-sprt-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.2/sprt/__main__.py` & `suanpan-sprt-0.6.3/sprt/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     signal.signal(signal.SIGTERM, receive_signal)
     signal.signal(signal.SIGINT, receive_signal)
     app = server.create_app(working_dir, log_file, new_log)
     app.logger.info(f'use {log_file} {log_level} {new_log}')
 
     config = Config()
     config.bind = [f'{host}:{port}']
+    if log_level.upper() == 'DEBUG':
+        config.accesslog = '-'
     app.logger.info(f'python runtime running on {host}:{port}')
     asyncio.run(serve(app, config))
 
 
 def receive_signal(signal_number, frame):
     print('receive_signal', signal_number)
     sys.exit(128 + signal_number)
```

### Comparing `suanpan-sprt-0.6.2/sprt/arguments.py` & `suanpan-sprt-0.6.3/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.2/sprt/envs.py` & `suanpan-sprt-0.6.3/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.2/sprt/loader.py` & `suanpan-sprt-0.6.3/sprt/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         logger.addHandler(sh)
 
         return logger
 
     def __del__(self):
         # os.remove(self.location)
         self._logkit.handlers.clear()
+        del self.module
 
 
 class RuntimeContext(object):
     def __init__(self, user_id, app_id, node_id):
         self.request_id = None
         self.user_id = user_id
         self.app_id = app_id
```

### Comparing `suanpan-sprt-0.6.2/sprt/log.py` & `suanpan-sprt-0.6.3/sprt/log.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.2/sprt/master.py` & `suanpan-sprt-0.6.3/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.2/sprt/server.py` & `suanpan-sprt-0.6.3/sprt/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import gc
 import json
 import logging
 import typing
 import pathlib
 import dataclasses
 import pydantic
 from contextlib import redirect_stdout, redirect_stderr, contextmanager
@@ -86,16 +87,16 @@
 def create_app(working_dir='.', log_file='', new_log=False):
     log_path = pathlib.Path(log_file).parent.parent
     app = Quart(__name__)
     QuartSchema(app)
 
     @app.post("/")
     @validate_request(FunctionParams)
-    @validate_response(FunctionResponse)
-    async def function_invoke(data: FunctionParams) -> FunctionResponse:
+    # @validate_response(FunctionResponse)
+    async def function_invoke(data: FunctionParams):
         user_id = data.context.user_id
         app_id = data.context.app_id
         node_id = data.context.node_id
         if new_log:
             log_dir = log_path / f'{app_id}-{user_id}-{node_id}'
             log_dir.mkdir(parents=True, exist_ok=True)
             log_name = log_dir / f'app-{app_id}-{node_id}'
@@ -119,14 +120,17 @@
                 except Exception as e:
                     if function is not None:
                         function.context.log.exception(f'event error: {e}')
                     else:
                         logging.exception(f'event error: {e}')
                     resp = FunctionResponse(id=data.id, success=False, error=str(e))
 
+        r = dataclasses.asdict(resp)
+        resp = await app.make_response(json.dumps(r))
+        resp.timeout = 2
         return resp
 
     @app.errorhandler(RequestSchemaValidationError)
     async def handle_request_validation_error(error):
         if isinstance(error.validation_error, TypeError):
             err = str(error.validation_error)
         else:
@@ -134,33 +138,40 @@
 
         return {"errors": err}, 400
 
     @app.post("/function/release")
     @validate_request(FunctionReleaseParams)
     @validate_response(FunctionReleaseResponse)
     async def function_release(data: FunctionReleaseParams) -> FunctionReleaseResponse:
-        for node_id in list(module_imported):
-            node_function = module_imported[node_id]
-            if node_function.context.app_id == data.app_id:
-                logging.info(f'node {node_id} release')
-                del module_imported[node_id]
-
+        app.add_background_task(background_garbage_collection, data.app_id)
         return FunctionReleaseResponse(success=True)
 
     @app.get("/health/liveness")
     async def liveness():
         return "OK"
 
     @app.get("/health/readiness")
     async def readiness():
         return "OK"
 
     return app
 
 
+async def background_garbage_collection(app_id):
+    del_nodes = []
+    for node_id, node_function in module_imported.items():
+        if node_function.context.app_id == app_id:
+            del_nodes.append(node_id)
+
+    for node_id in del_nodes:
+        logging.info(f'node {node_id} release')
+        del module_imported[node_id]
+
+    gc.collect()
+
 module_imported = {}
 
 
 def load(data: FunctionParams, default_dir):
     user_id = data.context.user_id
     app_id = data.context.app_id
     node_id = data.context.node_id
```

### Comparing `suanpan-sprt-0.6.2/sprt/storage.py` & `suanpan-sprt-0.6.3/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.2/sprt/testing.py` & `suanpan-sprt-0.6.3/sprt/testing.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.2/sprt/utils.py` & `suanpan-sprt-0.6.3/sprt/utils.py`

 * *Files identical despite different names*

