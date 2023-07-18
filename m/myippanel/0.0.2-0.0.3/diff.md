# Comparing `tmp/myippanel-0.0.2.tar.gz` & `tmp/myippanel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myippanel-0.0.2.tar", last modified: Tue Jul 18 05:21:40 2023, max compression
+gzip compressed data, was "myippanel-0.0.3.tar", last modified: Tue Jul 18 05:40:40 2023, max compression
```

## Comparing `myippanel-0.0.2.tar` & `myippanel-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:21:40.725890 myippanel-0.0.2/
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      286 2023-07-18 05:21:40.725890 myippanel-0.0.2/PKG-INFO
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      388 2023-07-18 05:21:19.000000 myippanel-0.0.2/pyproject.toml
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)       38 2023-07-18 05:21:40.725890 myippanel-0.0.2/setup.cfg
-drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:21:40.725890 myippanel-0.0.2/src/
-drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:21:40.725890 myippanel-0.0.2/src/myippanel/
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      246 2023-07-17 11:15:51.000000 myippanel-0.0.2/src/myippanel/__init__.py
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      648 2023-07-17 11:21:59.000000 myippanel-0.0.2/src/myippanel/errors.py
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     2706 2023-07-17 11:21:59.000000 myippanel-0.0.2/src/myippanel/httpclient.py
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     5458 2023-07-18 05:19:25.000000 myippanel-0.0.2/src/myippanel/ipclient.py
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     2337 2023-07-15 10:34:26.000000 myippanel-0.0.2/src/myippanel/models.py
-drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:21:40.725890 myippanel-0.0.2/src/myippanel.egg-info/
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      286 2023-07-18 05:21:40.000000 myippanel-0.0.2/src/myippanel.egg-info/PKG-INFO
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      290 2023-07-18 05:21:40.000000 myippanel-0.0.2/src/myippanel.egg-info/SOURCES.txt
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)        1 2023-07-18 05:21:40.000000 myippanel-0.0.2/src/myippanel.egg-info/dependency_links.txt
--rw-rw-r--   0 gatorova  (1000) gatorova  (1000)       10 2023-07-18 05:21:40.000000 myippanel-0.0.2/src/myippanel.egg-info/top_level.txt
+drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:40:40.539684 myippanel-0.0.3/
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      286 2023-07-18 05:40:40.539684 myippanel-0.0.3/PKG-INFO
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      388 2023-07-18 05:40:37.000000 myippanel-0.0.3/pyproject.toml
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)       38 2023-07-18 05:40:40.539684 myippanel-0.0.3/setup.cfg
+drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:40:40.539684 myippanel-0.0.3/src/
+drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:40:40.539684 myippanel-0.0.3/src/myippanel/
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      246 2023-07-17 11:15:51.000000 myippanel-0.0.3/src/myippanel/__init__.py
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      648 2023-07-17 11:21:59.000000 myippanel-0.0.3/src/myippanel/errors.py
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     2706 2023-07-17 11:21:59.000000 myippanel-0.0.3/src/myippanel/httpclient.py
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     5458 2023-07-18 05:28:59.000000 myippanel-0.0.3/src/myippanel/ipclient.py
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)     2337 2023-07-15 10:34:26.000000 myippanel-0.0.3/src/myippanel/models.py
+drwxrwxr-x   0 gatorova  (1000) gatorova  (1000)        0 2023-07-18 05:40:40.539684 myippanel-0.0.3/src/myippanel.egg-info/
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      286 2023-07-18 05:40:40.000000 myippanel-0.0.3/src/myippanel.egg-info/PKG-INFO
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)      290 2023-07-18 05:40:40.000000 myippanel-0.0.3/src/myippanel.egg-info/SOURCES.txt
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)        1 2023-07-18 05:40:40.000000 myippanel-0.0.3/src/myippanel.egg-info/dependency_links.txt
+-rw-rw-r--   0 gatorova  (1000) gatorova  (1000)       10 2023-07-18 05:40:40.000000 myippanel-0.0.3/src/myippanel.egg-info/top_level.txt
```

### Comparing `myippanel-0.0.2/src/myippanel/errors.py` & `myippanel-0.0.3/src/myippanel/errors.py`

 * *Files identical despite different names*

### Comparing `myippanel-0.0.2/src/myippanel/httpclient.py` & `myippanel-0.0.3/src/myippanel/httpclient.py`

 * *Files identical despite different names*

### Comparing `myippanel-0.0.2/src/myippanel/ipclient.py` & `myippanel-0.0.3/src/myippanel/ipclient.py`

 * *Files identical despite different names*

### Comparing `myippanel-0.0.2/src/myippanel/models.py` & `myippanel-0.0.3/src/myippanel/models.py`

 * *Files identical despite different names*

