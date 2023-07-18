# Comparing `tmp/tencentcloud-dlc-connector-1.0.3.tar.gz` & `tmp/tencentcloud-dlc-connector-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tencentcloud-dlc-connector-1.0.3.tar", last modified: Mon Feb 27 06:15:41 2023, max compression
+gzip compressed data, was "tencentcloud-dlc-connector-1.0.4.tar", last modified: Tue Jul 18 11:13:59 2023, max compression
```

## Comparing `tencentcloud-dlc-connector-1.0.3.tar` & `tencentcloud-dlc-connector-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-02-27 06:15:41.468328 tencentcloud-dlc-connector-1.0.3/
--rw-r--r--   0 valux      (501) staff       (20)     1488 2023-02-27 06:15:41.468157 tencentcloud-dlc-connector-1.0.3/PKG-INFO
--rw-r--r--   0 valux      (501) staff       (20)      593 2022-11-11 07:21:09.000000 tencentcloud-dlc-connector-1.0.3/README.md
--rw-r--r--   0 valux      (501) staff       (20)      921 2023-02-16 02:46:15.000000 tencentcloud-dlc-connector-1.0.3/README.rst
--rw-r--r--   0 valux      (501) staff       (20)       38 2023-02-27 06:15:41.468379 tencentcloud-dlc-connector-1.0.3/setup.cfg
--rw-r--r--   0 valux      (501) staff       (20)     1627 2022-12-29 03:31:58.000000 tencentcloud-dlc-connector-1.0.3/setup.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-02-27 06:15:41.467004 tencentcloud-dlc-connector-1.0.3/tdlc_connector/
--rw-r--r--   0 valux      (501) staff       (20)     2970 2022-11-16 03:00:17.000000 tencentcloud-dlc-connector-1.0.3/tdlc_connector/__init__.py
--rw-r--r--   0 valux      (501) staff       (20)     8696 2022-12-29 06:21:04.000000 tencentcloud-dlc-connector-1.0.3/tdlc_connector/api.py
--rw-r--r--   0 valux      (501) staff       (20)     3980 2022-12-28 07:33:35.000000 tencentcloud-dlc-connector-1.0.3/tdlc_connector/connections.py
--rw-r--r--   0 valux      (501) staff       (20)     3224 2023-02-16 02:38:37.000000 tencentcloud-dlc-connector-1.0.3/tdlc_connector/constants.py
--rw-r--r--   0 valux      (501) staff       (20)     3840 2023-02-16 07:34:47.000000 tencentcloud-dlc-connector-1.0.3/tdlc_connector/cursors.py
--rw-r--r--   0 valux      (501) staff       (20)      428 2022-11-04 03:21:23.000000 tencentcloud-dlc-connector-1.0.3/tdlc_connector/exceptions.py
--rw-r--r--   0 valux      (501) staff       (20)     5157 2022-12-05 02:29:28.000000 tencentcloud-dlc-connector-1.0.3/tdlc_connector/formats.py
--rw-r--r--   0 valux      (501) staff       (20)     6844 2022-12-29 03:31:58.000000 tencentcloud-dlc-connector-1.0.3/tdlc_connector/results.py
--rw-r--r--   0 valux      (501) staff       (20)       17 2023-02-16 07:39:07.000000 tencentcloud-dlc-connector-1.0.3/tdlc_connector/version.py
-drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-02-27 06:15:41.467940 tencentcloud-dlc-connector-1.0.3/tencentcloud_dlc_connector.egg-info/
--rw-r--r--   0 valux      (501) staff       (20)     1488 2023-02-27 06:15:41.000000 tencentcloud-dlc-connector-1.0.3/tencentcloud_dlc_connector.egg-info/PKG-INFO
--rw-r--r--   0 valux      (501) staff       (20)      518 2023-02-27 06:15:41.000000 tencentcloud-dlc-connector-1.0.3/tencentcloud_dlc_connector.egg-info/SOURCES.txt
--rw-r--r--   0 valux      (501) staff       (20)        1 2023-02-27 06:15:41.000000 tencentcloud-dlc-connector-1.0.3/tencentcloud_dlc_connector.egg-info/dependency_links.txt
--rw-r--r--   0 valux      (501) staff       (20)       42 2023-02-27 06:15:41.000000 tencentcloud-dlc-connector-1.0.3/tencentcloud_dlc_connector.egg-info/requires.txt
--rw-r--r--   0 valux      (501) staff       (20)       15 2023-02-27 06:15:41.000000 tencentcloud-dlc-connector-1.0.3/tencentcloud_dlc_connector.egg-info/top_level.txt
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-18 11:13:59.175625 tencentcloud-dlc-connector-1.0.4/
+-rw-r--r--   0 valux      (501) staff       (20)     1509 2023-07-18 11:13:59.175408 tencentcloud-dlc-connector-1.0.4/PKG-INFO
+-rw-r--r--   0 valux      (501) staff       (20)      593 2022-11-11 07:21:09.000000 tencentcloud-dlc-connector-1.0.4/README.md
+-rw-r--r--   0 valux      (501) staff       (20)      921 2023-02-16 02:46:15.000000 tencentcloud-dlc-connector-1.0.4/README.rst
+-rw-r--r--   0 valux      (501) staff       (20)       38 2023-07-18 11:13:59.175692 tencentcloud-dlc-connector-1.0.4/setup.cfg
+-rw-r--r--   0 valux      (501) staff       (20)     1627 2023-07-18 09:52:03.000000 tencentcloud-dlc-connector-1.0.4/setup.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-18 11:13:59.173959 tencentcloud-dlc-connector-1.0.4/tdlc_connector/
+-rw-r--r--   0 valux      (501) staff       (20)     2970 2022-11-16 03:00:17.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/__init__.py
+-rw-r--r--   0 valux      (501) staff       (20)     8696 2022-12-29 06:21:04.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/api.py
+-rw-r--r--   0 valux      (501) staff       (20)     3980 2022-12-28 07:33:35.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/connections.py
+-rw-r--r--   0 valux      (501) staff       (20)     3224 2023-02-16 02:38:37.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/constants.py
+-rw-r--r--   0 valux      (501) staff       (20)     3840 2023-07-18 09:42:25.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/cursors.py
+-rw-r--r--   0 valux      (501) staff       (20)      428 2022-11-04 03:21:23.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/exceptions.py
+-rw-r--r--   0 valux      (501) staff       (20)     5157 2022-12-05 02:29:28.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/formats.py
+-rw-r--r--   0 valux      (501) staff       (20)     6901 2023-07-18 09:43:19.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/results.py
+-rw-r--r--   0 valux      (501) staff       (20)       17 2023-07-18 09:43:59.000000 tencentcloud-dlc-connector-1.0.4/tdlc_connector/version.py
+drwxr-xr-x   0 valux      (501) staff       (20)        0 2023-07-18 11:13:59.175111 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/
+-rw-r--r--   0 valux      (501) staff       (20)     1509 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/PKG-INFO
+-rw-r--r--   0 valux      (501) staff       (20)      518 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 valux      (501) staff       (20)        1 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 valux      (501) staff       (20)       42 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/requires.txt
+-rw-r--r--   0 valux      (501) staff       (20)       15 2023-07-18 11:13:59.000000 tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/top_level.txt
```

### Comparing `tencentcloud-dlc-connector-1.0.3/PKG-INFO` & `tencentcloud-dlc-connector-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: tencentcloud-dlc-connector
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tencentcloud DLC connector, connect to DLC engines using SQL.
+Home-page: UNKNOWN
 Author: Tencentcloud DLC Team.
 Maintainer-email: valuxzhao@tencent.com
 License: Apache License Version 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -52,7 +53,9 @@
     count = cursor.execute("SELECT 1")
     cursor.fetchone()
 
 
 
 
 
+
+
```

### Comparing `tencentcloud-dlc-connector-1.0.3/README.md` & `tencentcloud-dlc-connector-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.3/README.rst` & `tencentcloud-dlc-connector-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.3/setup.py` & `tencentcloud-dlc-connector-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.3/tdlc_connector/__init__.py` & `tencentcloud-dlc-connector-1.0.4/tdlc_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.3/tdlc_connector/api.py` & `tencentcloud-dlc-connector-1.0.4/tdlc_connector/api.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.3/tdlc_connector/connections.py` & `tencentcloud-dlc-connector-1.0.4/tdlc_connector/connections.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.3/tdlc_connector/constants.py` & `tencentcloud-dlc-connector-1.0.4/tdlc_connector/constants.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.3/tdlc_connector/cursors.py` & `tencentcloud-dlc-connector-1.0.4/tdlc_connector/cursors.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.3/tdlc_connector/formats.py` & `tencentcloud-dlc-connector-1.0.4/tdlc_connector/formats.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-connector-1.0.3/tdlc_connector/results.py` & `tencentcloud-dlc-connector-1.0.4/tdlc_connector/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,20 +165,22 @@
     def _iter_rows(self):
 
         prefix = os.path.join(self._key, constants.CosKey.RESULT_DATA)
         for item in self._client.iter_cos_objects(self._bucket, prefix):
             name = tempfile.mktemp(prefix=f"RESULT-{self._statement_id}")
             self._client.get_cos_object_stream_to_file(self._bucket, item['Key'], name)
 
-            reader = csv.reader(open(name), escapechar='\\')
+            f = open(name, encoding='utf8')
+            reader = csv.reader(f, escapechar='\\')
             next(reader) # skip header
 
             for line in reader:
                 yield line
 
+            f.close()
             os.remove(name)
 
 
 class COSResultGenerator(LasyCOSResultGenerator):
 
     def _iter_rows(self):
```

### Comparing `tencentcloud-dlc-connector-1.0.3/tencentcloud_dlc_connector.egg-info/PKG-INFO` & `tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: tencentcloud-dlc-connector
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tencentcloud DLC connector, connect to DLC engines using SQL.
+Home-page: UNKNOWN
 Author: Tencentcloud DLC Team.
 Maintainer-email: valuxzhao@tencent.com
 License: Apache License Version 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -52,7 +53,9 @@
     count = cursor.execute("SELECT 1")
     cursor.fetchone()
 
 
 
 
 
+
+
```

### Comparing `tencentcloud-dlc-connector-1.0.3/tencentcloud_dlc_connector.egg-info/SOURCES.txt` & `tencentcloud-dlc-connector-1.0.4/tencentcloud_dlc_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

