# Comparing `tmp/influxdb3-python-0.1.9.tar.gz` & `tmp/influxdb3-python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.1.9.tar", last modified: Thu Jul 13 11:25:05 2023, max compression
+gzip compressed data, was "influxdb3-python-0.2.0.tar", last modified: Tue Jul 18 14:10:15 2023, max compression
```

## Comparing `influxdb3-python-0.1.9.tar` & `influxdb3-python-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/influxdb_client_3/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/influxdb_client_3/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.1.9/LICENSE` & `influxdb3-python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.9/PKG-INFO` & `influxdb3-python-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.9
+Version: 0.2.0
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `influxdb3-python-0.1.9/README.md` & `influxdb3-python-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.9/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.2.0/influxdb3_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.9
+Version: 0.2.0
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `influxdb3-python-0.1.9/influxdb_client_3/__init__.py` & `influxdb3-python-0.2.0/influxdb_client_3/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,46 @@
-import json
-import urllib.parse
+import urllib.parse, json
 import pyarrow as pa
 from influxdb_client import InfluxDBClient as _InfluxDBClient, WriteOptions, Point
 from influxdb_client.client.write_api import WriteApi as _WriteApi, SYNCHRONOUS, ASYNCHRONOUS, PointSettings
 from influxdb_client.domain.write_precision import WritePrecision
 from influxdb_client.client.exceptions import InfluxDBError
 from pyarrow.flight import FlightClient, Ticket, FlightCallOptions
-from influxdb_client_3.read_file import upload_file
+from influxdb_client_3.read_file import UploadFile
 
 
 def write_client_options(**kwargs):
+    """
+    Function for providing additional arguments for the WriteApi client.
+
+    :param kwargs: Additional arguments for the WriteApi client.
+    :return: dict with the arguments.
+    """
     return kwargs
 
 def default_client_options(**kwargs):
     return kwargs
 
 def flight_client_options(**kwargs):
-    return kwargs  # You can replace this with a specific data structure if needed
+    """
+    Function for providing additional arguments for the FlightClient.
+
+    :param kwargs: Additional arguments for the FlightClient.
+    :return: dict with the arguments.
+    """
+    return kwargs
+
+def file_parser_options(**kwargs):
+    """
+    Function for providing additional arguments for the file parser.
+
+    :param kwargs: Additional arguments for the file parser.
+    :return: dict with the arguments.
+    """
+    return kwargs  
 
 
 class InfluxDBClient3:
     def __init__(
             self,
             host=None,
             org=None,
@@ -36,21 +56,21 @@
         :type host: str
         :param org: The InfluxDB organization name for operations.
         :type org: str
         :param database: The database for InfluxDB operations.
         :type database: str
         :param token: The authentication token for accessing the InfluxDB server.
         :type token: str
-        :param write_client_options: Options for the WriteAPI.
-        :type write_client_options: dict
-        :param flight_client_options: Options for the FlightClient.
-        :type flight_client_options: dict
+        :param write_client_options: Function for providing additional arguments for the WriteApi client.
+        :type write_client_options: callable
+        :param flight_client_options: Function for providing additional arguments for the FlightClient.
+        :type flight_client_options: callable
         :param kwargs: Additional arguments for the InfluxDB Client.
         """
-        self._org = org
+        self._org = org if org is not None else "default"
         self._database = database
         self._token = token
         self._write_client_options = write_client_options if write_client_options is not None else default_client_options(write_options=SYNCHRONOUS)
 
         # Extracting the hostname from URL if provided
         parsed_url = urllib.parse.urlparse(host)
         host = parsed_url.hostname or host
@@ -68,45 +88,51 @@
 
 
     def write(self, record=None, database=None ,**kwargs):
         """
         Write data to InfluxDB.
 
         :param record: The data point(s) to write.
-        :type record: Point or list of Point objects
+        :type record: object or list of objects
+        :param database: The database to write to. If not provided, uses the database provided during initialization.
+        :type database: str
         :param kwargs: Additional arguments to pass to the write API.
         """
         if database is None:
             database = self._database
 
         try:
             self._write_api.write(bucket=database, record=record, **kwargs)
         except InfluxDBError as e:
             raise e
           
 
-    def write_file(self, file, measurement_name=None, tag_columns=None, timestamp_column='time', database=None, **kwargs):
+    def write_file(self, file, measurement_name=None, tag_columns=None, timestamp_column='time', database=None, file_parser_options=None ,**kwargs):
         """
         Write data from a file to InfluxDB.
 
         :param file: The file to write.
         :type file: str
         :param measurement_name: The name of the measurement.
         :type measurement_name: str
         :param tag_columns: Tag columns.
         :type tag_columns: list
         :param timestamp_column: Timestamp column name. Defaults to 'time'.
         :type timestamp_column: str
+        :param database: The database to write to. If not provided, uses the database provided during initialization.
+        :type database: str
+        :param file_parser_options: Function for providing additional arguments for the file parser.
+        :type file_parser_options: callable
         :param kwargs: Additional arguments to pass to the write API.
         """
         if database is None:
             database = self._database
 
         try:
-            table = upload_file(file).load_file()
+            table = UploadFile(file, file_parser_options).load_file()
             df = table.to_pandas() if isinstance(table, pa.Table) else table
             self._process_dataframe(df, measurement_name, tag_columns or [], timestamp_column, database=database, **kwargs)
         except Exception as e:
             raise e
             
 
     def _process_dataframe(self, df, measurement_name, tag_columns, timestamp_column, database, **kwargs):
@@ -134,18 +160,21 @@
 
     def query(self, query, language="sql", mode="all", database=None, **kwargs ):
         """
         Query data from InfluxDB.
 
         :param query: The query string.
         :type query: str
-        :param language: The query language (default is "sql").
+        :param language: The query language; "sql" or "influxql" (default is "sql").
         :type language: str
         :param mode: The mode of fetching data (all, pandas, chunk, reader, schema).
         :type mode: str
+        :param database: The database to query from. If not provided, uses the database provided during initialization.
+        :type database: str
+        :param kwargs: Additional arguments for the query.
         :return: The queried data.
         """
         if database is None:
             database = self._database
         
         try:
             # Create an authorization header
@@ -184,9 +213,10 @@
     "Point",
     "PointSettings",
     "SYNCHRONOUS",
     "ASYNCHRONOUS",
     "WritePrecision",
     "WriteOptions",
     "write_client_options",
-    "flight_client_options"
+    "flight_client_options",
+    "file_parser_options"
 ]
```

### Comparing `influxdb3-python-0.1.9/setup.py` & `influxdb3-python-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.9/tests/test_influxdb_client_3.py` & `influxdb3-python-0.2.0/tests/test_influxdb_client_3.py`

 * *Files identical despite different names*

