# Comparing `tmp/importer-local-0.0.6.tar.gz` & `tmp/importer-local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importer-local-0.0.6.tar", last modified: Wed May 24 02:09:08 2023, max compression
+gzip compressed data, was "importer-local-0.0.7.tar", last modified: Tue Jul 18 08:43:19 2023, max compression
```

## Comparing `importer-local-0.0.6.tar` & `importer-local-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:09:08.513712 importer-local-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:09:08.513712 importer-local-0.0.6/CirclesImporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:08:57.000000 importer-local-0.0.6/CirclesImporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-24 02:08:57.000000 importer-local-0.0.6/CirclesImporter/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-24 02:09:08.513712 importer-local-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-24 02:08:57.000000 importer-local-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:09:08.513712 importer-local-0.0.6/importer_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-24 02:09:08.000000 importer-local-0.0.6/importer_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-24 02:09:08.000000 importer-local-0.0.6/importer_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:09:08.000000 importer-local-0.0.6/importer_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 02:09:08.000000 importer-local-0.0.6/importer_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:09:08.513712 importer-local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-24 02:08:57.000000 importer-local-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:09:08.513712 importer-local-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-24 02:08:57.000000 importer-local-0.0.6/tests/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:19.556270 importer-local-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:19.556270 importer-local-0.0.7/CirclesImporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:02.000000 importer-local-0.0.7/CirclesImporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-18 08:43:02.000000 importer-local-0.0.7/CirclesImporter/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 08:43:19.556270 importer-local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 08:43:02.000000 importer-local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:19.556270 importer-local-0.0.7/importer_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 08:43:19.000000 importer-local-0.0.7/importer_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-18 08:43:19.000000 importer-local-0.0.7/importer_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:43:19.000000 importer-local-0.0.7/importer_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 08:43:19.000000 importer-local-0.0.7/importer_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:43:19.556270 importer-local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-18 08:43:02.000000 importer-local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:43:19.556270 importer-local-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-18 08:43:02.000000 importer-local-0.0.7/tests/test_importer.py
```

### Comparing `importer-local-0.0.6/CirclesImporter/importer.py` & `importer-local-0.0.7/CirclesImporter/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from circles_local_database_python.database import database
-from opencage_get_country_name import Country
+from CirclesGetCountryName.opencage_get_country_name import Country
 from dotenv import load_dotenv
-from CirclesLocalLoggerPython.LoggerServiceSingleton import locallgr
+from LoggerLocalPythonPackage.LocalLogger import _Local_Logger
 from functools import wraps
 load_dotenv()
 
 
 def log_function_execution(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         start_message = "Function %s started." % func.__name__
-        locallgr.log(start_message)
+        _Local_Logger.start(start_message)
 
         result = func(*args, **kwargs)  # Execute the function
 
         finish_message = "Function %s completed." % func.__name__
-        locallgr.log(finish_message)
+        _Local_Logger.end(finish_message)
         return result
     return wrapper
 
 
 class Importer:
     def __init__(self, source):
         self.source_name = source
@@ -43,15 +43,15 @@
             query_entity_ml = "INSERT INTO {}(`entity_type_name`,`entity_type_id`,`lang_code`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, %s, 1, 1)".format('entity_type.entity_type_ml_table')
             cursor.execute(query_entity_ml, (entity_type_name, last_inserted_id, 'en'))
 
             db.commit()
         else:
             source_message = "Entity %s already exist." % entity_type_name
-            locallgr.log(source_message)
+            _Local_Logger.end(source_message)
         db.close()
 
     @log_function_execution
     def insert_new_source(self):
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
@@ -69,15 +69,15 @@
             query_importer_source_ml = "INSERT INTO {}(`source_name`,`source_id`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, 1, 1)".format('source.source_ml_table')
             cursor.execute(query_importer_source_ml, (self.source_name, last_inserted_id))
 
             db.commit()
         else:
             source_message = "Source %s already exist." % self.source_name
-            locallgr.log(source_message)
+            _Local_Logger.end(source_message)
         db.close()
 
     @log_function_execution
     def insert_record_source(self, location, entity_type_name, entity_id, url):
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
```

### Comparing `importer-local-0.0.6/README.md` & `importer-local-0.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,9 +15,12 @@
 
 # Update the serverless.yml in the root directory
 provider:
   stage: play1
   
 Update the endpoints in serverless.yml
 
-To access the OpenCage API, you can visit the following website: 
-https://opencagedata.com/
+To access the OpenCage API:
+1. visit the following website: https://opencagedata.com/
+2. sign up to the service.
+3. you can retrive access token in quick_start 
+
```

### Comparing `importer-local-0.0.6/setup.py` & `importer-local-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix)
      name='importer-local',  
-     version='0.0.6',
+     version='0.0.7',
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles <project-name> Local/Remote Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
```

### Comparing `importer-local-0.0.6/tests/test_importer.py` & `importer-local-0.0.7/tests/test_importer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,31 @@
 import unittest
-from unittest.mock import MagicMock
-from importer import Importer
-from unittest.mock import patch
+from unittest.mock import MagicMock, patch
+import sys
+import os
+from LoggerLocalPythonPackage.LocalLogger import _Local_Logger
+# Add the parent directory to the sys.path
+parent_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
+sys.path.append(parent_dir)
+# Import the correct module from the CirclesImporter package
+from CirclesImporter import importer
 
 
 class TestImporter(unittest.TestCase):
     def setUp(self):
-        self.importer = Importer(source="TestSource")
+        self.importer = importer.Importer(source="TestSource")
         self.database_mock = MagicMock()
 
-    def test_get_country_id(self):
-        geocoder_mock = MagicMock()
-        geocoder_mock.geocode.return_value = [
-            {
-                'components': {
-                    'country': 'United States',
-                    'country_code': 'US'
-                }
-            }
-        ]
-        self.importer.geocoder = geocoder_mock
-
-        country_id = self.importer.get_country_id('New York')
-        self.assertEqual(country_id, 'United States')
-
-    @patch('importer.database')
+    @patch('CirclesImporter.importer.database')
     def test_insert_new_entity(self, database_mock):
         entity_type_name = "TestEntity"
-
         cursor_mock = MagicMock()
         cursor_mock.fetchone.return_value = None
         cursor_mock.lastrowid = 1
-
+        _Local_Logger.info(os.getenv("OPENCAGE_KEY"))
         database_mock.return_value.connect_to_database.return_value.cursor.return_value = cursor_mock
         self.importer.database = database_mock
         self.importer.insert_new_entity(entity_type_name)
 
         expected_query_entity = "INSERT INTO entity_type.entity_type_table(`created_user_id`,`updated_user_id`) VALUES (1, 1)"
         expected_query_entity_ml = "INSERT INTO entity_type.entity_type_ml_table(`entity_type_name`,`entity_type_id`,`lang_code`,`created_user_id`,`updated_user_id`) VALUES (%s, %s, %s, 1, 1)"
 
@@ -43,41 +33,39 @@
         cursor_mock.execute.assert_any_call(expected_query_entity_ml, (entity_type_name, 1, 'en'))
         assert cursor_mock.execute.call_count >= 2
         try:
             database_mock.return_value.commit.assert_called()
         except AssertionError:
             database_mock.return_value.commit.assert_not_called()
 
-    @patch('importer.database')
+    @patch('CirclesImporter.importer.database')
     def test_insert_new_source(self, database_mock):
         cursor_mock = MagicMock()
         cursor_mock.fetchone.return_value = None
         cursor_mock.lastrowid = 1
-
         database_mock.return_value.connect_to_database.return_value.cursor.return_value = cursor_mock
         self.importer.database = database_mock
         self.importer.insert_new_source()
 
         expected_query_importer_source = "INSERT INTO source.source_table(`created_user_id`,`updated_user_id`) VALUES (1, 1)"
         expected_query_importer_source_ml = "INSERT INTO source.source_ml_table(`source_name`,`source_id`,`created_user_id`,`updated_user_id`) VALUES (%s, %s, 1, 1)"
         cursor_mock.execute.assert_any_call(expected_query_importer_source)
         cursor_mock.execute.assert_any_call(expected_query_importer_source_ml, ("TestSource", 1))
         assert cursor_mock.execute.call_count >= 2
         try:
             database_mock.return_value.commit.assert_called()
         except AssertionError:
             database_mock.return_value.commit.assert_not_called()
 
-    @patch('importer.database')
-    def test_insert_record_source(self,database_mock):
+    @patch('CirclesImporter.importer.database')
+    def test_insert_record_source(self, database_mock):
         location = "New York"
         entity_type_name = "TestEntity"
         entity_id = 1
         url = "https://example.com"
-
         cursor_mock = MagicMock()
         cursor_mock.fetchone.side_effect = [(1,), (2,), (3,)]
         database_mock.return_value.connect_to_database.return_value.cursor.return_value = cursor_mock
 
         self.importer.get_country_id = MagicMock(return_value="United States")
         self.importer.database = database_mock
         self.importer.insert_record_source(location, entity_type_name, entity_id, url)
```

