# Comparing `tmp/databricks_helper-0.0.4.tar.gz` & `tmp/databricks_helper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_helper-0.0.4.tar", last modified: Tue Jul 18 03:08:36 2023, max compression
+gzip compressed data, was "databricks_helper-0.0.5.tar", last modified: Tue Jul 18 03:14:59 2023, max compression
```

## Comparing `databricks_helper-0.0.4.tar` & `databricks_helper-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.395537 databricks_helper-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      702 2023-07-18 03:08:36.396535 databricks_helper-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.372346 databricks_helper-0.0.4/databricks_helper/
--rw-rw-rw-   0        0        0     1788 2023-07-18 02:51:23.000000 databricks_helper-0.0.4/databricks_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.357466 databricks_helper-0.0.4/databricks_helper/api/
-drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.394540 databricks_helper-0.0.4/databricks_helper/api/src/
--rw-rw-rw-   0        0        0    13412 2023-07-18 03:08:01.000000 databricks_helper-0.0.4/databricks_helper/api/src/basic_code.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:08:36.392545 databricks_helper-0.0.4/databricks_helper.egg-info/
--rw-rw-rw-   0        0        0      702 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       66 2023-07-18 03:08:36.000000 databricks_helper-0.0.4/databricks_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 03:08:36.398530 databricks_helper-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-07-18 03:08:14.000000 databricks_helper-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.544726 databricks_helper-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-07-18 03:14:59.544726 databricks_helper-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.510839 databricks_helper-0.0.5/databricks_helper/
+-rw-rw-rw-   0        0        0     1788 2023-07-18 02:51:23.000000 databricks_helper-0.0.5/databricks_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.496696 databricks_helper-0.0.5/databricks_helper/api/
+drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.542733 databricks_helper-0.0.5/databricks_helper/api/src/
+-rw-rw-rw-   0        0        0    13526 2023-07-18 03:14:32.000000 databricks_helper-0.0.5/databricks_helper/api/src/basic_code.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:14:59.540737 databricks_helper-0.0.5/databricks_helper.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       66 2023-07-18 03:14:59.000000 databricks_helper-0.0.5/databricks_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-18 03:14:59.546721 databricks_helper-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-07-18 03:14:42.000000 databricks_helper-0.0.5/setup.py
```

### Comparing `databricks_helper-0.0.4/LICENSE` & `databricks_helper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.4/PKG-INFO` & `databricks_helper-0.0.5/databricks_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: databricks_helper
-Version: 0.0.4
+Name: databricks-helper
+Version: 0.0.5
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.4.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.5.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.4/databricks_helper/__init__.py` & `databricks_helper-0.0.5/databricks_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.4/databricks_helper/api/src/basic_code.py` & `databricks_helper-0.0.5/databricks_helper/api/src/basic_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from pyspark.sql.dataframe import DataFrame
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import col as spark_col
 from pyspark.sql.functions import sum as spark_sum
 from pyspark.sql.functions import round as spark_round
 from pyspark.sql.types import StructType, StructField, StringType, DoubleType, DecimalType, IntegerType, DateType, TimestampType
 
+global DB_SPARK_SESSION
+global DB_SPARK_DF_DISPLAY
 
 DB_SPARK_SESSION = 'default spark session'
 DB_SPARK_DF_DISPLAY = 'default spark dataframe display'
 
 
 spark_col = spark_col
 spark_sum = spark_sum
@@ -27,28 +29,30 @@
 TimestampType = TimestampType
 Decimal = Decimal
 
 
 def get_spark_session(spark_session: SparkSession = None) -> SparkSession: 
     if ObjectHelper.isNotNone(spark_session):
         return spark_session
+    global DB_SPARK_SESSION
     try:
         return DB_SPARK_SESSION
     except Exception as exception:
         print(exception)
         print(f'''databricks_helper.DB_SPARK_SESSION = spark''')
     return None
 
 
 spark = get_spark_session()
 
 
 def get_display_spark_dataframe_caller(spark_df_display = None):
     if ObjectHelper.isNotNone(spark_df_display):
         return spark_df_display
+    global DB_SPARK_DF_DISPLAY
     try:
         return DB_SPARK_DF_DISPLAY
     except Exception as exception:
         print(exception)
         print(f'''databricks_helper.DB_SPARK_DF_DISPLAY = display''')
     return None
```

### Comparing `databricks_helper-0.0.4/databricks_helper.egg-info/PKG-INFO` & `databricks_helper-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: databricks-helper
-Version: 0.0.4
+Name: databricks_helper
+Version: 0.0.5
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.4.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.5.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.4/setup.py` & `databricks_helper-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.0.4'
+version = '0.0.5'
 name = 'databricks_helper'
 packageName = name
 repositoryName = name.replace("_", "-")
 url = f'https://github.com/SamuelJansen/{repositoryName}/'
 
 
 setup(
@@ -23,15 +23,15 @@
     author = 'Samuel Jansen',
     author_email = 'samuel.jansenn@gmail.com',
     url = url,
     download_url = f'{url}archive/v{version}.tar.gz',
     keywords = ['helper', 'databricks helper package', 'databricks helper', 'helper package'],
     install_requires = [
         'pyspark<4.0.0,>=3.0.0',
-        'python-helper<1.0.0,>=0.3.67'
+        'python_helper<1.0.0,>=0.3.67'
     ],
     classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7'
```

