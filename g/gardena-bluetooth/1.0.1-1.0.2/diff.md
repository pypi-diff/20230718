# Comparing `tmp/gardena_bluetooth-1.0.1.tar.gz` & `tmp/gardena_bluetooth-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardena_bluetooth-1.0.1.tar", max compression
+gzip compressed data, was "gardena_bluetooth-1.0.2.tar", max compression
```

## Comparing `gardena_bluetooth-1.0.1.tar` & `gardena_bluetooth-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0      704 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/README.rst
--rw-r--r--   0        0        0      497 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/gardena_bluetooth/__init__.py
--rw-r--r--   0        0        0     2234 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/gardena_bluetooth/__main__.py
--rw-r--r--   0        0        0     8013 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/gardena_bluetooth/client.py
--rw-r--r--   0        0        0     4938 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/gardena_bluetooth/const.py
--rw-r--r--   0        0        0      250 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/gardena_bluetooth/exceptions.py
--rw-r--r--   0        0        0     5094 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/gardena_bluetooth/parse.py
--rw-r--r--   0        0        0        0 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/gardena_bluetooth/py.typed
--rw-r--r--   0        0        0      792 2023-07-08 07:41:01.808183 gardena_bluetooth-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 gardena_bluetooth-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      704 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/README.rst
+-rw-r--r--   0        0        0      497 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/gardena_bluetooth/__init__.py
+-rw-r--r--   0        0        0     2234 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/gardena_bluetooth/__main__.py
+-rw-r--r--   0        0        0     8013 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/gardena_bluetooth/client.py
+-rw-r--r--   0        0        0     4938 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/gardena_bluetooth/const.py
+-rw-r--r--   0        0        0      250 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/gardena_bluetooth/exceptions.py
+-rw-r--r--   0        0        0     5099 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/gardena_bluetooth/parse.py
+-rw-r--r--   0        0        0        0 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/gardena_bluetooth/py.typed
+-rw-r--r--   0        0        0      792 2023-07-18 20:29:05.621094 gardena_bluetooth-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 gardena_bluetooth-1.0.2/PKG-INFO
```

### Comparing `gardena_bluetooth-1.0.1/LICENSE.txt` & `gardena_bluetooth-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-1.0.1/README.rst` & `gardena_bluetooth-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-1.0.1/gardena_bluetooth/__main__.py` & `gardena_bluetooth-1.0.2/gardena_bluetooth/__main__.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-1.0.1/gardena_bluetooth/client.py` & `gardena_bluetooth-1.0.2/gardena_bluetooth/client.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-1.0.1/gardena_bluetooth/const.py` & `gardena_bluetooth-1.0.2/gardena_bluetooth/const.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-1.0.1/gardena_bluetooth/parse.py` & `gardena_bluetooth-1.0.2/gardena_bluetooth/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 @dataclass
 class CharacteristicBool(Characteristic[bool]):
     @classmethod
     def decode(cls, data: bytes) -> bool:
         return data[0] != 0
 
     @classmethod
-    def encode(data: bool) -> bytes:
+    def encode(cls, data: bool) -> bytes:
         if data:
             return b"\x01"
         return b"\x00"
 
 
 @dataclass
 class CharacteristicString(Characteristic[str]):
```

### Comparing `gardena_bluetooth-1.0.1/pyproject.toml` & `gardena_bluetooth-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gardena-bluetooth"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 authors = ["Joakim Plate <elupus@ecce.se>"]
 readme = "README.rst"
 packages = [
     {include = "gardena_bluetooth"},
     {include = "gardena_bluetooth/py.typed"},
 ]
```

### Comparing `gardena_bluetooth-1.0.1/PKG-INFO` & `gardena_bluetooth-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gardena-bluetooth
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: Joakim Plate
 Author-email: elupus@ecce.se
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

