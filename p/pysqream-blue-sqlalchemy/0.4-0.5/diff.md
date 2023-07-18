# Comparing `tmp/pysqream_blue_sqlalchemy-0.4.tar.gz` & `tmp/pysqream_blue_sqlalchemy-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysqream_blue_sqlalchemy-0.4.tar", last modified: Thu Jul  6 13:53:52 2023, max compression
+gzip compressed data, was "dist/pysqream_blue_sqlalchemy-0.5.tar", last modified: Tue Jul 18 12:17:19 2023, max compression
```

## Comparing `pysqream_blue_sqlalchemy-0.4.tar` & `pysqream_blue_sqlalchemy-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-06 13:53:38.000000 pysqream_blue_sqlalchemy-0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:53:38.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-06 13:53:38.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:53:52.000000 pysqream_blue_sqlalchemy-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-06 13:53:38.000000 pysqream_blue_sqlalchemy-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-18 12:17:08.000000 pysqream_blue_sqlalchemy-0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:17:08.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-18 12:17:08.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 12:17:19.000000 pysqream_blue_sqlalchemy-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-18 12:17:08.000000 pysqream_blue_sqlalchemy-0.5/setup.py
```

### Comparing `pysqream_blue_sqlalchemy-0.4/PKG-INFO` & `pysqream_blue_sqlalchemy-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.2
 Name: pysqream_blue_sqlalchemy
-Version: 0.4
+Version: 0.5
 Summary: SQLAlchemy dialect for SQream Blue
 Home-page: https://github.com/SQream/pysqream_blue_sqlalchemy
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Description: **********************************
         SQLAlchemy Dialect for SQream DB
         **********************************
         
         Requirements
         =====================
         
         * Python > 3.9.
         * SQLAlchemy > 1.3.18
-        * SQream Blue DB-API Connector >= 1.0.26
+        * SQream Blue DB-API Connector >= 1.0.30
         
         Installation
         =====================
         
         Install from the PyPi repository using `pip`:
         
         .. code-block:: bash
```

### Comparing `pysqream_blue_sqlalchemy-0.4/README.rst` & `pysqream_blue_sqlalchemy-0.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 **********************************
 
 Requirements
 =====================
 
 * Python > 3.9.
 * SQLAlchemy > 1.3.18
-* SQream Blue DB-API Connector >= 1.0.26
+* SQream Blue DB-API Connector >= 1.0.30
 
 Installation
 =====================
 
 Install from the PyPi repository using `pip`:
 
 .. code-block:: bash
```

### Comparing `pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy/dialect.py` & `pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `pysqream_blue_sqlalchemy-0.4/pysqream_blue_sqlalchemy.egg-info/PKG-INFO` & `pysqream_blue_sqlalchemy-0.5/pysqream_blue_sqlalchemy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.2
 Name: pysqream-blue-sqlalchemy
-Version: 0.4
+Version: 0.5
 Summary: SQLAlchemy dialect for SQream Blue
 Home-page: https://github.com/SQream/pysqream_blue_sqlalchemy
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Description: **********************************
         SQLAlchemy Dialect for SQream DB
         **********************************
         
         Requirements
         =====================
         
         * Python > 3.9.
         * SQLAlchemy > 1.3.18
-        * SQream Blue DB-API Connector >= 1.0.26
+        * SQream Blue DB-API Connector >= 1.0.30
         
         Installation
         =====================
         
         Install from the PyPi repository using `pip`:
         
         .. code-block:: bash
```

### Comparing `pysqream_blue_sqlalchemy-0.4/setup.py` & `pysqream_blue_sqlalchemy-0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 
 setup_params = dict(
     
     name =             'pysqream_blue_sqlalchemy',
-    version =          '0.4',
+    version =          '0.5',
     description =      'SQLAlchemy dialect for SQream Blue', 
     long_description = open("README.rst", "r", encoding="utf-8").read(),
     url=               "https://github.com/SQream/pysqream_blue_sqlalchemy",
     
     author =           'SQream',
     author_email =     'info@sqream.com',
     
@@ -18,15 +18,15 @@
         "Operating System :: OS Independent",
     ],
     keywords = 'database sqlalchemy sqream sqreamdb',
 
     python_requires =  '>=3.9',
     
     install_requires = ['sqlalchemy>=1.3.18',
-                        'pysqream-blue>=1.0.28',
+                        'pysqream-blue>=1.0.30',
                         'setuptools>=57.4.0',
                         'pudb==2022.1.2',
                         'pandas==1.1.5',
                         'numpy==1.22.0',
                         'alembic>=1.6.3'],
     
     packages         = ['pysqream_blue_sqlalchemy'],
```

