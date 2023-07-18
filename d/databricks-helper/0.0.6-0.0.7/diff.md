# Comparing `tmp/databricks_helper-0.0.6.tar.gz` & `tmp/databricks_helper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_helper-0.0.6.tar", last modified: Tue Jul 18 03:26:50 2023, max compression
+gzip compressed data, was "databricks_helper-0.0.7.tar", last modified: Tue Jul 18 03:42:14 2023, max compression
```

## Comparing `databricks_helper-0.0.6.tar` & `databricks_helper-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.056483 databricks_helper-0.0.6/
--rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      702 2023-07-18 03:26:50.057480 databricks_helper-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.031550 databricks_helper-0.0.6/databricks_helper/
--rw-rw-rw-   0        0        0     1864 2023-07-18 03:25:26.000000 databricks_helper-0.0.6/databricks_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.022574 databricks_helper-0.0.6/databricks_helper/api/
-drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.054488 databricks_helper-0.0.6/databricks_helper/api/src/
--rw-rw-rw-   0        0        0    13747 2023-07-18 03:24:46.000000 databricks_helper-0.0.6/databricks_helper/api/src/basic_code.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:26:50.053490 databricks_helper-0.0.6/databricks_helper.egg-info/
--rw-rw-rw-   0        0        0      702 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       66 2023-07-18 03:26:49.000000 databricks_helper-0.0.6/databricks_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 03:26:50.059475 databricks_helper-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-07-18 03:26:28.000000 databricks_helper-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.472393 databricks_helper-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-07-18 03:42:14.472393 databricks_helper-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.437944 databricks_helper-0.0.7/databricks_helper/
+-rw-rw-rw-   0        0        0     1901 2023-07-18 03:39:12.000000 databricks_helper-0.0.7/databricks_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.423172 databricks_helper-0.0.7/databricks_helper/api/
+drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.470399 databricks_helper-0.0.7/databricks_helper/api/src/
+-rw-rw-rw-   0        0        0    13916 2023-07-18 03:38:53.000000 databricks_helper-0.0.7/databricks_helper/api/src/basic_code.py
+drwxrwxrwx   0        0        0        0 2023-07-18 03:42:14.468405 databricks_helper-0.0.7/databricks_helper.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       66 2023-07-18 03:42:14.000000 databricks_helper-0.0.7/databricks_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-18 03:42:14.475385 databricks_helper-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-07-18 03:41:37.000000 databricks_helper-0.0.7/setup.py
```

### Comparing `databricks_helper-0.0.6/LICENSE` & `databricks_helper-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.6/PKG-INFO` & `databricks_helper-0.0.7/databricks_helper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: databricks_helper
-Version: 0.0.6
+Name: databricks-helper
+Version: 0.0.7
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.6.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.7.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.6/databricks_helper/__init__.py` & `databricks_helper-0.0.7/databricks_helper/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     DoubleType,
     DecimalType,
     IntegerType,
     DateType,
     TimestampType,
     Decimal,
 
+    DataFrame,
+    SparkSession,
+
     two_digits_prefixed_with_zeros_as_string,
     remove_leading_zeros,
     build_first_month_date_given_date_as_string_list,
     get_first_month_date,
     get_last_month_date,
     get_last_month_day,
     get_year_dash_month,
```

### Comparing `databricks_helper-0.0.6/databricks_helper/api/src/basic_code.py` & `databricks_helper-0.0.7/databricks_helper/api/src/basic_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from python_helper import DateTimeHelper, StringHelper, Constant, ObjectHelper, log
 
 from decimal import Decimal
 
-from pyspark.sql.dataframe import DataFrame
-from pyspark.sql import SparkSession
+try:
+    from pyspark.sql.dataframe import DataFrame
+    from pyspark.sql import SparkSession
+except Exception as exception:
+    print(exception)
+    DataFrame = None
+    SparkSession = None
 from pyspark.sql.functions import col as spark_col
 from pyspark.sql.functions import sum as spark_sum
 from pyspark.sql.functions import round as spark_round
 from pyspark.sql.types import StructType, StructField, StringType, DoubleType, DecimalType, IntegerType, DateType, TimestampType
 
 
 global DB_SPARK_SESSION
@@ -26,14 +31,17 @@
 DoubleType = DoubleType
 DecimalType = DecimalType
 IntegerType = IntegerType
 DateType = DateType
 TimestampType = TimestampType
 Decimal = Decimal
 
+DataFrame = DataFrame
+SparkSession = SparkSession
+
 
 def set_default_spark_session(spark_session):
     global DB_SPARK_SESSION
     DB_SPARK_SESSION = spark_session
 
 
 def set_default_display_spark_dataframe(spark_df_display):
```

### Comparing `databricks_helper-0.0.6/databricks_helper.egg-info/PKG-INFO` & `databricks_helper-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: databricks-helper
-Version: 0.0.6
+Name: databricks_helper
+Version: 0.0.7
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.6.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.7.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.6/setup.py` & `databricks_helper-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.0.6'
+version = '0.0.7'
 name = 'databricks_helper'
 packageName = name
 repositoryName = name.replace("_", "-")
 url = f'https://github.com/SamuelJansen/{repositoryName}/'
 
 
 setup(
@@ -22,15 +22,15 @@
     description = 'databricks helper package',
     author = 'Samuel Jansen',
     author_email = 'samuel.jansenn@gmail.com',
     url = url,
     download_url = f'{url}archive/v{version}.tar.gz',
     keywords = ['helper', 'databricks helper package', 'databricks helper', 'helper package'],
     install_requires = [
-        'pyspark<4.0.0,>=3.0.0',
+        'pyspark<4.0.0,>=2.0.0',
         'python_helper<1.0.0,>=0.3.67'
     ],
     classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
```

