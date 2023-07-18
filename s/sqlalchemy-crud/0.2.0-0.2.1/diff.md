# Comparing `tmp/sqlalchemy_crud-0.2.0.tar.gz` & `tmp/sqlalchemy_crud-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_crud-0.2.0.tar", max compression
+gzip compressed data, was "sqlalchemy_crud-0.2.1.tar", max compression
```

## Comparing `sqlalchemy_crud-0.2.0.tar` & `sqlalchemy_crud-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/LICENSE
--rw-r--r--   0        0        0     3959 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/README.md
--rw-r--r--   0        0        0      657 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      221 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/sqlalchemy_crud/__init__.py
--rw-r--r--   0        0        0     3542 2023-07-17 21:50:55.751247 sqlalchemy_crud-0.2.0/sqlalchemy_crud/crud.py
--rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 sqlalchemy_crud-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-18 02:36:25.515597 sqlalchemy_crud-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3959 2023-07-18 02:36:25.515597 sqlalchemy_crud-0.2.1/README.md
+-rw-r--r--   0        0        0      657 2023-07-18 02:36:25.515597 sqlalchemy_crud-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-18 02:36:25.515597 sqlalchemy_crud-0.2.1/sqlalchemy_crud/__init__.py
+-rw-r--r--   0        0        0     3542 2023-07-18 02:36:25.515597 sqlalchemy_crud-0.2.1/sqlalchemy_crud/crud.py
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 sqlalchemy_crud-0.2.1/PKG-INFO
```

### Comparing `sqlalchemy_crud-0.2.0/LICENSE` & `sqlalchemy_crud-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_crud-0.2.0/README.md` & `sqlalchemy_crud-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_crud-0.2.0/pyproject.toml` & `sqlalchemy_crud-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sqlalchemy-crud"
 repository = "https://github.com/cblack34/sqlalchemy-crud"
-version = "0.2.0"
+version = "0.2.1"
 description = "Basic C.R.U.D for SQLAlchemy models"
 authors = ["Clayton Black"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/cblack34/sqlalchemy-crud/issues"
```

### Comparing `sqlalchemy_crud-0.2.0/sqlalchemy_crud/crud.py` & `sqlalchemy_crud-0.2.1/sqlalchemy_crud/crud.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_crud-0.2.0/PKG-INFO` & `sqlalchemy_crud-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-crud
-Version: 0.2.0
+Version: 0.2.1
 Summary: Basic C.R.U.D for SQLAlchemy models
 Home-page: https://github.com/cblack34/sqlalchemy-crud
 License: MIT
 Author: Clayton Black
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

