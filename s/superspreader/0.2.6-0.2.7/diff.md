# Comparing `tmp/superspreader-0.2.6.tar.gz` & `tmp/superspreader-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superspreader-0.2.6.tar", last modified: Thu Jun 15 07:34:20 2023, max compression
+gzip compressed data, was "superspreader-0.2.7.tar", last modified: Tue Jul 18 08:49:28 2023, max compression
```

## Comparing `superspreader-0.2.6.tar` & `superspreader-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.975258 superspreader-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 07:34:11.000000 superspreader-0.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-15 07:34:20.975258 superspreader-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-15 07:34:11.000000 superspreader-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 07:34:11.000000 superspreader-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-15 07:34:20.975258 superspreader-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-15 07:34:11.000000 superspreader-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.971258 superspreader-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.975258 superspreader-0.2.6/src/superspreader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-06-15 07:34:11.000000 superspreader-0.2.6/src/superspreader/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.975258 superspreader-0.2.6/src/superspreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 07:34:20.000000 superspreader-0.2.6/src/superspreader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:34:20.975258 superspreader-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 07:34:11.000000 superspreader-0.2.6/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-15 07:34:11.000000 superspreader-0.2.6/tests/test_full_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-15 07:34:11.000000 superspreader-0.2.6/tests/test_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:28.398425 superspreader-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 08:49:18.000000 superspreader-0.2.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-18 08:49:28.398425 superspreader-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-18 08:49:18.000000 superspreader-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 08:49:18.000000 superspreader-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 08:49:28.398425 superspreader-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-18 08:49:18.000000 superspreader-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:28.394425 superspreader-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:28.398425 superspreader-0.2.7/src/superspreader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:18.000000 superspreader-0.2.7/src/superspreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-18 08:49:18.000000 superspreader-0.2.7/src/superspreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-18 08:49:18.000000 superspreader-0.2.7/src/superspreader/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-18 08:49:18.000000 superspreader-0.2.7/src/superspreader/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-18 08:49:18.000000 superspreader-0.2.7/src/superspreader/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-07-18 08:49:18.000000 superspreader-0.2.7/src/superspreader/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:28.398425 superspreader-0.2.7/src/superspreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-18 08:49:28.000000 superspreader-0.2.7/src/superspreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-18 08:49:28.000000 superspreader-0.2.7/src/superspreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:49:28.000000 superspreader-0.2.7/src/superspreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 08:49:28.000000 superspreader-0.2.7/src/superspreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 08:49:28.000000 superspreader-0.2.7/src/superspreader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:49:28.398425 superspreader-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-18 08:49:18.000000 superspreader-0.2.7/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-18 08:49:18.000000 superspreader-0.2.7/tests/test_full_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-18 08:49:18.000000 superspreader-0.2.7/tests/test_sheet.py
```

### Comparing `superspreader-0.2.6/LICENSE.txt` & `superspreader-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.6/PKG-INFO` & `superspreader-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.6
+Version: 0.2.7
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Intended Audience :: Developers
@@ -80,14 +80,18 @@
 # {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}
 ```
 
 In `tests/spreadsheets` is a sample spreadsheet that is used for testing. Feel free to fiddle around.
 
 There’s a lot more to say and I’ll update the documentation as I go.
 
+## Field params
+
+Fields must have a `source`”`parameter, that holds the column name for the spreadsheet.`unique=True` may be used to indicate that a field’s value must be unique.
+
 ## Adding static & dynamic data to rows
 
 To provide additional data, use `extra_data`. Data from the spreadsheet take precedence over extra data.
 
 ```
 extra_data = {
     "status": "released"
@@ -106,14 +110,18 @@
 
 sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
 # {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': '“Toy” by David Bowie'}
 ```
 
 ## Changelog
 
+### 0.2.7
+
+- Adds support for unique validation
+
 ### 0.2.3
 
 - Adds support for inheriting sheets (before that, fields from base classes weren’t recognized)
 
 ### 0.2.2
 
 - Adds support for callables in `extra_data`
```

### Comparing `superspreader-0.2.6/README.md` & `superspreader-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,18 @@
 # {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}
 ```
 
 In `tests/spreadsheets` is a sample spreadsheet that is used for testing. Feel free to fiddle around.
 
 There’s a lot more to say and I’ll update the documentation as I go.
 
+## Field params
+
+Fields must have a `source`”`parameter, that holds the column name for the spreadsheet.`unique=True` may be used to indicate that a field’s value must be unique.
+
 ## Adding static & dynamic data to rows
 
 To provide additional data, use `extra_data`. Data from the spreadsheet take precedence over extra data.
 
 ```
 extra_data = {
     "status": "released"
@@ -82,14 +86,18 @@
 
 sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
 # {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': '“Toy” by David Bowie'}
 ```
 
 ## Changelog
 
+### 0.2.7
+
+- Adds support for unique validation
+
 ### 0.2.3
 
 - Adds support for inheriting sheets (before that, fields from base classes weren’t recognized)
 
 ### 0.2.2
 
 - Adds support for callables in `extra_data`
```

### Comparing `superspreader-0.2.6/setup.py` & `superspreader-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="superspreader",
-    version="0.2.6",
+    version="0.2.7",
     description="Load data from spreadsheets easily",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/julianklotz/superspreader",
     author="Julian Klotz",
     author_email="post@julianklotz.de",
     classifiers=[
```

### Comparing `superspreader-0.2.6/src/superspreader/fields.py` & `superspreader-0.2.7/src/superspreader/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,26 @@
 
 
 class BaseField(ABC):
     target_type = None
     default = None
     cast_type = True
 
-    def __init__(self, source, required=True, default=None):
+    def __init__(self, source, required=True, default=None, unique=False):
+        """
+        :param str source: The column name from the spreadsheet
+        :param bool required: Indicates whether a non-`None` value is required.
+                              Ignored when a default value is provided.
+        :param any default: The default value to use
+        :param bool unique: Indicates whether values must be unique
+        """
         self.source = source
         self.required = required
+        self.unique = unique
+
         self.language = None
         self.extra_context = None
 
         if default is not None:
             self.default = default
 
     def __call__(self, value, language, extra_context=None):
```

### Comparing `superspreader-0.2.6/src/superspreader/i18n.py` & `superspreader-0.2.7/src/superspreader/i18n.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.6/src/superspreader/messages.py` & `superspreader-0.2.7/src/superspreader/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,18 @@
         "field.related_multiple_objects_returned": (
             "More than one related object identified by %(value)s on “%(field)s”",
             None,
         ),
         "sheet.row_info": ("Row %(row)s: %(message)s", None),
         "sheet.column_missing": ("Column “%(column)s” not present in sheet", None),
         "sheet.sheet_missing": ("Sheet “%(sheet)s” not present in document", None),
+        "sheet.unique_violation": (
+            "“%(column)s” must contain unique values only, but “%(value)s” occurs %(total)i times",
+            None,
+        ),
     },
     DE: {
         "field.wrong_type": (
             "„%(field)s“ sollte den Typ %(target_type)s haben, aber der"
             "Typ ist %(actual_type)s",
             None,
         ),
@@ -41,9 +45,13 @@
         "field.related_multiple_objects_returned": (
             "Mehr als ein Objekt mit %(value)s beim „%(field)s“ gefunden",
             None,
         ),
         "sheet.row_info": ("Zeile %(row)s: %(message)s", None),
         "sheet.column_missing": ("Die Spalte „%(column)s“ fehlt im Blatt", None),
         "sheet.sheet_missing": ("Das Blatt „%(sheet)s“ ist nicht vorhanden", None),
+        "sheet.unique_violation": (
+            "„%(column)s“ darf nur eindeutige Werte enthalten, „%(value)s“ kommt aber %(total)i mal vor",
+            None,
+        ),
     },
 }
```

### Comparing `superspreader-0.2.6/src/superspreader/sheets.py` & `superspreader-0.2.7/src/superspreader/sheets.py`

 * *Files 10% similar despite different names*

```diff
@@ -123,14 +123,16 @@
                 # Use extra data as a basis
                 full_dict = self.get_extra_data(row_dict)
                 # And update with “real” data, which takes precedence
                 full_dict.update(row_dict)
                 self._rows.append(full_dict)
                 self._add_errors(error_cache)
 
+        self._validate_unique_fields()
+
     def get_sheet_name(self):
         """
         Gets the sheet
         :return: str
         """
         return self.sheet_name
 
@@ -226,14 +228,32 @@
                 params={
                     "row": index + 1 + self.get_header_rows(),
                     "message": message,
                 },
             )
         self._infos.append(message)
 
+    def _validate_unique_fields(self):
+        for name, field in self._fields.items():
+            if field.unique is True:
+                self._validate_unique_field(name, field.source)
+
+    def _validate_unique_field(self, field_name, column_name):
+        values = list(map(lambda row: row.get(field_name), self._rows))
+        distinct_values = set(values)
+
+        for value in distinct_values:
+            if total := values.count(value) > 1:
+                msg = _(
+                    "sheet.unique_violation",
+                    self.language,
+                    params={"column": column_name, "value": value, "total": total},
+                )
+                self._add_error(msg)
+
     def _check(self) -> None:
         """
         Perform configuration checks. Add your own in subclasses
         :raises ImproperlyConfigured
         """
         if self.get_header_rows() < 1:
             raise ImproperlyConfigured("Sheets must have at least one header row")
@@ -276,16 +296,15 @@
     def __check_columns_present(self, column_map) -> None:
         """
         Checks whether the columns (described by the source attribute of fields) are present.
         Missing columns are added to error list.
 
         :param column_map: The column map
         """
-        fields = self._build_fields()
-        used_fields = set([field.source for field in fields.values()])
+        used_fields = set([field.source for field in self._fields.values()])
         all_fields = set(column_map.keys())
 
         for field in used_fields:
             if field not in all_fields:
                 msg = _("sheet.column_missing", self.language, params={"column": field})
                 self._add_error(msg)
```

### Comparing `superspreader-0.2.6/src/superspreader.egg-info/PKG-INFO` & `superspreader-0.2.7/src/superspreader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.6
+Version: 0.2.7
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Intended Audience :: Developers
@@ -80,14 +80,18 @@
 # {'artist': 'Kokoroko', 'album': 'Could We Be More', 'release_date': datetime.date(2022, 8, 1), 'average_review': 4.7, 'chart_position': 30}
 ```
 
 In `tests/spreadsheets` is a sample spreadsheet that is used for testing. Feel free to fiddle around.
 
 There’s a lot more to say and I’ll update the documentation as I go.
 
+## Field params
+
+Fields must have a `source`”`parameter, that holds the column name for the spreadsheet.`unique=True` may be used to indicate that a field’s value must be unique.
+
 ## Adding static & dynamic data to rows
 
 To provide additional data, use `extra_data`. Data from the spreadsheet take precedence over extra data.
 
 ```
 extra_data = {
     "status": "released"
@@ -106,14 +110,18 @@
 
 sheet = AlbumSheet("albums.xlsx", extra_data=extra_data)
 # {'artist': 'David Bowie', 'album': 'Toy', 'release_date': datetime.date(2022, 1, 7), 'average_review': 4.3, 'chart_position': 5, 'summary': '“Toy” by David Bowie'}
 ```
 
 ## Changelog
 
+### 0.2.7
+
+- Adds support for unique validation
+
 ### 0.2.3
 
 - Adds support for inheriting sheets (before that, fields from base classes weren’t recognized)
 
 ### 0.2.2
 
 - Adds support for callables in `extra_data`
```

### Comparing `superspreader-0.2.6/tests/test_fields.py` & `superspreader-0.2.7/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.6/tests/test_full_import.py` & `superspreader-0.2.7/tests/test_full_import.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # the inclusion of the tests module is not meant to offer best practices for
 # testing in general, but rather to support the `find_packages` example in
 # setup.py that excludes installing the "tests" package
 
 import datetime
-import os
 import unittest
-from pathlib import Path
 from unittest.mock import MagicMock
 
 from superspreader import fields
 from superspreader.sheets import BaseSheet
+from tests import file_path
 
 
 class AlbumSheet(BaseSheet):
     sheet_name = "Albums"
     header_rows = 3
     label_row = 2
 
@@ -25,21 +24,16 @@
 
 
 class TestFullImport(unittest.TestCase):
     """
     Test the process of importing a spreadsheet
     """
 
-    def _file_path(self, file_name):
-        tests_dir = Path(__file__).parent.absolute()
-        path = os.path.join(tests_dir, "spreadsheets", file_name)
-        return path
-
     def setUp(self) -> None:
-        self.sheet = AlbumSheet(self._file_path("albums.xlsx"))
+        self.sheet = AlbumSheet(file_path("albums.xlsx"))
 
     def test_basics(self):
         self.sheet.load()
         self.assertFalse(self.sheet.has_errors)
         self.assertEqual(len(self.sheet), 3)
 
     def test_record(self):
@@ -59,45 +53,45 @@
             rows[0]["album"]
 
     def test_info(self):
         self.sheet.load()
         self.assertEqual("Row 6: Skipped row", self.sheet.infos[0])
 
     def test_errors(self):
-        path = self._file_path("albums_with_errors.xlsx")
+        path = file_path("albums_with_errors.xlsx")
         sheet_with_errors = AlbumSheet(path)
         sheet_with_errors.load()
 
         self.assertTrue(sheet_with_errors.has_errors)
         self.assertEqual(sheet_with_errors.errors[0], "Row 7: “Album” is required")
 
     def test_empty_sheet_with_extra_data(self):
         """Tests whether empty rows are skipped, even when extra data is provided"""
-        path = self._file_path("albums_empty.xlsx")
+        path = file_path("albums_empty.xlsx")
         sheet = AlbumSheet(path, extra_data={"status": "released"})
         self.assertFalse(sheet.has_errors)
         self.assertEqual(len(sheet), 0)
 
     def test_extra_data_static(self):
         """Tests whether extra data is returned in the resulting row"""
-        fp = self._file_path("albums.xlsx")
+        fp = file_path("albums.xlsx")
         sheet = AlbumSheet(path=fp, extra_data={"status": "released"})
         sheet.load()
         self.assertEqual(sheet.rows()[0].get("status"), "released")
 
     def test_extra_data_dynamic(self):
         """Tests whether callables in extra data are called"""
-        fp = self._file_path("albums.xlsx")
+        fp = file_path("albums.xlsx")
         test_fn = MagicMock()
         sheet = AlbumSheet(path=fp, extra_data={"test_fn": test_fn})
         sheet.load()
         test_fn.assert_called()
 
     def test_extra_data_dynamic_args(self):
         """Tests whether callables in extra data are called with the row"""
-        fp = self._file_path("albums.xlsx")
+        fp = file_path("albums.xlsx")
 
         def test_fn(row):
             self.assertIsInstance(row, dict)
 
         sheet = AlbumSheet(path=fp, extra_data={"test_fn": test_fn})
         sheet.load()
```

### Comparing `superspreader-0.2.6/tests/test_sheet.py` & `superspreader-0.2.7/tests/test_sheet.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,17 +3,25 @@
 # setup.py that excludes installing the "tests" package
 
 import unittest
 
 from superspreader import fields
 from superspreader.exceptions import ImproperlyConfigured
 from superspreader.sheets import BaseSheet
+from tests import file_path
 
 
-class TestSheet(unittest.TestCase):
+class ContactSheet(BaseSheet):
+    sheet_name = "Contacts"
+
+    id = fields.CharField(source="ID", unique=True)
+    name = fields.CharField(source="Name")
+
+
+class SheetTestCase(unittest.TestCase):
     def test_sheet_name(self):
         class AlbumSheet(BaseSheet):
             pass
 
         with self.assertRaises(ImproperlyConfigured):
             AlbumSheet(path="test")
 
@@ -39,7 +47,21 @@
         class BSheet(ASheet):
             pass
 
         sheet = BSheet(path="test")
         sheet_fields = sheet._build_fields()
 
         self.assertTrue("a_field" in sheet_fields)
+
+    def test_unique_violation(self):
+        """
+        Tests whether unique fields are validate properly
+        """
+        path = file_path("contacts_duplicates.xlsx")
+        sheet = ContactSheet(path)
+        sheet.load()
+
+        self.assertEqual(len(sheet.errors), 1)
+        self.assertEqual(
+            sheet.errors[0],
+            "“ID” must contain unique values only, but “1” occurs 1 times",
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

