# Comparing `tmp/connectors_to_databases-1.0.6.tar.gz` & `tmp/connectors_to_databases-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectors_to_databases-1.0.6.tar", last modified: Mon Jul 17 07:42:32 2023, max compression
+gzip compressed data, was "connectors_to_databases-1.1.0.tar", last modified: Tue Jul 18 05:07:35 2023, max compression
```

## Comparing `connectors_to_databases-1.0.6.tar` & `connectors_to_databases-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:42:32.747212 connectors_to_databases-1.0.6/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.0.6/LICENSE.MD
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     4166 2023-07-17 07:42:32.747066 connectors_to_databases-1.0.6/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     3033 2023-07-17 07:08:57.000000 connectors_to_databases-1.0.6/README.md
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:42:32.746222 connectors_to_databases-1.0.6/connectors_to_databases/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     3984 2023-07-17 06:50:16.000000 connectors_to_databases-1.0.6/connectors_to_databases/BaseOperator.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1161 2023-06-03 06:35:40.000000 connectors_to_databases-1.0.6/connectors_to_databases/ClickHouse.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     7957 2023-07-17 07:40:12.000000 connectors_to_databases-1.0.6/connectors_to_databases/PostgreSQL.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.0.6/connectors_to_databases/TypeHinting.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      346 2023-07-17 07:42:19.000000 connectors_to_databases-1.0.6/connectors_to_databases/__init__.py
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      494 2023-07-17 07:31:57.000000 connectors_to_databases-1.0.6/connectors_to_databases/class_use.py
-drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-17 07:42:32.746896 connectors_to_databases-1.0.6/connectors_to_databases.egg-info/
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     4166 2023-07-17 07:42:32.000000 connectors_to_databases-1.0.6/connectors_to_databases.egg-info/PKG-INFO
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      506 2023-07-17 07:42:32.000000 connectors_to_databases-1.0.6/connectors_to_databases.egg-info/SOURCES.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-07-17 07:42:32.000000 connectors_to_databases-1.0.6/connectors_to_databases.egg-info/dependency_links.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)      117 2023-07-17 07:42:32.000000 connectors_to_databases-1.0.6/connectors_to_databases.egg-info/requires.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-07-17 07:42:32.000000 connectors_to_databases-1.0.6/connectors_to_databases.egg-info/top_level.txt
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1076 2023-07-17 06:54:10.000000 connectors_to_databases-1.0.6/pyproject.toml
--rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-07-17 07:42:32.747251 connectors_to_databases-1.0.6/setup.cfg
--rw-r--r--   0 ivankorsakov   (501) staff       (20)     1725 2023-07-17 07:42:19.000000 connectors_to_databases-1.0.6/setup.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-18 05:07:35.498667 connectors_to_databases-1.1.0/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)    11347 2023-02-18 06:59:30.000000 connectors_to_databases-1.1.0/LICENSE.MD
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-18 05:07:35.498545 connectors_to_databases-1.1.0/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1280 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.0/README.md
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-18 05:07:35.497838 connectors_to_databases-1.1.0/connectors_to_databases/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     3984 2023-07-17 10:03:04.000000 connectors_to_databases-1.1.0/connectors_to_databases/BaseOperator.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1161 2023-07-17 10:03:04.000000 connectors_to_databases-1.1.0/connectors_to_databases/ClickHouse.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     7957 2023-07-17 09:10:29.000000 connectors_to_databases-1.1.0/connectors_to_databases/PostgreSQL.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       41 2022-11-15 09:41:17.000000 connectors_to_databases-1.1.0/connectors_to_databases/TypeHinting.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      346 2023-07-17 10:26:40.000000 connectors_to_databases-1.1.0/connectors_to_databases/__init__.py
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      132 2023-07-17 09:59:52.000000 connectors_to_databases-1.1.0/connectors_to_databases/class_use.py
+drwxr-xr-x   0 ivankorsakov   (501) staff       (20)        0 2023-07-18 05:07:35.498387 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     2413 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/PKG-INFO
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      506 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/SOURCES.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)        1 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/dependency_links.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)      140 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/requires.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       24 2023-07-18 05:07:35.000000 connectors_to_databases-1.1.0/connectors_to_databases.egg-info/top_level.txt
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1076 2023-07-17 09:10:29.000000 connectors_to_databases-1.1.0/pyproject.toml
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)       38 2023-07-18 05:07:35.498701 connectors_to_databases-1.1.0/setup.cfg
+-rw-r--r--   0 ivankorsakov   (501) staff       (20)     1760 2023-07-18 05:06:59.000000 connectors_to_databases-1.1.0/setup.py
```

### Comparing `connectors_to_databases-1.0.6/LICENSE.MD` & `connectors_to_databases-1.1.0/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.6/README.md` & `connectors_to_databases-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,44 @@
+Metadata-Version: 2.1
+Name: connectors_to_databases
+Version: 1.1.0
+Summary: Python module for connect with PostgreSQL and ClickHouse 
+Home-page: https://github.com/k0rsakov/connectors_to_databases
+Download-URL: https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
+Author: k0rsakov
+Author-email: korsakov.iyu@gmail.com
+License: Apache License, Version 2.0, see LICENSE file
+Keywords: database,SQL,PostgreSQL,ClickHouse,dataframe
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.MD
+
 # Connector to databases
 
 ![PyPI](https://img.shields.io/pypi/v/connectors-to-databases?color=blueviolet) 
-![Python 3, 3.10, 3.11](https://img.shields.io/pypi/pyversions/clubhouse?color=blueviolet)
-![License](https://img.shields.io/pypi/l/connectors-to-databases?color=blueviolet) 
+![Python](https://img.shields.io/pypi/pyversions/connectors-to-databases?color=blueviolet)
+![License](https://img.shields.io/pypi/l/connectors-to-databases?color=blueviolet)
+
+![PG](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
+![PG](https://img.shields.io/badge/ClickHouse-white?style=for-the-badge&logo=clickhouse&logoColor=yellow)
 
-**Connector to databases** – easy package for connect with database 
-[PostgreSQL](https://github.com/postgres/postgres) and 
-[ClickHouse](https://github.com/ClickHouse/ClickHouse)
+**Connector to databases** – easy package for connect with database:
+- [PostgreSQL](https://github.com/postgres/postgres)
+- [ClickHouse](https://github.com/ClickHouse/ClickHouse)
 
 ## Installation
 
 Install the current version with 
 [PyPI](https://pypi.org/project/connectors-to-databases/):
 
 ```bash
@@ -19,160 +47,19 @@
 
 Or from GitHub:
 
 ```bash
 pip install https://github.com/k0rsakov/connectors_to_databases/archive/refs/heads/main.zip
 ```
 
-## How to use class PostgreSQL
-
-### Creating instance of class
-
-You can create as many database connectors as you want.
-
-```python
-from connectors_to_databases import PostgreSQL
-
-pg = PostgreSQL()
-
-pg_other = PostgreSQL(
-    host='0.0.0.0',
-    port=0,
-    database='main',
-    login='admin',
-    password='admin',
-)
-```
-
-### Check connection to database
-
-```python
-pg.check_connection()
-```
-
-### Creating a table for examples
-
-```python
-pg.execute_script('CREATE TABLE simple_ (id int4)')
-```
-
-### Filling the table with data
-
-```python
-# simple pd.DataFrame
-df = pd.DataFrame(data={'id':[1]})
-
-pg.insert_df(
-    df=df,
-    pg_table_name='simple_'
-)
-```
-
-### Getting data from a table
-
-```python
-pg.execute_to_df(
-    '''select * from simple_'''
-)
-```
-
-### Getting a connector to the database.
-
-It can be used as you need.
-
-```python
-pg.get_uri()
-```
-
-What does the connector look like
-
-```log
-Engine(postgresql://postgres:***@localhost:5432/postgres)
-```
-
-### Delete our `simple_` table
-
-```python
-pg.execute_script('DROP TABLE simple_')
-```
-
-## How to use class ClickHouse
-
-### Creating instance of class
-
-You can create as many database connectors as you want.
-
-```python
-from connectors_to_databases import ClickHouse
-
-ch = ClickHouse()
-
-ch_other = ClickHouse(
-    host='0.0.0.0',
-    port=0,
-    login='admin',
-    password='admin',
-)
-```
-
-### Creating a table for examples
-
-```python
-ch.execute_script(
-    '''
-    CREATE TABLE test 
-    (
-        value Int64
-    ) 
-    ENGINE = MergeTree 
-    ORDER BY value
-    '''
-)
-```
-
-### Filling the table with data
-
-```python
-# simple pd.DataFrame
-df = ch.DataFrame(data={'value':[1]})
-
-ch.insert_df(
-    df=df,
-    pg_table_name='test'
-)
-```
-
-### Getting data from a table
-
-```python
-ch.execute_to_df(
-    '''select * from test'''
-)
-```
-
-### Getting a connector to the database.
-
-It can be used as you need.
-
-```python
-ch.get_uri()
-```
-
-What does the connector look like
-
-```log
-Engine(clickhouse://click:***@localhost:8123/default)
-```
-
-### Delete our `simple_` table
-
-```python
-ch.execute_script('DROP TABLE test')
-```
+## Usage
 
+How to use connections:
+- [ClickHouse.md](doc/ClickHouse.md)
+- [PostgreSQL.md](doc/PostgreSQL.md)
 
 ## Contributing
 
 Bug reports and/or pull requests are welcome
 
 ## License
```

### Comparing `connectors_to_databases-1.0.6/connectors_to_databases/BaseOperator.py` & `connectors_to_databases-1.1.0/connectors_to_databases/BaseOperator.py`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.6/connectors_to_databases/ClickHouse.py` & `connectors_to_databases-1.1.0/connectors_to_databases/ClickHouse.py`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.6/connectors_to_databases/PostgreSQL.py` & `connectors_to_databases-1.1.0/connectors_to_databases/PostgreSQL.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .BaseOperator import BaseOperator
-# from connectors_to_databases.BaseOperator import BaseOperator
+# from .BaseOperator import BaseOperator
+from connectors_to_databases.BaseOperator import BaseOperator
 from urllib.parse import quote
 from typing import Union, Iterable
 
 from sqlalchemy import create_engine, engine
 
 
 class PostgreSQL(BaseOperator):
```

### Comparing `connectors_to_databases-1.0.6/pyproject.toml` & `connectors_to_databases-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connectors_to_databases-1.0.6/setup.py` & `connectors_to_databases-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '1.0.6'
+version = '1.1.0'
 
 with open('README.md', encoding='utf-8-sig') as f:
     long_description = f.read()
 
 setup(
     name='connectors_to_databases',
     version=version,
@@ -26,18 +26,19 @@
     license='Apache License, Version 2.0, see LICENSE file',
     
     # TODO: deprecated psycopg2, clickhouse-sqlalchemy
     packages=['connectors_to_databases'],
     install_requires=[
         'SQLAlchemy==1.4.44',
         'pandas==1.5.1',
+        'psycopg2-binary==2.9.6',
         'psycopg2==2.9.5',
         'clickhouse-sqlalchemy==0.2.3',
         'clickhouse_driver==0.2.5',
-        'ruff==0.0.278'
+        'ruff==0.0.278',
     ],
 
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Developers',
```

