# Comparing `tmp/neo-fairy-client-3.5.0.5.tar.gz` & `tmp/neo-fairy-client-3.5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo-fairy-client-3.5.0.5.tar", last modified: Tue Jun 27 09:03:29 2023, max compression
+gzip compressed data, was "neo-fairy-client-3.5.0.7.tar", last modified: Tue Jul 18 08:39:36 2023, max compression
```

## Comparing `neo-fairy-client-3.5.0.5.tar` & `neo-fairy-client-3.5.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:03:29.618564 neo-fairy-client-3.5.0.5/
--rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo-fairy-client-3.5.0.5/LICENSE
--rw-rw-rw-   0        0        0   139301 2023-06-27 09:03:29.617565 neo-fairy-client-3.5.0.5/PKG-INFO
--rw-rw-rw-   0        0        0   138843 2023-06-14 05:42:43.000000 neo-fairy-client-3.5.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 09:03:29.602480 neo-fairy-client-3.5.0.5/neo_fairy_client/
--rw-rw-rw-   0        0        0      109 2022-09-22 08:08:31.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:03:29.607583 neo-fairy-client-3.5.0.5/neo_fairy_client/rpc/
--rw-rw-rw-   0        0        0       74 2022-09-21 02:51:06.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/rpc/__init__.py
--rw-rw-rw-   0        0        0    55740 2023-06-27 08:52:24.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/rpc/fairy_client.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:03:29.612659 neo-fairy-client-3.5.0.5/neo_fairy_client/utils/
--rw-rw-rw-   0        0        0     1379 2022-09-21 06:25:56.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/utils/WitnessRule.py
--rw-rw-rw-   0        0        0      293 2023-04-26 05:30:10.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/utils/__init__.py
--rw-rw-rw-   0        0        0     1588 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/utils/interpreters.py
--rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/utils/misc.py
--rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/utils/timers.py
--rw-rw-rw-   0        0        0     5625 2022-10-10 02:34:50.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:03:29.614660 neo-fairy-client-3.5.0.5/neo_fairy_client/vm/
--rw-rw-rw-   0        0        0       58 2022-09-21 02:49:39.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/vm/__init__.py
--rw-rw-rw-   0        0        0    15030 2022-09-22 08:50:45.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/vm/fairy_engine.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:03:29.616563 neo-fairy-client-3.5.0.5/neo_fairy_client/websocket/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:00:53.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/websocket/__init__.py
--rw-rw-rw-   0        0        0     4694 2023-03-06 02:47:25.000000 neo-fairy-client-3.5.0.5/neo_fairy_client/websocket/fairy_websocket.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:03:29.606581 neo-fairy-client-3.5.0.5/neo_fairy_client.egg-info/
--rw-rw-rw-   0        0        0   139301 2023-06-27 09:03:29.000000 neo-fairy-client-3.5.0.5/neo_fairy_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-06-27 09:03:29.000000 neo-fairy-client-3.5.0.5/neo_fairy_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:03:29.000000 neo-fairy-client-3.5.0.5/neo_fairy_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-27 09:03:29.000000 neo-fairy-client-3.5.0.5/neo_fairy_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-27 09:03:29.000000 neo-fairy-client-3.5.0.5/neo_fairy_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 09:03:29.618564 neo-fairy-client-3.5.0.5/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-06-27 09:01:50.000000 neo-fairy-client-3.5.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.832974 neo-fairy-client-3.5.0.7/
+-rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo-fairy-client-3.5.0.7/LICENSE
+-rw-rw-rw-   0        0        0   139301 2023-07-18 08:39:36.832974 neo-fairy-client-3.5.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0   138843 2023-06-14 05:42:43.000000 neo-fairy-client-3.5.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.789777 neo-fairy-client-3.5.0.7/neo_fairy_client/
+-rw-rw-rw-   0        0        0      109 2022-09-22 08:08:31.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.805259 neo-fairy-client-3.5.0.7/neo_fairy_client/rpc/
+-rw-rw-rw-   0        0        0       74 2022-09-21 02:51:06.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/rpc/__init__.py
+-rw-rw-rw-   0        0        0    55864 2023-07-18 08:27:33.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/rpc/fairy_client.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.819873 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/
+-rw-rw-rw-   0        0        0     1379 2022-09-21 06:25:56.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/WitnessRule.py
+-rw-rw-rw-   0        0        0      293 2023-04-26 05:30:10.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/__init__.py
+-rw-rw-rw-   0        0        0     1588 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/interpreters.py
+-rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/misc.py
+-rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/timers.py
+-rw-rw-rw-   0        0        0     5625 2022-10-10 02:34:50.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.823922 neo-fairy-client-3.5.0.7/neo_fairy_client/vm/
+-rw-rw-rw-   0        0        0       58 2022-09-21 02:49:39.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/vm/__init__.py
+-rw-rw-rw-   0        0        0    15030 2022-09-22 08:50:45.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/vm/fairy_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.829815 neo-fairy-client-3.5.0.7/neo_fairy_client/websocket/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:00:53.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/websocket/__init__.py
+-rw-rw-rw-   0        0        0     4694 2023-03-06 02:47:25.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/websocket/fairy_websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.802220 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/
+-rw-rw-rw-   0        0        0   139301 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 08:39:36.833852 neo-fairy-client-3.5.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-07-18 08:38:53.000000 neo-fairy-client-3.5.0.7/setup.py
```

### Comparing `neo-fairy-client-3.5.0.5/LICENSE` & `neo-fairy-client-3.5.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.5/PKG-INFO` & `neo-fairy-client-3.5.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.5.0.5
+Version: 3.5.0.7
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neo-fairy-client-3.5.0.5/README.md` & `neo-fairy-client-3.5.0.7/README.md`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.5/neo_fairy_client/rpc/fairy_client.py` & `neo-fairy-client-3.5.0.7/neo_fairy_client/rpc/fairy_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         return result
 
     def meta_rpc_method(self, method: str, parameters: List, relay: bool = None, do_not_raise_on_result=False) -> Any:
         post_data = self.request_body_builder(method, parameters)
         self.previous_post_data = post_data
         result = json.loads(self.requests_session.post(self.target_url, post_data, timeout=self.requests_timeout, verify=self.verify_SSL).text)
         if 'error' in result:
-            raise ValueError(f"""{result['error']['message']}\r\n{result['error']['data']}""")
+            raise ValueError(f"""{result['error']['message']}\r\n{result['error']['data']}""" if 'data' in result['error'] else result['error'])
         if type(result['result']) is dict:
             result_result: dict = result['result']
             if gas_consumed := result_result.get('gasconsumed'):
                 self.previous_gas_consumed = int(gas_consumed)
             if gas_consumed := result_result.get('networkfee'):
                 self.previous_network_fee = int(gas_consumed)
             if 'exception' in result_result and result_result['exception'] is not None:
@@ -366,15 +366,15 @@
         if len(stack) > 1:  # typically happens when we invoke a script calling a series of methods
             return [self.parse_single_item(item) for item in stack]
         else:  # if the stack has only 1 item, we simply return the item without a wrapping list
             result: List = stack[0]
             return self.parse_single_item(result)
     
     @classmethod
-    def parse_params(cls, param: Union[str, int, dict, Hash160Str, UInt160, UInt256, bytes]) -> Dict[str, str]:
+    def parse_params(cls, param: Union[str, int, dict, Hash160Str, UInt160, UInt256, bytes, bytearray]) -> Dict[str, str]:
         type_param = type(param)
         if type_param is UInt160:
             return {
                 'type': 'Hash160',
                 'value': str(Hash160Str.from_UInt160(param)),
             }
         elif type_param is Hash160Str:
@@ -408,15 +408,15 @@
                 'value': str(param),
             }
         elif type_param is str:
             return {
                 'type': 'String',
                 'value': param,
             }
-        elif type_param is bytes:
+        elif type_param is bytes or type_param is bytearray:
             # not the best way to judge, but maybe no better method
             try:
                 return {
                     'type': 'String',
                     'value': param.decode(),
                 }
             except UnicodeDecodeError:
@@ -437,15 +437,15 @@
         elif param is None:
             return {
                 'type': 'Any',
             }
         raise ValueError(f'Unable to handle param {param} with type {type_param}')
     
     def invokefunction_of_any_contract(self, scripthash: Hash160Str, operation: str,
-                                       params: List[Union[str, int, dict, Hash160Str, UInt160]] = None,
+                                       params: List[Union[str, int, dict, Hash160Str, UInt160, bytes, bytearray]] = None,
                                        signers: Union[Signer, List[Signer]] = None, relay: bool = None, do_not_raise_on_result=False,
                                        with_print=True, fairy_session: str = None) -> Any:
         fairy_session = fairy_session or self.fairy_session
         params = params or []
         signers = to_list(signers or self.signers)
         if self.with_print and with_print:
             if fairy_session:
@@ -464,15 +464,15 @@
                 'invokefunctionwithsession', [fairy_session, relay or (relay is None and self.function_default_relay)] + parameters, relay=False,
                 do_not_raise_on_result=do_not_raise_on_result)
         else:
             result = self.meta_rpc_method('invokefunction', parameters, relay=relay,
                                           do_not_raise_on_result=do_not_raise_on_result)
         return result
     
-    def invokefunction(self, operation: str, params: List[Union[str, int, Hash160Str, UInt160]] = None,
+    def invokefunction(self, operation: str, params: List[Union[str, int, Hash160Str, UInt160, bytes, bytearray]] = None,
                        signers: Union[Signer, List[Signer]] = None, relay: bool = None, do_not_raise_on_result=False, with_print=True,
                        fairy_session: str = None) -> Any:
         if self.contract_scripthash is None or self.contract_scripthash == Hash160Str.zero():
             raise ValueError(f'Please set client.contract_scripthash before invoking function. Got {self.contract_scripthash}')
         return self.invokefunction_of_any_contract(self.contract_scripthash, operation, params,
                                                    signers=signers, relay=relay or (relay is None and self.function_default_relay),
                                                    do_not_raise_on_result=do_not_raise_on_result,
```

### Comparing `neo-fairy-client-3.5.0.5/neo_fairy_client/utils/WitnessRule.py` & `neo-fairy-client-3.5.0.7/neo_fairy_client/utils/WitnessRule.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.5/neo_fairy_client/utils/interpreters.py` & `neo-fairy-client-3.5.0.7/neo_fairy_client/utils/interpreters.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.5/neo_fairy_client/utils/timers.py` & `neo-fairy-client-3.5.0.7/neo_fairy_client/utils/timers.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.5/neo_fairy_client/utils/types.py` & `neo-fairy-client-3.5.0.7/neo_fairy_client/utils/types.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.5/neo_fairy_client/vm/fairy_engine.py` & `neo-fairy-client-3.5.0.7/neo_fairy_client/vm/fairy_engine.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.5/neo_fairy_client/websocket/fairy_websocket.py` & `neo-fairy-client-3.5.0.7/neo_fairy_client/websocket/fairy_websocket.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.5/neo_fairy_client.egg-info/PKG-INFO` & `neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.5.0.5
+Version: 3.5.0.7
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neo-fairy-client-3.5.0.5/neo_fairy_client.egg-info/SOURCES.txt` & `neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.5/setup.py` & `neo-fairy-client-3.5.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="neo-fairy-client",
-    version="3.5.0.5",
+    version="3.5.0.7",
     author="Hecate2",
     author_email="hecate2@qq.com",
     description="Test & debug your Neo3 smart contracts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Hecate2/neo-fairy-client",
     packages=setuptools.find_packages(),
```

