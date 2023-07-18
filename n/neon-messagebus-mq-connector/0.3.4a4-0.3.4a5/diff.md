# Comparing `tmp/neon-messagebus-mq-connector-0.3.4a4.tar.gz` & `tmp/neon-messagebus-mq-connector-0.3.4a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-messagebus-mq-connector-0.3.4a4.tar", last modified: Tue Jun 27 00:37:15 2023, max compression
+gzip compressed data, was "neon-messagebus-mq-connector-0.3.4a5.tar", last modified: Tue Jul 18 18:29:57 2023, max compression
```

## Comparing `neon-messagebus-mq-connector-0.3.4a4.tar` & `neon-messagebus-mq-connector-0.3.4a5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:37:15.861693 neon-messagebus-mq-connector-0.3.4a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 00:37:10.000000 neon-messagebus-mq-connector-0.3.4a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-27 00:37:15.857692 neon-messagebus-mq-connector-0.3.4a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 00:37:10.000000 neon-messagebus-mq-connector-0.3.4a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:37:15.857692 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-27 00:37:10.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-27 00:37:10.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-27 00:37:10.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-06-27 00:37:10.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-27 00:37:10.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-27 00:37:10.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 00:37:15.857692 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-27 00:37:15.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-27 00:37:15.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 00:37:15.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-27 00:37:15.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-27 00:37:15.000000 neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 00:37:15.861693 neon-messagebus-mq-connector-0.3.4a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-27 00:37:10.000000 neon-messagebus-mq-connector-0.3.4a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:29:57.783431 neon-messagebus-mq-connector-0.3.4a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-18 18:29:52.000000 neon-messagebus-mq-connector-0.3.4a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-18 18:29:57.783431 neon-messagebus-mq-connector-0.3.4a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 18:29:52.000000 neon-messagebus-mq-connector-0.3.4a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:29:57.779431 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 18:29:52.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-18 18:29:52.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-18 18:29:52.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-07-18 18:29:52.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-18 18:29:52.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-18 18:29:52.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:29:57.783431 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-18 18:29:57.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-18 18:29:57.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:29:57.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 18:29:57.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 18:29:57.000000 neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:29:57.783431 neon-messagebus-mq-connector-0.3.4a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-18 18:29:52.000000 neon-messagebus-mq-connector-0.3.4a5/setup.py
```

### Comparing `neon-messagebus-mq-connector-0.3.4a4/LICENSE.md` & `neon-messagebus-mq-connector-0.3.4a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a4/PKG-INFO` & `neon-messagebus-mq-connector-0.3.4a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus-mq-connector
-Version: 0.3.4a4
+Version: 0.3.4a5
 Summary: MQ-Messagebus Connector Module
 Home-page: https://github.com/neongeckocom/neon-messagebus-mq-connector
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/__init__.py` & `neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/__main__.py` & `neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/config.py` & `neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/config.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/controller.py` & `neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/controller.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/enums.py` & `neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/enums.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector/messages.py` & `neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector/messages.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector.egg-info/PKG-INFO` & `neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus-mq-connector
-Version: 0.3.4a4
+Version: 0.3.4a5
 Summary: MQ-Messagebus Connector Module
 Home-page: https://github.com/neongeckocom/neon-messagebus-mq-connector
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-messagebus-mq-connector-0.3.4a4/neon_messagebus_mq_connector.egg-info/SOURCES.txt` & `neon-messagebus-mq-connector-0.3.4a5/neon_messagebus_mq_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a4/setup.py` & `neon-messagebus-mq-connector-0.3.4a5/setup.py`

 * *Files identical despite different names*

