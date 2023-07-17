# Comparing `tmp/dbt-snowflake-1.6.0b3.tar.gz` & `tmp/dbt-snowflake-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-snowflake-1.6.0b3.tar", last modified: Thu Jun  8 23:32:37 2023, max compression
+gzip compressed data, was "dbt-snowflake-1.6.0rc1.tar", last modified: Mon Jul 17 23:12:10 2023, max compression
```

## Comparing `dbt-snowflake-1.6.0b3.tar` & `dbt-snowflake-1.6.0rc1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.756438 dbt-snowflake-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-08 23:32:37.756438 dbt-snowflake-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.744438 dbt-snowflake-1.6.0b3/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.740438 dbt-snowflake-1.6.0b3/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.748438 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    20966 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.748438 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/dynamic_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/target_lag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.744438 dbt-snowflake-1.6.0b3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.748438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.748438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.752438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.752438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/dynamic_table/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/dynamic_table/ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/dynamic_table/materialization.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.752438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.756438 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:32:37.756438 dbt-snowflake-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.752766 dbt-snowflake-1.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-17 23:12:10.752766 dbt-snowflake-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.744766 dbt-snowflake-1.6.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.744766 dbt-snowflake-1.6.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.744766 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20966 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.748766 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/relation_configs/dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/relation_configs/target_lag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.744766 dbt-snowflake-1.6.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.748766 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.748766 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.748766 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/clone.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.748766 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/dynamic_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/dynamic_table/ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/dynamic_table/materialization.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.748766 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/dbt/include/snowflake/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:12:10.752766 dbt-snowflake-1.6.0rc1/dbt_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-17 23:12:10.000000 dbt-snowflake-1.6.0rc1/dbt_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-17 23:12:10.000000 dbt-snowflake-1.6.0rc1/dbt_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:12:10.000000 dbt-snowflake-1.6.0rc1/dbt_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:12:10.000000 dbt-snowflake-1.6.0rc1/dbt_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 23:12:10.000000 dbt-snowflake-1.6.0rc1/dbt_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 23:12:10.000000 dbt-snowflake-1.6.0rc1/dbt_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:12:10.752766 dbt-snowflake-1.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-17 23:11:56.000000 dbt-snowflake-1.6.0rc1/setup.py
```

### Comparing `dbt-snowflake-1.6.0b3/LICENSE.md` & `dbt-snowflake-1.6.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/PKG-INFO` & `dbt-snowflake-1.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.6.0b3
+Version: 1.6.0rc1
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b3 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0rc1 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.6.0b3/README.md` & `dbt-snowflake-1.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/__init__.py` & `dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/column.py` & `dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/column.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/connections.py` & `dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/impl.py` & `dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     automatic_clustering: Optional[bool] = None
     secure: Optional[bool] = None
     copy_grants: Optional[bool] = None
     snowflake_warehouse: Optional[str] = None
     query_tag: Optional[str] = None
     tmp_relation_type: Optional[str] = None
     merge_update_columns: Optional[str] = None
+    target_lag: Optional[str] = None
 
 
 class SnowflakeAdapter(SQLAdapter):
     Relation = SnowflakeRelation
     Column = SnowflakeColumn
     ConnectionManager = SnowflakeConnectionManager
```

### Comparing `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation.py` & `dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/dynamic_table.py` & `dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/relation_configs/dynamic_table.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/target_lag.py` & `dbt-snowflake-1.6.0rc1/dbt/adapters/snowflake/relation_configs/target_lag.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/adapters.sql` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/catalog.sql` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/catalog.sql`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,19 @@
 
               'Last Modified' as "stats:last_modified:label",
               to_varchar(convert_timezone('UTC', last_altered), 'yyyy-mm-dd HH24:MI'||'UTC') as "stats:last_modified:value",
               'The timestamp for last update/change' as "stats:last_modified:description",
               (last_altered is not null and table_type='BASE TABLE') as "stats:last_modified:include"
 
           from {{ information_schema }}.tables
+          where (
+            {%- for schema in schemas -%}
+              upper("table_schema") = upper('{{ schema }}'){%- if not loop.last %} or {% endif -%}
+            {%- endfor -%}
+          )
 
       ),
 
       columns as (
 
           select
               table_catalog as "table_database",
@@ -45,23 +50,23 @@
 
               column_name as "column_name",
               ordinal_position as "column_index",
               data_type as "column_type",
               comment as "column_comment"
 
           from {{ information_schema }}.columns
+          where (
+            {%- for schema in schemas -%}
+              upper("table_schema") = upper('{{ schema }}'){%- if not loop.last %} or {% endif -%}
+            {%- endfor -%}
+          )
       )
 
       select *
       from tables
       join columns using ("table_database", "table_schema", "table_name")
-      where (
-        {%- for schema in schemas -%}
-          upper("table_schema") = upper('{{ schema }}'){%- if not loop.last %} or {% endif -%}
-        {%- endfor -%}
-      )
       order by "column_index"
     {%- endset -%}
 
   {{ return(run_query(query)) }}
 
 {%- endmacro %}
```

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/dynamic_table/ddl.sql` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/dynamic_table/ddl.sql`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,34 @@
 
 {% macro snowflake__get_create_dynamic_table_as_sql(relation, sql) -%}
     {{- log('Applying CREATE to: ' ~ relation) -}}
 
     create or replace dynamic table {{ relation }}
         lag = '{{ config.get("target_lag") }}'
         warehouse = {{ config.get("warehouse") }}
-        as ({{ sql }})
+        as (
+            {{ sql }}
+        )
+    ;
+    {{ snowflake__refresh_dynamic_table(relation) }}
 
 {%- endmacro %}
 
 
 {% macro snowflake__get_replace_dynamic_table_as_sql(relation, sql, existing_relation, backup_relation, intermediate_relation) -%}
     {{- log('Applying REPLACE to: ' ~ relation) -}}
     {{ snowflake__get_drop_dynamic_table_sql(existing_relation) }};
     {{ snowflake__get_create_dynamic_table_as_sql(relation, sql) }}
 {%- endmacro %}
 
 
 {% macro snowflake__refresh_dynamic_table(relation) -%}
     {{- log('Applying REFRESH to: ' ~ relation) -}}
-    {%- do return('') -%}
+
+    alter dynamic table {{ relation }} refresh
 {%- endmacro %}
 
 
 {% macro snowflake__get_dynamic_table_configuration_changes(relation, new_config) -%}
     {{- log('Determining configuration changes on: ' ~ relation) -}}
     {%- do return(None) -%}
 {%- endmacro %}
```

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/dynamic_table/materialization.sql` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/dynamic_table/materialization.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/incremental.sql` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/merge.sql` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/seed.sql` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/table.sql` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/timestamps.sql` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt/include/snowflake/profile_template.yml` & `dbt-snowflake-1.6.0rc1/dbt/include/snowflake/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/PKG-INFO` & `dbt-snowflake-1.6.0rc1/dbt_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.6.0b3
+Version: 1.6.0rc1
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b3 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0rc1 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/SOURCES.txt` & `dbt-snowflake-1.6.0rc1/dbt_snowflake.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 dbt/adapters/snowflake/relation_configs/target_lag.py
 dbt/include/snowflake/__init__.py
 dbt/include/snowflake/dbt_project.yml
 dbt/include/snowflake/profile_template.yml
 dbt/include/snowflake/macros/adapters.sql
 dbt/include/snowflake/macros/apply_grants.sql
 dbt/include/snowflake/macros/catalog.sql
+dbt/include/snowflake/macros/materializations/clone.sql
 dbt/include/snowflake/macros/materializations/incremental.sql
 dbt/include/snowflake/macros/materializations/merge.sql
 dbt/include/snowflake/macros/materializations/seed.sql
 dbt/include/snowflake/macros/materializations/snapshot.sql
 dbt/include/snowflake/macros/materializations/table.sql
 dbt/include/snowflake/macros/materializations/test.sql
 dbt/include/snowflake/macros/materializations/view.sql
```

### Comparing `dbt-snowflake-1.6.0b3/setup.py` & `dbt-snowflake-1.6.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-snowflake"
-package_version = "1.6.0b3"
+package_version = "1.6.0rc1"
 dbt_core_version = _get_dbt_core_version()
 description = """The Snowflake adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

