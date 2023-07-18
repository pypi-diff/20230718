# Comparing `tmp/databricks_helper-0.0.2.tar.gz` & `tmp/databricks_helper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_helper-0.0.2.tar", last modified: Tue Jul 18 02:38:58 2023, max compression
+gzip compressed data, was "databricks_helper-0.0.3.tar", last modified: Tue Jul 18 02:55:35 2023, max compression
```

## Comparing `databricks_helper-0.0.2.tar` & `databricks_helper-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.436047 databricks_helper-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      702 2023-07-18 02:38:58.436047 databricks_helper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.409119 databricks_helper-0.0.2/databricks_helper/
--rw-rw-rw-   0        0        0     1743 2023-07-18 01:31:38.000000 databricks_helper-0.0.2/databricks_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.393894 databricks_helper-0.0.2/databricks_helper/api/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.434052 databricks_helper-0.0.2/databricks_helper/api/src/
--rw-rw-rw-   0        0        0    13116 2023-07-18 02:38:19.000000 databricks_helper-0.0.2/databricks_helper/api/src/basic_code.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.432057 databricks_helper-0.0.2/databricks_helper.egg-info/
--rw-rw-rw-   0        0        0      702 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       66 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 02:38:58.438042 databricks_helper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-07-18 02:38:25.000000 databricks_helper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.845292 databricks_helper-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-07-18 02:55:35.845292 databricks_helper-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.809390 databricks_helper-0.0.3/databricks_helper/
+-rw-rw-rw-   0        0        0     1788 2023-07-18 02:51:23.000000 databricks_helper-0.0.3/databricks_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.778472 databricks_helper-0.0.3/databricks_helper/api/
+drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.843297 databricks_helper-0.0.3/databricks_helper/api/src/
+-rw-rw-rw-   0        0        0    13222 2023-07-18 02:54:35.000000 databricks_helper-0.0.3/databricks_helper/api/src/basic_code.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.841304 databricks_helper-0.0.3/databricks_helper.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       66 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-18 02:55:35.847287 databricks_helper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-07-18 02:48:16.000000 databricks_helper-0.0.3/setup.py
```

### Comparing `databricks_helper-0.0.2/LICENSE` & `databricks_helper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.2/PKG-INFO` & `databricks_helper-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks_helper
-Version: 0.0.2
+Version: 0.0.3
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.2.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.3.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.2/databricks_helper/__init__.py` & `databricks_helper-0.0.3/databricks_helper/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 from databricks_helper.api.src.basic_code import (
+
+    get_spark_session,
+    get_display_spark_dataframe_caller,
+
     spark_col,
     spark_sum,
     spark_round,
     StructType,
     StructField,
     StringType,
     DoubleType,
@@ -44,15 +48,14 @@
     cast_to_query_2_digits_decimal,
     cast_to_query_percentual_decimal,
     cast_to_query_monetary_decimal,
     cast_to_query_integer,
     concat_query_date,
     get_distinct_integer_collection_from_table,
     get_distinct_integer_collection_from_table_by_cd,
-    get_spark_session,
     display_spark_dataframe,
     display_query,
     spark_sql,
     spark_create_or_replace_temp_view_from_sql,
     spark_big_sql,
     spark_spark_create_or_replace_temp_view_from_big_sql,
     spark_createDataFrame,
```

### Comparing `databricks_helper-0.0.2/databricks_helper/api/src/basic_code.py` & `databricks_helper-0.0.3/databricks_helper/api/src/basic_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 db_spark = spark''')
     return None
 
 
 spark = get_spark_session()
 
 
-def get_display_spark_dataframe_caller():
+def get_display_spark_dataframe_caller(display_spark_df = None):
+    if ObjectHelper.isNotNone(display_spark_df):
+        return display_spark_df
     try:
         global db_display
         return db_display
     except Exception as exception:
         print(exception)
         print(f'''global db_display
 db_display = display''')
```

### Comparing `databricks_helper-0.0.2/databricks_helper.egg-info/PKG-INFO` & `databricks_helper-0.0.3/databricks_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks-helper
-Version: 0.0.2
+Version: 0.0.3
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.2.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.3.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.2/setup.py` & `databricks_helper-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.0.2'
+version = '0.0.3'
 name = 'databricks_helper'
 packageName = name
 repositoryName = name.replace("_", "-")
 url = f'https://github.com/SamuelJansen/{repositoryName}/'
 
 
 setup(
```

