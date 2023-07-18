# Comparing `tmp/superspreader-0.2.7.1.tar.gz` & `tmp/superspreader-0.2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superspreader-0.2.7.1.tar", last modified: Tue Jul 18 09:29:55 2023, max compression
+gzip compressed data, was "superspreader-0.2.7.2.tar", last modified: Tue Jul 18 09:35:28 2023, max compression
```

## Comparing `superspreader-0.2.7.1.tar` & `superspreader-0.2.7.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:29:55.597172 superspreader-0.2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-18 09:29:55.597172 superspreader-0.2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 09:29:55.597172 superspreader-0.2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:29:55.593172 superspreader-0.2.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:29:55.593172 superspreader-0.2.7.1/src/superspreader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/src/superspreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/src/superspreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/src/superspreader/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/src/superspreader/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/src/superspreader/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/src/superspreader/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:29:55.597172 superspreader-0.2.7.1/src/superspreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-18 09:29:55.000000 superspreader-0.2.7.1/src/superspreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-18 09:29:55.000000 superspreader-0.2.7.1/src/superspreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:29:55.000000 superspreader-0.2.7.1/src/superspreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 09:29:55.000000 superspreader-0.2.7.1/src/superspreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 09:29:55.000000 superspreader-0.2.7.1/src/superspreader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:29:55.597172 superspreader-0.2.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/tests/test_full_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-18 09:29:43.000000 superspreader-0.2.7.1/tests/test_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:35:28.081697 superspreader-0.2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-18 09:35:28.081697 superspreader-0.2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 09:35:28.085697 superspreader-0.2.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:35:28.081697 superspreader-0.2.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:35:28.081697 superspreader-0.2.7.2/src/superspreader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/src/superspreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/src/superspreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/src/superspreader/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/src/superspreader/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/src/superspreader/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/src/superspreader/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:35:28.081697 superspreader-0.2.7.2/src/superspreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-18 09:35:28.000000 superspreader-0.2.7.2/src/superspreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-18 09:35:28.000000 superspreader-0.2.7.2/src/superspreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:35:28.000000 superspreader-0.2.7.2/src/superspreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 09:35:28.000000 superspreader-0.2.7.2/src/superspreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 09:35:28.000000 superspreader-0.2.7.2/src/superspreader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:35:28.081697 superspreader-0.2.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/tests/test_full_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-18 09:35:18.000000 superspreader-0.2.7.2/tests/test_sheet.py
```

### Comparing `superspreader-0.2.7.1/LICENSE.txt` & `superspreader-0.2.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.7.1/PKG-INFO` & `superspreader-0.2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.7.1
+Version: 0.2.7.2
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Intended Audience :: Developers
```

### Comparing `superspreader-0.2.7.1/README.md` & `superspreader-0.2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.7.1/setup.py` & `superspreader-0.2.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="superspreader",
-    version="0.2.7.1",
+    version="0.2.7.2",
     description="Load data from spreadsheets easily",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/julianklotz/superspreader",
     author="Julian Klotz",
     author_email="post@julianklotz.de",
     classifiers=[
```

### Comparing `superspreader-0.2.7.1/src/superspreader/fields.py` & `superspreader-0.2.7.2/src/superspreader/fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.7.1/src/superspreader/i18n.py` & `superspreader-0.2.7.2/src/superspreader/i18n.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.7.1/src/superspreader/messages.py` & `superspreader-0.2.7.2/src/superspreader/messages.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.7.1/src/superspreader/sheets.py` & `superspreader-0.2.7.2/src/superspreader/sheets.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,16 @@
                 self._validate_unique_field(name, field.source)
 
     def _validate_unique_field(self, field_name, column_name):
         values = list(map(lambda row: row.get(field_name), self._rows))
         distinct_values = set(values)
 
         for value in distinct_values:
-            if total := values.count(value) > 1:
+            total = values.count(value)
+            if total > 1:
                 msg = _(
                     "sheet.unique_violation",
                     self.language,
                     params={"column": column_name, "value": value, "total": total},
                 )
                 self._add_error(msg)
```

### Comparing `superspreader-0.2.7.1/src/superspreader.egg-info/PKG-INFO` & `superspreader-0.2.7.2/src/superspreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.7.1
+Version: 0.2.7.2
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Intended Audience :: Developers
```

### Comparing `superspreader-0.2.7.1/tests/test_fields.py` & `superspreader-0.2.7.2/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.7.1/tests/test_full_import.py` & `superspreader-0.2.7.2/tests/test_full_import.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.7.1/tests/test_sheet.py` & `superspreader-0.2.7.2/tests/test_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,9 +66,9 @@
         path = file_path("contacts_duplicates.xlsx")
         sheet = ContactSheet(path)
         sheet.load()
 
         self.assertEqual(len(sheet.errors), 1)
         self.assertEqual(
             sheet.errors[0],
-            "“ID” must contain unique values only, but “1” occurs 1 times",
+            "“ID” must contain unique values only, but “1” occurs 2 times",
         )
```

