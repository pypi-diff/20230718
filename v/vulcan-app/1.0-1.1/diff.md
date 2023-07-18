# Comparing `tmp/vulcan-app-1.0.tar.gz` & `tmp/vulcan-app-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-app-1.0.tar", last modified: Tue Jul 11 08:28:41 2023, max compression
+gzip compressed data, was "vulcan-app-1.1.tar", last modified: Tue Jul 18 13:53:35 2023, max compression
```

## Comparing `vulcan-app-1.0.tar` & `vulcan-app-1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 08:28:41.440645 vulcan-app-1.0/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-15 10:28:00.000000 vulcan-app-1.0/LICENSE
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-11 08:28:41.440645 vulcan-app-1.0/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       62 2023-02-15 10:28:00.000000 vulcan-app-1.0/README.md
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-07-11 08:28:41.440645 vulcan-app-1.0/setup.cfg
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1157 2023-07-11 08:27:55.000000 vulcan-app-1.0/setup.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 08:28:41.440645 vulcan-app-1.0/vulcan_app/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      475 2023-07-11 08:23:00.000000 vulcan-app-1.0/vulcan_app/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      805 2023-02-23 08:06:39.000000 vulcan-app-1.0/vulcan_app/configuration.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 08:28:41.440645 vulcan-app-1.0/vulcan_app/database/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1520 2023-02-23 13:43:03.000000 vulcan-app-1.0/vulcan_app/database/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      251 2023-02-15 06:39:24.000000 vulcan-app-1.0/vulcan_app/database/mongo.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1257 2023-02-15 06:59:22.000000 vulcan-app-1.0/vulcan_app/database/postgre.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      686 2023-01-09 13:08:56.000000 vulcan-app-1.0/vulcan_app/database/tunnel.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     5693 2023-07-11 08:26:50.000000 vulcan-app-1.0/vulcan_app/security.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2442 2023-02-15 10:40:00.000000 vulcan-app-1.0/vulcan_app/services.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2860 2023-07-04 14:18:15.000000 vulcan-app-1.0/vulcan_app/worklog_processor.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 08:28:41.440645 vulcan-app-1.0/vulcan_app.egg-info/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      446 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/SOURCES.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/dependency_links.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      161 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/requires.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       11 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/top_level.txt
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-18 13:53:35.213420 vulcan-app-1.1/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-15 10:28:00.000000 vulcan-app-1.1/LICENSE
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-18 13:53:35.213420 vulcan-app-1.1/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       62 2023-02-15 10:28:00.000000 vulcan-app-1.1/README.md
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-07-18 13:53:35.213420 vulcan-app-1.1/setup.cfg
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1157 2023-07-18 13:52:59.000000 vulcan-app-1.1/setup.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-18 13:53:35.213420 vulcan-app-1.1/vulcan_app/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      533 2023-07-18 13:53:23.000000 vulcan-app-1.1/vulcan_app/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      805 2023-02-23 08:06:39.000000 vulcan-app-1.1/vulcan_app/configuration.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-18 13:53:35.213420 vulcan-app-1.1/vulcan_app/database/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1520 2023-02-23 13:43:03.000000 vulcan-app-1.1/vulcan_app/database/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      251 2023-02-15 06:39:24.000000 vulcan-app-1.1/vulcan_app/database/mongo.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1257 2023-02-15 06:59:22.000000 vulcan-app-1.1/vulcan_app/database/postgre.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      686 2023-01-09 13:08:56.000000 vulcan-app-1.1/vulcan_app/database/tunnel.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     5693 2023-07-11 08:26:50.000000 vulcan-app-1.1/vulcan_app/security.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2442 2023-02-15 10:40:00.000000 vulcan-app-1.1/vulcan_app/services.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2860 2023-07-04 14:18:15.000000 vulcan-app-1.1/vulcan_app/worklog_processor.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-18 13:53:35.213420 vulcan-app-1.1/vulcan_app.egg-info/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-18 13:53:35.000000 vulcan-app-1.1/vulcan_app.egg-info/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      446 2023-07-18 13:53:35.000000 vulcan-app-1.1/vulcan_app.egg-info/SOURCES.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-07-18 13:53:35.000000 vulcan-app-1.1/vulcan_app.egg-info/dependency_links.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      161 2023-07-18 13:53:35.000000 vulcan-app-1.1/vulcan_app.egg-info/requires.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       11 2023-07-18 13:53:35.000000 vulcan-app-1.1/vulcan_app.egg-info/top_level.txt
```

### Comparing `vulcan-app-1.0/LICENSE` & `vulcan-app-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.0/PKG-INFO` & `vulcan-app-1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-app
-Version: 1.0
+Version: 1.1
 Summary: Vulcan's web application server.
 Home-page: https://github.com/vulcan-coalition/vulcan-app.git
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vulcan-app-1.0/setup.py` & `vulcan-app-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="vulcan-app",
-    version="1.0",
+    version="1.1",
     author="Chatavut Viriyasuthee",
     author_email="chatavut@lab.ai",
     description="Vulcan's web application server.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vulcan-coalition/vulcan-app.git",
     packages=["vulcan_app", "vulcan_app.database"],
```

### Comparing `vulcan-app-1.0/vulcan_app/configuration.py` & `vulcan-app-1.1/vulcan_app/configuration.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.0/vulcan_app/database/__init__.py` & `vulcan-app-1.1/vulcan_app/database/__init__.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.0/vulcan_app/database/postgre.py` & `vulcan-app-1.1/vulcan_app/database/postgre.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.0/vulcan_app/database/tunnel.py` & `vulcan-app-1.1/vulcan_app/database/tunnel.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.0/vulcan_app/security.py` & `vulcan-app-1.1/vulcan_app/security.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.0/vulcan_app/services.py` & `vulcan-app-1.1/vulcan_app/services.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.0/vulcan_app/worklog_processor.py` & `vulcan-app-1.1/vulcan_app/worklog_processor.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-1.0/vulcan_app.egg-info/PKG-INFO` & `vulcan-app-1.1/vulcan_app.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-app
-Version: 1.0
+Version: 1.1
 Summary: Vulcan's web application server.
 Home-page: https://github.com/vulcan-coalition/vulcan-app.git
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

