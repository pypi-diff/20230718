# Comparing `tmp/mrsal-0.5.0a0.tar.gz` & `tmp/mrsal-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrsal-0.5.0a0.tar", max compression
+gzip compressed data, was "mrsal-0.6.0a0.tar", max compression
```

## Comparing `mrsal-0.5.0a0.tar` & `mrsal-0.6.0a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35148 2022-09-08 10:55:29.050700 mrsal-0.5.0a0/LICENSE.txt
--rw-r--r--   0        0        0     8736 2023-05-16 08:38:05.358774 mrsal-0.5.0a0/README.md
--rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.5.0a0/mrsal/__init__.py
--rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.5.0a0/mrsal/config/__init__.py
--rw-r--r--   0        0        0     1345 2023-05-16 08:04:45.500230 mrsal-0.5.0a0/mrsal/config/config.py
--rw-r--r--   0        0        0      286 2023-04-26 07:24:07.167406 mrsal-0.5.0a0/mrsal/config/exceptions.py
--rw-r--r--   0        0        0     2431 2022-08-17 10:39:13.102254 mrsal-0.5.0a0/mrsal/config/logging.py
--rw-r--r--   0        0        0    32547 2023-05-16 08:04:00.028901 mrsal-0.5.0a0/mrsal/mrsal.py
--rw-r--r--   0        0        0      330 2023-05-16 08:04:59.520011 mrsal-0.5.0a0/mrsal/utils/utils.py
--rw-r--r--   0        0        0      684 2023-05-16 08:39:42.918078 mrsal-0.5.0a0/pyproject.toml
--rw-r--r--   0        0        0     9473 1970-01-01 00:00:00.000000 mrsal-0.5.0a0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-09-08 10:55:29.050700 mrsal-0.6.0a0/LICENSE.txt
+-rw-r--r--   0        0        0     8736 2023-05-22 09:49:44.867143 mrsal-0.6.0a0/README.md
+-rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.6.0a0/mrsal/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.6.0a0/mrsal/config/__init__.py
+-rw-r--r--   0        0        0     1349 2023-07-18 07:37:02.804267 mrsal-0.6.0a0/mrsal/config/config.py
+-rw-r--r--   0        0        0      289 2023-07-17 11:17:31.722576 mrsal-0.6.0a0/mrsal/config/exceptions.py
+-rw-r--r--   0        0        0     2443 2023-07-18 08:59:41.089318 mrsal-0.6.0a0/mrsal/config/logging.py
+-rw-r--r--   0        0        0    36078 2023-07-18 08:57:30.540133 mrsal-0.6.0a0/mrsal/mrsal.py
+-rw-r--r--   0        0        0      344 2023-07-18 09:00:30.088267 mrsal-0.6.0a0/mrsal/utils/utils.py
+-rw-r--r--   0        0        0      675 2023-07-17 10:51:03.596481 mrsal-0.6.0a0/pyproject.toml
+-rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 mrsal-0.6.0a0/PKG-INFO
```

### Comparing `mrsal-0.5.0a0/LICENSE.txt` & `mrsal-0.6.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mrsal-0.5.0a0/README.md` & `mrsal-0.6.0a0/README.md`

 * *Files identical despite different names*

### Comparing `mrsal-0.5.0a0/mrsal/config/config.py` & `mrsal-0.6.0a0/mrsal/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Tuple, Dict
 import os
+from typing import Dict, Tuple
 
-RABBITMQ_SERVICE_NAME_DOCKER_COMPOSE: str = os.environ.get('RABBITMQ_SERVICE_NAME')  # Service name in docker-compose.yaml
+# Service name in docker-compose.yaml
+RABBITMQ_SERVICE_NAME_DOCKER_COMPOSE: str = os.environ.get('RABBITMQ_SERVICE_NAME')
 RABBITMQ_SERVER: str = 'localhost'
 V_HOST: str = os.environ.get('RABBITMQ_DEFAULT_VHOST', 'myMrsalHost')
 RABBITMQ_PORT: int = os.environ.get('RABBITMQ_PORT', 5672)
 RABBITMQ_PORT_TLS: int = os.environ.get('RABBITMQ_PORT_TLS', 5671)
 RABBIT_DOMAIN: str = os.environ.get('RABBITMQ_DOMAIN', 'localhost')
 
 RABBITMQ_USER = os.environ.get('RABBITMQ_DEFAULT_USER', 'root')
@@ -17,15 +18,16 @@
 RABBITMQ_BIND_ROUTING_KEY: str = 'emergency'
 RABBITMQ_QUEUE: str = 'emergency_queue'
 RABBITMQ_DEAD_LETTER_ROUTING_KEY: str = 'dead_letter'
 RABBITMQ_DEAD_LETTER_QUEUE: str = 'dead_letter-queue'
 
 DELAY_EXCHANGE_TYPE: str = 'x-delayed-message'
 DELAY_EXCHANGE_ARGS: Dict[str, str] = {'x-delayed-type': 'direct'}
-DEAD_LETTER_QUEUE_ARGS: Dict[str, str] = {'x-dead-letter-exchange': '', 'x-dead-letter-routing-key': ''}
+DEAD_LETTER_QUEUE_ARGS: Dict[str, str] = {
+    'x-dead-letter-exchange': '', 'x-dead-letter-routing-key': ''}
 
 CONTENT_TYPE: str = 'text/plain'
 CONTENT_ENCODING: str = 'utf-8'
 
 RETRY_LIMIT_KEY: str = 'x-retry-limit'
 RETRY_KEY: str = 'x-retry'
 MESSAGE_HEADERS_KEY: str = 'headers'
```

### Comparing `mrsal-0.5.0a0/mrsal/config/logging.py` & `mrsal-0.6.0a0/mrsal/config/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 
 # Setting color logs
 SUCCESS = 21
 FAIL = 22
 PIPE = 55
 LOG_LEVEL = logging.INFO
 LOG_LEVEL_E = logging.WARNING
-LOGFORMAT = '%(log_color)s[%(asctime)s] [%(levelname)-8s] %(reset)s | %(log_color)s%(message)s%(reset)s'
-LOGFORMAT_ERROR = '%(log_color)s%(asctime)-8s%(reset)s | %(log_color)s%(levelname)-8s%(reset)s | %(log_color)s%(message)s%(reset)s'
+LOGFORMAT = '%(log_color)s[%(asctime)s] [%(levelname)-8s] %(reset)s | \
+    %(log_color)s%(message)s%(reset)s'
+LOGFORMAT_ERROR = '%(log_color)s%(asctime)-8s%(reset)s | \
+    %(log_color)s%(levelname)-8s%(reset)s | %(log_color)s%(message)s%(reset)s'
 
 ROOT = os.getcwd()  # os.environ['PYTHONPATH']
 
 # Adding file path for error logs and levels above
 FILE_PATH = os.path.join(ROOT, 'docs/logs/level_errors_logs.log')
-Path(FILE_PATH).parent.mkdir(exist_ok=True, parents=True)  # It is sad with non existent parents
+# It is sad with non existent parents
+Path(FILE_PATH).parent.mkdir(exist_ok=True, parents=True)
 
 logging.addLevelName(SUCCESS, 'SUCCESS')
 
 
 def success(self, message, *args, **kws):
     if self.isEnabledFor(SUCCESS):
         self._log(SUCCESS, message, args, **kws)
@@ -81,14 +84,15 @@
 stream.setLevel(LOG_LEVEL)
 # TODO: Only save loglevel error to file
 file_handler.setLevel(LOG_LEVEL)
 
 stream.setFormatter(formatter)
 file_handler.setFormatter(e_formatter)
 
+
 def get_logger(name):
     log = logging.getLogger(name)
     log.setLevel(LOG_LEVEL)
     if (log.hasHandlers()):
         log.handlers.clear()
     log.addHandler(stream)
     log.addHandler(file_handler)
```

### Comparing `mrsal-0.5.0a0/mrsal/mrsal.py` & `mrsal-0.6.0a0/mrsal/mrsal.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,63 +6,75 @@
 from socket import gaierror
 from typing import Any, Callable, Dict, NoReturn, Tuple
 
 import pika
 from pika import SSLOptions
 from pika.exchange_type import ExchangeType
 from retry import retry
-import mrsal.config.config as config
-from mrsal.utils.utils import is_redelivery_configured
 
+import mrsal.config.config as config
 from mrsal.config.logging import get_logger
+from mrsal.utils.utils import is_redelivery_configured
 
 
 @dataclass
 class Mrsal:
     """
     Mrsal creates a layer on top of Pika's core, providing methods to setup a
     RabbitMQ broker with multiple functionalities.
 
     Properties:
         :prop str host: Hostname or IP Address to connect to
         :prop int port: TCP port to connect to
         :prop pika.credentials.Credentials credentials: auth credentials
         :prop str virtual_host: RabbitMQ virtual host to use
         :prop bool verbose: If True then more INFO logs will be printed
-        :prop int heartbeat: Controls RabbitMQ's server heartbeat timeout negotiation during connection tuning.
-        :prop int blocked_connection_timeout: blocked_connection_timeout is the timeout, in seconds,
-            for the connection to remain blocked; if the timeout expires, the connection will be torn down
+        :prop int heartbeat: Controls RabbitMQ's server heartbeat timeout negotiation \
+            during connection tuning.
+        :prop int blocked_connection_timeout: blocked_connection_timeout \
+            is the timeout, in seconds,
+            for the connection to remain blocked; if the timeout expires, \
+                the connection will be torn down
         :prop int prefetch_count: Specifies a prefetch window in terms of whole messages.
-        :prop bool ssl: Set this flag to true if you want to connect externally to the rabbitserver. 
+        :prop bool ssl: Set this flag to true if you want to connect \
+            externally to the rabbitserver.
     """
     host: str
     port: str
     credentials: Tuple[str, str]
     virtual_host: str
     ssl: bool = False
     verbose: bool = False
     prefetch_count: int = 1
     heartbeat: int = 5 * 60 * 60  # 5 hours
     blocked_connection_timeout: int = 300  # sec
     _connection: pika.BlockingConnection = None
     _channel = None
     log = get_logger(__name__)
 
-    @retry((pika.exceptions.AMQPConnectionError, TypeError, gaierror), tries=2, delay=5, jitter=(1, 3))
+    @retry((pika.exceptions.AMQPConnectionError, TypeError,
+           gaierror), tries=2, delay=5, jitter=(1, 3))
     def connect_to_server(self, context: Dict[str, str] = None):
         """ We can use connect_to_server for establishing a connection to
         RabbitMQ server specifying connection parameters.
 
         Parameters
         ----------
         context : Dict[str, str]
             context is the structured map with information regarding the SSL
             options for connecting with rabbitserver via TLS.
         """
-        connection_info = f'host={self.host}, virtual_host={self.virtual_host}, port={self.port}, heartbeat={self.heartbeat}, ssl={self.ssl}'
+        connection_info = f'''
+                            Mrsal connection parameters:
+                            host={self.host},
+                            virtual_host={self.virtual_host},
+                            port={self.port},
+                            heartbeat={self.heartbeat},
+                            ssl={self.ssl}
+                            '''
         if self.verbose:
             self.log.info(f'Establishing connection to RabbitMQ on {connection_info}')
         if self.ssl:
             self.log.info('setting up TLS connection')
             context = self.__ssl_setup()
         ssl_options = SSLOptions(context, self.host) if context else None
         credentials = pika.PlainCredentials(*self.credentials)
@@ -73,81 +85,93 @@
                     port=self.port,
                     ssl_options=ssl_options,
                     virtual_host=self.virtual_host,
                     credentials=credentials,
                     heartbeat=self.heartbeat,
                     blocked_connection_timeout=self.blocked_connection_timeout
                 ))
-            self._channel: pika.adapters.blocking_connection.BlockingChannel = self._connection.channel()
+            self._channel: pika.adapters.blocking_connection.BlockingChannel = \
+                self._connection.channel()
             # Note: prefetch is set to 1 here as an example only.
             # In production you will want to test with different prefetch values
-            # to find which one provides the best performance and usability for your solution
+            # to find which one provides the best performance and usability for your
+            # solution
             self._channel.basic_qos(prefetch_count=self.prefetch_count)
-            self.log.success(f'Connection established with RabbitMQ on {connection_info}')
+            self.log.success(
+                f'Connection established with RabbitMQ on {connection_info}')
             return self._connection
         except TypeError as err:
             self.log.error(f'Caught a type error: {err}')
             raise TypeError
         except pika.exceptions.AMQPConnectionError as err:
             self.log.error(f'Caught a connection error: {err}')
             raise pika.exceptions.AMQPConnectionError
         except gaierror as err:
             self.log.error(f'Caught a socket error: {err}')
             raise gaierror
 
-    def setup_exchange(self, exchange: str, exchange_type: str, arguments: Dict[str, str] = None,
-                       durable=True, passive=False, internal=False, auto_delete=False):
+    def setup_exchange(self, exchange: str, exchange_type: str,
+                       arguments: Dict[str, str] = None, durable=True, passive=False,
+                       internal=False, auto_delete=False):
         """This method creates an exchange if it does not already exist, and if
         the exchange exists, verifies that it is of the correct and expected
         class.
 
         If passive set, the server will reply with Declare-Ok if the exchange
         already exists with the same name, and raise an error if not and if the
         exchange does not already exist, the server MUST raise a channel
         exception with reply code 404 (not found).
 
-        :param str exchange: The exchange name 
+        :param str exchange: The exchange name
         :param str exchange_type: The exchange type to use
         :param bool passive: Perform a declare or just check to see if it exists
         :param bool durable: Survive a reboot of RabbitMQ
         :param bool auto_delete: Remove when no more queues are bound to it
         :param bool internal: Can only be published to by other exchanges
         :param dict arguments: Custom key/value pair arguments for the exchange
         :returns: Method frame from the Exchange.Declare-ok response
         :rtype: `pika.frame.Method` having `method` attribute of type
             `spec.Exchange.DeclareOk`
         """
-        exchange_declare_info = f'exchange={exchange}, exchange_type={exchange_type}, durable={durable}, passive={passive}, internal={internal}, auto_delete={auto_delete}, arguments={arguments}'
+        exchange_declare_info = f'''
+                                exchange={exchange},
+                                exchange_type={exchange_type},
+                                durable={durable},
+                                passive={passive},
+                                internal={internal},
+                                auto_delete={auto_delete},
+                                arguments={arguments}
+                                '''
         if self.verbose:
             self.log.info(f'Declaring exchange with: {exchange_declare_info}')
         try:
-            exchange_declare_result = self._channel.exchange_declare(exchange=exchange,
-                                                                     exchange_type=exchange_type,
-                                                                     arguments=arguments,
-                                                                     durable=durable,
-                                                                     passive=passive,
-                                                                     internal=internal,
-                                                                     auto_delete=auto_delete)
-            self.log.success(f'Exchange is declared successfully: {exchange_declare_info}, result={exchange_declare_result}')
+            exchange_declare_result = self._channel.exchange_declare(
+                exchange=exchange, exchange_type=exchange_type, arguments=arguments,
+                durable=durable, passive=passive, internal=internal,
+                auto_delete=auto_delete)
+            self.log.success(
+                f'Exchange is declared successfully: {exchange_declare_info}, \
+                result={exchange_declare_result}')
             return exchange_declare_result
         except TypeError as err:
             self.log.error(f'Caught a type error: {err}')
             raise TypeError
         except AttributeError as err:
             self.log.error(f'Caught a attribute error: {err}')
             raise AttributeError
         except pika.exceptions.ChannelClosedByBroker as err:
             self.log.error(f'Caught ChannelClosedByBroker error: {err}')
             raise pika.exceptions.ChannelClosedByBroker(404, str(err))
         except pika.exceptions.ConnectionClosedByBroker as err:
             self.log.error(f'Caught ConnectionClosedByBroker error: {err}')
             raise pika.exceptions.ConnectionClosedByBroker(503, str(err))
 
-    def setup_queue(self, queue: str, arguments: Dict[str, str] = None, durable: bool = True,
-                    exclusive: bool = False, auto_delete: bool = False, passive: bool = False):
+    def setup_queue(
+            self, queue: str, arguments: Dict[str, str] = None, durable: bool = True,
+            exclusive: bool = False, auto_delete: bool = False, passive: bool = False):
         """Declare queue, create if needed. This method creates or checks a
         queue. When creating a new queue the client can specify various
         properties that control the durability of the queue and its contents,
         and the level of sharing for the queue.
 
         Use an empty string as the queue name for the broker to auto-generate
         one. Retrieve this auto-generated queue name from the returned
@@ -162,52 +186,73 @@
         :param bool auto_delete: Delete after consumer cancels or disconnects
         :param dict arguments: Custom key/value arguments for the queue
         :returns: Method frame from the Queue.Declare-ok response
         :rtype: `pika.frame.Method` having `method` attribute of type
             `spec.Queue.DeclareOk`
 
         """
-        queue_declare_info = f'queue={queue}, durable={durable}, exclusive={exclusive}, auto_delete={auto_delete}, arguments={arguments}'
+        queue_declare_info = f'''
+                                queue={queue},
+                                durable={durable},
+                                exclusive={exclusive},
+                                auto_delete={auto_delete},
+                                arguments={arguments}
+                                '''
         if self.verbose:
             self.log.info(f'Declaring queue with: {queue_declare_info}')
         try:
             queue_declare_result = self._channel.queue_declare(queue=queue,
                                                                arguments=arguments,
                                                                durable=durable,
                                                                exclusive=exclusive,
                                                                auto_delete=auto_delete,
                                                                passive=passive)
-            self.log.success(f'Queue is declared successfully: {queue_declare_info}, result={queue_declare_result.method}')
+            self.log.success(f'Queue is declared successfully: {queue_declare_info}, \
+                result={queue_declare_result.method}')
             return queue_declare_result
-        except (pika.exceptions.ChannelClosedByBroker, pika.exceptions.ChannelWrongStateError) as err:
+        except (pika.exceptions.ChannelClosedByBroker,
+                pika.exceptions.ChannelWrongStateError) as err:
             self.log.error(f'Caught ChannelClosedByBroker: {err}')
             raise pika.exceptions.ChannelClosedByBroker(404, str(err))
 
-    def setup_queue_binding(self, exchange: str, queue: str, routing_key: str = None, arguments=None):
+    def setup_queue_binding(self, exchange: str, queue: str,
+                            routing_key: str = None, arguments=None):
         """Bind queue to exchange.
 
         :param str queue: The queue to bind to the exchange
         :param str exchange: The source exchange to bind to
         :param str routing_key: The routing key to bind on
         :param dict arguments: Custom key/value pair arguments for the binding
 
         :returns: Method frame from the Queue.Bind-ok response
         :rtype: `pika.frame.Method` having `method` attribute of type
             `spec.Queue.BindOk`
 
         """
         if self.verbose:
-            self.log.info(f'Binding queue to exchange: queue={queue}, exchange={exchange}, routing_key={routing_key}')
+            self.log.info(f'''Binding queue to exchange:
+                                queue={queue},
+                                exchange={exchange},
+                                routing_key={routing_key}
+                            ''')
         try:
             bind_result = self._channel.queue_bind(
-                exchange=exchange, queue=queue, routing_key=routing_key, arguments=arguments)
-            self.log.success(f'The queue is bound to exchange successfully: queue={queue}, exchange={exchange}, routing_key={routing_key}, result={bind_result}')
+                exchange=exchange, queue=queue, routing_key=routing_key,
+                arguments=arguments)
+            self.log.success(f'''The queue is bound to exchange successfully:
+                                queue={queue},
+                                exchange={exchange},
+                                routing_key={routing_key},
+                                result={bind_result}
+                            ''')
             if self.verbose:
-                self.log.info(f'In such setup a message published to the exchange "{exchange}" \
-                            with routing key "{routing_key}" will be routed to queue "{queue}"')
+                self.log.info(f'''In such setup a message published to the \
+                                        exchange "{exchange}"
+                                    with routing key "{routing_key}" \
+                                        will be routed to queue "{queue}"''')
             return bind_result
         except pika.exceptions.ChannelClosedByBroker as err:
             self.log.error(f'Caught ChannelClosedByBroker: {err}')
             raise pika.exceptions.ChannelClosedByBroker(503, str(err))
 
     def __ssl_setup(self) -> Dict[str, str]:
         """__ssl_setup is private method we are using to connect with rabbitserver
@@ -261,191 +306,265 @@
     def queue_exist(self, queue: str):
         queue_result = self.setup_queue(queue=queue, passive=True)
         # message_count1 = result1.method.message_count
         return queue_result
 
     # --------------------------------------------------------------
     # --------------------------------------------------------------
-    # TODO NOT IN USE: Need to reformat it to publish messages to dead letters exchange after exceeding retries limit
-    def consume_messages_with_retries(self, queue: str, callback: Callable, callback_args=None, escape_after=-1,
-                                      dead_letters_exchange: str = None, dead_letters_routing_key: str = None,
-                                      prop: pika.BasicProperties = None, inactivity_timeout=None):
+    # TODO NOT IN USE: Need to reformat it to publish messages to dead letters
+    # exchange after exceeding retries limit
+    def consume_messages_with_retries(
+            self, queue: str, callback: Callable, callback_args=None, escape_after=-1,
+            dead_letters_exchange: str = None, dead_letters_routing_key: str = None,
+            prop: pika.BasicProperties = None, inactivity_timeout=None):
         self.log.info(f'Consuming messages: queue= {queue}')
 
         try:
-            for method_frame, properties, body in self._channel.consume(queue=queue, inactivity_timeout=inactivity_timeout):
+            for method_frame, properties, body in self._channel.consume(
+                    queue=queue, inactivity_timeout=inactivity_timeout):
                 consumer_tags = self._channel.consumer_tags
                 # Let the message be in whatever data type it needs to
                 message = json.loads(body)
                 exchange = method_frame.exchange
                 routing_key = method_frame.routing_key
                 delivery_tag = method_frame.delivery_tag
-                self.log.info(f'consumer_callback info: exchange: {exchange}, routing_key: {routing_key}, delivery_tag: {delivery_tag}, properties: {properties}, consumer_tags: {consumer_tags}')
+                self.log.info(f'''consumer_callback info:
+                                    exchange: {exchange},
+                                    routing_key: {routing_key},
+                                    delivery_tag: {delivery_tag},
+                                    properties: {properties},
+                                    consumer_tags: {consumer_tags}
+                            ''')
                 is_processed = callback(*callback_args, message)
                 self.log.info(f'is_processed= {is_processed}')
                 if is_processed:
                     self._channel.basic_ack(delivery_tag=delivery_tag)
                     # self._channel.basic_nack(delivery_tag=delivery_tag)
                     self.log.info('Message acknowledged')
 
                     if method_frame.delivery_tag == escape_after:
                         self.log.info(
                             f'Break! Max messages to be processed is {escape_after}')
                         break
                 else:
-                    self.log.warning(f'Could not process the message= {message}. Process it as dead letter.')
-                    is_dead_letter_published = self.publish_dead_letter(message=message, delivery_tag=delivery_tag, dead_letters_exchange=dead_letters_exchange,
-                                                                        dead_letters_routing_key=dead_letters_routing_key, prop=prop)
+                    self.log.warning(f'Could not process the message= {message}. \
+                                        Process it as dead letter.')
+                    is_dead_letter_published = self.publish_dead_letter(
+                        message=message, delivery_tag=delivery_tag,
+                        dead_letters_exchange=dead_letters_exchange,
+                        dead_letters_routing_key=dead_letters_routing_key, prop=prop)
                     if is_dead_letter_published:
                         self._channel.basic_ack(delivery_tag)
                 self.log.info('----------------------------------------------------')
         except FileNotFoundError as e:
             self.log.error(f'Connection closed with error: {e}')
             self._channel.stop_consuming()
 
-    def start_consumer(
-            self, queue: str, callback: Callable, callback_args: Tuple[str, Any] = None,
-            exchange: str = None, exchange_type: str = None, routing_key: str = None,
-            inactivity_timeout: int = None, requeue: bool = False, fast_setup: bool = False,
-            callback_with_delivery_info: bool = False, thread_num: int = None
-    ):
+    def start_consumer(self, queue: str, callback: Callable,
+                       callback_args: Tuple[str, Any] = None, exchange: str = None,
+                       exchange_type: str = None, routing_key: str = None,
+                       inactivity_timeout: int = None, requeue: bool = False,
+                       fast_setup: bool = False,
+                       callback_with_delivery_info: bool = False,
+                       thread_num: int = None):
         """
         Setup consumer:
             1- Consumer start consuming the messages from the queue.
-            2- If `inactivity_timeout` is given (in seconds) the consumer will be canceled when the time of inactivity 
+            2- If `inactivity_timeout` is given (in seconds) the consumer \
+                will be canceled when the time of inactivity
                 exceeds inactivity_timeout.
-            3- Send the consumed message to callback method to be processed, and then the message can be either:
-                - Processed, then correctly-acknowledge and deleted from QUEUE or 
-                - Failed to process, negatively-acknowledged and then the message will be rejected and either
-                    - Redelivered if 'x-retry-limit' and 'x-retry' are configured in 'BasicProperties.headers'.
+            3- Send the consumed message to callback method to be processed, \
+                and then the message can be either:
+                - Processed, then correctly-acknowledge and deleted from QUEUE or
+                - Failed to process, negatively-acknowledged and then the message \
+                    will be rejected and either
+                    - Redelivered if 'x-retry-limit' and 'x-retry' are configured \
+                        in 'BasicProperties.headers'.
                     - Requeued if requeue is True
-                    - Sent to dead-letters-exchange if it configured and 
+                    - Sent to dead-letters-exchange if it configured and
                         - requeue is False
                         - requeue is True and requeue attempt fails.
                     - Unless deleted.
 
 
         :param str queue: The queue name to consume
         :param Callable callback: Method where received messages are sent to be processed
         :param Tuple callback_args: Tuple of arguments for callback method
-        :param float inactivity_timeout: 
-            - if a number is given (in seconds), will cause the method to yield (None, None, None) after the
+        :param float inactivity_timeout:
+            - if a number is given (in seconds), will cause the method \
+                to yield (None, None, None) after the
                 given period of inactivity.
-            - If None is given (default), then the method blocks until the next event arrives.
+            - If None is given (default), then the method blocks \
+                until the next event arrives.
         :param bool requeue: If requeue is true, the server will attempt to
                              requeue the message. If requeue is false or the
                              requeue attempt fails the messages are discarded or
                              dead-lettered.
-        :param bool callback_with_delivery_info: Specify whether the callback method needs delivery info.
-                - spec.Basic.Deliver: Captures the fields for delivered message. E.g:(consumer_tag, delivery_tag, redelivered, exchange, routing_key).
-                - spec.BasicProperties: Captures the client message sent to the server. E.g:(CONTENT_TYPE, DELIVERY_MODE, MESSAGE_ID, APP_ID). 
-        :param bool fast_setup: 
-                - when True, the method will create the specified exchange, queue 
-                and bind them together using the routing kye. 
-                - If False, this method will check if the specified exchange and queue 
+        :param bool callback_with_delivery_info: Specify whether the callback method \
+            needs delivery info.
+                - spec.Basic.Deliver: Captures the fields for delivered message. \
+                    E.g:(consumer_tag, delivery_tag, \
+                    redelivered, exchange, routing_key).
+                - spec.BasicProperties: Captures the client message sent to the server. \
+                    E.g:(CONTENT_TYPE, DELIVERY_MODE, MESSAGE_ID, APP_ID).
+        :param bool fast_setup:
+                - when True, the method will create the specified exchange, queue
+                and bind them together using the routing kye.
+                - If False, this method will check if the specified exchange and queue
                 already exist before start consuming.
         """
-        print_thread_index = f"thread={str(thread_num)} -> " if thread_num is not None else ""
-        self.log.info(f'{print_thread_index} Consuming messages queue= {queue}, requeue= {requeue}, inactivity_timeout= {inactivity_timeout}')
+        print_thread_index = f"thread={str(thread_num)} -> " \
+                             if thread_num is not None else ""
+        self.log.info(
+            f'''{print_thread_index} Consuming messages:
+                    queue={queue},
+                    requeue={requeue},
+                    inactivity_timeout={inactivity_timeout}
+                ''')
         if fast_setup:
             # setting up the necessary connections
             self.setup_exchange(exchange=exchange, exchange_type=exchange_type)
             self.setup_queue(queue=queue)
-            self.setup_queue_binding(exchange=exchange, queue=queue, routing_key=routing_key)
+            self.setup_queue_binding(
+                exchange=exchange,
+                queue=queue,
+                routing_key=routing_key)
         else:
             # Check if the necessary resources (exch & queue) are active
             try:
                 if exchange is not None and exchange_type is not None:
                     self.exchange_exist(exchange=exchange, exchange_type=exchange_type)
                 self.queue_exist(queue=queue)
-            except (pika.exceptions.ChannelClosedByBroker, pika.exceptions.ConnectionClosedByBroker) as err:
-                self.log.error(f'{print_thread_index} Failed to check active resources. Cancel consumer. {str(err)}')
+            except (pika.exceptions.ChannelClosedByBroker,
+                    pika.exceptions.ConnectionClosedByBroker) as err:
+                self.log.error(f'{print_thread_index} Failed to check active resources. \
+                    Cancel consumer. {str(err)}')
                 self._channel.cancel()
                 raise pika.exceptions.ChannelClosedByBroker(404, str(err))
         try:
             self.consumer_tag = None
-            method_frame: spec.Basic.Deliver
-            prop: spec.BasicProperties
+            method_frame: pika.spec.Basic.Deliver
+            properties: pika.spec.BasicProperties
             body: Any
-            for method_frame, properties, body in \
-                    self._channel.consume(queue=queue, inactivity_timeout=inactivity_timeout):
+            for method_frame, properties, body in self._channel.consume(
+                    queue=queue, inactivity_timeout=inactivity_timeout):
                 try:
                     if (method_frame, properties, body) != (None, None, None):
                         consumer_tags = self._channel.consumer_tags
                         self.consumer_tag = method_frame.consumer_tag
                         app_id = properties.app_id
                         msg_id = properties.message_id
-                        
                         if self.verbose:
                             self.log.info(
                                 f"""
                                 Consumed message:
-                                method_frame= {method_frame},
-                                redelivered= {method_frame.redelivered},
-                                exchange= {method_frame.exchange},
-                                routing_key= {method_frame.routing_key},
-                                delivery_tag= {method_frame.delivery_tag},
-                                properties= {properties},
-                                consumer_tags= {consumer_tags},
-                                consumer_tag= {self.consumer_tag}
+                                method_frame={method_frame},
+                                redelivered={method_frame.redelivered},
+                                exchange={method_frame.exchange},
+                                routing_key={method_frame.routing_key},
+                                delivery_tag={method_frame.delivery_tag},
+                                properties={properties},
+                                consumer_tags={consumer_tags},
+                                consumer_tag={self.consumer_tag}
                                 """)
                         if callback_with_delivery_info:
-                            is_processed = callback(*callback_args, method_frame, properties, body) if callback_args else callback(method_frame, properties, body)
+                            is_processed = callback(
+                                *callback_args,
+                                method_frame,
+                                properties,
+                                body) if callback_args else callback(
+                                method_frame,
+                                properties,
+                                body)
                         else:
-                            is_processed = callback(*callback_args, body) if callback_args else callback(body)
+                            is_processed = callback(*callback_args, body) \
+                                if callback_args else callback(body)
                         if is_processed:
-                            self._channel.basic_ack(delivery_tag=method_frame.delivery_tag)
-                            self.log.info(f'{print_thread_index} Message coming from the app={app_id} with messageId={msg_id} is acknowledged.')
+                            self._channel.basic_ack(
+                                delivery_tag=method_frame.delivery_tag)
+                            self.log.info(
+                                f'{print_thread_index} Message coming from the \
+                                    app={app_id} with messageId={msg_id} \
+                                    is acknowledged.')
                         else:
-                            self.log.warning(f'{print_thread_index} Could not process the message coming from the app={app_id} with messageId={msg_id}.')
-                            self._channel.basic_nack(delivery_tag=method_frame.delivery_tag, requeue=requeue)
+                            self.log.warning(
+                                f'{print_thread_index} Could not process the message \
+                                    coming from the app={app_id} \
+                                    with messageId={msg_id}.')
+                            self._channel.basic_nack(
+                                delivery_tag=method_frame.delivery_tag, requeue=requeue)
                             self.log.warning(f'{print_thread_index} Message rejected')
-                            
                             if is_redelivery_configured(properties):
                                 msg_headers = properties.headers
                                 x_retry = msg_headers[config.RETRY_KEY]
                                 x_retry_limit = msg_headers[config.RETRY_LIMIT_KEY]
-                                self.log.warning(f'{print_thread_index} Redelivery options are configured in message headers: x-retry={x_retry}, x-retry-limit={x_retry_limit}')
+                                self.log.warning(
+                                    f'{print_thread_index} Redelivery options are \
+                                        configured in message headers: \
+                                            x-retry={x_retry}, \
+                                            x-retry-limit={x_retry_limit}')
                                 if x_retry < x_retry_limit:
-                                    self.log.warning(f'{print_thread_index} Redelivering the message with messageId={msg_id}.')
+                                    self.log.warning(
+                                        f'{print_thread_index} Redelivering the message \
+                                            with messageId={msg_id}.')
                                     msg_headers[config.RETRY_KEY] = x_retry + 1
                                     prop_redeliver = pika.BasicProperties(
                                         app_id=app_id,
                                         message_id=msg_id,
                                         content_type=config.CONTENT_TYPE,
                                         content_encoding=config.CONTENT_ENCODING,
                                         delivery_mode=pika.DeliveryMode.Persistent,
                                         headers=msg_headers)
-                                    self._channel.basic_publish(exchange=method_frame.exchange, routing_key=method_frame.routing_key, body=body, properties=prop_redeliver)
-                                    self.log.warning(f'{print_thread_index} Message with messageId={msg_id} is successfully redelivered.')
+                                    self._channel.basic_publish(
+                                        exchange=method_frame.exchange,
+                                        routing_key=method_frame.routing_key, body=body,
+                                        properties=prop_redeliver)
+                                    self.log.warning(
+                                        f'{print_thread_index} Message with \
+                                            messageId={msg_id} is successfully \
+                                            redelivered.')
                                 else:
-                                    self.log.warning(f'{print_thread_index} Max number of redeliveries ({x_retry_limit}) are reached for messageId={msg_id}.')
-                        self.log.info(f'[*] {print_thread_index} keep listening on {queue}...')
+                                    self.log.warning(f'{print_thread_index} Max number \
+                                        of redeliveries ({x_retry_limit}) are reached \
+                                        for messageId={msg_id}.')
+                        self.log.info(
+                            f'[*] {print_thread_index} keep listening on {queue}...')
                     else:
-                        self.log.warning(f'{print_thread_index} Given period of inactivity {inactivity_timeout} is exceeded. Cancel consumer.')
+                        self.log.warning(
+                            f'{print_thread_index} Given period of inactivity \
+                                {inactivity_timeout} is exceeded. Cancel consumer.')
                         self.stop_consuming(self.consumer_tag)
                         self._channel.cancel()
-                except (pika.exceptions.StreamLostError, pika.exceptions.ConnectionClosedByBroker, ValueError, TypeError):
-                    self.log.error(f'{print_thread_index} I lost the connection with the Mrsal.', exc_info=True)
+                except (pika.exceptions.StreamLostError,
+                        pika.exceptions.ConnectionClosedByBroker,
+                        ValueError, TypeError):
+                    self.log.error(
+                        f'{print_thread_index} I lost the connection with the Mrsal.',
+                        exc_info=True)
                     pass
                 except KeyboardInterrupt:
                     self.log(f'{print_thread_index} Stopping Mrsal consumption.')
                     self.stop_consuming(self.consumer_tag)
                     self.close_connection()
                     break
         except pika.exceptions.ChannelClosed as err2:
-            self.log.error(f'{print_thread_index} ChannelClosed is caught while consuming. Channel is closed by broker. Cancel consumer. {str(err2)}')
+            self.log.error(
+                f'{print_thread_index} ChannelClosed is caught while consuming. \
+                Channel is closed by broker. Cancel consumer. {str(err2)}')
             self._channel.cancel()
 
     # --------------------------------------------------------------
     # --------------------------------------------------------------
-    def _spawn_mrsal_and_start_new_consumer(self, thread_num: int, queue: str, callback: Callable, callback_args: Tuple[str, Any] = None,
-                                            exchange: str = None, exchange_type: str = None, routing_key: str = None,
-                                            inactivity_timeout: int = None, requeue: bool = False, fast_setup: bool = False,
-                                            callback_with_delivery_info: bool = False):
+    def _spawn_mrsal_and_start_new_consumer(
+            self, thread_num: int, queue: str, callback: Callable,
+            callback_args: Tuple[str, Any] = None, exchange: str = None,
+            exchange_type: str = None, routing_key: str = None,
+            inactivity_timeout: int = None,
+            requeue: bool = False, fast_setup: bool = False,
+            callback_with_delivery_info: bool = False):
         try:
             self.log.info(f"thread_num={thread_num} -> Start consumer")
             mrsal_obj = Mrsal(host=self.host,
                               port=self.port,
                               credentials=self.credentials,
                               virtual_host=self.virtual_host,
                               ssl=self.ssl,
@@ -471,90 +590,120 @@
 
             mrsal_obj.stop_consuming(mrsal_obj.consumer_tag)
             mrsal_obj.close_connection()
             self.log.info(f"thread_num={thread_num} -> End consumer")
         except Exception as e:
             self.log.error(f"thread_num={thread_num} -> Failed to consumer: {e}")
 
-    def start_concurrence_consumer(self, total_threads: int, queue: str, callback: Callable, callback_args: Tuple[str, Any] = None,
-                                   exchange: str = None, exchange_type: str = None, routing_key: str = None,
-                                   inactivity_timeout: int = None, requeue: bool = False, fast_setup: bool = False,
-                                   callback_with_delivery_info: bool = False):
-        with concurrent.futures.ThreadPoolExecutor(max_workers=total_threads) as executor:
-            executor.map(self._spawn_mrsal_and_start_new_consumer, range(total_threads), [queue]*total_threads, [callback]*total_threads, [callback_args]*total_threads,
-                         [exchange]*total_threads, [exchange_type]*total_threads, [routing_key]*total_threads,
-                         [inactivity_timeout]*total_threads, [requeue]*total_threads, [fast_setup]*total_threads,
-                         [callback_with_delivery_info]*total_threads)
+    def start_concurrence_consumer(
+            self, total_threads: int, queue: str, callback: Callable,
+            callback_args: Tuple[str, Any] = None, exchange: str = None,
+            exchange_type: str = None, routing_key: str = None,
+            inactivity_timeout: int = None,
+            requeue: bool = False, fast_setup: bool = False,
+            callback_with_delivery_info: bool = False):
+        with concurrent.futures.ThreadPoolExecutor(max_workers=total_threads) \
+                as executor:
+            executor.map(
+                self._spawn_mrsal_and_start_new_consumer,
+                range(total_threads),
+                [queue] * total_threads,
+                [callback] * total_threads,
+                [callback_args] * total_threads,
+                [exchange] * total_threads,
+                [exchange_type] * total_threads,
+                [routing_key] * total_threads,
+                [inactivity_timeout] * total_threads,
+                [requeue] * total_threads,
+                [fast_setup] * total_threads,
+                [callback_with_delivery_info] * total_threads)
 
     @retry((pika.exceptions.UnroutableError), tries=2, delay=5, jitter=(1, 3))
     def publish_message(
-            self, exchange: str, routing_key: str, message: Any, exchange_type: ExchangeType = ExchangeType.direct,
-            queue: str = None, fast_setup: bool = False, prop: pika.BasicProperties = None
-    ):
+            self, exchange: str, routing_key: str, message: Any,
+            exchange_type: ExchangeType = ExchangeType.direct, queue: str = None,
+            fast_setup: bool = False, prop: pika.BasicProperties = None):
         """Publish message to the exchange specifying routing key and properties.
 
         :param str exchange: The exchange to publish to
         :param str routing_key: The routing key to bind on
         :param bytes body: The message body; empty string if no body
         :param pika.spec.BasicProperties properties: message properties
-        :param bool fast_setup: 
-                - when True, will the method create the specified exchange, queue 
-                and bind them together using the routing kye. 
-                - If False, this method will check if the specified exchange and queue 
-                already exist before publishing. 
+        :param bool fast_setup:
+                - when True, will the method create the specified exchange, queue
+                and bind them together using the routing kye.
+                - If False, this method will check if the specified exchange and queue
+                already exist before publishing.
 
         :raises UnroutableError: raised when a message published in
             publisher-acknowledgments mode (see
             `BlockingChannel.confirm_delivery`) is returned via `Basic.Return`
             followed by `Basic.Ack`.
         :raises NackError: raised when a message published in
             publisher-acknowledgements mode is Nack'ed by the broker. See
             `BlockingChannel.confirm_delivery`.
 
         """
         if fast_setup:
             # setting up the necessary connections
             self.setup_exchange(exchange=exchange, exchange_type=exchange_type)
             self.setup_queue(queue=queue)
-            self.setup_queue_binding(exchange=exchange, queue=queue, routing_key=routing_key)
+            self.setup_queue_binding(
+                exchange=exchange,
+                queue=queue,
+                routing_key=routing_key)
         else:
             # Check if the necessary resources (exch & queue) are active
             try:
                 self.exchange_exist(exchange=exchange, exchange_type=exchange_type)
                 if queue is not None:
                     self.queue_exist(queue=queue)
-            except (pika.exceptions.ChannelClosedByBroker, pika.exceptions.ConnectionClosedByBroker) as err:
-                self.log.error(f'Failed to check active resources. Cancel consumer. {str(err)}')
+            except (pika.exceptions.ChannelClosedByBroker,
+                    pika.exceptions.ConnectionClosedByBroker) as err:
+                self.log.error(
+                    f'Failed to check active resources. Cancel consumer. {str(err)}')
                 self._channel.cancel()
                 raise pika.exceptions.ChannelClosedByBroker(404, str(err))
 
         try:
             # Publish the message by serializing it in json dump
             self._channel.basic_publish(exchange=exchange,
                                         routing_key=routing_key,
                                         body=json.dumps(message),
                                         properties=prop)
-            self.log.info(
-                f'Message ({message}) is published to the exchange "{exchange}" with a routing key "{routing_key}"')
+            self.log.info(f'Message ({message}) is published to the exchange \
+                "{exchange}" with a routing key "{routing_key}"')
 
             # The message will be returned if no one is listening
             return True
         except pika.exceptions.UnroutableError as err1:
-            self.log.error(
-                f'Producer could not publish the message ({message}) to the exchange "{exchange}" with a routing key "{routing_key}": {err1}', exc_info=True)
+            self.log.error(f'''Producer could not publish
+                                message:{message}
+                                to the exchange "{exchange}" with a routing key \
+                                "{routing_key}": {err1}
+                            ''', exc_info=True)
             return False
 
-    # TODO NOT IN USE: maybe we will use it in the method consume_messages_with_retries to publish messages to dead letters exchange after retries limit. (remove or use)
-    def publish_dead_letter(self, message: str, delivery_tag: int, dead_letters_exchange: str = None,
-                            dead_letters_routing_key: str = None, prop: pika.BasicProperties = None):
+    # TODO NOT IN USE: maybe we will use it in the method consume_messages_with_retries
+    # to publish messages to dead letters exchange after retries limit. (remove or use)
+    def publish_dead_letter(self, message: str, delivery_tag: int,
+                            dead_letters_exchange: str = None,
+                            dead_letters_routing_key: str = None,
+                            prop: pika.BasicProperties = None):
         if dead_letters_exchange is not None and dead_letters_routing_key is not None:
-            self.log.warning(f'Re-route the message= {message} to the exchange= {dead_letters_exchange} with routing_key= {dead_letters_routing_key}')
+            self.log.warning(f'Re-route the message={message} to the \
+                    exchange={dead_letters_exchange} with \
+                    routing_key= {dead_letters_routing_key}')
             try:
                 self.publish_message(exchange=dead_letters_exchange,
                                      routing_key=dead_letters_routing_key,
                                      message=json.dumps(message),
                                      properties=prop)
-                self.log.info(f'Dead letter was published: message= {message}, exchange= {dead_letters_exchange}, routing_key= {dead_letters_routing_key}')
+                self.log.info(f'''Dead letter was published:
+                                    message={message},
+                                    exchange={dead_letters_exchange},
+                                    routing_key={dead_letters_routing_key}
+                                ''')
                 return True
             except pika.exceptions.UnroutableError:
                 self.log.error('Dead letter was returned')
                 return False
```

### Comparing `mrsal-0.5.0a0/pyproject.toml` & `mrsal-0.6.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
-name = "mrsal"
-version = "0.5.0-alpha"
-description = "Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika."
 authors = ["Raafat <rafatzahran90@gmail.com>", "Jon E Nesvold <jnesvold@pm.me>"]
-maintainers = ["Raafat <rafatzahran90@gmail.com>", "Jon E Nesvold <jnesvold@pm.me>"]
+description = "Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika."
 keywords = ["message broker", "RabbitMQ", "Pika", "Mrsal"]
-readme = "README.md"
 license = ""
+maintainers = ["Raafat <rafatzahran90@gmail.com>", "Jon E Nesvold <jnesvold@pm.me>"]
+name = "mrsal"
+readme = "README.md"
+version = "0.6.0-alpha"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+colorlog = "^6.7.0"
 pika = "^1.3.0"
+python = "^3.10"
 retry = "^0.9.2"
-colorlog = "^6.7.0"
 
-[tool.poetry.dev-dependencies]
-autopep8 = "^1.6.0"
-pytest = "^7.1.2"
-tox = "^3.25.1"
+[tool.poetry.group.dev.dependencies]
+coverage = "^7.2.7"
+pytest = "^7.4.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `mrsal-0.5.0a0/PKG-INFO` & `mrsal-0.6.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: mrsal
-Version: 0.5.0a0
+Version: 0.6.0a0
 Summary: Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika.
 Keywords: message broker,RabbitMQ,Pika,Mrsal
 Author: Raafat
 Author-email: rafatzahran90@gmail.com
 Maintainer: Raafat
 Maintainer-email: rafatzahran90@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: pika (>=1.3.0,<2.0.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Description-Content-Type: text/markdown
```

