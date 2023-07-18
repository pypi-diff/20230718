# Comparing `tmp/clickzetta-migration-0.0.0.1.tar.gz` & `tmp/clickzetta-migration-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-migration-0.0.0.1.tar", last modified: Thu Jul 13 14:08:22 2023, max compression
+gzip compressed data, was "clickzetta-migration-0.0.0.2.tar", last modified: Tue Jul 18 07:23:23 2023, max compression
```

## Comparing `clickzetta-migration-0.0.0.1.tar` & `clickzetta-migration-0.0.0.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.105131 clickzetta-migration-0.0.0.1/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       71 2023-07-12 11:59:10.000000 clickzetta-migration-0.0.0.1/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-13 14:08:22.104987 clickzetta-migration-0.0.0.1/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.095511 clickzetta-migration-0.0.0.1/clickzetta_migration.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-13 14:08:22.000000 clickzetta-migration-0.0.0.1/clickzetta_migration.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-13 14:08:22.000000 clickzetta-migration-0.0.0.1/clickzetta_migration.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-13 14:08:22.000000 clickzetta-migration-0.0.0.1/clickzetta_migration.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-13 14:08:22.000000 clickzetta-migration-0.0.0.1/clickzetta_migration.egg-info/entry_points.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-13 14:08:22.000000 clickzetta-migration-0.0.0.1/clickzetta_migration.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       79 2023-07-13 14:08:22.000000 clickzetta-migration-0.0.0.1/clickzetta_migration.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-13 14:08:22.000000 clickzetta-migration-0.0.0.1/clickzetta_migration.egg-info/top_level.txt
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.095991 clickzetta-migration-0.0.0.1/migration/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.1/migration/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.096587 clickzetta-migration-0.0.0.1/migration/base/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.1/migration/base/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.1/migration/base/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.1/migration/base/status.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.096894 clickzetta-migration-0.0.0.1/migration/connector/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.1/migration/connector/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.097050 clickzetta-migration-0.0.0.1/migration/connector/destination/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.1/migration/connector/destination/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.1/migration/connector/destination/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.097324 clickzetta-migration-0.0.0.1/migration/connector/destination/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.1/migration/connector/destination/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.1/migration/connector/destination/clickzetta/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.097745 clickzetta-migration-0.0.0.1/migration/connector/destination/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.1/migration/connector/destination/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.1/migration/connector/destination/doris/destination.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.098408 clickzetta-migration-0.0.0.1/migration/connector/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.1/migration/connector/source/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.1/migration/connector/source/base.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.098784 clickzetta-migration-0.0.0.1/migration/connector/source/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.1/migration/connector/source/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7338 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.1/migration/connector/source/clickzetta/source.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.099306 clickzetta-migration-0.0.0.1/migration/connector/source/doris/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.1/migration/connector/source/doris/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.1/migration/connector/source/doris/source.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.1/migration/connector/source/enum.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.099707 clickzetta-migration-0.0.0.1/migration/connector/source/hive/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.1/migration/connector/source/hive/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.099798 clickzetta-migration-0.0.0.1/migration/connector/source/odps/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.1/migration/connector/source/odps/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11575 2023-07-12 12:06:34.000000 clickzetta-migration-0.0.0.1/migration/migration.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.100451 clickzetta-migration-0.0.0.1/migration/scheduler/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.1/migration/scheduler/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.100889 clickzetta-migration-0.0.0.1/migration/scheduler/data_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.1/migration/scheduler/data_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.1/migration/scheduler/data_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.101229 clickzetta-migration-0.0.0.1/migration/scheduler/data_validation/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.1/migration/scheduler/data_validation/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2845 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.1/migration/scheduler/data_validation/validation.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4408 2023-07-13 11:53:01.000000 clickzetta-migration-0.0.0.1/migration/scheduler/scheduler.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.101628 clickzetta-migration-0.0.0.1/migration/scheduler/schema_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.1/migration/scheduler/schema_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.1/migration/scheduler/schema_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.102964 clickzetta-migration-0.0.0.1/migration/scheduler/task/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.1/migration/scheduler/task/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-13 11:48:05.000000 clickzetta-migration-0.0.0.1/migration/scheduler/task/base_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.1/migration/scheduler/task/data_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.1/migration/scheduler/task/schema_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3356 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.1/migration/scheduler/task/validation_task.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.1/migration/scheduler/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.103351 clickzetta-migration-0.0.0.1/migration/scheduler/unify_transformer/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.1/migration/scheduler/unify_transformer/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.1/migration/scheduler/unify_transformer/transformer.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.103685 clickzetta-migration-0.0.0.1/migration/test/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.1/migration/test/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2348 2023-07-13 12:19:13.000000 clickzetta-migration-0.0.0.1/migration/test/util_test.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-13 14:08:22.104612 clickzetta-migration-0.0.0.1/migration/util/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.1/migration/util/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4898 2023-07-12 11:48:07.000000 clickzetta-migration-0.0.0.1/migration/util/migration_tasks_status.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.1/migration/util/object_storage_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1531 2023-07-12 14:04:44.000000 clickzetta-migration-0.0.0.1/migration/util/script_util.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-11 02:16:24.000000 clickzetta-migration-0.0.0.1/migration/version.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-13 14:08:22.105172 clickzetta-migration-0.0.0.1/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1383 2023-07-11 05:41:26.000000 clickzetta-migration-0.0.0.1/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.534304 clickzetta-migration-0.0.0.2/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       34 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.2/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-18 07:23:23.534177 clickzetta-migration-0.0.0.2/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.526798 clickzetta-migration-0.0.0.2/clickzetta_migration.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      259 2023-07-18 07:23:23.000000 clickzetta-migration-0.0.0.2/clickzetta_migration.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2086 2023-07-18 07:23:23.000000 clickzetta-migration-0.0.0.2/clickzetta_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-18 07:23:23.000000 clickzetta-migration-0.0.0.2/clickzetta_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       58 2023-07-18 07:23:23.000000 clickzetta-migration-0.0.0.2/clickzetta_migration.egg-info/entry_points.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-07-18 07:23:23.000000 clickzetta-migration-0.0.0.2/clickzetta_migration.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      111 2023-07-18 07:23:23.000000 clickzetta-migration-0.0.0.2/clickzetta_migration.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       10 2023-07-18 07:23:23.000000 clickzetta-migration-0.0.0.2/clickzetta_migration.egg-info/top_level.txt
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.527222 clickzetta-migration-0.0.0.2/migration/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:52:59.000000 clickzetta-migration-0.0.0.2/migration/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.527753 clickzetta-migration-0.0.0.2/migration/base/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       90 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.2/migration/base/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      532 2023-07-13 08:55:34.000000 clickzetta-migration-0.0.0.2/migration/base/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-07-07 03:37:28.000000 clickzetta-migration-0.0.0.2/migration/base/status.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.527978 clickzetta-migration-0.0.0.2/migration/connector/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:53:59.000000 clickzetta-migration-0.0.0.2/migration/connector/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.528138 clickzetta-migration-0.0.0.2/migration/connector/destination/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 12:17:46.000000 clickzetta-migration-0.0.0.2/migration/connector/destination/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1249 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.2/migration/connector/destination/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.528403 clickzetta-migration-0.0.0.2/migration/connector/destination/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-29 06:42:41.000000 clickzetta-migration-0.0.0.2/migration/connector/destination/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6137 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.2/migration/connector/destination/clickzetta/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.528688 clickzetta-migration-0.0.0.2/migration/connector/destination/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-11 15:28:35.000000 clickzetta-migration-0.0.0.2/migration/connector/destination/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6243 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.2/migration/connector/destination/doris/destination.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.529341 clickzetta-migration-0.0.0.2/migration/connector/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       72 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.2/migration/connector/source/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1879 2023-07-12 03:16:08.000000 clickzetta-migration-0.0.0.2/migration/connector/source/base.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.529622 clickzetta-migration-0.0.0.2/migration/connector/source/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-12 02:11:46.000000 clickzetta-migration-0.0.0.2/migration/connector/source/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7338 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.2/migration/connector/source/clickzetta/source.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.529902 clickzetta-migration-0.0.0.2/migration/connector/source/doris/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:41.000000 clickzetta-migration-0.0.0.2/migration/connector/source/doris/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6298 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.2/migration/connector/source/doris/source.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      352 2023-07-11 07:29:24.000000 clickzetta-migration-0.0.0.2/migration/connector/source/enum.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.530096 clickzetta-migration-0.0.0.2/migration/connector/source/hive/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:22.000000 clickzetta-migration-0.0.0.2/migration/connector/source/hive/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.530169 clickzetta-migration-0.0.0.2/migration/connector/source/odps/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:15:30.000000 clickzetta-migration-0.0.0.2/migration/connector/source/odps/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11861 2023-07-17 08:44:25.000000 clickzetta-migration-0.0.0.2/migration/migration.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.530691 clickzetta-migration-0.0.0.2/migration/scheduler/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-07-11 04:22:08.000000 clickzetta-migration-0.0.0.2/migration/scheduler/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.530970 clickzetta-migration-0.0.0.2/migration/scheduler/data_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:25.000000 clickzetta-migration-0.0.0.2/migration/scheduler/data_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3630 2023-07-12 11:45:19.000000 clickzetta-migration-0.0.0.2/migration/scheduler/data_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.531256 clickzetta-migration-0.0.0.2/migration/scheduler/data_validation/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:22:21.000000 clickzetta-migration-0.0.0.2/migration/scheduler/data_validation/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2845 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.2/migration/scheduler/data_validation/validation.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-07-17 07:57:48.000000 clickzetta-migration-0.0.0.2/migration/scheduler/scheduler.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.531526 clickzetta-migration-0.0.0.2/migration/scheduler/schema_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 03:21:14.000000 clickzetta-migration-0.0.0.2/migration/scheduler/schema_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4197 2023-07-12 09:39:55.000000 clickzetta-migration-0.0.0.2/migration/scheduler/schema_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.532583 clickzetta-migration-0.0.0.2/migration/scheduler/task/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      249 2023-07-11 03:06:38.000000 clickzetta-migration-0.0.0.2/migration/scheduler/task/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1395 2023-07-17 07:55:15.000000 clickzetta-migration-0.0.0.2/migration/scheduler/task/base_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1717 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.2/migration/scheduler/task/data_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1339 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.2/migration/scheduler/task/schema_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3356 2023-07-13 09:44:01.000000 clickzetta-migration-0.0.0.2/migration/scheduler/task/validation_task.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2685 2023-07-13 10:20:49.000000 clickzetta-migration-0.0.0.2/migration/scheduler/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.532854 clickzetta-migration-0.0.0.2/migration/scheduler/unify_transformer/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-07-10 03:55:07.000000 clickzetta-migration-0.0.0.2/migration/scheduler/unify_transformer/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3881 2023-07-11 13:22:48.000000 clickzetta-migration-0.0.0.2/migration/scheduler/unify_transformer/transformer.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.533129 clickzetta-migration-0.0.0.2/migration/test/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-28 07:15:40.000000 clickzetta-migration-0.0.0.2/migration/test/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2348 2023-07-13 12:19:13.000000 clickzetta-migration-0.0.0.2/migration/test/util_test.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-07-18 07:23:23.533880 clickzetta-migration-0.0.0.2/migration/util/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-20 02:54:06.000000 clickzetta-migration-0.0.0.2/migration/util/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7638 2023-07-17 09:06:42.000000 clickzetta-migration-0.0.0.2/migration/util/migration_tasks_status.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1180 2023-07-12 10:01:25.000000 clickzetta-migration-0.0.0.2/migration/util/object_storage_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1531 2023-07-12 14:04:44.000000 clickzetta-migration-0.0.0.2/migration/util/script_util.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       23 2023-07-18 07:18:22.000000 clickzetta-migration-0.0.0.2/migration/version.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-07-18 07:23:23.534348 clickzetta-migration-0.0.0.2/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1453 2023-07-18 07:23:21.000000 clickzetta-migration-0.0.0.2/setup.py
```

### Comparing `clickzetta-migration-0.0.0.1/clickzetta_migration.egg-info/SOURCES.txt` & `clickzetta-migration-0.0.0.2/clickzetta_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/base/exceptions.py` & `clickzetta-migration-0.0.0.2/migration/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/connector/destination/base.py` & `clickzetta-migration-0.0.0.2/migration/connector/destination/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/connector/destination/clickzetta/destination.py` & `clickzetta-migration-0.0.0.2/migration/connector/destination/clickzetta/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/connector/destination/doris/destination.py` & `clickzetta-migration-0.0.0.2/migration/connector/destination/doris/destination.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/connector/source/base.py` & `clickzetta-migration-0.0.0.2/migration/connector/source/base.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/connector/source/clickzetta/source.py` & `clickzetta-migration-0.0.0.2/migration/connector/source/clickzetta/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/connector/source/doris/source.py` & `clickzetta-migration-0.0.0.2/migration/connector/source/doris/source.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/migration.py` & `clickzetta-migration-0.0.0.2/migration/migration.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,15 @@
     cz-migration meta -p <profile_path>  --out_path <meta_out_file_path>[generate meta from source]
     cz-migration schema -p <profile_path> [--table_list_file <external_table_list_file>][migrate schema from source to destination]
     cz-migration data -p <profile_path> --meta_conf <meta_conf> --storage_conf <storage_conf> [--table_list_file <external_table_list_file>][migrate data from source to destination]
     cz-migration validate -p <profile_path> [--table_list_file <external_table_list_file>][validate data from source and destination]
     cz-migration run -p <profile_path> --meta_conf <meta_conf> --storage_conf <storage_conf> [--table_list_file <external_table_list_file>][migrate schema and data from source to destination, including validation]
     cz-migration status -p <profile_path> [check migration status]
     cz-migration resume -p <profile_path> [resume migration]
-    cz-migration report -p <profile_path>  [generate migration report]
-options:
-    cz-migration -h | --help
+    cz-migration report -p <profile_path> [generate migration report]
 """
 import logging
 import os.path
 
 import docopt
 import yaml
 
@@ -84,24 +82,26 @@
         project_name: str, concurrency: int, quit_if_fail: bool):
     logger.info(f"Running migration from source {source} to destination {destination}")
     print(f"Running migration from source {source} to destination {destination}")
     UnifyTransformer(source, destination, project_name, db_list, config_table_list, external_table_list, concurrency,
                      quit_if_fail).transform()
 
 
-def status(destination: Destination):
-    pass
+def status(destination: Destination, project_name: str):
+    import migration.util.migration_tasks_status as mts
+    mts.get_last_migration_status(destination, project_name)
 
 
 def resume(source: Source, destination: Destination):
     pass
 
 
-def report(destination: Destination):
-    pass
+def report(destination: Destination, project_name: str):
+    import migration.util.migration_tasks_status as mts
+    mts.get_last_migration_report(destination, project_name)
 
 
 def main():
     logging.basicConfig(level=logging.INFO)
     args = docopt.docopt(__doc__)
     profile = None
     source = None
@@ -219,16 +219,18 @@
     elif args['validate']:
         validate(source, destination, db_list, config_table_list, external_table_list, project_name, concurrency,
                  quit_if_fail)
     elif args['run']:
         run(source, destination, db_list, config_table_list, external_table_list, project_name, concurrency,
             quit_if_fail)
     elif args['status']:
-        status(destination)
+        status(destination, project_name)
     elif args['resume']:
         resume(source, destination)
     elif args['report']:
-        report(destination)
+        report(destination, project_name)
+    else:
+        print("Unknown command")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/data_transformer/transformer.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/data_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/data_validation/validation.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/data_validation/validation.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/scheduler.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/scheduler.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,35 +82,38 @@
 
     def process_done_task_feature(self, feature):
         try:
             result = feature.result()
             if result.is_success():
                 self.succeed_tasks.append(result)
             elif result.is_failed():
-                logger.info(
-                    f"Task:{result.__str__} is failed, begin to retry the {result.retry_times + 1} time, "
-                    f"max_retry is {self.config.task_retry}")
                 if result.retry_times < self.config.task_retry:
+                    logger.info(
+                        f"Task:{result.__str__} is failed, begin to retry the {result.retry_times + 1} time, "
+                        f"max_retry is {self.config.task_retry}")
                     result.retry_times += 1
                     self.future_results.put(self.executor.submit(result.run))
                 else:
+                    logger.error(f"Task:{result.__str__} is failed, max_retry is {self.config.task_retry}")
                     self.failed_tasks.append(result)
         except TaskRuntimeError as e:
             raise e
 
     def check_running_task_status(self):
         for task in self.running_tasks:
             if task.done():
                 self.process_done_task_feature(task)
                 self.running_tasks.remove(task)
                 print(f"remove running task {task} from running_tasks")
 
     def finish(self):
         while True:
-            print(len(self.succeed_tasks), len(self.failed_tasks), len(self.running_tasks), self.tasks_num)
+            logger.info(
+                f"succeed_task_count:{self.succeed_tasks.__len__()}, "
+                f"failed_task_count:{self.failed_tasks.__len__()}, total_task_count:{self.tasks_num}")
             if self.succeed_tasks.__len__() + self.failed_tasks.__len__() == self.tasks_num:
                 self.finish_called = True
                 self.shutdown()
                 break
             else:
                 logger.info(
                     f"Waiting for {len(self.running_tasks)} tasks to finish")
```

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/schema_transformer/transformer.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/schema_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/task/base_task.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/task/base_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self.project_id = project_id
         self.id = self._gen_task_id()
         self.args = args
         self.kwargs = kwargs
         self.status = TaskStatus.INIT
         self.start_time = datetime.now()
         self.end_time = ""
-        self.retry_times = 0
+        self.retry_times = 1
         self.status_id = None
 
     def init_task(self, *args, **kwargs):
         pass
 
     def _gen_task_id(self):
         return f"{self.name}_{self.task_type.value}_{datetime.now().strftime('%Y%m%d%H%M%S%f')}"
```

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/task/data_task.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/task/data_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/task/schema_task.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/task/schema_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/task/validation_task.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/task/validation_task.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/transformer.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/scheduler/unify_transformer/transformer.py` & `clickzetta-migration-0.0.0.2/migration/scheduler/unify_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/test/util_test.py` & `clickzetta-migration-0.0.0.2/migration/test/util_test.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/util/object_storage_util.py` & `clickzetta-migration-0.0.0.2/migration/util/object_storage_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/migration/util/script_util.py` & `clickzetta-migration-0.0.0.2/migration/util/script_util.py`

 * *Files identical despite different names*

### Comparing `clickzetta-migration-0.0.0.1/setup.py` & `clickzetta-migration-0.0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 3 - Alpha"
 dependencies = [
     'scheduler >= 0.8.4',
     'clickzetta-connector >= 0.8.29',
     'docopt >= 0.6.2',
     'pyyaml >= 6.0',
+    'openpyxl >= 3.1.2',
+    'tabulate >= 0.8.9',
 ]
 extras = {
 
 }
 
 all_extras = []
 
@@ -36,15 +38,15 @@
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 version = {}
 with open(os.path.join(package_root, "migration/version.py")) as fp:
     exec(fp.read(), version)
 version = version["__version__"]
 
-packages = setuptools.find_packages(exclude=["tests", "tests.*"])
+packages = setuptools.find_packages(exclude=["test", "test.*", "script", "script.*"])
 
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     url='https://www.yunqi.tech/',
     author="mocun",
```

