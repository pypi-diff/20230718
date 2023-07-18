# Comparing `tmp/taichu-serve-2.0.31.tar.gz` & `tmp/taichu-serve-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taichu-serve-2.0.31.tar", last modified: Tue Jul 18 09:10:23 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.9.tar", last modified: Wed Apr 19 02:34:49 2023, max compression
```

## Comparing `taichu-serve-2.0.31.tar` & `taichu-serve-2.0.9.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/
--rw-r--r--   0 caiyueliang   (501) staff       (20)      236 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/PKG-INFO
--rw-r--r--   0 caiyueliang   (501) staff       (20)     7501 2023-07-12 08:51:53.000000 taichu-serve-2.0.31/README.md
--rw-r--r--   0 caiyueliang   (501) staff       (20)       38 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/setup.cfg
--rw-r--r--   0 caiyueliang   (501) staff       (20)     1244 2023-07-18 09:08:29.000000 taichu-serve-2.0.31/setup.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve/
--rw-r--r--   0 caiyueliang   (501) staff       (20)     4712 2023-05-11 03:11:54.000000 taichu-serve-2.0.31/taichu_serve/__init__.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)    14450 2023-07-18 09:03:53.000000 taichu-serve-2.0.31/taichu_serve/app.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     8721 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/command.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      889 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/common.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     6712 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/dockerfile.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     1521 2023-07-18 08:53:12.000000 taichu-serve-2.0.31/taichu_serve/error_code.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     6336 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/grpc_predict_v2_pb2.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)    13010 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     6812 2023-05-09 09:29:15.000000 taichu-serve-2.0.31/taichu_serve/grpc_server.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     2316 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/log.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     5481 2023-05-09 10:49:43.000000 taichu-serve-2.0.31/taichu_serve/model_server.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      205 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/ratelimiter.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     3351 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/settings.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve/template/
--rw-r--r--   0 caiyueliang   (501) staff       (20)        0 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/template/__init__.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      848 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/template/model_service.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve/template/test/
--rw-r--r--   0 caiyueliang   (501) staff       (20)        0 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/template/test/__init__.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      691 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/template/test/grpc_client.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      286 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/template/test/http_client.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)      932 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/template/test/stream_grpc_client.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve/third/
--rw-r--r--   0 caiyueliang   (501) staff       (20)        0 2023-05-09 04:36:22.000000 taichu-serve-2.0.31/taichu_serve/third/__init__.py
--rw-r--r--   0 caiyueliang   (501) staff       (20)     2988 2023-05-10 07:54:39.000000 taichu-serve-2.0.31/taichu_serve/third/tracer.py
-drwxr-xr-x   0 caiyueliang   (501) staff       (20)        0 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve.egg-info/
--rw-r--r--   0 caiyueliang   (501) staff       (20)      236 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 caiyueliang   (501) staff       (20)      894 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 caiyueliang   (501) staff       (20)        1 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 caiyueliang   (501) staff       (20)       58 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 caiyueliang   (501) staff       (20)      194 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 caiyueliang   (501) staff       (20)       13 2023-07-18 09:10:23.000000 taichu-serve-2.0.31/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.797402 taichu-serve-2.0.9/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:34:49.797253 taichu-serve-2.0.9/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-19 02:34:49.797443 taichu-serve-2.0.9/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      947 2023-04-19 02:34:18.000000 taichu-serve-2.0.9/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.793674 taichu-serve-2.0.9/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.9/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.9/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     5479 2023-04-19 02:05:09.000000 taichu-serve-2.0.9/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      934 2023-04-18 09:03:28.000000 taichu-serve-2.0.9/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     2118 2023-04-19 02:34:18.000000 taichu-serve-2.0.9/taichu_serve/dockerfile.py
+-rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.9/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.9/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.9/taichu_serve/log.py
+-rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.9/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.9/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     2253 2023-04-19 01:27:54.000000 taichu-serve-2.0.9/taichu_serve/settings.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.795889 taichu-serve-2.0.9/taichu_serve/template/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.9/taichu_serve/template/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      123 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/config.ini
+-rw-r--r--   0 chen       (501) staff       (20)      741 2023-04-18 03:02:30.000000 taichu-serve-2.0.9/taichu_serve/template/customize_service.py
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-18 03:02:30.000000 taichu-serve-2.0.9/taichu_serve/template/requirements.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.796946 taichu-serve-2.0.9/taichu_serve/template/test/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-04-18 02:46:49.000000 taichu-serve-2.0.9/taichu_serve/template/test/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)      690 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/test/grpc_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      285 2023-04-18 08:45:26.000000 taichu-serve-2.0.9/taichu_serve/template/test/http_client.py
+-rw-r--r--   0 chen       (501) staff       (20)      931 2023-04-18 08:48:18.000000 taichu-serve-2.0.9/taichu_serve/template/test/stream_grpc_client.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-19 02:34:49.794937 taichu-serve-2.0.9/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      900 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-19 02:34:49.000000 taichu-serve-2.0.9/taichu_serve.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `taichu-serve-2.0.31/taichu_serve/app.py` & `taichu-serve-2.0.9/taichu_serve/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 # -*- coding: utf-8 -*-
 """
 DL webservice app
 """
+import ctypes
 import inspect
 import json
 import logging
 import os
-import sys
 import threading
 import time
 import traceback
-import typing
-import pickle
 import uuid
-import retry
-from opentelemetry import trace
-from opentelemetry.trace import set_span_in_context
 
 from flask import Flask, request, g
 
 from taichu_serve.log import init_logger
 from taichu_serve.settings import parse_args
 from taichu_serve.ratelimiter import semaphore
 
-args = parse_args()
-if args.env == "prod":
-    init_logger(json_format=True)
-else:
-    init_logger()
+init_logger()
 
-app = Flask("app")
+app = Flask("aa")
 
 from taichu_serve.error_code import ModelNotFoundError, ModelPredictError, TooManyRequestsError
-from taichu_serve import ModelServer
+from taichu_serve import Service
 from taichu_serve.common import Local
-from taichu_serve.third import tracer
-
 
 LOGGER = logging.getLogger(__name__)
 
 import multiprocessing
 
+args = parse_args()
+
 workers_status = []
 
 
 class WorkersPipeMgr(object):
     def __init__(self, num):
         self._list = []
         self._occupied = []
@@ -77,14 +68,15 @@
 
 
 workers_pipe = WorkersPipeMgr(args.instances_num)
 
 
 def worker_main_loop(args, pipe, status):
     # pwd = os.path.dirname(os.path.abspath(__file__))
+
     # args = parse_args()
 
     LOGGER.info("args: %s", args)
 
     from taichu_serve.model_server import load_service
     dict_model_service = {}
 
@@ -93,42 +85,30 @@
 
     model_service_file = args.service_file
 
     print(
         "model_path={} \n model_service_file={} "
         .format(model_path, model_service_file))
 
-    if not os.path.exists(model_path):
-        LOGGER.error("model_path not found.")
-        sys.exit(1)
-    if model_service_file is None:
-        LOGGER.error("model_service_file not found.")
-        sys.exit(1)
-    # 检查model_service_file是否存在
-    if model_service_file and not os.path.exists(os.path.join(model_path, model_service_file)):
-        LOGGER.error("model_service_file not found.")
-        sys.exit(1)
-
     module = load_service(os.path.join(model_path, model_service_file)
-                          ) if model_service_file else ModelServer
+                          ) if model_service_file else Service
     classes = [cls[1] for cls in inspect.getmembers(module, inspect.isclass)]
 
-    # 如果没有自定义的ModelServer，则退出
-    if len(classes) == 0:
-        LOGGER.error("No user defined ModelServer found.")
-        sys.exit(1)
+    assert len(classes) > 0, "There should be one user defined service derived from ModelService."
 
     class_defs = list(
         filter(
-            lambda c: issubclass(c, ModelServer) and len(
+            lambda c: issubclass(c, Service) and len(
                 c.__subclasses__()) == 0, classes))
 
-    if len(class_defs) == 0:
-        LOGGER.error("No user defined ModelServer found.")
-        sys.exit(1)
+    # if len(class_defs) != 1:
+    #     raise Exception(
+    #         'There should be one user defined service derived from ModelService.'
+    #     )
+    assert len(class_defs) > 0, "There should be one user defined service derived from ModelService."
 
     for c in class_defs:
         LOGGER.info("class_defs: %s", c.__name__)
         instance = c(model_path)
         # threading.Thread(target=instance.warmup).start()
         instance.warmup()
         dict_model_service[f'{str(c.__name__).lower()}_{instance.model_version.lower()}'] = instance
@@ -139,163 +119,51 @@
 
     while True:
         data = pipe.recv()
         try:
             model_name = data.get('model_name')
             model_version = data.get('model_version')
             request_id = data.get('request_id', str(uuid.uuid4()))
-            span_ctx = pickle.loads(data.get('span_ctx').encode('latin1'))
 
             Local.request_id = request_id
-            LOGGER.info("[worker_main_loop] recv a request: %s", request_id)
-            stream = False
             ins = dict_model_service.get(f'{model_name.lower()}_{model_version.lower()}', None)
             if ins is None:
-                LOGGER.error("[worker_main_loop] model not found: %s", model_name)
                 ret = {
                     'data': None,
                     'status': 'error',
                     'error': 'model not found',
                 }
-                pipe.send(ret)
-                continue
-
-            method = data.get('method', None)
-            if method == 'destroy_context':
-                LOGGER.info("[worker_main_loop] destroy context: %s", request_id)
-                ins.destroy_context(request_id)
-
-                ret = {'status': 'ok'}
-                pipe.send(ret)
-                continue
-
-            stream = data.get('stream', False)
-            resp = ins.inference(data.get('data'), request_id, span_ctx=span_ctx, stream=stream)
-            cnt = 0
-            if stream:
-                for item in resp:
-                    ret = {
-                        'data': item,
-                        'status': 'ok',
-                    }
-                    pipe.send(ret)
-                    cnt += 1
             else:
-                all_resp = []
                 ret = {
+                    'data': ins.inference(data.get('data'), request_id),
                     'status': 'ok',
                 }
-                for item in resp:
-                    all_resp.append(item)
-
-                if len(all_resp) > 1:
-                    LOGGER.error("[worker_main_loop] stream is false, but got more than one item")
-                    data = {}
-                    for index, item in enumerate(all_resp):
-                        data[f'item_{index}'] = json.dumps(item)
-                    ret['data'] = data
-
-                if len(all_resp) == 0:
-                    raise ModelPredictError("no response")
-
-                if len(all_resp) == 1:
-                    ret['data'] = all_resp[0]
-
-                pipe.send(ret)
-
         except Exception as e:
             LOGGER.error(traceback.format_exc())
             ret = {
                 'data': None,
                 'status': 'error',
                 'error': str(e),
             }
-            pipe.send(ret)
-        finally:
-            if stream:
-                pipe.send({
-                    'status': 'end'
-                })
-
-@retry.retry(tries=60, delay=1, logger=LOGGER)
-def get_worker(request_id):
-    p = workers_pipe.acquire(request_id)
-    if p is None:
-        raise TooManyRequestsError()
-    return p
-
-
-@tracer.tracer.start_as_current_span("model_stream_inference")
-def model_stream_inference(model_name, model_version, data, request_id, method=None):
-    try:
-        with tracer.tracer.start_as_current_span("pipe-acquire") as span:
-            tracer.add_event(span=span, name="[model_stream_inference] pipe acquire start")
-            # p = workers_pipe.acquire(request_id)
-            # if p is None:
-            #     raise TooManyRequestsError()
-            p = get_worker(request_id=request_id)
-            tracer.add_event(span=span, name="[model_stream_inference] pipe acquire end")
-
-        with tracer.tracer.start_as_current_span("pipe-send") as span:
-            span_ctx = trace.get_current_span().get_span_context()
-            payload = {'model_name': model_name, 'model_version': model_version, 'data': data,
-                       'request_id': request_id, 'stream': True,
-                       'span_ctx': pickle.dumps(span_ctx).decode('latin1')}
-            if method:
-                payload['method'] = method
-
-            tracer.add_event(span=span, name="[model_stream_inference] pipe send")
-            p.send(payload)
-            while True:
-                ret = p.recv()
-                tracer.add_event(span=span, name="[model_stream_inference] pipe recv")
-                if ret.get('status') == 'error':
-                    tracer.add_event(span=span, name="[model_stream_inference] pipe error")
-                    raise ModelPredictError(message=ret.get('error'))
-
-                if ret.get('status') == 'end':
-                    tracer.add_event(span=span, name="[model_stream_inference] pipe end")
-                    return
+        pipe.send(ret)
 
-                yield ret.get('data')
+    # return dict_model_service
 
-    finally:
-        if p is not None:
-            workers_pipe.release(request_id)
 
-
-@tracer.tracer.start_as_current_span("model_inference")
-def model_inference(model_name, model_version, data, request_id, method=None):
+def model_inference(model_name, model_version, data, request_id):
     try:
-        with tracer.tracer.start_as_current_span("pipe-acquire") as span:
-            tracer.add_event(span=span, name="[model_inference] pipe acquire start")
-            # p = workers_pipe.acquire(request_id)
-            # if p is None:
-            #     LOGGER.info("no available worker")
-            #     raise TooManyRequestsError()
-            p = get_worker(request_id=request_id)
-            tracer.add_event(span=span, name="[model_inference] pipe acquire start")
-
-        with tracer.tracer.start_as_current_span("pipe-send") as span:
-            span_ctx = trace.get_current_span().get_span_context()
-            payload = {'model_name': model_name, 'model_version': model_version, 'data': data,
-                       'request_id': request_id, 'stream': False,
-                       'span_ctx': pickle.dumps(span_ctx).decode('latin1')}
-            if method:
-                payload['method'] = method
-
-            tracer.add_event(span=span, name="[model_inference] pipe send")
-            p.send(payload)
-            ret = p.recv()
-            tracer.add_event(span=span, name="[model_inference] pipe recv")
-
-            if ret.get('status') == 'error':
-                raise ModelPredictError(message=ret.get('error'))
-            return ret.get('data')
-
+        p = workers_pipe.acquire(request_id)
+        if p is None:
+            raise TooManyRequestsError()
+        p.send({'model_name': model_name, 'model_version': model_version, 'data': data, 'request_id': request_id})
+        ret = p.recv()
+
+        if ret.get('status') == 'error':
+            raise ModelPredictError(message=ret.get('error'))
+        return ret.get('data')
     finally:
         if p is not None:
             workers_pipe.release(request_id)
 
 
 def init_model_service_instance():
     for i in range(args.instances_num):
```

### Comparing `taichu-serve-2.0.31/taichu_serve/common.py` & `taichu-serve-2.0.9/taichu_serve/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 Local = threading.local()
 logger = logging.getLogger(__name__)
 
 
 def grpc_interceptor(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
+        Local.request_id = str(uuid.uuid4())
         context = args[2]
         start_time = time.time()
         try:
             ret = func(*args, **kwargs)
         except ModelPredictError as e:
             logger.error('[grpc_interceptor] error: %s', e.message)
             context.set_code(grpc.StatusCode.INTERNAL)
```

### Comparing `taichu-serve-2.0.31/taichu_serve/error_code.py` & `taichu-serve-2.0.9/taichu_serve/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.31/taichu_serve/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.31/taichu_serve/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.9/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.31/taichu_serve/log.py` & `taichu-serve-2.0.9/taichu_serve/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,18 +53,14 @@
         for (k, v) in record.__dict__.items():
             if k not in exclude_fields:
                 data[k] = v
 
         return json.dumps(data, ensure_ascii=False)
 
 
-def init_logger(json_format: bool = False):
+def init_logger():
     logging.basicConfig(level=logging.INFO)
     logger = logging.getLogger()
     logger.handlers = []
     consoleHandler = logging.StreamHandler(stream=sys.stdout)
-    if json_format:
-        consoleHandler.setFormatter(JsonFormatter(datefmt='%Y-%m-%d %H:%M:%S'))
-    else:
-        consoleHandler.setFormatter(
-            logging.Formatter('%(asctime)s %(levelname)s %(pathname)s:%(lineno)d - [PID:%(process)d] %(message)s'))
+    consoleHandler.setFormatter(JsonFormatter(datefmt='%Y-%m-%d %H:%M:%S'))
     logger.addHandler(consoleHandler)
```

### Comparing `taichu-serve-2.0.31/taichu_serve/model_server.py` & `taichu-serve-2.0.9/taichu_serve/model_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     '''ModelService wraps up all preprocessing, inference and postprocessing
     functions used by model service. It is defined in a flexible manner to
     be easily extended to support different frameworks.
     '''
     __metaclass__ = ABCMeta
 
     def __init__(self, model_path):
-        self.model_path = model_path
+        self.ctx = None
 
     @abstractmethod
-    def inference(self, data, request_id, span_ctx, stream=False):
+    def inference(self, data, request_id):
         '''
         Wrapper function to run preprocess, inference and postprocess functions.
 
         Parameters
         ----------
         data : map of object
             Raw input from request.
```

### Comparing `taichu-serve-2.0.31/taichu_serve/template/test/grpc_client.py` & `taichu-serve-2.0.9/taichu_serve/template/test/grpc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import grpc
 import taichu_serve.grpc_predict_v2_pb2 as grpc_predict_v2_pb2
 import taichu_serve.grpc_predict_v2_pb2_grpc as grpc_predict_v2_pb2_grpc
 
-model_name = "ModelService"
+model_name = "TestService"
 
 
 def run():
     conn = grpc.insecure_channel('localhost:8080')
     client = grpc_predict_v2_pb2_grpc.GRPCInferenceServiceStub(channel=conn)
 
     req = grpc_predict_v2_pb2.ModelInferRequest()
```

### Comparing `taichu-serve-2.0.31/taichu_serve/template/test/stream_grpc_client.py` & `taichu-serve-2.0.9/taichu_serve/template/test/stream_grpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import grpc
 import taichu_serve.grpc_predict_v2_pb2 as grpc_predict_v2_pb2
 import taichu_serve.grpc_predict_v2_pb2_grpc as grpc_predict_v2_pb2_grpc
 
-model_name = "ModelService"
+model_name = "TestService"
 
 
 def guide_list_features(stub):
     num = 5
 
     while True:
```

### Comparing `taichu-serve-2.0.31/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-2.0.9/taichu_serve.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.md
 setup.py
 taichu_serve/__init__.py
 taichu_serve/app.py
 taichu_serve/command.py
 taichu_serve/common.py
 taichu_serve/dockerfile.py
 taichu_serve/error_code.py
@@ -16,14 +15,14 @@
 taichu_serve.egg-info/PKG-INFO
 taichu_serve.egg-info/SOURCES.txt
 taichu_serve.egg-info/dependency_links.txt
 taichu_serve.egg-info/entry_points.txt
 taichu_serve.egg-info/requires.txt
 taichu_serve.egg-info/top_level.txt
 taichu_serve/template/__init__.py
-taichu_serve/template/model_service.py
+taichu_serve/template/config.ini
+taichu_serve/template/customize_service.py
+taichu_serve/template/requirements.txt
 taichu_serve/template/test/__init__.py
 taichu_serve/template/test/grpc_client.py
 taichu_serve/template/test/http_client.py
-taichu_serve/template/test/stream_grpc_client.py
-taichu_serve/third/__init__.py
-taichu_serve/third/tracer.py
+taichu_serve/template/test/stream_grpc_client.py
```

