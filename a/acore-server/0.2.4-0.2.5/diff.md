# Comparing `tmp/acore_server-0.2.4.tar.gz` & `tmp/acore_server-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server-0.2.4.tar", last modified: Wed Jun 28 16:14:41 2023, max compression
+gzip compressed data, was "acore_server-0.2.5.tar", last modified: Tue Jul 18 14:08:25 2023, max compression
```

## Comparing `acore_server-0.2.4.tar` & `acore_server-0.2.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 16:14:41.046853 acore_server-0.2.4/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-27 04:12:52.000000 acore_server-0.2.4/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-06-27 04:12:52.000000 acore_server-0.2.4/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      320 2023-06-27 04:12:52.000000 acore_server-0.2.4/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4817 2023-06-28 16:14:41.046696 acore_server-0.2.4/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3694 2023-06-27 05:07:58.000000 acore_server-0.2.4/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 16:14:41.044599 acore_server-0.2.4/acore_server/
--rw-r--r--   0 sanhehu    (501) staff       (20)      393 2023-06-27 04:56:34.000000 acore_server-0.2.4/acore_server/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-28 16:12:48.000000 acore_server-0.2.4/acore_server/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-06-27 04:49:35.000000 acore_server-0.2.4/acore_server/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      107 2023-06-27 04:26:27.000000 acore_server-0.2.4/acore_server/constants.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 16:14:41.045360 acore_server-0.2.4/acore_server/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-27 04:12:52.000000 acore_server-0.2.4/acore_server/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17596 2023-06-28 16:14:14.000000 acore_server-0.2.4/acore_server/fleet.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      936 2023-06-27 04:26:42.000000 acore_server-0.2.4/acore_server/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 16:14:41.045885 acore_server-0.2.4/acore_server/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-27 04:12:52.000000 acore_server-0.2.4/acore_server/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-27 04:12:52.000000 acore_server-0.2.4/acore_server/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 16:14:41.046251 acore_server-0.2.4/acore_server/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-27 04:12:52.000000 acore_server-0.2.4/acore_server/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-27 04:12:52.000000 acore_server-0.2.4/acore_server/vendor/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3272 2023-06-26 05:55:10.000000 acore_server-0.2.4/acore_server/wserver_infra_exports.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 16:14:41.045251 acore_server-0.2.4/acore_server.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4817 2023-06-28 16:14:41.000000 acore_server-0.2.4/acore_server.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      722 2023-06-28 16:14:41.000000 acore_server-0.2.4/acore_server.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-28 16:14:41.000000 acore_server-0.2.4/acore_server.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      392 2023-06-28 16:14:41.000000 acore_server-0.2.4/acore_server.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       13 2023-06-28 16:14:41.000000 acore_server-0.2.4/acore_server.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1727 2023-06-28 16:13:17.000000 acore_server-0.2.4/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-27 04:12:52.000000 acore_server-0.2.4/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-27 04:12:52.000000 acore_server-0.2.4/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-27 04:12:52.000000 acore_server-0.2.4/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-27 04:12:52.000000 acore_server-0.2.4/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      253 2023-06-28 16:12:32.000000 acore_server-0.2.4/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-28 16:14:41.046898 acore_server-0.2.4/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7561 2023-06-27 04:12:52.000000 acore_server-0.2.4/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 16:14:41.046407 acore_server-0.2.4/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1016 2023-06-27 14:01:20.000000 acore_server-0.2.4/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-18 14:08:25.367878 acore_server-0.2.5/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-27 04:12:52.000000 acore_server-0.2.5/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1123 2023-06-27 04:12:52.000000 acore_server-0.2.5/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      320 2023-06-27 04:12:52.000000 acore_server-0.2.5/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4817 2023-07-18 14:08:25.367698 acore_server-0.2.5/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3694 2023-06-27 05:07:58.000000 acore_server-0.2.5/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-18 14:08:25.365400 acore_server-0.2.5/acore_server/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      393 2023-06-27 04:56:34.000000 acore_server-0.2.5/acore_server/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-18 14:07:57.000000 acore_server-0.2.5/acore_server/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      145 2023-06-27 04:49:35.000000 acore_server-0.2.5/acore_server/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      107 2023-06-27 04:26:27.000000 acore_server-0.2.5/acore_server/constants.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-18 14:08:25.366236 acore_server-0.2.5/acore_server/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-27 04:12:52.000000 acore_server-0.2.5/acore_server/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17705 2023-07-18 02:50:11.000000 acore_server-0.2.5/acore_server/fleet.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      936 2023-06-27 04:26:42.000000 acore_server-0.2.5/acore_server/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-18 14:08:25.366665 acore_server-0.2.5/acore_server/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-27 04:12:52.000000 acore_server-0.2.5/acore_server/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-27 04:12:52.000000 acore_server-0.2.5/acore_server/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-18 14:08:25.367122 acore_server-0.2.5/acore_server/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-27 04:12:52.000000 acore_server-0.2.5/acore_server/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-27 04:12:52.000000 acore_server-0.2.5/acore_server/vendor/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3272 2023-06-26 05:55:10.000000 acore_server-0.2.5/acore_server/wserver_infra_exports.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-18 14:08:25.366115 acore_server-0.2.5/acore_server.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4817 2023-07-18 14:08:25.000000 acore_server-0.2.5/acore_server.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      722 2023-07-18 14:08:25.000000 acore_server-0.2.5/acore_server.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-18 14:08:25.000000 acore_server-0.2.5/acore_server.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      392 2023-07-18 14:08:25.000000 acore_server-0.2.5/acore_server.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       13 2023-07-18 14:08:25.000000 acore_server-0.2.5/acore_server.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2001 2023-07-18 02:51:39.000000 acore_server-0.2.5/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-27 04:12:52.000000 acore_server-0.2.5/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-27 04:12:52.000000 acore_server-0.2.5/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-27 04:12:52.000000 acore_server-0.2.5/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-27 04:12:52.000000 acore_server-0.2.5/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      253 2023-06-28 16:12:32.000000 acore_server-0.2.5/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-18 14:08:25.367931 acore_server-0.2.5/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7561 2023-06-27 04:12:52.000000 acore_server-0.2.5/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-18 14:08:25.367283 acore_server-0.2.5/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1016 2023-06-27 14:01:20.000000 acore_server-0.2.5/tests/test_api.py
```

### Comparing `acore_server-0.2.4/AUTHORS.rst` & `acore_server-0.2.5/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server-0.2.4/LICENSE.txt` & `acore_server-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server-0.2.4/PKG-INFO` & `acore_server-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server
-Version: 0.2.4
+Version: 0.2.5
 Summary: AzerothCore World of Warcraft Logic Server Data Model.
 Home-page: https://github.com/MacHu-GWU/acore_server-project
-Download-URL: https://pypi.python.org/pypi/acore_server/0.2.4#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server/0.2.5#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server-0.2.4/README.rst` & `acore_server-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server-0.2.4/acore_server/fleet.py` & `acore_server-0.2.5/acore_server/fleet.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,23 +174,25 @@
 
     def run_ec2(
         self,
         bsm: "BotoSesManager",
         stack_exports: "StackExports",
         python_version: str = "3.8",
         acore_soap_app_version: T.Optional[str] = None,
+        acore_db_app_version: T.Optional[str] = None,
         acore_server_bootstrap_version: T.Optional[str] = None,
     ):
         """
         为服务器创建一台新的 EC2. 注意, 一般先创建 RDS, 等 RDS 已经在运行了, 再创建 EC2.
         因为 EC2 有一个 bootstrap 的过程, 这个过程中需要跟数据库通信.
         """
         bootstrap_command = self.build_bootstrap_command(
             python_version=python_version,
             acore_soap_app_version=acore_soap_app_version,
+            acore_db_app_version=acore_db_app_version,
             acore_server_bootstrap_version=acore_server_bootstrap_version,
         )
         user_data_lines = [
             "#!/bin/bash",
             bootstrap_command,
         ]
         return self.metadata.run_ec2(
```

### Comparing `acore_server-0.2.4/acore_server/paths.py` & `acore_server-0.2.5/acore_server/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server-0.2.4/acore_server/vendor/pytest_cov_helper.py` & `acore_server-0.2.5/acore_server/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server-0.2.4/acore_server/wserver_infra_exports.py` & `acore_server-0.2.5/acore_server/wserver_infra_exports.py`

 * *Files identical despite different names*

### Comparing `acore_server-0.2.4/acore_server.egg-info/PKG-INFO` & `acore_server-0.2.5/acore_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server
-Version: 0.2.4
+Version: 0.2.5
 Summary: AzerothCore World of Warcraft Logic Server Data Model.
 Home-page: https://github.com/MacHu-GWU/acore_server-project
-Download-URL: https://pypi.python.org/pypi/acore_server/0.2.4#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server/0.2.5#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server-0.2.4/acore_server.egg-info/SOURCES.txt` & `acore_server-0.2.5/acore_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server-0.2.4/release-history.rst` & `acore_server-0.2.5/release-history.rst`

 * *Files 22% similar despite different names*

```diff
@@ -11,19 +11,32 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.5 (Backlog)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+**Minor Improvements**
+
+- add ``acore_db_app_version`` argument to ``acore_server.fleet.Server.run_ec2`` method.
+
+**Bugfixes**
+
+**Miscellaneous**
+
+
 0.2.4 (2023-06-28)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Miscellaneous**
 
-- Upgrade ``acore_server_config`` dependency from 0.5.2 to 0.6.1.
+- Upgrade ``acore_server_config`` dependency from 0.4.2 to 0.5.1.
 
 
 0.2.3 (2023-06-28)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Miscellaneous**
 
 - Upgrade dependencies.
```

### Comparing `acore_server-0.2.4/requirements-doc.txt` & `acore_server-0.2.5/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server-0.2.4/setup.py` & `acore_server-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server-0.2.4/tests/test_api.py` & `acore_server-0.2.5/tests/test_api.py`

 * *Files identical despite different names*

