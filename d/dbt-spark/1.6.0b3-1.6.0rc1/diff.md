# Comparing `tmp/dbt-spark-1.6.0b3.tar.gz` & `tmp/dbt-spark-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-spark-1.6.0b3.tar", last modified: Fri Jun  9 01:08:22 2023, max compression
+gzip compressed data, was "dbt-spark-1.6.0rc1.tar", last modified: Mon Jul 17 22:45:39 2023, max compression
```

## Comparing `dbt-spark-1.6.0b3.tar` & `dbt-spark-1.6.0rc1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.078732 dbt-spark-1.6.0b3/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.078732 dbt-spark-1.6.0b3/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    19596 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/adapters/spark/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.078732 dbt-spark-1.6.0b3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/apply_grants.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.082733 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 01:08:22.000000 dbt-spark-1.6.0b3/dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:08:22.086733 dbt-spark-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-09 01:08:04.000000 dbt-spark-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.133829 dbt-spark-1.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-07-17 22:45:39.133829 dbt-spark-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.129829 dbt-spark-1.6.0rc1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.129829 dbt-spark-1.6.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.129829 dbt-spark-1.6.0rc1/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22264 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/adapters/spark/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.129829 dbt-spark-1.6.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.129829 dbt-spark-1.6.0rc1/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.129829 dbt-spark-1.6.0rc1/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/apply_grants.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.129829 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/clone.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.129829 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.133829 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:45:39.133829 dbt-spark-1.6.0rc1/dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-07-17 22:45:39.000000 dbt-spark-1.6.0rc1/dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-17 22:45:39.000000 dbt-spark-1.6.0rc1/dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:45:39.000000 dbt-spark-1.6.0rc1/dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:45:39.000000 dbt-spark-1.6.0rc1/dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-17 22:45:39.000000 dbt-spark-1.6.0rc1/dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 22:45:39.000000 dbt-spark-1.6.0rc1/dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:45:39.133829 dbt-spark-1.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-17 22:45:27.000000 dbt-spark-1.6.0rc1/setup.py
```

### Comparing `dbt-spark-1.6.0b3/PKG-INFO` & `dbt-spark-1.6.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.6.0b3
+Version: 1.6.0rc1
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b3 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0rc1 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-spark-1.6.0b3/README.md` & `dbt-spark-1.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/adapters/spark/column.py` & `dbt-spark-1.6.0rc1/dbt/adapters/spark/column.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def translate_type(cls, dtype: str) -> str:
         return dtype
 
     def can_expand_to(self: Self, other_column: Self) -> bool:  # type: ignore
         """returns True if both columns are strings"""
         return self.is_string() and other_column.is_string()
 
-    def literal(self, value):
+    def literal(self, value: Any) -> str:
         return "cast({} as {})".format(value, self.dtype)
 
     @property
     def quoted(self) -> str:
         return "`{}`".format(self.column)
 
     @property
```

### Comparing `dbt-spark-1.6.0b3/dbt/adapters/spark/connections.py` & `dbt-spark-1.6.0rc1/dbt/adapters/spark/connections.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from contextlib import contextmanager
-from typing import Tuple
 
 import dbt.exceptions
 from dbt.adapters.base import Credentials
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import ConnectionState, AdapterResponse
 from dbt.events import AdapterLogger
 from dbt.utils import DECIMALS
@@ -19,18 +18,18 @@
     hive = None
 try:
     import pyodbc
 except ImportError:
     pyodbc = None
 from datetime import datetime
 import sqlparams
-
+from dbt.contracts.connection import Connection
 from hologram.helpers import StrEnum
 from dataclasses import dataclass, field
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union, Tuple, List, Generator, Iterable
 
 try:
     from thrift.transport.TSSLSocket import TSSLSocket
     import thrift
     import ssl
     import sasl
     import thrift_sasl
@@ -41,15 +40,15 @@
 import time
 
 logger = AdapterLogger("Spark")
 
 NUMBERS = DECIMALS + (int, float)
 
 
-def _build_odbc_connnection_string(**kwargs) -> str:
+def _build_odbc_connnection_string(**kwargs: Any) -> str:
     return ";".join([f"{k}={v}" for k, v in kwargs.items()])
 
 
 class SparkConnectionMethod(StrEnum):
     THRIFT = "thrift"
     HTTP = "http"
     ODBC = "odbc"
@@ -74,25 +73,25 @@
     connect_retries: int = 0
     connect_timeout: int = 10
     use_ssl: bool = False
     server_side_parameters: Dict[str, Any] = field(default_factory=dict)
     retry_all: bool = False
 
     @classmethod
-    def __pre_deserialize__(cls, data):
+    def __pre_deserialize__(cls, data: Any) -> Any:
         data = super().__pre_deserialize__(data)
         if "database" not in data:
             data["database"] = None
         return data
 
     @property
-    def cluster_id(self):
+    def cluster_id(self) -> Optional[str]:
         return self.cluster
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         # spark classifies database and schema as the same thing
         if self.database is not None and self.database != self.schema:
             raise dbt.exceptions.DbtRuntimeError(
                 f"    schema: {self.schema} \n"
                 f"    database: {self.database} \n"
                 f"On Spark, database must be omitted or have the same value as"
                 f" schema."
@@ -136,65 +135,72 @@
                     f"{self.method} connection method requires "
                     "additional dependencies. \n"
                     "Install the additional required dependencies with "
                     "`pip install dbt-spark[session]`\n\n"
                     f"ImportError({e.msg})"
                 ) from e
 
+        if self.method != SparkConnectionMethod.SESSION:
+            self.host = self.host.rstrip("/")
+
     @property
-    def type(self):
+    def type(self) -> str:
         return "spark"
 
     @property
-    def unique_field(self):
+    def unique_field(self) -> str:
         return self.host
 
     def _connection_keys(self) -> Tuple[str, ...]:
-        return ("host", "port", "cluster", "endpoint", "schema", "organization")
+        return "host", "port", "cluster", "endpoint", "schema", "organization"
 
 
 class PyhiveConnectionWrapper(object):
     """Wrap a Spark connection in a way that no-ops transactions"""
 
     # https://forums.databricks.com/questions/2157/in-apache-spark-sql-can-we-roll-back-the-transacti.html  # noqa
 
-    def __init__(self, handle):
+    handle: "pyodbc.Connection"
+    _cursor: "Optional[pyodbc.Cursor]"
+
+    def __init__(self, handle: "pyodbc.Connection") -> None:
         self.handle = handle
         self._cursor = None
 
-    def cursor(self):
+    def cursor(self) -> "PyhiveConnectionWrapper":
         self._cursor = self.handle.cursor()
         return self
 
-    def cancel(self):
+    def cancel(self) -> None:
         if self._cursor:
             # Handle bad response in the pyhive lib when
             # the connection is cancelled
             try:
                 self._cursor.cancel()
             except EnvironmentError as exc:
                 logger.debug("Exception while cancelling query: {}".format(exc))
 
-    def close(self):
+    def close(self) -> None:
         if self._cursor:
             # Handle bad response in the pyhive lib when
             # the connection is cancelled
             try:
                 self._cursor.close()
             except EnvironmentError as exc:
                 logger.debug("Exception while closing cursor: {}".format(exc))
         self.handle.close()
 
-    def rollback(self, *args, **kwargs):
+    def rollback(self, *args: Any, **kwargs: Any) -> None:
         logger.debug("NotImplemented: rollback")
 
-    def fetchall(self):
+    def fetchall(self) -> List["pyodbc.Row"]:
+        assert self._cursor, "Cursor not available"
         return self._cursor.fetchall()
 
-    def execute(self, sql, bindings=None):
+    def execute(self, sql: str, bindings: Optional[List[Any]] = None) -> None:
         if sql.strip().endswith(";"):
             sql = sql.strip()[:-1]
 
         # Reaching into the private enumeration here is bad form,
         # but there doesn't appear to be any way to determine that
         # a query has completed executing from the pyhive public API.
         # We need to use an async query + poll here, otherwise our
@@ -208,14 +214,16 @@
         STATE_SUCCESS = [
             ThriftState.FINISHED_STATE,
         ]
 
         if bindings is not None:
             bindings = [self._fix_binding(binding) for binding in bindings]
 
+        assert self._cursor, "Cursor not available"
+
         self._cursor.execute(sql, bindings, async_=True)
         poll_state = self._cursor.poll()
         state = poll_state.operationState
 
         while state in STATE_PENDING:
             logger.debug("Poll status: {}, sleeping".format(state))
 
@@ -241,31 +249,33 @@
             raise dbt.exceptions.DbtDatabaseError(
                 "Query failed with status: {}".format(status_type)
             )
 
         logger.debug("Poll status: {}, query complete".format(state))
 
     @classmethod
-    def _fix_binding(cls, value):
+    def _fix_binding(cls, value: Any) -> Union[float, str]:
         """Convert complex datatypes to primitives that can be loaded by
         the Spark driver"""
         if isinstance(value, NUMBERS):
             return float(value)
         elif isinstance(value, datetime):
             return value.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
         else:
             return value
 
     @property
-    def description(self):
+    def description(self) -> Tuple[Tuple[str, Any, int, int, int, int, bool]]:
+        assert self._cursor, "Cursor not available"
         return self._cursor.description
 
 
 class PyodbcConnectionWrapper(PyhiveConnectionWrapper):
-    def execute(self, sql, bindings=None):
+    def execute(self, sql: str, bindings: Optional[List[Any]] = None) -> None:
+        assert self._cursor, "Cursor not available"
         if sql.strip().endswith(";"):
             sql = sql.strip()[:-1]
         # pyodbc does not handle a None type binding!
         if bindings is None:
             self._cursor.execute(sql)
         else:
             # pyodbc only supports `qmark` sql params!
@@ -278,15 +288,15 @@
     TYPE = "spark"
 
     SPARK_CLUSTER_HTTP_PATH = "/sql/protocolv1/o/{organization}/{cluster}"
     SPARK_SQL_ENDPOINT_HTTP_PATH = "/sql/1.0/endpoints/{endpoint}"
     SPARK_CONNECTION_URL = "{host}:{port}" + SPARK_CLUSTER_HTTP_PATH
 
     @contextmanager
-    def exception_handler(self, sql):
+    def exception_handler(self, sql: str) -> Generator[None, None, None]:
         try:
             yield
 
         except Exception as exc:
             logger.debug("Error while running:\n{}".format(sql))
             logger.debug(exc)
             if len(exc.args) == 0:
@@ -295,49 +305,49 @@
             thrift_resp = exc.args[0]
             if hasattr(thrift_resp, "status"):
                 msg = thrift_resp.status.errorMessage
                 raise dbt.exceptions.DbtRuntimeError(msg)
             else:
                 raise dbt.exceptions.DbtRuntimeError(str(exc))
 
-    def cancel(self, connection):
+    def cancel(self, connection: Connection) -> None:
         connection.handle.cancel()
 
     @classmethod
-    def get_response(cls, cursor) -> AdapterResponse:
+    def get_response(cls, cursor: Any) -> AdapterResponse:
         # https://github.com/dbt-labs/dbt-spark/issues/142
         message = "OK"
         return AdapterResponse(_message=message)
 
     # No transactions on Spark....
-    def add_begin_query(self, *args, **kwargs):
+    def add_begin_query(self, *args: Any, **kwargs: Any) -> None:
         logger.debug("NotImplemented: add_begin_query")
 
-    def add_commit_query(self, *args, **kwargs):
+    def add_commit_query(self, *args: Any, **kwargs: Any) -> None:
         logger.debug("NotImplemented: add_commit_query")
 
-    def commit(self, *args, **kwargs):
+    def commit(self, *args: Any, **kwargs: Any) -> None:
         logger.debug("NotImplemented: commit")
 
-    def rollback(self, *args, **kwargs):
+    def rollback(self, *args: Any, **kwargs: Any) -> None:
         logger.debug("NotImplemented: rollback")
 
     @classmethod
-    def validate_creds(cls, creds, required):
+    def validate_creds(cls, creds: Any, required: Iterable[str]) -> None:
         method = creds.method
 
         for key in required:
             if not hasattr(creds, key):
                 raise dbt.exceptions.DbtProfileError(
                     "The config '{}' is required when using the {} method"
                     " to connect to Spark".format(key, method)
                 )
 
     @classmethod
-    def open(cls, connection):
+    def open(cls, connection: Connection) -> Connection:
         if connection.state == ConnectionState.OPEN:
             logger.debug("Connection is already open, skipping open.")
             return connection
 
         creds = connection.credentials
         exc = None
 
@@ -446,15 +456,15 @@
                     handle = PyodbcConnectionWrapper(conn)
                 elif creds.method == SparkConnectionMethod.SESSION:
                     from .session import (  # noqa: F401
                         Connection,
                         SessionConnectionWrapper,
                     )
 
-                    handle = SessionConnectionWrapper(Connection())
+                    handle = SessionConnectionWrapper(Connection())  # type: ignore
                 else:
                     raise dbt.exceptions.DbtProfileError(
                         f"invalid credential method: {creds.method}"
                     )
                 break
             except Exception as e:
                 exc = e
@@ -483,15 +493,15 @@
                         f"({i} of {creds.connect_retries})"
                     )
                     logger.warning(msg)
                     time.sleep(creds.connect_timeout)
                 else:
                     raise dbt.exceptions.FailedToConnectError("failed to connect") from e
         else:
-            raise exc
+            raise exc  # type: ignore
 
         connection.handle = handle
         connection.state = ConnectionState.OPEN
         return connection
 
     @classmethod
     def data_type_code_to_name(cls, type_code: Union[type, str]) -> str:  # type: ignore
@@ -503,15 +513,22 @@
         :rtype: str
         """
         if isinstance(type_code, str):
             return type_code
         return type_code.__name__.upper()
 
 
-def build_ssl_transport(host, port, username, auth, kerberos_service_name, password=None):
+def build_ssl_transport(
+    host: str,
+    port: int,
+    username: str,
+    auth: str,
+    kerberos_service_name: str,
+    password: Optional[str] = None,
+) -> "thrift_sasl.TSaslClientTransport":
     transport = None
     if port is None:
         port = 10000
     if auth is None:
         auth = "NONE"
     socket = TSSLSocket(host, port, cert_reqs=ssl.CERT_NONE)
     if auth == "NOSASL":
@@ -527,15 +544,15 @@
         else:
             sasl_auth = "PLAIN"
             if password is None:
                 # Password doesn't matter in NONE mode, just needs
                 # to be nonempty.
                 password = "x"
 
-        def sasl_factory():
+        def sasl_factory() -> sasl.Client:
             sasl_client = sasl.Client()
             sasl_client.setAttr("host", host)
             if sasl_auth == "GSSAPI":
                 sasl_client.setAttr("service", kerberos_service_name)
             elif sasl_auth == "PLAIN":
                 sasl_client.setAttr("username", username)
                 sasl_client.setAttr("password", password)
```

### Comparing `dbt-spark-1.6.0b3/dbt/adapters/spark/impl.py` & `dbt-spark-1.6.0rc1/dbt/adapters/spark/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import re
 from concurrent.futures import Future
 from dataclasses import dataclass
-from typing import Any, Dict, Iterable, List, Optional, Union, Type, Tuple, Callable
+from typing import Any, Dict, Iterable, List, Optional, Union, Type, Tuple, Callable, Set
+
+from dbt.adapters.base.relation import InformationSchema
+from dbt.contracts.graph.manifest import Manifest
 
 from typing_extensions import TypeAlias
 
 import agate
 
 import dbt
 import dbt.exceptions
@@ -105,35 +108,35 @@
     AdapterSpecificConfigs: TypeAlias = SparkConfig
 
     @classmethod
     def date_function(cls) -> str:
         return "current_timestamp()"
 
     @classmethod
-    def convert_text_type(cls, agate_table, col_idx):
+    def convert_text_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "string"
 
     @classmethod
-    def convert_number_type(cls, agate_table, col_idx):
+    def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))
         return "double" if decimals else "bigint"
 
     @classmethod
-    def convert_date_type(cls, agate_table, col_idx):
+    def convert_date_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "date"
 
     @classmethod
-    def convert_time_type(cls, agate_table, col_idx):
+    def convert_time_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "time"
 
     @classmethod
-    def convert_datetime_type(cls, agate_table, col_idx):
+    def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "timestamp"
 
-    def quote(self, identifier):
+    def quote(self, identifier: str) -> str:  # type: ignore
         return "`{}`".format(identifier)
 
     def _get_relation_information(self, row: agate.Row) -> RelationInfo:
         """relation info was fetched with SHOW TABLES EXTENDED"""
         try:
             _schema, name, _, information = row
         except ValueError:
@@ -340,15 +343,15 @@
             # convert SparkColumns into catalog dicts
             as_dict = column.to_column_dict()
             as_dict["column_name"] = as_dict.pop("column", None)
             as_dict["column_type"] = as_dict.pop("dtype")
             as_dict["table_database"] = None
             yield as_dict
 
-    def get_catalog(self, manifest):
+    def get_catalog(self, manifest: Manifest) -> Tuple[agate.Table, List[Exception]]:
         schema_map = self._get_catalog_schemas(manifest)
         if len(schema_map) > 1:
             raise dbt.exceptions.CompilationError(
                 f"Expected only one database in get_catalog, found " f"{list(schema_map)}"
             )
 
         with executor(self.config) as tpe:
@@ -366,17 +369,17 @@
                         )
                     )
             catalogs, exceptions = catch_as_completed(futures)
         return catalogs, exceptions
 
     def _get_one_catalog(
         self,
-        information_schema,
-        schemas,
-        manifest,
+        information_schema: InformationSchema,
+        schemas: Set[str],
+        manifest: Manifest,
     ) -> agate.Table:
         if len(schemas) != 1:
             raise dbt.exceptions.CompilationError(
                 f"Expected only one schema in spark _get_one_catalog, found " f"{schemas}"
             )
 
         database = information_schema.database
@@ -384,15 +387,15 @@
 
         columns: List[Dict[str, Any]] = []
         for relation in self.list_relations(database, schema):
             logger.debug("Getting table schema for relation {}", str(relation))
             columns.extend(self._get_columns_for_catalog(relation))
         return agate.Table.from_object(columns, column_types=DEFAULT_TYPE_TESTER)
 
-    def check_schema_exists(self, database, schema):
+    def check_schema_exists(self, database: str, schema: str) -> bool:
         results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database})
 
         exists = True if schema in [row[0] for row in results] else False
         return exists
 
     def get_rows_different_sql(
         self,
@@ -421,15 +424,15 @@
         )
 
         return sql
 
     # This is for use in the test suite
     # Spark doesn't have 'commit' and 'rollback', so this override
     # doesn't include those commands.
-    def run_sql_for_tests(self, sql, fetch, conn):
+    def run_sql_for_tests(self, sql, fetch, conn):  # type: ignore
         cursor = conn.handle.cursor()
         try:
             cursor.execute(sql)
             if fetch == "one":
                 if hasattr(cursor, "fetchone"):
                     return cursor.fetchone()
                 else:
@@ -473,15 +476,15 @@
             if object_type == "TABLE" and privilege != "OWN":
                 if privilege in grants_dict.keys():
                     grants_dict[privilege].append(grantee)
                 else:
                     grants_dict.update({privilege: [grantee]})
         return grants_dict
 
-    def debug_query(self):
+    def debug_query(self) -> None:
         """Override for DebugTask method"""
         self.execute("select 1 as id")
 
 
 # spark does something interesting with joins when both tables have the same
 # static values for the join condition and complains that the join condition is
 # "trivial". Which is true, though it seems like an unreasonable cause for
```

### Comparing `dbt-spark-1.6.0b3/dbt/adapters/spark/python_submissions.py` & `dbt-spark-1.6.0rc1/dbt/adapters/spark/python_submissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import base64
 import time
 import requests
-from typing import Any, Dict
+from typing import Any, Dict, Callable, Iterable
 import uuid
 
 import dbt.exceptions
 from dbt.adapters.base import PythonJobHelper
 from dbt.adapters.spark import SparkCredentials
 from dbt.adapters.spark import __version__
 
@@ -145,26 +145,26 @@
     def submit(self, compiled_code: str) -> None:
         raise NotImplementedError(
             "BasePythonJobHelper is an abstract class and you should implement submit method."
         )
 
     def polling(
         self,
-        status_func,
-        status_func_kwargs,
-        get_state_func,
-        terminal_states,
-        expected_end_state,
-        get_state_msg_func,
+        status_func: Callable,
+        status_func_kwargs: Dict,
+        get_state_func: Callable,
+        terminal_states: Iterable[str],
+        expected_end_state: str,
+        get_state_msg_func: Callable,
     ) -> Dict:
         state = None
         start = time.time()
         exceeded_timeout = False
-        response = {}
-        while state not in terminal_states:
+        response: Dict = {}
+        while state is None or state not in terminal_states:
             if time.time() - start > self.timeout:
                 exceeded_timeout = True
                 break
             # should we do exponential backoff?
             time.sleep(self.polling_interval)
             response = status_func(**status_func_kwargs)
             state = get_state_func(response)
```

### Comparing `dbt-spark-1.6.0b3/dbt/adapters/spark/relation.py` & `dbt-spark-1.6.0rc1/dbt/adapters/spark/relation.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,18 +32,18 @@
     quote_character: str = "`"
     is_delta: Optional[bool] = None
     is_hudi: Optional[bool] = None
     is_iceberg: Optional[bool] = None
     # TODO: make this a dict everywhere
     information: Optional[str] = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.database != self.schema and self.database:
             raise DbtRuntimeError("Cannot set database in spark!")
 
-    def render(self):
+    def render(self) -> str:
         if self.include_policy.database and self.include_policy.schema:
             raise DbtRuntimeError(
                 "Got a spark relation with schema and database set to "
                 "include, but only one can be set"
             )
         return super().render()
```

### Comparing `dbt-spark-1.6.0b3/dbt/adapters/spark/session.py` & `dbt-spark-1.6.0rc1/dbt/adapters/spark/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Spark session integration."""
 
 from __future__ import annotations
 
 import datetime as dt
 from types import TracebackType
-from typing import Any, List, Optional, Tuple
+from typing import Any, List, Optional, Tuple, Union
 
 from dbt.events import AdapterLogger
 from dbt.utils import DECIMALS
 from pyspark.sql import DataFrame, Row, SparkSession
 
 
 logger = AdapterLogger("Spark")
@@ -168,53 +168,59 @@
         out : Cursor
             The cursor.
         """
         return Cursor()
 
 
 class SessionConnectionWrapper(object):
-    """Connection wrapper for the sessoin connection method."""
+    """Connection wrapper for the session connection method."""
 
-    def __init__(self, handle):
+    handle: Connection
+    _cursor: Optional[Cursor]
+
+    def __init__(self, handle: Connection) -> None:
         self.handle = handle
         self._cursor = None
 
-    def cursor(self):
+    def cursor(self) -> "SessionConnectionWrapper":
         self._cursor = self.handle.cursor()
         return self
 
-    def cancel(self):
+    def cancel(self) -> None:
         logger.debug("NotImplemented: cancel")
 
-    def close(self):
+    def close(self) -> None:
         if self._cursor:
             self._cursor.close()
 
-    def rollback(self, *args, **kwargs):
+    def rollback(self, *args: Any, **kwargs: Any) -> None:
         logger.debug("NotImplemented: rollback")
 
-    def fetchall(self):
+    def fetchall(self) -> Optional[List[Row]]:
+        assert self._cursor, "Cursor not available"
         return self._cursor.fetchall()
 
-    def execute(self, sql, bindings=None):
+    def execute(self, sql: str, bindings: Optional[List[Any]] = None) -> None:
         if sql.strip().endswith(";"):
             sql = sql.strip()[:-1]
 
+        assert self._cursor, "Cursor not available"
         if bindings is None:
             self._cursor.execute(sql)
         else:
             bindings = [self._fix_binding(binding) for binding in bindings]
             self._cursor.execute(sql, *bindings)
 
     @property
-    def description(self):
+    def description(self) -> List[Tuple[str, str, None, None, None, None, bool]]:
+        assert self._cursor, "Cursor not available"
         return self._cursor.description
 
     @classmethod
-    def _fix_binding(cls, value):
+    def _fix_binding(cls, value: Any) -> Union[str, float]:
         """Convert complex datatypes to primitives that can be loaded by
         the Spark driver"""
         if isinstance(value, NUMBERS):
             return float(value)
         elif isinstance(value, dt.datetime):
             return f"'{value.strftime('%Y-%m-%d %H:%M:%S.%f')[:-3]}'"
         else:
```

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/adapters.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/apply_grants.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/incremental/validate.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/seed.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/snapshot.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/materializations/table.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/dateadd.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/datediff.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/macros/utils/listagg.sql` & `dbt-spark-1.6.0rc1/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt/include/spark/profile_template.yml` & `dbt-spark-1.6.0rc1/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.6.0b3/dbt_spark.egg-info/PKG-INFO` & `dbt-spark-1.6.0rc1/dbt_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.6.0b3
+Version: 1.6.0rc1
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b3 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0rc1 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-spark-1.6.0b3/dbt_spark.egg-info/SOURCES.txt` & `dbt-spark-1.6.0rc1/dbt_spark.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 dbt/adapters/spark/relation.py
 dbt/adapters/spark/session.py
 dbt/include/spark/__init__.py
 dbt/include/spark/dbt_project.yml
 dbt/include/spark/profile_template.yml
 dbt/include/spark/macros/adapters.sql
 dbt/include/spark/macros/apply_grants.sql
+dbt/include/spark/macros/materializations/clone.sql
 dbt/include/spark/macros/materializations/seed.sql
 dbt/include/spark/macros/materializations/snapshot.sql
 dbt/include/spark/macros/materializations/table.sql
 dbt/include/spark/macros/materializations/view.sql
 dbt/include/spark/macros/materializations/incremental/column_helpers.sql
 dbt/include/spark/macros/materializations/incremental/incremental.sql
 dbt/include/spark/macros/materializations/incremental/strategies.sql
```

### Comparing `dbt-spark-1.6.0b3/setup.py` & `dbt-spark-1.6.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-spark"
-package_version = "1.6.0b3"
+package_version = "1.6.0rc1"
 dbt_core_version = _get_dbt_core_version()
 description = """The Apache Spark adapter plugin for dbt"""
 
 odbc_extras = ["pyodbc~=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.17.0",
```

