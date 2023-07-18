# Comparing `tmp/elefantolib_events-0.5.0.tar.gz` & `tmp/elefantolib_events-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_events-0.5.0.tar", max compression
+gzip compressed data, was "elefantolib_events-0.6.0.tar", max compression
```

## Comparing `elefantolib_events-0.5.0.tar` & `elefantolib_events-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/elefantolib_events/__init__.py
--rw-r--r--   0        0        0      765 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/elefantolib_events/emitter.py
--rw-r--r--   0        0        0     1071 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/elefantolib_events/listener.py
--rw-r--r--   0        0        0      336 2023-06-20 14:38:04.671449 elefantolib_events-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 elefantolib_events-0.5.0/setup.py
--rw-r--r--   0        0        0      331 1970-01-01 00:00:00.000000 elefantolib_events-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 14:29:27.899414 elefantolib_events-0.6.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-18 14:29:27.899414 elefantolib_events-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 14:29:27.899414 elefantolib_events-0.6.0/elefantolib_events/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-18 14:29:27.899414 elefantolib_events-0.6.0/elefantolib_events/emitter.py
+-rw-r--r--   0        0        0     1072 2023-07-18 14:29:27.899414 elefantolib_events-0.6.0/elefantolib_events/listener.py
+-rw-r--r--   0        0        0      336 2023-07-18 14:29:39.691365 elefantolib_events-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 elefantolib_events-0.6.0/setup.py
+-rw-r--r--   0        0        0      331 1970-01-01 00:00:00.000000 elefantolib_events-0.6.0/PKG-INFO
```

### Comparing `elefantolib_events-0.5.0/LICENSE` & `elefantolib_events-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elefantolib_events-0.5.0/elefantolib_events/emitter.py` & `elefantolib_events-0.6.0/elefantolib_events/emitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
     async def emit(self, event_name: str, payload: dict) -> None:
         connection = await aio_pika.connect(self.rabbitmq_url)
 
         async with connection:
             channel = await connection.channel()
             await channel.declare_queue(event_name)
 
-            exchange = await channel.declare_exchange(event_name, ExchangeType.TOPIC)
+            exchange = await channel.declare_exchange(event_name, ExchangeType.FANOUT)
             body = json.dumps(payload, default=str)
             await exchange.publish(
                 aio_pika.Message(body=str.encode(body), delivery_mode=DeliveryMode.PERSISTENT),
                 routing_key=event_name,
             )
```

### Comparing `elefantolib_events-0.5.0/elefantolib_events/listener.py` & `elefantolib_events-0.6.0/elefantolib_events/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     async def listen(self, event_name, fn):
         connection = await self._connections.get()
 
         async with connection:
             channel = await connection.channel()
             queue = await channel.declare_queue(event_name)
-            exchange = await channel.declare_exchange(event_name, ExchangeType.TOPIC)
+            exchange = await channel.declare_exchange(event_name, ExchangeType.FANOUT)
 
             await queue.bind(exchange)
 
             async with queue.iterator() as queue_iter:
                 async for message in queue_iter:
                     async with message.process():
                         data = json.loads(message.body.decode())
```

### Comparing `elefantolib_events-0.5.0/setup.py` & `elefantolib_events-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aio-pika>=9.1.2,<10.0.0']
 
 setup_kwargs = {
     'name': 'elefantolib-events',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': '',
     'long_description': '',
     'author': 'Aibar',
     'author_email': 'bekaybar@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

