# Comparing `tmp/databricks_helper-0.0.0.tar.gz` & `tmp/databricks_helper-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_helper-0.0.0.tar", last modified: Tue Jul 18 01:52:43 2023, max compression
+gzip compressed data, was "databricks_helper-0.0.1.tar", last modified: Tue Jul 18 02:20:23 2023, max compression
```

## Comparing `databricks_helper-0.0.0.tar` & `databricks_helper-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 01:52:43.763871 databricks_helper-0.0.0/
--rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      702 2023-07-18 01:52:43.763871 databricks_helper-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 01:52:43.721982 databricks_helper-0.0.0/databricks_helper/
--rw-rw-rw-   0        0        0     1743 2023-07-18 01:31:38.000000 databricks_helper-0.0.0/databricks_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:52:43.699528 databricks_helper-0.0.0/databricks_helper/api/
-drwxrwxrwx   0        0        0        0 2023-07-18 01:52:43.761876 databricks_helper-0.0.0/databricks_helper/api/src/
--rw-rw-rw-   0        0        0    12535 2023-07-18 01:33:26.000000 databricks_helper-0.0.0/databricks_helper/api/src/basic_code.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:52:43.760909 databricks_helper-0.0.0/databricks_helper.egg-info/
--rw-rw-rw-   0        0        0      702 2023-07-18 01:52:43.000000 databricks_helper-0.0.0/databricks_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-18 01:52:43.000000 databricks_helper-0.0.0/databricks_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 01:52:43.000000 databricks_helper-0.0.0/databricks_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-18 01:52:43.000000 databricks_helper-0.0.0/databricks_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       66 2023-07-18 01:52:43.000000 databricks_helper-0.0.0/databricks_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 01:52:43.772847 databricks_helper-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-07-18 01:22:22.000000 databricks_helper-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.175180 databricks_helper-0.0.1/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-07-18 02:20:23.175180 databricks_helper-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.153240 databricks_helper-0.0.1/databricks_helper/
+-rw-rw-rw-   0        0        0     1743 2023-07-18 01:31:38.000000 databricks_helper-0.0.1/databricks_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.139121 databricks_helper-0.0.1/databricks_helper/api/
+drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.174183 databricks_helper-0.0.1/databricks_helper/api/src/
+-rw-rw-rw-   0        0        0    13042 2023-07-18 02:19:35.000000 databricks_helper-0.0.1/databricks_helper/api/src/basic_code.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.172189 databricks_helper-0.0.1/databricks_helper.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       66 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-18 02:20:23.177175 databricks_helper-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-07-18 02:20:05.000000 databricks_helper-0.0.1/setup.py
```

### Comparing `databricks_helper-0.0.0/LICENSE` & `databricks_helper-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.0/PKG-INFO` & `databricks_helper-0.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks_helper
-Version: 0.0.0
+Version: 0.0.1
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.0.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.1.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.0/databricks_helper/__init__.py` & `databricks_helper-0.0.1/databricks_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.0/databricks_helper/api/src/basic_code.py` & `databricks_helper-0.0.1/databricks_helper/api/src/basic_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,47 @@
 DecimalType = DecimalType
 IntegerType = IntegerType
 DateType = DateType
 TimestampType = TimestampType
 Decimal = Decimal
 
 
+def get_spark_session(spark_session: SparkSession = None) -> SparkSession: 
+    if ObjectHelper.isNotNone(spark_session):
+        return spark_session
+    try:
+        global spark
+        return spark
+    except Exception as exception:
+        print(exception)
+        spark = None
+        return spark
+
+
+spark = get_spark_session()
+
+
+def get_display_spark_dataframe_caller():
+    try:
+        global display
+        return display
+    except Exception as exception:
+        print(exception)
+        display = None
+        return display
+
+
+display_spark_dataframe_caller = get_display_spark_dataframe_caller()
+
+
 def two_digits_prefixed_with_zeros_as_string(day_as_int):
     return f'{day_as_int:0>2}'
 
 
+
 ONE_MILION = 1000000
 VERY_LOW_DECIMAL_VALUE = 1 / (100 * ONE_MILION)
 
 NULL_QUERY = 'null'
 
 FIRST_MONTH_DAY = 1
 MINIMUM_LAST_MONTH_DAY = 28
@@ -291,21 +320,17 @@
             if query_value_as_string_is_not_null(cd_as_string)
         ])
     except Exception as exception:
         log.failure(get_distinct_integer_collection_from_table_by_cd, 'Not possible to extract collection. Returning empty collection by default', exception=exception, muteStackTrace=True)
         return []
 
 
-def get_spark_session(spark_session: SparkSession = None) -> SparkSession: 
-    return spark_session if ObjectHelper.isNotNone(spark_session) else spark
-
-
 def display_spark_dataframe(spark_df: DataFrame, *args, **kwargs) -> DataFrame:
     ###- Here, display() is a builting function in databricks
-    display(spark_df, *args, **kwargs)
+    display_spark_dataframe_caller(spark_df, *args, **kwargs)
     return spark_df
 
 
 def display_query(givenQuery: str, show_query=True) -> str:
     if show_query:
         print(givenQuery)
     return givenQuery
```

### Comparing `databricks_helper-0.0.0/databricks_helper.egg-info/PKG-INFO` & `databricks_helper-0.0.1/databricks_helper.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: databricks-helper
-Version: 0.0.0
+Version: 0.0.1
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.0.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.1.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.0/setup.py` & `databricks_helper-0.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.0.0'
+version = '0.0.1'
 name = 'databricks_helper'
 packageName = name
 repositoryName = name.replace("_", "-")
 url = f'https://github.com/SamuelJansen/{repositoryName}/'
 
 
 setup(
```

