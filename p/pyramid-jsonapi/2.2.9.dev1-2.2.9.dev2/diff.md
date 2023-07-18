# Comparing `tmp/pyramid_jsonapi-2.2.9.dev1.tar.gz` & `tmp/pyramid_jsonapi-2.2.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyramid_jsonapi-2.2.9.dev1.tar", last modified: Wed Jun 28 14:41:01 2023, max compression
+gzip compressed data, was "pyramid_jsonapi-2.2.9.dev2.tar", last modified: Tue Jul 18 15:23:11 2023, max compression
```

## Comparing `pyramid_jsonapi-2.2.9.dev1.tar` & `pyramid_jsonapi-2.2.9.dev2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    34521 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/LICENSE
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1131 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/PKG-INFO
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3974 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/README.rst
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    24791 2023-06-28 14:32:06.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/__init__.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1471 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/authoriser.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3898 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/callbacks_doc.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    50085 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/collection_view.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3911 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/db_query.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    20994 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/endpoints.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3679 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/filters.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     7282 2023-06-28 14:32:26.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/http_query.py
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/JSONSchema/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    11280 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/JSONSchema/__init__.py
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/OpenAPI/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    10756 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/OpenAPI/__init__.py
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/OpenAPI/swagger-ui/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3771 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/OpenAPI/swagger-ui/index.mako
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     2633 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/__init__.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     6307 2022-03-25 12:58:00.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/permissions.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      401 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/resource.py
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/schema/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    11044 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/schema/jsonapi-schema.json
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     9550 2023-06-28 14:33:17.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/serialiser.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     4295 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/unit_tests.py
--rwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)     1634 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/version.py
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    43757 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/__init__.py
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     5161 2023-06-20 15:29:35.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/__init__.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3447 2023-06-21 21:04:27.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/collection_get.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     4646 2023-06-19 21:41:07.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/collection_post.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      735 2023-06-19 21:41:20.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/item_delete.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      818 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/item_get.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     5918 2023-02-28 11:42:33.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/item_patch.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     2748 2023-02-28 11:42:33.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/related_get.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1703 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/relationships_delete.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      218 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/relationships_get.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3163 2022-03-25 12:58:00.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/relationships_patch.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     2364 2022-04-06 11:18:05.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/relationships_post.py
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/selectin/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)       33 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/selectin/__init__.py
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     4023 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/selectin/collection_get.py
-drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-06-28 14:41:01.678712 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi.egg-info/
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1131 2023-06-28 14:41:01.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi.egg-info/PKG-INFO
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1505 2023-06-28 14:41:01.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi.egg-info/SOURCES.txt
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)        1 2023-06-28 14:41:01.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi.egg-info/dependency_links.txt
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      128 2023-06-28 14:41:01.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi.egg-info/requires.txt
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)       16 2023-06-28 14:41:01.000000 pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi.egg-info/top_level.txt
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)       79 2023-06-28 14:41:01.682712 pyramid_jsonapi-2.2.9.dev1/setup.cfg
--rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1831 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev1/setup.py
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.695595 pyramid_jsonapi-2.2.9.dev2/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    34521 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/LICENSE
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1131 2023-07-18 15:23:11.695595 pyramid_jsonapi-2.2.9.dev2/PKG-INFO
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3974 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/README.rst
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.687595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    24791 2023-06-28 14:32:06.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/__init__.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1471 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/authoriser.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3898 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/callbacks_doc.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    50085 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/collection_view.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3911 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/db_query.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    20994 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/endpoints.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3679 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/filters.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     7420 2023-07-18 15:15:51.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/http_query.py
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.691595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.691595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/JSONSchema/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    11280 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/JSONSchema/__init__.py
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.691595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/OpenAPI/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    10756 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/OpenAPI/__init__.py
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.691595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/OpenAPI/swagger-ui/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3771 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/OpenAPI/swagger-ui/index.mako
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     2633 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/__init__.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     6307 2022-03-25 12:58:00.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/permissions.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      401 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/resource.py
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.691595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/schema/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    11044 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/schema/jsonapi-schema.json
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     9549 2023-07-18 15:16:13.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/serialiser.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     4295 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/unit_tests.py
+-rwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)     1634 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/version.py
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.691595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)    43757 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/__init__.py
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.691595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     5161 2023-06-20 15:29:35.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/__init__.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3447 2023-06-21 21:04:27.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/collection_get.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     4646 2023-06-19 21:41:07.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/collection_post.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      735 2023-06-19 21:41:20.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/item_delete.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      818 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/item_get.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     5918 2023-02-28 11:42:33.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/item_patch.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     2748 2023-02-28 11:42:33.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/related_get.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1703 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/relationships_delete.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      218 2022-03-24 13:46:48.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/relationships_get.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     3163 2022-03-25 12:58:00.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/relationships_patch.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     2364 2022-04-06 11:18:05.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/relationships_post.py
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.695595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/selectin/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)       33 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/selectin/__init__.py
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     4023 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/selectin/collection_get.py
+drwxrwxr-x   0 chiggs1   (1001) chiggs1   (1001)        0 2023-07-18 15:23:11.691595 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi.egg-info/
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1131 2023-07-18 15:23:11.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi.egg-info/PKG-INFO
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1505 2023-07-18 15:23:11.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)        1 2023-07-18 15:23:11.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)      128 2023-07-18 15:23:11.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi.egg-info/requires.txt
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)       16 2023-07-18 15:23:11.000000 pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi.egg-info/top_level.txt
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)       79 2023-07-18 15:23:11.695595 pyramid_jsonapi-2.2.9.dev2/setup.cfg
+-rw-rw-r--   0 chiggs1   (1001) chiggs1   (1001)     1831 2023-06-28 14:28:19.000000 pyramid_jsonapi-2.2.9.dev2/setup.py
```

### Comparing `pyramid_jsonapi-2.2.9.dev1/LICENSE` & `pyramid_jsonapi-2.2.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/PKG-INFO` & `pyramid_jsonapi-2.2.9.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyramid_jsonapi
-Version: 2.2.9.dev1
+Version: 2.2.9.dev2
 Summary: Auto-build JSON API from sqlalchemy models using the pyramid framework
 Home-page: https://github.com/colinhiggs/pyramid-jsonapi
 Author: Colin Higgs
 Author-email: colin.higgs70@gmail.com
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Keywords: json,api,json-api,jsonapi,jsonschema,openapi,pyramid,sqlalchemy
 Platform: UNKNOWN
```

### Comparing `pyramid_jsonapi-2.2.9.dev1/README.rst` & `pyramid_jsonapi-2.2.9.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/__init__.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/authoriser.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/authoriser.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/callbacks_doc.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/callbacks_doc.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/collection_view.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/collection_view.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/db_query.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/db_query.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/endpoints.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/filters.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/filters.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/http_query.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/http_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,20 @@
     def __post_init__(self):
         if self.value.startswith('-'):
             self.ascending = False
             self.value = self.value[1:]
         else:
             self.ascending = True
 
+    def __str__(self) -> str:
+        if self.ascending:
+            return self.value
+        else:
+            return f'-{self.value}'
+
     @cached_property
     def colspec(self):
         return tuple(
             self.view_class.key_column.name if cname == 'id' else cname
             for cname in self.value.split('.')
         )
```

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/JSONSchema/__init__.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/JSONSchema/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/OpenAPI/__init__.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/OpenAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/OpenAPI/swagger-ui/index.mako` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/OpenAPI/swagger-ui/index.mako`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/metadata/__init__.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/permissions.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/permissions.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/schema/jsonapi-schema.json` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/schema/jsonapi-schema.json`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/serialiser.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/serialiser.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     def before_after_pagination_links(self, data):
         links = {}
         req = self.view.request
         route_name = req.matched_route.name
         qinfo = self.view.query_info
         _query = {'page[limit]': qinfo.paging_info.limit}
-        _query['sort'] = ','.join(qi.value for qi in qinfo.sorting_info)
+        _query['sort'] = ','.join(str(qi) for qi in qinfo.sorting_info)
         for filtr in qinfo.filter_info:
             _query[filtr.pname] = filtr.value
         if req.params.get('include'):
             _query['include'] = req.params.get('include')
         for finfo in qinfo.field_info:
             _query[finfo.key] = finfo.val
         for filtr in qinfo.filter_info:
```

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/unit_tests.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/unit_tests.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/version.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/version.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/__init__.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/__init__.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/collection_get.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/collection_get.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/collection_post.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/collection_post.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/item_delete.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/item_delete.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/item_get.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/item_get.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/item_patch.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/item_patch.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/related_get.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/related_get.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/relationships_delete.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/relationships_delete.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/relationships_patch.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/relationships_patch.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/loop/relationships_post.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/loop/relationships_post.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi/workflow/selectin/collection_get.py` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi/workflow/selectin/collection_get.py`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi.egg-info/PKG-INFO` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyramid-jsonapi
-Version: 2.2.9.dev1
+Version: 2.2.9.dev2
 Summary: Auto-build JSON API from sqlalchemy models using the pyramid framework
 Home-page: https://github.com/colinhiggs/pyramid-jsonapi
 Author: Colin Higgs
 Author-email: colin.higgs70@gmail.com
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Keywords: json,api,json-api,jsonapi,jsonschema,openapi,pyramid,sqlalchemy
 Platform: UNKNOWN
```

### Comparing `pyramid_jsonapi-2.2.9.dev1/pyramid_jsonapi.egg-info/SOURCES.txt` & `pyramid_jsonapi-2.2.9.dev2/pyramid_jsonapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyramid_jsonapi-2.2.9.dev1/setup.py` & `pyramid_jsonapi-2.2.9.dev2/setup.py`

 * *Files identical despite different names*

