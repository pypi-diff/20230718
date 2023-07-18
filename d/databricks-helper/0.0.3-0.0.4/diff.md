# Comparing `tmp/databricks_helper-0.0.3.tar.gz` & `tmp/databricks_helper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_helper-0.0.3.tar", last modified: Tue Jul 18 02:55:35 2023, max compression
+gzip compressed data, was "databricks_helper-0.0.4.tar", last modified: Tue Jul 18 03:08:36 2023, max compression
```

## Comparing `databricks_helper-0.0.3.tar` & `databricks_helper-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.845292 databricks_helper-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      702 2023-07-18 02:55:35.845292 databricks_helper-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.809390 databricks_helper-0.0.3/databricks_helper/
--rw-rw-rw-   0        0        0     1788 2023-07-18 02:51:23.000000 databricks_helper-0.0.3/databricks_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.778472 databricks_helper-0.0.3/databricks_helper/api/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.843297 databricks_helper-0.0.3/databricks_helper/api/src/
--rw-rw-rw-   0        0        0    13222 2023-07-18 02:54:35.000000 databricks_helper-0.0.3/databricks_helper/api/src/basic_code.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:55:35.841304 databricks_helper-0.0.3/databricks_helper.egg-info/
--rw-rw-rw-   0        0        0      702 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       66 2023-07-18 02:55:35.000000 databricks_helper-0.0.3/databricks_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 02:55:35.847287 databricks_helper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-07-18 02:48:16.000000 databricks_helper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.395537 databricks_helper-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-07-18 03:08:36.396535 databricks_helper-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.372346 databricks_helper-0.0.4/databricks_helper/
+-rw-rw-rw-   0        0        0     1788 2023-07-18 02:51:23.000000 databricks_helper-0.0.4/databricks_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.357466 databricks_helper-0.0.4/databricks_helper/api/
+drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.394540 databricks_helper-0.0.4/databricks_helper/api/src/
+-rw-rw-rw-   0        0        0    13412 2023-07-18 03:08:01.000000 databricks_helper-0.0.4/databricks_helper/api/src/basic_code.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.392545 databricks_helper-0.0.4/databricks_helper.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       66 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-18 03:08:36.398530 databricks_helper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-07-18 03:08:14.000000 databricks_helper-0.0.4/setup.py
```

### Comparing `databricks_helper-0.0.3/LICENSE` & `databricks_helper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.3/PKG-INFO` & `databricks_helper-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks_helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.4.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.3/databricks_helper/__init__.py` & `databricks_helper-0.0.4/databricks_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.3/databricks_helper/api/src/basic_code.py` & `databricks_helper-0.0.4/databricks_helper/api/src/basic_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import col as spark_col
 from pyspark.sql.functions import sum as spark_sum
 from pyspark.sql.functions import round as spark_round
 from pyspark.sql.types import StructType, StructField, StringType, DoubleType, DecimalType, IntegerType, DateType, TimestampType
 
 
+DB_SPARK_SESSION = 'default spark session'
+DB_SPARK_DF_DISPLAY = 'default spark dataframe display'
+
+
 spark_col = spark_col
 spark_sum = spark_sum
 spark_round = spark_round
 StructType = StructType
 StructField = StructField
 StringType = StringType
 DoubleType = DoubleType
@@ -24,42 +28,35 @@
 Decimal = Decimal
 
 
 def get_spark_session(spark_session: SparkSession = None) -> SparkSession: 
     if ObjectHelper.isNotNone(spark_session):
         return spark_session
     try:
-        global db_spark
-        return db_spark
+        return DB_SPARK_SESSION
     except Exception as exception:
         print(exception)
-        print(f'''global db_spark
-db_spark = spark''')
+        print(f'''databricks_helper.DB_SPARK_SESSION = spark''')
     return None
 
 
 spark = get_spark_session()
 
 
-def get_display_spark_dataframe_caller(display_spark_df = None):
-    if ObjectHelper.isNotNone(display_spark_df):
-        return display_spark_df
+def get_display_spark_dataframe_caller(spark_df_display = None):
+    if ObjectHelper.isNotNone(spark_df_display):
+        return spark_df_display
     try:
-        global db_display
-        return db_display
+        return DB_SPARK_DF_DISPLAY
     except Exception as exception:
         print(exception)
-        print(f'''global db_display
-db_display = display''')
+        print(f'''databricks_helper.DB_SPARK_DF_DISPLAY = display''')
     return None
 
 
-display_spark_dataframe_caller = get_display_spark_dataframe_caller()
-
-
 def two_digits_prefixed_with_zeros_as_string(day_as_int):
     return f'{day_as_int:0>2}'
 
 
 
 ONE_MILION = 1000000
 VERY_LOW_DECIMAL_VALUE = 1 / (100 * ONE_MILION)
@@ -324,30 +321,30 @@
             if query_value_as_string_is_not_null(cd_as_string)
         ])
     except Exception as exception:
         log.failure(get_distinct_integer_collection_from_table_by_cd, 'Not possible to extract collection. Returning empty collection by default', exception=exception, muteStackTrace=True)
         return []
 
 
-def display_spark_dataframe(spark_df: DataFrame, *args, **kwargs) -> DataFrame:
+def display_spark_dataframe(spark_df: DataFrame, *args, spark_df_display=None, **kwargs) -> DataFrame:
     ###- Here, display() is a builting function in databricks
-    display_spark_dataframe_caller(spark_df, *args, **kwargs)
+    get_display_spark_dataframe_caller(spark_df_display=spark_df_display)(spark_df, *args, **kwargs)
     return spark_df
 
 
 def display_query(givenQuery: str, show_query=True) -> str:
     if show_query:
         print(givenQuery)
     return givenQuery
 
 
-def spark_sql(*agrs, show_dataframe=True, spark_session: SparkSession = None, **kwargs) -> DataFrame:
+def spark_sql(*agrs, show_dataframe=True, spark_session: SparkSession = None, spark_df_display=None, **kwargs) -> DataFrame:
     df = get_spark_session(spark_session=spark_session).sql(display_query(*agrs, **kwargs))
     if show_dataframe:
-        display_spark_dataframe(df)
+        display_spark_dataframe(df, spark_df_display=spark_df_display)
     return df
 
 
 def spark_create_or_replace_temp_view_from_sql(*agrs, view_name=None, **kwargs) -> DataFrame:
     df = spark_sql(*agrs, **kwargs)
     df.createOrReplaceTempView(view_name)
     return df
@@ -359,20 +356,20 @@
     return df
 
 
 def spark_spark_create_or_replace_temp_view_from_big_sql(*agrs, **kwargs) -> DataFrame:
     return spark_big_sql(*agrs, spark_sql_caller=spark_create_or_replace_temp_view_from_sql, **kwargs)
     
 
-def spark_createDataFrame(*agrs, show_dataframe=True, order_by=None, spark_session: SparkSession = None, **kwargs) -> DataFrame:
+def spark_createDataFrame(*agrs, show_dataframe=True, order_by=None, spark_session: SparkSession = None, spark_df_display=None, **kwargs) -> DataFrame:
     df = get_spark_session(spark_session=spark_session).createDataFrame(*agrs, **kwargs)
     if ObjectHelper.isNotEmpty(order_by):
         df = df.orderBy(*order_by)
     if show_dataframe:
-        display_spark_dataframe(df)
+        display_spark_dataframe(df, spark_df_display=spark_df_display)
     return df
 
 
 def override_table_and_schema(spark_df, table_name):
     return save_as_table(to_spark_df_override_delta_mode(spark_df).option('overwriteSchema', 'true'), table_name)
```

### Comparing `databricks_helper-0.0.3/databricks_helper.egg-info/PKG-INFO` & `databricks_helper-0.0.4/databricks_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks-helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.3.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.4.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.3/setup.py` & `databricks_helper-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.0.3'
+version = '0.0.4'
 name = 'databricks_helper'
 packageName = name
 repositoryName = name.replace("_", "-")
 url = f'https://github.com/SamuelJansen/{repositoryName}/'
 
 
 setup(
```

