# Comparing `tmp/pgsqlx-1.0.4.tar.gz` & `tmp/pgsqlx-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.0.4.tar", last modified: Tue Jul 18 02:02:53 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.0.5.tar", last modified: Tue Jul 18 02:05:46 2023, max compression
```

## Comparing `pgsqlx-1.0.4.tar` & `pgsqlx-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/pgsqlx/
--rw-rw-rw-   0        0        0      678 2023-07-15 12:19:37.000000 pgsqlx-1.0.4/pgsqlx/constant.py
--rw-rw-rw-   0        0        0    19483 2023-07-18 01:59:21.000000 pgsqlx-1.0.4/pgsqlx/db.py
--rw-rw-rw-   0        0        0    13886 2023-07-17 09:29:32.000000 pgsqlx-1.0.4/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.4/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0    37747 2023-07-17 09:02:03.000000 pgsqlx-1.0.4/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 pgsqlx-1.0.4/pgsqlx/snowflake.py
--rw-rw-rw-   0        0        0     5119 2023-07-14 23:31:12.000000 pgsqlx-1.0.4/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6487 2023-07-17 09:30:08.000000 pgsqlx-1.0.4/pgsqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.4/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4268 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      357 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4268 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-18 02:02:53.000000 pgsqlx-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1203 2023-07-18 02:02:21.000000 pgsqlx-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4268 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      197 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4268 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-18 02:05:46.000000 pgsqlx-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-07-18 02:04:16.000000 pgsqlx-1.0.5/setup.py
```

### Comparing `pgsqlx-1.0.4/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.0.5/pgsqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.4
+Version: 1.0.5
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.0.4/PKG-INFO` & `pgsqlx-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.4
+Version: 1.0.5
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.0.4/README.rst` & `pgsqlx-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.4/setup.py` & `pgsqlx-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
         return fp.read()
 
 long_description = read("README.rst")
 
 setup(
     name='pgsqlx',
-    packages=['pgsqlx'],
+    packages=['source'],
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'psycopg2>=2.7.4',
     ],
-    version='1.0.4',
+    version='1.0.5',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

