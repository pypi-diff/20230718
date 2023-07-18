# Comparing `tmp/easy_ge-0.1.12.3.tar.gz` & `tmp/easy_ge-0.1.12.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ge-0.1.12.3.tar", max compression
+gzip compressed data, was "easy_ge-0.1.12.4.tar", max compression
```

## Comparing `easy_ge-0.1.12.3.tar` & `easy_ge-0.1.12.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1059 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/LICENSE
--rw-r--r--   0        0        0      550 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/docs/pypi_readme.md
--rw-r--r--   0        0        0       41 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/easy_ge/__init__.py
--rw-r--r--   0        0        0      310 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/easy_ge/entrypoint.py
--rw-r--r--   0        0        0     6701 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/easy_ge/expectation_manager.py
--rw-r--r--   0        0        0     4468 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/easy_ge/helpers.py
--rw-r--r--   0        0        0     2177 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/easy_ge/main.py
--rw-r--r--   0        0        0      908 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/easy_ge/templates/checkpoint.tpl
--rw-r--r--   0        0        0     4535 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/easy_ge/templates/great_expectations.tpl
--rw-r--r--   0        0        0     5091 2023-07-18 13:35:05.871916 easy_ge-0.1.12.3/easy_ge/templates/schema.json
--rw-r--r--   0        0        0     1291 2023-07-18 13:35:05.875916 easy_ge-0.1.12.3/pyproject.toml
--rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 easy_ge-0.1.12.3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-18 16:11:42.883860 easy_ge-0.1.12.4/LICENSE
+-rw-r--r--   0        0        0      550 2023-07-18 16:11:42.883860 easy_ge-0.1.12.4/docs/pypi_readme.md
+-rw-r--r--   0        0        0       41 2023-07-18 16:11:42.883860 easy_ge-0.1.12.4/easy_ge/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-18 16:11:42.883860 easy_ge-0.1.12.4/easy_ge/entrypoint.py
+-rw-r--r--   0        0        0     6701 2023-07-18 16:11:42.887861 easy_ge-0.1.12.4/easy_ge/expectation_manager.py
+-rw-r--r--   0        0        0     4468 2023-07-18 16:11:42.887861 easy_ge-0.1.12.4/easy_ge/helpers.py
+-rw-r--r--   0        0        0     2177 2023-07-18 16:11:42.887861 easy_ge-0.1.12.4/easy_ge/main.py
+-rw-r--r--   0        0        0      908 2023-07-18 16:11:42.887861 easy_ge-0.1.12.4/easy_ge/templates/checkpoint.tpl
+-rw-r--r--   0        0        0     4535 2023-07-18 16:11:42.887861 easy_ge-0.1.12.4/easy_ge/templates/great_expectations.tpl
+-rw-r--r--   0        0        0     5091 2023-07-18 16:11:42.887861 easy_ge-0.1.12.4/easy_ge/templates/schema.json
+-rw-r--r--   0        0        0     1291 2023-07-18 16:11:42.887861 easy_ge-0.1.12.4/pyproject.toml
+-rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 easy_ge-0.1.12.4/PKG-INFO
```

### Comparing `easy_ge-0.1.12.3/LICENSE` & `easy_ge-0.1.12.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.3/docs/pypi_readme.md` & `easy_ge-0.1.12.4/docs/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.3/easy_ge/expectation_manager.py` & `easy_ge-0.1.12.4/easy_ge/expectation_manager.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.3/easy_ge/helpers.py` & `easy_ge-0.1.12.4/easy_ge/helpers.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.3/easy_ge/main.py` & `easy_ge-0.1.12.4/easy_ge/main.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.3/easy_ge/templates/checkpoint.tpl` & `easy_ge-0.1.12.4/easy_ge/templates/checkpoint.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.3/easy_ge/templates/great_expectations.tpl` & `easy_ge-0.1.12.4/easy_ge/templates/great_expectations.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.3/easy_ge/templates/schema.json` & `easy_ge-0.1.12.4/easy_ge/templates/schema.json`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.3/pyproject.toml` & `easy_ge-0.1.12.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy-ge"
-version = "0.1.12.3"
+version = "0.1.12.4"
 description = "A package that simplifies usage of Great Expectations tool for Data Validation."
 authors = ["Elsayed91 <elsayed.is@outlook.com>"]
 readme = "docs/pypi_readme.md"
 packages = [{include = "easy_ge"}]
 repository = "https://github.com/Elsayed91/easy_ge"
 keywords = ["Great Expectations", "data quality", "data validation"]
```

### Comparing `easy_ge-0.1.12.3/PKG-INFO` & `easy_ge-0.1.12.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ge
-Version: 0.1.12.3
+Version: 0.1.12.4
 Summary: A package that simplifies usage of Great Expectations tool for Data Validation.
 Home-page: https://github.com/Elsayed91/easy_ge
 Keywords: Great Expectations,data quality,data validation
 Author: Elsayed91
 Author-email: elsayed.is@outlook.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
```

