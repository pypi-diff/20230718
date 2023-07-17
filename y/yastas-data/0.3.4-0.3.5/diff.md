# Comparing `tmp/yastas-data-0.3.4.tar.gz` & `tmp/yastas-data-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yastas-data-0.3.4.tar", last modified: Wed Jul 12 21:36:25 2023, max compression
+gzip compressed data, was "yastas-data-0.3.5.tar", last modified: Mon Jul 17 22:00:25 2023, max compression
```

## Comparing `yastas-data-0.3.4.tar` & `yastas-data-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 21:36:25.014628 yastas-data-0.3.4/
--rw-rw-rw-   0        0        0      583 2023-07-12 21:36:25.003700 yastas-data-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-10 20:00:47.000000 yastas-data-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.752498 yastas-data-0.3.4/data_code/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.3.4/data_code/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.775649 yastas-data-0.3.4/data_code/beam/
--rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.3.4/data_code/beam/__init__.py
--rw-rw-rw-   0        0        0     1080 2023-07-12 21:01:11.000000 yastas-data-0.3.4/data_code/beam/database.py
-drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.882716 yastas-data-0.3.4/data_code/gcp/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.3.4/data_code/gcp/__init__.py
--rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.3.4/data_code/gcp/bq.py
--rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.3.4/data_code/gcp/secrets.py
--rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.3.4/data_code/gcp/service_account.py
--rw-rw-rw-   0        0        0     3597 2023-07-12 21:35:49.000000 yastas-data-0.3.4/data_code/gcp/sql.py
--rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.3.4/data_code/gcp/storage.py
-drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.927109 yastas-data-0.3.4/data_code/parquets/
--rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.3.4/data_code/parquets/__init__.py
--rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.3.4/data_code/parquets/get_schema.py
--rw-rw-rw-   0        0        0      998 2023-06-13 02:01:53.000000 yastas-data-0.3.4/data_code/parquets/parquet2csv.py
--rw-rw-rw-   0        0        0       42 2023-07-12 21:36:25.015699 yastas-data-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-12 21:36:01.000000 yastas-data-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 21:36:24.991840 yastas-data-0.3.4/yastas_data.egg-info/
--rw-rw-rw-   0        0        0      583 2023-07-12 21:36:24.000000 yastas-data-0.3.4/yastas_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-07-12 21:36:24.000000 yastas-data-0.3.4/yastas_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 21:36:24.000000 yastas-data-0.3.4/yastas_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 21:36:24.000000 yastas-data-0.3.4/yastas_data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 22:00:25.721192 yastas-data-0.3.5/
+-rw-rw-rw-   0        0        0      583 2023-07-17 22:00:25.711631 yastas-data-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-10 20:00:47.000000 yastas-data-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 22:00:25.485151 yastas-data-0.3.5/data_code/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:24:11.000000 yastas-data-0.3.5/data_code/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 22:00:25.514208 yastas-data-0.3.5/data_code/beam/
+-rw-rw-rw-   0        0        0        0 2023-07-10 19:17:14.000000 yastas-data-0.3.5/data_code/beam/__init__.py
+-rw-rw-rw-   0        0        0     2249 2023-07-17 21:52:14.000000 yastas-data-0.3.5/data_code/beam/database.py
+-rw-rw-rw-   0        0        0      677 2023-07-17 21:54:13.000000 yastas-data-0.3.5/data_code/beam/processing.py
+drwxrwxrwx   0        0        0        0 2023-07-17 22:00:25.605659 yastas-data-0.3.5/data_code/gcp/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:34:31.000000 yastas-data-0.3.5/data_code/gcp/__init__.py
+-rw-rw-rw-   0        0        0     1684 2023-07-07 18:59:37.000000 yastas-data-0.3.5/data_code/gcp/bq.py
+-rw-rw-rw-   0        0        0      416 2023-06-26 22:44:12.000000 yastas-data-0.3.5/data_code/gcp/secrets.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 22:17:23.000000 yastas-data-0.3.5/data_code/gcp/service_account.py
+-rw-rw-rw-   0        0        0     2394 2023-07-17 21:42:31.000000 yastas-data-0.3.5/data_code/gcp/sql.py
+-rw-rw-rw-   0        0        0       43 2023-06-21 19:52:01.000000 yastas-data-0.3.5/data_code/gcp/storage.py
+drwxrwxrwx   0        0        0        0 2023-07-17 22:00:25.648236 yastas-data-0.3.5/data_code/parquets/
+-rw-rw-rw-   0        0        0        0 2023-06-22 23:30:05.000000 yastas-data-0.3.5/data_code/parquets/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-06-27 22:57:11.000000 yastas-data-0.3.5/data_code/parquets/get_schema.py
+-rw-rw-rw-   0        0        0      637 2023-07-17 21:57:17.000000 yastas-data-0.3.5/data_code/parquets/parquet2csv.py
+-rw-rw-rw-   0        0        0       42 2023-07-17 22:00:25.721192 yastas-data-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-17 21:54:47.000000 yastas-data-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 22:00:25.702156 yastas-data-0.3.5/yastas_data.egg-info/
+-rw-rw-rw-   0        0        0      583 2023-07-17 22:00:24.000000 yastas-data-0.3.5/yastas_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-07-17 22:00:25.000000 yastas-data-0.3.5/yastas_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 22:00:24.000000 yastas-data-0.3.5/yastas_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 22:00:24.000000 yastas-data-0.3.5/yastas_data.egg-info/top_level.txt
```

### Comparing `yastas-data-0.3.4/PKG-INFO` & `yastas-data-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.3.4
+Version: 0.3.5
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

### Comparing `yastas-data-0.3.4/data_code/gcp/bq.py` & `yastas-data-0.3.5/data_code/gcp/bq.py`

 * *Files identical despite different names*

### Comparing `yastas-data-0.3.4/setup.py` & `yastas-data-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('requirements.txt') as file:
         return file.read().splitlines()
     
 readme = open("./README.md", "r")
 
 setup(
     name='yastas-data',
-    version='0.3.4',
+    version='0.3.5',
     author='Data - Aaron',
     author_email="e-ajuareza@minsait.com",
     description='Paquete distribuible en repositorio de funciones locales',
     long_description=readme.read(),
     packages=find_packages(),
     url="https://bitbucket.org/gentera-insumos/data-code",
     keywords=['data', 'big_data', 'data_analytics', 'data_engineer', 'data_science'],
```

### Comparing `yastas-data-0.3.4/yastas_data.egg-info/PKG-INFO` & `yastas-data-0.3.5/yastas_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: yastas-data
-Version: 0.3.4
+Version: 0.3.5
 Summary: Paquete distribuible en repositorio de funciones locales
 Home-page: https://bitbucket.org/gentera-insumos/data-code
 Author: Data - Aaron
 Author-email: e-ajuareza@minsait.com
 License: MIT
 Description: # InstalaciÃ³n
```

