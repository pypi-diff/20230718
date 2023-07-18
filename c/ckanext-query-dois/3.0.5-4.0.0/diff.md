# Comparing `tmp/ckanext-query-dois-3.0.5.tar.gz` & `tmp/ckanext-query-dois-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-query-dois-3.0.5.tar", last modified: Mon Jul 17 08:21:40 2023, max compression
+gzip compressed data, was "ckanext-query-dois-4.0.0.tar", last modified: Tue Jul 18 09:46:30 2023, max compression
```

## Comparing `ckanext-query-dois-3.0.5.tar` & `ckanext-query-dois-4.0.0.tar`

### file list

```diff
@@ -1,66 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.745512 ckanext-query-dois-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-17 08:21:40.745512 ckanext-query-dois-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/doi.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/logic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/routes/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/routes/query_doi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/less/query_dois.less
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/less/visual_query.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/scripts/multisearch_download.js
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/multisearch_landing_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/single_landing_page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/recent_dois_sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_multisearch.html
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 08:21:40.000000 ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.741512 ckanext-query-dois-3.0.5/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:21:40.745512 ckanext-query-dois-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.737512 ckanext-query-dois-3.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:40.745512 ckanext-query-dois-3.0.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-17 08:21:28.000000 ckanext-query-dois-3.0.5/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.816272 ckanext-query-dois-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-18 09:46:30.816272 ckanext-query-dois-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.808272 ckanext-query-dois-4.0.0/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.808272 ckanext-query-dois-4.0.0/ckanext/query_dois/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/lib/doi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/lib/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/lib/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/lib/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/logic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/logic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/logic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/logic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.808272 ckanext-query-dois-4.0.0/ckanext/query_dois/migration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/migration/query_dois/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/migration/query_dois/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/migration/query_dois/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/migration/query_dois/versions/a74242a670e0_set_old_query_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/routes/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/routes/query_doi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.808272 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/assets/less/query_dois.less
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/assets/less/visual_query.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/assets/scripts/multisearch_download.js
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.808272 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/multisearch_landing_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/single_landing_page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/snippets/recent_dois_sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_multisearch.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-18 09:46:30.000000 ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-18 09:46:30.000000 ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:46:30.000000 ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 09:46:30.000000 ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:46:30.000000 ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 09:46:30.000000 ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 09:46:30.000000 ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.808272 ckanext-query-dois-4.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.812272 ckanext-query-dois-4.0.0/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:46:30.816272 ckanext-query-dois-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.808272 ckanext-query-dois-4.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:30.816272 ckanext-query-dois-4.0.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/tests/unit/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/tests/unit/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-18 09:46:19.000000 ckanext-query-dois-4.0.0/tests/unit/test_utils.py
```

### Comparing `ckanext-query-dois-3.0.5/LICENSE` & `ckanext-query-dois-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/PKG-INFO` & `ckanext-query-dois-4.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-query-dois
-Version: 3.0.5
+Version: 4.0.0
 Summary: A CKAN extension that creates DOIs for queries on resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-query-dois
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-query-dois/blob/main/CHANGELOG.md
 Keywords: CKAN,data,doi
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,17 +35,15 @@
 <!--header-end-->
 
 # Overview
 
 <!--overview-start-->
 This extension creates (mints) digital object identifiers (DOIs) for queries on resources. By recording the query parameters used and the exact version of the data at the time of the query, this allows precise retrieval of the data as it looked when the DOI was minted.
 
-**Must be used in conjunction with v4+ of the [ckanext-versioned-datastore](https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore).**
-
-_Optionally:_ [ckanext-ckanpackager](https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager) can be used to get DOIs for downloads (`query-dois` automatically hooks into the `ckanext-ckanpackager` interface if it finds the plugin is active in the running CKAN environment).
+Can be used in conjunction with **v5+** of [ckanext-versioned-datastore](https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore).
 
 You will need an account with a DataCite DOI service provider to use this extension.
 
 <!--overview-end-->
 
 # Installation
```

### Comparing `ckanext-query-dois-3.0.5/README.md` & `ckanext-query-dois-4.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 <!--header-end-->
 
 # Overview
 
 <!--overview-start-->
 This extension creates (mints) digital object identifiers (DOIs) for queries on resources. By recording the query parameters used and the exact version of the data at the time of the query, this allows precise retrieval of the data as it looked when the DOI was minted.
 
-**Must be used in conjunction with v4+ of the [ckanext-versioned-datastore](https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore).**
-
-_Optionally:_ [ckanext-ckanpackager](https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager) can be used to get DOIs for downloads (`query-dois` automatically hooks into the `ckanext-ckanpackager` interface if it finds the plugin is active in the running CKAN environment).
+Can be used in conjunction with **v5+** of [ckanext-versioned-datastore](https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore).
 
 You will need an account with a DataCite DOI service provider to use this extension.
 
 <!--overview-end-->
 
 # Installation
```

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/cli.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/helpers.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/doi.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/lib/doi.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,16 @@
         doi,
         datastore_query.query,
         datastore_query.query_hash,
         resources_and_versions,
         timestamp,
         record_count,
         requested_version=datastore_query.requested_version,
+        query_version='v0',
+        resource_counts={resource_id: record_count},
     )
     return True, query_doi
 
 
 def mint_multisearch_doi(query, query_version, resource_ids_and_versions):
     """
     Mint a DOI on datacite using their API and create a new QueryDOI object, saving it
```

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/emails.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/lib/emails.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/query.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/lib/query.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/stats.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/lib/stats.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/lib/utils.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/lib/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/logic/action.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/logic/schema.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/logic/utils.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/logic/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/model.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/model.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/plugin.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,34 +13,33 @@
 from . import helpers, routes, cli
 from .lib.doi import mint_doi, mint_multisearch_doi, find_existing_doi
 from .lib.query import DatastoreQuery
 from .lib.stats import DOWNLOAD_ACTION, record_stat
 from .logic import auth, action
 from .logic.utils import extract_resource_ids_and_versions
 
+
 log = logging.getLogger(__name__)
 
 
 class QueryDOIsPlugin(plugins.SingletonPlugin):
     plugins.implements(plugins.IBlueprint, inherit=True)
     plugins.implements(plugins.IConfigurer, inherit=True)
     plugins.implements(plugins.ITemplateHelpers)
     plugins.implements(plugins.IActions)
     plugins.implements(plugins.IAuthFunctions)
     plugins.implements(plugins.IClick)
-    # if the ckanpackager is available, we have a hook for it
-    with suppress(ImportError):
-        from ckanext.ckanpackager.interfaces import ICkanPackager
-
-        plugins.implements(ICkanPackager)
     # if the versioned datastore downloader is available, we have a hook for it
-    with suppress(ImportError):
+    try:
         from ckanext.versioned_datastore.interfaces import IVersionedDatastoreDownloads
 
         plugins.implements(IVersionedDatastoreDownloads, inherit=True)
+        versioned_datastore_available = True
+    except ImportError:
+        versioned_datastore_available = False
 
     # IBlueprint
     def get_blueprint(self):
         return routes.blueprints
 
     # IClick
     def get_commands(self):
@@ -124,68 +123,20 @@
             if doi and request.state == 'complete':
                 # record a download stat against the DOI
                 record_stat(doi, DOWNLOAD_ACTION, identifier=request.id)
         except:
             # just log the error and move on
             log.error('Failed to retrieve DOI and/or create stats', exc_info=True)
 
-    # ICkanPackager
-    def before_package_request(
-        self, resource_id, package_id, packager_url, request_params
-    ):
-        """
-        This is called prior to the ckanpackager plugin starting it's creation of a
-        download, therefore we can use it to mint DOIs and record a stat.
-
-        :param resource_id: the resource id of the resource that is about to be packaged
-        :param package_id: the package id of the resource that is about to be packaged
-        :param packager_url: the target url for this packaging request
-        :param request_params: a dict of parameters that will be sent with the request
-        :return: the url and the params as a tuple
-        """
-        resource = plugins.toolkit.get_action('resource_show')({}, {'id': resource_id})
-        package = plugins.toolkit.get_action('package_show')({}, {'id': package_id})
-        # only handle DOIs for resources with data in the datastore and that aren't in private
-        # packages
-        if resource.get('datastore_active', False) and not package.get('private', True):
-            try:
-                # the request_params dict comes through with a lot of other parameters in it beyond
-                # the query params, therefore we need to do some stripping out (otherwise the exact
-                # same query will look different due to a different format choice or email address)
-                allowed_keys = {'q', 'filters', 'version'}
-                data_dict = {
-                    k: v for k, v in request_params.items() if k in allowed_keys
-                }
-
-                # the packager converts the filters dict to JSON so we need to convert it back
-                if 'filters' in data_dict:
-                    data_dict['filters'] = json.loads(data_dict['filters'])
-
-                # mint the DOI on datacite if necessary
-                _minted, query_doi = mint_doi(
-                    [resource_id], DatastoreQuery(data_dict=data_dict)
-                )
-                # record a download stat against the DOI
-                record_stat(query_doi, DOWNLOAD_ACTION, request_params['email'])
-                # add the doi to the ckanpackager params so that it can be reported in the email
-                request_params['doi'] = query_doi.doi
-            except:
-                # if anything goes wrong we don't want to stop the download from going ahead, just
-                # log the error and move on
-                log.error(
-                    'Failed to mint/retrieve DOI and/or create stats', exc_info=True
-                )
-
-        return packager_url, request_params
-
     # ITemplateHelpers
     def get_helpers(self):
         return {
             'render_filter_value': helpers.render_filter_value,
             'get_most_recent_dois': helpers.get_most_recent_dois,
             'get_time_ago_description': helpers.get_time_ago_description,
             'get_landing_page_url': helpers.get_landing_page_url,
             'create_citation_text': helpers.create_citation_text,
             'create_multisearch_citation_text': helpers.create_multisearch_citation_text,
             'pretty_print_query': helpers.pretty_print_query,
             'get_doi_count': helpers.get_doi_count,
+            'versioned_datastore_available': self.versioned_datastore_available,
         }
```

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/routes/_helpers.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/routes/_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -157,35 +157,14 @@
             'current': api_url
             + '?'
             + encode_params(query, extras=api_extras, for_api=True),
         },
     }
 
 
-def get_download_url(package, resource, query, rounded_version):
-    """
-    Returns the URL for the CKANPackager's download endpoint, or None if the
-    CKANPackager is not in use.
-
-    :param package: the package dict
-    :param resource: the resource dict
-    :param query: the query dict
-    :param rounded_version: the version rounded down to the nearest available on the resource
-    :return: the URL for packaging the resource up with the CKANPackager or None if the
-             CKANPackager is not installed
-    """
-    try:
-        from ckanext.ckanpackager.lib.utils import url_for_package_resource
-
-        url = url_for_package_resource(package['id'], resource['id'], use_request=False)
-        return url + '&' + encode_params(query, version=rounded_version)
-    except ImportError:
-        return None
-
-
 def get_stats(query_doi):
     '''
     Retrieve some simple stats about the query DOI - this includes the total downloads and the
     last download timestamp. Note that we are specifically looking for downloads here, no other
     actions are considered.
 
     :param query_doi: the QueryDOI object
@@ -239,17 +218,14 @@
         # demand we should open this up so that we can support other dois on packages extensions
         'package_doi': package['doi'] if package.get('doi_status', False) else None,
         'authors': get_authors([package]),
         'version': rounded_version,
         'reruns': generate_rerun_urls(
             resource, package, query_doi.query, rounded_version
         ),
-        'download_url': get_download_url(
-            package, resource, query_doi.query, rounded_version
-        ),
         'downloads': downloads,
         'last_download_timestamp': last_download_timestamp,
     }
 
     return toolkit.render('query_dois/single_landing_page.html', context)
```

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/routes/query_doi.py` & `ckanext-query-dois-4.0.0/ckanext/query_dois/routes/query_doi.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     :return: the rendered landing page
     """
     doi = '{}/{}'.format(data_centre, identifier)
     query_doi = _helpers.get_query_doi(doi)
     if query_doi is None:
         raise toolkit.abort(404, toolkit._('DOI not recognised'))
 
-    if query_doi.query_version is not None:
+    if query_doi.query_version is not None and query_doi.query_version != 'v0':
         return _helpers.render_multisearch_doi_page(query_doi)
     else:
         return _helpers.render_datastore_search_doi_page(query_doi)
 
 
 @blueprint.route('')
 def doi_stats():
```

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/less/query_dois.less` & `ckanext-query-dois-4.0.0/ckanext/query_dois/theme/assets/less/query_dois.less`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/assets/scripts/multisearch_download.js` & `ckanext-query-dois-4.0.0/ckanext/query_dois/theme/assets/scripts/multisearch_download.js`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/multisearch_landing_page.html` & `ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/single_landing_page.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,174 +1,162 @@
 {% extends "page.html" %}
 
 {% block title %}
-  {{ _('DOI') }}: {{ query_doi.doi }}
+{{ _('DOI') }}: {{ doi }}
 {% endblock %}
 
 {%- block meta -%}
-  {{ super() }}
-    <meta name="citation_doi" content="doi:https://doi.org/{{ query_doi.doi }}"/>
-    <meta name="citation_title"
-          content="Data Portal Query on {{ resource_count }} resources, {{ query_doi.count }} records"/>
-    <meta name="citation_author" content="{{ ', '.join(authors) }}"/>
-    <meta name="citation_online_date" content="{{ query_doi.timestamp }}"/>
-    <meta name="citation_publisher" content="{{ publisher }}"/>
+    {{ super() }}
+    <meta name="citation_doi" content="doi:https://doi.org/{{ doi }}" />
+    <meta name="citation_title" content="Data Portal Query on {{ resource['name'] }}, {{ query_doi.count }} records" />
+    <meta name="citation_author" content="{{', '.join(authors)}}" />
+    <meta name="citation_online_date" content="{{ query_doi.timestamp }}" />
+    <meta name="citation_publisher" content="{{ publisher }}" />
 {%- endblock -%}
 
 {% block primary_content %}
-  {% asset 'ckanext-query-dois/main' %}
-    <article class="module">
-        <div class="module-content">
-            <h1 class="page-heading">{{ _('DOI') }}: {{ query_doi.doi }}</h1>
-
-          {% block visual_query %}
-            {% snippet "query_dois/snippets/visual_datastore_multisearch.html", query=query_doi.query %}
-              <br/>
-          {% endblock %}
-
-          {% block citation %}
-              <h3>{{ _('Cite this as') }}</h3>
-              <hr>
-              <div>
-                  <p>
-                    {{ h.create_multisearch_citation_text(query_doi, html=True) | safe }}
-                  </p>
-              </div>
-              <br/>
-          {% endblock %}
-
-          {% block details %}
-              <h3>{{ _('Details') }}</h3>
-              <hr>
-              <div class="qd_details">
-                  <div>
-                      <b>{{ _('Resource count:') }}</b> {{ resource_count }}
-                  </div>
-                  <div>
-                      <b>{{ _('Dataset count:') }}</b> {{ package_count }}
-                  </div>
-                {#            <div>#}
-                {#                <b>{{ _('License:') }}</b> {% snippet "snippets/license.html", pkg_dict=package, text_only=True %}#}
-                {#            </div>#}
-                  <div>
-                      <b>{{ _('Retrieved:') }}</b> {{ query_doi.timestamp }}
-                  </div>
-                  <div>
-                      <b>{{ _('Total records:') }}</b> {{ query_doi.count }}
-                  </div>
-              </div>
-          {% endblock %}
-
-          {% block stats %}
-              <h3>{{ _('Statistics') }}</h3>
-              <hr>
-              <div class="qd_stats">
-                  <div>
-                      <b>{{ _('Total downloads:') }}</b> {{ downloads }}
-                  </div>
-                  <div>
-                      <b>{{ _('Total saves:') }}</b> {{ saves }}
-                  </div>
-                  <div>
-                      <b>{{ _('Last downloaded:') }}</b> {{ last_download_timestamp }}
-                  </div>
-              </div>
-          {% endblock %}
-          {% block resource_breakdown %}
-              <h3>{{ _('Resource breakdown') }}</h3>
-              <hr>
-              <div>
-                  <table class="qd_breakdown">
-                    {% for resource_id, count in sorted_resource_counts %}
-                      {% set resource_info = resources[resource_id] %}
-                      {% set package_info = packages[resource_info['package_id']] %}
-                      {% set resource_url = h.url_for('resource.read', id=package_info['name'], resource_id=resource_id) %}
-                      {% set package_url = h.url_for('dataset.read', id=package_info['name']) %}
-                        <tr>
-                            <td><a href="{{ package_url }}">{{ package_info['title'] }}</a> / <a
-                                    href="{{ resource_url }}">{{ resource_info['name'] }}</a></td>
-                            <td><b>{{ count }} {{ _('records') }}</b></td>
-                        </tr>
-                    {% endfor %}
-                  </table>
-              </div>
-          {% endblock %}
+{% asset 'ckanext-query-dois/main' %}
+<article class="module">
+    <div class="module-content">
+        <h1 class="page-heading">{{ _('DOI') }}: {{ doi }}</h1>
+
+        {% block visual_query %}
+        {% snippet "query_dois/snippets/visual_datastore_search.html", search=query_doi.query %}
+        <br />
+        {% endblock %}
+
+        {% block citation %}
+        <h3>{{ _('Cite this as') }}</h3>
+        <hr>
+        <div>
+            <p>
+                {{ h.create_citation_text(query_doi.doi, query_doi.timestamp, resource['name'],
+                                          package['title'], package_doi, html=True) | safe }}
+            </p>
         </div>
-    </article>
-{% endblock %}
+        <br />
+        {% endblock %}
 
-
-{% block secondary_content %}
-    <div class="module module-narrow module-shallow">
-        <h2 class="module-heading">
-            <i class="fas fa-eye fa-lg inline-icon-left"></i>{{ _('View data') }}
-        </h2>
-        <div class="module-content">
-            <a target="_blank" href="/search/{{ original_slug }}">{{ _('Original') }} <i class="fas fa-arrow-circle-right"></i></a>
-            <div class="qd_help_text">
-              {% trans %}
-                  View the data as it looked when the DOI was originally minted.
-              {% endtrans %}
+        {% block details %}
+        <h3>{{ _('Details') }}</h3>
+        <hr>
+        <div class="qd_details">
+            <div>
+                {% set resource_url = h.url_for('resource.read', id=package['name'], resource_id=resource['id']) %}
+                {% set package_url = h.url_for('dataset.read', id=package['name']) %}
+                <b>{{ _('Resource:') }}</b> <a href="{{ resource_url }}">{{ resource['name'] }}</a>
             </div>
-        </div>
-        <div class="module-content">
-            <a target="_blank" href="/search/{{ current_slug }}">{{ _('Current') }} <i class="fas fa-arrow-circle-right"></i></a>
-            <div class="qd_help_text">
-              {% trans %}
-                  View the data as it looks now. This may result in different results to the DOI's
-                  original data if the data has been modified since it was minted.
-              {% endtrans %}
+            <div>
+                <b>{{ _('Package:') }}</b> <a href="{{ package_url }}">{{ package['title'] }}</a>
+            </div>
+            <div>
+                <b>{{ _('License:') }}</b> {% snippet "snippets/license.html", pkg_dict=package, text_only=True %}
+            </div>
+            <div>
+                <b>{{ _('Retrieved:') }}</b> {{ query_doi.timestamp }}
+            </div>
+            <div>
+                <b>{{ _('Total records:') }}</b> {{ query_doi.count }}
             </div>
         </div>
-    </div>
+        {% endblock %}
 
-    <div class="module, module-narrow module-shallow">
-        {% asset 'ckanext-query-dois/multisearch' %}
-        <h2 class="module-heading">
-            <i class="far fa-arrow-alt-circle-down fa-lg inline-icon-left"></i>{{ _('Download') }}
-        </h2>
-        <div class="module-content">
-            <p>
-              {% trans %}
-                  Request to download the data associated with this DOI as it looked when the DOI
-                  was minted.
-              {% endtrans %}
-            </p>
-            <div class="form-group">
-                <div class="form-row">
-                    <label for="download-format">File format</label>
-                    <select id="download-format"
-                            class="full-width">
-                        <option value="csv">CSV/TSV</option>
-                        <option value="dwc">Darwin Core</option>
-                        <option value="xlsx">Excel (XLSX)</option>
-                        <option value="json">JSON</option>
-                    </select>
-                </div>
-                <div class="form-row flex-container flex-wrap flex-between">
-                    <div class="no-pad-h">
-                        <label for="download-sep">One file per resource</label>
-                        <input
-                            id="download-sep"
-                            type="checkbox" checked>
-                    </div>
-                    <div class="no-pad-h">
-                        <label for="download-empty">Skip empty columns</label>
-                        <input id="download-empty"
-                               type="checkbox" checked>
-                    </div>
-                </div>
-                <small>View this query on the <a target="_blank" href="/search/{{ original_slug }}">search page</a> for more advanced download options, including email notifications.</small>
-            </div>
-
-            {% block privacy_warning %}{% endblock %}
-            <div class="text-left">
-                <a id="download-button" href="#" class="btn btn-primary text-right"
-                   data-query='{{ query_doi.query|tojson }}'
-                   data-query-version='{{ query_doi.query_version }}'
-                   data-resources-and-versions='{{ query_doi.resources_and_versions|tojson }}'>
-                    <i class="fas fa-download"></i> Request Download
-                </a>
+        {% block stats %}
+        <h3>{{ _('Statistics') }}</h3>
+        <hr>
+        <div class="qd_stats">
+            <div>
+                <b>{{ _('Total downloads:') }}</b> {{ downloads }}
+            </div>
+            <div>
+                <b>{{ _('Last downloaded:') }}</b> {{ last_download_timestamp }}
             </div>
         </div>
+        {% endblock %}
+    </div>
+</article>
+{% endblock %}
+
+
+{% block secondary_content %}
+<div class="module module-narrow module-shallow">
+    <h2 class="module-heading">
+        <i class="fas fa-eye fa-lg inline-icon-left"></i>{{ _('View data') }}
+        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
+            <span class="qd_tooltiptext">
+                {% trans %}
+                Use the links to view the data associated with this DOI.
+                {% endtrans %}
+            </span>
+        </i>
+    </h2>
+    <div class="module-content">
+        <a href="{{ reruns.page.original }}">{{ _('Original') }}</a>
+        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
+            <span class="qd_tooltiptext">
+                {% trans %}
+                View the data as it looked when the DOI was originally minted.
+                {% endtrans %}
+            </span>
+        </i>
+    </div>
+    <div class="module-content">
+        <a href="{{ reruns.page.current }}">{{ _('Current') }}</a>
+        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
+            <span class="qd_tooltiptext">
+                {% trans %}
+                View the data as it looks now. This may result in different results to the DOI's
+                original data if the data has been modified since it was minted.
+                {% endtrans %}
+            </span>
+        </i>
+    </div>
+</div>
+
+<div class="module module-narrow module-shallow">
+    <h2 class="module-heading">
+        <i class="fas fa-flask fa-lg inline-icon-left"></i>{{ _('View with API') }}
+        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
+            <span class="qd_tooltiptext">
+                {% trans %}
+                Use the links to view the data associated with this DOI through the API.
+                {% endtrans %}
+            </span>
+        </i>
+    </h2>
+    <div class="module-content">
+        <a href="{{ reruns.api.original }}">{{ _('Original') }}</a>
+        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
+            <span class="qd_tooltiptext">
+                {% trans %}
+                View the data as it looked when the DOI was originally minted.
+                {% endtrans %}
+            </span>
+        </i>
+    </div>
+    <div class="module-content">
+        <a href="{{ reruns.api.current }}">{{ _('Current') }}</a>
+        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
+            <span class="qd_tooltiptext">
+                {% trans %}
+                View the data as it looks now. This may result in different results to the DOI's
+                original data if the data has been modified since it was minted.
+                {% endtrans %}
+            </span>
+        </i>
+    </div>
+</div>
+
+{% if h.versioned_datastore_available %}
+<div class="module, module-narrow module-shallow">
+    <h2 class="module-heading">
+        <i class="far fa-arrow-alt-circle-down fa-lg inline-icon-left"></i>{{ _('Download') }}
+    </h2>
+    <div class="module-content">
+        {% snippet 'versioned_datastore/snippets/download_button.html',
+            slug_or_doi=query_doi.doi,
+            icon_class="fas fa-download",
+            label=_('Download') %}
     </div>
+</div>
+{% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,60 +1,54 @@
-{% extends "page.html" %} {% block title %} {{ _('DOI') }}: {{ query_doi.doi }}
-{% endblock %} {%- block meta -%} {{ super() }}
+{% extends "page.html" %} {% block title %} {{ _('DOI') }}: {{ doi }} {%
+endblock %} {%- block meta -%} {{ super() }}
 
 
 
 
  {%- endblock -%} {% block primary_content %} {% asset 'ckanext-query-dois/
 main' %}
-****** {{ _('DOI') }}: {{ query_doi.doi }} ******
+****** {{ _('DOI') }}: {{ doi }} ******
 {% block visual_query %} {% snippet "query_dois/snippets/
-visual_datastore_multisearch.html", query=query_doi.query %}
+visual_datastore_search.html", search=query_doi.query %}
 {% endblock %} {% block citation %}
 **** {{ _('Cite this as') }} ****
 ===============================================================================
-{{ h.create_multisearch_citation_text(query_doi, html=True) | safe }}
+{{ h.create_citation_text(query_doi.doi, query_doi.timestamp, resource['name'],
+package['title'], package_doi, html=True) | safe }}
 
 {% endblock %} {% block details %}
 **** {{ _('Details') }} ****
 ===============================================================================
-{{ _('Resource count:') }} {{ resource_count }}
-{{ _('Dataset count:') }} {{ package_count }}
-{#
-#} {# {{ _('License:') }} {% snippet "snippets/license.html", pkg_dict=package,
-text_only=True %}#} {#
-#}
+{% set resource_url = h.url_for('resource.read', id=package['name'],
+resource_id=resource['id']) %} {% set package_url = h.url_for('dataset.read',
+id=package['name']) %} {{ _('Resource:') }} {{_resource['name']_}}
+{{ _('Package:') }} {{_package['title']_}}
+{{ _('License:') }} {% snippet "snippets/license.html", pkg_dict=package,
+text_only=True %}
 {{ _('Retrieved:') }} {{ query_doi.timestamp }}
 {{ _('Total records:') }} {{ query_doi.count }}
 {% endblock %} {% block stats %}
 **** {{ _('Statistics') }} ****
 ===============================================================================
 {{ _('Total downloads:') }} {{ downloads }}
-{{ _('Total saves:') }} {{ saves }}
 {{ _('Last downloaded:') }} {{ last_download_timestamp }}
-{% endblock %} {% block resource_breakdown %}
-**** {{ _('Resource breakdown') }} ****
-===============================================================================
-{{_package_info['title']_}} / {{_resource_info {{ count }} {{ _('records') }}
-['name']_}}
 {% endblock %}
  {% endblock %} {% block secondary_content %}
-{{ _('View data') }}
-{{__('Original')_}}
-{% trans %} View the data as it looked when the DOI was originally minted. {%
-endtrans %}
-{{__('Current')_}}
-{% trans %} View the data as it looks now. This may result in different results
-to the DOI's original data if the data has been modified since it was minted.
-{% endtrans %}
-{% asset 'ckanext-query-dois/multisearch' %}
+{{ _('View data') }}  {% trans %} Use the links to view the data associated
+with this DOI. {% endtrans %}
+{{__('Original')_}}  {% trans %} View the data as it looked when the DOI was
+originally minted. {% endtrans %}
+{{__('Current')_}}  {% trans %} View the data as it looks now. This may result
+in different results to the DOI's original data if the data has been modified
+since it was minted. {% endtrans %}
+{{ _('View with API') }}  {% trans %} Use the links to view the data associated
+with this DOI through the API. {% endtrans %}
+{{__('Original')_}}  {% trans %} View the data as it looked when the DOI was
+originally minted. {% endtrans %}
+{{__('Current')_}}  {% trans %} View the data as it looks now. This may result
+in different results to the DOI's original data if the data has been modified
+since it was minted. {% endtrans %}
+{% if h.versioned_datastore_available %}
 {{ _('Download') }}
-{% trans %} Request to download the data associated with this DOI as it looked
-when the DOI was minted. {% endtrans %}
-File format [One of: CSV/TSV/Darwin Core/Excel (XLSX)/JSON]
-One file per resource *
-Skip empty columns *
-View this query on the search_page for more advanced download options,
-including email notifications.
-{% block privacy_warning %}{% endblock %}
- Request_Download
-{% endblock %}
+{% snippet 'versioned_datastore/snippets/download_button.html',
+slug_or_doi=query_doi.doi, icon_class="fas fa-download", label=_('Download') %}
+{% endif %} {% endblock %}
```

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/single_landing_page.html` & `ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/multisearch_landing_page.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,158 +1,137 @@
 {% extends "page.html" %}
 
 {% block title %}
-{{ _('DOI') }}: {{ doi }}
+  {{ _('DOI') }}: {{ query_doi.doi }}
 {% endblock %}
 
 {%- block meta -%}
-    {{ super() }}
-    <meta name="citation_doi" content="doi:https://doi.org/{{ doi }}" />
-    <meta name="citation_title" content="Data Portal Query on {{ resource['name'] }}, {{ query_doi.count }} records" />
-    <meta name="citation_author" content="{{', '.join(authors)}}" />
-    <meta name="citation_online_date" content="{{ query_doi.timestamp }}" />
-    <meta name="citation_publisher" content="{{ publisher }}" />
+  {{ super() }}
+    <meta name="citation_doi" content="doi:https://doi.org/{{ query_doi.doi }}"/>
+    <meta name="citation_title"
+          content="Data Portal Query on {{ resource_count }} resources, {{ query_doi.count }} records"/>
+    <meta name="citation_author" content="{{ ', '.join(authors) }}"/>
+    <meta name="citation_online_date" content="{{ query_doi.timestamp }}"/>
+    <meta name="citation_publisher" content="{{ publisher }}"/>
 {%- endblock -%}
 
 {% block primary_content %}
-{% asset 'ckanext-query-dois/main' %}
-<article class="module">
-    <div class="module-content">
-        <h1 class="page-heading">{{ _('DOI') }}: {{ doi }}</h1>
-
-        {% block visual_query %}
-        {% snippet "query_dois/snippets/visual_datastore_search.html", search=query_doi.query %}
-        <br />
-        {% endblock %}
-
-        {% block citation %}
-        <h3>{{ _('Cite this as') }}</h3>
-        <hr>
-        <div>
-            <p>
-                {{ h.create_citation_text(query_doi.doi, query_doi.timestamp, resource['name'],
-                                          package['title'], package_doi, html=True) | safe }}
-            </p>
+  {% asset 'ckanext-query-dois/main' %}
+    <article class="module">
+        <div class="module-content">
+            <h1 class="page-heading">{{ _('DOI') }}: {{ query_doi.doi }}</h1>
+
+          {% block visual_query %}
+            {% snippet "query_dois/snippets/visual_datastore_multisearch.html", query=query_doi.query %}
+              <br/>
+          {% endblock %}
+
+          {% block citation %}
+              <h3>{{ _('Cite this as') }}</h3>
+              <hr>
+              <div>
+                  <p>
+                    {{ h.create_multisearch_citation_text(query_doi, html=True) | safe }}
+                  </p>
+              </div>
+              <br/>
+          {% endblock %}
+
+          {% block details %}
+              <h3>{{ _('Details') }}</h3>
+              <hr>
+              <div class="qd_details">
+                  <div>
+                      <b>{{ _('Resource count:') }}</b> {{ resource_count }}
+                  </div>
+                  <div>
+                      <b>{{ _('Dataset count:') }}</b> {{ package_count }}
+                  </div>
+                {#            <div>#}
+                {#                <b>{{ _('License:') }}</b> {% snippet "snippets/license.html", pkg_dict=package, text_only=True %}#}
+                {#            </div>#}
+                  <div>
+                      <b>{{ _('Retrieved:') }}</b> {{ query_doi.timestamp }}
+                  </div>
+                  <div>
+                      <b>{{ _('Total records:') }}</b> {{ query_doi.count }}
+                  </div>
+              </div>
+          {% endblock %}
+
+          {% block stats %}
+              <h3>{{ _('Statistics') }}</h3>
+              <hr>
+              <div class="qd_stats">
+                  <div>
+                      <b>{{ _('Total downloads:') }}</b> {{ downloads }}
+                  </div>
+                  <div>
+                      <b>{{ _('Total saves:') }}</b> {{ saves }}
+                  </div>
+                  <div>
+                      <b>{{ _('Last downloaded:') }}</b> {{ last_download_timestamp }}
+                  </div>
+              </div>
+          {% endblock %}
+          {% block resource_breakdown %}
+              <h3>{{ _('Resource breakdown') }}</h3>
+              <hr>
+              <div>
+                  <table class="qd_breakdown">
+                    {% for resource_id, count in sorted_resource_counts %}
+                      {% set resource_info = resources[resource_id] %}
+                      {% set package_info = packages[resource_info['package_id']] %}
+                      {% set resource_url = h.url_for('resource.read', id=package_info['name'], resource_id=resource_id) %}
+                      {% set package_url = h.url_for('dataset.read', id=package_info['name']) %}
+                        <tr>
+                            <td><a href="{{ package_url }}">{{ package_info['title'] }}</a> / <a
+                                    href="{{ resource_url }}">{{ resource_info['name'] }}</a></td>
+                            <td><b>{{ count }} {{ _('records') }}</b></td>
+                        </tr>
+                    {% endfor %}
+                  </table>
+              </div>
+          {% endblock %}
         </div>
-        <br />
-        {% endblock %}
+    </article>
+{% endblock %}
 
-        {% block details %}
-        <h3>{{ _('Details') }}</h3>
-        <hr>
-        <div class="qd_details">
-            <div>
-                {% set resource_url = h.url_for('resource.read', id=package['name'], resource_id=resource['id']) %}
-                {% set package_url = h.url_for('dataset.read', id=package['name']) %}
-                <b>{{ _('Resource:') }}</b> <a href="{{ resource_url }}">{{ resource['name'] }}</a>
-            </div>
-            <div>
-                <b>{{ _('Package:') }}</b> <a href="{{ package_url }}">{{ package['title'] }}</a>
-            </div>
-            <div>
-                <b>{{ _('License:') }}</b> {% snippet "snippets/license.html", pkg_dict=package, text_only=True %}
-            </div>
-            <div>
-                <b>{{ _('Retrieved:') }}</b> {{ query_doi.timestamp }}
-            </div>
-            <div>
-                <b>{{ _('Total records:') }}</b> {{ query_doi.count }}
-            </div>
-        </div>
-        {% endblock %}
 
-        {% block stats %}
-        <h3>{{ _('Statistics') }}</h3>
-        <hr>
-        <div class="qd_stats">
-            <div>
-                <b>{{ _('Total downloads:') }}</b> {{ downloads }}
+{% block secondary_content %}
+    <div class="module module-narrow module-shallow">
+        <h2 class="module-heading">
+            <i class="fas fa-eye fa-lg inline-icon-left"></i>{{ _('View data') }}
+        </h2>
+        <div class="module-content">
+            <a target="_blank" href="/search/{{ original_slug }}">{{ _('Original') }} <i class="fas fa-arrow-circle-right"></i></a>
+            <div class="qd_help_text">
+              {% trans %}
+                  View the data as it looked when the DOI was originally minted.
+              {% endtrans %}
             </div>
-            <div>
-                <b>{{ _('Last downloaded:') }}</b> {{ last_download_timestamp }}
+        </div>
+        <div class="module-content">
+            <a target="_blank" href="/search/{{ current_slug }}">{{ _('Current') }} <i class="fas fa-arrow-circle-right"></i></a>
+            <div class="qd_help_text">
+              {% trans %}
+                  View the data as it looks now. This may result in different results to the DOI's
+                  original data if the data has been modified since it was minted.
+              {% endtrans %}
             </div>
         </div>
-        {% endblock %}
     </div>
-</article>
-{% endblock %}
-
 
-{% block secondary_content %}
-<div class="module module-narrow module-shallow">
-    <h2 class="module-heading">
-        <i class="fas fa-eye fa-lg inline-icon-left"></i>{{ _('View data') }}
-        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
-            <span class="qd_tooltiptext">
-                {% trans %}
-                Use the links to view the data associated with this DOI.
-                {% endtrans %}
-            </span>
-        </i>
-    </h2>
-    <div class="module-content">
-        <a href="{{ reruns.page.original }}">{{ _('Original') }}</a>
-        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
-            <span class="qd_tooltiptext">
-                {% trans %}
-                View the data as it looked when the DOI was originally minted.
-                {% endtrans %}
-            </span>
-        </i>
-    </div>
-    <div class="module-content">
-        <a href="{{ reruns.page.current }}">{{ _('Current') }}</a>
-        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
-            <span class="qd_tooltiptext">
-                {% trans %}
-                View the data as it looks now. This may result in different results to the DOI's
-                original data if the data has been modified since it was minted.
-                {% endtrans %}
-            </span>
-        </i>
-    </div>
-</div>
-
-<div class="module module-narrow module-shallow">
-    <h2 class="module-heading">
-        <i class="fas fa-flask fa-lg inline-icon-left"></i>{{ _('View with API') }}
-        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
-            <span class="qd_tooltiptext">
-                {% trans %}
-                Use the links to view the data associated with this DOI through the API.
-                {% endtrans %}
-            </span>
-        </i>
-    </h2>
-    <div class="module-content">
-        <a href="{{ reruns.api.original }}">{{ _('Original') }}</a>
-        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
-            <span class="qd_tooltiptext">
-                {% trans %}
-                View the data as it looked when the DOI was originally minted.
-                {% endtrans %}
-            </span>
-        </i>
-    </div>
-    <div class="module-content">
-        <a href="{{ reruns.api.current }}">{{ _('Current') }}</a>
-        <i class="fas fa-info-circle fa-xs inline-icon-right qd_tooltip">
-            <span class="qd_tooltiptext">
-                {% trans %}
-                View the data as it looks now. This may result in different results to the DOI's
-                original data if the data has been modified since it was minted.
-                {% endtrans %}
-            </span>
-        </i>
+    {% if h.versioned_datastore_available %}
+    <div class="module, module-narrow module-shallow">
+        <h2 class="module-heading">
+            <i class="far fa-arrow-alt-circle-down fa-lg inline-icon-left"></i>{{ _('Download') }}
+        </h2>
+        <div class="module-content">
+            {% snippet 'versioned_datastore/snippets/download_button.html',
+            slug_or_doi=query_doi.doi,
+            icon_class="fas fa-download",
+            label=_('Download') %}
+        </div>
     </div>
-</div>
-
-<div class="module, module-narrow module-shallow">
-    <h2 class="module-heading">
-        <i class="far fa-arrow-alt-circle-down fa-lg inline-icon-left"></i>{{ _('Download') }}
-    </h2>
-    {% asset 'ckanext-ckanpackager/main-css' %}
-    {% asset 'ckanext-ckanpackager/main-js' %}
-    <a data-module="ckanpackager-download-link" data-module-resource-id="{{ resource['id'] }}"
-       class="packager-link btn btn-primary" href="{{ download_url }}">{{ _('Download') }}</a>
-</div>
+    {% endif %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,53 +1,53 @@
-{% extends "page.html" %} {% block title %} {{ _('DOI') }}: {{ doi }} {%
-endblock %} {%- block meta -%} {{ super() }}
+{% extends "page.html" %} {% block title %} {{ _('DOI') }}: {{ query_doi.doi }}
+{% endblock %} {%- block meta -%} {{ super() }}
 
 
 
 
  {%- endblock -%} {% block primary_content %} {% asset 'ckanext-query-dois/
 main' %}
-****** {{ _('DOI') }}: {{ doi }} ******
+****** {{ _('DOI') }}: {{ query_doi.doi }} ******
 {% block visual_query %} {% snippet "query_dois/snippets/
-visual_datastore_search.html", search=query_doi.query %}
+visual_datastore_multisearch.html", query=query_doi.query %}
 {% endblock %} {% block citation %}
 **** {{ _('Cite this as') }} ****
 ===============================================================================
-{{ h.create_citation_text(query_doi.doi, query_doi.timestamp, resource['name'],
-package['title'], package_doi, html=True) | safe }}
+{{ h.create_multisearch_citation_text(query_doi, html=True) | safe }}
 
 {% endblock %} {% block details %}
 **** {{ _('Details') }} ****
 ===============================================================================
-{% set resource_url = h.url_for('resource.read', id=package['name'],
-resource_id=resource['id']) %} {% set package_url = h.url_for('dataset.read',
-id=package['name']) %} {{ _('Resource:') }} {{_resource['name']_}}
-{{ _('Package:') }} {{_package['title']_}}
-{{ _('License:') }} {% snippet "snippets/license.html", pkg_dict=package,
-text_only=True %}
+{{ _('Resource count:') }} {{ resource_count }}
+{{ _('Dataset count:') }} {{ package_count }}
+{#
+#} {# {{ _('License:') }} {% snippet "snippets/license.html", pkg_dict=package,
+text_only=True %}#} {#
+#}
 {{ _('Retrieved:') }} {{ query_doi.timestamp }}
 {{ _('Total records:') }} {{ query_doi.count }}
 {% endblock %} {% block stats %}
 **** {{ _('Statistics') }} ****
 ===============================================================================
 {{ _('Total downloads:') }} {{ downloads }}
+{{ _('Total saves:') }} {{ saves }}
 {{ _('Last downloaded:') }} {{ last_download_timestamp }}
+{% endblock %} {% block resource_breakdown %}
+**** {{ _('Resource breakdown') }} ****
+===============================================================================
+{{_package_info['title']_}} / {{_resource_info {{ count }} {{ _('records') }}
+['name']_}}
 {% endblock %}
  {% endblock %} {% block secondary_content %}
-{{ _('View data') }}  {% trans %} Use the links to view the data associated
-with this DOI. {% endtrans %}
-{{__('Original')_}}  {% trans %} View the data as it looked when the DOI was
-originally minted. {% endtrans %}
-{{__('Current')_}}  {% trans %} View the data as it looks now. This may result
-in different results to the DOI's original data if the data has been modified
-since it was minted. {% endtrans %}
-{{ _('View with API') }}  {% trans %} Use the links to view the data associated
-with this DOI through the API. {% endtrans %}
-{{__('Original')_}}  {% trans %} View the data as it looked when the DOI was
-originally minted. {% endtrans %}
-{{__('Current')_}}  {% trans %} View the data as it looks now. This may result
-in different results to the DOI's original data if the data has been modified
-since it was minted. {% endtrans %}
+{{ _('View data') }}
+{{__('Original')_}}
+{% trans %} View the data as it looked when the DOI was originally minted. {%
+endtrans %}
+{{__('Current')_}}
+{% trans %} View the data as it looks now. This may result in different results
+to the DOI's original data if the data has been modified since it was minted.
+{% endtrans %}
+{% if h.versioned_datastore_available %}
 {{ _('Download') }}
-{% asset 'ckanext-ckanpackager/main-css' %} {% asset 'ckanext-ckanpackager/
-main-js' %} {{__('Download')_}}
-{% endblock %}
+{% snippet 'versioned_datastore/snippets/download_button.html',
+slug_or_doi=query_doi.doi, icon_class="fas fa-download", label=_('Download') %}
+{% endif %} {% endblock %}
```

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/recent_dois_sidebar.html` & `ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/snippets/recent_dois_sidebar.html`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_search.html` & `ckanext-query-dois-4.0.0/ckanext/query_dois/theme/templates/query_dois/snippets/visual_datastore_search.html`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/PKG-INFO` & `ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-query-dois
-Version: 3.0.5
+Version: 4.0.0
 Summary: A CKAN extension that creates DOIs for queries on resources.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-query-dois
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-query-dois/blob/main/CHANGELOG.md
 Keywords: CKAN,data,doi
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,17 +35,15 @@
 <!--header-end-->
 
 # Overview
 
 <!--overview-start-->
 This extension creates (mints) digital object identifiers (DOIs) for queries on resources. By recording the query parameters used and the exact version of the data at the time of the query, this allows precise retrieval of the data as it looked when the DOI was minted.
 
-**Must be used in conjunction with v4+ of the [ckanext-versioned-datastore](https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore).**
-
-_Optionally:_ [ckanext-ckanpackager](https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager) can be used to get DOIs for downloads (`query-dois` automatically hooks into the `ckanext-ckanpackager` interface if it finds the plugin is active in the running CKAN environment).
+Can be used in conjunction with **v5+** of [ckanext-versioned-datastore](https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore).
 
 You will need an account with a DataCite DOI service provider to use this extension.
 
 <!--overview-end-->
 
 # Installation
```

### Comparing `ckanext-query-dois-3.0.5/ckanext_query_dois.egg-info/SOURCES.txt` & `ckanext-query-dois-4.0.0/ckanext_query_dois.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 ckanext/query_dois/lib/stats.py
 ckanext/query_dois/lib/utils.py
 ckanext/query_dois/logic/__init__.py
 ckanext/query_dois/logic/action.py
 ckanext/query_dois/logic/auth.py
 ckanext/query_dois/logic/schema.py
 ckanext/query_dois/logic/utils.py
+ckanext/query_dois/migration/query_dois/env.py
+ckanext/query_dois/migration/query_dois/versions/a74242a670e0_set_old_query_version.py
 ckanext/query_dois/routes/__init__.py
 ckanext/query_dois/routes/_helpers.py
 ckanext/query_dois/routes/query_doi.py
 ckanext/query_dois/theme/assets/webassets.yml
 ckanext/query_dois/theme/assets/less/query_dois.less
 ckanext/query_dois/theme/assets/less/visual_query.less
 ckanext/query_dois/theme/assets/scripts/multisearch_download.js
```

### Comparing `ckanext-query-dois-3.0.5/docs/_scripts/gen_api_pages.py` & `ckanext-query-dois-4.0.0/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/pyproject.toml` & `ckanext-query-dois-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-query-dois"
-version = "3.0.5"
+version = "4.0.0"
 description = "A CKAN extension that creates DOIs for queries on resources."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -54,15 +54,15 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.query_dois.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "3.0.5"
+version = "4.0.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-query-dois-3.0.5/tests/unit/test_helpers.py` & `ckanext-query-dois-4.0.0/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/tests/unit/test_plugin.py` & `ckanext-query-dois-4.0.0/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-query-dois-3.0.5/tests/unit/test_utils.py` & `ckanext-query-dois-4.0.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

