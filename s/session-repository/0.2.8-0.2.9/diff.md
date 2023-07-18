# Comparing `tmp/session-repository-0.2.8.tar.gz` & `tmp/session-repository-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.2.8.tar", last modified: Tue Jul 18 08:40:36 2023, max compression
+gzip compressed data, was "session-repository-0.2.9.tar", last modified: Tue Jul 18 08:48:10 2023, max compression
```

## Comparing `session-repository-0.2.8.tar` & `session-repository-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 08:40:36.625167 session-repository-0.2.8/
--rw-rw-rw-   0        0        0      599 2023-07-18 08:40:36.623394 session-repository-0.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 08:40:36.591286 session-repository-0.2.8/session_repository/
--rw-rw-rw-   0        0        0      175 2023-07-18 08:38:06.000000 session-repository-0.2.8/session_repository/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.8/session_repository/enum.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:40:36.620467 session-repository-0.2.8/session_repository/models/
--rw-rw-rw-   0        0        0     7426 2023-07-18 08:36:44.000000 session-repository-0.2.8/session_repository/models/repository.py
--rw-rw-rw-   0        0        0      475 2023-07-18 08:36:28.000000 session-repository-0.2.8/session_repository/models/service.py
--rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.8/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:40:36.611885 session-repository-0.2.8/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 08:40:36.625842 session-repository-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-07-18 08:40:02.000000 session-repository-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:48:10.278839 session-repository-0.2.9/
+-rw-rw-rw-   0        0        0      599 2023-07-18 08:48:10.277837 session-repository-0.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 08:48:10.239329 session-repository-0.2.9/session_repository/
+-rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.2.9/session_repository/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.9/session_repository/enum.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:48:10.274234 session-repository-0.2.9/session_repository/models/
+-rw-rw-rw-   0        0        0     7424 2023-07-18 08:46:35.000000 session-repository-0.2.9/session_repository/models/repository.py
+-rw-rw-rw-   0        0        0      475 2023-07-18 08:36:28.000000 session-repository-0.2.9/session_repository/models/service.py
+-rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.9/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:48:10.264187 session-repository-0.2.9/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 08:48:10.000000 session-repository-0.2.9/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 08:48:10.279891 session-repository-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-18 08:47:07.000000 session-repository-0.2.9/setup.py
```

### Comparing `session-repository-0.2.8/PKG-INFO` & `session-repository-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.8
+Version: 0.2.9
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.8.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.8/session_repository/enum.py` & `session-repository-0.2.9/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.8/session_repository/models/repository.py` & `session-repository-0.2.9/session_repository/models/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     apply_no_load,
     apply_filters,
     apply_order_by,
     apply_limit,
     apply_pagination,
 )
 
-
 def with_session(func):
     def wrapper(self, *args, **kwargs):
         if "current_session" in kwargs:
             return func(self, *args, **kwargs)
 
         with self.session_manager() as session:
             kwargs["current_session"] = session
```

### Comparing `session-repository-0.2.8/session_repository/utils.py` & `session-repository-0.2.9/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.8/session_repository.egg-info/PKG-INFO` & `session-repository-0.2.9/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.8
+Version: 0.2.9
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.8.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.8/setup.py` & `session-repository-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.8"
+version = "0.2.9"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
         "session_repository.models",
```

