# Comparing `tmp/memphis-py-1.0.5.tar.gz` & `tmp/memphis-py-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/memphis-py-1.0.5.tar", last modified: Mon Jul 10 06:46:13 2023, max compression
+gzip compressed data, was "dist/memphis-py-1.0.6.tar", last modified: Tue Jul 18 08:44:39 2023, max compression
```

## Comparing `memphis-py-1.0.5.tar` & `memphis-py-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-10 06:46:13.000000 memphis-py-1.0.5/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16847 2023-07-10 06:46:13.000000 memphis-py-1.0.5/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12843 2023-07-10 06:46:06.000000 memphis-py-1.0.5/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-10 06:46:13.000000 memphis-py-1.0.5/memphis/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9588 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/consumer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/exceptions.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/headers.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    34977 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/memphis.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/message.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13667 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/producer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/station.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/types.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-07-10 06:46:06.000000 memphis-py-1.0.5/memphis/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-10 06:46:13.000000 memphis-py-1.0.5/memphis_py.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16847 2023-07-10 06:46:13.000000 memphis-py-1.0.5/memphis_py.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      404 2023-07-10 06:46:13.000000 memphis-py-1.0.5/memphis_py.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-10 06:46:13.000000 memphis-py-1.0.5/memphis_py.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-07-10 06:46:13.000000 memphis-py-1.0.5/memphis_py.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-07-10 06:46:13.000000 memphis-py-1.0.5/memphis_py.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-07-10 06:46:06.000000 memphis-py-1.0.5/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-07-10 06:46:13.000000 memphis-py-1.0.5/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1326 2023-07-10 06:46:12.000000 memphis-py-1.0.5/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 08:44:39.000000 memphis-py-1.0.6/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16847 2023-07-18 08:44:39.000000 memphis-py-1.0.6/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12843 2023-07-18 08:44:32.000000 memphis-py-1.0.6/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 08:44:39.000000 memphis-py-1.0.6/memphis/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11224 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/consumer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/exceptions.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/headers.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    34977 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/memphis.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/message.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13678 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/producer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/station.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/types.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-07-18 08:44:32.000000 memphis-py-1.0.6/memphis/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 08:44:39.000000 memphis-py-1.0.6/memphis_py.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16847 2023-07-18 08:44:39.000000 memphis-py-1.0.6/memphis_py.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      404 2023-07-18 08:44:39.000000 memphis-py-1.0.6/memphis_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-18 08:44:39.000000 memphis-py-1.0.6/memphis_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-07-18 08:44:39.000000 memphis-py-1.0.6/memphis_py.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-07-18 08:44:39.000000 memphis-py-1.0.6/memphis_py.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-07-18 08:44:32.000000 memphis-py-1.0.6/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-07-18 08:44:39.000000 memphis-py-1.0.6/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1326 2023-07-18 08:44:39.000000 memphis-py-1.0.6/setup.py
```

### Comparing `memphis-py-1.0.5/PKG-INFO` & `memphis-py-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py
-Version: 1.0.5
+Version: 1.0.6
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.5.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.6.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
```

### Comparing `memphis-py-1.0.5/README.md` & `memphis-py-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.5/memphis/__init__.py` & `memphis-py-1.0.6/memphis/__init__.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.5/memphis/consumer.py` & `memphis-py-1.0.6/memphis/consumer.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,48 @@
         self.t_consume = None
 
     def set_context(self, context):
         """Set a context (dict) that will be passed to each message handler call."""
         self.context = context
 
     def consume(self, callback):
-        """Consume events."""
+        """
+        This method starts consuming events from the specified station and invokes the provided callback function for each batch of messages received.
+
+        Parameters:
+            callback (function): A function that will be called with each batch of messages received. The function should have the following signature:
+                - `callback(messages: List[Message], error: Optional[MemphisError], context: Dict) -> Awaitable[None]`
+                - `messages`: A list of `Message` objects representing the batch of messages received.
+                - `error`: An optional `MemphisError` object if there was an error while consuming the messages.
+                - `context`: A dictionary representing the context that was set using the `set_context()` method.
+
+        Example:
+            import asyncio
+            from memphis import Memphis
+
+            async def message_handler(messages, error, context):
+                if error:
+                    print(f"Error occurred: {error}")
+                    return
+
+                for message in messages:
+                    print(f"Received message: {message}")
+
+            async def main():
+                memphis = Memphis()
+                await memphis.connect(host='localhost', username='user', password='pass')
+                consumer = await memphis.consumer(station_name='my_station', consumer_name='my_consumer', consumer_group='my_group')
+                consumer.set_context({'key': 'value'})
+                consumer.consume(message_handler)
+
+                # Keep the event loop running
+                while True:
+                    await asyncio.sleep(1)
+            asyncio.run(main())
+        """
         self.dls_callback_func = callback
         self.t_consume = asyncio.create_task(self.__consume(callback))
 
     async def __consume(self, callback):
         subject = get_internal_name(self.station_name)
         consumer_group = get_internal_name(self.consumer_group)
         self.psub = await self.connection.broker_connection.pull_subscribe(
@@ -125,15 +158,15 @@
 
         Example:
 
             import asyncio
             
             from memphis import Memphis
 
-            async def main(/, host, username, password, station):
+            async def main(host, username, password, station):
                 memphis = Memphis()
                 await memphis.connect(host=host,
                                       username=username,
                                       password=password)
             
                 consumer = await memphis.consumer(station_name=station,
                                                   consumer_name="test-consumer",
@@ -145,18 +178,18 @@
                     for msg in batch:
                         serialized_record = msg.get_data()
                         print("Message:", serialized_record)
             
                 await memphis.close()
 
             if __name__ == '__main__':
-                asyncio.run(main(host=host,
-                                 username=username,
-                                 password=password,
-                                 station=station))
+                asyncio.run(main(host,
+                                 username,
+                                 password,
+                                 station))
         
         """
         messages = []
         if self.connection.is_connection_active:
             try:
                 if batch_size > self.MAX_BATCH_SIZE:
                     raise MemphisError(
```

### Comparing `memphis-py-1.0.5/memphis/exceptions.py` & `memphis-py-1.0.6/memphis/exceptions.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.5/memphis/headers.py` & `memphis-py-1.0.6/memphis/headers.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.5/memphis/memphis.py` & `memphis-py-1.0.6/memphis/memphis.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.5/memphis/message.py` & `memphis-py-1.0.6/memphis/message.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.5/memphis/producer.py` & `memphis-py-1.0.6/memphis/producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,21 +261,20 @@
                         + self.producer_name
                         + "\nError:"
                         + str(e),
                         msg_to_send,
                         schemaverse_fail_alert_type,
                     )
             raise e
-        except Exception as e:
+        except Exception as e: # pylint: disable-next=no-member
             if hasattr(e, "status_code") and e.status_code == "503":
                 raise MemphisError(
                     "Produce operation has failed, please check whether Station/Producer still exist"
                 )
-            else:
-                raise MemphisError(str(e)) from e
+            raise MemphisError(str(e)) from e
 
     async def destroy(self):
         """Destroy the producer."""
         try:
             destroy_producer_req = {
                 "name": self.producer_name,
                 "station_name": self.station_name,
```

### Comparing `memphis-py-1.0.5/memphis/station.py` & `memphis-py-1.0.6/memphis/station.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.5/memphis/types.py` & `memphis-py-1.0.6/memphis/types.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.5/memphis/utils.py` & `memphis-py-1.0.6/memphis/utils.py`

 * *Files identical despite different names*

### Comparing `memphis-py-1.0.5/memphis_py.egg-info/PKG-INFO` & `memphis-py-1.0.6/memphis_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py
-Version: 1.0.5
+Version: 1.0.6
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.5.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.6.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
```

### Comparing `memphis-py-1.0.5/setup.py` & `memphis-py-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="memphis-py",
     packages=["memphis"],
-    version="1.0.5",
+    version="1.0.6",
     license="Apache-2.0",
     description="A powerful messaging platform for modern developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Memphis.dev",
     author_email="team@memphis.dev",
     url="https://github.com/memphisdev/memphis.py",
-    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.5.tar.gz",
+    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.6.tar.gz",
     keywords=["message broker", "devtool", "streaming", "data"],
     install_requires=["asyncio", "nats-py", "protobuf", "jsonschema", "graphql-core"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "License :: OSI Approved :: GNU General Public License (GPL)",
```

