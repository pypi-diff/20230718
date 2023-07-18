# Comparing `tmp/databricks_helper-0.0.5.tar.gz` & `tmp/databricks_helper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_helper-0.0.5.tar", last modified: Tue Jul 18 03:14:59 2023, max compression
+gzip compressed data, was "databricks_helper-0.0.6.tar", last modified: Tue Jul 18 03:26:50 2023, max compression
```

## Comparing `databricks_helper-0.0.5.tar` & `databricks_helper-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.544726 databricks_helper-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      702 2023-07-18 03:14:59.544726 databricks_helper-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.510839 databricks_helper-0.0.5/databricks_helper/
--rw-rw-rw-   0        0        0     1788 2023-07-18 02:51:23.000000 databricks_helper-0.0.5/databricks_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.496696 databricks_helper-0.0.5/databricks_helper/api/
-drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.542733 databricks_helper-0.0.5/databricks_helper/api/src/
--rw-rw-rw-   0        0        0    13526 2023-07-18 03:14:32.000000 databricks_helper-0.0.5/databricks_helper/api/src/basic_code.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.540737 databricks_helper-0.0.5/databricks_helper.egg-info/
--rw-rw-rw-   0        0        0      702 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       66 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 03:14:59.546721 databricks_helper-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-07-18 03:14:42.000000 databricks_helper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.056483 databricks_helper-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-07-18 03:26:50.057480 databricks_helper-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.031550 databricks_helper-0.0.6/databricks_helper/
+-rw-rw-rw-   0        0        0     1864 2023-07-18 03:25:26.000000 databricks_helper-0.0.6/databricks_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.022574 databricks_helper-0.0.6/databricks_helper/api/
+drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.054488 databricks_helper-0.0.6/databricks_helper/api/src/
+-rw-rw-rw-   0        0        0    13747 2023-07-18 03:24:46.000000 databricks_helper-0.0.6/databricks_helper/api/src/basic_code.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.053490 databricks_helper-0.0.6/databricks_helper.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       66 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-18 03:26:50.059475 databricks_helper-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-07-18 03:26:28.000000 databricks_helper-0.0.6/setup.py
```

### Comparing `databricks_helper-0.0.5/LICENSE` & `databricks_helper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.5/PKG-INFO` & `databricks_helper-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks_helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.5.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.6.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.5/databricks_helper/__init__.py` & `databricks_helper-0.0.6/databricks_helper/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from databricks_helper.api.src.basic_code import (
 
     get_spark_session,
     get_display_spark_dataframe_caller,
 
+    set_default_spark_session,
+    set_default_display_spark_dataframe,
+
     spark_col,
     spark_sum,
     spark_round,
     StructType,
     StructField,
     StringType,
     DoubleType,
```

### Comparing `databricks_helper-0.0.5/databricks_helper/api/src/basic_code.py` & `databricks_helper-0.0.6/databricks_helper/api/src/basic_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from pyspark.sql.dataframe import DataFrame
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import col as spark_col
 from pyspark.sql.functions import sum as spark_sum
 from pyspark.sql.functions import round as spark_round
 from pyspark.sql.types import StructType, StructField, StringType, DoubleType, DecimalType, IntegerType, DateType, TimestampType
 
+
 global DB_SPARK_SESSION
-global DB_SPARK_DF_DISPLAY
+DB_SPARK_SESSION = None
 
-DB_SPARK_SESSION = 'default spark session'
-DB_SPARK_DF_DISPLAY = 'default spark dataframe display'
+global DB_SPARK_DF_DISPLAY
+DB_SPARK_DF_DISPLAY = None
 
 
 spark_col = spark_col
 spark_sum = spark_sum
 spark_round = spark_round
 StructType = StructType
 StructField = StructField
@@ -26,34 +27,42 @@
 DecimalType = DecimalType
 IntegerType = IntegerType
 DateType = DateType
 TimestampType = TimestampType
 Decimal = Decimal
 
 
+def set_default_spark_session(spark_session):
+    global DB_SPARK_SESSION
+    DB_SPARK_SESSION = spark_session
+
+
+def set_default_display_spark_dataframe(spark_df_display):
+    global DB_SPARK_DF_DISPLAY
+    DB_SPARK_DF_DISPLAY = spark_df_display
+
+
 def get_spark_session(spark_session: SparkSession = None) -> SparkSession: 
     if ObjectHelper.isNotNone(spark_session):
         return spark_session
-    global DB_SPARK_SESSION
     try:
+        global DB_SPARK_SESSION
         return DB_SPARK_SESSION
     except Exception as exception:
         print(exception)
         print(f'''databricks_helper.DB_SPARK_SESSION = spark''')
     return None
 
 
-spark = get_spark_session()
-
-
 def get_display_spark_dataframe_caller(spark_df_display = None):
     if ObjectHelper.isNotNone(spark_df_display):
         return spark_df_display
-    global DB_SPARK_DF_DISPLAY
+    # global DB_SPARK_DF_DISPLAY
     try:
+        global DB_SPARK_DF_DISPLAY
         return DB_SPARK_DF_DISPLAY
     except Exception as exception:
         print(exception)
         print(f'''databricks_helper.DB_SPARK_DF_DISPLAY = display''')
     return None
```

### Comparing `databricks_helper-0.0.5/databricks_helper.egg-info/PKG-INFO` & `databricks_helper-0.0.6/databricks_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks-helper
-Version: 0.0.5
+Version: 0.0.6
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.5.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.6.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.5/setup.py` & `databricks_helper-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.0.5'
+version = '0.0.6'
 name = 'databricks_helper'
 packageName = name
 repositoryName = name.replace("_", "-")
 url = f'https://github.com/SamuelJansen/{repositoryName}/'
 
 
 setup(
```

