# Comparing `tmp/seatable-api-2.6.7.tar.gz` & `tmp/seatable-api-2.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatable-api-2.6.7.tar", last modified: Mon Jul 17 08:26:43 2023, max compression
+gzip compressed data, was "seatable-api-2.6.8.tar", last modified: Tue Jul 18 02:30:55 2023, max compression
```

## Comparing `seatable-api-2.6.7.tar` & `seatable-api-2.6.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 skywalker   (501) staff       (20)        0 2023-07-17 08:26:43.036495 seatable-api-2.6.7/
--rw-r--r--   0 skywalker   (501) staff       (20)    11357 2023-03-22 02:01:50.000000 seatable-api-2.6.7/LICENSE
--rw-r--r--   0 skywalker   (501) staff       (20)      656 2023-07-17 08:26:43.036366 seatable-api-2.6.7/PKG-INFO
--rw-r--r--   0 skywalker   (501) staff       (20)      300 2023-03-22 02:01:50.000000 seatable-api-2.6.7/README.md
-drwxr-xr-x   0 skywalker   (501) staff       (20)        0 2023-07-17 08:26:43.034819 seatable-api-2.6.7/seatable_api/
--rw-r--r--   0 skywalker   (501) staff       (20)      171 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/__init__.py
--rw-r--r--   0 skywalker   (501) staff       (20)    11418 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/column.py
--rw-r--r--   0 skywalker   (501) staff       (20)     1135 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/constants.py
--rw-r--r--   0 skywalker   (501) staff       (20)     1322 2023-07-10 10:10:12.000000 seatable-api-2.6.7/seatable_api/context.py
--rw-r--r--   0 skywalker   (501) staff       (20)    29203 2023-07-17 08:23:32.000000 seatable-api-2.6.7/seatable_api/convert_airtable.py
--rw-r--r--   0 skywalker   (501) staff       (20)    13988 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/date_utils.py
--rw-r--r--   0 skywalker   (501) staff       (20)      119 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/exception.py
--rw-r--r--   0 skywalker   (501) staff       (20)    42361 2023-07-10 10:10:12.000000 seatable-api-2.6.7/seatable_api/main.py
--rw-r--r--   0 skywalker   (501) staff       (20)     2876 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/message.py
--rw-r--r--   0 skywalker   (501) staff       (20)     9400 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/query.py
--rw-r--r--   0 skywalker   (501) staff       (20)     2744 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/socket_io.py
--rw-r--r--   0 skywalker   (501) staff       (20)     6424 2023-03-22 02:01:50.000000 seatable-api-2.6.7/seatable_api/utils.py
-drwxr-xr-x   0 skywalker   (501) staff       (20)        0 2023-07-17 08:26:43.035716 seatable-api-2.6.7/seatable_api.egg-info/
--rw-r--r--   0 skywalker   (501) staff       (20)      656 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/PKG-INFO
--rw-r--r--   0 skywalker   (501) staff       (20)      546 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/SOURCES.txt
--rw-r--r--   0 skywalker   (501) staff       (20)        1 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/dependency_links.txt
--rw-r--r--   0 skywalker   (501) staff       (20)       47 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/requires.txt
--rw-r--r--   0 skywalker   (501) staff       (20)       19 2023-07-17 08:26:43.000000 seatable-api-2.6.7/seatable_api.egg-info/top_level.txt
--rw-r--r--   0 skywalker   (501) staff       (20)       38 2023-07-17 08:26:43.036553 seatable-api-2.6.7/setup.cfg
--rw-r--r--   0 skywalker   (501) staff       (20)      723 2023-07-17 08:26:31.000000 seatable-api-2.6.7/setup.py
-drwxr-xr-x   0 skywalker   (501) staff       (20)        0 2023-07-17 08:26:43.035967 seatable-api-2.6.7/tests/
--rw-r--r--   0 skywalker   (501) staff       (20)        0 2023-03-22 02:01:50.000000 seatable-api-2.6.7/tests/__init__.py
--rw-r--r--   0 skywalker   (501) staff       (20)     5261 2023-03-22 02:01:50.000000 seatable-api-2.6.7/tests/dateutils_test.py
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-18 02:30:55.472575 seatable-api-2.6.8/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    11357 2023-01-04 02:34:58.000000 seatable-api-2.6.8/LICENSE
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-07-18 02:30:55.471937 seatable-api-2.6.8/PKG-INFO
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      300 2023-01-04 02:34:58.000000 seatable-api-2.6.8/README.md
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-18 02:30:55.457288 seatable-api-2.6.8/seatable_api/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      171 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/__init__.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    11418 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/column.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     1135 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/constants.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     1338 2023-07-18 02:27:59.000000 seatable-api-2.6.8/seatable_api/context.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    29203 2023-07-18 02:27:59.000000 seatable-api-2.6.8/seatable_api/convert_airtable.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    13988 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/date_utils.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      119 2023-04-03 02:56:24.000000 seatable-api-2.6.8/seatable_api/exception.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)    42361 2023-07-14 06:55:21.000000 seatable-api-2.6.8/seatable_api/main.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     2876 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/message.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     9400 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/query.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     2744 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/socket_io.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     6424 2023-01-04 02:34:58.000000 seatable-api-2.6.8/seatable_api/utils.py
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-18 02:30:55.467387 seatable-api-2.6.8/seatable_api.egg-info/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      656 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/PKG-INFO
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      546 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/SOURCES.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)        1 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/dependency_links.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)       47 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/requires.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)       19 2023-07-18 02:30:55.000000 seatable-api-2.6.8/seatable_api.egg-info/top_level.txt
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)       38 2023-07-18 02:30:55.473270 seatable-api-2.6.8/setup.cfg
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)      723 2023-07-18 02:29:40.000000 seatable-api-2.6.8/setup.py
+drwxr-xr-x   0 chengxiongchao   (501) staff       (20)        0 2023-07-18 02:30:55.469389 seatable-api-2.6.8/tests/
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)        0 2023-06-13 02:45:17.000000 seatable-api-2.6.8/tests/__init__.py
+-rw-r--r--   0 chengxiongchao   (501) staff       (20)     5261 2023-06-13 02:45:20.000000 seatable-api-2.6.8/tests/dateutils_test.py
```

### Comparing `seatable-api-2.6.7/LICENSE` & `seatable-api-2.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/PKG-INFO` & `seatable-api-2.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.7
+Version: 2.6.8
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `seatable-api-2.6.7/seatable_api/column.py` & `seatable-api-2.6.8/seatable_api/column.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/seatable_api/constants.py` & `seatable-api-2.6.8/seatable_api/constants.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/seatable_api/context.py` & `seatable-api-2.6.8/seatable_api/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     @property
     @need_data
     def current_username(self):
         return context_data.get('current_username')
 
     @property
     @need_data
-    def id_in_org(self):
-        return context_data.get('id_in_org')
+    def current_id_in_org(self):
+        return context_data.get('current_id_in_org')
 
     @need_data
     def get_setting_by_key(self, key):
         return context_data.get(key)
 
 
 context = Context()
```

### Comparing `seatable-api-2.6.7/seatable_api/convert_airtable.py` & `seatable-api-2.6.8/seatable_api/convert_airtable.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/seatable_api/date_utils.py` & `seatable-api-2.6.8/seatable_api/date_utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/seatable_api/main.py` & `seatable-api-2.6.8/seatable_api/main.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/seatable_api/message.py` & `seatable-api-2.6.8/seatable_api/message.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/seatable_api/query.py` & `seatable-api-2.6.8/seatable_api/query.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/seatable_api/socket_io.py` & `seatable-api-2.6.8/seatable_api/socket_io.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/seatable_api/utils.py` & `seatable-api-2.6.8/seatable_api/utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/seatable_api.egg-info/PKG-INFO` & `seatable-api-2.6.8/seatable_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.6.7
+Version: 2.6.8
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `seatable-api-2.6.7/seatable_api.egg-info/SOURCES.txt` & `seatable-api-2.6.8/seatable_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatable-api-2.6.7/setup.py` & `seatable-api-2.6.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '2.6.7'
+__version__ = '2.6.8'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='seatable-api',
     version=__version__,
```

### Comparing `seatable-api-2.6.7/tests/dateutils_test.py` & `seatable-api-2.6.8/tests/dateutils_test.py`

 * *Files identical despite different names*

