# Comparing `tmp/miauw-base-service-1.8.0.tar.gz` & `tmp/miauw-base-service-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.8.0.tar", last modified: Sun Jul 16 15:16:58 2023, max compression
+gzip compressed data, was "miauw-base-service-1.9.0.tar", last modified: Tue Jul 18 06:47:12 2023, max compression
```

## Comparing `miauw-base-service-1.8.0.tar` & `miauw-base-service-1.9.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 15:16:58.571073 miauw-base-service-1.8.0/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 15:16:58.571073 miauw-base-service-1.8.0/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 15:16:58.567740 miauw-base-service-1.8.0/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)      110 2023-07-16 11:46:05.000000 miauw-base-service-1.8.0/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1154 2023-07-16 11:46:05.000000 miauw-base-service-1.8.0/base_service/email_worker.py
--rw-r--r--   0 leo       (1000) leo       (1000)      528 2023-07-16 11:46:05.000000 miauw-base-service-1.8.0/base_service/exceptions.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2226 2023-07-16 15:16:48.000000 miauw-base-service-1.8.0/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2715 2023-07-16 15:16:48.000000 miauw-base-service-1.8.0/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-16 15:16:58.567740 miauw-base-service-1.8.0/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      360 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-16 15:16:58.000000 miauw-base-service-1.8.0/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-16 15:16:48.000000 miauw-base-service-1.8.0/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-16 15:16:58.571073 miauw-base-service-1.8.0/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-16 15:16:48.000000 miauw-base-service-1.8.0/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)      110 2023-07-16 11:46:05.000000 miauw-base-service-1.9.0/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1154 2023-07-16 11:46:05.000000 miauw-base-service-1.9.0/base_service/email_worker.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      528 2023-07-16 11:46:05.000000 miauw-base-service-1.9.0/base_service/exceptions.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4137 2023-07-18 06:41:20.000000 miauw-base-service-1.9.0/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      875 2023-07-18 06:17:46.000000 miauw-base-service-1.9.0/base_service/utils.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2669 2023-07-18 06:00:14.000000 miauw-base-service-1.9.0/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      382 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       44 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-18 06:47:12.000000 miauw-base-service-1.9.0/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      332 2023-07-18 06:38:20.000000 miauw-base-service-1.9.0/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-18 06:47:12.845892 miauw-base-service-1.9.0/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-18 06:39:06.000000 miauw-base-service-1.9.0/setup.py
```

### Comparing `miauw-base-service-1.8.0/base_service/email_worker.py` & `miauw-base-service-1.9.0/base_service/email_worker.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.8.0/base_service/exceptions.py` & `miauw-base-service-1.9.0/base_service/exceptions.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.8.0/base_service/worker.py` & `miauw-base-service-1.9.0/base_service/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Callable, Awaitable, Any
 import aio_pika
 import json
-import asyncio
 import traceback
 import os
 
 
 class RabbitMQWorker:
     """RabbitMQ Base Worker Class"""
 
@@ -21,17 +20,17 @@
         self.channel = await self.connection.channel(channel_number=chan_id)
         self.ex = self.channel.default_exchange
         return self
 
     async def send(self, queue_name: str, data: dict | str | bytes) -> None:
         """sends something to queue"""
         try:
-            data = json.loads(message.body)
+            data = json.dumps(data).encode("utf-8")
         except json.JSONDecodeError:
-            data = message.body.decode("utf-8")
+            data = data.encode("utf-8")
         await self.ex.publish(aio_pika.Message(data), routing_key=queue_name)
 
     async def listen(
         self,
         queue_name: str,
         worker_function: Callable[[Any], Awaitable[Any]]
     ):
@@ -44,15 +43,14 @@
                     async with message.process(requeue=False):
                         assert message.reply_to is not None
                         try:
                             data = json.loads(message.body)
                         except json.JSONDecodeError:
                             data = message.body.decode("utf-8")
                         res = await worker_function(data)
-                        return
                         await self.ex.publish(
                             aio_pika.Message(
                                 body=json.dumps(res).encode("utf-8"),
                                 correlation_id=message.correlation_id,
                             ),
                             routing_key=message.reply_to,
                         )
```

