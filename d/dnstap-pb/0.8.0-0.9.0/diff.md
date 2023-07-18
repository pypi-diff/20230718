# Comparing `tmp/dnstap_pb-0.8.0.tar.gz` & `tmp/dnstap_pb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnstap_pb-0.8.0.tar", last modified: Sat Sep  3 07:37:35 2022, max compression
+gzip compressed data, was "dnstap_pb-0.9.0.tar", last modified: Tue Jul 18 06:32:23 2023, max compression
```

## Comparing `dnstap_pb-0.8.0.tar` & `dnstap_pb-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:37:35.681170 dnstap_pb-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-03 07:37:26.000000 dnstap_pb-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-09-03 07:37:35.681170 dnstap_pb-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2526 2022-09-03 07:37:26.000000 dnstap_pb-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:37:35.681170 dnstap_pb-0.8.0/dnstap_pb/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-03 07:37:26.000000 dnstap_pb-0.8.0/dnstap_pb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-09-03 07:37:26.000000 dnstap_pb-0.8.0/dnstap_pb/dnstap_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:37:35.681170 dnstap_pb-0.8.0/dnstap_pb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-09-03 07:37:35.000000 dnstap_pb-0.8.0/dnstap_pb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-03 07:37:35.000000 dnstap_pb-0.8.0/dnstap_pb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-03 07:37:35.000000 dnstap_pb-0.8.0/dnstap_pb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-03 07:37:35.000000 dnstap_pb-0.8.0/dnstap_pb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-03 07:37:35.000000 dnstap_pb-0.8.0/dnstap_pb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-03 07:37:35.681170 dnstap_pb-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-09-03 07:37:35.000000 dnstap_pb-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:23.741455 dnstap_pb-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 06:32:07.000000 dnstap_pb-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-18 06:32:23.741455 dnstap_pb-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-18 06:32:07.000000 dnstap_pb-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:23.737455 dnstap_pb-0.9.0/dnstap_pb/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 06:32:07.000000 dnstap_pb-0.9.0/dnstap_pb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-18 06:32:07.000000 dnstap_pb-0.9.0/dnstap_pb/dnstap_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:23.741455 dnstap_pb-0.9.0/dnstap_pb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-18 06:32:23.000000 dnstap_pb-0.9.0/dnstap_pb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 06:32:23.000000 dnstap_pb-0.9.0/dnstap_pb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:32:23.000000 dnstap_pb-0.9.0/dnstap_pb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 06:32:23.000000 dnstap_pb-0.9.0/dnstap_pb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 06:32:23.000000 dnstap_pb-0.9.0/dnstap_pb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:32:23.741455 dnstap_pb-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-18 06:32:23.000000 dnstap_pb-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:32:23.741455 dnstap_pb-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-18 06:32:07.000000 dnstap_pb-0.9.0/tests/test_dnstap.py
```

### Comparing `dnstap_pb-0.8.0/LICENSE` & `dnstap_pb-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dnstap_pb-0.8.0/PKG-INFO` & `dnstap_pb-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnstap_pb
-Version: 0.8.0
+Version: 0.9.0
 Summary: Dnstap Protocol Buffers implementation in Python
 Home-page: https://github.com/dmachard/python-dnstap-protobuf
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: dnstap protobuf decoder encoder
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dnstap Protocol Buffers implementation in Python
 
 Dnstap Protocol Buffers implementation in Python, more informations on dnstap http://dnstap.info/.
-This library is based on the following [protocol buffers schema](https://raw.githubusercontent.com/dnstap/dnstap.pb/master/dnstap.proto).
+This library is based on the following [protocol buffers schema](https://raw.githubusercontent.com/dnstap/dnstap.pb/master/dnstap.proto) from github https://github.com/dnstap/dnstap.pb
 
 ## Installation
 
 This module can be installed from [pypi](https://pypi.org/project/dnstap_pb) website
 
 ```python
 pip install dnstap_pb
```

### Comparing `dnstap_pb-0.8.0/README.md` & `dnstap_pb-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Dnstap Protocol Buffers implementation in Python
 
 Dnstap Protocol Buffers implementation in Python, more informations on dnstap http://dnstap.info/.
-This library is based on the following [protocol buffers schema](https://raw.githubusercontent.com/dnstap/dnstap.pb/master/dnstap.proto).
+This library is based on the following [protocol buffers schema](https://raw.githubusercontent.com/dnstap/dnstap.pb/master/dnstap.proto) from github https://github.com/dnstap/dnstap.pb
 
 ## Installation
 
 This module can be installed from [pypi](https://pypi.org/project/dnstap_pb) website
 
 ```python
 pip install dnstap_pb
```

### Comparing `dnstap_pb-0.8.0/dnstap_pb/dnstap_pb2.py` & `dnstap_pb-0.9.0/dnstap_pb/dnstap_pb2.py`

 * *Files identical despite different names*

### Comparing `dnstap_pb-0.8.0/dnstap_pb.egg-info/PKG-INFO` & `dnstap_pb-0.9.0/dnstap_pb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnstap-pb
-Version: 0.8.0
+Version: 0.9.0
 Summary: Dnstap Protocol Buffers implementation in Python
 Home-page: https://github.com/dmachard/python-dnstap-protobuf
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: dnstap protobuf decoder encoder
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dnstap Protocol Buffers implementation in Python
 
 Dnstap Protocol Buffers implementation in Python, more informations on dnstap http://dnstap.info/.
-This library is based on the following [protocol buffers schema](https://raw.githubusercontent.com/dnstap/dnstap.pb/master/dnstap.proto).
+This library is based on the following [protocol buffers schema](https://raw.githubusercontent.com/dnstap/dnstap.pb/master/dnstap.proto) from github https://github.com/dnstap/dnstap.pb
 
 ## Installation
 
 This module can be installed from [pypi](https://pypi.org/project/dnstap_pb) website
 
 ```python
 pip install dnstap_pb
```

### Comparing `dnstap_pb-0.8.0/setup.py` & `dnstap_pb-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
     
 KEYWORDS = ('dnstap protobuf decoder encoder')
 
 setuptools.setup(
     name="dnstap_pb",
-    version="0.8.0",
+    version="0.9.0",
     author="Denis MACHARD",
     author_email="d.machard@gmail.com",
     description="Dnstap Protocol Buffers implementation in Python",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/dmachard/python-dnstap-protobuf",
     packages=['dnstap_pb'],
```

