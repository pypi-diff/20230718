# Comparing `tmp/airflow-commons-0.0.8.tar.gz` & `tmp/airflow-commons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-commons-0.0.8.tar", last modified: Tue Mar 16 16:16:42 2021, max compression
+gzip compressed data, was "airflow-commons-0.0.9.tar", last modified: Wed Mar 31 16:23:37 2021, max compression
```

## Comparing `airflow-commons-0.0.8.tar` & `airflow-commons-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.225332 airflow-commons-0.0.8/airflow_commons/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17711 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/bigquery_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/config_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.225332 airflow-commons-0.0.8/airflow_commons/glossary/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/glossary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2312 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/mysql_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/s3_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.225332 airflow-commons-0.0.8/airflow_commons/sql_resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.225332 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/archive/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/archive/delete_where_statement.sql
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/archive/source_statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/deduplication/
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/deduplication/get_oldest_partition_field.sql
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/deduplication/merge_keys_partition_pruning_params.sql
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/deduplication/source_statement.sql
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/deduplication/source_where_statement.sql
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/deduplication/source_where_statement_partition_pruning_params.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/dml/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/dml/delete.sql
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/dml/insert.sql
--rw-r--r--   0 runner    (1001) docker     (121)      231 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/dml/upsert.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/information_schema/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/information_schema/get_column_names.sql
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/information_schema/get_table_names.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/airflow_commons/sql_resources/mysql/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/sql_resources/mysql/delete.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/airflow_commons/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/airflow_commons/utils/bigquery/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/utils/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7008 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/utils/bigquery/bigquery_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7691 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/utils/bigquery/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/utils/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/airflow_commons/utils/mysql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/utils/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/utils/mysql/mysql_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/utils/mysql/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/airflow_commons/utils/time_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 16:16:42.225332 airflow-commons-0.0.8/airflow_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-03-16 16:16:42.000000 airflow-commons-0.0.8/airflow_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-03-16 16:16:42.000000 airflow-commons-0.0.8/airflow_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-16 16:16:42.000000 airflow-commons-0.0.8/airflow_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-16 16:16:42.000000 airflow-commons-0.0.8/airflow_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-16 16:16:42.000000 airflow-commons-0.0.8/airflow_commons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-16 16:16:42.229332 airflow-commons-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      797 2021-03-16 16:16:33.000000 airflow-commons-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.029776 airflow-commons-0.0.9/airflow_commons/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17711 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/bigquery_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/config_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.029776 airflow-commons-0.0.9/airflow_commons/glossary/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/glossary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      399 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2312 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/mysql_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/s3_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.029776 airflow-commons-0.0.9/airflow_commons/sql_resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.029776 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/archive/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/archive/delete_where_statement.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/archive/source_statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/deduplication/
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/deduplication/get_oldest_partition_field.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/deduplication/merge_keys_partition_pruning_params.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/deduplication/source_statement.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/deduplication/source_where_statement.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/deduplication/source_where_statement_partition_pruning_params.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/dml/
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/dml/delete.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/dml/insert.sql
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/dml/upsert.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/information_schema/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/information_schema/get_column_names.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/information_schema/get_table_names.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/airflow_commons/sql_resources/mysql/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/sql_resources/mysql/delete.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/airflow_commons/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/airflow_commons/utils/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/utils/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7008 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/utils/bigquery/bigquery_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7691 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/utils/bigquery/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/utils/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/airflow_commons/utils/mysql/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/utils/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1856 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/utils/mysql/mysql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/utils/mysql/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/airflow_commons/utils/time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-31 16:23:37.029776 airflow-commons-0.0.9/airflow_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2021-03-31 16:23:36.000000 airflow-commons-0.0.9/airflow_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-03-31 16:23:36.000000 airflow-commons-0.0.9/airflow_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-31 16:23:36.000000 airflow-commons-0.0.9/airflow_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-03-31 16:23:36.000000 airflow-commons-0.0.9/airflow_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-03-31 16:23:36.000000 airflow-commons-0.0.9/airflow_commons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-31 16:23:37.033776 airflow-commons-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-03-31 16:23:28.000000 airflow-commons-0.0.9/setup.py
```

### Comparing `airflow-commons-0.0.8/PKG-INFO` & `airflow-commons-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-commons
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common functions for airflow
 Home-page: https://github.com/migroscomtr/airflow-commons/
 Author: Startup Heroes
 License: UNKNOWN
 Description: # airflow-commons
         A python package that contains common functionalities for airflow
```

### Comparing `airflow-commons-0.0.8/airflow_commons/bigquery_operator.py` & `airflow-commons-0.0.9/airflow_commons/bigquery_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-commons-0.0.8/airflow_commons/mysql_operator.py` & `airflow-commons-0.0.9/airflow_commons/mysql_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-commons-0.0.8/airflow_commons/sql_resources/bigquery/__init__.py` & `airflow-commons-0.0.9/airflow_commons/sql_resources/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-commons-0.0.8/airflow_commons/utils/bigquery/bigquery_utils.py` & `airflow-commons-0.0.9/airflow_commons/utils/bigquery/bigquery_utils.py`

 * *Files identical despite different names*

### Comparing `airflow-commons-0.0.8/airflow_commons/utils/bigquery/sql_utils.py` & `airflow-commons-0.0.9/airflow_commons/utils/bigquery/sql_utils.py`

 * *Files identical despite different names*

### Comparing `airflow-commons-0.0.8/airflow_commons/utils/mysql/mysql_utils.py` & `airflow-commons-0.0.9/airflow_commons/utils/mysql/mysql_utils.py`

 * *Files identical despite different names*

### Comparing `airflow-commons-0.0.8/airflow_commons.egg-info/PKG-INFO` & `airflow-commons-0.0.9/airflow_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-commons
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common functions for airflow
 Home-page: https://github.com/migroscomtr/airflow-commons/
 Author: Startup Heroes
 License: UNKNOWN
 Description: # airflow-commons
         A python package that contains common functionalities for airflow
```

### Comparing `airflow-commons-0.0.8/airflow_commons.egg-info/SOURCES.txt` & `airflow-commons-0.0.9/airflow_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

