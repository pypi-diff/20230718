# Comparing `tmp/databricks_helper-0.0.1.tar.gz` & `tmp/databricks_helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_helper-0.0.1.tar", last modified: Tue Jul 18 02:20:23 2023, max compression
+gzip compressed data, was "databricks_helper-0.0.2.tar", last modified: Tue Jul 18 02:38:58 2023, max compression
```

## Comparing `databricks_helper-0.0.1.tar` & `databricks_helper-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.175180 databricks_helper-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      702 2023-07-18 02:20:23.175180 databricks_helper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.153240 databricks_helper-0.0.1/databricks_helper/
--rw-rw-rw-   0        0        0     1743 2023-07-18 01:31:38.000000 databricks_helper-0.0.1/databricks_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.139121 databricks_helper-0.0.1/databricks_helper/api/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.174183 databricks_helper-0.0.1/databricks_helper/api/src/
--rw-rw-rw-   0        0        0    13042 2023-07-18 02:19:35.000000 databricks_helper-0.0.1/databricks_helper/api/src/basic_code.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:20:23.172189 databricks_helper-0.0.1/databricks_helper.egg-info/
--rw-rw-rw-   0        0        0      702 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       66 2023-07-18 02:20:23.000000 databricks_helper-0.0.1/databricks_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 02:20:23.177175 databricks_helper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-07-18 02:20:05.000000 databricks_helper-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.436047 databricks_helper-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-18 00:40:50.000000 databricks_helper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      702 2023-07-18 02:38:58.436047 databricks_helper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:40:50.000000 databricks_helper-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.409119 databricks_helper-0.0.2/databricks_helper/
+-rw-rw-rw-   0        0        0     1743 2023-07-18 01:31:38.000000 databricks_helper-0.0.2/databricks_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.393894 databricks_helper-0.0.2/databricks_helper/api/
+drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.434052 databricks_helper-0.0.2/databricks_helper/api/src/
+-rw-rw-rw-   0        0        0    13116 2023-07-18 02:38:19.000000 databricks_helper-0.0.2/databricks_helper/api/src/basic_code.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:38:58.432057 databricks_helper-0.0.2/databricks_helper.egg-info/
+-rw-rw-rw-   0        0        0      702 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       66 2023-07-18 02:38:58.000000 databricks_helper-0.0.2/databricks_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-18 02:38:58.438042 databricks_helper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-07-18 02:38:25.000000 databricks_helper-0.0.2/setup.py
```

### Comparing `databricks_helper-0.0.1/LICENSE` & `databricks_helper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.1/PKG-INFO` & `databricks_helper-0.0.2/databricks_helper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: databricks_helper
-Version: 0.0.1
+Name: databricks-helper
+Version: 0.0.2
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.1.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.2.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.1/databricks_helper/__init__.py` & `databricks_helper-0.0.2/databricks_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_helper-0.0.1/databricks_helper/api/src/basic_code.py` & `databricks_helper-0.0.2/databricks_helper/api/src/basic_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,33 +24,35 @@
 Decimal = Decimal
 
 
 def get_spark_session(spark_session: SparkSession = None) -> SparkSession: 
     if ObjectHelper.isNotNone(spark_session):
         return spark_session
     try:
-        global spark
-        return spark
+        global db_spark
+        return db_spark
     except Exception as exception:
         print(exception)
-        spark = None
-        return spark
+        print(f'''global db_spark
+db_spark = spark''')
+    return None
 
 
 spark = get_spark_session()
 
 
 def get_display_spark_dataframe_caller():
     try:
-        global display
-        return display
+        global db_display
+        return db_display
     except Exception as exception:
         print(exception)
-        display = None
-        return display
+        print(f'''global db_display
+db_display = display''')
+    return None
 
 
 display_spark_dataframe_caller = get_display_spark_dataframe_caller()
 
 
 def two_digits_prefixed_with_zeros_as_string(day_as_int):
     return f'{day_as_int:0>2}'
```

### Comparing `databricks_helper-0.0.1/databricks_helper.egg-info/PKG-INFO` & `databricks_helper-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: databricks-helper
-Version: 0.0.1
+Name: databricks_helper
+Version: 0.0.2
 Summary: databricks helper package
 Home-page: https://github.com/SamuelJansen/databricks-helper/
-Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.1.tar.gz
+Download-URL: https://github.com/SamuelJansen/databricks-helper/archive/v0.0.2.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: helper,databricks helper package,databricks helper,helper package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `databricks_helper-0.0.1/setup.py` & `databricks_helper-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 import os
 
 OS_SEPARATOR = os.path.sep
 
-version = '0.0.1'
+version = '0.0.2'
 name = 'databricks_helper'
 packageName = name
 repositoryName = name.replace("_", "-")
 url = f'https://github.com/SamuelJansen/{repositoryName}/'
 
 
 setup(
```

