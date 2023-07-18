# Comparing `tmp/motordantic-0.0.2a1.tar.gz` & `tmp/motordantic-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motordantic-0.0.2a1.tar", last modified: Wed May 31 16:19:04 2023, max compression
+gzip compressed data, was "motordantic-0.1.0a1.tar", last modified: Tue Jul 18 20:15:38 2023, max compression
```

## Comparing `motordantic-0.0.2a1.tar` & `motordantic-0.1.0a1.tar`

### file list

```diff
@@ -1,47 +1,61 @@
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1075 2022-09-01 11:47:34.000000 motordantic-0.0.2a1/LICENCE
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5763 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5463 2022-09-18 15:33:09.000000 motordantic-0.0.2a1/README.md
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.452948 motordantic-0.0.2a1/motordantic/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        0 2022-08-23 10:08:05.000000 motordantic-0.0.2a1/motordantic/__init__.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     6518 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/aggregate.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3082 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/aggregate_expressions.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4382 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/connection.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2133 2022-11-09 14:00:58.000000 motordantic-0.0.2a1/motordantic/exceptions.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     9219 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/extra.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5714 2022-11-01 07:31:58.000000 motordantic-0.0.2a1/motordantic/fields.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    18659 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/models.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      616 2022-11-01 07:31:58.000000 motordantic-0.0.2a1/motordantic/property.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     8609 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/query.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    49044 2023-05-31 16:17:59.000000 motordantic-0.0.2a1/motordantic/querybuilder.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4562 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/relation.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     6500 2022-11-01 07:31:58.000000 motordantic-0.0.2a1/motordantic/schema.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1565 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/session.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      272 2022-08-31 08:42:52.000000 motordantic-0.0.2a1/motordantic/singleton.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      556 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/sync.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3496 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/types.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      725 2022-11-01 07:31:58.000000 motordantic-0.0.2a1/motordantic/typing.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1978 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/validaton.py
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/motordantic.egg-info/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5763 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1032 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/SOURCES.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/dependency_links.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       43 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/requires.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/top_level.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/setup.cfg
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      646 2023-05-31 16:18:18.000000 motordantic-0.0.2a1/setup.py
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/tests/
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/tests/queries/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        0 2023-03-31 20:51:37.000000 motordantic-0.0.2a1/tests/queries/__init__.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    10287 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/queries/test_aggregation.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7072 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/queries/test_basic_queries.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1607 2023-03-31 20:44:32.000000 motordantic-0.0.2a1/tests/queries/test_indexes.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2597 2022-11-10 14:58:18.000000 motordantic-0.0.2a1/tests/queries/test_inner_qyeries.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1469 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/queries/test_query.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1638 2023-03-31 20:24:13.000000 motordantic-0.0.2a1/tests/queries/test_raw_queries.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1384 2022-11-10 14:58:18.000000 motordantic-0.0.2a1/tests/test_connection.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2746 2023-04-12 19:32:32.000000 motordantic-0.0.2a1/tests/test_create_model.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3501 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/test_extraquerymapper.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      196 2022-09-02 10:52:13.000000 motordantic-0.0.2a1/tests/test_force_sync.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3911 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/test_relation.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2050 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/test_sync.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-07-18 20:15:38.016106 motordantic-0.1.0a1/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1075 2022-09-01 11:47:34.000000 motordantic-0.1.0a1/LICENCE
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5748 2023-07-18 20:15:38.016106 motordantic-0.1.0a1/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5448 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/README.md
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-07-18 20:15:38.012106 motordantic-0.1.0a1/motordantic/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        0 2022-08-23 10:08:05.000000 motordantic-0.1.0a1/motordantic/__init__.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-07-18 20:15:38.012106 motordantic-0.1.0a1/motordantic/aggregate/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       51 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/aggregate/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     6649 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/aggregate/aggregate.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3315 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/aggregate/expressions.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4070 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/connection.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    17343 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/document.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2745 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/exceptions.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5767 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/fields.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5299 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/manager.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      100 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/models.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      616 2022-11-01 07:31:58.000000 motordantic-0.1.0a1/motordantic/property.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-07-18 20:15:38.012106 motordantic-0.1.0a1/motordantic/query/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      273 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/query/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    28891 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/query/builder.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     9165 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/query/extra.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     8232 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/query/query.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3497 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/query/result.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4399 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/relation.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     6567 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/schema.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1520 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/session.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      272 2023-06-09 09:49:09.000000 motordantic-0.1.0a1/motordantic/singleton.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-07-18 20:15:38.012106 motordantic-0.1.0a1/motordantic/sync/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       65 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/sync/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      564 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/sync/query.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      779 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/sync/sync.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4080 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/types.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      765 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/typing.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2758 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/motordantic/validation.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-07-18 20:15:38.012106 motordantic-0.1.0a1/motordantic.egg-info/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5748 2023-07-18 20:15:37.000000 motordantic-0.1.0a1/motordantic.egg-info/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1377 2023-07-18 20:15:37.000000 motordantic-0.1.0a1/motordantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2023-07-18 20:15:37.000000 motordantic-0.1.0a1/motordantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       43 2023-07-18 20:15:37.000000 motordantic-0.1.0a1/motordantic.egg-info/requires.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2023-07-18 20:15:37.000000 motordantic-0.1.0a1/motordantic.egg-info/top_level.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2023-07-18 20:15:38.016106 motordantic-0.1.0a1/setup.cfg
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      646 2023-07-18 20:15:20.000000 motordantic-0.1.0a1/setup.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-07-18 20:15:38.012106 motordantic-0.1.0a1/tests/
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-07-18 20:15:38.016106 motordantic-0.1.0a1/tests/queries/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        0 2023-03-31 20:51:37.000000 motordantic-0.1.0a1/tests/queries/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1418 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/queries/test_Q.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    10316 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/queries/test_aggregation.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7116 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/queries/test_basic_queries.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1603 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/queries/test_indexes.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2595 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/queries/test_inner_queries.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1568 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/queries/test_raw_queries.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1137 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/queries/test_uuid_field.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1603 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/queries/test_validation.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      770 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/queries/test_write_concern.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1196 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/test_connection.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2820 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/test_create_document.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3505 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/test_extraquerymapper.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2444 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/test_fields.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      196 2023-06-24 16:51:23.000000 motordantic-0.1.0a1/tests/test_force_sync.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3858 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/test_relation.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2046 2023-07-18 20:12:43.000000 motordantic-0.1.0a1/tests/test_sync.py
```

### Comparing `motordantic-0.0.2a1/LICENCE` & `motordantic-0.1.0a1/LICENCE`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a1/PKG-INFO` & `motordantic-0.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motordantic
-Version: 0.0.2a1
+Version: 0.1.0a1
 Summary: Mongo ODM, based on motor+pydantic
 Home-page: https://github.com/bogdanjz/motordantic
 Author: bogdanjz
 Author-email: bzdv.dn@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -153,24 +153,24 @@
 class Stats(MongoModel):
     id: int
     cost: float
     clicks: int
     shows: int
     date: str
 
-from motordantic.aggregation import Sum, Min, Max
+from motordantic.aggregate import Sum, Min, Max
 
 summ_cost = await Stats.Q.simple_aggregate(date='2020-01-20', aggregation=Sum('cost'))
 min_clicks = await Stats.Q.simple_aggregate(date='2020-01-20', aggregation=Min('clicks'))
 min_shows = await Stats.Q.simple_aggregate(date='2020-01-20', aggregation=Max('shows'))
 
 # logical
-from motordantic.query import Query
-data = Banner.Q.find_one(Query(name='test') | Query(name__regex='testerino'))
+from motordantic.query import Q
+data = Banner.Q.find_one(Q(name='test') | Q(name__regex='testerino'))
 ```
 
 ### sync queries
 
 ```python
-sync_result = Banner.Q.sync.find_one()
+sync_result = Banner.Qsync.find_one()
 
 ```
```

### Comparing `motordantic-0.0.2a1/README.md` & `motordantic-0.1.0a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -141,24 +141,24 @@
 class Stats(MongoModel):
     id: int
     cost: float
     clicks: int
     shows: int
     date: str
 
-from motordantic.aggregation import Sum, Min, Max
+from motordantic.aggregate import Sum, Min, Max
 
 summ_cost = await Stats.Q.simple_aggregate(date='2020-01-20', aggregation=Sum('cost'))
 min_clicks = await Stats.Q.simple_aggregate(date='2020-01-20', aggregation=Min('clicks'))
 min_shows = await Stats.Q.simple_aggregate(date='2020-01-20', aggregation=Max('shows'))
 
 # logical
-from motordantic.query import Query
-data = Banner.Q.find_one(Query(name='test') | Query(name__regex='testerino'))
+from motordantic.query import Q
+data = Banner.Q.find_one(Q(name='test') | Q(name__regex='testerino'))
 ```
 
 ### sync queries
 
 ```python
-sync_result = Banner.Q.sync.find_one()
+sync_result = Banner.Qsync.find_one()
 
 ```
```

### Comparing `motordantic-0.0.2a1/motordantic/aggregate.py` & `motordantic-0.1.0a1/motordantic/aggregate/aggregate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from typing import TYPE_CHECKING, Any, Optional, Dict, List, Union
 
-from .exceptions import MotordanticValidationError
-from .query import generate_basic_query, Query, QueryCombination
+from ..exceptions import MotordanticValidationError
+from ..query import generate_basic_query, Q, QCombination, AggregateResult
 
 __all__ = ('Aggregate',)
 
 if TYPE_CHECKING:
-    from .typing import MongoModel
+    from .document import Document
 
 
 class Aggregate(object):
-    def __init__(self, mongo_model_class: 'MongoModel'):
-        self.mongo_model_class = mongo_model_class
+    def __init__(self, document_class: 'Document'):
+        self.document_class = document_class
         self.pipeline: List[Dict] = []
 
     def match(
-        self, logical_query: Optional[Union[Query, QueryCombination]] = None, **query
+        self, logical_query: Optional[Union[Q, QCombination]] = None, **query
     ) -> 'Aggregate':
         if logical_query is not None:
-            query_params = self.mongo_model_class._check_query_args(logical_query)  # type: ignore
+            query_params = self.document_class.Q._check_query_args(logical_query)  # type: ignore
         else:
-            query_params = generate_basic_query(self.mongo_model_class, query, False)
+            query_params = generate_basic_query(
+                self.document_class.manager, query, False
+            )
         self.pipeline.append({'$match': {**query_params}})
         return self
 
     def raw_match(self, native_match_query: dict) -> 'Aggregate':
         self.pipeline.append({'$match': native_match_query})
         return self
 
@@ -50,32 +52,29 @@
 
     def sort(self, **sort_kwargs) -> 'Aggregate':
         self.pipeline.append({'$sort': {**sort_kwargs}})
         return self
 
     def lookup(
         self,
-        from_: 'MongoModel',
+        from_: 'Document',
         local_field: str,
         foreign_field: str,
         as_: Optional[str] = None,
     ) -> 'Aggregate':
-        if (
-            local_field not in self.mongo_model_class.__fields__
-            and local_field != '_id'
-        ):
+        if local_field not in self.document_class.__fields__ and local_field != '_id':
             raise MotordanticValidationError(
                 f'field - {local_field} not a field from model: {from_.__name__}'
             )
         if foreign_field not in from_.__fields__ and foreign_field != '_id':
             raise MotordanticValidationError(
-                f'field - {foreign_field} not a field from model: {self.mongo_model_class.__name__}'
+                f'field - {foreign_field} not a field from model: {self.document_class.__name__}'
             )
         lookup = {
-            'from': from_.set_collection_name(),
+            'from': from_.get_collection_name(),
             'localField': local_field,
             'foreignField': foreign_field,
         }
         if as_:
             lookup['as'] = as_
         else:
             lookup['as'] = (
@@ -171,14 +170,14 @@
         self.pipeline.append({'$geoNear': geo_near})
         return self
 
     def let(self, let: dict) -> 'Aggregate':
         self.pipeline.append({'$let': {**let}})
         return self
 
-    async def result(self) -> list:
-        result = await self.mongo_model_class.Q.raw_aggregate(self.pipeline)
-        return result
-
-    def result_sync(self) -> list:
-        result = self.mongo_model_class.Q.sync.raw_aggregate(self.pipeline)
-        return result
+    async def result(self) -> AggregateResult:
+        result = await self.document_class.Q.raw_aggregate(self.pipeline)
+        return AggregateResult(native_result=result, document_class=self.document_class)
+
+    def result_sync(self) -> AggregateResult:
+        result = self.document_class.Qsync.raw_aggregate(self.pipeline)
+        return AggregateResult(native_result=result, document_class=self.document_class)
```

### Comparing `motordantic-0.0.2a1/motordantic/aggregate_expressions.py` & `motordantic-0.1.0a1/motordantic/aggregate/expressions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import TYPE_CHECKING, Dict, Any
 from dataclasses import dataclass
 
-from .exceptions import MotordanticValidationError
+from ..exceptions import MotordanticValidationError
 
 __all__ = ('Sum', 'Avg', 'Min', 'Count', 'Max')
 
 if TYPE_CHECKING:
-    from .models import MongoModel
+    from ..document import Document
 
 
 class BaseAggregationOperation(object):
     """Abstract class for Aggregation"""
 
     __slots__ = ('field', '_operation')
 
@@ -21,24 +21,27 @@
 
     @property
     def operation(self) -> str:
         if not self._operation:
             raise NotImplementedError('implement _operation')
         return self._operation
 
-    def _validate_field(self, mongo_model_class: 'MongoModel'):
-        if self.field not in mongo_model_class.__fields__ and self.field != '_id':
+    def _validate_field(self, document_class: 'Document'):
+        # if self.field in document_class.__motordantic_extra_fields__.values():
+        #     return None
+        if self.field not in document_class.__fields__ and self.field != '_id':
             raise MotordanticValidationError(
-                f'invalid field "{self.field}" for this model, field must be one of {list(mongo_model_class.__fields__.keys())}'
+                f'invalid field "{self.field}" for this model, field must be one of {list(document_class.__fields__.keys())}'
             )
 
-    def _aggregate_query(self, mongo_model_class: 'MongoModel') -> dict:
-        self._validate_field(mongo_model_class)
+    def _aggregate_query(self, document_class: 'Document') -> dict:
+        self._validate_field(document_class)
+        query_field = document_class.__mapping_query_fields__[self.field]
         query = {
-            f'{self.field}__{self.operation}': {f'${self.operation}': f'${self.field}'}
+            f'{query_field}__{self.operation}': {f'${self.operation}': f'${self.field}'}
         }
         return query
 
 
 class Sum(BaseAggregationOperation):
     """
     Simple sum aggregation
@@ -94,27 +97,28 @@
     generated query:
         - if field = _id
             {
                 '_id': None
                 'count': {'$sum': 1},
             }
         - else
-            {
+            {S
                 '_id': 'field'
                 'count': {'$sum': 1},
             }
     return: {'_id': <value>, 'count': value}
     """
 
     _operation: str = 'count'
 
-    def _aggregate_query(self, mongo_model_class: 'MongoModel') -> dict:
-        self._validate_field(mongo_model_class)
+    def _aggregate_query(self, document_class: 'Document') -> dict:
+        self._validate_field(document_class)
+        query_field = document_class.__mapping_query_fields__[self.field]
         query = {
-            "_id": f'${self.field}' if self.field != '_id' else None,
+            "_id": f'${query_field}' if self.field != '_id' else None,
             f'count': {'$sum': 1},
         }
         return query
 
 
 @dataclass
 class Bucket(object):
```

### Comparing `motordantic-0.0.2a1/motordantic/connection.py` & `motordantic-0.1.0a1/motordantic/connection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,67 @@
 import os
 from typing import Optional
 
 from motor.motor_asyncio import AsyncIOMotorClient
+from bson.raw_bson import RawBSONDocument
 
 from .singleton import Singleton
-from .models import MongoModel
-
-DEFAULT_ENV_NAME: str = 'default'
-
-
-_connections: dict = {}
+from .manager import ODMManager
 
 
 class MotordanticConnection(object, metaclass=Singleton):
     __slots__ = (
         'address',
         'database_name',
         'max_pool_size',
         'server_selection_timeout_ms',
         'connect_timeout_ms',
         'socket_timeout_ms',
         'ssl_cert_path',
-        'env_name',
     )
 
     _connections: dict = {}
 
     def __init__(
         self,
         address: str,
         database_name: str,
         max_pool_size: int = 250,
         ssl_cert_path: Optional[str] = None,
         server_selection_timeout_ms: int = 60000,
         connect_timeout_ms: int = 30000,
         socket_timeout_ms: int = 60000,
-        env_name: str = DEFAULT_ENV_NAME,
     ):
         self.address = address
         self.database_name = database_name
         self.max_pool_size = max_pool_size
         self.ssl_cert_path = ssl_cert_path
         self.server_selection_timeout_ms = server_selection_timeout_ms
         self.connect_timeout_ms = connect_timeout_ms
         self.socket_timeout_ms = socket_timeout_ms
-        if env_name not in _connections:
-            _connections[env_name] = self
 
-    def _init_mongo_connection(self, connect: bool = False) -> AsyncIOMotorClient:
+    def _init_mongo_connection(self, connect: bool = False) -> AsyncIOMotorClient:  # type: ignore
         connection_params: dict = {
             'host': self.address,
             'connect': connect,
             'serverSelectionTimeoutMS': self.server_selection_timeout_ms,
             'maxPoolSize': self.max_pool_size,
             'connectTimeoutMS': self.connect_timeout_ms,
             'socketTimeoutMS': self.socket_timeout_ms,
         }
         if self.ssl_cert_path:
             connection_params['tlsCAFile'] = self.ssl_cert_path
             connection_params['tlsAllowInvalidCertificates'] = bool(self.ssl_cert_path)
-        client = AsyncIOMotorClient(**connection_params)
+        client = AsyncIOMotorClient(
+            **connection_params,
+            document_class=RawBSONDocument,
+        )
         return client
 
-    def _get_motor_client(self) -> AsyncIOMotorClient:
+    def _get_motor_client(self) -> AsyncIOMotorClient:  # type: ignore
         pid = os.getpid()
         if pid in self._connections:
             return self._connections[pid]
         else:
             mongo_connection = self._init_mongo_connection()
             self._connections[os.getpid()] = mongo_connection
             return mongo_connection
@@ -76,47 +71,43 @@
     address: str,
     database_name: str,
     max_pool_size: int = 100,
     ssl_cert_path: Optional[str] = None,
     server_selection_timeout_ms: int = 60000,
     connect_timeout_ms: int = 30000,
     socket_timeout_ms: int = 60000,
-    env_name: Optional[str] = DEFAULT_ENV_NAME,
 ) -> MotordanticConnection:
     """init connection to mongodb
 
     Args:
         address (str): full connection string
         database_name (str): mongo db name
         max_pool_size (int, optional): max connection pool. Defaults to 100.
         ssl_cert_path (Optional[str], optional): path to ssl cert. Defaults to None.
         server_selection_timeout_ms (int, optional): ServerSelectionTimeoutMS. Defaults to 60000.
         connect_timeout_ms (int, optional): ConnectionTimeoutMS. Defaults to 30000.
         socket_timeout_ms (int, optional): SocketTimeoutMS. Defaults to 60000.
-        env_name (Optional[str], optional): connection env name. Defaults to None.
 
     Returns:
         MotordanticConnection: motordantic connection
     """
     os.environ['MOTORDANTIC_DATABASE'] = database_name
     os.environ['MOTORDANTIC_ADDRESS'] = address
-    os.environ['MOTORDANTIC_ENV_NAME'] = env_name or DEFAULT_ENV_NAME
     os.environ['MOTORDANTIC_MAX_POOL_SIZE'] = str(max_pool_size)
     os.environ['MOTORDANTIC_SERVER_SELECTION_TIMOUT_MS'] = str(
         server_selection_timeout_ms
     )
     os.environ['MOTORDANTIC_CONNECT_TIMEOUT_MS'] = str(connect_timeout_ms)
     os.environ['MOTORDANTIC_SOCKET_TIMEOUT_MS'] = str(socket_timeout_ms)
     if ssl_cert_path:
         os.environ['MOTORDANTIC_SSL_CERT_PATH'] = ssl_cert_path
     connection = MotordanticConnection(
         address=address,
         database_name=database_name,
-        env_name=env_name or DEFAULT_ENV_NAME,
         max_pool_size=max_pool_size,
         server_selection_timeout_ms=server_selection_timeout_ms,
         connect_timeout_ms=connect_timeout_ms,
         socket_timeout_ms=socket_timeout_ms,
         ssl_cert_path=ssl_cert_path,
     )
-    MongoModel.use(connection)
+    ODMManager.use(connection)
     return connection
```

### Comparing `motordantic-0.0.2a1/motordantic/exceptions.py` & `motordantic-0.1.0a1/motordantic/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import json
 from time import sleep
 from types import GeneratorType
-from typing import Callable, Any
+from typing import Callable, Any, Union
 
 from pymongo.errors import (
     ServerSelectionTimeoutError,
     AutoReconnect,
     NetworkTimeout,
     ConnectionFailure,
 )
@@ -30,15 +31,27 @@
         self.model_name = model_name
 
     def __str__(self):
         return f'row does not exist for model: {self.model_name}'
 
 
 class MotordanticValidationError(BaseMotorDanticException):
-    pass
+    def __init__(self, error_message: Any, pydanctic_validation_error: Any = None):
+        self.error_message = error_message
+        self.pydanctic_validation_error = pydanctic_validation_error
+
+    def errors(self):
+        if self.pydanctic_validation_error is None:
+            return self.error_message
+        return self.pydanctic_validation_error.errors()
+
+    def json(self, *, indent: Union[None, int, str] = 2) -> str:
+        if self.pydanctic_validation_error is None:
+            return json.dumps(self.error_message, indent=indent)
+        return self.pydanctic_validation_error.json()
 
 
 class MotordanticInvalidArgsParams(BaseMotorDanticException):
     def __str__(self):
         return 'Arguments must be Query objects'
```

### Comparing `motordantic-0.0.2a1/motordantic/extra.py` & `motordantic-0.1.0a1/motordantic/query/extra.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,53 +13,50 @@
 from re import compile, IGNORECASE
 
 from bson import ObjectId, Regex
 from pymongo import UpdateOne
 from pydantic.fields import ModelField
 from pydantic.typing import get_origin
 
-from .property import cached_classproperty
-from .validaton import validate_field_value
-from .exceptions import MotordanticValidationError
-from .types import Relation, RelationInfo, RelationTypes
+from ..property import cached_classproperty
+from ..validation import validate_field_value, validate_object_id
+from ..exceptions import MotordanticValidationError
+from ..types import Relation, RelationInfo, RelationTypes
 
 __all__ = (
     'ExtraQueryMapper',
     'group_by_aggregate_generation',
     'generate_name_field',
     'chunk_by_length',
     'bulk_query_generator',
     'take_relation',
 )
 
 if TYPE_CHECKING:
-    from .models import MongoModel
-    from .typing import MongoModelType
+    from ..document import Document
 
 
 class ExtraQueryMapper(object):
     """extra mapper for __ queries like find(_id__in=[], name__regex='123')"""
 
     __slots__ = (
-        'mongo_model',
+        'document',
         'field_name',
     )
 
-    def __init__(
-        self, mongo_model: Union['MongoModel', 'MongoModelType'], field_name: str
-    ):
+    def __init__(self, document: 'Document', field_name: str):
         self.field_name = field_name
-        self.mongo_model = mongo_model
+        self.document = document
 
     def query(self, extra_methods: List, values: Any) -> Dict:
         if self.field_name == '_id':
             values = (
-                [ObjectId(v) for v in values]
+                [validate_object_id(self.document, v) for v in values]
                 if isinstance(values, list)
-                else ObjectId(values)
+                else validate_object_id(self.document, values)
             )
         if extra_methods:
             query: Dict = {self.field_name: {}}
             for extra_method in extra_methods:
                 if extra_method == 'in':
                     extra_method = 'in_'
                 elif extra_method == 'inc':
@@ -72,15 +69,15 @@
 
     def in_(self, list_values: List) -> dict:
         if not isinstance(list_values, list):
             raise TypeError("values must be a list type")
         try:
             return {
                 "$in": [
-                    validate_field_value(self.mongo_model, self.field_name, v)
+                    validate_field_value(self.document, self.field_name, v)
                     for v in list_values
                 ]
             }
         except MotordanticValidationError:
             return {"$in": list_values}
 
     def regex(self, regex_value: str) -> dict:
@@ -89,15 +86,15 @@
     def iregex(self, regex_value: str) -> dict:
         return {"$regex": Regex.from_native(compile(regex_value, IGNORECASE))}
 
     def regex_ne(self, regex_value: str) -> dict:
         return {"$not": Regex.from_native(compile(regex_value))}
 
     def ne(self, value: Any) -> dict:
-        return {"$ne": validate_field_value(self.mongo_model, self.field_name, value)}
+        return {"$ne": validate_field_value(self.document, self.field_name, value)}
 
     def startswith(self, value: str) -> dict:
         return {"$regex": Regex.from_native(compile(f"^{value}"))}
 
     def istartswith(self, value: str) -> dict:
         return {"$regex": Regex.from_native(compile(f"^{value}", IGNORECASE))}
 
@@ -118,15 +115,15 @@
 
     def nin(self, list_values: List) -> dict:
         if not isinstance(list_values, list):
             raise TypeError("values must be a list type")
         try:
             return {
                 "$nin": [
-                    validate_field_value(self.mongo_model, self.field_name, v)
+                    validate_field_value(self.document, self.field_name, v)
                     for v in list_values
                 ]
             }
         except MotordanticValidationError:
             return {"$nin": list_values}
 
     def exists(self, boolean_value: bool) -> dict:
@@ -143,38 +140,38 @@
     def all(self, query: Any) -> dict:
         return {'$all': query}
 
     def unset(self, value: Any) -> dict:
         return {"$unset": {self.field_name: value}}
 
     def gte(self, value: Any) -> dict:
-        return {"$gte": validate_field_value(self.mongo_model, self.field_name, value)}
+        return {"$gte": validate_field_value(self.document, self.field_name, value)}
 
     def lte(self, value: Any) -> dict:
-        return {"$lte": validate_field_value(self.mongo_model, self.field_name, value)}
+        return {"$lte": validate_field_value(self.document, self.field_name, value)}
 
     def gt(self, value: Any) -> dict:
-        return {"$gt": validate_field_value(self.mongo_model, self.field_name, value)}
+        return {"$gt": validate_field_value(self.document, self.field_name, value)}
 
     def lt(self, value: Any) -> dict:
-        return {"$lt": validate_field_value(self.mongo_model, self.field_name, value)}
+        return {"$lt": validate_field_value(self.document, self.field_name, value)}
 
     def inc(self, value: int) -> dict:
         if isinstance(value, int):
             return {'$inc': {self.field_name: value}}
         raise ValueError('value must be integer')
 
     def range(self, range_values: Union[List, Tuple]) -> dict:
         if len(range_values) != 2:
             raise ValueError("range must have 2 params")
         from_ = range_values[0]
         to_ = range_values[1]
         return {
-            "$gte": validate_field_value(self.mongo_model, self.field_name, from_),
-            "$lte": validate_field_value(self.mongo_model, self.field_name, to_),
+            "$gte": validate_field_value(self.document, self.field_name, from_),
+            "$lte": validate_field_value(self.document, self.field_name, to_),
         }
 
     @cached_classproperty
     def methods(cls) -> list:
         methods = []
         for f in cls.__dict__:
             if f == 'in_':
@@ -242,39 +239,39 @@
     return data
 
 
 def take_relation(field: ModelField) -> Optional[RelationInfo]:
     """take relations from model
 
     Args:
-        field (ModelField): MongoModel field
+        field (ModelField): Document field
 
     Returns:
         Optional[RelationInfo]: relation info
     """
     if field.type_ == Relation:
         if field.allow_none is True:
             return RelationInfo(
                 field=field.name,
-                mongo_model_class=field.sub_fields[0].type_,  # type: ignore
+                document_class=field.sub_fields[0].type_,  # type: ignore
                 relation_type=RelationTypes.OPTIONAL_SINGLE,
             )
         return RelationInfo(
             field=field.name,
-            mongo_model_class=field.sub_fields[0].type_,  # type: ignore
+            document_class=field.sub_fields[0].type_,  # type: ignore
             relation_type=RelationTypes.SINGLE,
         )
     if (
         inspect.isclass(get_origin(field.outer_type_))
         and issubclass(get_origin(field.outer_type_), list)  # type: ignore
         and len(field.sub_fields) == 1  # type: ignore
     ):
         internal_field = field.sub_fields[0]  # type: ignore
         if internal_field.type_ == Relation:
             if internal_field.allow_none is True:
                 return None
             return RelationInfo(
                 field=field.name,
-                mongo_model_class=internal_field.sub_fields[0].type_,  # type: ignore
+                document_class=internal_field.sub_fields[0].type_,  # type: ignore
                 relation_type=RelationTypes.ARRAY,
             )
     return None
```

### Comparing `motordantic-0.0.2a1/motordantic/fields.py` & `motordantic-0.1.0a1/motordantic/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Type, cast
 
 from pydantic.fields import Field as PydanticField
 from pydantic.fields import FieldInfo as PydanticFieldInfo
 from pydantic.fields import ModelField, Representation, Undefined
 
 __all__ = (
-    'Field',
-    'FieldInfo',
+    'ExtraDBField',
+    'MotordanticFieldInfo',
     'ComputedField',
     'computed_field',
 )
 
 if TYPE_CHECKING:
     from typing import Callable, Union
 
     from pydantic import BaseConfig, BaseModel
     from pydantic.class_validators import Validator
     from pydantic.fields import ModelField
 
 
-class FieldInfo:
+class MotordanticFieldInfo:
     __slots__ = ("pydantic_field_info", "db_field_name", "default")
 
     def __init__(
         self,
         *,
         pydantic_field_info: PydanticFieldInfo,
         db_field_name: Optional[str],
     ):
         self.pydantic_field_info = pydantic_field_info
         self.db_field_name = db_field_name
 
 
-def Field(
+def ExtraDBField(
     default: Any = Undefined,
     *,
-    db_field_name: Optional[str] = None,
+    db_field_name: str,
     default_factory: Optional[Callable[[], Any]] = None,
     title: Optional[str] = None,
     description: Optional[str] = None,
     const: Optional[bool] = None,
     gt: Optional[float] = None,
     ge: Optional[float] = None,
     lt: Optional[float] = None,
@@ -67,15 +67,18 @@
         min_items=cast(int, min_items),
         max_items=cast(int, max_items),
         min_length=cast(int, min_length),
         max_length=cast(int, max_length),
         regex=cast(str, regex),
         **extra,
     )
-    return FieldInfo(pydantic_field_info=pydantic_field, db_field_name=db_field_name)
+    return MotordanticFieldInfo(
+        pydantic_field_info=pydantic_field,
+        db_field_name=db_field_name,
+    )
 
 
 def computed_field(
     func: Optional[Any] = None,
     *,
     alias: Optional[str] = None,
     title: Optional[str] = None,
```

### Comparing `motordantic-0.0.2a1/motordantic/models.py` & `motordantic-0.1.0a1/motordantic/document.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,116 +6,142 @@
     Optional,
     List,
     Tuple,
     TYPE_CHECKING,
     ClassVar,
 )
 
-from bson import ObjectId, DBRef
-from motor.core import AgnosticClientSession, AgnosticCollection, AgnosticDatabase
-
+from bson import ObjectId, DBRef, decode as bson_decode
+from bson.raw_bson import RawBSONDocument
+from motor.core import AgnosticClientSession
 from pydantic.main import ModelMetaclass as PydanticModelMetaclass, default_ref_template
-from pydantic import BaseModel as BasePydanticModel, root_validator, BaseConfig
+from pydantic import (
+    BaseModel as BasePydanticModel,
+    root_validator,
+    BaseConfig,
+    ValidationError,
+)
 from pydantic.main import ValueItems, _missing
+from pydantic.typing import resolve_annotations
+from pydantic.fields import Undefined
 from pymongo import IndexModel
 
 
 from .relation import RelationManager
 from .types import ObjectIdStr, RelationInfo, Relation
 from .exceptions import (
-    NotDeclaredField,
-    MotordanticInvalidArgsParams,
     MotordanticValidationError,
     MotordanticConnectionError,
 )
 from .property import classproperty
-from .extra import ExtraQueryMapper, take_relation
-from .query import Query, QueryCombination, generate_basic_query
-from .querybuilder import QueryBuilder
-from .fields import ComputedField
+from .query.extra import take_relation
+from .fields import ComputedField, MotordanticFieldInfo
 from .schema import model_schema
+from .manager import ODMManager
 
 
-__all__ = ('MongoModel', 'ModelMetaclass')
+__all__ = ('Document', 'DocumentMetaclass')
 
 if TYPE_CHECKING:
+    from asyncio import AbstractEventLoop
     from pydantic.main import MappingIntStrAny, TupleGenerator
-    from .typing import DictStrAny, AbstractSetIntStr, SetStr, MongoModelType
-    from .connection import MotordanticConnection
+    from .typing import DictStrAny, AbstractSetIntStr, SetStr
+    from .query import QueryBuilder
+    from .sync.query import SyncQueryBuilder
 
 
-_is_mongo_model_class_defined = False
+_is_document_class_defined = False
 
 
-class ModelMetaclass(PydanticModelMetaclass):
+class DocumentMetaclass(PydanticModelMetaclass):
     def __new__(mcs, name, bases, namespace, **kwargs):  # type: ignore
+        annotations = resolve_annotations(
+            namespace.get("__annotations__", {}), namespace.get("__module__")
+        )
+        mapping_query_fields = {'_id': '_id'}
+        for field_name in annotations:
+            value = namespace.get(field_name, Undefined)
+            if isinstance(value, MotordanticFieldInfo):
+                namespace[field_name] = value.pydantic_field_info
+                mapping_query_fields[field_name] = value.db_field_name or field_name
+            else:
+                mapping_query_fields[field_name] = field_name
+        namespace['__mapping_query_fields__'] = mapping_query_fields
+        namespace['__mapping_from_fields__'] = {
+            db_field: cls_field for cls_field, db_field in mapping_query_fields.items()
+        }
         cls = super().__new__(mcs, name, bases, namespace, **kwargs)
         indexes = set()
         config = BaseConfig
-        if _is_mongo_model_class_defined and issubclass(cls, MongoModel):
+        if _is_document_class_defined and issubclass(cls, Document):
             db_refs = {}
             for k, v in cls.__fields__.items():
                 relation_info = take_relation(v)
                 if relation_info is not None:
                     db_refs[k] = relation_info
             setattr(cls, '__db_refs__', db_refs)
             if db_refs:
+                setattr(cls, 'has_relations', True)
                 setattr(cls, '__relation_manager__', RelationManager(cls))  # type: ignore
             computed_fields = {}
             for var_name, value in namespace.items():
                 if isinstance(value, ComputedField):
                     computed_fields[var_name] = value
                     value.set_config_and_prepare_field(config)
             if computed_fields:
                 setattr(cls, '__motordantic_computed_fields__', computed_fields)
         json_encoders = getattr(cls.Config, 'json_encoders', {})  # type: ignore
         json_encoders.update({ObjectId: lambda f: str(f)})
         setattr(cls.Config, 'json_encoders', json_encoders)  # type: ignore
         exclude_fields = getattr(cls.Config, 'exclude_fields', tuple())  # type: ignore
+        collection_name = (
+            getattr(cls.Config, 'collection_name', None) or cls.__name__.lower()
+        )
+        setattr(cls, '__collection_name__', collection_name)
         setattr(cls, '__indexes__', indexes)
         setattr(cls, '__database_exclude_fields__', exclude_fields)
+        setattr(cls, '__manager__', ODMManager(cls))  # type: ignore
         return cls
 
 
-class MongoModel(BasePydanticModel, metaclass=ModelMetaclass):
-    __database__: Optional[AgnosticDatabase] = None
-    __collection__: Optional[AgnosticCollection] = None
-    __connection__: Optional['MotordanticConnection'] = None
+class Document(BasePydanticModel, metaclass=DocumentMetaclass):
     __indexes__: 'SetStr' = set()
+    __manager__: ODMManager
     __database_exclude_fields__: Union[Tuple, List] = tuple()
-    __querybuilder__: Optional[QueryBuilder] = None
     __db_refs__: ClassVar[Optional[Dict[str, RelationInfo]]] = None
     __relation_manager__: Optional[RelationManager] = None
     __motordantic_computed_fields__: Dict[str, ComputedField] = {}
+    __mapping_query_fields__: Dict[str, str] = {}
+    __mapping_from_fields__: Dict[str, str] = {}
+    __collection_name__: Optional[str] = None
     _id: Optional[ObjectIdStr] = None
+    has_relations: ClassVar[bool] = False
+
+    def __init__(self, **data):
+        try:
+            super().__init__(**data)
+        except ValidationError as e:
+            raise MotordanticValidationError(e.errors, e)
 
     def __setattr__(self, key, value):
         if key == '_id':
             self.__dict__[key] = value
             return value
         else:
             return super().__setattr__(key, value)
 
     def __getattribute__(self, attr):
         attribute = super().__getattribute__(attr)
         if isinstance(attribute, ComputedField):
             return attribute.fget(self)
         return attribute
 
-    @classproperty
-    def relation_manager(cls) -> Optional[RelationManager]:
-        return cls.__relation_manager__
-
-    @classproperty
-    def connection(cls) -> Optional['MotordanticConnection']:
-        return cls.__connection__
-
-    @classmethod
-    async def _start_session(cls) -> AgnosticClientSession:
-        return await cls.Q.motor_client.start_session()
+    @property
+    def _io_loop(self) -> 'AbstractEventLoop':
+        return self.manager._io_loop
 
     @classmethod
     async def ensure_indexes(cls):
         """method for create/update/delete indexes if indexes declared in Config property"""
 
         indexes = getattr(cls.__config__, 'indexes', [])
         if not all([isinstance(index, IndexModel) for index in indexes]):
@@ -150,17 +176,20 @@
             for prop in dir(cls)
             if prop
             not in (
                 "__values__",
                 "data",
                 "querybuilder",
                 "Q",
+                "Qsync",
                 "pk",
                 "_query_data",
+                "_mongo_query_data",
                 "fields_all",
+                "_io_loop",
             )
             and isinstance(getattr(cls, prop), property)
         ]
 
     @classmethod
     def parse_obj(cls, data: Any) -> Any:
         if cls.__motordantic_computed_fields__:
@@ -192,15 +221,16 @@
                 ):
                     raise MotordanticValidationError('invalid field in updated_fields')
             else:
                 updated_fields = tuple(self.__fields__.keys())
             for field in updated_fields:
                 if field in self.__motordantic_computed_fields__:
                     continue
-                data[f'{field}__set'] = getattr(self, field)
+                else:
+                    data[f'{field}__set'] = getattr(self, field)
             await self.Q.update_one(
                 session=session,
                 **data,
             )
             return self
         data = {
             field: value
@@ -215,119 +245,40 @@
         return self
 
     def save_sync(
         self,
         updated_fields: Union[Tuple, List] = [],
         session: Optional[AgnosticClientSession] = None,
     ):
-        return self.Q.sync._io_loop.run_until_complete(
-            self.save(updated_fields, session)
-        )
+        return self._io_loop.run_until_complete(self.save(updated_fields, session))
 
     async def delete(self) -> None:
         await self.Q.delete_one(_id=self.pk)
 
     def delete_sync(self) -> None:
-        return self.Q.sync._io_loop.run_until_complete(self.delete())
-
-    @classmethod
-    def _validate_field(cls, field: str) -> bool:
-        if field not in cls.__fields__ and field != '_id':
-            raise NotDeclaredField(field, list(cls.__fields__.keys()))
-        elif field in cls.__database_exclude_fields__:
-            return False
-        return True
-
-    @classmethod
-    def _check_query_args(
-        cls,
-        logical_query: Union[
-            List[Any], Dict[Any, Any], str, Query, QueryCombination, None
-        ] = None,
-    ) -> 'DictStrAny':
-        """check if query = Query obj or QueryCombination
-
-        Args:
-            logical_query (Union[ List[Any], Dict[Any, Any], str, Query, QueryCombination ], optional): Query | QueryCombination. Defaults to None.
-
-        Raises:
-            InvalidArgsParams: if not Query | QueryCombination
-
-        Returns:
-            Dict: generated query dict
-        """
-        if not isinstance(logical_query, (QueryCombination, Query)):
-            raise MotordanticInvalidArgsParams()
-        return logical_query.to_query(cls)  # type: ignore
-
-    @classmethod
-    def use(cls: 'MongoModelType', connection: 'MotordanticConnection') -> None:
-        assert connection is not None
-        cls.__connection__ = connection
-        cls.__database__ = connection._get_motor_client().get_database(
-            connection.database_name
-        )
-
-    @classmethod
-    def _parse_extra_params(cls, extra_params: List) -> tuple:
-        field_param, extra = [], []
-        methods = ExtraQueryMapper.methods
-        for param in extra_params:
-            if param in methods:
-                extra.append(param)
-            else:
-                field_param.append(param)
-        return field_param, extra
-
-    @classmethod
-    def _validate_query_data(cls, query: Dict) -> 'DictStrAny':
-        """main validation method
-
-        Args:
-            query (Dict): basic query
-
-        Returns:
-            Dict: parsed query
-        """
-        query_params: dict = generate_basic_query(cls, query)
-
-        return query_params
-
-    @classproperty
-    def database(cls) -> AgnosticDatabase:
-        """Returns the database that is currently associated with this document."""
-        if not hasattr(cls, "__database__") or cls.__database__ is None:
-            raise AttributeError("Accessing database without using it first.")
-        return cls.__database__
-
-    @classproperty
-    def collection(cls: 'MongoModel') -> AgnosticCollection:
-        """Returns the collection for this :class:`MongoModel`."""
-        if (
-            cls.__collection__ is None
-            or cls.__collection__.database is not cls.database
-        ):
-            cls.__collection__ = cls.database.get_collection(cls.set_collection_name())  # type: ignore
-        return cls.__collection__
+        return self._io_loop.run_until_complete(self.delete())
 
     @classproperty
     def fields_all(cls) -> list:
         """return all fields with properties(not document fields)"""
         fields = list(cls.__fields__.keys())
         return_fields = fields + cls._get_properties()
         return return_fields
 
     @classproperty
-    def Q(cls) -> QueryBuilder:
-        if cls.connection is None:
-            raise RuntimeError('not connected to mongodb, use `connect`')
-        if cls.__querybuilder__ is None:
-            querybuilder = QueryBuilder(cls)
-            cls.__querybuilder__ = querybuilder
-        return cls.__querybuilder__
+    def manager(cls) -> ODMManager:
+        return cls.__manager__
+
+    @classproperty
+    def Q(cls) -> 'QueryBuilder':
+        return cls.manager.querybuilder
+
+    @classproperty
+    def Qsync(cls) -> 'SyncQueryBuilder':
+        return cls.manager.sync_querybuilder
 
     def _iter(
         self,
         to_dict: bool = False,
         by_alias: bool = False,
         include: Optional[Union['AbstractSetIntStr', 'MappingIntStrAny']] = None,
         exclude: Optional[Union['AbstractSetIntStr', 'MappingIntStrAny']] = None,
@@ -427,18 +378,19 @@
                 props = [prop for prop in props if prop in include]
             if exclude:
                 props = [prop for prop in props if prop not in exclude]
 
             # Update the attribute dict with the properties
             if props:
                 attribs.update({prop: getattr(self, prop) for prop in props})
-            if self.__motordantic_computed_fields__ and not with_props:
+        else:
+            if self.__motordantic_computed_fields__:
                 for field in self.__motordantic_computed_fields__:
                     attribs.pop(field)
-        if self.has_db_refs():
+        if self.has_relations:
             for field in self.__db_refs__:  # type: ignore
                 attrib_data = attribs[field]
                 if attrib_data and not isinstance(attrib_data, dict):
                     attribs[field] = (
                         attrib_data.to_dict()
                         if not isinstance(attrib_data, list)
                         else [
@@ -456,45 +408,55 @@
         if cached is not None:
             return cached
         s = model_schema(cls, by_alias=by_alias, ref_template=ref_template)
         cls.__schema_cache__[(by_alias, ref_template)] = s
         return s
 
     @classmethod
+    def from_bson(cls, bson_raw_data: RawBSONDocument) -> 'Document':
+        data = bson_decode(bson_raw_data.raw)
+        data = {
+            cls.__mapping_from_fields__[field]: value for field, value in data.items()
+        }
+        obj = cls(**data)
+        obj._id = data.get('_id')
+        return obj
+
+    @classmethod
     def to_db_ref(cls, object_id: Union[str, ObjectId]) -> DBRef:
         if isinstance(object_id, str):
             object_id = ObjectId(object_id)
-        db_ref = DBRef(collection=cls.set_collection_name(), id=object_id)
+        db_ref = DBRef(collection=cls.get_collection_name(), id=object_id)
         return db_ref
 
     @classmethod
     def to_relation(cls, object_id: Union[str, ObjectId]) -> Relation:
         db_ref = cls.to_db_ref(object_id=object_id)
         return Relation(db_ref, cls)
 
-    @classmethod
-    def has_db_refs(cls) -> bool:
-        return bool(cls.__db_refs__)
-
     @property
     def data(self) -> 'DictStrAny':
         return self.dict(with_props=True)
 
     @property
     def _query_data(self) -> 'DictStrAny':
         return self.dict(with_props=False)
 
+    @property
+    def _mongo_query_data(self) -> 'DictStrAny':
+        return self._query_data
+
     @classmethod
-    def set_collection_name(cls) -> str:
+    def get_collection_name(cls) -> str:
         """main method for set collection
 
         Returns:
             str: collection name
         """
-        return cls.__name__.lower()
+        return cls.__collection_name__ or cls.__name__.lower()
 
     def serialize(self, fields: Union[Tuple, List]) -> 'DictStrAny':
         data: dict = self.dict(include=set(fields))
         return {f: data[f] for f in fields}
 
     def serialize_json(self, fields: Union[Tuple, List]) -> str:
         return json.dumps(self.serialize(fields))
@@ -502,15 +464,15 @@
     @property
     def pk(self):
         return self._id
 
     @root_validator
     def validate_all_fields(cls, values):
         for field, value in values.items():
-            if isinstance(value, MongoModel):
+            if isinstance(value, Document):
                 raise ValueError(
-                    f'{field} - cant be instance of MongoModel without Relation'
+                    f'{field} - cant be instance of Document without Relation'
                 )
         return values
 
 
-_is_mongo_model_class_defined = True
+_is_document_class_defined = True
```

### Comparing `motordantic-0.0.2a1/motordantic/property.py` & `motordantic-0.1.0a1/motordantic/property.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a1/motordantic/query.py` & `motordantic-0.1.0a1/motordantic/query/query.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,158 +1,201 @@
 import copy
-from json import dumps
-from typing import Generator, List, Union, Any, Tuple, List, TYPE_CHECKING, Union
-
-from bson import ObjectId
+from typing import TYPE_CHECKING, Union, Dict, Type, Any
 
 from .extra import ExtraQueryMapper
-from .validaton import validate_field_value
+
+from ..validation import validate_field_value, validate_object_id
 
 
 __all__ = (
-    "Query",
-    "QueryCombination",
-    "FindResult",
-    "SimpleAggregateResult",
+    "Q",
+    "QCombination",
 )
 
 
 if TYPE_CHECKING:
-    from .models import MongoModel
-    from .typing import MongoModelType
+    from ..manager import ODMManager
+    from ..typing import DictStrAny
+    from .builder import Builder
 
 
-def _validate_query_data(
-    model: Union['MongoModel', 'MongoModelType'], query: dict
-) -> dict:
-    return model._validate_query_data(query)
+class BaseQuery(object):
+    __slots__ = ('_builder', 'method_name')
+
+    def __init__(self, builder: 'Builder', method_name: str):
+        self._builder = builder
+        self.method_name = method_name
+
+    def __call__(self, *args, **kwargs):
+        method = getattr(self._builder, self.method_name)
+        return method(*args, **kwargs)
+
+
+class Query(BaseQuery):
+    def __getattr__(self, method_name: str) -> 'Query':
+        return Query(self._builder, method_name)
+
+
+class QueryBuilder(object):
+    query_class: Type[BaseQuery] = Query
+
+    __slots__ = ('builder', '_valid_methods')
 
+    def __init__(self, builder: 'Builder'):
+        self.builder = builder
+        self._valid_methods = {
+            attr_name: attr_name
+            for attr_name in dir(self.builder)
+            if attr_name != 'odm_manager' and not attr_name.endswith('__')
+        }
 
-class QueryNodeVisitor(object):
-    """Base visitor class for visiting Query-object nodes in a query tree."""
+    def __getattr__(self, method_name: str) -> Any:
+        if method_name in self._valid_methods:
+            return self.query_class(self.builder, method_name)
+        raise AttributeError(f'invalid Q attr query: {method_name}')
+
+    def _validate_query_data(self, query: Dict) -> 'DictStrAny':
+        return self.builder._validate_query_data(query)
+
+    def _check_query_args(self, *args, **kwargs):
+        return self.builder._check_query_args(*args, **kwargs)
+
+    def _validate_raw_query(self, *args, **kwargs):
+        return self.builder._validate_raw_query(*args, **kwargs)
+
+    def __call__(self, method_name, *args, **method_kwargs):
+        return getattr(self, method_name)(*args, **method_kwargs)
+
+
+def _validate_query_data(builder: 'Builder', query: dict) -> dict:
+    return builder._validate_query_data(query)
+
+
+class QNodeVisitor(object):
+    """Base visitor class for visiting Q-object nodes in a query tree."""
 
     def prepare_combination(
-        self, combination: 'QueryCombination'
-    ) -> Union['QueryCombination', dict]:
-        """Called by QueryCombination objects."""
+        self, combination: 'QCombination'
+    ) -> Union['QCombination', dict]:
+        """Called by QCombination objects."""
         return combination
 
-    def visit_query(self, query: 'Query') -> Union['Query', dict]:
-        """Called by (New)Query objects."""
+    def visit_query(self, query: 'Q') -> Union['Q', dict]:
+        """Called by (New)Q objects."""
         return query
 
 
-class SimplificationVisitor(QueryNodeVisitor):
-    def __init__(self, model: Union['MongoModel', 'MongoModelType']):
-        self.model = model
+class SimplificationVisitor(QNodeVisitor):
+    def __init__(self, builder: 'Builder'):
+        self.builder = builder
 
     def prepare_combination(
-        self, combination: 'QueryCombination'
-    ) -> Union['QueryCombination', dict]:
+        self, combination: 'QCombination'
+    ) -> Union['QCombination', dict]:
         if combination.operation == combination.AND:
             # The simplification only applies to 'simple' queries
-            if all(isinstance(node, Query) for node in combination.children):
+            if all(isinstance(node, Q) for node in combination.children):
                 queries = [n.query for n in combination.children]
                 query = self._query_conjunction(queries)
                 return {"$and": query}
 
         return combination
 
     def _query_conjunction(self, queries):
         """Merges query dicts - effectively &ing them together."""
         combined_query = []
         for query in queries:
-            query = _validate_query_data(self.model, query)
+            query = _validate_query_data(self.builder, query)
             combined_query.append(copy.deepcopy(query))
         return combined_query
 
 
-class QueryCompilerVisitor(QueryNodeVisitor):
+class QCompilerVisitor(QNodeVisitor):
     """Compiles the nodes in a query tree to a PyMongo-compatible query
     dictionary.
     """
 
-    def __init__(self, model: Union['MongoModel', 'MongoModelType']):
-        self.model = model
+    def __init__(self, builder: 'Builder'):
+        self.builder = builder
 
     def prepare_combination(
-        self, combination: 'QueryCombination'
-    ) -> Union['QueryCombination', dict]:
+        self, combination: 'QCombination'
+    ) -> Union['QCombination', dict]:
         operator = "$and"
         if combination.operation == combination.OR:
             operator = "$or"
         return {operator: combination.children}
 
-    def visit_query(self, query: 'Query') -> Union['Query', dict]:
-        data = _validate_query_data(self.model, query.query)
+    def visit_query(self, query: 'Q') -> Union['Q', dict]:
+        data = _validate_query_data(self.builder, query.query)
         return data
 
 
-class QueryNode(object):
+class QNode(object):
     """Base class for nodes in query trees."""
 
     AND = 0
     OR = 1
 
-    def to_query(self, model: Union['MongoModel', 'MongoModelType']) -> dict:
-        query = self.accept(SimplificationVisitor(model))
+    def to_query(self, builder: 'Builder') -> dict:
+        query = self.accept(SimplificationVisitor(builder))
         if not isinstance(query, dict):
-            query = query.accept(QueryCompilerVisitor(model))
+            query = query.accept(QCompilerVisitor(builder))
         return query
 
     def accept(self, visitor):
         raise NotImplementedError
 
     def _combine(self, other, operation):
-        """Combine this node with another node into a QueryCombination
+        """Combine this node with another node into a QCombination
         object.
         """
-        # If the other Query() is empty, ignore it and just use `self`.
+        # If the other Q() is empty, ignore it and just use `self`.
         if getattr(other, "empty", True):
             return self
 
         # Or if this Q is empty, ignore it and just use `other`.
         if self.empty:
             return other
 
-        return QueryCombination(operation, [self, other])
+        return QCombination(operation, [self, other])
 
     @property
     def empty(self):
         return False
 
     def __or__(self, other):
         return self._combine(other, self.OR)
 
     def __and__(self, other):
         return self._combine(other, self.AND)
 
 
-class QueryCombination(QueryNode):
+class QCombination(QNode):
     def __init__(self, operation, children):
         self.operation = operation
         self.children = []
         for node in children:
             # If the child is a combination of the same type, we can merge its
             # children directly into this combinations children
-            if isinstance(node, QueryCombination) and node.operation == operation:
+            if isinstance(node, QCombination) and node.operation == operation:
                 self.children += node.children
             else:
                 self.children.append(node)
 
     def __repr__(self):
         op = " & " if self.operation is self.AND else " | "
         return "(%s)" % op.join([repr(node) for node in self.children])
 
     def __bool__(self):
         return bool(self.children)
 
-    def accept(self, visitor) -> Union['QueryCombination', dict]:
+    def accept(self, visitor) -> Union['QCombination', dict]:
         for i in range(len(self.children)):
-            if isinstance(self.children[i], QueryNode):
+            if isinstance(self.children[i], QNode):
                 self.children[i] = self.children[i].accept(visitor)
 
         return visitor.prepare_combination(self)
 
     @property
     def empty(self):
         return not bool(self.children)
@@ -161,139 +204,66 @@
         return (
             self.__class__ == other.__class__
             and self.operation == other.operation
             and self.children == other.children
         )
 
 
-class Query(QueryNode):
+class Q(QNode):
     """A simple query object, used in a query tree to build up more complex
     query structures.
     """
 
     def __init__(self, **query):
         self.query = query
 
     def __repr__(self):
-        return "Query(**%s)" % repr(self.query)
+        return "Q(**%s)" % repr(self.query)
 
     def __bool__(self):
         return bool(self.query)
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.query == other.query
 
-    def accept(self, visit: 'QueryNodeVisitor') -> Union['Query', dict]:
+    def accept(self, visit: 'QNodeVisitor') -> Union['Q', dict]:
         return visit.visit_query(self)
 
     @property
     def empty(self) -> bool:
         return not bool(self.query)
 
 
-class FindResult(object):
-    __slots__ = ('_data', 'mongo_model_class')
-
-    def __init__(
-        self,
-        mongo_model_class: 'MongoModel',
-        data: list,
-    ):
-        self._data = data
-        self.mongo_model_class = mongo_model_class
-
-    # @handle_and_convert_connection_errors
-    def __iter__(self):
-        for obj in self._data:
-            yield obj
-
-    def __next__(self):
-        return next(self.__iter__())
-
-    @property
-    def data(self) -> List:
-        return [obj.data for obj in self.__iter__()]
-
-    @property
-    def generator(self) -> Generator:
-        return self.__iter__()
-
-    @property
-    def data_generator(self) -> Generator:
-        for obj in self.__iter__():
-            yield obj.data
-
-    @property
-    def list(self) -> List:
-        return list(self.__iter__())
-
-    def json(self) -> str:
-        return dumps(self.data)
-
-    def first(self) -> Any:
-        return next(self.__iter__())
-
-    def serialize(
-        self, fields: Union[Tuple, List], to_list: bool = True
-    ) -> Union[Tuple, List]:
-        return (
-            [obj.serialize(fields) for obj in self.__iter__()]
-            if to_list
-            else tuple(obj.serialize(fields) for obj in self.__iter__())
-        )
-
-    def serialize_generator(self, fields: Union[Tuple, List]) -> Generator:
-        for obj in self.__iter__():
-            yield obj.serialize(fields)
-
-    def serialize_json(self, fields: Union[Tuple, List]) -> str:
-        return dumps(self.serialize(fields))
-
-
-class SimpleAggregateResult(object):
-    __slots__ = ('_data', 'mongo_model_class')
-
-    def __init__(
-        self,
-        mongo_model_class: 'MongoModel',
-        data: dict,
-    ):
-        self._data = data
-        self.mongo_model_class = mongo_model_class
-
-    def json(self) -> str:
-        return dumps(self._data)
-
-    @property
-    def data(self) -> dict:
-        return self._data
-
-
 def generate_basic_query(
-    cls: Union['MongoModel', 'MongoModelType'],
+    manager: 'ODMManager',
     query: dict,
-    with_validate_model_fields: bool = True,
+    with_validate_document_fields: bool = True,
 ) -> dict:
     query_params: dict = {}
     for query_field, value in query.items():
         field, *extra_params = query_field.split("__")
-        inners, extra_params = cls._parse_extra_params(extra_params)
-        if with_validate_model_fields and not cls._validate_field(field):
+        inners, extra_params = manager._parse_extra_params(extra_params)
+        if with_validate_document_fields and not manager._validate_field(field):
             continue
-        extra = ExtraQueryMapper(cls, field).query(extra_params, value)
+        query_field_name = manager.document.__mapping_query_fields__[field]
+        extra = ExtraQueryMapper(manager.document, field).query(extra_params, value)
         if extra:
             value = extra[field]
         elif field == '_id':
-            value = ObjectId(value)
+            value = validate_object_id(manager.document, value)
         else:
-            value = validate_field_value(cls, field, value) if not inners else value
+            value = (
+                validate_field_value(manager.document, field, value)
+                if not inners
+                else value
+            )
         if inners:
-            field = f'{field}.{".".join(i for i in inners)}'
+            query_field_name = f'{query_field_name}.{".".join(i for i in inners)}'
         if (
             extra
-            and field in query_params
+            and query_field_name in query_params
             and ('__gt' in query_field or '__lt' in query_field)
         ):
-            query_params[field].update(value)
+            query_params[query_field_name].update(value)
         else:
-            query_params[field] = value
+            query_params[query_field_name] = value
     return query_params
```

### Comparing `motordantic-0.0.2a1/motordantic/querybuilder.py` & `motordantic-0.1.0a1/motordantic/query/builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,95 @@
-import asyncio
 from typing import (
     AsyncIterable,
     Union,
     List,
     Dict,
     Optional,
     Any,
     Tuple,
     TYPE_CHECKING,
     Iterable,
-    Type,
-    no_type_check,
 )
 
-from bson import ObjectId
+from bson import ObjectId, decode as bson_decode
+from bson.raw_bson import RawBSONDocument
 from pymongo import ReturnDocument, IndexModel
+from pymongo.collection import WriteConcern
 from motor.core import AgnosticClientSession as ClientSession
 
-
-from .query import Query, QueryCombination, FindResult, SimpleAggregateResult
-from .validaton import sort_validation
-from .exceptions import DoesNotExist, MotordanticValidationError, MotordanticIndexError
-from .aggregate_expressions import Sum, Max, Min, Avg
-from .aggregate import Aggregate
-from .extra import (
-    generate_name_field,
-    group_by_aggregate_generation,
-    bulk_query_generator,
-    chunk_by_length,
+from .query import generate_basic_query, Q, QCombination
+from .result import FindResult, SimpleAggregateResult
+from .extra import group_by_aggregate_generation, generate_name_field
+
+from ..aggregate.expressions import Sum, Max, Min, Avg
+from ..exceptions import (
+    MotordanticInvalidArgsParams,
+    MotordanticValidationError,
+    MotordanticIndexError,
+    DoesNotExist,
 )
+from ..validation import sort_validation
+
 
-__all__ = ('QueryBuilder',)
+__all__ = ('Builder',)
 
 if TYPE_CHECKING:
-    from .models import MongoModel
+    from ..manager import ODMManager
+    from ..typing import DictStrAny
+    from ..document import Document
+
 
+class Builder(object):
+    __slots__ = ('odm_manager',)
 
-MongoModelType = Type['MongoModel']
+    def __init__(self, odm_manager: 'ODMManager'):
+        self.odm_manager: 'ODMManager' = odm_manager
 
+    def _validate_query_data(self, query: Dict) -> 'DictStrAny':
+        """main validation method
 
-class QueryBuilder(object):
-    __slots__ = ('mongo_model_class', 'motor_client', '_io_loop')
+        Args:
+            query (Dict): basic query
 
-    def __init__(self, mongo_model_class: 'MongoModel'):
-        self.mongo_model_class: 'MongoModel' = mongo_model_class
-        self.motor_client = mongo_model_class.connection._get_motor_client()
+        Returns:
+            Dict: parsed query
+        """
+        query_params: dict = generate_basic_query(self.odm_manager, query)
 
-    @property
-    def sync(self) -> "SyncQueryBuilder":
-        s = SyncQueryBuilder(self.mongo_model_class)
-        return s
+        return query_params
+
+    def _check_query_args(
+        self,
+        logical_query: Union[
+            List[Any], Dict[Any, Any], str, Q, QCombination, None
+        ] = None,
+    ) -> 'DictStrAny':
+        """check if query = Query obj or QueryCombination
+
+        Args:
+            logical_query (Union[ List[Any], Dict[Any, Any], str, Q, QCombination ], optional): Query | QueryCombination. Defaults to None.
+
+        Raises:
+            InvalidArgsParams: if not Query | QueryCombination
+
+        Returns:
+            Dict: generated query dict
+        """
+        if not isinstance(logical_query, (Q, QCombination)):
+            raise MotordanticInvalidArgsParams()
+        return logical_query.to_query(self)  # type: ignore
 
     async def _make_query(
         self,
         method_name: str,
-        query_params: Union[List, Dict, str, Query, QueryCombination],
+        query_params: Union[List, Dict, str, Q, QCombination],
         set_values: Optional[Dict] = None,
         session: Optional[ClientSession] = None,
         logical: bool = False,
+        write_concern: Optional[WriteConcern] = None,
         **kwargs,
     ) -> Any:
         """main query function
 
         Args:
             method_name (str): query method like find, find_one and other
             query_params (Union[List, Dict, str, Query, LogicalCombination]): query params: dict or Query or LogicalCombination
@@ -69,43 +97,56 @@
             session (Optional[ClientSession], optional): motor session. Defaults to None.
             logical (bool, optional): if logical. Defaults to False.
 
         Returns:
             Any: query result
         """
         if logical:
-            query_params = self.mongo_model_class._check_query_args(query_params)
+            query_params = self._check_query_args(query_params)
         elif isinstance(query_params, dict):
-            query_params = self.mongo_model_class._validate_query_data(query_params)
-        method = getattr(self.mongo_model_class.collection, method_name)
+            query_params = self._validate_query_data(query_params)
+        if write_concern:
+            collection = self.odm_manager.collection.with_options(  # type: ignore
+                write_concern=write_concern
+            )
+        else:
+            collection = self.odm_manager.collection
+        print(query_params)
+        method = getattr(collection, method_name)
         query: tuple = (query_params,)
         if session:
             kwargs['session'] = session
         if set_values:
             query = (query_params, set_values)
         if kwargs:
             return await method(*query, **kwargs)
         return await method(*query)
 
+    async def get(self, session: Optional[ClientSession] = None, **query) -> 'Document':
+        obj = await self.find_one(session=session, **query)
+        if not obj:
+            raise DoesNotExist(self.odm_manager.document.__name__)
+        return obj
+
     async def count(
         self,
-        logical_query: Union[Query, QueryCombination, None] = None,
+        logical_query: Union[Q, QCombination, None] = None,
         session: Optional[ClientSession] = None,
         **query,
     ) -> int:
         """count query
 
         Args:
-            logical_query (Union[Query, QueryCombination, None], optional): Query | QueryCombination. Defaults to None.
+            logical_query (Union[Q, QCombination, None], optional): Query | QueryCombination. Defaults to None.
             session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
             int: count of documents
         """
-        if getattr(self.mongo_model_class.collection, 'count_documents'):
+        if getattr(self.odm_manager.collection, 'count_documents'):
             return await self._make_query(
                 'count_documents',
                 logical_query or query,
                 session=session,
                 logical=bool(logical_query),
             )
         return await self._make_query(
@@ -113,15 +154,15 @@
             logical_query or query,
             session=session,
             logical=bool(logical_query),
         )
 
     async def count_documents(
         self,
-        logical_query: Union[Query, QueryCombination, None] = None,
+        logical_query: Union[Q, QCombination, None] = None,
         session: Optional[ClientSession] = None,
         **query,
     ) -> int:
         """count_documents query
 
         Args:
             logical_query (Union[Query, LogicalCombination, None], optional): Query | QueryCombination. Defaults to None.
@@ -139,48 +180,66 @@
 
         Args:
             session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
             ObjectId: created document _id
         """
-        obj = self.mongo_model_class.parse_obj(query)
-        data = await self._make_query('insert_one', obj._query_data, session=session)
+        obj = self.odm_manager.document.parse_obj(query)
+        data = await self._make_query(
+            'insert_one',
+            obj._mongo_query_data,
+            session=session,
+        )
         return data.inserted_id
 
     async def insert_many(
-        self, data: List, session: Optional[ClientSession] = None
+        self,
+        data: List,
+        session: Optional[ClientSession] = None,
+        ordered: bool = True,
+        bypass_document_validation: bool = False,
+        write_concern: Optional[WriteConcern] = None,
     ) -> int:
         """insert many documents
 
         Args:
-            data (List): List of dict or MongoModels
+            data (List): List of dict or Documents
             session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
             int: count inserted ids
         """
-        parse_obj = self.mongo_model_class.parse_obj
+        parse_obj = self.odm_manager.document.parse_obj
         query = [
-            parse_obj(obj)._query_data if isinstance(obj, dict) else obj._query_data
+            parse_obj(obj)._mongo_query_data
+            if isinstance(obj, dict)
+            else obj._mongo_query_data
             for obj in data
         ]
-        r = await self._make_query('insert_many', query, session=session)
+        r = await self._make_query(
+            'insert_many',
+            query,
+            session=session,
+            ordered=ordered,
+            bypass_document_validation=bypass_document_validation,
+            write_concern=write_concern,
+        )
         return len(r.inserted_ids)
 
     async def delete_one(
         self,
-        logical_query: Union[Query, QueryCombination, None] = None,
+        logical_query: Union[Q, QCombination, None] = None,
         session: Optional[ClientSession] = None,
         **query,
     ) -> int:
         """delete one document
 
         Args:
-            logical_query (Union[Query, QueryCombination, None], optional): Query|QueryCombination. Defaults to None.
+            logical_query (Union[Q, QCombination, None], optional): Query|QueryCombination. Defaults to None.
             session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
             int: deleted documents count
         """
         r = await self._make_query(
             'delete_one',
@@ -188,112 +247,121 @@
             session=session,
             logical=bool(logical_query),
         )
         return r.deleted_count
 
     async def delete_many(
         self,
-        logical_query: Union[Query, QueryCombination, None] = None,
+        logical_query: Union[Q, QCombination, None] = None,
         session: Optional[ClientSession] = None,
         **query,
     ) -> int:
         """delete many document
 
         Args:
-            logical_query (Union[Query, QueryCombination, None], optional): Query|QueryCombination. Defaults to None.
+            logical_query (Union[Q, QCombination, None], optional): Query|QueryCombination. Defaults to None.
             session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
             int: deleted documents count
         """
         r = await self._make_query(
             'delete_many',
             logical_query or query,
             session=session,
             logical=bool(logical_query),
         )
         return r.deleted_count
 
-    async def list_indexes(self, session: Optional[ClientSession] = None) -> dict:
-        """get indexes for this collection
+    async def distinct(
+        self, field: str, session: Optional[ClientSession] = None, **query
+    ) -> list:
+        """wrapper for pymongo distinct
+
+        Args:
+            field (str): distinct field
+            session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
-            dict: indexes result
+            list: list of distinct values
         """
-        list_indexes_cursor = getattr(self.mongo_model_class.collection, 'list_indexes')
-        query = list_indexes_cursor(session=session)
-        index_list = await query.to_list(None)
-        return_data = {}
-        for index in index_list:
-            dict_index = dict(index)
-            data = {dict_index['name']: {'key': dict(dict_index['key'])}}
-            return_data.update(data)
-        return return_data
+        query = self._validate_query_data(query)
+        method = getattr(self.odm_manager.collection, 'distinct')
+        return await method(key=field, filter=query, session=session)
 
-    async def create_indexes(
+    async def find_one(
         self,
-        indexes: List[IndexModel],
+        logical_query: Union[Q, QCombination, None] = None,
+        sort_fields: Optional[Union[Tuple, List]] = None,
         session: Optional[ClientSession] = None,
-    ) -> List[str]:
-        create_indexes_cursor = getattr(
-            self.mongo_model_class.collection, 'create_index'
-        )
-        result = []
-        for index in indexes:
-            index_value = list(index.document['key'].items())
-            res = await create_indexes_cursor(
-                index_value,
-                session=session,
-                background=True,
-            )
-            result.append(res)
-        return result
+        sort: Optional[int] = None,
+        with_relations_objects: bool = False,
+        **query,
+    ) -> Optional['Document']:
+        """find one document
 
-    async def drop_index(
-        self, index_name: str, session: Optional[ClientSession] = None
-    ) -> str:
-        indexes = await self.list_indexes(session)
-        if index_name in indexes:
-            await self._make_query('drop_index', index_name, session=session)
-            return f'{index_name} dropped.'
-        raise MotordanticIndexError(f'invalid index name - {index_name}')
+        Args:
+            logical_query (Union[Q, QCombination, None], optional): Query | LogicalCombination. Defaults to None.
+            session (Optional[ClientSession], optional): motor session. Defaults to None.
+            sort_fields (Optional[Union[Tuple, List]], optional): iterable from sort fielda. Defaults to None.
+            sort (Optional[int], optional): sort value -1 or 1. Defaults to None.
+
+        Returns:
+            Optional[Document]: Document instance or None
+        """
+        sort, sort_fields = sort_validation(sort, sort_fields)
+        data = await self._make_query(
+            'find_one',
+            logical_query or query,
+            logical=bool(logical_query),
+            sort=[(field, sort or 1) for field in sort_fields] if sort_fields else None,
+            session=session,
+        )
+        if data is not None:
+            obj = self.odm_manager.document.from_bson(data)
+            if with_relations_objects and self.odm_manager.relation_manager:
+                obj = await self.odm_manager.relation_manager.map_relation_for_single(
+                    obj
+                )
+            return obj
+        return None
 
     async def _find(
         self,
-        logical_query: Union[Query, QueryCombination, None] = None,
+        logical_query: Union[Q, QCombination, None] = None,
         skip_rows: Optional[int] = None,
         limit_rows: Optional[int] = None,
         session: Optional[ClientSession] = None,
         sort_fields: Optional[Union[Tuple, List]] = None,
         sort: Optional[int] = None,
         **query,
     ) -> AsyncIterable:
         sort, sort_fields_parsed = sort_validation(sort, sort_fields)
 
         async def context():
             if bool(logical_query):
-                query_params = self.mongo_model_class._check_query_args(logical_query)
+                query_params = self._check_query_args(logical_query)
             else:
-                query_params = self.mongo_model_class._validate_query_data(query)
-            find_cursor_method = getattr(self.mongo_model_class.collection, 'find')
+                query_params = self._validate_query_data(query)
+            find_cursor_method = getattr(self.odm_manager.collection, 'find')
             cursor = find_cursor_method(query_params, session=session)
             if skip_rows is not None:
                 cursor = cursor.skip(skip_rows)
             if limit_rows:
                 cursor = cursor.limit(limit_rows)
             if sort:
                 cursor.sort([(field, sort or 1) for field in sort_fields_parsed])
             async for doc in cursor:
-                yield self.mongo_model_class.parse_obj(doc)
+                yield self.odm_manager.document.from_bson(doc)
 
         return context()
 
     async def find(
         self,
-        logical_query: Union[Query, QueryCombination, None] = None,
+        logical_query: Union[Q, QCombination, None] = None,
         skip_rows: Optional[int] = None,
         limit_rows: Optional[int] = None,
         session: Optional[ClientSession] = None,
         sort_fields: Optional[Union[Tuple, List]] = None,
         sort: Optional[int] = None,
         with_relations_objects: bool = False,
         **query,
@@ -308,283 +376,43 @@
             sort_fields (Optional[Union[Tuple, List]], optional): iterable from sort fielda. Defaults to None.
             sort (Optional[int], optional): sort value -1 or 1. Defaults to None.
 
         Returns:
             FindResult: Motordantic FindResult
         """
         result = await self._find(
-            logical_query, skip_rows, limit_rows, session, sort_fields, sort, **query
-        )
-        data = [doc async for doc in result]
-        if with_relations_objects and self.mongo_model_class.relation_manager:
-            data = await self.mongo_model_class.relation_manager.map_relation_for_array(
-                data
-            )
-        return FindResult(self.mongo_model_class, data)
-
-    async def find_with_count(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        skip_rows: Optional[int] = None,
-        limit_rows: Optional[int] = None,
-        session: Optional[ClientSession] = None,
-        sort_fields: Optional[Union[Tuple, List]] = None,
-        sort: Optional[int] = None,
-        **query,
-    ) -> Tuple[int, FindResult]:
-        """find and count
-
-        Args:
-            logical_query (Union[Query, LogicalCombination, None], optional): Query|QueryCombination or None. Defaults to None.
-            skip_rows (Optional[int], optional): for pagination. Defaults to None.
-            limit_rows (Optional[int], optional): for pagination. Defaults to None.
-            session (Optional[ClientSession], optional): pymongo session. Defaults to None.
-            sort_fields (Optional[Union[Tuple, List]], optional): field for sort. Defaults to None.
-            sort (Optional[int], optional): sort value. Defaults to None.
-
-        Returns:
-            Tuple[int, FindResult]: count of query data, FindResult
-        """
-        count = await self.count(
-            session=session,
-            logical_query=logical_query,
+            logical_query,
+            skip_rows,
+            limit_rows,
+            session,
+            sort_fields,
+            sort,
             **query,
         )
-        results = await self.find(
-            skip_rows=skip_rows,
-            limit_rows=limit_rows,
-            session=session,
-            logical_query=logical_query,
-            sort_fields=sort_fields,
-            sort=sort,
-            **query,
-        )
-        return count, results
-
-    async def find_one(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        sort_fields: Optional[Union[Tuple, List]] = None,
-        session: Optional[ClientSession] = None,
-        sort: Optional[int] = None,
-        with_relations_objects: bool = False,
-        **query,
-    ) -> Optional['MongoModel']:
-        """find one document
-
-        Args:
-            logical_query (Union[Query, QueryCombination, None], optional): Query | LogicalCombination. Defaults to None.
-            session (Optional[ClientSession], optional): motor session. Defaults to None.
-            sort_fields (Optional[Union[Tuple, List]], optional): iterable from sort fielda. Defaults to None.
-            sort (Optional[int], optional): sort value -1 or 1. Defaults to None.
-
-        Returns:
-            Optional[MongoModel]: MongoModel instance or None
-        """
-        sort, sort_fields = sort_validation(sort, sort_fields)
-        data = await self._make_query(
-            'find_one',
-            logical_query or query,
-            logical=bool(logical_query),
-            sort=[(field, sort or 1) for field in sort_fields] if sort_fields else None,
-            session=session,
-        )
-        if data:
-            obj = self.mongo_model_class.parse_obj(data)
-            if with_relations_objects and self.mongo_model_class.relation_manager:
-                obj = await self.mongo_model_class.relation_manager.map_relation_for_single(
-                    obj
-                )
-            return obj
-        return None
+        data = [doc async for doc in result]
+        if with_relations_objects and self.odm_manager.relation_manager:
+            data = await self.odm_manager.relation_manager.map_relation_for_array(data)
+        return FindResult(self.odm_manager.document, data)
 
     def _prepare_update_data(self, **fields) -> tuple:
         """prepare and validate query data for update queries"""
 
         if not any("__set" in f for f in fields):
             raise MotordanticValidationError("not fields for updating!")
         query_params = {}
         set_values = {}
         for name, value in fields.items():
             if name.endswith('__set'):
                 name = name.replace('__set', '')
-                data = self.mongo_model_class._validate_query_data({name: value})
+                data = self._validate_query_data({name: value})
                 set_values.update(data)
             else:
                 query_params.update({name: value})
         return query_params, set_values
 
-    async def replace_one(
-        self,
-        replacement: Dict,
-        upsert: bool = False,
-        session: Optional[ClientSession] = None,
-        **filter_query,
-    ) -> Any:
-        """replace one
-
-        Args:
-            replacement (Dict): replacement object
-            upsert (bool, optional): pymongo upsert. Defaults to False.
-            session (Optional[ClientSession], optional): motor session. Defaults to None.
-
-        Raises:
-            MotordanticValidationError: if not filter query
-            MotordanticValidationError: if not replacement obj
-
-        Returns:
-            Any: pymongo replace_one query result
-        """
-        if not filter_query:
-            raise MotordanticValidationError('not filter parameters')
-        if not replacement:
-            raise MotordanticValidationError('not replacement parameters')
-        return await self._make_query(
-            'replace_one',
-            self.mongo_model_class._validate_query_data(filter_query),
-            replacement=self.mongo_model_class._validate_query_data(replacement),
-            upsert=upsert,
-            session=session,
-        )
-
-    async def get(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        session: Optional[ClientSession] = None,
-        sort_fields: Optional[Union[Tuple, List]] = None,
-        sort: Optional[int] = None,
-        with_relations_objects: bool = False,
-        **query,
-    ) -> Any:
-        """method like django orm get
-
-        Args:
-            logical_query (Union[Query, QueryCombination, None], optional): Query objects. Defaults to None.
-            session (Optional[ClientSession], optional): mongo session. Defaults to None.
-            sort_fields (Optional[Union[Tuple, List]], optional): sorts. Defaults to None.
-            sort (Optional[int], optional): sort. Defaults to None.
-
-        Raises:
-            DoesNotExist: raise if not found object
-
-        Returns:
-            Any: mongo model
-        """
-
-        obj = await self.find_one(
-            logical_query=logical_query,
-            session=session,
-            sort_fields=sort_fields,
-            sort=sort,
-            **query,
-        )
-        if not obj:
-            raise DoesNotExist(self.mongo_model_class.__name__)  # type: ignore
-        if with_relations_objects and self.mongo_model_class.relation_manager:
-            obj = await self.mongo_model_class.relation_manager.map_relation_for_single(
-                obj
-            )
-        return obj
-
-    async def get_or_create(self, **query) -> Tuple:
-        """like django orm get_or_create
-
-        Returns:
-            Tuple: MongoModel instance, True/False
-        """
-        defaults = query.pop('defaults', {})
-        with_relations_objects = query.pop('with_relations_objects', False)
-        obj = await self.find_one(
-            **query, with_relations_objects=with_relations_objects
-        )
-        if obj:
-            created = False
-        else:
-            created = True
-            inserted_id = await self.insert_one(**{**query, **defaults})
-            obj = await self.find_one(
-                _id=inserted_id, with_relations_objects=with_relations_objects
-            )
-        return obj, created
-
-    async def update_or_create(self, **query) -> Tuple:
-        """like django orm update_or_create
-
-        Returns:
-            Tuple: MongoModel instance, True/False
-        """
-        defaults = query.pop('defaults', {})
-        with_relations_objects = query.pop('with_relations_objects', False)
-        obj = await self.find_one(
-            **query, with_relations_objects=with_relations_objects
-        )
-        if obj is not None:
-            created = False
-            for field, value in defaults.items():
-                setattr(obj, field, value)
-        else:
-            created = True
-            obj = self.mongo_model_class(**{**query, **defaults})  # type: ignore
-        await obj.save()
-        if with_relations_objects:
-            obj = await self.get(
-                _id=obj._id, with_relations_objects=with_relations_objects
-            )
-        return obj, created
-
-    def _validate_raw_query(
-        self, method_name: str, raw_query: Union[Dict, List[Dict], Tuple[Dict]]
-    ) -> tuple:
-        if (
-            'insert' in method_name
-            or 'replace' in method_name
-            or 'update' in method_name
-        ):
-            if isinstance(raw_query, list):
-                raw_query = list(
-                    map(self.mongo_model_class._validate_query_data, raw_query)
-                )
-            elif isinstance(raw_query, dict):
-                raw_query = self.mongo_model_class._validate_query_data(raw_query)
-            else:
-                params = [
-                    query[key] if '$' in key else query
-                    for query in raw_query
-                    for key in query.keys()
-                ]
-                map(self.mongo_model_class._validate_query_data, params)
-        parsed_query = raw_query if isinstance(raw_query, tuple) else (raw_query,)
-        return parsed_query
-
-    async def raw_query(
-        self,
-        method_name: str,
-        raw_query: Union[Dict, List[Dict], Tuple[Dict]],
-        session: Optional[ClientSession] = None,
-    ) -> Any:
-        """pymongo raw query
-
-        Args:
-            method_name (str): pymongo method, like insert_one
-            raw_query (Union[Dict, List[Dict], Tuple[Dict]]): query data
-            session (Optional[ClientSession], optional): motor session. Defaults to None.
-
-        Raises:
-            MongoValidationError: raise if invalid data
-
-        Returns:
-            Any: pymongo query result
-        """
-        parsed_query = self._validate_raw_query(method_name, raw_query)
-        try:
-            query = getattr(self.mongo_model_class.collection, method_name)
-            return await query(*parsed_query, session=session)
-        except AttributeError:
-            raise MotordanticValidationError('invalid method name')
-
     async def _update(
         self,
         method: str,
         query: Dict,
         upsert: bool = True,
         session: Optional[ClientSession] = None,
     ) -> int:
@@ -629,271 +457,36 @@
             session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
             int: updated documents count
         """
         return await self._update('update_many', query, upsert=upsert, session=session)
 
-    async def distinct(
-        self, field: str, session: Optional[ClientSession] = None, **query
-    ) -> list:
-        """wrapper for pymongo distinct
-
-        Args:
-            field (str): distinct field
-            session (Optional[ClientSession], optional): motor session. Defaults to None.
-
-        Returns:
-            list: list of distinct values
-        """
-        query = self.mongo_model_class._validate_query_data(query)
-        method = getattr(self.mongo_model_class.collection, 'distinct')
-        return await method(key=field, filter=query, session=session)
-
-    async def raw_aggregate(
-        self, data: List[Dict[Any, Any]], session: Optional[ClientSession] = None
-    ) -> list:
-        """raw aggregation query
-
-        Args:
-            data (List[Dict[Any, Any]]): aggregation query
-            session (Optional[ClientSession], optional): motor session. Defaults to None.
-
-        Returns:
-            list: aggregation result
-        """
-        result = await self._motor_aggreggate_call(data, session)
-        return [row async for row in result]
-
-    async def _motor_aggreggate_call(
-        self, data: list, session: Optional[ClientSession]
-    ) -> AsyncIterable:
-        async def context():
-            aggregate_cursor = getattr(self.mongo_model_class.collection, 'aggregate')
-
-            async for row in aggregate_cursor(data, session=session):
-                yield row
-
-        return context()
-
-    async def _aggregate(self, *args, **query) -> SimpleAggregateResult:
-        """main aggregate method
-
-        Raises:
-            MongoValidationError: miss aggregation or group_by
-
-        Returns:
-            dict: aggregation result
-        """
-        session = query.pop('session', None)
-        aggregation = query.pop('aggregation', None)
-        group_by = query.pop('group_by', None)
-        if not aggregation and not group_by:
-            raise MotordanticValidationError('miss aggregation or group_by')
-        if isinstance(aggregation, Iterable):
-            aggregate_query = {}
-            for agg in aggregation:
-                aggregate_query.update(agg._aggregate_query(self.mongo_model_class))
-        elif aggregation is not None:
-            aggregate_query = aggregation._aggregate_query(self.mongo_model_class)
-        else:
-            aggregate_query = {}
-        if group_by:
-            group_by = group_by_aggregate_generation(group_by)
-            aggregate_query.pop('_id', None)
-            group_params = {"$group": {"_id": group_by, **aggregate_query}}
-        else:
-            group_params = {
-                "$group": {"_id": None, **aggregate_query}
-                if '_id' not in aggregate_query
-                else aggregate_query
-            }
-        data = [
-            {
-                "$match": self.mongo_model_class._validate_query_data(query)
-                if not args
-                else self.mongo_model_class._check_query_args(*args)
-            },
-            group_params,
-        ]
-
-        async_result = await self._motor_aggreggate_call(data, session)
-        result = [row async for row in async_result]
-        if not result:
-            return SimpleAggregateResult(self.mongo_model_class, {})
-        result_data = {}
-        for r in result:
-            name = generate_name_field(r.pop('_id'))
-            result_data.update({name: r} if name else r)
-        return SimpleAggregateResult(self.mongo_model_class, result_data)
-
-    async def simple_aggregate(self, *args, **kwargs) -> SimpleAggregateResult:
-        return await self._aggregate(*args, **kwargs)
-
-    def aggregate(self) -> Aggregate:
-        aggregate = Aggregate(self.mongo_model_class)
-        return aggregate
-
-    async def aggregate_sum(self, agg_field: str, **query) -> Union[int, float]:
-        result = await self._aggregate(aggregation=Sum(agg_field), **query)
-        return result.data.get(f'{agg_field}__sum', 0)
-
-    async def aggregate_max(self, agg_field: str, **query) -> Union[int, float]:
-        result = await self._aggregate(aggregation=Max(agg_field), **query)
-        return result.data.get(f'{agg_field}__max', 0)
-
-    async def aggregate_min(self, agg_field: str, **query) -> Union[int, float]:
-        result = await self._aggregate(aggregation=Min(agg_field), **query)
-        return result.data.get(f'{agg_field}__min', 0)
-
-    async def aggregate_avg(self, agg_field: str, **query) -> Union[int, float]:
-        result = await self._aggregate(aggregation=Avg(agg_field), **query)
-        return result.data.get(f'{agg_field}__avg', 0)
-
-    async def _bulk_operation(
-        self,
-        models: List,
-        updated_fields: Optional[List] = None,
-        query_fields: Optional[List] = None,
-        batch_size: Optional[int] = 10000,
-        upsert: bool = False,
-        session: Optional[ClientSession] = None,
-    ) -> None:
-        """base bulk operation method
-
-        Args:
-            models (List): MongoModels objects
-            updated_fields (Optional[List], optional): list of updated fields. Defaults to None.
-            query_fields (Optional[List], optional): list of query fields. Defaults to None.
-            batch_size (Optional[int], optional): query batch. Defaults to 10000.
-            upsert (bool, optional): for upsert pymongo queries. Defaults to False.
-            session (Optional[ClientSession], optional): motor session. Defaults to None.
-        """
-        if batch_size is not None and batch_size > 0:
-            for requests in chunk_by_length(models, batch_size):
-                data = bulk_query_generator(
-                    requests,
-                    updated_fields=updated_fields,
-                    query_fields=query_fields,
-                    upsert=upsert,
-                )
-                await self._make_query('bulk_write', data, session=session)
-            return None
-        data = bulk_query_generator(
-            models,
-            updated_fields=updated_fields,
-            query_fields=query_fields,
-            upsert=upsert,
-        )
-        await self._make_query('bulk_write', data, session=session)
-
-    async def bulk_update(
-        self,
-        models: List,
-        updated_fields: List,
-        batch_size: Optional[int] = None,
-        session: Optional[ClientSession] = None,
-    ) -> None:
-        """bulk update method
-
-        Args:
-            models (List): MongoModel objects
-            updated_fields (List): list of updated fields, like ['name', 'last_name']
-            batch_size (Optional[int], optional): query batch. Defaults to None.
-            session (Optional[ClientSession], optional): motor session. Defaults to None.
-
-        Raises:
-            MongoValidationError: if invalid param
-        """
-        if not updated_fields:
-            raise MotordanticValidationError('updated_fields cannot be empty')
-        await self._bulk_operation(
-            models,
-            updated_fields=updated_fields,
-            batch_size=batch_size
-            if batch_size is not None and batch_size > 0
-            else 10000,
-            session=session,
-        )
-
-    async def bulk_create(
-        self,
-        models: List,
-        batch_size: Optional[int] = 30000,
-        session: Optional[ClientSession] = None,
-    ) -> int:
-        """bulk create method
-
-        Args:
-            models (List): MongoModels obejcts
-            batch_size (Optional[int], optional): query batch. Defaults to None.
-            session (Optional[ClientSession], optional): motor session. Defaults to None.
-
-        Returns:
-            int: count of objects created
-        """
-        if batch_size is None or batch_size <= 0:
-            batch_size = 30000
-        result = 0
-        for data in chunk_by_length(models, batch_size):
-            inserted_count = await self.insert_many(data, session=session)
-            result += inserted_count
-        return result
-
-    async def bulk_update_or_create(
-        self,
-        models: List,
-        query_fields: List,
-        batch_size: Optional[int] = 10000,
-        session: Optional[ClientSession] = None,
-    ) -> None:
-        """Method for update/create rows
-
-        Args:
-            models (List): List of MongoModels objects
-            query_fields (List): list of query fields like ['name'], perfect if this fields in indexes
-            batch_size (Optional[int], optional): query obejcts batch. Defaults to 10000.
-            session (Optional[ClientSession], optional): motor session. Defaults to None.
-
-        Raises:
-            MongoValidationError: if invalid models
-
-        """
-        if not query_fields:
-            raise MotordanticValidationError('query_fields cannot be empty')
-        return await self._bulk_operation(
-            models,
-            query_fields=query_fields,
-            batch_size=batch_size,
-            upsert=True,
-            session=session,
-        )
-
     async def _find_with_replacement_or_with_update(
         self,
         operation: str,
         projection_fields: Optional[list] = None,
         sort_fields: Optional[Union[Tuple, List]] = None,
         sort: Optional[int] = None,
         upsert: bool = False,
         session: Optional[ClientSession] = None,
         **query,
-    ) -> Union[Dict, 'MongoModel', None]:
+    ) -> Union[Dict, 'Document', None]:
         """base method for find_with_<operation>
 
         Args:
             operation (str): operation name
             projection_fields (Optional[list], optional): prejection. Defaults to None.
             sort_fields (Optional[Union[Tuple, List]], optional): sort fields. Defaults to None.
             sort (Optional[int], optional): -1 or 1. Defaults to None.
             upsert (bool, optional): True/False. Defaults to False.
             session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
-            Union[Dict, 'MongoModel']: MongoModel or Dict
+            Union[Dict, 'Document']: Document or Dict or None
         """
         filter_, set_values = self._prepare_update_data(**query)
         return_document = ReturnDocument.AFTER
         replacement = query.pop('replacement', None)
 
         projection = {f: True for f in projection_fields} if projection_fields else None
         extra_params = {
@@ -912,38 +505,38 @@
             operation, filter_, set_values={'$set': set_values}, **extra_params
         )
         if projection:
             return {
                 field: value for field, value in data.items() if field in projection
             }
         if data:
-            return self.mongo_model_class.parse_obj(data)
+            return self.odm_manager.document.from_bson(data)
         return None
 
     async def find_one_and_update(
         self,
         projection_fields: Optional[list] = None,
         sort_fields: Optional[Union[Tuple, List]] = None,
         sort: Optional[int] = None,
         upsert: bool = False,
         session: Optional[ClientSession] = None,
         **query,
-    ) -> Union[Dict, 'MongoModel', None]:
+    ) -> Union[Dict, 'Document', None]:
         """find one and update
 
         Args:
             operation (str): operation name
             projection_fields (Optional[list], optional): prejection. Defaults to None.
             sort_fields (Optional[Union[Tuple, List]], optional): sort fields. Defaults to None.
             sort (Optional[int], optional): -1 or 1. Defaults to None.
             upsert (bool, optional): True/False. Defaults to False.
             session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
-            Union[Dict, 'MongoModel']: MongoModel or Dict
+            Union[Dict, 'Document']: Document or Dict or None
         """
         return await self._find_with_replacement_or_with_update(
             'find_one_and_update',
             projection_fields=projection_fields,
             sort_fields=[(field, sort or 1) for field in sort_fields]
             if sort_fields
             else None,
@@ -958,27 +551,27 @@
         replacement: Union[dict, Any],
         projection_fields: Optional[list] = None,
         sort_fields: Optional[Union[Tuple, List]] = None,
         sort: Optional[int] = None,
         upsert: bool = False,
         session: Optional[ClientSession] = None,
         **query,
-    ) -> Union[Dict, 'MongoModel', None]:
+    ) -> Union[Dict, 'Document', None]:
         """find one and replace
 
         Args:
             operation (str): operation name
             projection_fields (Optional[list], optional): prejection. Defaults to None.
             sort_fields (Optional[Union[Tuple, List]], optional): sort fields. Defaults to None.
             sort (Optional[int], optional): -1 or 1. Defaults to None.
             upsert (bool, optional): True/False. Defaults to False.
             session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
-            Union[Dict, 'MongoModel']: MongoModel or Dict
+            Union[Dict, 'Document']: Document or Dict or None
         """
         if not isinstance(replacement, dict):
             replacement = replacement.query_data
         return await self._find_with_replacement_or_with_update(
             'find_and_replace',
             projection_fields=projection_fields,
             sort_fields=[(field, sort) for field in sort_fields]
@@ -987,396 +580,219 @@
             sort=sort,
             upsert=upsert,
             session=session,
             replacement=replacement,
             **query,
         )
 
-    async def drop_collection(self, force: bool = False) -> bool:
-        """drop collection
+    async def _motor_aggreggate_call(
+        self, data: list, session: Optional[ClientSession]
+    ) -> AsyncIterable:
+        async def context():
+            aggregate_cursor = getattr(self.odm_manager.collection, 'aggregate')
+
+            async for row in aggregate_cursor(data, session=session):
+                yield row
+
+        return context()
+
+    def from_bson(self, row: RawBSONDocument) -> dict:
+        return bson_decode(row.raw)
+
+    async def raw_aggregate(
+        self, data: List[Dict[Any, Any]], session: Optional[ClientSession] = None
+    ) -> list:
+        """raw aggregation query
 
         Args:
-            force (bool, optional): if u wanna force drop. Defaults to False.
+            data (List[Dict[Any, Any]]): aggregation query
+            session (Optional[ClientSession], optional): motor session. Defaults to None.
 
         Returns:
-            bool: result message
+            list: aggregation result
         """
-        if force:
-            await self._make_query('drop', query_params={})
-            return True
-        value = input(
-            f'Are u sure for drop this collection - {self.mongo_model_class.__name__.lower()} (y, n)'  # type: ignore
-        )
-        if value.lower() == 'y':
-            await self._make_query('drop', query_params={})
-            return True
-        return False
-
-
-class SyncQueryBuilder(QueryBuilder):
-    def __init__(self, mongo_model_class: 'MongoModel'):
-        super().__init__(mongo_model_class)
-        try:
-            self._io_loop = (
-                self.motor_client.io_loop
-                if self.motor_client.io_loop is not None
-                else asyncio.get_running_loop()
-            )
-        except RuntimeError:
-            self._io_loop = asyncio.new_event_loop()
-            # asyncio.set_event_loop(self._io_loop)
-
-    @property
-    def sync(self):
-        raise AttributeError('cant call call in sync builder.')
-
-    @no_type_check
-    def insert_one(self, session: Optional[ClientSession] = None, **query) -> ObjectId:
-        return self._io_loop.run_until_complete(super().insert_one(session, **query))
-
-    @no_type_check
-    def insert_many(self, data: List, session: Optional[ClientSession] = None) -> int:
-        return self._io_loop.run_until_complete(super().insert_many(data, session))
+        result = await self._motor_aggreggate_call(data, session)
+        return [self.from_bson(row) async for row in result]
 
-    @no_type_check
-    def find_one(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        sort_fields: Optional[Union[Tuple, List]] = None,
-        session: Optional[ClientSession] = None,
-        sort: Optional[int] = None,
-        with_relations_objects: bool = False,
-        **query,
-    ) -> Optional['MongoModel']:
-        return self._io_loop.run_until_complete(
-            super().find_one(
-                logical_query,
-                sort_fields,
-                session,
-                sort,
-                with_relations_objects,
-                **query,
-            )
-        )
+    async def _aggregate(self, *args, **query) -> SimpleAggregateResult:
+        """main aggregate method
 
-    @no_type_check
-    def find(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        skip_rows: Optional[int] = None,
-        limit_rows: Optional[int] = None,
-        session: Optional[ClientSession] = None,
-        sort_fields: Optional[Union[Tuple, List]] = None,
-        sort: Optional[int] = None,
-        with_relations_objects: bool = False,
-        **query,
-    ) -> FindResult:
-        return self._io_loop.run_until_complete(
-            super().find(
-                logical_query,
-                skip_rows,
-                limit_rows,
-                session,
-                sort_fields,
-                sort,
-                with_relations_objects,
-                **query,
-            )
-        )
+        Raises:
+            MongoValidationError: miss aggregation or group_by
 
-    @no_type_check
-    def delete_one(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        session: Optional[ClientSession] = None,
-        **query,
-    ) -> int:
-        return self._io_loop.run_until_complete(
-            super().delete_one(logical_query, session, **query)
-        )
+        Returns:
+            dict: aggregation result
+        """
+        session = query.pop('session', None)
+        aggregation = query.pop('aggregation', None)
+        group_by = query.pop('group_by', None)
+        if not aggregation and not group_by:
+            raise MotordanticIndexError('miss aggregation or group_by')
+        if isinstance(aggregation, Iterable):
+            aggregate_query = {}
+            for agg in aggregation:
+                aggregate_query.update(agg._aggregate_query(self.odm_manager.document))
+        elif aggregation is not None:
+            aggregate_query = aggregation._aggregate_query(self.odm_manager.document)
+        else:
+            aggregate_query = {}
+        if group_by:
+            group_by = group_by_aggregate_generation(group_by)
+            aggregate_query.pop('_id', None)
+            group_params = {"$group": {"_id": group_by, **aggregate_query}}
+        else:
+            group_params = {
+                "$group": {"_id": None, **aggregate_query}
+                if '_id' not in aggregate_query
+                else aggregate_query
+            }
+        data = [
+            {
+                "$match": self._validate_query_data(query)
+                if not args
+                else self._check_query_args(*args)
+            },
+            group_params,
+        ]
 
-    @no_type_check
-    def delete_many(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        session: Optional[ClientSession] = None,
-        **query,
-    ) -> int:
-        return self._io_loop.run_until_complete(
-            super().delete_many(logical_query, session, **query)
-        )
+        async_result = await self._motor_aggreggate_call(data, session)
+        result = [self.from_bson(row) async for row in async_result]
+        if not result:
+            return SimpleAggregateResult(self.odm_manager.document, {})
+        result_data = {}
+        for r in result:
+            name = generate_name_field(r.pop('_id'))
+            result_data.update({name: r} if name else r)
+        return SimpleAggregateResult(self.odm_manager.document, result_data)
 
-    @no_type_check
-    def update_many(
-        self, upsert: bool = False, session: Optional[ClientSession] = None, **query
-    ) -> int:
-        return self._io_loop.run_until_complete(
-            super().update_many(upsert, session, **query)
-        )
+    async def simple_aggregate(self, *args, **kwargs) -> SimpleAggregateResult:
+        return await self._aggregate(*args, **kwargs)
 
-    @no_type_check
-    def update_one(
-        self, upsert: bool = False, session: Optional[ClientSession] = None, **query
-    ) -> int:
-        return self._io_loop.run_until_complete(
-            super().update_one(upsert, session, **query)
-        )
+    async def aggregate_sum(self, agg_field: str, **query) -> Union[int, float]:
+        result_field = self.odm_manager.document.__mapping_query_fields__[agg_field]
+        result = await self._aggregate(aggregation=Sum(agg_field), **query)
+        return result.data.get(f'{result_field}__sum', 0)
 
-    @no_type_check
-    def count(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        session: Optional[ClientSession] = None,
-        **query,
-    ) -> int:
-        return self._io_loop.run_until_complete(
-            super().count(logical_query, session, **query)
-        )
+    async def aggregate_max(self, agg_field: str, **query) -> Union[int, float]:
+        result = await self._aggregate(aggregation=Max(agg_field), **query)
+        result_field = self.odm_manager.document.__mapping_query_fields__[agg_field]
+        return result.data.get(f'{result_field}__max', 0)
 
-    @no_type_check
-    def count_documents(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        session: Optional[ClientSession] = None,
-        **query,
-    ) -> int:
-        return self._io_loop.run_until_complete(
-            super().count_documents(logical_query, session, **query)
-        )
+    async def aggregate_min(self, agg_field: str, **query) -> Union[int, float]:
+        result = await self._aggregate(aggregation=Min(agg_field), **query)
+        result_field = self.odm_manager.document.__mapping_query_fields__[agg_field]
+        return result.data.get(f'{result_field}__min', 0)
 
-    @no_type_check
-    def distinct(
-        self, field: str, session: Optional[ClientSession] = None, **query
-    ) -> list:
-        return self._io_loop.run_until_complete(
-            super().distinct(field, session, **query)
-        )
+    async def aggregate_avg(self, agg_field: str, **query) -> Union[int, float]:
+        result = await self._aggregate(aggregation=Avg(agg_field), **query)
+        result_field = self.odm_manager.document.__mapping_query_fields__[agg_field]
+        return result.data.get(f'{result_field}__avg', 0)
 
-    @no_type_check
-    def raw_aggregate(
-        self, data: List[Dict[Any, Any]], session: Optional[ClientSession] = None
-    ) -> list:
-        return self._io_loop.run_until_complete(super().raw_aggregate(data, session))
+    def _validate_raw_query(
+        self, method_name: str, raw_query: Union[Dict, List[Dict], Tuple[Dict]]
+    ) -> tuple:
+        if (
+            'insert' in method_name
+            or 'replace' in method_name
+            or 'update' in method_name
+        ):
+            if isinstance(raw_query, list):
+                raw_query = list(map(self._validate_query_data, raw_query))
+            elif isinstance(raw_query, dict):
+                raw_query = self._validate_query_data(raw_query)
+            else:
+                params = [
+                    query[key] if '$' in key else query
+                    for query in raw_query
+                    for key in query.keys()
+                ]
+                map(self._validate_query_data, params)
+        parsed_query = raw_query if isinstance(raw_query, tuple) else (raw_query,)
+        return parsed_query
 
-    @no_type_check
-    def raw_query(
+    async def raw_query(
         self,
         method_name: str,
         raw_query: Union[Dict, List[Dict], Tuple[Dict]],
         session: Optional[ClientSession] = None,
     ) -> Any:
-        return self._io_loop.run_until_complete(
-            super().raw_query(method_name, raw_query, session)
-        )
-
-    @no_type_check
-    def replace_one(
-        self,
-        replacement: Dict,
-        upsert: bool = False,
-        session: Optional[ClientSession] = None,
-        **filter_query,
-    ) -> Any:
-        return self._io_loop.run_until_complete(
-            super().replace_one(replacement, upsert, session, **filter_query)
-        )
-
-    @no_type_check
-    def find_with_count(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        skip_rows: Optional[int] = None,
-        limit_rows: Optional[int] = None,
-        session: Optional[ClientSession] = None,
-        sort_fields: Optional[Union[Tuple, List]] = None,
-        sort: Optional[int] = None,
-        **query,
-    ) -> Tuple[int, FindResult]:
-        return self._io_loop.run_until_complete(
-            super().find_with_count(
-                logical_query,
-                skip_rows,
-                limit_rows,
-                session,
-                sort_fields,
-                sort,
-                **query,
-            )
-        )
-
-    @no_type_check
-    def simple_aggregate(self, *args, **kwargs) -> SimpleAggregateResult:
-        return self._io_loop.run_until_complete(
-            super().simple_aggregate(*args, **kwargs)
-        )
-
-    @no_type_check
-    def aggregate_sum(self, agg_field: str, **query) -> Union[int, float]:
-        return self._io_loop.run_until_complete(
-            super().aggregate_sum(agg_field, **query)
-        )
-
-    @no_type_check
-    def aggregate_min(self, agg_field: str, **query) -> Union[int, float]:
-        return self._io_loop.run_until_complete(
-            super().aggregate_min(agg_field, **query)
-        )
-
-    @no_type_check
-    def aggregate_max(self, agg_field: str, **query) -> Union[int, float]:
-        return self._io_loop.run_until_complete(
-            super().aggregate_max(agg_field, **query)
-        )
+        """pymongo raw query
 
-    @no_type_check
-    def aggregate_avg(self, agg_field: str, **query) -> Union[int, float]:
-        return self._io_loop.run_until_complete(
-            super().aggregate_avg(agg_field, **query)
-        )
+        Args:
+            method_name (str): pymongo method, like insert_one
+            raw_query (Union[Dict, List[Dict], Tuple[Dict]]): query data
+            session (Optional[ClientSession], optional): motor session. Defaults to None.
 
-    @no_type_check
-    def drop_collection(self, force: bool = False) -> bool:
-        return self._io_loop.run_until_complete(super().drop_collection(force))
+        Raises:
+            MongoValidationError: raise if invalid data
 
-    @no_type_check
-    def find_and_replace(
-        self,
-        replacement: Union[dict, Any],
-        projection_fields: Optional[list] = None,
-        sort_fields: Optional[Union[Tuple, List]] = None,
-        sort: Optional[int] = None,
-        upsert: bool = False,
-        session: Optional[ClientSession] = None,
-        **query,
-    ) -> Union[Dict, 'MongoModel', None]:
-        return self._io_loop.run_until_complete(
-            super().find_and_replace(
-                replacement,
-                projection_fields,
-                sort_fields,
-                sort,
-                upsert,
-                session,
-                **query,
-            )
-        )
+        Returns:
+            Any: pymongo query result
+        """
+        parsed_query = self._validate_raw_query(method_name, raw_query)
+        try:
+            query = getattr(self.odm_manager.collection, method_name)
+            return await query(*parsed_query, session=session)
+        except AttributeError:
+            raise MotordanticValidationError('invalid method name')
 
-    @no_type_check
-    def find_one_and_update(
-        self,
-        projection_fields: Optional[list] = None,
-        sort_fields: Optional[Union[Tuple, List]] = None,
-        sort: Optional[int] = None,
-        upsert: bool = False,
-        session: Optional[ClientSession] = None,
-        **query,
-    ) -> Union[Dict, 'MongoModel', None]:
-        return self._io_loop.run_until_complete(
-            super().find_one_and_update(
-                projection_fields, sort_fields, sort, upsert, session, **query
-            )
-        )
+    async def list_indexes(self, session: Optional[ClientSession] = None) -> dict:
+        """get indexes for this collection
 
-    @no_type_check
-    def bulk_update_or_create(
-        self,
-        models: List,
-        query_fields: List,
-        batch_size: Optional[int] = 10000,
-        session: Optional[ClientSession] = None,
-    ) -> None:
-        return self._io_loop.run_until_complete(
-            super().bulk_update_or_create(models, query_fields, batch_size, session)
-        )
+        Returns:
+            dict: indexes result
+        """
+        list_indexes_cursor = getattr(self.odm_manager.collection, 'list_indexes')
+        query = list_indexes_cursor(session=session)
+        index_list = await query.to_list(None)
+        return_data = {}
+        for index in index_list:
+            dict_index = dict(index)
+            data = {dict_index['name']: {'key': dict(dict_index['key'])}}
+            return_data.update(data)
+        return return_data
 
-    @no_type_check
-    def bulk_create(
+    async def create_indexes(
         self,
-        models: List,
-        batch_size: Optional[int] = 30000,
+        indexes: List[IndexModel],
         session: Optional[ClientSession] = None,
-    ) -> int:
-        return self._io_loop.run_until_complete(
-            super().bulk_create(models, batch_size, session)
-        )
-
-    @no_type_check
-    def get_or_create(self, **query) -> Tuple:
-        """like django orm get_or_create
-
-        Returns:
-            Tuple: MongoModel instance, True/False
-        """
-        defaults = query.pop('defaults', {})
-        with_relations_objects = query.pop('with_relations_objects', False)
-        obj = self.find_one(**query, with_relations_objects=with_relations_objects)
-        if obj:
-            created = False
-        else:
-            created = True
-            inserted_id = self.insert_one(**{**query, **defaults})
-            obj = self.find_one(
-                _id=inserted_id, with_relations_objects=with_relations_objects
+    ) -> List[str]:
+        create_indexes_cursor = getattr(self.odm_manager.collection, 'create_index')
+        result = []
+        for index in indexes:
+            index_value = list(index.document['key'].items())
+            res = await create_indexes_cursor(
+                index_value,
+                session=session,
+                background=True,
             )
-        return obj, created
+            result.append(res)
+        return result
 
-    @no_type_check
-    def update_or_create(self, **query) -> Tuple:
-        """like django orm update_or_create
-
-        Returns:
-            Tuple: MongoModel instance, True/False
-        """
-        defaults = query.pop('defaults', {})
-        with_relations_objects = query.pop('with_relations_objects', False)
-        obj = self.find_one(**query, with_relations_objects=with_relations_objects)
-        if obj is not None:
-            created = False
-            for field, value in defaults.items():
-                setattr(obj, field, value)
-        else:
-            created = True
-            obj = self.mongo_model_class(**{**query, **defaults})  # type: ignore
-        obj.save_sync()
-        if with_relations_objects:
-            obj = self.get(_id=obj._id, with_relations_objects=with_relations_objects)
-        return obj, created
+    async def drop_index(
+        self, index_name: str, session: Optional[ClientSession] = None
+    ) -> str:
+        indexes = await self.list_indexes(session)
+        if index_name in indexes:
+            await self._make_query('drop_index', index_name, session=session)
+            return f'{index_name} dropped.'
+        raise MotordanticIndexError(f'invalid index name - {index_name}')
 
-    @no_type_check
-    def get(
-        self,
-        logical_query: Union[Query, QueryCombination, None] = None,
-        session: Optional[ClientSession] = None,
-        sort_fields: Optional[Union[Tuple, List]] = None,
-        sort: Optional[int] = None,
-        with_relations_objects: bool = False,
-        **query,
-    ) -> Any:
-        """method like django orm get
+    async def drop_collection(self, force: bool = False) -> bool:
+        """drop collection
 
         Args:
-            logical_query (Union[Query, QueryCombination, None], optional): Query objects. Defaults to None.
-            session (Optional[ClientSession], optional): mongo session. Defaults to None.
-            sort_fields (Optional[Union[Tuple, List]], optional): sorts. Defaults to None.
-            sort (Optional[int], optional): sort. Defaults to None.
-
-        Raises:
-            DoesNotExist: raise if not found object
+            force (bool, optional): if u wanna force drop. Defaults to False.
 
         Returns:
-            Any: mongo model
+            bool: result message
         """
-
-        obj = self.find_one(
-            logical_query=logical_query,
-            session=session,
-            sort_fields=sort_fields,
-            sort=sort,
-            **query,
+        if force:
+            await self.odm_manager.collection.drop()  # type: ignore
+            return True
+        value = input(
+            f'Are u sure for drop this collection - {self.odm_manager.document.__name__.lower()} (y, n)'  # type: ignore
         )
-        if not obj:
-            raise DoesNotExist(self.mongo_model_class.__name__)  # type: ignore
-        if with_relations_objects and self.mongo_model_class.relation_manager:
-            obj = self._io_loop.run_until_complete(
-                self.mongo_model_class.relation_manager.map_relation_for_single(obj)
-            )
-        return obj
+        if value.lower() == 'y':
+            await self.odm_manager.collection.drop()  # type: ignore
+            return True
+        return False
```

### Comparing `motordantic-0.0.2a1/motordantic/relation.py` & `motordantic-0.1.0a1/motordantic/relation.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,116 +2,110 @@
 from typing import TYPE_CHECKING, List
 
 from .types import RelationTypes
 
 __all__ = ('RelationManager',)
 
 if TYPE_CHECKING:
-    from .models import MongoModel
-    from .typing import DictStrList, MongoModelType
+    from .document import Document
+    from .typing import DictStrList, DocumentType
 
 
 class RelationManager(object):
     """relation manager for get and set data from to to models instances"""
 
-    __slots__ = ('mongo_model_class', 'relation_fields')
+    __slots__ = ('document_class', 'relation_fields')
 
-    def __init__(self, mongo_model_class: 'MongoModelType'):
-        self.mongo_model_class = mongo_model_class
-        self.relation_fields = self._get_relation_fields(mongo_model_class)
+    def __init__(self, document_class: 'Document'):
+        self.document_class = document_class
+        self.relation_fields = self._get_relation_fields(document_class)
 
     @classmethod
-    def _get_relation_fields(cls, mongo_model_class: 'MongoModelType') -> dict:
-        return mongo_model_class.__db_refs__ or {}
+    def _get_relation_fields(cls, document_class: 'Document') -> dict:
+        return document_class.__db_refs__ or {}
 
-    def _relation_data_setter(
-        self, mongo_model: 'MongoModel', data: dict
-    ) -> 'MongoModel':
+    def _relation_data_setter(self, document: 'Document', data: dict) -> 'Document':
         """data setter
 
         Args:
-            mongo_model (MongoModel): mongo model insatance
+            document (Document): mongo model insatance
             data (dict): relations objects map
 
         Returns:
-            MongoModel: updated mongo model
+            Document: updated mongo model
         """
         for field, relation_info in self.relation_fields.items():
-            relation_attr = getattr(mongo_model, field)
+            relation_attr = getattr(document, field)
             if not relation_attr:
                 continue
             if relation_info.relation_type == RelationTypes.ARRAY:
                 relation_value = []
                 for rel in relation_attr:
                     v = data[field].get(str(rel.db_ref.id))
                     if v:
                         relation_value.append(v)
             else:
                 relation_value = data[field].get(str(relation_attr.db_ref.id))
-            setattr(mongo_model, field, relation_value)
-        return mongo_model
+            setattr(document, field, relation_value)
+        return document
 
     async def _get_relation_objects_by_model_class(
-        self, field: str, mongo_model_class: 'MongoModelType', ids: list
+        self, field: str, document_class: 'DocumentType', ids: list
     ) -> dict:
-        result = await mongo_model_class.Q.find(
-            _id__in=ids, with_relations_objects=True
-        )
+        result = await document_class.Q.find(_id__in=ids, with_relations_objects=True)
         return {field: {str(o._id): o for o in result}}
 
     async def get_relation_objects(self, pre_relation: 'DictStrList') -> dict:
         futures = []
         for field, ids in pre_relation.items():
-            mongo_model_class = self.relation_fields[field].mongo_model_class
+            document_class = self.relation_fields[field].document_class
             futures.append(
                 asyncio.ensure_future(
                     self._get_relation_objects_by_model_class(
-                        field, mongo_model_class, ids
+                        field, document_class, ids
                     )
                 )
             )
 
         relation_objects = {}
         for _, field_relation_result in enumerate(
             asyncio.as_completed(futures), start=1
         ):
             relation_objects.update(await field_relation_result)
         return relation_objects
 
-    def _get_pre_relation(
-        self, mongo_model_instances: List['MongoModel']
-    ) -> 'DictStrList':
+    def _get_pre_relation(self, document_instances: List['Document']) -> 'DictStrList':
         pre_relation: 'DictStrList' = {field: [] for field in self.relation_fields}
-        for mongo_model_instance in mongo_model_instances:
+        for document_instance in document_instances:
             for field in self.relation_fields:
-                attr = getattr(mongo_model_instance, field)
+                attr = getattr(document_instance, field)
                 if isinstance(attr, list):
                     ids = tuple(row.db_ref.id for row in attr)
                 else:
                     ids = (attr.db_ref.id,) if attr else tuple()
                 if ids:
                     pre_relation[field].extend(ids)
         return {f: list(set(items)) for f, items in pre_relation.items()}
 
     async def map_relation_for_single(
-        self, mongo_model_instance: 'MongoModel'
-    ) -> 'MongoModel':
+        self, document_instance: 'Document'
+    ) -> 'Document':
         """map relation data to mongo model instanc
 
         Args:
-            mongo_model_instances (List[MongoModel]): list of instances from MongoModel
+            document_instances (List[Document]): list of instances from Document
 
         Returns:
-            MongoModel: mapped mongo model
+            Document: mapped mongo model
         """
-        pre_relation: 'DictStrList' = self._get_pre_relation([mongo_model_instance])
+        pre_relation: 'DictStrList' = self._get_pre_relation([document_instance])
         relation_objects = await self.get_relation_objects(pre_relation)
-        return self._relation_data_setter(mongo_model_instance, relation_objects)
+        return self._relation_data_setter(document_instance, relation_objects)
 
-    async def map_relation_for_array(self, result: List) -> List['MongoModel']:
+    async def map_relation_for_array(self, result: List) -> List['Document']:
         """map relations data for _find method list result
 
         Args:
             result (List): _find query result converted to list
 
         Returns:
             List: mapped list
```

### Comparing `motordantic-0.0.2a1/motordantic/schema.py` & `motordantic-0.1.0a1/motordantic/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,21 @@
     get_model,
     get_flat_models_from_model,
     get_model_name_map,
     get_schema_ref,
 )
 
 if TYPE_CHECKING:
-    from .models import MongoModel
+    from .document import Document
+
+__all__ = ('model_type_schema', 'model_process_schema', 'model_schema')
 
 
 def model_type_schema(
-    model: Type['MongoModel'],
+    model: Type['Document'],
     *,
     by_alias: bool,
     model_name_map: Dict[TypeModelOrEnum, str],
     ref_template: str,
     ref_prefix: Optional[str] = None,
     known_models: TypeModelSet,
 ) -> Tuple[Dict[str, Any], Dict[str, Any], Set[str]]:
@@ -113,15 +115,15 @@
     from inspect import getdoc, signature
 
     known_models = known_models or set()
     if lenient_issubclass(model, Enum):
         model = cast(Type[Enum], model)
         s = enum_process_schema(model, field=field)
         return s, {}, set()
-    model = cast(Type['MongoModel'], model)
+    model = cast(Type['Document'], model)
     s = {'title': model.__config__.title or model.__name__}
     doc = getdoc(model)
     if doc:
         s['description'] = doc
     known_models.add(model)
     m_schema, m_definitions, nested_models = model_type_schema(
         model,
@@ -140,15 +142,15 @@
             schema_extra(s, model)
     else:
         s.update(schema_extra)
     return s, m_definitions, nested_models
 
 
 def model_schema(
-    model: Type['MongoModel'],
+    model: Type['Document'],
     by_alias: bool = True,
     ref_prefix: Optional[str] = None,
     ref_template: str = default_ref_template,
 ) -> Dict[str, Any]:
     """
     Generate a JSON Schema for one model. With all the sub-models defined in the ``definitions`` top-level
     JSON key.
```

### Comparing `motordantic-0.0.2a1/motordantic/sync.py` & `motordantic-0.1.0a1/motordantic/sync/sync.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,7 +18,17 @@
                 loop = asyncio.get_running_loop()
             except RuntimeError:
                 loop = asyncio.new_event_loop()
             return loop.run_until_complete(res)
         return res
 
     return wrapper
+
+
+def add_sync_version(func):
+    # assert asyncio.iscoroutine(func)
+
+    def wrapper(*args, **kwds):
+        return asyncio.new_event_loop().run_until_complete(func, *args, **kwds)
+
+    func.sync = wrapper
+    return func
```

### Comparing `motordantic-0.0.2a1/motordantic/typing.py` & `motordantic-0.1.0a1/motordantic/typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,32 +7,34 @@
     Mapping,
     Set,
     Type,
     Union,
 )
 
 __all__ = (
-    'MongoModelType',
+    'DocumentType',
     'DictStrList',
     'DictStrAny',
     'DictAny',
     'SetStr',
     'ListStr',
     'IntStr',
     'AbstractSetIntStr',
     'DictIntStrAny',
+    'ExcludeInclude',
+    'MappingIntStrAny',
 )
 
 if TYPE_CHECKING:
-    from .models import MongoModel
+    from .document import Document
 
 IntStr = Union[int, str]
 DictIntStrAny = Dict[IntStr, Any]
 MappingIntStrAny = Mapping[IntStr, Any]
-MongoModelType = Type['MongoModel']
+DocumentType = Type['Document']
 DictStrList = Dict[str, List]
 DictStrAny = Dict[str, Any]
 DictAny = Dict[Any, Any]
 SetStr = Set[str]
 ListStr = List[str]
 AbstractSetIntStr = AbstractSet[IntStr]
 ExcludeInclude = Union[AbstractSetIntStr, MappingIntStrAny, Any]
```

### Comparing `motordantic-0.0.2a1/motordantic/validaton.py` & `motordantic-0.1.0a1/motordantic/validation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,86 @@
 from typing import Any, Union, Optional, Tuple, TYPE_CHECKING
 
-from pydantic import BaseModel
+from bson import ObjectId
+from bson.errors import InvalidId
+from pydantic import BaseModel, ValidationError
+from pydantic.error_wrappers import ErrorWrapper
 
-from .types import ObjectIdStr
+from .types import ObjectIdStr, UUID
 from .exceptions import MotordanticValidationError
 
 
 __all__ = ('validate_field_value', 'sort_validation')
 
 if TYPE_CHECKING:
-    from .models import MongoModel
-    from .typing import MongoModelType
+    from .document import Document
+    from .typing import DocumentType
 
 
 def validate_field_value(
-    model: Union['MongoModel', 'MongoModelType'], field_name: str, value: Any
+    document: Union['Document', 'DocumentType'], field_name: str, value: Any
 ) -> Any:
     """extra helper value validation
 
     Args:
-        cls ('MongoModel'): mongo model class
+        cls ('Document'): mongo document class
         field_name (str): name of field
         value (Any): value
 
     Raises:
         AttributeError: if not field in __fields__
         MongoValidationError: if invalid value type
 
     Returns:
         Any: value
     """
     if field_name == '_id':
         field = ObjectIdStr()  # type: ignore
     else:
-        field = model.__fields__.get(field_name)  # type: ignore
+        field = document.__fields__.get(field_name)  # type: ignore
     error_ = None
     if isinstance(field, ObjectIdStr):
         try:
             value = field.validate(value)
         except ValueError as e:
-            error_ = e
+            error_ = ErrorWrapper(e, str(e))
     elif not field:
         raise AttributeError(f'invalid field - {field_name}')
     else:
-        value, error_ = field.validate(value, {}, loc=field.alias, cls=model)  # type: ignore
+        value, error_ = field.validate(value, {}, loc=field.alias, cls=document)  # type: ignore
     if error_:
-        raise MotordanticValidationError([error_], type(value))
-    if field_name in model.__db_refs__:  # type: ignore
+        pydantic_validation_error = ValidationError([error_], document)  # type: ignore
+        raise MotordanticValidationError(
+            pydantic_validation_error.errors(), pydantic_validation_error
+        )
+    if field_name in document.__db_refs__:  # type: ignore
         if isinstance(value, list):
             s = [v.to_ref() for v in value]
             return s
         return value.to_ref() if value else None
+    elif isinstance(value, UUID):
+        return value.hex
     else:
         return value.dict() if isinstance(value, BaseModel) else value
 
 
 def sort_validation(
     sort: Optional[int] = None, sort_fields: Union[list, tuple, None] = None
 ) -> Tuple[Any, ...]:
     if sort is not None:
         if sort not in (1, -1):
             raise ValueError(f'invalid sort value must be 1 or -1 not {sort}')
         if not sort_fields:
             sort_fields = ('_id',)
     return sort, sort_fields
+
+
+def validate_object_id(document: 'Document', value: str) -> ObjectId:
+    try:
+        o_id = ObjectId(value)
+    except InvalidId as e:
+        error_ = ErrorWrapper(e, str(e))
+        pydantic_validation_error = ValidationError([error_], document)  # type: ignore
+        raise MotordanticValidationError(
+            pydantic_validation_error.errors(), pydantic_validation_error
+        )
+    return o_id
```

### Comparing `motordantic-0.0.2a1/motordantic.egg-info/PKG-INFO` & `motordantic-0.1.0a1/motordantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motordantic
-Version: 0.0.2a1
+Version: 0.1.0a1
 Summary: Mongo ODM, based on motor+pydantic
 Home-page: https://github.com/bogdanjz/motordantic
 Author: bogdanjz
 Author-email: bzdv.dn@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -153,24 +153,24 @@
 class Stats(MongoModel):
     id: int
     cost: float
     clicks: int
     shows: int
     date: str
 
-from motordantic.aggregation import Sum, Min, Max
+from motordantic.aggregate import Sum, Min, Max
 
 summ_cost = await Stats.Q.simple_aggregate(date='2020-01-20', aggregation=Sum('cost'))
 min_clicks = await Stats.Q.simple_aggregate(date='2020-01-20', aggregation=Min('clicks'))
 min_shows = await Stats.Q.simple_aggregate(date='2020-01-20', aggregation=Max('shows'))
 
 # logical
-from motordantic.query import Query
-data = Banner.Q.find_one(Query(name='test') | Query(name__regex='testerino'))
+from motordantic.query import Q
+data = Banner.Q.find_one(Q(name='test') | Q(name__regex='testerino'))
 ```
 
 ### sync queries
 
 ```python
-sync_result = Banner.Q.sync.find_one()
+sync_result = Banner.Qsync.find_one()
 
 ```
```

### Comparing `motordantic-0.0.2a1/motordantic.egg-info/SOURCES.txt` & `motordantic-0.1.0a1/motordantic.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 LICENCE
 README.md
 setup.py
 motordantic/__init__.py
-motordantic/aggregate.py
-motordantic/aggregate_expressions.py
 motordantic/connection.py
+motordantic/document.py
 motordantic/exceptions.py
-motordantic/extra.py
 motordantic/fields.py
+motordantic/manager.py
 motordantic/models.py
 motordantic/property.py
-motordantic/query.py
-motordantic/querybuilder.py
 motordantic/relation.py
 motordantic/schema.py
 motordantic/session.py
 motordantic/singleton.py
-motordantic/sync.py
 motordantic/types.py
 motordantic/typing.py
-motordantic/validaton.py
+motordantic/validation.py
 motordantic.egg-info/PKG-INFO
 motordantic.egg-info/SOURCES.txt
 motordantic.egg-info/dependency_links.txt
 motordantic.egg-info/requires.txt
 motordantic.egg-info/top_level.txt
+motordantic/aggregate/__init__.py
+motordantic/aggregate/aggregate.py
+motordantic/aggregate/expressions.py
+motordantic/query/__init__.py
+motordantic/query/builder.py
+motordantic/query/extra.py
+motordantic/query/query.py
+motordantic/query/result.py
+motordantic/sync/__init__.py
+motordantic/sync/query.py
+motordantic/sync/sync.py
 tests/test_connection.py
-tests/test_create_model.py
+tests/test_create_document.py
 tests/test_extraquerymapper.py
+tests/test_fields.py
 tests/test_force_sync.py
 tests/test_relation.py
 tests/test_sync.py
 tests/queries/__init__.py
+tests/queries/test_Q.py
 tests/queries/test_aggregation.py
 tests/queries/test_basic_queries.py
 tests/queries/test_indexes.py
-tests/queries/test_inner_qyeries.py
-tests/queries/test_query.py
-tests/queries/test_raw_queries.py
+tests/queries/test_inner_queries.py
+tests/queries/test_raw_queries.py
+tests/queries/test_uuid_field.py
+tests/queries/test_validation.py
+tests/queries/test_write_concern.py
```

### Comparing `motordantic-0.0.2a1/setup.py` & `motordantic-0.1.0a1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(f):
     return open(f, "r").read()
 
 
 setup(
     name="motordantic",
-    version='0.0.2a1',
+    version='0.1.0a1',
     packages=find_packages(exclude=("tests", "docs", "examples")),
     install_requires=[
         "pydantic>=1.9,<2",
         "pymongo==4.1",
         "motor==3.0.0",
     ],
     description="Mongo ODM, based on motor+pydantic",
```

### Comparing `motordantic-0.0.2a1/tests/queries/test_aggregation.py` & `motordantic-0.1.0a1/tests/queries/test_aggregation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import pytest_asyncio
 import pytest
 
-from motordantic.models import MongoModel
+from motordantic.document import Document
 from motordantic.types import ObjectIdStr
-from motordantic.query import Query
-from motordantic.aggregate_expressions import Sum, Max, Min, Avg, Count
+from motordantic.query.query import Q
+from motordantic.aggregate.expressions import (
+    Sum,
+    Max,
+    Min,
+    Avg,
+    Count,
+)
 from motordantic.exceptions import MotordanticValidationError
 
 
-class Product(MongoModel):
+class Product(Document):
     title: str
     cost: float
     quantity: int
     product_type: str
     config: dict
 
 
-class ProductImage(MongoModel):
+class ProductImage(Document):
     url: str
     product_id: ObjectIdStr
 
 
 @pytest_asyncio.fixture(scope='session', autouse=True)
 async def innert_producs(event_loop):
     from random import randint
@@ -146,24 +152,24 @@
 
     result_agg = await Product.Q.simple_aggregate(
         aggregation=[Avg('cost'), Max('quantity')]
     )
     assert result_agg.data == {'cost__avg': 2.5, 'quantity__max': 4}
 
     result_not_match_agg = await Product.Q.simple_aggregate(
-        Query(title__ne='not_match') & Query(title__startswith='not'),
+        Q(title__ne='not_match') & Q(title__startswith='not'),
         aggregation=[Avg('cost'), Max('quantity')],
     )
     assert result_not_match_agg.data == {}
 
 
 @pytest.mark.asyncio
 async def test_aggregate_method(connection):
     aggregate = (
-        Product.Q.aggregate()
+        Product.manager.aggregate()
         .match(title__in=['1', '2', '3'])
         .group(_id={"quant": '$quantity'})
         .skip(1)
         .limit(1)
     )
     match_pipeline = [
         {'$match': {'title': {'$in': ['1', '2', '3']}}},
@@ -172,15 +178,15 @@
         {'$limit': 1},
     ]
     assert aggregate.pipeline == match_pipeline
     result = await aggregate.result()
     assert result == [{'_id': {'quant': 2}}]
 
     image_aggreagate = (
-        ProductImage.Q.aggregate()
+        ProductImage.manager.aggregate()
         .lookup(
             Product,
             local_field='product_id',
             foreign_field='_id',
             as_='product',
         )
         .unwind("$product")
@@ -211,15 +217,15 @@
         and 'product_image_url' in result[0]
     )
 
 
 @pytest.mark.asyncio
 async def test_logical_match_query_in_aggregate(connection):
     aggregate = (
-        Product.Q.aggregate().match(Query(title=1) | Query(title=4)).sort(title=-1)
+        Product.manager.aggregate().match(Q(title=1) | Q(title=4)).sort(title=-1)
     )
     assert aggregate.pipeline == [
         {'$match': {'$or': [{'title': '1'}, {'title': '4'}]}},
         {'$sort': {'title': -1}},
     ]
     result = await aggregate.result()
 
@@ -227,15 +233,15 @@
     assert result[-1]['title'] == '1'
 
 
 @pytest.mark.asyncio
 async def test_geo(connection):
     from pymongo import IndexModel
 
-    class Place(MongoModel):
+    class Place(Document):
         name: str
         location: dict
         category: str
 
         class Config:
             indexes = [IndexModel([('location', '2dsphere')])]
 
@@ -257,15 +263,15 @@
             'location': {'type': "Point", 'coordinates': [-73.9375, 40.8303]},
             'category': "Stadiums",
         },
     ]
     await Place.Q.insert_many(data)
 
     geo_aggregate = (
-        Place.Q.aggregate()
+        Place.manager.aggregate()
         .geo_near(
             near={'type': 'Point', 'coordinates': [-73.99279, 40.719296]},
             distance_field='dist.calculated',
             max_distance=2,
             query={'category': 'Parks'},
             include_locs='dist.location',
             spherical=True,
```

### Comparing `motordantic-0.0.2a1/tests/queries/test_basic_queries.py` & `motordantic-0.1.0a1/tests/queries/test_basic_queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pytest
 import pytest_asyncio
 
 from bson import ObjectId
 
 from motor.motor_asyncio import AsyncIOMotorClientSession
-from motordantic.exceptions import DoesNotExist
-from motordantic.models import MongoModel
+from motordantic.exceptions import DoesNotExist, MotordanticValidationError
+from motordantic.document import Document
 from motordantic.fields import computed_field
 from motordantic.session import Session
 
 
-class Ticket(MongoModel):
+class Ticket(Document):
     name: str
     position: int
     config: dict
     sign: int = 1
     type_: str = 'ga'
     array: list = [1, 2]
 
@@ -22,15 +22,15 @@
         excluded_query_fields = ('sign', 'type')
 
     @computed_field
     def position_property(self) -> int:
         return self.position
 
 
-class Trash(MongoModel):
+class Trash(Document):
     name: str
     date: str
 
 
 @pytest_asyncio.fixture(scope='session', autouse=True)
 async def drop_ticket_collection(event_loop):
     yield
@@ -93,15 +93,15 @@
 
 
 @pytest.mark.asyncio
 async def test_find_one(connection):
     await test_insert_one(connection)
     data = await Ticket.Q.find_one(name='second')
     second = await Ticket.Q.find_one(_id=data._id)
-    assert isinstance(data, MongoModel)
+    assert isinstance(data, Document)
     assert data.name == 'second'  # type: ignore
     assert data.position == 2  # type: ignore
     assert second._id == data._id
     assert second.position_property == 2
     assert second.data['position_property'] == 2
 
 
@@ -112,15 +112,15 @@
 
 
 @pytest.mark.asyncio
 async def test_async_get(connection):
     # await .test_insert_one()
     data = await Ticket.Q.get(name='second')
     second = await Ticket.Q.get(_id=data._id)
-    assert isinstance(data, MongoModel)
+    assert isinstance(data, Document)
     assert data.name == 'second'  # type: ignore
     assert data.position == 2  # type: ignore
     assert second._id == data._id
     with pytest.raises(DoesNotExist):
         _ = await Ticket.Q.get(name='invalid_name')
 
 
@@ -201,29 +201,29 @@
     )
     assert isinstance(data_with_prejection, dict)
     assert data_with_prejection['position'] == 12
 
 
 @pytest.mark.asyncio
 async def test_session_start(connection):
-    session = await Ticket._start_session()
+    session = await Ticket.manager._start_session()
     assert isinstance(session, AsyncIOMotorClientSession)
     await session.end_session()  # type: ignore
 
 
 @pytest.mark.asyncio
 async def test_session_find(connection):
-    session = await Ticket._start_session()
+    session = await Ticket.manager._start_session()
     ticket = await Ticket.Q.find_one(session=session)
     assert ticket is not None
 
 
 @pytest.mark.asyncio
 async def test_session_context(connection):
-    async with Session(Ticket) as session:
+    async with Session(Ticket.manager) as session:
         ticket = await Ticket.Q.find_one(session=session)
         assert ticket is not None
         new_ticket_id = await Ticket.Q.insert_one(
             name='session ticket',
             position=100,
             config={'param1': 'session'},
             session=session,
```

### Comparing `motordantic-0.0.2a1/tests/queries/test_indexes.py` & `motordantic-0.1.0a1/tests/queries/test_indexes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 import pytest_asyncio
 from pymongo import IndexModel
 
-from motordantic.models import MongoModel
+from motordantic.document import Document
 from motordantic.exceptions import MotordanticIndexError
 
 
-class IndexTicket(MongoModel):
+class IndexTicket(Document):
     name: str
     position: int
     config: dict
 
     class Config:
         indexes = [
             IndexModel([('position', 1)]),
@@ -33,15 +33,15 @@
         'position_1': {'key': {'position': 1}},
         'name_1': {'key': {'name': 1}},
     }
 
 
 @pytest.mark.asyncio
 async def test_check_indexes_if_remove(connection):
-    class IndexTicket(MongoModel):
+    class IndexTicket(Document):
         name: str
         position: int
         config: dict
 
         class Config:
             indexes = [
                 IndexModel([('position', 1)]),
```

### Comparing `motordantic-0.0.2a1/tests/queries/test_inner_qyeries.py` & `motordantic-0.1.0a1/tests/queries/test_inner_queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest_asyncio
 import pytest
 
-from motordantic.models import MongoModel
+from motordantic.document import Document
 
 
-class InnerTicket(MongoModel):
+class InnerTicket(Document):
     name: str
     position: int
     config: dict
     params: dict
     sign: int = 1
     type_: str = 'ga'
     array: list = []
```

### Comparing `motordantic-0.0.2a1/tests/queries/test_query.py` & `motordantic-0.1.0a1/tests/queries/test_Q.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import pytest
 import pytest_asyncio
 
-from motordantic.models import MongoModel
-from motordantic.query import Query
+from motordantic.document import Document
+from motordantic.query.query import Q
 
 
-class TicketForQuery(MongoModel):
+class TicketForQuery(Document):
     name: str
     position: int
 
 
 @pytest_asyncio.fixture(scope='session', autouse=True)
 async def drop_ticket_collection(event_loop):
     yield
     await TicketForQuery.Q.drop_collection(force=True)
 
 
 def test_query_organization(connection):
-    query = (
-        Query(name=123) | Query(name__ne=124) & Query(position=1) | Query(position=2)
-    )
-    data = query.to_query(TicketForQuery)
+    query = Q(name=123) | Q(name__ne=124) & Q(position=1) | Q(position=2)
+    data = query.to_query(TicketForQuery.manager._builder)
     value = {
         '$or': [
             {'name': '123'},
             {'$and': [{'name': {'$ne': '124'}}, {'position': 1}]},
             {'position': 2},
         ]
     }
@@ -36,18 +34,18 @@
     query = [
         TicketForQuery(name='first', position=1),
         TicketForQuery(name='second', position=2),
     ]
     inserted = await TicketForQuery.Q.insert_many(query)
     assert inserted == 2
 
-    query = Query(name='first') | Query(position=1) & Query(name='second')
+    query = Q(name='first') | Q(position=1) & Q(name='second')
     data = await TicketForQuery.Q.find_one(query)
     assert data.name == 'first'
 
-    query = Query(position=3) | Query(position=1) & Query(name='second')
+    query = Q(position=3) | Q(position=1) & Q(name='second')
     data = await TicketForQuery.Q.find_one(query)
     assert data is None
 
-    query = Query(position=3) | Query(position=2) & Query(name='second')
+    query = Q(position=3) | Q(position=2) & Q(name='second')
     data = await TicketForQuery.Q.find_one(query)
     assert data.name == 'second'
```

### Comparing `motordantic-0.0.2a1/tests/queries/test_raw_queries.py` & `motordantic-0.1.0a1/tests/queries/test_raw_queries.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import uuid
 
 import pytest_asyncio
 import pytest
 
 from bson import ObjectId
 
-from motordantic.models import MongoModel
+from motordantic.document import Document
 from motordantic.exceptions import MotordanticValidationError
 
 
-class User(MongoModel):
+class User(Document):
     id: str
     name: str
     email: str
 
-    class Config:
-        excluded_query_fields = ('sign', 'type')
-
 
 @pytest_asyncio.fixture(scope='session', autouse=True)
 async def innert_users(event_loop):
     yield
     await User.Q.drop_collection(force=True)
```

### Comparing `motordantic-0.0.2a1/tests/test_connection.py` & `motordantic-0.1.0a1/tests/test_connection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 import os
 
 from motordantic.connection import (
     connect,
     MotordanticConnection,
-    DEFAULT_ENV_NAME,
-    _connections,
 )
 
 from motor.motor_asyncio import AsyncIOMotorClient
 
 
 class TestWriteConnectionParams:
     def setup(self):
-        connect("mongodb://127.0.0.1:27017", "test")
-        self.connection = _connections[DEFAULT_ENV_NAME]
-        assert isinstance(self.connection, MotordanticConnection)
+        connection = connect("mongodb://127.0.0.1:27017", "test")
+        self.connection: MotordanticConnection = connection
 
     def test_envirnament_values(self):
         database_name = os.getenv('MOTORDANTIC_DATABASE')
         assert database_name == 'test'
 
         address = os.getenv('MOTORDANTIC_ADDRESS')
         assert address == "mongodb://127.0.0.1:27017"
 
-        env_name = os.getenv('MOTORDANTIC_ENV_NAME')
-        assert env_name == DEFAULT_ENV_NAME
-
     def test_connection_params(self):
         database_name = self.connection.database_name
         conn_string = self.connection.address
         assert database_name == "test"
         assert conn_string == "mongodb://127.0.0.1:27017"
 
     def test_connection(self):
```

### Comparing `motordantic-0.0.2a1/tests/test_create_model.py` & `motordantic-0.1.0a1/tests/test_create_document.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import pytest
 import pytest_asyncio
 
-from motordantic.models import MongoModel
+from motordantic.document import Document
 from motordantic.fields import computed_field
+from motordantic.exceptions import MotordanticValidationError
 from pydantic import BaseModel
 
 
 class Config(BaseModel):
     path: str = '/home/'
     env: str = 'test'
 
 
-class Application(MongoModel):
+class Application(Document):
     name: str
     config: Config
     lang: str
 
     @computed_field
     def lang_upper(self) -> str:
         return self.lang.upper()
@@ -76,13 +77,13 @@
     assert data.name == 'test'
     data = await Application.Q.find_one(config__env='invalid')
     assert data is None
 
 
 @pytest.mark.asyncio
 async def test_raise_with_field_mongo_model(connection):
-    class Default(MongoModel):
+    class Default(Document):
         name: str
         app: Application
 
-    with pytest.raises(ValueError):
+    with pytest.raises(MotordanticValidationError):
         await Default(name='default', app=await Application.Q.find_one()).save()
```

### Comparing `motordantic-0.0.2a1/tests/test_extraquerymapper.py` & `motordantic-0.1.0a1/tests/test_extraquerymapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 import re
 
 from bson import Regex
 
-from motordantic.models import MongoModel
-from motordantic.extra import ExtraQueryMapper
+from motordantic.document import Document
+from motordantic.query.extra import ExtraQueryMapper
 
 
-class User(MongoModel):
+class User(Document):
     id: str
     name: str
     counter: int
     date: str
 
 
 def test_in_extra_param():
```

### Comparing `motordantic-0.0.2a1/tests/test_relation.py` & `motordantic-0.1.0a1/tests/test_relation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import List, Optional
 
 import pytest_asyncio
 import pytest
 
-from motordantic.models import MongoModel
+from motordantic.document import Document
 from motordantic.types import Relation
 
 
-class Author(MongoModel):
+class Author(Document):
     name: str
 
 
-class Book(MongoModel):
+class Book(Document):
     title: str
     author: Relation[Author]
 
 
-class Publish(MongoModel):
+class Publish(Document):
     name: str
     books: List[Relation[Book]]
 
 
-class OptionalTestPublisher(MongoModel):
+class OptionalTestPublisher(Document):
     name: str
     author: Optional[Relation[Author]] = None
 
 
 @pytest_asyncio.fixture(scope='session', autouse=True)
 async def relation_data(event_loop, connection):
     authors = [Author(name='Author1'), Author(name='Author2')]
@@ -61,27 +61,26 @@
     await OptionalTestPublisher.Q.drop_collection(force=True)
 
 
 @pytest.mark.asyncio
 async def test_book_relation(connection):
     book = await Book.Q.find_one(title='first book from author1')
     book_author = await book.author.get()
-    native_author = await Author.Q.get(name='Author1')
+    native_author = await Author.Q.find_one(name='Author1')
     assert book_author == native_author
 
     book = await Book.Q.find_one(
         title='first book from author1', with_relations_objects=True
     )
     # assert book_author == 1
     assert book.author == native_author
 
 
 @pytest.mark.asyncio
 async def test_publish_relation(connection):
-    print('connected - ', Publish.__connection__)
     publish = await Publish.Q.find_one(name='publush1', with_relations_objects=True)
 
     assert publish.data['books'][0]['title'] == 'first book from author2'
     book = await Book.Q.find_one(
         title='first book from author2', with_relations_objects=True
     )
     assert publish.books == [book]
```

### Comparing `motordantic-0.0.2a1/tests/test_sync.py` & `motordantic-0.1.0a1/tests/test_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest_asyncio
 
 from bson import ObjectId
 
-from motordantic.models import MongoModel
+from motordantic.document import Document
 from motordantic.session import SessionSync
 
 
-class TicketSync(MongoModel):
+class TicketSync(Document):
     name: str
     position: int
     config: dict
     sign: int = 1
     type_: str = 'ga'
     array: list = [1, 2]
 
@@ -22,56 +22,56 @@
 async def drop_ticket_sync_collection(event_loop):
     yield
     await TicketSync.Q.drop_collection(force=True)
 
 
 def test_sync_insert_one(connection):
     data = {'name': 'sync1', 'position': 2310, 'config': {'as_sync': True}}
-    object_id = TicketSync.Q.sync.insert_one(**data)
+    object_id = TicketSync.Qsync.insert_one(**data)
     assert isinstance(object_id, ObjectId)
 
 
 def test_sync_find_one(connection):
-    ticket = TicketSync.Q.sync.find_one(name='sync1')
+    ticket = TicketSync.Qsync.find_one(name='sync1')
     assert ticket.name == 'sync1'
     assert ticket.position == 2310
 
 
 def test_sync_insert_many(connection):
     data = [
         {'name': 'sync2', 'position': 2, 'config': {'as_sync': True}},
         {'name': 'sync3', 'position': 3, 'config': {'as_sync': True}},
         {'name': 'sync_fourth', 'position': 4, 'config': {'as_sync': False}},
     ]
-    inserted = TicketSync.Q.sync.insert_many(data)
+    inserted = TicketSync.Qsync.insert_many(data)
     assert inserted == 3
 
 
 def test_sync_aggregation(connection):
-    summ = TicketSync.Q.sync.aggregate_sum('position')
+    summ = TicketSync.Qsync.aggregate_sum('position')
     assert summ == 2319
 
-    max_ = TicketSync.Q.sync.aggregate_max('position')
+    max_ = TicketSync.Qsync.aggregate_max('position')
     assert max_ == 2310
 
-    min_ = TicketSync.Q.sync.aggregate_min('position')
+    min_ = TicketSync.Qsync.aggregate_min('position')
     assert min_ == 2
 
-    avg = TicketSync.Q.sync.aggregate_avg('position')
+    avg = TicketSync.Qsync.aggregate_avg('position')
     assert avg == 579.75
 
 
 def test_find_sync(connection):
-    data = TicketSync.Q.sync.find().list
+    data = TicketSync.Qsync.find().list
     assert len(data) == 4
     assert data[-1].name == 'sync_fourth'
 
 
 def test_sync_distinct(connection):
-    data = TicketSync.Q.sync.distinct('position', name='sync2')
+    data = TicketSync.Qsync.distinct('position', name='sync2')
     assert data == [2]
 
 
 def test_session_sync(connection):
-    with SessionSync(TicketSync) as session:
-        ticket = TicketSync.Q.sync.find_one(session=session)
+    with SessionSync(TicketSync.manager) as session:
+        ticket = TicketSync.Qsync.find_one(session=session)
         assert ticket is not None
```

