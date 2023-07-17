# Comparing `tmp/acore_paths-0.3.1.tar.gz` & `tmp/acore_paths-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_paths-0.3.1.tar", last modified: Wed Jun 28 15:12:43 2023, max compression
+gzip compressed data, was "acore_paths-0.3.2.tar", last modified: Mon Jul 17 22:32:35 2023, max compression
```

## Comparing `acore_paths-0.3.1.tar` & `acore_paths-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 15:12:43.244418 acore_paths-0.3.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 18:34:07.000000 acore_paths-0.3.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1122 2023-06-17 18:34:07.000000 acore_paths-0.3.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      319 2023-06-17 18:34:07.000000 acore_paths-0.3.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4563 2023-06-28 15:12:43.244282 acore_paths-0.3.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3275 2023-06-17 18:56:37.000000 acore_paths-0.3.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 15:12:43.242572 acore_paths-0.3.1/acore_paths/
--rw-r--r--   0 sanhehu    (501) staff       (20)      428 2023-06-17 18:37:18.000000 acore_paths-0.3.1/acore_paths/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-28 15:11:31.000000 acore_paths-0.3.1/acore_paths/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4707 2023-06-28 15:11:01.000000 acore_paths-0.3.1/acore_paths/acore_paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1088 2023-06-28 15:11:09.000000 acore_paths-0.3.1/acore_paths/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 15:12:43.243307 acore_paths-0.3.1/acore_paths/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 18:34:07.000000 acore_paths-0.3.1/acore_paths/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-17 18:34:07.000000 acore_paths-0.3.1/acore_paths/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 15:12:43.243592 acore_paths-0.3.1/acore_paths/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 18:34:07.000000 acore_paths-0.3.1/acore_paths/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 18:34:07.000000 acore_paths-0.3.1/acore_paths/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 15:12:43.243878 acore_paths-0.3.1/acore_paths/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 18:34:07.000000 acore_paths-0.3.1/acore_paths/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 18:34:07.000000 acore_paths-0.3.1/acore_paths/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 15:12:43.243192 acore_paths-0.3.1/acore_paths.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4563 2023-06-28 15:12:43.000000 acore_paths-0.3.1/acore_paths.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      649 2023-06-28 15:12:43.000000 acore_paths-0.3.1/acore_paths.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-28 15:12:43.000000 acore_paths-0.3.1/acore_paths.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      139 2023-06-28 15:12:43.000000 acore_paths-0.3.1/acore_paths.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       12 2023-06-28 15:12:43.000000 acore_paths-0.3.1/acore_paths.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1968 2023-06-28 15:12:04.000000 acore_paths-0.3.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 18:34:07.000000 acore_paths-0.3.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-17 18:34:07.000000 acore_paths-0.3.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 18:34:07.000000 acore_paths-0.3.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-17 18:34:07.000000 acore_paths-0.3.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-06-17 18:34:07.000000 acore_paths-0.3.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-28 15:12:43.244459 acore_paths-0.3.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7707 2023-06-17 18:53:16.000000 acore_paths-0.3.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-28 15:12:43.244100 acore_paths-0.3.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1008 2023-06-28 15:11:22.000000 acore_paths-0.3.1/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 22:32:35.449712 acore_paths-0.3.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 18:34:07.000000 acore_paths-0.3.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1122 2023-06-17 18:34:07.000000 acore_paths-0.3.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      319 2023-06-17 18:34:07.000000 acore_paths-0.3.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4563 2023-07-17 22:32:35.449565 acore_paths-0.3.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3275 2023-06-17 18:56:37.000000 acore_paths-0.3.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 22:32:35.447644 acore_paths-0.3.2/acore_paths/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      428 2023-06-17 18:37:18.000000 acore_paths-0.3.2/acore_paths/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-17 22:31:15.000000 acore_paths-0.3.2/acore_paths/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5002 2023-07-17 22:28:16.000000 acore_paths-0.3.2/acore_paths/acore_paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1088 2023-06-28 15:11:09.000000 acore_paths-0.3.2/acore_paths/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 22:32:35.448376 acore_paths-0.3.2/acore_paths/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 18:34:07.000000 acore_paths-0.3.2/acore_paths/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-17 18:34:07.000000 acore_paths-0.3.2/acore_paths/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 22:32:35.448782 acore_paths-0.3.2/acore_paths/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 18:34:07.000000 acore_paths-0.3.2/acore_paths/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 18:34:07.000000 acore_paths-0.3.2/acore_paths/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 22:32:35.449111 acore_paths-0.3.2/acore_paths/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 18:34:07.000000 acore_paths-0.3.2/acore_paths/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 18:34:07.000000 acore_paths-0.3.2/acore_paths/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 22:32:35.448261 acore_paths-0.3.2/acore_paths.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4563 2023-07-17 22:32:35.000000 acore_paths-0.3.2/acore_paths.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      649 2023-07-17 22:32:35.000000 acore_paths-0.3.2/acore_paths.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-17 22:32:35.000000 acore_paths-0.3.2/acore_paths.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      139 2023-07-17 22:32:35.000000 acore_paths-0.3.2/acore_paths.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       12 2023-07-17 22:32:35.000000 acore_paths-0.3.2/acore_paths.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2171 2023-07-17 22:32:12.000000 acore_paths-0.3.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 18:34:07.000000 acore_paths-0.3.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-17 18:34:07.000000 acore_paths-0.3.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 18:34:07.000000 acore_paths-0.3.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-17 18:34:07.000000 acore_paths-0.3.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-06-17 18:34:07.000000 acore_paths-0.3.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-17 22:32:35.449756 acore_paths-0.3.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7707 2023-06-17 18:53:16.000000 acore_paths-0.3.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-17 22:32:35.449270 acore_paths-0.3.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1008 2023-06-28 15:11:22.000000 acore_paths-0.3.2/tests/test_api.py
```

### Comparing `acore_paths-0.3.1/AUTHORS.rst` & `acore_paths-0.3.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_paths-0.3.1/LICENSE.txt` & `acore_paths-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_paths-0.3.1/PKG-INFO` & `acore_paths-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_paths
-Version: 0.3.1
+Version: 0.3.2
 Summary: Azerothcore World of Warcraft Server File / Folder structure definition.
 Home-page: https://github.com/MacHu-GWU/acore_paths-project
-Download-URL: https://pypi.python.org/pypi/acore_paths/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_paths/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_paths-0.3.1/README.rst` & `acore_paths-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `acore_paths-0.3.1/acore_paths/acore_paths.py` & `acore_paths-0.3.2/acore_paths/acore_paths.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 """
 Todo: doc string here
 """
 
-from pathlib import Path
+from pathlib import PurePosixPath
 
-dir_home = Path("/home/ubuntu")
+dir_home = PurePosixPath("/home/ubuntu")
 
 # ------------------------------------------------------------------------------
 # Azerothcore Server
 # 跟游戏服务器相关的路径
 # ------------------------------------------------------------------------------
 # 用 https://github.com/azerothcore/azerothcore-wotlk 编译好后的游戏服务器的根目录
 # ${HOME}/azeroth-server/
@@ -86,22 +86,23 @@
 # 用于远程运行 GM 命令的执行代理项目的 Git 仓库所在位置
 # https://github.com/MacHu-GWU/acore_soap_app-project
 dir_acore_soap_app_project = dir_git_repos / "acore_soap_app-project"
 
 # GM 命令执行代理的命令行工具所在位置
 path_acore_soap_app_cli = dir_acore_soap_app_project / ".venv" / "bin" / "acsoap"
 
-# 用于远程运行 SQL 的 DB App 项目的 Git 仓库所在位置
+# 用于远程运行 SQL 的 DB App 项目的 Git 仓库所在位置, 请阅读项目文档了解这个项目的作用.
 # https://github.com/MacHu-GWU/acore_db_app-project
 dir_acore_db_app_project = dir_git_repos / "acore_db_app-project"
 
-# DB App 的命令行工具所在位置
+# DB App 的命令行工具所在位置. 这个命令行工具可以在 EC2 上执行被封装后的数据库程序.
+# 同时允许开发者通过 SSM Run Command 功能远程执行.
 path_acore_db_app_cli = dir_acore_db_app_project / ".venv" / "bin" / "acdb"
 
-# 游戏服务器 EC2 的引导任务自动化项目的 Git 仓库所在位置
+# 游戏服务器 EC2 的引导任务自动化项目的 Git 仓库所在位置, 请阅读项目文档了解这个项目的作用.
 # https://github.com/MacHu-GWU/acore_server_bootstrap-project
 dir_acore_server_bootstrap_project = dir_git_repos / "acore_server_bootstrap-project"
 
-# 引导任务自动化的命令行工具所在位置
+# 引导任务自动化的命令行工具所在位置. 这个命令行工具可以在
 path_acore_server_bootstrap_cli = (
     dir_acore_server_bootstrap_project / ".venv" / "bin" / "acorebs"
 )
```

### Comparing `acore_paths-0.3.1/acore_paths/api.py` & `acore_paths-0.3.2/acore_paths/api.py`

 * *Files identical despite different names*

### Comparing `acore_paths-0.3.1/acore_paths/paths.py` & `acore_paths-0.3.2/acore_paths/paths.py`

 * *Files identical despite different names*

### Comparing `acore_paths-0.3.1/acore_paths/vendor/pytest_cov_helper.py` & `acore_paths-0.3.2/acore_paths/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_paths-0.3.1/acore_paths.egg-info/PKG-INFO` & `acore_paths-0.3.2/acore_paths.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-paths
-Version: 0.3.1
+Version: 0.3.2
 Summary: Azerothcore World of Warcraft Server File / Folder structure definition.
 Home-page: https://github.com/MacHu-GWU/acore_paths-project
-Download-URL: https://pypi.python.org/pypi/acore_paths/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_paths/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_paths-0.3.1/acore_paths.egg-info/SOURCES.txt` & `acore_paths-0.3.2/acore_paths.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_paths-0.3.1/release-history.rst` & `acore_paths-0.3.2/release-history.rst`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.2 (2023-07-17)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that every path should be POSIX style path regardless of the code runtime OS
+
+
 0.3.1 (2023-06-28)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add the following paths:
     - ``acore_paths.api.dir_acore_db_app_project``
     - ``acore_paths.api.path_acore_db_app_cli``
```

### Comparing `acore_paths-0.3.1/requirements-doc.txt` & `acore_paths-0.3.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_paths-0.3.1/setup.py` & `acore_paths-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `acore_paths-0.3.1/tests/test_api.py` & `acore_paths-0.3.2/tests/test_api.py`

 * *Files identical despite different names*

