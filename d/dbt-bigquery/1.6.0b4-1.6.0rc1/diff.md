# Comparing `tmp/dbt-bigquery-1.6.0b4.tar.gz` & `tmp/dbt-bigquery-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-bigquery-1.6.0b4.tar", last modified: Fri Jun 23 02:09:18 2023, max compression
+gzip compressed data, was "dbt-bigquery-1.6.0rc1.tar", last modified: Mon Jul 17 23:27:53 2023, max compression
```

## Comparing `dbt-bigquery-1.6.0b4.tar` & `dbt-bigquery-1.6.0rc1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.602444 dbt-bigquery-1.6.0b4/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.598444 dbt-bigquery-1.6.0b4/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    39652 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.598444 dbt-bigquery-1.6.0b4/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/etc.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/copy.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.610444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.610444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.829978 dbt-bigquery-1.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-17 23:27:53.829978 dbt-bigquery-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.821977 dbt-bigquery-1.6.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.821977 dbt-bigquery-1.6.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.821977 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28070 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40300 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.821977 dbt-bigquery-1.6.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.825977 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.825977 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.825977 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/etc.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.825977 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/copy.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.825977 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.825977 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.829978 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/dbt/include/bigquery/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:27:53.829978 dbt-bigquery-1.6.0rc1/dbt_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-17 23:27:53.000000 dbt-bigquery-1.6.0rc1/dbt_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-17 23:27:53.000000 dbt-bigquery-1.6.0rc1/dbt_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:27:53.000000 dbt-bigquery-1.6.0rc1/dbt_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:27:53.000000 dbt-bigquery-1.6.0rc1/dbt_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 23:27:53.000000 dbt-bigquery-1.6.0rc1/dbt_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 23:27:53.000000 dbt-bigquery-1.6.0rc1/dbt_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:27:53.829978 dbt-bigquery-1.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-17 23:27:39.000000 dbt-bigquery-1.6.0rc1/setup.py
```

### Comparing `dbt-bigquery-1.6.0b4/LICENSE.md` & `dbt-bigquery-1.6.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/PKG-INFO` & `dbt-bigquery-1.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.6.0b4
+Version: 1.6.0rc1
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b4 Summary: The Bigquery
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0rc1 Summary: The
+Bigquery adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+bigquery Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.6.0b4/README.md` & `dbt-bigquery-1.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/__init__.py` & `dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/column.py` & `dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/column.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from dataclasses import dataclass
 from typing import Optional, List, TypeVar, Iterable, Type, Any, Dict, Union
 
 from dbt.adapters.base.column import Column
 
 from google.cloud.bigquery import SchemaField
 
+_PARENT_DATA_TYPE_KEY = "__parent_data_type"
+
 Self = TypeVar("Self", bound="BigQueryColumn")
 
 
 @dataclass(init=False)
 class BigQueryColumn(Column):
     TYPE_LABELS = {
         "STRING": "STRING",
@@ -127,15 +129,15 @@
 
         return SchemaField(self.name, self.dtype, self.mode, **kwargs)  # type: ignore[arg-type]
 
 
 def get_nested_column_data_types(
     columns: Dict[str, Dict[str, Any]],
     constraints: Optional[Dict[str, str]] = None,
-) -> Dict[str, Dict[str, str]]:
+) -> Dict[str, Dict[str, Optional[str]]]:
     """
     columns:
         * Dictionary where keys are of flat columns names and values are dictionary of column attributes
         * column names with "." indicate a nested column within a STRUCT type
         * e.g. {"a": {"name": "a", "data_type": "string", ...}}
     constraints:
         * Dictionary where keys are flat column names and values are rendered constraints for the column
@@ -155,24 +157,24 @@
     returns: {
         "a": {"name": "a", "data_type": "string"},
         "b": {"name": "b": "data_type": "struct<nested string, nested2 string>}
     }
     """
     constraints = constraints or {}
 
-    nested_column_data_types: Dict[str, Union[str, Dict]] = {}
+    nested_column_data_types: Dict[str, Optional[Union[str, Dict]]] = {}
     for column in columns.values():
         _update_nested_column_data_types(
             column["name"],
-            column["data_type"],
+            column.get("data_type"),
             constraints.get(column["name"]),
             nested_column_data_types,
         )
 
-    formatted_nested_column_data_types: Dict[str, Dict[str, str]] = {}
+    formatted_nested_column_data_types: Dict[str, Dict[str, Optional[str]]] = {}
     for column_name, unformatted_column_type in nested_column_data_types.items():
         formatted_nested_column_data_types[column_name] = {
             "name": column_name,
             "data_type": _format_nested_data_type(unformatted_column_type),
         }
 
     # add column configs back to flat columns
@@ -187,17 +189,17 @@
             )
 
     return formatted_nested_column_data_types
 
 
 def _update_nested_column_data_types(
     column_name: str,
-    column_data_type: str,
+    column_data_type: Optional[str],
     column_rendered_constraint: Optional[str],
-    nested_column_data_types: Dict[str, Union[str, Dict]],
+    nested_column_data_types: Dict[str, Optional[Union[str, Dict]]],
 ) -> None:
     """
     Recursively update nested_column_data_types given a column_name, column_data_type, and optional column_rendered_constraint.
 
     Examples:
     >>> nested_column_data_types = {}
     >>> BigQueryAdapter._update_nested_column_data_types("a", "string", "not_null", nested_column_data_types)
@@ -211,49 +213,90 @@
     {"a": "string not null", "b": {"c": "string not null", "d": "string"}}
     """
     column_name_parts = column_name.split(".")
     root_column_name = column_name_parts[0]
 
     if len(column_name_parts) == 1:
         # Base case: column is not nested - store its data_type concatenated with constraint if provided.
-        nested_column_data_types[root_column_name] = (
-            column_data_type
-            if column_rendered_constraint is None
-            else f"{column_data_type} {column_rendered_constraint}"
+        column_data_type_and_constraints = (
+            (
+                column_data_type
+                if column_rendered_constraint is None
+                else f"{column_data_type} {column_rendered_constraint}"
+            )
+            if column_data_type
+            else None
         )
+
+        if existing_nested_column_data_type := nested_column_data_types.get(root_column_name):
+            assert isinstance(existing_nested_column_data_type, dict)  # keeping mypy happy
+            # entry could already exist if this is a parent column -- preserve the parent data type under "_PARENT_DATA_TYPE_KEY"
+            existing_nested_column_data_type.update(
+                {_PARENT_DATA_TYPE_KEY: column_data_type_and_constraints}
+            )
+        else:
+            nested_column_data_types.update({root_column_name: column_data_type_and_constraints})
     else:
-        # Initialize nested dictionary
-        if root_column_name not in nested_column_data_types:
-            nested_column_data_types[root_column_name] = {}
+        parent_data_type = nested_column_data_types.get(root_column_name)
+        if isinstance(parent_data_type, dict):
+            # nested dictionary already initialized
+            pass
+        elif parent_data_type is None:
+            # initialize nested dictionary
+            nested_column_data_types.update({root_column_name: {}})
+        else:
+            # a parent specified its base type -- preserve its data_type and potential rendered constraints
+            # this is used to specify a top-level 'struct' or 'array' field with its own description, constraints, etc
+            nested_column_data_types.update(
+                {root_column_name: {_PARENT_DATA_TYPE_KEY: parent_data_type}}
+            )
 
         # Recursively process rest of remaining column name
         remaining_column_name = ".".join(column_name_parts[1:])
         remaining_column_data_types = nested_column_data_types[root_column_name]
         assert isinstance(remaining_column_data_types, dict)  # keeping mypy happy
         _update_nested_column_data_types(
             remaining_column_name,
             column_data_type,
             column_rendered_constraint,
             remaining_column_data_types,
         )
 
 
-def _format_nested_data_type(unformatted_nested_data_type: Union[str, Dict[str, Any]]) -> str:
+def _format_nested_data_type(
+    unformatted_nested_data_type: Optional[Union[str, Dict[str, Any]]]
+) -> Optional[str]:
     """
     Recursively format a (STRUCT) data type given an arbitrarily nested data type structure.
 
     Examples:
     >>> BigQueryAdapter._format_nested_data_type("string")
     'string'
     >>> BigQueryAdapter._format_nested_data_type({'c': 'string not_null', 'd': 'string'})
     'struct<c string not_null, d string>'
     >>> BigQueryAdapter._format_nested_data_type({'c': 'string not_null', 'd': {'e': 'string'}})
     'struct<c string not_null, d struct<e string>>'
     """
-    if isinstance(unformatted_nested_data_type, str):
+    if unformatted_nested_data_type is None:
+        return None
+    elif isinstance(unformatted_nested_data_type, str):
         return unformatted_nested_data_type
     else:
+        parent_data_type, *parent_constraints = unformatted_nested_data_type.pop(
+            _PARENT_DATA_TYPE_KEY, ""
+        ).split() or [None]
+
         formatted_nested_types = [
-            f"{column_name} {_format_nested_data_type(column_type)}"
+            f"{column_name} {_format_nested_data_type(column_type) or ''}".strip()
             for column_name, column_type in unformatted_nested_data_type.items()
         ]
-        return f"""struct<{", ".join(formatted_nested_types)}>"""
+
+        formatted_nested_type = f"""struct<{", ".join(formatted_nested_types)}>"""
+
+        if parent_data_type and parent_data_type.lower() == "array":
+            formatted_nested_type = f"""array<{formatted_nested_type}>"""
+
+        if parent_constraints:
+            parent_constraints = " ".join(parent_constraints)
+            formatted_nested_type = f"""{formatted_nested_type} {parent_constraints}"""
+
+        return formatted_nested_type
```

### Comparing `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/connections.py` & `dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,20 @@
         "dataset": "schema",
         "target_project": "target_database",
         "target_dataset": "target_schema",
         "retries": "job_retries",
         "timeout_seconds": "job_execution_timeout_seconds",
     }
 
+    def __post_init__(self):
+        if self.keyfile_json and "private_key" in self.keyfile_json:
+            self.keyfile_json["private_key"] = self.keyfile_json["private_key"].replace(
+                "\\n", "\n"
+            )
+
     @property
     def type(self):
         return "bigquery"
 
     @property
     def unique_field(self):
         return self.database
@@ -417,15 +423,21 @@
         return credentials.job_retry_deadline_seconds
 
     @classmethod
     def get_table_from_response(cls, resp):
         column_names = [field.name for field in resp.schema]
         return agate_helper.table_from_data_flat(resp, column_names)
 
-    def raw_execute(self, sql, use_legacy_sql=False, limit: Optional[int] = None):
+    def raw_execute(
+        self,
+        sql,
+        use_legacy_sql=False,
+        limit: Optional[int] = None,
+        dry_run: bool = False,
+    ):
         conn = self.get_thread_connection()
         client = conn.handle
 
         fire_event(SQLQuery(conn_name=conn.name, sql=sql))
         if (
             hasattr(self.profile, "query_comment")
             and self.profile.query_comment
@@ -435,15 +447,19 @@
             labels = self._labels_from_query_comment(query_comment.comment)
         else:
             labels = {}
 
         if active_user:
             labels["dbt_invocation_id"] = active_user.invocation_id
 
-        job_params = {"use_legacy_sql": use_legacy_sql, "labels": labels}
+        job_params = {
+            "use_legacy_sql": use_legacy_sql,
+            "labels": labels,
+            "dry_run": dry_run,
+        }
 
         priority = conn.credentials.priority
         if priority == Priority.Batch:
             job_params["priority"] = google.cloud.bigquery.QueryPriority.BATCH
         else:
             job_params["priority"] = google.cloud.bigquery.QueryPriority.INTERACTIVE
 
@@ -529,31 +545,59 @@
             num_rows_formatted = self.format_rows_number(num_rows)
             message = f"{code} ({num_rows_formatted} rows, {processed_bytes} processed)"
         elif bytes_processed is not None:
             message = f"{code} ({processed_bytes} processed)"
         else:
             message = f"{code}"
 
-        if location is not None and job_id is not None and project_id is not None:
-            logger.debug(self._bq_job_link(location, project_id, job_id))
-
         response = BigQueryAdapterResponse(  # type: ignore[call-arg]
             _message=message,
             rows_affected=num_rows,
             code=code,
             bytes_processed=bytes_processed,
             bytes_billed=bytes_billed,
             location=location,
             project_id=project_id,
             job_id=job_id,
             slot_ms=slot_ms,
         )
 
         return response, table
 
+    def dry_run(self, sql: str) -> BigQueryAdapterResponse:
+        """Run the given sql statement with the `dry_run` job parameter set.
+
+        This will allow BigQuery to validate the SQL and immediately return job cost
+        estimates, which we capture in the BigQueryAdapterResponse. Invalid SQL
+        will result in an exception.
+        """
+        sql = self._add_query_comment(sql)
+        query_job, _ = self.raw_execute(sql, dry_run=True)
+
+        # TODO: Factor this repetitive block out into a factory method on
+        # BigQueryAdapterResponse
+        message = f"Ran dry run query for statement of type {query_job.statement_type}"
+        bytes_billed = query_job.total_bytes_billed
+        processed_bytes = self.format_bytes(query_job.total_bytes_processed)
+        location = query_job.location
+        project_id = query_job.project
+        job_id = query_job.job_id
+        slot_ms = query_job.slot_millis
+
+        return BigQueryAdapterResponse(
+            _message=message,
+            code="DRY RUN",
+            bytes_billed=bytes_billed,
+            bytes_processed=processed_bytes,
+            location=location,
+            project_id=project_id,
+            job_id=job_id,
+            slot_ms=slot_ms,
+        )
+
     @staticmethod
     def _bq_job_link(location, project_id, job_id) -> str:
         return f"https://console.cloud.google.com/bigquery?project={project_id}&j=bq:{location}:{job_id}&page=queryresults"
 
     def get_partitions_metadata(self, table):
         def standard_to_legacy(table):
             return table.project + ":" + table.dataset + "." + table.identifier
@@ -658,14 +702,24 @@
         job_execution_timeout=None,
         limit: Optional[int] = None,
     ):
         """Query the client and wait for results."""
         # Cannot reuse job_config if destination is set and ddl is used
         job_config = google.cloud.bigquery.QueryJobConfig(**job_params)
         query_job = client.query(query=sql, job_config=job_config, timeout=job_creation_timeout)
+
+        if (
+            query_job.location is not None
+            and query_job.job_id is not None
+            and query_job.project is not None
+        ):
+            logger.debug(
+                self._bq_job_link(query_job.location, query_job.project, query_job.job_id)
+            )
+
         iterator = query_job.result(max_results=limit, timeout=job_execution_timeout)
 
         return query_job, iterator
 
     def _retry_and_handle(self, msg, conn, fn):
         """retry a function call within the context of exception_handler."""
```

### Comparing `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/dataset.py` & `dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,44 @@
 from google.cloud.bigquery import Dataset, AccessEntry
 
 from dbt.events import AdapterLogger
 
 logger = AdapterLogger("BigQuery")
 
 
-def add_access_entry_to_dataset(dataset: Dataset, access_entry: AccessEntry) -> Dataset:
-    """Idempotently adds an access entry to a dataset
+def is_access_entry_in_dataset(dataset: Dataset, access_entry: AccessEntry) -> bool:
+    """Check if the access entry already exists in the dataset.
 
     Args:
         dataset (Dataset): the dataset to be updated
         access_entry (AccessEntry): the access entry to be added to the dataset
 
     Returns:
-        Dataset
+        bool: True if entry exists in dataset, False otherwise
     """
     access_entries: List[AccessEntry] = dataset.access_entries
     # we can't simply check if an access entry is in the list as the current equality check
     # does not work because the locally created AccessEntry can have extra properties.
     for existing_entry in access_entries:
         role_match = existing_entry.role == access_entry.role
         entity_type_match = existing_entry.entity_type == access_entry.entity_type
         property_match = existing_entry._properties.items() <= access_entry._properties.items()
         if role_match and entity_type_match and property_match:
-            logger.warning(f"Access entry {access_entry} " f"already exists in dataset")
-            return dataset
+            return True
+    return False
+
+
+def add_access_entry_to_dataset(dataset: Dataset, access_entry: AccessEntry) -> Dataset:
+    """Adds an access entry to a dataset, always use access_entry_present_in_dataset to check
+    if the access entry already exists before calling this function.
+
+    Args:
+        dataset (Dataset): the dataset to be updated
+        access_entry (AccessEntry): the access entry to be added to the dataset
+
+    Returns:
+        Dataset: the updated dataset
+    """
+    access_entries: List[AccessEntry] = dataset.access_entries
     access_entries.append(access_entry)
     dataset.access_entries = access_entries
     return dataset
```

### Comparing `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/gcloud.py` & `dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/gcloud.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/impl.py` & `dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 import threading
 from typing import Dict, List, Optional, Any, Set, Union, Type
 
+from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.graph.nodes import ColumnLevelConstraint, ModelLevelConstraint, ConstraintType  # type: ignore
 from dbt.dataclass_schema import dbtClassMixin, ValidationError
 
 import dbt.deprecations
 import dbt.exceptions
 import dbt.clients.agate_helper
 
@@ -21,15 +22,15 @@
     PythonJobHelper,
 )
 
 from dbt.adapters.cache import _make_ref_key_dict  # type: ignore
 
 from dbt.adapters.bigquery.column import get_nested_column_data_types
 from dbt.adapters.bigquery.relation import BigQueryRelation
-from dbt.adapters.bigquery.dataset import add_access_entry_to_dataset
+from dbt.adapters.bigquery.dataset import add_access_entry_to_dataset, is_access_entry_in_dataset
 from dbt.adapters.bigquery import BigQueryColumn
 from dbt.adapters.bigquery import BigQueryConnectionManager
 from dbt.adapters.bigquery.python_submissions import (
     ClusterDataprocHelper,
     ServerlessDataProcHelper,
 )
 from dbt.adapters.bigquery.connections import BigQueryAdapterResponse
@@ -296,15 +297,15 @@
 
     @available.parse(lambda *a, **k: {})
     @classmethod
     def nest_column_data_types(
         cls,
         columns: Dict[str, Dict[str, Any]],
         constraints: Optional[Dict[str, str]] = None,
-    ) -> Dict[str, Dict[str, str]]:
+    ) -> Dict[str, Dict[str, Optional[str]]]:
         return get_nested_column_data_types(columns, constraints)
 
     def get_columns_in_relation(self, relation: BigQueryRelation) -> List[BigQueryColumn]:
         try:
             table = self.connections.get_bq_table(
                 database=relation.database, schema=relation.schema, identifier=relation.identifier
             )
@@ -895,16 +896,20 @@
         grant_target = GrantTarget.from_dict(grant_target_dict)
         if entity_type == "view":
             entity = self.get_table_ref_from_relation(entity).to_api_repr()
         with _dataset_lock:
             dataset_ref = self.connections.dataset_ref(grant_target.project, grant_target.dataset)
             dataset = client.get_dataset(dataset_ref)
             access_entry = AccessEntry(role, entity_type, entity)
-            dataset = add_access_entry_to_dataset(dataset, access_entry)
-            client.update_dataset(dataset, ["access_entries"])
+            # only perform update if access entry not in dataset
+            if is_access_entry_in_dataset(dataset, access_entry):
+                logger.warning(f"Access entry {access_entry} " f"already exists in dataset")
+            else:
+                dataset = add_access_entry_to_dataset(dataset, access_entry)
+                client.update_dataset(dataset, ["access_entries"])
 
     @available.parse_none
     def get_dataset_location(self, relation):
         conn = self.connections.get_thread_connection()
         client = conn.handle
         dataset_ref = self.connections.dataset_ref(relation.project, relation.dataset)
         dataset = client.get_dataset(dataset_ref)
@@ -1016,7 +1021,16 @@
             return f"{c} not enforced" if c else None
 
         return c
 
     def debug_query(self):
         """Override for DebugTask method"""
         self.execute("select 1 as id")
+
+    def validate_sql(self, sql: str) -> AdapterResponse:
+        """Submit the given SQL to the engine for validation, but not execution.
+
+        This submits the query with the `dry_run` flag set True.
+
+        :param str sql: The sql to validate
+        """
+        return self.connections.dry_run(sql)
```

### Comparing `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/python_submissions.py` & `dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/relation.py` & `dbt-bigquery-1.6.0rc1/dbt/adapters/bigquery/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters/apply_grants.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/catalog.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/copy.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/copy.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% macro bq_generate_incremental_insert_overwrite_build_sql(
-    tmp_relation, target_relation, sql, unique_key, partition_by, partitions, dest_columns, on_schema_change, copy_partitions
+    tmp_relation, target_relation, sql, unique_key, partition_by, partitions, dest_columns, tmp_relation_exists, copy_partitions
 ) %}
     {% if partition_by is none %}
       {% set missing_partition_msg -%}
       The 'insert_overwrite' strategy requires the `partition_by` config.
       {%- endset %}
       {% do exceptions.raise_compiler_error(missing_partition_msg) %}
     {% endif %}
 
     {% set build_sql = bq_insert_overwrite_sql(
-        tmp_relation, target_relation, sql, unique_key, partition_by, partitions, dest_columns, on_schema_change, copy_partitions
+        tmp_relation, target_relation, sql, unique_key, partition_by, partitions, dest_columns, tmp_relation_exists, copy_partitions
     ) %}
 
     {{ return(build_sql) }}
 
 {% endmacro %}
 
 {% macro bq_copy_partitions(tmp_relation, target_relation, partitions, partition_by) %}
@@ -35,51 +35,65 @@
 
 {% endmacro %}
 
 {% macro bq_insert_overwrite_sql(
     tmp_relation, target_relation, sql, unique_key, partition_by, partitions, dest_columns, tmp_relation_exists, copy_partitions
 ) %}
   {% if partitions is not none and partitions != [] %} {# static #}
-      {{ bq_static_insert_overwrite_sql(tmp_relation, target_relation, sql, partition_by, partitions, dest_columns, copy_partitions) }}
+      {{ bq_static_insert_overwrite_sql(tmp_relation, target_relation, sql, partition_by, partitions, dest_columns, tmp_relation_exists, copy_partitions) }}
   {% else %} {# dynamic #}
       {{ bq_dynamic_insert_overwrite_sql(tmp_relation, target_relation, sql, unique_key, partition_by, dest_columns, tmp_relation_exists, copy_partitions) }}
   {% endif %}
 {% endmacro %}
 
 {% macro bq_static_insert_overwrite_sql(
-    tmp_relation, target_relation, sql, partition_by, partitions, dest_columns, copy_partitions
+    tmp_relation, target_relation, sql, partition_by, partitions, dest_columns, tmp_relation_exists, copy_partitions
 ) %}
 
       {% set predicate -%}
           {{ partition_by.render_wrapped(alias='DBT_INTERNAL_DEST') }} in (
               {{ partitions | join (', ') }}
           )
       {%- endset %}
 
       {%- set source_sql -%}
         (
-          {%- if partition_by.time_ingestion_partitioning -%}
-          {{ wrap_with_time_ingestion_partitioning_sql(partition_by, sql, True) }}
+          {% if partition_by.time_ingestion_partitioning and tmp_relation_exists -%}
+          select
+            {{ partition_by.insertable_time_partitioning_field() }},
+            * from {{ tmp_relation }}
+          {% elif tmp_relation_exists -%}
+            select
+            * from {{ tmp_relation }}
+          {%- elif partition_by.time_ingestion_partitioning -%}
+            {{ wrap_with_time_ingestion_partitioning_sql(partition_by, sql, True) }}
           {%- else -%}
-          {{sql}}
+            {{sql}}
           {%- endif -%}
+
         )
       {%- endset -%}
 
       {% if copy_partitions %}
           {% do bq_copy_partitions(tmp_relation, target_relation, partitions, partition_by) %}
       {% else %}
 
-      {#-- Because we're putting the model SQL _directly_ into the MERGE statement,
+      {#-- In case we're putting the model SQL _directly_ into the MERGE statement,
          we need to prepend the MERGE statement with the user-configured sql_header,
          which may be needed to resolve that model SQL (e.g. referencing a variable or UDF in the header)
-         in the "dynamic" case, we save the model SQL result as a temp table first, wherein the
+         in the "temporary table exists" case, we save the model SQL result as a temp table first, wherein the
          sql_header is included by the create_table_as macro.
       #}
-      {{ get_insert_overwrite_merge_sql(target_relation, source_sql, dest_columns, [predicate], include_sql_header=true) }}
+      -- 1. run the merge statement
+      {{ get_insert_overwrite_merge_sql(target_relation, source_sql, dest_columns, [predicate], include_sql_header = not tmp_relation_exists) }};
+
+      {%- if tmp_relation_exists -%}
+      -- 2. clean up the temp table
+      drop table if exists {{ tmp_relation }};
+      {%- endif -%}
 
   {% endif %}
 {% endmacro %}
 
 {% macro bq_dynamic_copy_partitions_insert_overwrite_sql(
   tmp_relation, target_relation, sql, unique_key, partition_by, dest_columns, tmp_relation_exists, copy_partitions
   ) %}
```

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/seed.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/table.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/view.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 {% macro bigquery__format_column(column) -%}
   {% set data_type = column.data_type %}
   {% set formatted = column.column.lower() ~ " " ~ data_type %}
   {{ return({'name': column.name, 'data_type': data_type, 'formatted': formatted}) }}
 {%- endmacro -%}
 
 {% macro bigquery__get_empty_schema_sql(columns) %}
+    {%- set col_err = [] -%}
+    {% for col in columns.values() %}
+      {%- if col['data_type'] is not defined -%}
+        {{ col_err.append(col['name']) }}
+      {%- endif -%}
+    {%- endfor -%}
+    {%- if (col_err | length) > 0 -%}
+      {{ exceptions.column_type_missing(column_names=col_err) }}
+    {%- endif -%}
+
     {%- set columns = adapter.nest_column_data_types(columns) -%}
     {{ return(dbt.default__get_empty_schema_sql(columns)) }}
 {% endmacro %}
 
 {% macro bigquery__get_select_subquery(sql) %}
     select {{ adapter.dispatch('get_column_names')() }}
     from (
```

### Comparing `dbt-bigquery-1.6.0b4/dbt/include/bigquery/profile_template.yml` & `dbt-bigquery-1.6.0rc1/dbt/include/bigquery/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/PKG-INFO` & `dbt-bigquery-1.6.0rc1/dbt_bigquery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.6.0b4
+Version: 1.6.0rc1
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b4 Summary: The Bigquery
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0rc1 Summary: The
+Bigquery adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+bigquery Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/SOURCES.txt` & `dbt-bigquery-1.6.0rc1/dbt_bigquery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 dbt/include/bigquery/__init__.py
 dbt/include/bigquery/dbt_project.yml
 dbt/include/bigquery/profile_template.yml
 dbt/include/bigquery/macros/adapters.sql
 dbt/include/bigquery/macros/catalog.sql
 dbt/include/bigquery/macros/etc.sql
 dbt/include/bigquery/macros/adapters/apply_grants.sql
+dbt/include/bigquery/macros/materializations/clone.sql
 dbt/include/bigquery/macros/materializations/copy.sql
 dbt/include/bigquery/macros/materializations/incremental.sql
 dbt/include/bigquery/macros/materializations/seed.sql
 dbt/include/bigquery/macros/materializations/snapshot.sql
 dbt/include/bigquery/macros/materializations/table.sql
 dbt/include/bigquery/macros/materializations/view.sql
 dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
```

### Comparing `dbt-bigquery-1.6.0b4/setup.py` & `dbt-bigquery-1.6.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     else:
         core_patch = "0"
 
     return f"{major}.{minor}.{core_patch}"
 
 
 package_name = "dbt-bigquery"
-package_version = "1.6.0b4"
+package_version = "1.6.0rc1"
 dbt_core_version = _dbt_core_version(_dbt_bigquery_version())
 description = """The BigQuery adapter plugin for dbt"""
 
 setup(
     name="dbt-bigquery",
     version=_dbt_bigquery_version(),
     description="The Bigquery adapter plugin for dbt",
```

