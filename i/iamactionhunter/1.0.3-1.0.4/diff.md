# Comparing `tmp/iamactionhunter-1.0.3.tar.gz` & `tmp/iamactionhunter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamactionhunter-1.0.3.tar", max compression
+gzip compressed data, was "iamactionhunter-1.0.4.tar", max compression
```

## Comparing `iamactionhunter-1.0.3.tar` & `iamactionhunter-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11430 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/IAMActionHunter.py
--rw-r--r--   0        0        0        0 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/configs/__init.py__
--rw-r--r--   0        0        0     5970 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/configs/all.py
--rw-r--r--   0        0        0        0 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/__init__.py
--rw-r--r--   0        0        0     1973 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/create_csv.py
--rw-r--r--   0        0        0     6108 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/data_collection.py
--rw-r--r--   0        0        0     4141 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/statement_parser.py
--rw-r--r--   0        0        0      433 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/IAMActionHunter/lib/text_formatter.py
--rw-r--r--   0        0        0    11357 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/LICENSE
--rw-r--r--   0        0        0     4183 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/README.md
--rw-r--r--   0        0        0      882 2023-06-27 22:17:51.073304 iamactionhunter-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 iamactionhunter-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11430 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/IAMActionHunter/IAMActionHunter.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/IAMActionHunter/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/IAMActionHunter/configs/__init.py__
+-rw-r--r--   0        0        0     5970 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/IAMActionHunter/configs/all.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/IAMActionHunter/lib/__init__.py
+-rw-r--r--   0        0        0     1973 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/IAMActionHunter/lib/create_csv.py
+-rw-r--r--   0        0        0     6108 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/IAMActionHunter/lib/data_collection.py
+-rw-r--r--   0        0        0     4141 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/IAMActionHunter/lib/statement_parser.py
+-rw-r--r--   0        0        0      433 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/IAMActionHunter/lib/text_formatter.py
+-rw-r--r--   0        0        0    11357 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4183 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/README.md
+-rw-r--r--   0        0        0      882 2023-07-18 19:51:42.296387 iamactionhunter-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 iamactionhunter-1.0.4/PKG-INFO
```

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/IAMActionHunter.py` & `iamactionhunter-1.0.4/IAMActionHunter/IAMActionHunter.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/configs/all.py` & `iamactionhunter-1.0.4/IAMActionHunter/configs/all.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/lib/create_csv.py` & `iamactionhunter-1.0.4/IAMActionHunter/lib/create_csv.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/lib/data_collection.py` & `iamactionhunter-1.0.4/IAMActionHunter/lib/data_collection.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/IAMActionHunter/lib/statement_parser.py` & `iamactionhunter-1.0.4/IAMActionHunter/lib/statement_parser.py`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/LICENSE` & `iamactionhunter-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/README.md` & `iamactionhunter-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `iamactionhunter-1.0.3/pyproject.toml` & `iamactionhunter-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "IAMActionHunter"
-version = "1.0.3"
+version = "1.0.4"
 description = "A query tool for AWS IAM policy statements."
 authors = ["Dave Yesland with Rhino Security Labs"]
 readme = "README.md"
 packages = [{include = "IAMActionHunter"},{include="lib", from="IAMActionHunter"},{include="configs", from="IAMActionHunter"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `iamactionhunter-1.0.3/PKG-INFO` & `iamactionhunter-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamactionhunter
-Version: 1.0.3
+Version: 1.0.4
 Summary: A query tool for AWS IAM policy statements.
 Author: Dave Yesland with Rhino Security Labs
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

