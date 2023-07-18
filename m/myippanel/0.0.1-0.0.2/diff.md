# Comparing `tmp/myippanel-0.0.1.tar.gz` & `tmp/myippanel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myippanel-0.0.1.tar", last modified: Mon Jul 17 11:22:35 2023, max compression
+gzip compressed data, was "myippanel-0.0.2.tar", last modified: Tue Jul 18 05:21:40 2023, max compression
```

## Comparing `myippanel-0.0.1.tar` & `myippanel-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-17 11:22:35.629782 myippanel-0.0.1/
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      286 2023-07-17 11:22:35.629782 myippanel-0.0.1/PKG-INFO
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      388 2023-07-17 11:20:05.000000 myippanel-0.0.1/pyproject.toml
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)       38 2023-07-17 11:22:35.629782 myippanel-0.0.1/setup.cfg
-drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-17 11:22:35.629782 myippanel-0.0.1/src/
-drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-17 11:22:35.629782 myippanel-0.0.1/src/myippanel/
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      246 2023-07-17 11:15:51.000000 myippanel-0.0.1/src/myippanel/__init__.py
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      648 2023-07-17 11:21:59.000000 myippanel-0.0.1/src/myippanel/errors.py
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     2706 2023-07-17 11:21:59.000000 myippanel-0.0.1/src/myippanel/httpclient.py
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     5360 2023-07-17 11:21:59.000000 myippanel-0.0.1/src/myippanel/ipclient.py
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     2337 2023-07-15 10:34:26.000000 myippanel-0.0.1/src/myippanel/models.py
-drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-17 11:22:35.629782 myippanel-0.0.1/src/myippanel.egg-info/
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      286 2023-07-17 11:22:35.000000 myippanel-0.0.1/src/myippanel.egg-info/PKG-INFO
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      290 2023-07-17 11:22:35.000000 myippanel-0.0.1/src/myippanel.egg-info/SOURCES.txt
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)        1 2023-07-17 11:22:35.000000 myippanel-0.0.1/src/myippanel.egg-info/dependency_links.txt
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)       10 2023-07-17 11:22:35.000000 myippanel-0.0.1/src/myippanel.egg-info/top_level.txt
+drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:21:40.725890 myippanel-0.0.2/
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      286 2023-07-18 05:21:40.725890 myippanel-0.0.2/PKG-INFO
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      388 2023-07-18 05:21:19.000000 myippanel-0.0.2/pyproject.toml
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)       38 2023-07-18 05:21:40.725890 myippanel-0.0.2/setup.cfg
+drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:21:40.725890 myippanel-0.0.2/src/
+drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:21:40.725890 myippanel-0.0.2/src/myippanel/
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      246 2023-07-17 11:15:51.000000 myippanel-0.0.2/src/myippanel/__init__.py
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      648 2023-07-17 11:21:59.000000 myippanel-0.0.2/src/myippanel/errors.py
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     2706 2023-07-17 11:21:59.000000 myippanel-0.0.2/src/myippanel/httpclient.py
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     5458 2023-07-18 05:19:25.000000 myippanel-0.0.2/src/myippanel/ipclient.py
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     2337 2023-07-15 10:34:26.000000 myippanel-0.0.2/src/myippanel/models.py
+drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:21:40.725890 myippanel-0.0.2/src/myippanel.egg-info/
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      286 2023-07-18 05:21:40.000000 myippanel-0.0.2/src/myippanel.egg-info/PKG-INFO
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      290 2023-07-18 05:21:40.000000 myippanel-0.0.2/src/myippanel.egg-info/SOURCES.txt
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)        1 2023-07-18 05:21:40.000000 myippanel-0.0.2/src/myippanel.egg-info/dependency_links.txt
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)       10 2023-07-18 05:21:40.000000 myippanel-0.0.2/src/myippanel.egg-info/top_level.txt
```

### Comparing `myippanel-0.0.1/src/myippanel/errors.py` & `myippanel-0.0.2/src/myippanel/errors.py`

 * *Files identical despite different names*

### Comparing `myippanel-0.0.1/src/myippanel/httpclient.py` & `myippanel-0.0.2/src/myippanel/httpclient.py`

 * *Files identical despite different names*

### Comparing `myippanel-0.0.1/src/myippanel/ipclient.py` & `myippanel-0.0.2/src/myippanel/ipclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         :rtype: models.Message
         """
         res = self.client.get("sms/message/all", {
             'message_id': message_id,
         })
 
         try:
-            return Message(res.data[0])
+            return Message(next(item for item in res.data if item['message_id'] == message_id))
+            # return Message(res.data[0])
         except:
             raise ValueError("returned response not valid")
 
     def fetch_statuses(self, message_id, page=0, limit=10):
         r"""Fetch message recipients status
 
         :param message_id: message id, int.
```

### Comparing `myippanel-0.0.1/src/myippanel/models.py` & `myippanel-0.0.2/src/myippanel/models.py`

 * *Files identical despite different names*

