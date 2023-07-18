# Comparing `tmp/heps_ds_utils-0.4.7a7.tar.gz` & `tmp/heps_ds_utils-0.4.7a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heps_ds_utils-0.4.7a7.tar", max compression
+gzip compressed data, was "heps_ds_utils-0.4.7a8.tar", max compression
```

## Comparing `heps_ds_utils-0.4.7a7.tar` & `heps_ds_utils-0.4.7a8.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rwxr-xr-x   0        0        0     1068 2022-09-01 11:55:01.744801 heps_ds_utils-0.4.7a7/LICENSE
--rwxr-xr-x   0        0        0    14573 2022-12-11 18:10:56.592911 heps_ds_utils-0.4.7a7/README.md
--rwxr-xr-x   0        0        0      512 2022-12-09 05:15:00.108829 heps_ds_utils-0.4.7a7/heps_ds_utils/__init__.py
--rwxr-xr-x   0        0        0    11172 2022-12-11 19:13:24.791308 heps_ds_utils-0.4.7a7/heps_ds_utils/bigquery_operations.py
--rwxr-xr-x   0        0        0    13847 2022-12-09 05:15:00.119371 heps_ds_utils-0.4.7a7/heps_ds_utils/bucket_operations.py
--rwxr-xr-x   0        0        0    10180 2023-02-06 11:54:45.208078 heps_ds_utils-0.4.7a7/heps_ds_utils/elastic_operations.py
--rwxr-xr-x   0        0        0    15822 2022-12-09 05:15:00.121133 heps_ds_utils-0.4.7a7/heps_ds_utils/hive_operations.py
--rwxr-xr-x   0        0        0      198 2022-09-01 11:55:01.755733 heps_ds_utils-0.4.7a7/heps_ds_utils/http_request_operations.py
--rwxr-xr-x   0        0        0      183 2022-09-01 11:55:01.756457 heps_ds_utils-0.4.7a7/heps_ds_utils/kafka_operations.py
--rwxr-xr-x   0        0        0     4048 2022-09-01 11:55:01.758186 heps_ds_utils-0.4.7a7/heps_ds_utils/logging_operations.py
--rwxr-xr-x   0        0        0    13717 2022-12-09 05:15:00.121947 heps_ds_utils-0.4.7a7/heps_ds_utils/mongo_operations.py
--rwxr-xr-x   0        0        0     2797 2022-09-01 11:55:01.759045 heps_ds_utils-0.4.7a7/heps_ds_utils/read_from_bq_file.py
--rwxr-xr-x   0        0        0      183 2022-09-01 11:55:01.759589 heps_ds_utils-0.4.7a7/heps_ds_utils/slack_operations.py
--rwxr-xr-x   0        0        0     2230 2023-02-06 11:54:54.709105 heps_ds_utils-0.4.7a7/pyproject.toml
--rw-r--r--   0        0        0    16315 1970-01-01 00:00:00.000000 heps_ds_utils-0.4.7a7/setup.py
--rw-r--r--   0        0        0    16058 1970-01-01 00:00:00.000000 heps_ds_utils-0.4.7a7/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2022-09-01 11:55:01.744801 heps_ds_utils-0.4.7a8/LICENSE
+-rwxr-xr-x   0        0        0    14573 2022-12-11 18:10:56.592911 heps_ds_utils-0.4.7a8/README.md
+-rwxr-xr-x   0        0        0      512 2022-12-09 05:15:00.108829 heps_ds_utils-0.4.7a8/heps_ds_utils/__init__.py
+-rwxr-xr-x   0        0        0    11172 2022-12-11 19:13:24.791308 heps_ds_utils-0.4.7a8/heps_ds_utils/bigquery_operations.py
+-rwxr-xr-x   0        0        0    13847 2022-12-09 05:15:00.119371 heps_ds_utils-0.4.7a8/heps_ds_utils/bucket_operations.py
+-rwxr-xr-x   0        0        0    10180 2023-02-06 12:18:55.687753 heps_ds_utils-0.4.7a8/heps_ds_utils/elastic_operations.py
+-rwxr-xr-x   0        0        0    15822 2022-12-09 05:15:00.121133 heps_ds_utils-0.4.7a8/heps_ds_utils/hive_operations.py
+-rwxr-xr-x   0        0        0      198 2022-09-01 11:55:01.755733 heps_ds_utils-0.4.7a8/heps_ds_utils/http_request_operations.py
+-rwxr-xr-x   0        0        0      183 2022-09-01 11:55:01.756457 heps_ds_utils-0.4.7a8/heps_ds_utils/kafka_operations.py
+-rwxr-xr-x   0        0        0     4048 2022-09-01 11:55:01.758186 heps_ds_utils-0.4.7a8/heps_ds_utils/logging_operations.py
+-rwxr-xr-x   0        0        0    13717 2022-12-09 05:15:00.121947 heps_ds_utils-0.4.7a8/heps_ds_utils/mongo_operations.py
+-rwxr-xr-x   0        0        0     2797 2022-09-01 11:55:01.759045 heps_ds_utils-0.4.7a8/heps_ds_utils/read_from_bq_file.py
+-rwxr-xr-x   0        0        0      183 2022-09-01 11:55:01.759589 heps_ds_utils-0.4.7a8/heps_ds_utils/slack_operations.py
+-rwxr-xr-x   0        0        0     2247 2023-07-18 08:39:18.901712 heps_ds_utils-0.4.7a8/pyproject.toml
+-rw-r--r--   0        0        0    16059 1970-01-01 00:00:00.000000 heps_ds_utils-0.4.7a8/PKG-INFO
```

### Comparing `heps_ds_utils-0.4.7a7/LICENSE` & `heps_ds_utils-0.4.7a8/LICENSE`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/README.md` & `heps_ds_utils-0.4.7a8/README.md`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/heps_ds_utils/__init__.py` & `heps_ds_utils-0.4.7a8/heps_ds_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/heps_ds_utils/bigquery_operations.py` & `heps_ds_utils-0.4.7a8/heps_ds_utils/bigquery_operations.py`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/heps_ds_utils/bucket_operations.py` & `heps_ds_utils-0.4.7a8/heps_ds_utils/bucket_operations.py`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/heps_ds_utils/elastic_operations.py` & `heps_ds_utils-0.4.7a8/heps_ds_utils/elastic_operations.py`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/heps_ds_utils/hive_operations.py` & `heps_ds_utils-0.4.7a8/heps_ds_utils/hive_operations.py`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/heps_ds_utils/logging_operations.py` & `heps_ds_utils-0.4.7a8/heps_ds_utils/logging_operations.py`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/heps_ds_utils/mongo_operations.py` & `heps_ds_utils-0.4.7a8/heps_ds_utils/mongo_operations.py`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/heps_ds_utils/read_from_bq_file.py` & `heps_ds_utils-0.4.7a8/heps_ds_utils/read_from_bq_file.py`

 * *Files identical despite different names*

### Comparing `heps_ds_utils-0.4.7a7/pyproject.toml` & `heps_ds_utils-0.4.7a8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heps_ds_utils"
-version = "0.4.7-alpha.7"
+version = "0.4.7-alpha.8"
 description = "A Module to enable Hepsiburada Data Science Team to utilize different tools."
 authors = ["FarukBuldur <faruk.buldur@hepsiburada.com>"]
 maintainers = ["FıratÖncü <firat.oncu@hepsiburada.com>", "AysenurKulunk <aysenur.kulunk@hepsiburada.com>", "HakanAtesli <hakan.atesli@hepsiburada.com>", "EnisTeper <enis.teper@hepsiburada.com>"]
 license = "MIT License"
 readme = "README.md"
 classifiers = [
     "Operating System :: MacOS",
@@ -12,42 +12,43 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">= 3.8, < 3.11"
 paramiko = "^2.10.3"
 scp = { version = "^0.14.4", optional = true }
 PyHive = { version = "^0.6.5", optional = true }
-pandas = "^1.4.1"
+pandas = ">=1.4.1, <=2.0.3"
 thrift = {version = "^0.15.0", optional = true }
 sasl = {version="^0.3.1", optional = true, markers = "sys_platform == 'linux' or sys_platform == 'darwin'"}
 thrift-sasl = {version = "^0.4.3", optional = true }
 colorama = "^0.4.4"
 google-cloud-bigquery = {extras = ["bqstorage", "pandas"], version = "^3.0.1"}
-tqdm = "^4.64.0"
+tqdm = "^4.42.0"
 google-cloud-logging = "^3.0.0"
 google-cloud-storage = "^2.5.0"
 elasticsearch = "7.17.7"
 pymongo = "^4.3.2"
 
-[tool.poetry.dev-dependencies]
+
+[tool.poetry.extras]
+hive = ["PyHive", "thrift", "thrift-sasl", "sasl", "scp"]
+
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.7.0"
 pylint = "^2.13.4"
 python-dotenv = "^0.20.0"
 ipykernel = "^6.13.0"
-black = "^22.3.0"
 pytest = "^7.1.2"
 jupyter = "^1.0.0"
 isort = "^5.10.1"
 flake8 = "^5.0.4"
 pre-commit = "^2.20.0"
 interrogate = "^1.5.0"
 
-[tool.poetry.extras]
-hive = ["PyHive", "thrift", "thrift-sasl", "sasl", "scp"]
-
-
 [tool.black]
 line-length = 79
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
 |   \.venv
```

### Comparing `heps_ds_utils-0.4.7a7/setup.py` & `heps_ds_utils-0.4.7a8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,430 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: heps-ds-utils
+Version: 0.4.7a8
+Summary: A Module to enable Hepsiburada Data Science Team to utilize different tools.
+License: MIT
+Author: FarukBuldur
+Author-email: faruk.buldur@hepsiburada.com
+Maintainer: FıratÖncü
+Maintainer-email: firat.oncu@hepsiburada.com
+Requires-Python: >=3.8,<3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: hive
+Requires-Dist: PyHive (>=0.6.5,<0.7.0) ; extra == "hive"
+Requires-Dist: colorama (>=0.4.4,<0.5.0)
+Requires-Dist: elasticsearch (==7.17.7)
+Requires-Dist: google-cloud-bigquery[bqstorage,pandas] (>=3.0.1,<4.0.0)
+Requires-Dist: google-cloud-logging (>=3.0.0,<4.0.0)
+Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0)
+Requires-Dist: pandas (>=1.4.1,<=2.0.3)
+Requires-Dist: paramiko (>=2.10.3,<3.0.0)
+Requires-Dist: pymongo (>=4.3.2,<5.0.0)
+Requires-Dist: sasl (>=0.3.1,<0.4.0) ; (sys_platform == "linux" or sys_platform == "darwin") and (extra == "hive")
+Requires-Dist: scp (>=0.14.4,<0.15.0) ; extra == "hive"
+Requires-Dist: thrift (>=0.15.0,<0.16.0) ; extra == "hive"
+Requires-Dist: thrift-sasl (>=0.4.3,<0.5.0) ; extra == "hive"
+Requires-Dist: tqdm (>=4.42.0,<5.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['heps_ds_utils']
+# Hepsiburada Data Science Utilities
 
-package_data = \
-{'': ['*']}
+This module includes utilities for Hepsiburada Data Science Team.
 
-install_requires = \
-['colorama>=0.4.4,<0.5.0',
- 'elasticsearch==7.17.7',
- 'google-cloud-bigquery[bqstorage,pandas]>=3.0.1,<4.0.0',
- 'google-cloud-logging>=3.0.0,<4.0.0',
- 'google-cloud-storage>=2.5.0,<3.0.0',
- 'pandas>=1.4.1,<2.0.0',
- 'paramiko>=2.10.3,<3.0.0',
- 'pymongo>=4.3.2,<5.0.0',
- 'tqdm>=4.64.0,<5.0.0']
-
-extras_require = \
-{'hive': ['scp>=0.14.4,<0.15.0',
-          'PyHive>=0.6.5,<0.7.0',
-          'thrift>=0.15.0,<0.16.0',
-          'thrift-sasl>=0.4.3,<0.5.0'],
- 'hive:sys_platform == "linux" or sys_platform == "darwin"': ['sasl>=0.3.1,<0.4.0']}
-
-setup_kwargs = {
-    'name': 'heps-ds-utils',
-    'version': '0.4.7a7',
-    'description': 'A Module to enable Hepsiburada Data Science Team to utilize different tools.',
-    'long_description': '# Hepsiburada Data Science Utilities\n\nThis module includes utilities for Hepsiburada Data Science Team.\n\n- Library is available via PyPi. \n- Library can be downloaded using pip as follows: `pip install heps-ds-utils`\n- Existing library can be upgraded using pip as follows: `pip install heps-ds-utils --upgrade`\n\n***\n## Available Modules\n\n1. Hive Operations\n\n```python\nfrom heps_ds_utils import HiveOperations\n\n# A connection is needed to be generated in a specific runtime.\n# There are 3 ways to set credentials for connection.\n\n# 1) Instance try to set default credentials from Environment Variables.\nhive_ds = HiveOperations()\nhive_ds.connect_to_hive()\n\n# 2) One can pass credentials to instance initiation to override default.\nhive_ds = HiveOperations(HIVE_HOST="XXX", HIVE_PORT="YYY", HIVE_USER="ZZZ", HIVE_PASS="WWW", HADOOP_EDGE_HOST="QQQ")\nhive_ds = HiveOperations(HIVE_USER="ZZZ", HIVE_PASS="WWW")\nhive_ds.connect_to_hive()\n\n# 3) One can change any of the credentials after initiation using appropriate attribute.\nhive_ds = HiveOperations()\nhive_ds.hive_username = \'XXX\'\nhive_ds.hive_password = \'YYY\'\nhive_ds.connect_to_hive()\n\n#\xa0Execute an SQL query to retrieve data.\n# Currently Implemented Types: DataFrame, Numpy Array, Dictionary, List.\nSQL_QUERY = "SELECT * FROM {db}.{table}"\ndata, columns = hive_ds.execute_query(SQL_QUERY, return_type="dataframe", return_columns=False)\n\n# Execute an SQL query to create and insert data into table.\nSQL_QUERY = "INSERT INTO .."\nhive_ds.create_insert_table(SQL_QUERY)\n\n# Send Files to Hive and Create a Table with the Data.\n# Currently DataFrame or Numpy Array can be sent to Hive.\n# While sending Numpy Array columns have to be provided.\nSQL_QUERY = "INSERT INTO .."\nhive_ds.send_files_to_hive("{db}.{table}", data, columns=None)\n\n# Close the connection at the end of the runtime.\n\nhive_ds.disconnect_from_hive()\n\n```\n\n2. BigQuery Operations\n\n```python\nfrom heps_ds_utils import BigQueryOperations, execute_from_bq_file\n\n# A connection is needed to be generated in a specific runtime.\n# There are 3 ways to set credentials for connection.\n\n# 1) Instance try to set default credentials from Environment Variables.\nbq_ds = BigQueryOperations()\n\n# 2) One can pass credentials to instance initiation to override default.\nbq_ds = BigQueryOperations(gcp_key_path="/tmp/keys/ds_qos.json")\n\n# Unlike HiveOperations, initiation creates a direct connection. Absence of\n# credentials will throw an error.\n\n#\xa0Execute an SQL query to retrieve data.\n# Currently Implemented Types: DataFrame.\nQUERY_STRING = """SELECT * FROM `[project_name].[dataset_name].[table_name]` LIMIT 20"""\ndata = bq_ds.execute_query(QUERY_STRING, return_type=\'dataframe\')\n\n#\xa0Create a Dataset in BigQuery.\nbq_ds.create_new_dataset("example_dataset")\n\n# Create a Table under a Dataset in BigQuery.\nschema = [\n    {"field_name": "id", "field_type": "INTEGER", "field_mode": "REQUIRED"},\n    {"field_name": "first_name", "field_type": "STRING", "field_mode": "REQUIRED"},\n    {"field_name": "last_name", "field_type": "STRING", "field_mode": "REQUIRED"},\n    {"field_name": "email", "field_type": "STRING", "field_mode": "REQUIRED"},\n    {"field_name": "gender", "field_type": "STRING", "field_mode": "REQUIRED"},\n    {"field_name": "ip_address", "field_type": "STRING", "field_mode": "REQUIRED"}]\n\nbq_ds.create_new_table(dataset=\'example_dataset\', table_name=\'mock_data\', schema=schema)\n\n# Insert into an existing Table from Dataframe.\n# Don\'t create and insert in the same runtime.\n# Google throws an error when creation and insertion time is close.\nbq_ds.insert_rows_into_existing_table(dataset=\'example_dataset\', table=\'mock_data\', data=df)\n\n# Delete a Table.\nbq_ds.delete_existing_table(\'example_dataset\', \'mock_data\')\n\n# Delete a Dataset.\n# Trying to delete a dataset consisting of tables will throw an error.\nbq_ds.delete_existing_dataset(\'example_dataset\')\n\n# Load Dataframe As a Table. BigQuery will infer the data types.\nbq_ds.load_data_to_table(\'example_dataset\', \'mock_data\', df, overwrite=False)\n\n# To execute BQ commands sequentially from a BigQuery Script without a return statement !\nexecute_from_bq_file(bq_client=bq_ds, bq_file_path="tests/test_data/test_case_2.bq", verbose=True)\n\n```\n\n3. Logging Operations\n\n```python\nfrom heps_ds_utils import LoggingOperations\n\n# A connection is needed to be generated in a specific runtime.\n# There are 3 ways to set credentials for connection.\n\n# 1) Instance try to set default credentials from Environment Variables.\nlogger_ds = LoggingOperations()\n\n# 2) One can pass credentials to instance initiation to override default.\nlogger_ds = LoggingOperations(gcp_key_path="/tmp/keys/ds_qos.json")\n\n# Unlike HiveOperations, initiation creates a direct connection. Absence of\n# credentials will throw an error.\n\n\n```\n\n4. Bucket Operations\n\n```python\nfrom heps_ds_utils import BucketOperations\n\n# A connection is needed to be generated in a specific runtime.\n# There are 2 ways to set credentials for connection.\n\n# 1) Instance try to set default credentials from Environment Variables.\nbct_ds = BucketOperations()\n\n# 2) One can pass credentials to instance initiation to override default.\nbct_ds = BucketOperations(gcp_key_path="/tmp/keys/ds_qos.json")\n\n# Unlike HiveOperations, initiation creates a direct connection. Absence of\n# credentials will throw an error.\n\nBUCKET_NAME = "bucket-name"\n\n# Upload File using filepath.\n# Blob name is the filepath you want the file to be under the bucket.\n# Filepath is the path to the file you want to upload.\nbct_ds.upload_from_filepath(BUCKET_NAME, "project_name/dev/data/output.csv", "data/output.csv")\n\n# Upload File from memory data.\n# If you want to save the data in memory to a file, you can use this function.\nbct_ds.upload_from_memory(BUCKET_NAME, "project_name/dev/model/model.pkl", model)\n\n# Download file from bucket to filepath.\nbct_ds.download_to_filepath(BUCKET_NAME, "project_name/dev/data/sample.json", "data/sample.json")\n\n# Download data from bucket to memory.\n# If you want to save the data in a file to memory, you can use this function.\nframe = bct_ds.download_to_memory(BUCKET_NAME, "project_name/dev/data/sample.csv", "dataframe")\n\n# Delete file from bucket.\nbct_ds.delete_file_from_bucket(BUCKET_NAME, "project_name/dev/data/sample.json")\n\n# Create empty folder to bucket.\nbct_ds.create_new_folders(BUCKET_NAME, "project_name/dev/data/")\n\nOVERWRITE = True/False\n# Download files from bucket recursively.\nbct_ds.download_recursively(BUCKET_NAME, "path/to/blob", OVERWRITE, "local/destination/path")\n\n# Upload files to bucket recursively\nbct_ds.upload_recursively(BUCKET_NAME, "path/to/blob", OVERWRITE, "local/source/path")\n\n# Check if blob already exists.\nbct_ds.does_blob_exist(BUCKET_NAME, \'path/to/blob\')\n\n```\n\n5. Elastic Operations\n```python\nfrom heps_ds_utils import ElasticOperations\n\n# A connection is needed to be generated in a specific runtime.\n# There are 2 ways to set credentials for connection.\n\n# 1) Instance try to set default credentials from Environment Variables.\nelastic_ds = ElasticOperations()\n\n# 2) One can pass credentials to instance initiation to override default.\nelastic_ds = ElasticOperations(ip="connetcion-ip", port="connection-port")\n\nINDEX_NAME = "index-name"\n\n# Get data count of index\ncount = elastic_ds.get_count(INDEX_NAME)\n\n# Adjust read only parameter of the index.\n# Prevent index from modifications.\nelastic_ds.adjust_readonly(INDEX_NAME, True)\n\n# Allow index to modifications\nelastic_ds.adjust_readonly(INDEX_NAME, False)\n\n# Recreate the index.\n# Deletes the index and generates new one with same name.\nelastic_ds.recreate_index(INDEX_NAME)\n\n# Upload data to index.\n# Example data\ndata = [{\'field-name1\' : [\'0000\', \'0001\', \'0002\'],\n        \'field-name2\' : \'2011-20-11\'},\n        {\'field-name1\' : [\'0003\', \'0002\', \'0001\', \'0000\'],\n        \'field-name2\' : \'2011-21-11\'}]\nelastic_ds.send_data_to_elastic(INDEX_NAME, data=data)\n\n# Get data from the index.\n# Currently Implemented Types: DataFrame.\ndata = elastic_ds.get_data_from_elastic(INDEX_NAME)\n\n# Run custom search query at ElasticSearch.\n# Implemented return methods: Hits-Hits (Default), Raw, Hits, Total, Value\nresult = elastic_ds.run_query(indexName=INDEX_NAME,\n                               return_method="raw",\n                               body={"query": {"match_all": {}}})\n                            \n```\n\n6. Mongo Operations\n```python\nfrom heps_ds_utils import MongoOperations\n# A connection is needed to be generated in a specific runtime.\n# There are 2 ways to set credentials for connection.\n\n# 1) One can pass connection string to instance initiation.\nmongo_ds = MongoOperations(connection_string="connection-string")\n\n# 2) One can pass ip and port credentials to instance initiation.\nmongo_ds = MongoOperations(ip="connetcion-ip", port=int("connection-port"))\n\nDATABASE_NAME = "database-name"\nCOLLECTION_NAME = "collection-name"\n\n# Create database\ndatabase = mongo_ds.create_database(DATABASE_NAME)\n\n# Create collection\ncollection = mongo_ds.create_collection(DATABASE_NAME, COLLECTION_NAME)\n\n# Get database\ndatabase = mongo_ds.get_database(DATABASE_NAME)\n\n# Get collection\ncollection = mongo_ds.get_collection(DATABASE_NAME, COLLECTION_NAME)\n\n# Get document count of collection.\n# filter parameter is optional\ncount = mongo_ds.get_count(DATABASE_NAME, COLLECTION_NAME, filter=\'filter\')\n\n# Find documents in collection\n# filter, sort and limit parameters are optional.\n# Currently Implemented Types: List of dictionaries, DataFrame\ndocuments = mongo_ds.find_document(database_name=DATABASE_NAME,\n                                   collection_name=COLLECTION_NAME,\n                                   filter=\'filter\',\n                                   sort=\'sort\',\n                                   limit=\'limit\')\n\n# Insert Document\n# Currently Implemented Types: Dictionary, Records (List of Dictionaries), DataFrame\nmongo_ds.insert_document(database_name=DATABASE_NAME,\n                        collection_name=COLLECTION_NAME,\n                        data=\'data\')\n\n# Update Document\nmongo_ds.update_document(database_name=DATABASE_NAME,\n                         collection_name=COLLECTION_NAME,\n                         filter=\'filter\',\n                         new_values=\'new-values\')\n\n# Delete Document\nmongo_ds.delete_document(database_name=DATABASE_NAME,\n                         collection_name=COLLECTION_NAME,\n                         filter=\'filter\')\n\n# Drop Database\nmongo_ds.drop_database(database_name=DATABASE_NAME)\n\n# Drop Collection\nmongo_ds.drop_collection(database_name=DATABASE_NAME,\n                         collection_name=COLLECTION_NAME)\n                         \n```\n\nRelease Notes:\n\n0.4.4:\n- BigQueryOperations:\n    - insert_rows_into_existing_table: insertion exception handling added.\n    - insert_rows_into_existing_table: retry added. \n        - Put time between table creation and insertion.\n    - execute_query: total_bytes_processed info added.\n    - execute_query: max allowed total_bytes_processed set to 100GB.\n    - execute_query: return_type=None for Queries w/o any return.\n    - load_data_to_table: kwargs[\'overwrite\'] is added.\n        - load_data_to_table(..., overwrite=True) to overwrite to table.\n        - load_data_to_table(..., overwrite=False) to append to table.\n        - not passing overwrite kwarg will print a DeprecationWarning.\n    - execute_from_bq_file: sequential execution of BigQuery commands from\n    a file. It has its own parser. \n        - execute_from_bq_file(..., verbose=True) to print BigQuery commands to console.\n        - execute_from_bq_file(..., verbose=False) not to print BigQuery commands to console.\n\n0.4.5:\n- LoggingOperations\n    - Bug Fix in Authentication to GCP Logging !\n- BigQueryOperations\n    - Executing BQ files for different environments !\n\n0.4.6:\n- BigQueryOperations\n    - BQ Parser bug fix !\n    - BQ File Execution dependent queries\n        - Some of the queries depends on the previous command executions. For these cases:\n        dependent_queries is needed to be set to True !\n        execute_from_bq_file(\n            bq_ds,\n            "tests/test_data/test_case_4.bq",\n            verbose=True,\n            config=configs,\n            dependent_queries=True)\n    - BQ Create Table Results in Empty Table Check Added!\n        - Raises an error if CREATE TABLE ... SELECT AS ... query results in empty table.\n        - This doesn\'t work in the case of dependent_queries=True !!!\n    - 100GB limit is turned into a warning, which will not be displayed in prod env.\n    - BQ Return Types Implemented (Numpy Array and Arrow Formats)\n- LoggingOperations\n    - protobuf dependency issue resolved!\n- BucketOperations\n    - upload_from_filepath function added.\n    - upload_from_memory function added.\n    - download_to_filepath function added.\n    - download_to_memory function added.\n    - delete_file_from_bucket function added.\n    - create_new_folders function added.\n    - delete_folder function added.\n\n0.4.7\n- ElasticOperations\n    - create_client function added.\n    - get_count function added.\n    - set_max_result_window function added.\n    - check_readonly function added.\n    - nonreadonly function added.\n    - readonly function added.\n    - adjust_readonly function added.\n    - create_index function added.\n    - delete_index function added.\n    - recreate_index function added.\n    - send_data_to_elastic function added.\n    - get_data_from_elastic function added.\n    - run_query function added.\n- MongoOperations\n    - create_client function added.\n    - show_databases function added.\n    - show_collections function added.\n    - create_database function added.\n    - create_collection function added.\n    - get_database function added.\n    - get_collection function added.\n    - get_count function added.\n    - find_document function added.\n    - insert_document function added.\n    - update_document function added. \n    - delete_document function added.\n    - drop_database function added.\n    - drop_collection function added.\n- BigQueryOperations\n    - execute_query: return_type="records" (list of dictionaries) implemented.\n    - Different Region connection implemented.\n- HiveOperations\n    - MAJOR UPDATE: HiveOperations are now in extras.\n    - If you want to install extra hive dependencies \n    - poetry add heps-ds-utils=^0.4.7a3 -extras hive\n- BucketOperations\n    - upload_from_filepath: uploaded file and source file size check added.\n    - download_to_filepath: zip extraction added.\n    - download_recursively function added.\n    - upload_recursively function added.\n    - does_blob_exist function added.\n',
-    'author': 'FarukBuldur',
-    'author_email': 'faruk.buldur@hepsiburada.com',
-    'maintainer': 'FıratÖncü',
-    'maintainer_email': 'firat.oncu@hepsiburada.com',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<3.11',
-}
+- Library is available via PyPi. 
+- Library can be downloaded using pip as follows: `pip install heps-ds-utils`
+- Existing library can be upgraded using pip as follows: `pip install heps-ds-utils --upgrade`
 
+***
+## Available Modules
+
+1. Hive Operations
+
+```python
+from heps_ds_utils import HiveOperations
+
+# A connection is needed to be generated in a specific runtime.
+# There are 3 ways to set credentials for connection.
+
+# 1) Instance try to set default credentials from Environment Variables.
+hive_ds = HiveOperations()
+hive_ds.connect_to_hive()
+
+# 2) One can pass credentials to instance initiation to override default.
+hive_ds = HiveOperations(HIVE_HOST="XXX", HIVE_PORT="YYY", HIVE_USER="ZZZ", HIVE_PASS="WWW", HADOOP_EDGE_HOST="QQQ")
+hive_ds = HiveOperations(HIVE_USER="ZZZ", HIVE_PASS="WWW")
+hive_ds.connect_to_hive()
+
+# 3) One can change any of the credentials after initiation using appropriate attribute.
+hive_ds = HiveOperations()
+hive_ds.hive_username = 'XXX'
+hive_ds.hive_password = 'YYY'
+hive_ds.connect_to_hive()
+
+# Execute an SQL query to retrieve data.
+# Currently Implemented Types: DataFrame, Numpy Array, Dictionary, List.
+SQL_QUERY = "SELECT * FROM {db}.{table}"
+data, columns = hive_ds.execute_query(SQL_QUERY, return_type="dataframe", return_columns=False)
+
+# Execute an SQL query to create and insert data into table.
+SQL_QUERY = "INSERT INTO .."
+hive_ds.create_insert_table(SQL_QUERY)
+
+# Send Files to Hive and Create a Table with the Data.
+# Currently DataFrame or Numpy Array can be sent to Hive.
+# While sending Numpy Array columns have to be provided.
+SQL_QUERY = "INSERT INTO .."
+hive_ds.send_files_to_hive("{db}.{table}", data, columns=None)
+
+# Close the connection at the end of the runtime.
+
+hive_ds.disconnect_from_hive()
+
+```
+
+2. BigQuery Operations
+
+```python
+from heps_ds_utils import BigQueryOperations, execute_from_bq_file
+
+# A connection is needed to be generated in a specific runtime.
+# There are 3 ways to set credentials for connection.
+
+# 1) Instance try to set default credentials from Environment Variables.
+bq_ds = BigQueryOperations()
+
+# 2) One can pass credentials to instance initiation to override default.
+bq_ds = BigQueryOperations(gcp_key_path="/tmp/keys/ds_qos.json")
+
+# Unlike HiveOperations, initiation creates a direct connection. Absence of
+# credentials will throw an error.
+
+# Execute an SQL query to retrieve data.
+# Currently Implemented Types: DataFrame.
+QUERY_STRING = """SELECT * FROM `[project_name].[dataset_name].[table_name]` LIMIT 20"""
+data = bq_ds.execute_query(QUERY_STRING, return_type='dataframe')
+
+# Create a Dataset in BigQuery.
+bq_ds.create_new_dataset("example_dataset")
+
+# Create a Table under a Dataset in BigQuery.
+schema = [
+    {"field_name": "id", "field_type": "INTEGER", "field_mode": "REQUIRED"},
+    {"field_name": "first_name", "field_type": "STRING", "field_mode": "REQUIRED"},
+    {"field_name": "last_name", "field_type": "STRING", "field_mode": "REQUIRED"},
+    {"field_name": "email", "field_type": "STRING", "field_mode": "REQUIRED"},
+    {"field_name": "gender", "field_type": "STRING", "field_mode": "REQUIRED"},
+    {"field_name": "ip_address", "field_type": "STRING", "field_mode": "REQUIRED"}]
+
+bq_ds.create_new_table(dataset='example_dataset', table_name='mock_data', schema=schema)
+
+# Insert into an existing Table from Dataframe.
+# Don't create and insert in the same runtime.
+# Google throws an error when creation and insertion time is close.
+bq_ds.insert_rows_into_existing_table(dataset='example_dataset', table='mock_data', data=df)
+
+# Delete a Table.
+bq_ds.delete_existing_table('example_dataset', 'mock_data')
+
+# Delete a Dataset.
+# Trying to delete a dataset consisting of tables will throw an error.
+bq_ds.delete_existing_dataset('example_dataset')
+
+# Load Dataframe As a Table. BigQuery will infer the data types.
+bq_ds.load_data_to_table('example_dataset', 'mock_data', df, overwrite=False)
+
+# To execute BQ commands sequentially from a BigQuery Script without a return statement !
+execute_from_bq_file(bq_client=bq_ds, bq_file_path="tests/test_data/test_case_2.bq", verbose=True)
+
+```
+
+3. Logging Operations
+
+```python
+from heps_ds_utils import LoggingOperations
+
+# A connection is needed to be generated in a specific runtime.
+# There are 3 ways to set credentials for connection.
+
+# 1) Instance try to set default credentials from Environment Variables.
+logger_ds = LoggingOperations()
+
+# 2) One can pass credentials to instance initiation to override default.
+logger_ds = LoggingOperations(gcp_key_path="/tmp/keys/ds_qos.json")
+
+# Unlike HiveOperations, initiation creates a direct connection. Absence of
+# credentials will throw an error.
+
+
+```
+
+4. Bucket Operations
+
+```python
+from heps_ds_utils import BucketOperations
+
+# A connection is needed to be generated in a specific runtime.
+# There are 2 ways to set credentials for connection.
+
+# 1) Instance try to set default credentials from Environment Variables.
+bct_ds = BucketOperations()
+
+# 2) One can pass credentials to instance initiation to override default.
+bct_ds = BucketOperations(gcp_key_path="/tmp/keys/ds_qos.json")
+
+# Unlike HiveOperations, initiation creates a direct connection. Absence of
+# credentials will throw an error.
+
+BUCKET_NAME = "bucket-name"
+
+# Upload File using filepath.
+# Blob name is the filepath you want the file to be under the bucket.
+# Filepath is the path to the file you want to upload.
+bct_ds.upload_from_filepath(BUCKET_NAME, "project_name/dev/data/output.csv", "data/output.csv")
+
+# Upload File from memory data.
+# If you want to save the data in memory to a file, you can use this function.
+bct_ds.upload_from_memory(BUCKET_NAME, "project_name/dev/model/model.pkl", model)
+
+# Download file from bucket to filepath.
+bct_ds.download_to_filepath(BUCKET_NAME, "project_name/dev/data/sample.json", "data/sample.json")
+
+# Download data from bucket to memory.
+# If you want to save the data in a file to memory, you can use this function.
+frame = bct_ds.download_to_memory(BUCKET_NAME, "project_name/dev/data/sample.csv", "dataframe")
+
+# Delete file from bucket.
+bct_ds.delete_file_from_bucket(BUCKET_NAME, "project_name/dev/data/sample.json")
+
+# Create empty folder to bucket.
+bct_ds.create_new_folders(BUCKET_NAME, "project_name/dev/data/")
+
+OVERWRITE = True/False
+# Download files from bucket recursively.
+bct_ds.download_recursively(BUCKET_NAME, "path/to/blob", OVERWRITE, "local/destination/path")
+
+# Upload files to bucket recursively
+bct_ds.upload_recursively(BUCKET_NAME, "path/to/blob", OVERWRITE, "local/source/path")
+
+# Check if blob already exists.
+bct_ds.does_blob_exist(BUCKET_NAME, 'path/to/blob')
+
+```
+
+5. Elastic Operations
+```python
+from heps_ds_utils import ElasticOperations
+
+# A connection is needed to be generated in a specific runtime.
+# There are 2 ways to set credentials for connection.
+
+# 1) Instance try to set default credentials from Environment Variables.
+elastic_ds = ElasticOperations()
+
+# 2) One can pass credentials to instance initiation to override default.
+elastic_ds = ElasticOperations(ip="connetcion-ip", port="connection-port")
+
+INDEX_NAME = "index-name"
+
+# Get data count of index
+count = elastic_ds.get_count(INDEX_NAME)
+
+# Adjust read only parameter of the index.
+# Prevent index from modifications.
+elastic_ds.adjust_readonly(INDEX_NAME, True)
+
+# Allow index to modifications
+elastic_ds.adjust_readonly(INDEX_NAME, False)
+
+# Recreate the index.
+# Deletes the index and generates new one with same name.
+elastic_ds.recreate_index(INDEX_NAME)
+
+# Upload data to index.
+# Example data
+data = [{'field-name1' : ['0000', '0001', '0002'],
+        'field-name2' : '2011-20-11'},
+        {'field-name1' : ['0003', '0002', '0001', '0000'],
+        'field-name2' : '2011-21-11'}]
+elastic_ds.send_data_to_elastic(INDEX_NAME, data=data)
+
+# Get data from the index.
+# Currently Implemented Types: DataFrame.
+data = elastic_ds.get_data_from_elastic(INDEX_NAME)
+
+# Run custom search query at ElasticSearch.
+# Implemented return methods: Hits-Hits (Default), Raw, Hits, Total, Value
+result = elastic_ds.run_query(indexName=INDEX_NAME,
+                               return_method="raw",
+                               body={"query": {"match_all": {}}})
+                            
+```
+
+6. Mongo Operations
+```python
+from heps_ds_utils import MongoOperations
+# A connection is needed to be generated in a specific runtime.
+# There are 2 ways to set credentials for connection.
+
+# 1) One can pass connection string to instance initiation.
+mongo_ds = MongoOperations(connection_string="connection-string")
+
+# 2) One can pass ip and port credentials to instance initiation.
+mongo_ds = MongoOperations(ip="connetcion-ip", port=int("connection-port"))
+
+DATABASE_NAME = "database-name"
+COLLECTION_NAME = "collection-name"
+
+# Create database
+database = mongo_ds.create_database(DATABASE_NAME)
+
+# Create collection
+collection = mongo_ds.create_collection(DATABASE_NAME, COLLECTION_NAME)
+
+# Get database
+database = mongo_ds.get_database(DATABASE_NAME)
+
+# Get collection
+collection = mongo_ds.get_collection(DATABASE_NAME, COLLECTION_NAME)
+
+# Get document count of collection.
+# filter parameter is optional
+count = mongo_ds.get_count(DATABASE_NAME, COLLECTION_NAME, filter='filter')
+
+# Find documents in collection
+# filter, sort and limit parameters are optional.
+# Currently Implemented Types: List of dictionaries, DataFrame
+documents = mongo_ds.find_document(database_name=DATABASE_NAME,
+                                   collection_name=COLLECTION_NAME,
+                                   filter='filter',
+                                   sort='sort',
+                                   limit='limit')
+
+# Insert Document
+# Currently Implemented Types: Dictionary, Records (List of Dictionaries), DataFrame
+mongo_ds.insert_document(database_name=DATABASE_NAME,
+                        collection_name=COLLECTION_NAME,
+                        data='data')
+
+# Update Document
+mongo_ds.update_document(database_name=DATABASE_NAME,
+                         collection_name=COLLECTION_NAME,
+                         filter='filter',
+                         new_values='new-values')
+
+# Delete Document
+mongo_ds.delete_document(database_name=DATABASE_NAME,
+                         collection_name=COLLECTION_NAME,
+                         filter='filter')
+
+# Drop Database
+mongo_ds.drop_database(database_name=DATABASE_NAME)
+
+# Drop Collection
+mongo_ds.drop_collection(database_name=DATABASE_NAME,
+                         collection_name=COLLECTION_NAME)
+                         
+```
+
+Release Notes:
+
+0.4.4:
+- BigQueryOperations:
+    - insert_rows_into_existing_table: insertion exception handling added.
+    - insert_rows_into_existing_table: retry added. 
+        - Put time between table creation and insertion.
+    - execute_query: total_bytes_processed info added.
+    - execute_query: max allowed total_bytes_processed set to 100GB.
+    - execute_query: return_type=None for Queries w/o any return.
+    - load_data_to_table: kwargs['overwrite'] is added.
+        - load_data_to_table(..., overwrite=True) to overwrite to table.
+        - load_data_to_table(..., overwrite=False) to append to table.
+        - not passing overwrite kwarg will print a DeprecationWarning.
+    - execute_from_bq_file: sequential execution of BigQuery commands from
+    a file. It has its own parser. 
+        - execute_from_bq_file(..., verbose=True) to print BigQuery commands to console.
+        - execute_from_bq_file(..., verbose=False) not to print BigQuery commands to console.
+
+0.4.5:
+- LoggingOperations
+    - Bug Fix in Authentication to GCP Logging !
+- BigQueryOperations
+    - Executing BQ files for different environments !
+
+0.4.6:
+- BigQueryOperations
+    - BQ Parser bug fix !
+    - BQ File Execution dependent queries
+        - Some of the queries depends on the previous command executions. For these cases:
+        dependent_queries is needed to be set to True !
+        execute_from_bq_file(
+            bq_ds,
+            "tests/test_data/test_case_4.bq",
+            verbose=True,
+            config=configs,
+            dependent_queries=True)
+    - BQ Create Table Results in Empty Table Check Added!
+        - Raises an error if CREATE TABLE ... SELECT AS ... query results in empty table.
+        - This doesn't work in the case of dependent_queries=True !!!
+    - 100GB limit is turned into a warning, which will not be displayed in prod env.
+    - BQ Return Types Implemented (Numpy Array and Arrow Formats)
+- LoggingOperations
+    - protobuf dependency issue resolved!
+- BucketOperations
+    - upload_from_filepath function added.
+    - upload_from_memory function added.
+    - download_to_filepath function added.
+    - download_to_memory function added.
+    - delete_file_from_bucket function added.
+    - create_new_folders function added.
+    - delete_folder function added.
+
+0.4.7
+- ElasticOperations
+    - create_client function added.
+    - get_count function added.
+    - set_max_result_window function added.
+    - check_readonly function added.
+    - nonreadonly function added.
+    - readonly function added.
+    - adjust_readonly function added.
+    - create_index function added.
+    - delete_index function added.
+    - recreate_index function added.
+    - send_data_to_elastic function added.
+    - get_data_from_elastic function added.
+    - run_query function added.
+- MongoOperations
+    - create_client function added.
+    - show_databases function added.
+    - show_collections function added.
+    - create_database function added.
+    - create_collection function added.
+    - get_database function added.
+    - get_collection function added.
+    - get_count function added.
+    - find_document function added.
+    - insert_document function added.
+    - update_document function added. 
+    - delete_document function added.
+    - drop_database function added.
+    - drop_collection function added.
+- BigQueryOperations
+    - execute_query: return_type="records" (list of dictionaries) implemented.
+    - Different Region connection implemented.
+- HiveOperations
+    - MAJOR UPDATE: HiveOperations are now in extras.
+    - If you want to install extra hive dependencies 
+    - poetry add heps-ds-utils=^0.4.7a3 -extras hive
+- BucketOperations
+    - upload_from_filepath: uploaded file and source file size check added.
+    - download_to_filepath: zip extraction added.
+    - download_recursively function added.
+    - upload_recursively function added.
+    - does_blob_exist function added.
 
-setup(**setup_kwargs)
```

