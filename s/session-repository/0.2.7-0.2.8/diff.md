# Comparing `tmp/session-repository-0.2.7.tar.gz` & `tmp/session-repository-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.2.7.tar", last modified: Mon Jul 17 19:22:12 2023, max compression
+gzip compressed data, was "session-repository-0.2.8.tar", last modified: Tue Jul 18 08:40:36 2023, max compression
```

## Comparing `session-repository-0.2.7.tar` & `session-repository-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 19:22:12.758985 session-repository-0.2.7/
--rw-rw-rw-   0        0        0      599 2023-07-17 19:22:12.753290 session-repository-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 19:22:12.690904 session-repository-0.2.7/session_repository/
--rw-rw-rw-   0        0        0     7787 2023-07-17 19:19:07.000000 session-repository-0.2.7/session_repository/core.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.7/session_repository/enum.py
--rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.7/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 19:22:12.746919 session-repository-0.2.7/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-17 19:22:12.000000 session-repository-0.2.7/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 19:22:12.766781 session-repository-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-17 19:20:25.000000 session-repository-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:40:36.625167 session-repository-0.2.8/
+-rw-rw-rw-   0        0        0      599 2023-07-18 08:40:36.623394 session-repository-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 08:40:36.591286 session-repository-0.2.8/session_repository/
+-rw-rw-rw-   0        0        0      175 2023-07-18 08:38:06.000000 session-repository-0.2.8/session_repository/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.2.8/session_repository/enum.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:40:36.620467 session-repository-0.2.8/session_repository/models/
+-rw-rw-rw-   0        0        0     7426 2023-07-18 08:36:44.000000 session-repository-0.2.8/session_repository/models/repository.py
+-rw-rw-rw-   0        0        0      475 2023-07-18 08:36:28.000000 session-repository-0.2.8/session_repository/models/service.py
+-rw-rw-rw-   0        0        0     9499 2023-07-13 16:52:30.000000 session-repository-0.2.8/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:40:36.611885 session-repository-0.2.8/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-18 08:40:36.000000 session-repository-0.2.8/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 08:40:36.625842 session-repository-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-18 08:40:02.000000 session-repository-0.2.8/setup.py
```

### Comparing `session-repository-0.2.7/PKG-INFO` & `session-repository-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.7
+Version: 0.2.8
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.7.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.8.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.7/session_repository/core.py` & `session-repository-0.2.8/session_repository/models/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 # MODULES
-from contextlib import AbstractContextManager
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 from logging import Logger
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Union,
-    TypeVar
-)
+
+# CONNTEXTLIB
+from contextlib import AbstractContextManager
 
 # SQLALCHEMY
 from sqlalchemy.orm import Session, InstrumentedAttribute, Query
 
 # UTILS
 from session_repository.utils import (
     _FilterType,
@@ -280,21 +273,7 @@
 
         if flush:
             current_session.flush()
         if commit:
             current_session.commit()
 
         return True
-
-
-T = TypeVar("T", bound=SessionRepository)
-class SessionService:
-    def __init__(
-        self,
-        repository: T,
-        logger: Logger,
-    ) -> None:
-        self._repository = repository
-        self._logger = logger
-
-    def session_manager(self):
-        return self._repository.session_manager()
```

### Comparing `session-repository-0.2.7/session_repository/enum.py` & `session-repository-0.2.8/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.7/session_repository/utils.py` & `session-repository-0.2.8/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.2.7/session_repository.egg-info/PKG-INFO` & `session-repository-0.2.8/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.2.7
+Version: 0.2.8
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.7.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.2.8.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.2.7/setup.py` & `session-repository-0.2.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup
 
-version = "0.2.7"
+version = "0.2.8"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
+        "session_repository.models",
     ],
     install_requires=[
         "sqlalchemy==1.4.41",
     ],
     license="MIT",
     author="Maxime MARTIN",
     author_email="maxime.martin02@hotmail.fr",
```

