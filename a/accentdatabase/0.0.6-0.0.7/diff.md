# Comparing `tmp/accentdatabase-0.0.6.tar.gz` & `tmp/accentdatabase-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accentdatabase-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "accentdatabase-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `accentdatabase-0.0.6.tar` & `accentdatabase-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentdatabase-0.0.6/.flake8
--rw-r--r--   0        0        0      929 2023-07-10 10:47:48.676086 accentdatabase-0.0.6/.github/workflows/test.yml
--rw-r--r--   0        0        0       98 2022-10-05 13:05:19.000000 accentdatabase-0.0.6/.gitignore
--rw-r--r--   0        0        0     1090 2022-10-10 11:22:41.000000 accentdatabase-0.0.6/LICENSE
--rw-r--r--   0        0        0      319 2022-10-06 08:19:07.000000 accentdatabase-0.0.6/README.md
--rw-r--r--   0        0        0      134 2023-07-10 10:53:16.119670 accentdatabase-0.0.6/accentdatabase/__init__.py
--rw-r--r--   0        0        0      481 2023-03-30 07:48:07.000000 accentdatabase-0.0.6/accentdatabase/base.py
--rw-r--r--   0        0        0      413 2023-07-10 10:42:42.375920 accentdatabase-0.0.6/accentdatabase/config.py
--rw-r--r--   0        0        0      333 2022-10-07 08:58:02.000000 accentdatabase-0.0.6/accentdatabase/encoders.py
--rw-r--r--   0        0        0      243 2023-07-10 10:09:15.252548 accentdatabase-0.0.6/accentdatabase/engine.py
--rw-r--r--   0        0        0      658 2023-02-24 15:56:58.000000 accentdatabase-0.0.6/accentdatabase/mixins.py
--rw-r--r--   0        0        0     6675 2023-01-03 13:49:46.000000 accentdatabase-0.0.6/accentdatabase/operations.py
--rw-r--r--   0        0        0      852 2023-07-10 10:52:21.692037 accentdatabase-0.0.6/accentdatabase/session.py
--rw-r--r--   0        0        0     1007 2023-07-10 10:09:51.012364 accentdatabase-0.0.6/accentdatabase/testing.py
--rw-r--r--   0        0        0     1304 2023-07-10 10:45:05.999094 accentdatabase-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 accentdatabase-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentdatabase-0.0.7/.flake8
+-rw-r--r--   0        0        0      929 2023-07-10 10:47:48.676086 accentdatabase-0.0.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0       98 2022-10-05 13:05:19.000000 accentdatabase-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1090 2022-10-10 11:22:41.000000 accentdatabase-0.0.7/LICENSE
+-rw-r--r--   0        0        0      319 2022-10-06 08:19:07.000000 accentdatabase-0.0.7/README.md
+-rw-r--r--   0        0        0      134 2023-07-18 11:10:48.248747 accentdatabase-0.0.7/accentdatabase/__init__.py
+-rw-r--r--   0        0        0      481 2023-03-30 07:48:07.000000 accentdatabase-0.0.7/accentdatabase/base.py
+-rw-r--r--   0        0        0      384 2023-07-18 11:09:14.197112 accentdatabase-0.0.7/accentdatabase/config.py
+-rw-r--r--   0        0        0      243 2023-07-10 10:09:15.252548 accentdatabase-0.0.7/accentdatabase/engine.py
+-rw-r--r--   0        0        0      658 2023-02-24 15:56:58.000000 accentdatabase-0.0.7/accentdatabase/mixins.py
+-rw-r--r--   0        0        0     6675 2023-01-03 13:49:46.000000 accentdatabase-0.0.7/accentdatabase/operations.py
+-rw-r--r--   0        0        0      852 2023-07-10 10:52:21.692037 accentdatabase-0.0.7/accentdatabase/session.py
+-rw-r--r--   0        0        0     1007 2023-07-10 10:09:51.012364 accentdatabase-0.0.7/accentdatabase/testing.py
+-rw-r--r--   0        0        0     1304 2023-07-10 10:45:05.999094 accentdatabase-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 accentdatabase-0.0.7/PKG-INFO
```

### Comparing `accentdatabase-0.0.6/.github/workflows/test.yml` & `accentdatabase-0.0.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.6/LICENSE` & `accentdatabase-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.6/accentdatabase/mixins.py` & `accentdatabase-0.0.7/accentdatabase/mixins.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.6/accentdatabase/operations.py` & `accentdatabase-0.0.7/accentdatabase/operations.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.6/accentdatabase/session.py` & `accentdatabase-0.0.7/accentdatabase/session.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.6/accentdatabase/testing.py` & `accentdatabase-0.0.7/accentdatabase/testing.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.6/pyproject.toml` & `accentdatabase-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.6/PKG-INFO` & `accentdatabase-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accentdatabase
-Version: 0.0.6
+Version: 0.0.7
 Summary: Handling sqlalchemy connection and test helpers including
 Author-email: Accent Design Group Ltd <support@accentdesign.co.uk>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: accentdatabase Version: 0.0.6 Summary: Handling
+Metadata-Version: 2.1 Name: accentdatabase Version: 0.0.7 Summary: Handling
 sqlalchemy connection and test helpers including Author-email: Accent Design
 Group Ltd
 accentdesign.co.uk> Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 Requires-Dist: pydantic>=2.0.1,<2.1.0 Requires-Dist: pydantic-
 settings>=2.0.1,<2.1.0 Requires-Dist: sqlalchemy>=2.0.0,<2.1.0 Requires-Dist:
```

