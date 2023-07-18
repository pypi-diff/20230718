# Comparing `tmp/dbt-redshift-1.6.0b5.tar.gz` & `tmp/dbt-redshift-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-redshift-1.6.0b5.tar", last modified: Fri Jun 23 21:42:01 2023, max compression
+gzip compressed data, was "dbt-redshift-1.6.0rc1.tar", last modified: Tue Jul 18 00:00:35 2023, max compression
```

## Comparing `dbt-redshift-1.6.0b5.tar` & `dbt-redshift-1.6.0rc1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.685997 dbt-redshift-1.6.0b5/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.685997 dbt-redshift-1.6.0b5/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.656087 dbt-redshift-1.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-18 00:00:35.656087 dbt-redshift-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.648087 dbt-redshift-1.6.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.644087 dbt-redshift-1.6.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.648087 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.648087 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.644087 dbt-redshift-1.6.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.652087 dbt-redshift-1.6.0rc1/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.652087 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.652087 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.652087 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/materializations/incremental_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.652087 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.652087 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:00:35.656087 dbt-redshift-1.6.0rc1/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-18 00:00:35.000000 dbt-redshift-1.6.0rc1/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-18 00:00:35.000000 dbt-redshift-1.6.0rc1/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:00:35.000000 dbt-redshift-1.6.0rc1/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:00:35.000000 dbt-redshift-1.6.0rc1/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-18 00:00:35.000000 dbt-redshift-1.6.0rc1/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 00:00:35.000000 dbt-redshift-1.6.0rc1/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 00:00:35.656087 dbt-redshift-1.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-18 00:00:21.000000 dbt-redshift-1.6.0rc1/setup.py
```

### Comparing `dbt-redshift-1.6.0b5/LICENSE.md` & `dbt-redshift-1.6.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/PKG-INFO` & `dbt-redshift-1.6.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b5
+Version: 1.6.0rc1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b5 Summary: The Redshift
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0rc1 Summary: The
+Redshift adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+redshift Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.6.0b5/README.md` & `dbt-redshift-1.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/adapters/redshift/__init__.py` & `dbt-redshift-1.6.0rc1/dbt/adapters/redshift/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dbt.adapters.base import AdapterPlugin
 
 from dbt.adapters.redshift.connections import (  # noqa: F401
     RedshiftConnectionManager,
     RedshiftCredentials,
 )
+
 from dbt.adapters.redshift.relation import RedshiftRelation  # noqa: F401
 from dbt.adapters.redshift.impl import RedshiftAdapter
 from dbt.include import redshift
 
 
 Plugin: AdapterPlugin = AdapterPlugin(
     adapter=RedshiftAdapter,  # type: ignore
```

### Comparing `dbt-redshift-1.6.0b5/dbt/adapters/redshift/connections.py` & `dbt-redshift-1.6.0rc1/dbt/adapters/redshift/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,18 @@
         validator_msg = self.validator_error_message(self.exc)
         msg = f"Could not parse SSL config: {validator_msg}"
         return msg
 
 
 logger = AdapterLogger("Redshift")
 
+
 drop_lock: Lock = dbt.flags.MP_CONTEXT.Lock()  # type: ignore
 
+
 IAMDuration = NewType("IAMDuration", int)
 
 
 class IAMDurationEncoder(FieldEncoder):
     @property
     def json_schema(self):
         return {"type": "integer", "minimum": 0, "maximum": 65535}
@@ -176,15 +178,15 @@
         self.credentials = credentials
 
     def get_connect_method(self):
         method = self.credentials.method
         kwargs = {
             "host": self.credentials.host,
             "database": self.credentials.database,
-            "port": self.credentials.port if self.credentials.port else 5439,
+            "port": int(self.credentials.port) if self.credentials.port else int(5439),
             "auto_create": self.credentials.autocreate,
             "db_groups": self.credentials.db_groups,
             "region": self.credentials.region,
             "timeout": self.credentials.connect_timeout,
         }
 
         redshift_ssl_config = RedshiftSSLConfig.parse(self.credentials.sslmode)
@@ -347,14 +349,15 @@
     def execute(
         self,
         sql: str,
         auto_begin: bool = False,
         fetch: bool = False,
         limit: Optional[int] = None,
     ) -> Tuple[AdapterResponse, agate.Table]:
+        sql = self._add_query_comment(sql)
         _, cursor = self.add_query(sql, auto_begin)
         response = self.get_response(cursor)
         if fetch:
             table = self.get_result_from_cursor(cursor, limit)
         else:
             table = dbt.clients.agate_helper.empty_table()
         return response, table
```

### Comparing `dbt-redshift-1.6.0b5/dbt/adapters/redshift/impl.py` & `dbt-redshift-1.6.0rc1/dbt/adapters/redshift/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from dataclasses import dataclass
 from typing import Optional, Set, Any, Dict, Type
 from collections import namedtuple
-
 from dbt.adapters.base import PythonJobHelper
 from dbt.adapters.base.impl import AdapterConfig, ConstraintSupport
 from dbt.adapters.base.meta import available
 from dbt.adapters.sql import SQLAdapter
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.graph.nodes import ConstraintType
 from dbt.events import AdapterLogger
+
+
 import dbt.exceptions
 
 from dbt.adapters.redshift import RedshiftConnectionManager, RedshiftRelation
 
 
 logger = AdapterLogger("Redshift")
 
@@ -23,19 +24,19 @@
 @dataclass
 class RedshiftConfig(AdapterConfig):
     sort_type: Optional[str] = None
     dist: Optional[str] = None
     sort: Optional[str] = None
     bind: Optional[bool] = None
     backup: Optional[bool] = True
-    autorefresh: Optional[bool] = False
+    auto_refresh: Optional[bool] = False
 
 
 class RedshiftAdapter(SQLAdapter):
-    Relation = RedshiftRelation
+    Relation = RedshiftRelation  # type: ignore
     ConnectionManager = RedshiftConnectionManager
     connections: RedshiftConnectionManager
 
     AdapterSpecificConfigs = RedshiftConfig  # type: ignore
 
     CONSTRAINT_SUPPORT = {
         ConstraintType.check: ConstraintSupport.NOT_SUPPORTED,
@@ -105,15 +106,15 @@
             msg = f"Cross-db references allowed only in {self.type()} RA3.* node. Got {exc.msg}"
             raise dbt.exceptions.CompilationError(msg)
 
     def valid_incremental_strategies(self):
         """The set of standard builtin strategies which this adapter supports out-of-the-box.
         Not used to validate custom strategies defined by end users.
         """
-        return ["append", "delete+insert"]
+        return ["append", "delete+insert", "merge"]
 
     def timestamp_add_sql(self, add_to: str, number: int = 1, interval: str = "hour") -> str:
         return f"{add_to} + interval '{number} {interval}'"
 
     def _link_cached_database_relations(self, schemas: Set[str]):
         """
         :param schemas: The set of schemas that should have links added.
```

### Comparing `dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation.py` & `dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/__init__.py` & `dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/base.py` & `dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/dist.py` & `dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/dist.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/materialized_view.py` & `dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/materialized_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,16 @@
 
     @classmethod
     def parse_model_node(cls, model_node: ModelNode) -> dict:
         config_dict = {
             "mv_name": model_node.identifier,
             "schema_name": model_node.schema,
             "database_name": model_node.database,
-            "backup": model_node.config.get("backup"),
-            "autorefresh": model_node.config.get("auto_refresh"),
+            "backup": model_node.config.extra.get("backup"),
+            "autorefresh": model_node.config.extra.get("auto_refresh"),
         }
 
         if query := model_node.compiled_code:
             config_dict.update({"query": query.strip()})
 
         if model_node.config.get("dist"):
             config_dict.update({"dist": RedshiftDistConfig.parse_model_node(model_node)})
@@ -170,15 +170,15 @@
         )
         query: agate.Row = cls._get_first_row(relation_results.get("query"))
 
         config_dict = {
             "mv_name": materialized_view.get("table"),
             "schema_name": materialized_view.get("schema"),
             "database_name": materialized_view.get("database"),
-            "autorefresh": {"t": True, "f": False}.get(materialized_view.get("autorefresh")),
+            "autorefresh": materialized_view.get("autorefresh"),
             "query": cls._parse_query(query.get("definition")),
         }
 
         # the default for materialized views differs from the default for diststyle in general
         # only set it if we got a value
         if materialized_view.get("diststyle"):
             config_dict.update(
```

### Comparing `dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/sort.py` & `dbt-redshift-1.6.0rc1/dbt/adapters/redshift/relation_configs/sort.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters.sql` & `dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/adapters.sql`

 * *Files 2% similar despite different names*

```diff
@@ -219,51 +219,50 @@
     {% endif %}
     order by ordinal_position
   {% endcall %}
   {% set table = load_result('get_columns_in_relation').table %}
   {{ return(sql_convert_columns_in_relation(table)) }}
 {% endmacro %}
 
-
 {% macro redshift__list_relations_without_caching(schema_relation) %}
+
   {% call statement('list_relations_without_caching', fetch_result=True) -%}
     select
-      '{{ schema_relation.database }}' as database,
-      tablename as name,
-      schemaname as schema,
-      'table' as type
-    from pg_tables
-    where schemaname ilike '{{ schema_relation.schema }}'
+        table_catalog as database,
+        table_name as name,
+        table_schema as schema,
+        'table' as type
+    from information_schema.tables
+    where table_schema ilike '{{ schema_relation.schema }}'
+    and table_type = 'BASE TABLE'
     union all
     select
-      '{{ schema_relation.database }}' as database,
-      viewname as name,
-      schemaname as schema,
+      table_catalog as database,
+      table_name as name,
+      table_schema as schema,
       case
-        when definition ilike '%create materialized view%'
+        when view_definition ilike '%create materialized view%'
           then 'materialized_view'
         else 'view'
       end as type
-    from pg_views
-    where schemaname ilike '{{ schema_relation.schema }}'
+    from information_schema.views
+    where table_schema ilike '{{ schema_relation.schema }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
-
 {% macro redshift__information_schema_name(database) -%}
   {{ return(postgres__information_schema_name(database)) }}
 {%- endmacro %}
 
 
 {% macro redshift__list_schemas(database) -%}
   {{ return(postgres__list_schemas(database)) }}
 {%- endmacro %}
 
-
 {% macro redshift__check_schema_exists(information_schema, schema) -%}
   {{ return(postgres__check_schema_exists(information_schema, schema)) }}
 {%- endmacro %}
 
 
 {% macro redshift__persist_docs(relation, model, for_relation, for_columns) -%}
   {% if for_relation and config.persist_relation_docs() and model.description %}
```

### Comparing `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/catalog.sql` & `dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/materialized_view.sql` & `dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/materializations/materialized_view.sql`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     {%- set materialized_view = relation.from_runtime_config(config) -%}
 
     create materialized view {{ materialized_view.path }}
         backup {% if materialized_view.backup %}yes{% else %}no{% endif %}
         diststyle {{ materialized_view.dist.diststyle }}
         {% if materialized_view.dist.distkey %}distkey ({{ materialized_view.dist.distkey }}){% endif %}
         {% if materialized_view.sort.sortkey %}sortkey ({{ ','.join(materialized_view.sort.sortkey) }}){% endif %}
-        auto refresh {% if materialized_view.auto_refresh %}yes{% else %}no{% endif %}
+        auto refresh {% if materialized_view.autorefresh %}yes{% else %}no{% endif %}
     as (
         {{ materialized_view.query }}
     );
 
 {% endmacro %}
```

### Comparing `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/relations.sql` & `dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/listagg.sql` & `dbt-redshift-1.6.0rc1/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt/include/redshift/profile_template.yml` & `dbt-redshift-1.6.0rc1/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b5/dbt_redshift.egg-info/PKG-INFO` & `dbt-redshift-1.6.0rc1/dbt_redshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b5
+Version: 1.6.0rc1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b5 Summary: The Redshift
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0rc1 Summary: The
+Redshift adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+redshift Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-redshift The `dbt-redshift` package contains all of
```

### Comparing `dbt-redshift-1.6.0b5/dbt_redshift.egg-info/SOURCES.txt` & `dbt-redshift-1.6.0rc1/dbt_redshift.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 dbt/include/redshift/dbt_project.yml
 dbt/include/redshift/profile_template.yml
 dbt/include/redshift/macros/adapters.sql
 dbt/include/redshift/macros/catalog.sql
 dbt/include/redshift/macros/relations.sql
 dbt/include/redshift/macros/timestamps.sql
 dbt/include/redshift/macros/adapters/apply_grants.sql
+dbt/include/redshift/macros/materializations/incremental_merge.sql
 dbt/include/redshift/macros/materializations/materialized_view.sql
 dbt/include/redshift/macros/materializations/snapshot_merge.sql
 dbt/include/redshift/macros/materializations/seeds/helpers.sql
 dbt/include/redshift/macros/utils/array_append.sql
 dbt/include/redshift/macros/utils/array_concat.sql
 dbt/include/redshift/macros/utils/array_construct.sql
 dbt/include/redshift/macros/utils/cast_bool_to_text.sql
```

### Comparing `dbt-redshift-1.6.0b5/setup.py` & `dbt-redshift-1.6.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,16 +80,18 @@
     author_email="info@dbtlabs.com",
     url="https://github.com/dbt-labs/dbt-redshift",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         f"dbt-core~={_core_version()}",
         f"dbt-postgres~={_core_version()}",
-        "boto3~=1.26.26",
-        "redshift-connector~=2.0.911",
+        "boto3~=1.26.157",
+        # dbt-redshift depends deeply on this package. it does not follow SemVer, therefore there have been breaking changes in previous patch releases
+        # Pin to the patch or minor version, and bump in each new minor version of dbt-redshift.
+        "redshift-connector==2.0.913",
         # installed via dbt-core but referenced directly; don't pin to avoid version conflicts with dbt-core
         "agate",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
```

