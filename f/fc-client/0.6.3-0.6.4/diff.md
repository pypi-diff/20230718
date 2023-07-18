# Comparing `tmp/fc-client-0.6.3.tar.gz` & `tmp/fc-client-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-client-0.6.3.tar", last modified: Tue Jul 18 04:27:05 2023, max compression
+gzip compressed data, was "dist/fc-client-0.6.4.tar", last modified: Tue Jul 18 05:39:55 2023, max compression
```

## Comparing `fc-client-0.6.3.tar` & `fc-client-0.6.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-18 04:26:21.000000 fc-client-0.6.3/LICENSE
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 04:27:05.000000 fc-client-0.6.3/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-18 04:26:21.000000 fc-client-0.6.3/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    14179 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_client/client.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      410 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/entry_points.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       92 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/requires.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client.egg-info/top_level.txt
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_client_daemon/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     7064 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_client_daemon/client_daemon.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-0.6.3/fc_common/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/VERSION
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/etcd.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/logger.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-18 04:26:21.000000 fc-client-0.6.3/fc_common/version.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-18 04:27:05.000000 fc-client-0.6.3/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-18 04:26:21.000000 fc-client-0.6.3/setup.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-client-0.6.4/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-18 05:39:49.000000 fc-client-0.6.4/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 05:39:55.000000 fc-client-0.6.4/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-18 05:39:49.000000 fc-client-0.6.4/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_client/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    14179 2023-07-18 05:39:49.000000 fc-client-0.6.4/fc_client/client.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_client.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_client.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      410 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_client.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       92 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_client.egg-info/requires.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_client.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_client_daemon/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     7064 2023-07-18 05:39:49.000000 fc-client-0.6.4/fc_client_daemon/client_daemon.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-client-0.6.4/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-18 05:39:49.000000 fc-client-0.6.4/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-18 05:39:49.000000 fc-client-0.6.4/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-18 05:39:49.000000 fc-client-0.6.4/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-18 05:39:49.000000 fc-client-0.6.4/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-18 05:39:49.000000 fc-client-0.6.4/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-18 05:39:49.000000 fc-client-0.6.4/fc_common/version.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-18 05:39:55.000000 fc-client-0.6.4/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-18 05:39:49.000000 fc-client-0.6.4/setup.py
```

### Comparing `fc-client-0.6.3/LICENSE` & `fc-client-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.3/PKG-INFO` & `fc-client-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.6.3
+Version: 0.6.4
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-client-0.6.3/README.rst` & `fc-client-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.3/fc_client/client.py` & `fc-client-0.6.4/fc_client/client.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.3/fc_client.egg-info/PKG-INFO` & `fc-client-0.6.4/fc_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client
-Version: 0.6.3
+Version: 0.6.4
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-client-0.6.3/fc_client_daemon/client_daemon.py` & `fc-client-0.6.4/fc_client_daemon/client_daemon.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.3/fc_common/config.py` & `fc-client-0.6.4/fc_common/config.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.3/fc_common/etcd.py` & `fc-client-0.6.4/fc_common/etcd.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.3/fc_common/logger.py` & `fc-client-0.6.4/fc_common/logger.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.3/fc_common/version.py` & `fc-client-0.6.4/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.3/setup.cfg` & `fc-client-0.6.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-client-0.6.3/setup.py` & `fc-client-0.6.4/setup.py`

 * *Files identical despite different names*

