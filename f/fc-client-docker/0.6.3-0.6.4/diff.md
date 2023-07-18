# Comparing `tmp/fc-client-docker-0.6.3.tar.gz` & `tmp/fc-client-docker-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-client-docker-0.6.3.tar", last modified: Tue Jul 18 04:27:05 2023, max compression
+gzip compressed data, was "dist/fc-client-docker-0.6.4.tar", last modified: Tue Jul 18 05:39:56 2023, max compression
```

## Comparing `fc-client-docker-0.6.3.tar` & `fc-client-docker-0.6.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/LICENSE
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      675 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/fc_client_docker/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      331 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/fc_client_docker/__init__.py
--rwxr-xr-x   0 nxa13855  (1001) atg       (1001)      102 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/fc_client_docker/fc_client_docker
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/fc_client_docker.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      675 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/fc_client_docker.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      422 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/fc_client_docker.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/fc_client_docker.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       59 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/fc_client_docker.egg-info/entry_points.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       27 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/fc_client_docker.egg-info/top_level.txt
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/fc_common/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/fc_common/VERSION
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/fc_common/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/fc_common/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/fc_common/etcd.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/fc_common/logger.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/fc_common/version.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-18 04:27:05.000000 fc-client-docker-0.6.3/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-18 04:26:21.000000 fc-client-docker-0.6.3/setup.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      675 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/fc_client_docker/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      331 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/fc_client_docker/__init__.py
+-rwxr-xr-x   0 nxa13855  (1001) atg       (1001)      102 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/fc_client_docker/fc_client_docker
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/fc_client_docker.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      675 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/fc_client_docker.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      422 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/fc_client_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/fc_client_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       59 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/fc_client_docker.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       27 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/fc_client_docker.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/fc_common/version.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-18 05:39:56.000000 fc-client-docker-0.6.4/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-18 05:39:49.000000 fc-client-docker-0.6.4/setup.py
```

### Comparing `fc-client-docker-0.6.3/LICENSE` & `fc-client-docker-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.3/PKG-INFO` & `fc-client-docker-0.6.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client-docker
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

### Comparing `fc-client-docker-0.6.3/README.rst` & `fc-client-docker-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.3/fc_client_docker.egg-info/PKG-INFO` & `fc-client-docker-0.6.4/fc_client_docker.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-client-docker
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

### Comparing `fc-client-docker-0.6.3/fc_common/config.py` & `fc-client-docker-0.6.4/fc_common/config.py`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.3/fc_common/etcd.py` & `fc-client-docker-0.6.4/fc_common/etcd.py`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.3/fc_common/logger.py` & `fc-client-docker-0.6.4/fc_common/logger.py`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.3/fc_common/version.py` & `fc-client-docker-0.6.4/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.3/setup.cfg` & `fc-client-docker-0.6.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-client-docker-0.6.3/setup.py` & `fc-client-docker-0.6.4/setup.py`

 * *Files identical despite different names*

