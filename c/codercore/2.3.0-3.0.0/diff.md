# Comparing `tmp/codercore-2.3.0.tar.gz` & `tmp/codercore-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codercore-2.3.0.tar", last modified: Mon Jun 26 15:07:49 2023, max compression
+gzip compressed data, was "codercore-3.0.0.tar", last modified: Tue Jul 18 13:08:07 2023, max compression
```

## Comparing `codercore-2.3.0.tar` & `codercore-3.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 15:07:49.303639 codercore-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 15:07:23.000000 codercore-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.299639 codercore-2.3.0/codercore/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.299639 codercore-2.3.0/codercore/db/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/db/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/codercore/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/codercore/lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/schemas/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/codercore/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/test/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/test/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.299639 codercore-2.3.0/codercore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-26 15:07:23.000000 codercore-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:07:49.303639 codercore-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-26 15:07:23.000000 codercore-2.3.0/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:08:07.742183 codercore-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 13:08:07.742183 codercore-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 13:07:42.000000 codercore-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:08:07.734183 codercore-3.0.0/codercore/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:08:07.738183 codercore-3.0.0/codercore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/db/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:08:07.738183 codercore-3.0.0/codercore/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/lib/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/lib/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/lib/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:08:07.738183 codercore-3.0.0/codercore/lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/lib/schemas/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:08:07.742183 codercore-3.0.0/codercore/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/test/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/test/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 13:07:42.000000 codercore-3.0.0/codercore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:08:07.738183 codercore-3.0.0/codercore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 13:08:07.000000 codercore-3.0.0/codercore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-18 13:08:07.000000 codercore-3.0.0/codercore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:08:07.000000 codercore-3.0.0/codercore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-18 13:08:07.000000 codercore-3.0.0/codercore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 13:08:07.000000 codercore-3.0.0/codercore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-18 13:07:42.000000 codercore-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:08:07.742183 codercore-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:08:07.742183 codercore-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-18 13:07:42.000000 codercore-3.0.0/tests/test_types.py
```

### Comparing `codercore-2.3.0/codercore/db/__init__.py` & `codercore-3.0.0/codercore/db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from functools import cache
 from typing import Callable, Optional, Type
 
 from asyncpg.connection import Connection
 from asyncstdlib.functools import cache as async_cache
 from google.cloud.sql.connector import IPTypes, create_async_connector
-from sqlalchemy import select as sa_select
 from sqlalchemy.dialects.postgresql.asyncpg import (
     AsyncAdapt_asyncpg_connection,
     AsyncAdapt_asyncpg_dbapi,
 )
 from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
 from sqlalchemy.orm import Session as Session_, sessionmaker as sessionmaker_
 from sqlalchemy.pool import Pool
-from sqlalchemy.sql import Select
 from sqlalchemy.util import await_only
 
 from codercore.db.models import Base
-from codercore.db.pagination import paginate
 
 
 @cache
 def Session(connection_url: str) -> Session_:  # noqa
     return sessionmaker(connection_url)()
 
 
@@ -65,13 +62,7 @@
         )
         return AsyncAdapt_asyncpg_connection(
             AsyncAdapt_asyncpg_dbapi(__import__("asyncpg")),
             await_only(connection),
         )
 
     return creator
-
-
-def select(*args, **kwargs) -> Select:
-    statement = sa_select(*args, **kwargs)
-    statement.paginate = paginate.__get__(statement)
-    return statement
```

### Comparing `codercore-2.3.0/codercore/db/pagination.py` & `codercore-3.0.0/codercore/db/pagination.py`

 * *Files identical despite different names*

### Comparing `codercore-2.3.0/codercore/lib/hash.py` & `codercore-3.0.0/codercore/lib/hash.py`

 * *Files identical despite different names*

### Comparing `codercore-2.3.0/codercore/lib/redis.py` & `codercore-3.0.0/codercore/lib/redis.py`

 * *Files identical despite different names*

### Comparing `codercore-2.3.0/codercore/lib/settings.py` & `codercore-3.0.0/codercore/lib/settings.py`

 * *Files identical despite different names*

### Comparing `codercore-2.3.0/codercore/test/fixtures.py` & `codercore-3.0.0/codercore/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `codercore-2.3.0/codercore/test/pydantic.py` & `codercore-3.0.0/codercore/test/pydantic.py`

 * *Files identical despite different names*

### Comparing `codercore-2.3.0/codercore.egg-info/SOURCES.txt` & `codercore-3.0.0/codercore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codercore-2.3.0/pyproject.toml` & `codercore-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codercore"
-version = "2.3.0"
+version = "3.0.0"
 description = "codercore"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
     'asyncpg ~= 0.27',
     'asyncstdlib ~= 3.10',
     'bcrypt ~= 4.0',
@@ -31,15 +31,15 @@
 dev = [
     'black ~= 22.10',
     'flake8 ~= 6.0',
     'isort ~= 5.11',
 ]
 
 [tool.bumpver]
-current_version = "2.3.0"
+current_version = "3.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

