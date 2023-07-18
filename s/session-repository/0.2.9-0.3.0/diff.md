# Comparing `tmp/session-repository-0.2.9.tar.gz` & `tmp/session-repository-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.2.9.tar", last modified: Tue Jul 18 08:48:10 2023, max compression
+gzip compressed data, was "session-repository-0.3.0.tar", last modified: Tue Jul 18 09:06:09 2023, max compression
```

## Comparing `session-repository-0.2.9.tar` & `session-repository-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 08:48:10.278839 session-repository-0.2.9/
--rw-rw-rw-   0        0        0      599 2023-07-18 08:48:10.277837 session-repository-0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 08:48:10.239329 session-repository-0.2.9/session_repository/
--rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.2.9/session_repository/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.9/session_repository/enum.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:48:10.274234 session-repository-0.2.9/session_repository/models/
--rw-rw-rw-   0        0        0     7424 2023-07-18 08:46:35.000000 session-repository-0.2.9/session_repository/models/repository.py
--rw-rw-rw-   0        0        0      475 2023-07-18 08:36:28.000000 session-repository-0.2.9/session_repository/models/service.py
--rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.9/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:48:10.264187 session-repository-0.2.9/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 08:48:10.279891 session-repository-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-07-18 08:47:07.000000 session-repository-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:06:09.224960 session-repository-0.3.0/
+-rw-rw-rw-   0        0        0      599 2023-07-18 09:06:09.222284 session-repository-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 09:06:09.155172 session-repository-0.3.0/session_repository/
+-rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.0/session_repository/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.0/session_repository/enum.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:06:09.214361 session-repository-0.3.0/session_repository/models/
+-rw-rw-rw-   0        0        0     7424 2023-07-18 08:46:35.000000 session-repository-0.3.0/session_repository/models/repository.py
+-rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.0/session_repository/models/service.py
+-rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.3.0/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:06:09.199899 session-repository-0.3.0/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-18 09:06:09.000000 session-repository-0.3.0/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-18 09:06:09.000000 session-repository-0.3.0/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 09:06:09.000000 session-repository-0.3.0/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 09:06:09.000000 session-repository-0.3.0/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 09:06:09.000000 session-repository-0.3.0/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 09:06:09.226795 session-repository-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-18 09:05:32.000000 session-repository-0.3.0/setup.py
```

### Comparing `session-repository-0.2.9/PKG-INFO` & `session-repository-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.9
+Version: 0.3.0
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.9.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.9/session_repository/enum.py` & `session-repository-0.3.0/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.9/session_repository/models/repository.py` & `session-repository-0.3.0/session_repository/models/repository.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.9/session_repository/utils.py` & `session-repository-0.3.0/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.9/session_repository.egg-info/PKG-INFO` & `session-repository-0.3.0/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.9
+Version: 0.3.0
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.9.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.0.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.9/setup.py` & `session-repository-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.9"
+version = "0.3.0"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
         "session_repository.models",
```

