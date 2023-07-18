# Comparing `tmp/ckanext-versioned-datastore-4.2.2.tar.gz` & `tmp/ckanext-versioned-datastore-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-versioned-datastore-4.2.2.tar", last modified: Mon Jul 17 08:28:42 2023, max compression
+gzip compressed data, was "ckanext-versioned-datastore-5.0.0.tar", last modified: Tue Jul 18 09:08:49 2023, max compression
```

## Comparing `ckanext-versioned-datastore-4.2.2.tar` & `ckanext-versioned-datastore-5.0.0.tar`

### file list

```diff
@@ -1,215 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16585 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/datastore_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.642268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    17480 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/servers/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/servers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/servers/direct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/queuing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/query_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/slug_words.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/slugs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/v1_0_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.646268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/basic_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    35737 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/multisearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/README
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/details.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/slugs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/download-status.less
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/search.less
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/slugerator.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/api.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.650268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.654268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/1.json
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/10.json
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/12.json
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/2.json
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/3.json
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/4.json
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/7.json
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/8.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/
--rw-r--r--   0 runner    (1001) docker     (123)  3183938 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson
--rw-r--r--   0 runner    (1001) docker     (123)  4137025 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson
--rw-r--r--   0 runner    (1001) docker     (123)  1316321 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json
--rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/resource_data.html
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/resource_edit_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/slugerator.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.662268 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/status/
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/status/download.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 08:28:42.000000 ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/helpers/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/helpers/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/helpers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/integration/downloads/
--rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/integration/downloads/test_downloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/
--rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_notifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_runmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/importing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/importing/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/importing/ingestion/test_ingestion_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/test_query_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/test_query_v1_0_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/lib/test_datastore_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.638268 ckanext-versioned-datastore-4.2.2/tests/unit/logic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:28:42.666268 ckanext-versioned-datastore-4.2.2/tests/unit/logic/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/logic/actions/test_actions_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-17 08:28:31.000000 ckanext-versioned-datastore-4.2.2/tests/unit/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.204766 ckanext-versioned-datastore-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-18 09:08:49.204766 ckanext-versioned-datastore-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16360 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.176766 ckanext-versioned-datastore-5.0.0/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.176766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.176766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.176766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/basic_query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/basic_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/basic_query/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/basic_query/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/basic_query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/datastore_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.176766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.176766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.176766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.180766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/notifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/notifiers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/notifiers/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.180766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/servers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/servers/direct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.180766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.180766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.180766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/queuing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.184766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/query_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16045 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/slug_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/v1_0_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.184766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.184766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/basic_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.184766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36112 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/meta/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/meta/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/multisearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.184766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.184766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/versions/526b12c69d55_add_navigational_slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/versions/d2ca5da0573f_add_server_args_to_download_request_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.184766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/model/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/model/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/model/slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/model/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.184766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/routes/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/routes/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/routes/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/routes/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.188766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.188766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/less/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/less/download-popup.less
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/less/download-status.less
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/less/search.less
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/less/slugerator.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.188766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/scripts/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/scripts/modules/download-button.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.188766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/scripts/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.188766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/api.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.188766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.188766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/12.json
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/8.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)  3183938 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)  4137025 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)  1316321 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/ajax_snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/ajax_snippets/download_popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/resource_data.html
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/resource_edit_base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/search/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/search/slugerator.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/status/download.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/versioned_datastore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/versioned_datastore/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/versioned_datastore/snippets/download_button.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17386 2023-07-18 09:08:49.000000 ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-07-18 09:08:49.000000 ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:08:49.000000 ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-18 09:08:49.000000 ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:08:48.000000 ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-18 09:08:49.000000 ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 09:08:49.000000 ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:08:49.204766 ckanext-versioned-datastore-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/helpers/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/helpers/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/helpers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/tests/integration/downloads/
+-rw-r--r--   0 runner    (1001) docker     (123)    21716 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/integration/downloads/test_downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/tests/unit/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.200766 ckanext-versioned-datastore-5.0.0/tests/unit/lib/basic_query/
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/basic_query/test_basic_query_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/basic_query/test_basic_query_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/basic_query/test_basic_query_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.204766 ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.204766 ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/test_downloads_notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/test_downloads_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/test_downloads_runmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/test_downloads_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/tests/unit/lib/importing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.204766 ckanext-versioned-datastore-5.0.0/tests/unit/lib/importing/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/importing/ingestion/test_ingestion_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.204766 ckanext-versioned-datastore-5.0.0/tests/unit/lib/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/query/test_query_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/query/test_query_v1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/lib/test_datastore_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.172766 ckanext-versioned-datastore-5.0.0/tests/unit/logic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:08:49.204766 ckanext-versioned-datastore-5.0.0/tests/unit/logic/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/logic/actions/test_actions_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-18 09:08:37.000000 ckanext-versioned-datastore-5.0.0/tests/unit/test_helpers.py
```

### Comparing `ckanext-versioned-datastore-4.2.2/LICENSE` & `ckanext-versioned-datastore-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/PKG-INFO` & `ckanext-versioned-datastore-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-datastore
-Version: 4.2.2
+Version: 5.0.0
 Summary: A CKAN extension providing a versioned datastore using MongoDB and Elasticsearch
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_datastore
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-versioned-datastore-4.2.2/README.md` & `ckanext-versioned-datastore-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/cli.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/helpers.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from ckan.plugins import toolkit
 from datetime import date
 
 from .lib.common import ALL_FORMATS
 from .lib.importing import stats
+from .lib.query.slugs import create_nav_slug
 
 
 def is_duplicate_ingestion(stat):
     """
     Detects whether the error message on this ImportStats object is a
     DuplicateDataSource error message or not. This is based on the error containing the
     phrase "this file has been ingested before" and is therefore a quite fragile, but
@@ -146,7 +147,19 @@
     )
     data_dict = {'resource_id': resource_id}
     if record_id:
         data_dict['id'] = record_id
 
     versions = toolkit.get_action(action)({}, data_dict)
     return versions[-1]
+
+
+def nav_slug(
+    query=None, version=None, resource_ids=None, resource_ids_and_versions=None
+):
+    """
+    Just a helper proxy for create_nav_slug.
+    """
+    is_new, slug = create_nav_slug(
+        {}, query or {}, version, resource_ids, resource_ids_and_versions
+    )
+    return slug.get_slug_string()
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/interfaces.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,14 +210,36 @@
         datastore_multisearch action before it is returned.
 
         :param response: the dict to be returned to the caller
         :return: the response dict
         """
         return response
 
+    def datastore_before_convert_basic_query(self, basic_query):
+        """
+        Allows plugins to modify a basic query (probably taken from a URL), e.g. to
+        remove custom filters before processing.
+
+        :param basic_query: the query dict to be modified
+        :return: the modified query
+        """
+        return basic_query
+
+    def datastore_after_convert_basic_query(self, basic_query, multisearch_query):
+        """
+        Allows plugins to modify a converted query, e.g. to add back in any complex
+        custom filters.
+
+        :param basic_query: the original basic query, before it was modified by other
+                            plugins
+        :param multisearch_query: the converted multisearch version of the query
+        :return: the modified multisearch query
+        """
+        return multisearch_query
+
 
 class IVersionedDatastoreQuerySchema(interfaces.Interface):
     def get_query_schemas(self):
         """
         Hook to allow registering custom query schemas.
 
         :return: a list of tuples of the format (query schema version, schema object)
@@ -357,14 +379,25 @@
 
         :param manifest: the manifest dict
         :param request: the DownloadRequest object
         :return: the manifest dict
         """
         return manifest
 
+    def download_modify_eml(self, eml_dict, query):
+        """
+        Hook allowing other extensions to modify the content of the EML before it's
+        transformed into XML and written to file.
+
+        :param eml_dict: the current eml content, as a dict
+        :param query: the query for this download
+        :return: the modified eml dict
+        """
+        return eml_dict
+
     def download_after_run(self, request):
         """
         Hook notifying that a download has finished (whether failed or completed). Does
         not allow modification; purely for notification purposes.
 
         :param request: the DownloadRequest object
         :return: None
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/geo.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/basic_query/geo.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/search.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/basic_query/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/basic_query/utils.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/basic_query/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from ckan.lib.search import SearchIndexError
-from splitgill.indexing.utils import DOC_TYPE
-from splitgill.search import create_version_query
+import copy
+import json
 from elasticsearch import NotFoundError
 from elasticsearch_dsl import MultiSearch, Search
+from splitgill.indexing.utils import DOC_TYPE
+from splitgill.search import create_version_query
 
+from ckan.lib.search import SearchIndexError
+from ckan.plugins import PluginImplementations
 from .. import common
 from ..datastore_utils import prefix_resource, prefix_field
 from ..importing.details import get_all_details
+from ...interfaces import IVersionedDatastore
 
 
 def run_search(search, indexes, version=None):
     """
     Convenience function to runs a search on the given indexes using the client
     available in this module.
 
@@ -180,7 +184,60 @@
                     }
                 )
 
     # stick the result in the cache for next time
     field_cache[cache_key] = (mapping, fields)
 
     return mapping, fields
+
+
+def convert_to_multisearch(query):
+    # save a copy of the original query
+    basic_query = copy.deepcopy(query)
+    multisearch_query = {}
+
+    # allow other plugins to modify the query before processing, e.g. to remove any
+    # custom filters
+    for plugin in PluginImplementations(IVersionedDatastore):
+        query = plugin.datastore_before_convert_basic_query(query)
+
+    if 'q' in query:
+        multisearch_query['search'] = query['q']
+
+    if 'filters' in query:
+        filter_list = []
+        for field, values in query['filters'].items():
+            if not isinstance(values, list):
+                values = [values]
+            if field == '__geo__':
+                for value in values:
+                    if isinstance(value, str):
+                        value = json.loads(value)
+                    if value['type'] == 'Polygon':
+                        filter_list.append({'geo_custom_area': [value['coordinates']]})
+                    else:
+                        # I cannot find any examples of anything other than polygons, so
+                        # I'm not sure it was ever implemented for the old searches
+                        raise NotImplemented
+            else:
+                subgroup = []
+                subgroup_count = 0
+                for value in values:
+                    if field != '' and value != '':
+                        subgroup.append(
+                            {'string_equals': {'fields': [field], 'value': value}}
+                        )
+                        subgroup_count += 1
+                if subgroup_count > 1:
+                    filter_list.append({'or': subgroup})
+                elif subgroup_count == 1:
+                    filter_list += subgroup
+        multisearch_query['filters'] = {'and': filter_list}
+
+    # allow plugins to modify the output, with the additional context of the original
+    # basic query
+    for plugin in PluginImplementations(IVersionedDatastore):
+        multisearch_query = plugin.datastore_after_convert_basic_query(
+            basic_query, multisearch_query
+        )
+
+    return multisearch_query
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/common.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
 # global variables to hold the splitgill config (not the CKAN one), the splitgill search helper object and
 # an elasticsearch client object
 CONFIG = None
 SEARCH_HELPER = None
 ES_CLIENT = None
 
+NON_DATASTORE_VERSION = -1
+
 
 def setup(ckan_config):
     """
     Given the CKAN config, setup the plugin's global variables.
 
     :param ckan_config: the ckan config
     """
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/datastore_utils.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/datastore_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/base.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/csv.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import shutil
 from collections import OrderedDict
 from datetime import datetime as dt
 from uuid import uuid4
 
 from lxml import etree
 
-from ckan.plugins import toolkit, plugin_loaded
+from ckan.plugins import toolkit, plugin_loaded, PluginImplementations
 from . import urls, utils
 from .schema import Schema
 from ..base import BaseDerivativeGenerator
+from .....interfaces import IVersionedDatastoreDownloads
 
 
 class DwcDerivativeGenerator(BaseDerivativeGenerator):
     name = 'dwc'
     extension = 'zip'
 
     def __init__(
@@ -75,19 +76,16 @@
             schema_args['extension_urls'] = ext_urls
         self.schema = Schema.load(
             toolkit.config.get('ckanext.versioned_datastore.dwc_schema_cache'),
             **schema_args,
         )
 
         # set up file paths & divide fields between core/extensions
-        self.file_paths = {
-            'core': os.path.join(
-                self._build_dir, f'{self.schema.row_type_name.lower()}.csv'
-            )
-        }
+        self._core_file_name = f'{self.schema.row_type_name.lower()}.csv'
+        self.file_paths = {'core': os.path.join(self._build_dir, self._core_file_name)}
         root_field_names = set([f.split('.')[0] for f in self.all_fields])
         all_ext_field_names = [
             item for ext in self.schema.extensions for item in ext.location.fields
         ]
         dataset_fields = [
             f
             for f in root_field_names
@@ -241,15 +239,15 @@
             'ignoreHeaderLines': '1',
         }
         core = etree.SubElement(
             root, 'core', rowType=self.schema.row_type, **attributes
         )
         core_files = etree.SubElement(core, 'files')
         core_files_location = etree.SubElement(core_files, 'location')
-        core_files_location.text = self.file_paths['core']
+        core_files_location.text = self._core_file_name
         etree.SubElement(core, 'id', index='0')
         for i, c in enumerate(self.writers['core'].fieldnames):
             if c == '_id':
                 continue
             prop = self.schema.props.get(c)
             if prop is None:
                 continue
@@ -332,14 +330,25 @@
                 'language': utils.get_setting('ckan.locale_default'),
                 'abstract': {
                     'para': f'Query ID {self._query.hash} on {site_name} ({self.rows_written} records).'
                 },
                 'keywordSet': [],
                 'intellectualRights': {'para': query_license},
                 'distribution': ({'online': {'url': site_url}}, {'scope': 'document'}),
+                'coverage': {
+                    'geographicCoverage': {
+                        'geographicDescription': 'Unbound',
+                        'boundingCoordinates': {
+                            'westBoundingCoordinates': -180,
+                            'eastBoundingCoordinates': 180,
+                            'northBoundingCoordinates': -90,
+                            'southBoundingCoordinates': 90,
+                        },
+                    }
+                },
                 'contact': [org],
             }
         )
         additional_metadata = {
             'metadata': {
                 'gbif': {
                     'dateStamp': dt.now().strftime('%Y-%m-%dT%H:%M:%SZ'),
@@ -438,14 +447,17 @@
                             'surName': c['agent']['family_name'],
                         }
                     else:
                         agent['organizationName'] = c['agent']['name']
                     dataset_metadata['creator'].append(agent)
                     authors.append(c['agent']['id'])
 
+        for plugin in PluginImplementations(IVersionedDatastoreDownloads):
+            dataset_metadata = plugin.download_modify_eml(dataset_metadata, self._query)
+
         nsmap = utils.NSMap(
             eml=urls.XMLUrls.eml,
             dc=urls.XMLUrls.dc,
             xsi=urls.XMLUrls.xsi,
             xml=urls.XMLUrls.xml,
         )
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/schema_parts.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/urls.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/dwc/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 node.append(n)
         return [node]
     elif isinstance(content, list):
         nodes = [item for e in content for item in json_to_xml(tag, e)]
         return nodes
     else:
         node = etree.Element(tag, **attrs)
-        node.text = content
+        node.text = str(content)
         return [node]
 
 
 def get_setting(*config_names, default=None):
     setting = None
     for c in config_names:
         setting = toolkit.config.get(c)
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/json.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/json.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/derivatives/xlsx.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/download.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/download.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+import os.path
+from collections import defaultdict
+
+import fastavro
 import hashlib
 import json
 import os
-import os.path
+import shutil
 import tempfile
 import zipfile
-from collections import defaultdict
 from datetime import datetime as dt
+from elasticsearch_dsl import Search
 from functools import partial
 from glob import iglob
-import shutil
-
-import fastavro
-from ckan.plugins import toolkit, PluginImplementations
-from elasticsearch_dsl import Search
 from splitgill.indexing.utils import get_elasticsearch_client
 from splitgill.search import create_version_query
 
+from ckan.lib import uploader
+from ckan.plugins import toolkit, PluginImplementations
 from .loaders import (
     get_derivative_generator,
     get_file_server,
     get_notifier,
     get_transformation,
 )
 from .query import Query
@@ -33,40 +34,69 @@
 
 
 class DownloadRunManager:
     download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
     if download_dir is None:
         raise Exception('ckanext.versioned_datastore.download_dir must be set.')
     core_dir = os.path.join(download_dir, 'core')
+    custom_dir = toolkit.config.get(
+        'ckanext.versioned_datastore.custom_dir', os.path.join(download_dir, 'custom')
+    )
 
     def __init__(self, query_args, derivative_args, server_args, notifier_args):
         # allow plugins to make changes to the args
         for plugin in PluginImplementations(IVersionedDatastoreDownloads):
             (
                 query_args,
                 derivative_args,
                 server_args,
                 notifier_args,
             ) = plugin.download_before_run(
                 query_args, derivative_args, server_args, notifier_args
             )
 
-        self.query = Query.from_query_args(query_args)
+        if derivative_args.format == 'raw':
+            # if we're serving raw files then we're not doing any transformations
+            derivative_args.separate_files = True
+            derivative_args.ignore_empty_fields = False
+            derivative_args.transform = {}
+            # we also can't use a query
+            query_args.query = {}
+            query_args.slug_or_doi = None
+            # resource versions will always be the latest version
+            query_args.resource_ids = query_args.resource_ids or list(
+                query_args.resource_ids_and_versions.keys()
+            )
+            query_args.resource_ids_and_versions = None
+
+        self.allow_non_datastore = (
+            derivative_args.format == 'raw'
+            and derivative_args.format_args.get('allow_non_datastore', False)
+        )
+        self.query = Query.from_query_args(
+            query_args, allow_non_datastore=self.allow_non_datastore
+        )
         self.derivative_options = derivative_args
         for field, default_value in DerivativeArgs.defaults.items():
             if getattr(self.derivative_options, field) is None:
                 setattr(self.derivative_options, field, default_value)
-        self.server = get_file_server(server_args.type, **server_args.type_args)
+        self.server = get_file_server(
+            server_args.type,
+            filename=server_args.custom_filename,
+            **server_args.type_args,
+        )
 
         # initialise core and derivative records
         self.core_record, self.derivative_record = self.check_for_records()
 
         # initialises a log entry in the database
         self.request = DownloadRequest(
-            core_id=self.core_record.id, derivative_id=self.derivative_record.id
+            core_id=self.core_record.id,
+            derivative_id=self.derivative_record.id,
+            server_args={f: getattr(server_args, f) for f in server_args.fields},
         )
         self.request.save()
 
         self.notifier = get_notifier(
             notifier_args.type, request=self.request, **notifier_args.type_args
         )
 
@@ -113,14 +143,17 @@
             # different session (the __init__ is run by the main ckan process,
             # this is run by the download worker)
             self.request = DownloadRequest.get(self.request.id)
             self.core_record = CoreFileRecord.get(self.core_record.id)
             self.derivative_record = DerivativeFileRecord.get(self.derivative_record.id)
 
             # generate core file if needed
+            # technically we don't need core files if the format is 'raw', but we'll
+            # generate them anyway for consistency/avoidance of thousands of ifs, and
+            # also so we have some field metadata
             self.generate_core()
 
             # generate derivative file if needed
             self.generate_derivative()
 
             # finish up
             self.request.update_status(DownloadRequest.state_complete)
@@ -159,16 +192,21 @@
             os.mkdir(self.core_dir)
 
         # initialise empty variables
         core_record = None
         derivative_record = None
 
         # search for derivative first
-        fn = f'*_{self.hash}.zip'
-        existing_file = next(iglob(os.path.join(self.download_dir, fn)), None)
+        fp = os.path.join(self.download_dir, f'{self.hash}.zip')
+        if os.path.exists(fp):
+            existing_file = fp
+        else:
+            # check old-style names with the request id in front as well
+            fn = f'*_{self.hash}.zip'
+            existing_file = next(iglob(os.path.join(self.download_dir, fn)), None)
         if existing_file is not None:
             # could return multiple options, sorted by most recent first
             possible_records = DerivativeFileRecord.get_by_filepath(existing_file)
             if possible_records:
                 # use the most recent one
                 derivative_record = possible_records[0]
                 core_record = derivative_record.core_record
@@ -222,25 +260,26 @@
 
         # check if there are new resources to generate
         existing_files = os.listdir(self.core_folder_path)
         resources_to_generate = {
             rid: v
             for rid, v in self.query.resource_ids_and_versions.items()
             if f'{rid}_{v}.avro' not in existing_files
+            and v != common.NON_DATASTORE_VERSION
         }
 
         resource_totals = {k: None for k in self.core_record.resource_ids_and_versions}
         field_counts = {k: None for k in self.core_record.resource_ids_and_versions}
 
         # get info for resources that weren't just generated first, so we know if they
         # need regenerating
         existing_resources = [
             k
-            for k in self.query.resource_ids_and_versions
-            if k not in resources_to_generate
+            for k, v in self.query.resource_ids_and_versions.items()
+            if k not in resources_to_generate and v != common.NON_DATASTORE_VERSION
         ]
         for resource_id in existing_resources:
             # find a matching core record
             record = CoreFileRecord.find_resource(
                 self.query.hash,
                 resource_id,
                 self.query.resource_ids_and_versions[resource_id],
@@ -302,14 +341,23 @@
                     resource_totals[resource_id] += 1
                     chunk.append(data)
                     if len(chunk) == chunk_size:
                         _flush(chunk)
                         chunk = []
                 _flush(chunk)
 
+        non_datastore_resources = [
+            k
+            for k, v in self.query.resource_ids_and_versions.items()
+            if v == common.NON_DATASTORE_VERSION
+        ]
+        for resource_id in non_datastore_resources:
+            resource_totals[resource_id] = 1
+            field_counts[resource_id] = {}
+
         self.core_record.update(
             resource_totals=resource_totals,
             total=sum(resource_totals.values()),
             field_counts=field_counts,
         )
 
         return self.core_record
@@ -320,134 +368,184 @@
 
         :return:
         """
 
         self.request.update_status(DownloadRequest.state_derivative_gen)
 
         if self.derivative_record.filepath is None:
-            zip_name = f'{self.request.id}_{self.hash}.zip'
+            # if this _is_ defined, we don't need to generate the file
+            zip_name = f'{self.hash}.zip'
             zip_path = os.path.join(self.download_dir, zip_name)
 
             self.derivative_record.update(filepath=zip_path)
-        else:
-            # we don't want to proceed with the rest of the generation
-            return self.derivative_record
-
-        # for keeping track of elapsed generation time
-        start = dt.utcnow()
-        # for storing build files
-        temp_dir = tempfile.mkdtemp()
-        self._temp.append(temp_dir)
-
-        manifest = {
-            'download_id': self.request.id,
-            'resources': {},
-            'separate_files': self.derivative_options.separate_files,
-            'file_format': self.derivative_options.format,
-            'format_args': self.derivative_options.format_args,
-            'ignore_empty_fields': self.derivative_options.ignore_empty_fields,
-            'transform': self.derivative_options.transform,
-            'total_records': self.core_record.total,
-            'start': start.isoformat(),
-            # these get filled in later but we'll initialise them here
-            'files': [],
-            'end': None,
-            'duration_in_seconds': 0,
-        }
 
-        # set up the derivative generators; each generator creates one component.
-        # components = individual file groups within the main zip, e.g. one CSV for each
-        # resource (multiple components), or multiple files comprising a single DarwinCore
-        # archive (single component)
-        fields = partial(
-            get_fields,
-            self.core_record.field_counts,
-            self.derivative_options.ignore_empty_fields,
-        )
-        if self.derivative_options.separate_files:
-            components = {
-                rid: get_derivative_generator(
-                    self.derivative_options.format,
-                    output_dir=temp_dir,
-                    fields=fields(resource_id=rid),
-                    resource_id=rid,
-                    query=self.query,
-                    **self.derivative_options.format_args,
-                )
-                for rid in self.query.resource_ids_and_versions
+            # for keeping track of elapsed generation time
+            start = dt.utcnow()
+            # for storing build files
+            temp_dir = tempfile.mkdtemp()
+            self._temp.append(temp_dir)
+
+            manifest = {
+                'download_id': self.request.id,
+                'resources': {},
+                'separate_files': self.derivative_options.separate_files,
+                'file_format': self.derivative_options.format,
+                'format_args': self.derivative_options.format_args,
+                'ignore_empty_fields': self.derivative_options.ignore_empty_fields,
+                'transform': self.derivative_options.transform,
+                'total_records': self.core_record.total,
+                'start': start.isoformat(),
+                # these get filled in later but we'll initialise them here
+                'files': [],
+                'end': None,
+                'duration_in_seconds': 0,
             }
-        else:
-            gen = get_derivative_generator(
-                self.derivative_options.format,
-                output_dir=temp_dir,
-                fields=fields(),
-                query=self.query,
-                **self.derivative_options.format_args,
-            )
-            components = defaultdict(lambda: gen)
-
-        # load transformation functions
-        transformations = [
-            get_transformation(t, **targs)
-            for t, targs in (self.derivative_options.transform or {}).items()
-        ]
 
-        for resource_id, version in self.query.resource_ids_and_versions.items():
-            # add the resource ID as the message for use in the status page
-            self.request.update_status(
-                DownloadRequest.state_derivative_gen, resource_id
-            )
-            if (
-                len(self.query.resource_ids_and_versions) > 1
-                and self.core_record.resource_totals[resource_id] == 0
-            ):
-                # don't generate empty files unless there's only one resource
-                continue
-            derivative_generator = components[resource_id]
-            core_file_path = os.path.join(
-                self.core_folder_path, f'{resource_id}_{version}.avro'
-            )
-            with derivative_generator, open(core_file_path, 'rb') as core_file:
-                for record in fastavro.reader(core_file):
-                    # apply the transformations first
-                    for transform in transformations:
-                        record = transform(record)
-                    # filter out fields that are empty for all records
-                    if self.derivative_options.ignore_empty_fields:
-                        record = filter_data_fields(
-                            record, self.core_record.field_counts[resource_id]
+            if self.derivative_options.format != 'raw':
+                # set up the derivative generators; each generator creates one component.
+                # components = individual file groups within the main zip, e.g. one CSV for each
+                # resource (multiple components), or multiple files comprising a single DarwinCore
+                # archive (single component)
+                fields = partial(
+                    get_fields,
+                    self.core_record.field_counts,
+                    self.derivative_options.ignore_empty_fields,
+                )
+                if self.derivative_options.separate_files:
+                    components = {
+                        rid: get_derivative_generator(
+                            self.derivative_options.format,
+                            output_dir=temp_dir,
+                            fields=fields(resource_id=rid),
+                            resource_id=rid,
+                            query=self.query,
+                            **self.derivative_options.format_args,
                         )
-                    # then write the record
-                    derivative_generator.write(record)
+                        for rid in self.query.resource_ids_and_versions
+                    }
+                else:
+                    gen = get_derivative_generator(
+                        self.derivative_options.format,
+                        output_dir=temp_dir,
+                        fields=fields(),
+                        query=self.query,
+                        **self.derivative_options.format_args,
+                    )
+                    components = defaultdict(lambda: gen)
+
+                # load transformation functions
+                transformations = [
+                    get_transformation(t, **targs)
+                    for t, targs in (self.derivative_options.transform or {}).items()
+                ]
+
+                for (
+                    resource_id,
+                    version,
+                ) in self.query.resource_ids_and_versions.items():
+                    # add the resource ID as the message for use in the status page
+                    self.request.update_status(
+                        DownloadRequest.state_derivative_gen, resource_id
+                    )
+                    if (
+                        len(self.query.resource_ids_and_versions) > 1
+                        and self.core_record.resource_totals[resource_id] == 0
+                    ):
+                        # don't generate empty files unless there's only one resource
+                        continue
+                    derivative_generator = components[resource_id]
+                    core_file_path = os.path.join(
+                        self.core_folder_path, f'{resource_id}_{version}.avro'
+                    )
+                    with derivative_generator, open(core_file_path, 'rb') as core_file:
+                        for record in fastavro.reader(core_file):
+                            # apply the transformations first
+                            for transform in transformations:
+                                record = transform(record)
+                            # filter out fields that are empty for all records
+                            if self.derivative_options.ignore_empty_fields:
+                                record = filter_data_fields(
+                                    record, self.core_record.field_counts[resource_id]
+                                )
+                            # then write the record
+                            derivative_generator.write(record)
+
+                if self.derivative_options.separate_files:
+                    for generator in components.values():
+                        generator.cleanup()
+                else:
+                    components.default_factory().cleanup()
 
-        if self.derivative_options.separate_files:
-            for generator in components.values():
-                generator.cleanup()
-        else:
-            components.default_factory().cleanup()
+            else:
+                resource_show = toolkit.get_action('resource_show')
+                for (
+                    resource_id,
+                    version,
+                ) in self.query.resource_ids_and_versions.items():
+                    self.request.update_status(
+                        DownloadRequest.state_derivative_gen, resource_id
+                    )
+                    res = resource_show({}, {'id': resource_id})
+                    if res.get('url_type') == 'upload':
+                        upload = uploader.get_resource_uploader(res)
+                        if not upload.storage_path:
+                            # if ckan.storage_path is not set
+                            raise Exception('Non-datastore uploads are not configured.')
+                        filepath = upload.get_path(res['id'])
+                        original_filename = res.get('url', '').split('/')[-1]
+                        fileext = (
+                            os.path.splitext(original_filename)[-1].strip('.')
+                            or res['format'].lower()
+                        )
+                        filename = os.path.extsep.join([resource_id, fileext])
+                        shutil.copy2(filepath, os.path.join(temp_dir, filename))
+                    else:
+                        raise NotImplemented(
+                            f'No raw file is available for resource {resource_id}'
+                        )
 
-        # generation finished
-        self.request.update_status(DownloadRequest.state_packaging)
+            # generation finished
+            self.request.update_status(DownloadRequest.state_packaging)
 
-        end = dt.utcnow()
-        manifest['end'] = end.isoformat()
+            end = dt.utcnow()
+            manifest['end'] = end.isoformat()
 
-        duration = (end - start).total_seconds()
-        manifest['duration_in_seconds'] = duration
+            duration = (end - start).total_seconds()
+            manifest['duration_in_seconds'] = duration
 
-        files_to_zip = os.listdir(temp_dir) + ['manifest.json']
-        manifest['files'] = files_to_zip
+            files_to_zip = os.listdir(temp_dir) + ['manifest.json']
+            manifest['files'] = files_to_zip
 
-        # allow plugins to make changes
-        for plugin in PluginImplementations(IVersionedDatastoreDownloads):
-            manifest = plugin.download_modify_manifest(manifest, self.request)
+            # allow plugins to make changes
+            for plugin in PluginImplementations(IVersionedDatastoreDownloads):
+                manifest = plugin.download_modify_manifest(manifest, self.request)
 
-        # write out manifest
-        with open(os.path.join(temp_dir, 'manifest.json'), 'w', encoding='utf8') as f:
-            json.dump(manifest, f, sort_keys=True, indent=2, ensure_ascii=False)
-
-        # zip everything up
-        with zipfile.ZipFile(zip_path, 'w', zipfile.ZIP_DEFLATED, True) as z:
-            for filename in files_to_zip:
-                z.write(os.path.join(temp_dir, filename), arcname=filename)
+            # write out manifest
+            with open(
+                os.path.join(temp_dir, 'manifest.json'), 'w', encoding='utf8'
+            ) as f:
+                json.dump(manifest, f, sort_keys=True, indent=2, ensure_ascii=False)
+
+            # zip everything up
+            with zipfile.ZipFile(zip_path, 'w', zipfile.ZIP_DEFLATED, True) as z:
+                for filename in files_to_zip:
+                    z.write(os.path.join(temp_dir, filename), arcname=filename)
+
+        # auth checks should have already been done, so this should have been removed
+        # if not allowed
+        if self.server.filename:
+            # ensure the custom dir exists
+            if not os.path.exists(self.custom_dir):
+                os.mkdir(self.custom_dir)
+            symlink_path = os.path.join(self.custom_dir, f'{self.server.filename}.zip')
+            if (
+                os.path.islink(symlink_path)
+                and os.path.realpath(symlink_path) != self.derivative_record.filepath
+            ):
+                # this should only be being used by admins, so we assume it's okay to
+                # overwrite old symlinks
+                os.remove(symlink_path)
+            # test it again and create if necessary
+            if not os.path.islink(symlink_path):
+                os.symlink(self.derivative_record.filepath, symlink_path)
 
         return self.derivative_record
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/loaders.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/loaders.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/base.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/email.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/transforms/id_as_url.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/downloads/utils.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/downloads/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from elasticsearch import Elasticsearch
 from elasticsearch_dsl import Search, A
 from fastavro import parse_schema
 from splitgill.search import create_version_query
 
 from .query import Query
+from .. import common
 from ..datastore_utils import (
     prefix_resource,
     prefix_field,
     iter_data_fields,
     unprefix_index,
 )
 
@@ -18,15 +19,19 @@
 
     :param query: the Query object for this request
     :param es_client: a connected elasticsearch client
     :return: a parsed avro schema
     """
     resource_mapping = es_client.indices.get_mapping(
         index=','.join(
-            [prefix_resource(r) for r in query.resource_ids_and_versions.keys()]
+            [
+                prefix_resource(r)
+                for r, v in query.resource_ids_and_versions.items()
+                if v != common.NON_DATASTORE_VERSION
+            ]
         )
     )
 
     basic_avro_types = [
         'null',
         'boolean',
         'int',
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/details.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/details.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/importing.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/importing.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/indexing.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/indexing.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/deletion.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/exceptions.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/ingesting.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/readers.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/readers.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/records.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/records.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/ingestion/utils.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/ingestion/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/queuing.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/queuing.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/stats.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/stats.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/importing/utils.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/importing/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/fields.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/fields.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/query_log.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/query_log.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/schema.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/slug_words.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/slug_words.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/slugs.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/slugs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import datetime
 import hashlib
 import random
+import logging
 
 from ckan import model
 from ckan.plugins import toolkit
 from sqlalchemy.exc import IntegrityError
 
 from .schema import get_latest_query_version, hash_query
 from .schema import validate_query
 from .slug_words import list_one, list_two, list_three
-from .utils import get_available_datastore_resources
-from ...model.slugs import DatastoreSlug
+from .utils import get_available_datastore_resources, get_resources_and_versions
+from ...model.slugs import DatastoreSlug, NavigationalSlug
+
+log = logging.getLogger(__name__)
 
 
 def generate_query_hash(
     query, query_version, version, resource_ids, resource_ids_and_versions
 ):
     """
     Given a query and the parameters required to run it, create a unique id for it (a
@@ -91,20 +95,17 @@
     :return: a 2-tuple containing a boolean indicating whether the slug object returned was newly
              created and the DatastoreSlug object itself. If we couldn't create a slug object for
              some reason then (False, None) is returned.
     """
     # only store valid queries!
     validate_query(query, query_version)
 
-    if resource_ids:
-        resource_ids = list(get_available_datastore_resources(context, resource_ids))
-        if not resource_ids:
-            raise toolkit.ValidationError(
-                u"The requested resources aren't accessible to this user"
-            )
+    resource_ids, resource_ids_and_versions = get_resources_and_versions(
+        resource_ids, resource_ids_and_versions, version
+    )
 
     query_hash = generate_query_hash(
         query, query_version, version, resource_ids, resource_ids_and_versions
     )
 
     existing_slug = (
         model.Session.query(DatastoreSlug)
@@ -142,21 +143,74 @@
                 raise
     else:
         return False, None
 
     return True, new_slug
 
 
-def resolve_slug(slug):
+def create_nav_slug(
+    context, query, version=None, resource_ids=None, resource_ids_and_versions=None
+):
+    try:
+        # clear old slugs before we make new ones
+        clean_nav_slugs()
+    except Exception as e:
+        # if it fails, log it and move on
+        log.debug(f'Cleaning nav slugs failed: {e}')
+
+    query_version = get_latest_query_version()  # it should always be the latest version
+    validate_query(query, query_version)
+
+    resource_ids, resource_ids_and_versions = get_resources_and_versions(
+        resource_ids, resource_ids_and_versions, version
+    )
+
+    query_hash = generate_query_hash(
+        query, query_version, version, resource_ids, resource_ids_and_versions
+    )
+
+    existing_slug = (
+        model.Session.query(NavigationalSlug)
+        .filter(NavigationalSlug.query_hash == query_hash)
+        .first()
+    )
+
+    if existing_slug is not None:
+        return False, existing_slug
+
+    new_slug = NavigationalSlug(
+        query_hash=query_hash,
+        query=query,
+        resource_ids_and_versions=resource_ids_and_versions,
+    )
+    new_slug.save()
+
+    return True, new_slug
+
+
+def resolve_slug(slug, allow_nav=True):
     """
     Resolves the given slug and returns it if it's found, otherwise None is returned.
 
     :param slug: the slug
+    :param allow_nav: allow resolving to a navigational slug
     :return: a DatastoreSlug object or None if the slug couldn't be found
     """
+    if slug.startswith(NavigationalSlug.prefix) and allow_nav:
+        try:
+            # clean old slugs because we don't want old ones to continue resolving
+            clean_nav_slugs()
+        except Exception as e:
+            # if it fails, log it and move on
+            log.debug(f'Cleaning nav slugs failed: {e}')
+        return (
+            model.Session.query(NavigationalSlug)
+            .filter(NavigationalSlug.on_slug(slug))
+            .first()
+        )
     return (
         model.Session.query(DatastoreSlug).filter(DatastoreSlug.on_slug(slug)).first()
     )
 
 
 class DuplicateSlugException(Exception):
     pass
@@ -205,15 +259,15 @@
     if version is not None:
         assert isinstance(version, int)
     if resource_ids is not None:
         assert isinstance(resource_ids, list)
     if resource_ids_and_versions is not None:
         assert isinstance(resource_ids_and_versions, dict)
 
-    slug = resolve_slug(reserved_pretty_slug)
+    slug = resolve_slug(reserved_pretty_slug, False)
     if slug is not None:
         # a slug with this reserved pretty slug already exists
         return slug
     else:
         # there is no slug associated with this reserved pretty slug so let's see if there's a slug
         # using the query parameters
         query_hash = generate_query_hash(
@@ -249,7 +303,32 @@
                 slug.save()
                 return slug
             else:
                 raise DuplicateSlugException(
                     f'The query parameters are already associated with a '
                     f'different slug: {slug.get_slug_string()}'
                 )
+
+
+def clean_nav_slugs(before=None):
+    """
+    Delete old/expired navigational slugs.
+
+    :param before: a datetime object; slugs created before this time will be removed
+                   (defaults to 2 days ago)
+    :return: the number of deleted slugs
+    """
+    if before is None:
+        before = datetime.datetime.utcnow() - datetime.timedelta(days=2)
+
+    old_slugs = (
+        model.Session.query(NavigationalSlug)
+        .filter(NavigationalSlug.created < before)
+        .all()
+    )
+    slug_count = len(old_slugs)
+    for slug in old_slugs:
+        slug.delete()
+
+    model.Session.commit()
+
+    return slug_count
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/utils.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from copy import copy
-
-from ckan import model
-from ckan.plugins import toolkit
 from datetime import datetime
+
+from elasticsearch_dsl import Search, MultiSearch
 from splitgill.search import create_version_query, create_index_specific_version_filter
 from splitgill.utils import to_timestamp
-from elasticsearch_dsl import Search, MultiSearch
 
+from ckan import model
+from ckan.plugins import toolkit
 from .. import common
 from ..datastore_utils import prefix_resource, get_last_after, trim_index_name
 
 
 def get_available_datastore_resources(context, only=None):
     """
     Returns a set of resource ids accessible to the current user based on the given
@@ -219,7 +219,80 @@
     multisearch = MultiSearch(using=common.ES_CLIENT).add(search_copy)
     result = next(iter(multisearch.execute()))
     return [
         trim_index_name(bucket['key'])
         for bucket in result.aggs.to_dict()['indexes']['buckets']
         if bucket['doc_count'] > 0
     ]
+
+
+def get_resources_and_versions(
+    resource_ids=None,
+    resource_ids_and_versions=None,
+    version=None,
+    allow_non_datastore=False,
+):
+    """
+    Get a list of resource ids and a dict of resource ids and versions from either, e.g.
+    get the list of resource ids from a resource id and version dict.
+
+    :param resource_ids: a list of resource ids
+    :param resource_ids_and_versions: a dict of resource id: resource version
+    :param version: a datestamp used as a default version for resources without a version
+    :param allow_non_datastore: allow non datastore resources to be included (will be
+                                returned with common.NON_DATASTORE_VERSION)
+    :return: a tuple of resource_ids, resource_ids_and_versions
+    """
+
+    if resource_ids_and_versions is None:
+        resource_ids_and_versions = {}
+    else:
+        # use the resource_ids_and_versions dict first over the resource_ids and version params
+        resource_ids = list(resource_ids_and_versions.keys())
+
+    # first see what's available from the datastore
+    available_resource_ids = list(get_available_datastore_resources({}, resource_ids))
+    if (not available_resource_ids) and (not allow_non_datastore):
+        raise toolkit.ValidationError(
+            "The requested resources aren't accessible to this user"
+        )
+
+    unavailable_resource_ids = [
+        rid for rid in resource_ids or [] if rid not in available_resource_ids
+    ]
+    non_datastore_resources = []
+
+    if allow_non_datastore:
+        resource_show = toolkit.get_action('resource_show')
+        for resource_id in unavailable_resource_ids:
+            resource = resource_show({}, {'id': resource_id})
+            # if we get nothing back there's probably an access issue; if it's a
+            # datastore resource something went wrong earlier
+            if resource and not resource['datastore_active']:
+                available_resource_ids.append(resource_id)
+                non_datastore_resources.append(resource_id)
+
+    rounded_resource_ids_and_versions = {}
+    # see if a version was provided; we'll use this if a resource id we're searching doesn't
+    # have a directly assigned version (i.e. it was absent from the resource_ids_and_versions
+    # dict, or that parameter wasn't provided)
+    if version is None:
+        version = to_timestamp(datetime.now())
+    for resource_id in available_resource_ids:
+        if resource_id in non_datastore_resources:
+            rounded_resource_ids_and_versions[
+                resource_id
+            ] = common.NON_DATASTORE_VERSION
+            continue
+        # try to get the target version from the passed resource_ids_and_versions dict, but if
+        # it's not in there, default to the version variable
+        target_version = resource_ids_and_versions.get(resource_id, version)
+        index = prefix_resource(resource_id)
+        # round the version down to ensure we search the exact version requested
+        rounded_version = common.SEARCH_HELPER.get_rounded_versions(
+            [index], target_version
+        )[index]
+        if rounded_version is not None:
+            # resource ids without a rounded version are skipped
+            rounded_resource_ids_and_versions[resource_id] = rounded_version
+
+    return available_resource_ids, rounded_resource_ids_and_versions
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/lib/query/v1_0_0.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/lib/query/v1_0_0.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/basic_search.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/basic_search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/crud.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/crud.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/extras.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/extras.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/meta/arg_objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from ckan.plugins import toolkit
-from ckanext.datastore.logic.schema import json_validator
 from ckantools.validators import list_of_strings
 from ckantools.validators.ivalidators import BaseArgs
 
+from ckan.plugins import toolkit
+from ckanext.datastore.logic.schema import json_validator
+
 # grab all the validator functions upfront
 boolean_validator = toolkit.get_validator('boolean_validator')
 ignore_missing = toolkit.get_validator('ignore_missing')
 int_validator = toolkit.get_validator('int_validator')
 not_missing = toolkit.get_validator('not_missing')
 not_empty = toolkit.get_validator('not_empty')
 resource_id_exists = toolkit.get_validator('resource_id_exists')
@@ -53,20 +54,28 @@
         'transform': {},
     }
 
 
 class ServerArgs(BaseArgs):
     type: str
     type_args: dict
+    custom_filename: str
 
-    fields = {'type': [not_missing, str], 'type_args': [ignore_missing, json_validator]}
+    fields = {
+        'type': [ignore_missing, str],
+        'type_args': [ignore_missing, json_validator],
+        'custom_filename': [ignore_missing, str],
+    }
 
     defaults = {'type': 'direct', 'type_args': {}}
 
 
 class NotifierArgs(BaseArgs):
     type: str
     type_args: dict
 
-    fields = {'type': [not_missing, str], 'type_args': [ignore_missing, json_validator]}
+    fields = {
+        'type': [ignore_missing, str],
+        'type_args': [ignore_missing, json_validator],
+    }
 
-    defaults = {'type': 'email', 'type_args': {}}
+    defaults = {'type': 'none', 'type_args': {}}
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/help.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/meta/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -631,14 +631,25 @@
 
 **Results:**
 
 :returns: details about the job that has been submitted to fulfill the upsert request.
 :rtype: dict
 '''
 
+datastore_regenerate_download = '''
+Calls datastore_queue_download to regenerate a previous request. Note that notifier args
+are still required as these are not stored in the original request, and server args may
+be specified to override any stored ones.
+
+**Results:**
+
+:returns: details about the job that has been submitted to fulfill the upsert request.
+:rtype: dict
+'''
+
 datastore_guess_fields = '''
 This action allows you to retrieve a set of fields to display by default for a given search across
 potentially multiple resources. The returned list of groups of fields is ordered by the number of
 resources the fields in each group appears in under the provided query. Ties are handled by ordering
 the group with the fields that appear in the most records first. If there is only one resource id
 passed then the groups returned are ordered in ingestion order, if available.
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/meta/schema.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/meta/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,15 @@
     return {
         'query': [ignore_missing, json_validator],
         'version': [ignore_missing, int_validator],
         'query_version': [ignore_missing, str],
         'resource_ids': [ignore_missing, list_of_strings()],
         'resource_ids_and_versions': [ignore_missing, json_validator],
         'pretty_slug': [ignore_missing, boolean_validator],
+        'nav_slug': [ignore_missing, boolean_validator],
     }
 
 
 def datastore_resolve_slug():
     return {
         'slug': [str],
     }
@@ -193,14 +194,22 @@
             object_validator(DerivativeArgs),
         ],  # called 'file' instead of derivative to make its purpose clearer to the end user
         'server': [ignore_missing, object_validator(ServerArgs)],
         'notifier': [ignore_missing, object_validator(NotifierArgs)],
     }
 
 
+def datastore_regenerate_download():
+    return {
+        'download_id': [not_missing, str],
+        'server': [ignore_missing, object_validator(ServerArgs)],
+        'notifier': [ignore_missing, object_validator(NotifierArgs)],
+    }
+
+
 def datastore_guess_fields():
     return {
         'query': [ignore_missing, json_validator],
         'query_version': [ignore_missing, str],
         'version': [ignore_missing, int_validator],
         'resource_ids': [ignore_missing, list_of_strings()],
         'resource_ids_and_versions': [ignore_missing, json_validator],
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/actions/multisearch.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/actions/multisearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from collections import defaultdict
 from datetime import datetime
 
 import jsonschema
-from ckan.plugins import toolkit, PluginImplementations, plugin_loaded
-from splitgill.utils import to_timestamp
+from ckantools.decorators import action
+from ckantools.timer import Timer
 from elasticsearch_dsl import MultiSearch, A
+from splitgill.utils import to_timestamp
 
+from ckan.plugins import toolkit, PluginImplementations, plugin_loaded
 from .meta import help, schema
-from ckantools.decorators import action
-from ckantools.timer import Timer
 from ...interfaces import IVersionedDatastore
 from ...lib import common
+from ...lib.basic_query.utils import convert_to_multisearch
 from ...lib.datastore_utils import (
     prefix_resource,
     unprefix_index,
     iter_data_fields,
     trim_index_name,
     prefix_field,
 )
@@ -28,15 +29,15 @@
 from ...lib.query.schema import (
     get_latest_query_version,
     InvalidQuerySchemaVersionError,
     validate_query,
     translate_query,
     hash_query,
 )
-from ...lib.query.slugs import create_slug, resolve_slug
+from ...lib.query.slugs import create_slug, resolve_slug, create_nav_slug
 from ...lib.query.utils import (
     get_available_datastore_resources,
     determine_resources_to_search,
     determine_version_filter,
     calculate_after,
     find_searched_resources,
 )
@@ -195,14 +196,15 @@
     context,
     query=None,
     query_version=None,
     version=None,
     resource_ids=None,
     resource_ids_and_versions=None,
     pretty_slug=True,
+    nav_slug=False,
 ):
     """
     Creates a slug for the given multisearch parameters and returns it. This slug can be
     used, along with the resolve_slug action, to retrieve, at any point after the slug
     is created, the query parameters passed to this action. The slug is unique for the
     given query parameters and passing the same query parameters again at a later point
     will result in the same slug being returned.
@@ -220,41 +222,54 @@
                                       parameter. If None (default) then the resource_ids parameter
                                       is used together with the version parameter. If this parameter
                                       is provided though, it takes priority over the resource_ids
                                       and version parameters.
     :param pretty_slug: whether to produce a "pretty" slug or not. If True (the default) a selection
                         of 2 adjectives and an animal will be used to create the slug, otherwise if
                         False, a uuid will be used
+    :param nav_slug: if this is True, a temporary navigational slug will be produced
+                     instead of a standard slug
     :return: a dict containing the slug and whether it was created during this function call or not
     """
     if query is None:
         query = {}
+    if query_version and query_version.lower().startswith('v0'):
+        # this is an old/basic query so we need to convert it first
+        query = convert_to_multisearch(query)
+        query_version = None
     if query_version is None:
         query_version = get_latest_query_version()
 
     try:
-        is_new, slug = create_slug(
-            context,
-            query,
-            query_version,
-            version,
-            resource_ids,
-            resource_ids_and_versions,
-            pretty_slug=pretty_slug,
-        )
+        if nav_slug:
+            is_new, slug = create_nav_slug(
+                context, query, version, resource_ids, resource_ids_and_versions
+            )
+        else:
+            is_new, slug = create_slug(
+                context,
+                query,
+                query_version,
+                version,
+                resource_ids,
+                resource_ids_and_versions,
+                pretty_slug=pretty_slug,
+            )
     except (jsonschema.ValidationError, InvalidQuerySchemaVersionError) as e:
         raise toolkit.ValidationError(e.message)
 
     if slug is None:
         raise toolkit.ValidationError('Failed to generate new slug')
 
     return {
         'slug': slug.get_slug_string(),
         'is_new': is_new,
-        'is_reserved': slug.reserved_pretty_slug == slug.get_slug_string(),
+        'is_reserved': False
+        if nav_slug
+        else slug.reserved_pretty_slug == slug.get_slug_string(),
     }
 
 
 @action(
     schema.datastore_resolve_slug(),
     help.datastore_resolve_slug,
     toolkit.side_effect_free,
@@ -276,26 +291,35 @@
                 'query_version',
                 'version',
                 'resource_ids',
                 'resource_ids_and_versions',
             )
         }
         result['created'] = resolved.created.isoformat()
+        if result.get('query_version') == 'v0':
+            result['query'] = convert_to_multisearch(result['query'])
+            result['query_version'] = get_latest_query_version()
         return result
 
     # then check if it's a query DOI
     if plugin_loaded('query_dois'):
         from ckanext.query_dois.model import QueryDOI
         from ckan import model
 
         resolved = model.Session.query(QueryDOI).filter(QueryDOI.doi == slug).first()
         if resolved:
+            if resolved.query_version == 'v0':
+                query = convert_to_multisearch(resolved.query)
+                query_version = get_latest_query_version()
+            else:
+                query = resolved.query
+                query_version = resolved.query_version
             return {
-                'query': resolved.query,
-                'query_version': resolved.query_version,
+                'query': query,
+                'query_version': query_version,
                 'version': resolved.requested_version,
                 'resource_ids': list(resolved.resources_and_versions.keys()),
                 'resource_ids_and_versions': resolved.resources_and_versions,
                 'created': resolved.timestamp.isoformat(),
             }
 
     # if both slug and DOI have failed
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/logic/auth.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/logic/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -96,14 +96,20 @@
 @auth(anon=True)
 def datastore_queue_download(context, data_dict):
     # allow access to everyone
     return {'success': True}
 
 
 @auth(anon=True)
+def datastore_regenerate_download(context, data_dict):
+    # allow access to everyone
+    return {'success': True}
+
+
+@auth(anon=True)
 def datastore_guess_fields(context, data_dict):
     # allow access to everyone
     return {'success': True}
 
 
 @auth(anon=True)
 def datastore_hash_query(context, data_dict):
@@ -129,7 +135,14 @@
     return {'success': True}
 
 
 @auth()
 def datastore_edit_slug(context, data_dict):
     # only allows logged-in users
     return {'success': True}
+
+
+@auth()
+def datastore_custom_download_filename(context, data_dict):
+    # only allow access to admins (they usually skip this check)
+    user_is_sysadmin = context.get('auth_user_obj').sysadmin
+    return {'success': user_is_sysadmin}
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/env.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/details.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/model/details.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/downloads.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/model/downloads.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     'vds_download_request',
     meta.metadata,
     Column('id', UnicodeText, primary_key=True, default=make_uuid),
     Column('created', DateTime, nullable=False, default=datetime.utcnow),
     Column('modified', DateTime, nullable=False, default=datetime.utcnow),
     Column('state', UnicodeText, nullable=False, default=state_initial),
     Column('message', UnicodeText, nullable=True),
+    Column('server_args', JSONB, nullable=True),
     Column(
         'derivative_id',
         UnicodeText,
         ForeignKey(
             'vds_download_derivative.id', onupdate='CASCADE', ondelete='CASCADE'
         ),
         nullable=True,
@@ -199,14 +200,15 @@
     """
 
     id: str
     created: datetime
     modified: datetime
     state: str
     message: str
+    server_args: dict
     derivative_id: str
     derivative_record: DerivativeFileRecord
     core_record: CoreFileRecord
 
     state_initial = state_initial
     state_complete = 'complete'
     state_failed = 'failed'
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/model/stats.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/model/stats.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/plugin.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
             'get_stat_icon': helpers.get_stat_icon,
             'get_stat_activity_class': helpers.get_stat_activity_class,
             'get_stat_title': helpers.get_stat_title,
             'get_available_formats': helpers.get_available_formats,
             'pretty_print_json': helpers.pretty_print_json,
             'get_version_date': helpers.get_version_date,
             'latest_item_version': helpers.latest_item_version,
+            'nav_slug': helpers.nav_slug,
         }
 
     # IResourceController
     def before_show(self, resource_dict):
         resource_dict['datastore_active'] = is_datastore_resource(resource_dict['id'])
         return resource_dict
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/datastore.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/routes/datastore.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/downloads.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/routes/downloads.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,7 +12,20 @@
     development. In production we should always serve files through the web server.
 
     :param zip_name: the zip name
     :return: the send file response
     """
     download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
     return send_from_directory(download_dir, zip_name)
+
+
+@blueprint.route('/custom/<zip_name>')
+def custom(zip_name):
+    """
+    Basically exactly the same as the /direct/ route, but for serving the symlinks with
+    custom filenames.
+
+    :param zip_name: the zip name
+    :return: the send file response
+    """
+    download_dir = toolkit.config.get('ckanext.versioned_datastore.custom_dir')
+    return send_from_directory(download_dir, zip_name)
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/routes/search.py` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/routes/search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/less/datastore-activities.less`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/scripts/modules/search.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/api.html` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/api.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/11.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/5.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/6.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/resource_data.html` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/resource_data.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/search.html` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/search/slugerator.html` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/search/slugerator.html`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext/versioned_datastore/theme/templates/status/download.html` & `ckanext-versioned-datastore-5.0.0/ckanext/versioned_datastore/theme/templates/status/download.html`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,20 @@
                 </tr>
                 </tbody>
             </table>
             <h3>Request</h3>
             <table class="table table-striped table-bordered table-condensed">
                 <tbody>
                 {% if download_request.core_record %}
+                {% if search_url %}
+                <tr>
+                    <th scope="row">Search</th>
+                    <td><a href="{{ search_url }}" target="_blank">View</a></td>
+                </tr>
+                {% endif %}
                 <tr>
                     <th scope="row">Query</th>
                     <td>
                         <pre class="query-box">
                             {{- h.pretty_print_json(download_request.core_record.query) -}}
                         </pre>
                     </td>
@@ -124,24 +130,26 @@
             </table>
             <h3>Results</h3>
             <table class="table table-striped table-bordered table-condensed">
                 <tbody>
                 {% if doi %}
                 <tr>
                     <th scope="row">Query DOI</th>
-                    <td><a href="{{ doi_url }}">{{ doi.doi }}</a></td>
+                    <td><a href="{{ doi_url }}" target="_blank">{{ doi.doi }}</a></td>
                 </tr>
                 {% endif %}
                 {% if download_request.core_record and not download_request.state == 'failed' %}
                 <tr>
                     <th scope="row">Records</th>
                     <td>
                         <dl>
                             <dt>Total</dt>
-                            <dd>{{ download_request.core_record.total or _('processing') }}</dd>
+                            {% if download_request.core_record.total is not none %}
+                            <dd>{{ download_request.core_record.total }}</dd>
+                            {% endif %}
                             {% if download_request.core_record.resource_totals %}
                             {% for res_id, res in resources.items() %}
                             {% if download_request.core_record.resource_totals[res_id] > 0 %}
                             <dt>{{ res['name'] }}</dt>
                             <dd>{{ download_request.core_record.resource_totals[res_id] }}</dd>
                             {% endif %}
                             {% endfor %}
@@ -150,19 +158,23 @@
                     </td>
                 </tr>
                 {% endif %}
                 {% if download_request.state == 'complete' %}
                 <tr>
                     <th scope="row">Downloads</th>
                     <td>
+                        {% if file_exists %}
                         <ul class="download-links">
                             {% for server_name, url in urls.items() %}
                             <li><a href="{{ url }}" class="btn btn-primary"><i class="fas fa-download"></i> {{ server_name }} </a></li>
                             {% endfor %}
                         </ul>
+                        {% else %}
+                        {{_('File could not be found. Please request a new download from the search page, or contact us if you believe this is an error.')}}
+                        {% endif %}
                     </td>
                 </tr>
                 {% endif %}
                 </tbody>
             </table>
 
         </section>
```

#### html2text {}

```diff
@@ -17,28 +17,33 @@
 Created                {{ download_request.created.strftime('%Y-%m-%d %H:%M:
                        %S') }}
 Last updated           {{ download_request.modified.strftime('%Y-%m-%d %H:%M:
                        %S') }}
 Time elapsed           {{ total_time }}
 Download ID            {{ download_request.id }}
 **** Request ****
+Search                      View
 Query                                                   {{- h.pretty_print_json
                             (download_request.core_record.query) -}}
 Query version               {{ download_request.core_record.query_version }}
 Format                      {{ download_request.derivative_record.format }}
                             {% for k, v in
 Format details              download_request.derivative_record.options.get
                             ('format_args', {}).items() %}
 Resources in separate files {{ download_request.derivative_record.options.get
                             ('separate_files', True) }}
 Ignore empty fields         {{ download_request.derivative_record.options.get
                             ('ignore_empty_fields', True) }}
 **** Results ****
 Query DOI {{_doi.doi_}}
 Records
+          {% if file_exists %}
               * {% for server_name, url in urls.items() %}
-Downloads     *  {{_server_name_}}
-              * {% endfor %}
+              *  {{_server_name_}}
+Downloads     * {% endfor %}
+          {% else %} {{_('File could not be found. Please request a new
+          download from the search page, or contact us if you believe this is
+          an error.')}} {% endif %}
  {% else %}
 Invalid download ID. Please check the URL and try again.
 {% endif %}
  {% endblock %}
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/PKG-INFO` & `ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-versioned-datastore
-Version: 4.2.2
+Version: 5.0.0
 Summary: A CKAN extension providing a versioned datastore using MongoDB and Elasticsearch
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-versioned-datastore/blob/main/CHANGELOG.md
 Keywords: CKAN,data,versioned_datastore
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ckanext-versioned-datastore-4.2.2/ckanext_versioned_datastore.egg-info/SOURCES.txt` & `ckanext-versioned-datastore-5.0.0/ckanext_versioned_datastore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -77,29 +77,33 @@
 ckanext/versioned_datastore/logic/actions/meta/help.py
 ckanext/versioned_datastore/logic/actions/meta/schema.py
 ckanext/versioned_datastore/migration/versioned_datastore/README
 ckanext/versioned_datastore/migration/versioned_datastore/alembic.ini
 ckanext/versioned_datastore/migration/versioned_datastore/env.py
 ckanext/versioned_datastore/migration/versioned_datastore/script.py.mako
 ckanext/versioned_datastore/migration/versioned_datastore/versions/19a61e5b669f_add_new_download_tables.py
+ckanext/versioned_datastore/migration/versioned_datastore/versions/526b12c69d55_add_navigational_slugs.py
+ckanext/versioned_datastore/migration/versioned_datastore/versions/d2ca5da0573f_add_server_args_to_download_request_.py
 ckanext/versioned_datastore/model/__init__.py
 ckanext/versioned_datastore/model/details.py
 ckanext/versioned_datastore/model/downloads.py
 ckanext/versioned_datastore/model/slugs.py
 ckanext/versioned_datastore/model/stats.py
 ckanext/versioned_datastore/routes/__init__.py
 ckanext/versioned_datastore/routes/datastore.py
 ckanext/versioned_datastore/routes/downloads.py
 ckanext/versioned_datastore/routes/search.py
 ckanext/versioned_datastore/routes/status.py
 ckanext/versioned_datastore/theme/assets/webassets.yml
 ckanext/versioned_datastore/theme/assets/less/datastore-activities.less
+ckanext/versioned_datastore/theme/assets/less/download-popup.less
 ckanext/versioned_datastore/theme/assets/less/download-status.less
 ckanext/versioned_datastore/theme/assets/less/search.less
 ckanext/versioned_datastore/theme/assets/less/slugerator.less
+ckanext/versioned_datastore/theme/assets/scripts/modules/download-button.js
 ckanext/versioned_datastore/theme/assets/scripts/modules/search.js
 ckanext/versioned_datastore/theme/assets/scripts/vendor/bodybuilder.js
 ckanext/versioned_datastore/theme/public/api.html
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/README.md
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.json
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/v1.0.0.yml
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/examples/1.json
@@ -117,22 +121,24 @@
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-admin-0-countries-v4.1.0.geojson
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-geography-regions-v4.1.0.geojson
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/50m-marine-regions-v4.1.0.geojson
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/README.md
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-countries.json
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-geography.json
 ckanext/versioned_datastore/theme/public/querySchemas/v1.0.0/geojson/v1.0.0-marine.json
+ckanext/versioned_datastore/theme/templates/ajax_snippets/download_popup.html
 ckanext/versioned_datastore/theme/templates/package/resource_data.html
 ckanext/versioned_datastore/theme/templates/package/resource_edit_base.html
 ckanext/versioned_datastore/theme/templates/package/snippets/index_message.html
 ckanext/versioned_datastore/theme/templates/package/snippets/ingest_message.html
 ckanext/versioned_datastore/theme/templates/package/snippets/prep_message.html
 ckanext/versioned_datastore/theme/templates/search/search.html
 ckanext/versioned_datastore/theme/templates/search/slugerator.html
 ckanext/versioned_datastore/theme/templates/status/download.html
+ckanext/versioned_datastore/theme/templates/versioned_datastore/snippets/download_button.html
 ckanext_versioned_datastore.egg-info/PKG-INFO
 ckanext_versioned_datastore.egg-info/SOURCES.txt
 ckanext_versioned_datastore.egg-info/dependency_links.txt
 ckanext_versioned_datastore.egg-info/entry_points.txt
 ckanext_versioned_datastore.egg-info/not-zip-safe
 ckanext_versioned_datastore.egg-info/requires.txt
 ckanext_versioned_datastore.egg-info/top_level.txt
```

### Comparing `ckanext-versioned-datastore-4.2.2/docs/_scripts/gen_api_pages.py` & `ckanext-versioned-datastore-5.0.0/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/pyproject.toml` & `ckanext-versioned-datastore-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-versioned-datastore"
-version = "4.2.2"
+version = "5.0.0"
 description = "A CKAN extension providing a versioned datastore using MongoDB and Elasticsearch"
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -71,15 +71,15 @@
 
 [tool.setuptools.package-data]
 "ckanext.versioned_datastore.theme" = ["*", "**/*"]
 "ckanext.versioned_datastore.migration" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "4.2.2"
+version = "5.0.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

### Comparing `ckanext-versioned-datastore-4.2.2/tests/helpers/data.py` & `ckanext-versioned-datastore-5.0.0/tests/helpers/data.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/helpers/patches.py` & `ckanext-versioned-datastore-5.0.0/tests/helpers/patches.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,19 @@
         side_effect=MagicMock(),
     )
 
 
 def get_available_resources(resource_ids=None):
     resource_ids = resource_ids or ['test-resource-id']
     return patch(
-        'ckanext.versioned_datastore.lib.downloads.query.get_available_datastore_resources',
+        'ckanext.versioned_datastore.lib.query.utils.get_available_datastore_resources',
         return_value=resource_ids,
     )
 
 
 def query_schemas():
     test_schemas = {'v1.0.0': MagicMock(validate=MagicMock(return_value=True))}
     return patch('ckanext.versioned_datastore.lib.query.schema.schemas', test_schemas)
+
+
+def url_for():
+    return patch('ckan.plugins.toolkit.url_for', return_value='/banana')
```

### Comparing `ckanext-versioned-datastore-4.2.2/tests/helpers/utils.py` & `ckanext-versioned-datastore-5.0.0/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/integration/downloads/test_downloads.py` & `ckanext-versioned-datastore-5.0.0/tests/integration/downloads/test_downloads.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import csv
 import json
 import os
+import pytest
 import shutil
 import tempfile
 import zipfile
-
-import pytest
-from ckan.plugins import toolkit
 from mock import patch, MagicMock
-
 from tests.helpers import patches, data as test_data
 
+from ckan.plugins import toolkit
+from ckan.tests import factories
+from ckanext.versioned_datastore.model.downloads import DownloadRequest
+
 scenarios = [
     ('csv', {}),
     ('json', {}),
     ('xlsx', {}),
     ('dwc', {}),
     ('csv', {'delimiter': 'tab'}),
     (
@@ -40,32 +41,35 @@
 class TestQueueDownload:
     @patches.enqueue_job()
     @pytest.mark.parametrize('file_format,format_args', scenarios)
     @pytest.mark.parametrize('separate_files', [True, False])
     def test_run_download_formats(
         self, enqueue_job, with_vds_resource, file_format, format_args, separate_files
     ):
-        download_details = toolkit.get_action('datastore_queue_download')(
-            {},
-            {
-                'query': {'query': {}},
-                'file': {
-                    'format': file_format,
-                    'format_args': format_args,
-                    'separate_files': separate_files,
+        with patches.url_for():
+            download_details = toolkit.get_action('datastore_queue_download')(
+                {},
+                {
+                    'query': {'query': {}},
+                    'file': {
+                        'format': file_format,
+                        'format_args': format_args,
+                        'separate_files': separate_files,
+                    },
+                    'notifier': {'type': 'none'},
                 },
-                'notifier': {'type': 'none'},
-            },
-        )
+            )
         enqueue_job.assert_called()
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
         download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
         matching_zips = [
             f
             for f in os.listdir(download_dir)
-            if f.startswith(download_details['download_id'])
+            if f.startswith(download_request.derivative_record.download_hash)
         ]
         assert len(matching_zips) == 1
         with zipfile.ZipFile(os.path.join(download_dir, matching_zips[0]), 'r') as zf:
             archive_files = zf.namelist()
             assert 'manifest.json' in archive_files
             if not separate_files:
                 assert f'resource{expected_extensions[file_format]}' in archive_files
@@ -79,28 +83,31 @@
                 assert (
                     f'{with_vds_resource[1]["id"]}{expected_extensions[file_format]}'
                     in archive_files
                 )
 
     @patches.enqueue_job()
     def test_run_download_without_query(self, enqueue_job):
-        download_details = toolkit.get_action('datastore_queue_download')(
-            {},
-            {
-                'query': {'query': {}},
-                'file': {'format': 'csv'},
-                'notifier': {'type': 'none'},
-            },
-        )
+        with patches.url_for():
+            download_details = toolkit.get_action('datastore_queue_download')(
+                {},
+                {
+                    'query': {'query': {}},
+                    'file': {'format': 'csv'},
+                    'notifier': {'type': 'none'},
+                },
+            )
         enqueue_job.assert_called()
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
         download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
         matching_zips = [
             f
             for f in os.listdir(download_dir)
-            if f.startswith(download_details['download_id'])
+            if f.startswith(download_request.derivative_record.download_hash)
         ]
         assert len(matching_zips) == 1
         self.temp_dir = tempfile.mktemp()
         with zipfile.ZipFile(os.path.join(download_dir, matching_zips[0]), 'r') as zf:
             archive_files = zf.namelist()
             assert 'manifest.json' in archive_files
             zf.extract('manifest.json', self.temp_dir)
@@ -132,41 +139,44 @@
                 for k, v in test_data_record.items():
                     assert v == record[k]
 
         shutil.rmtree(self.temp_dir)
 
     @patches.enqueue_job()
     def test_run_download_with_query(self, enqueue_job, with_vds_resource):
-        download_details = toolkit.get_action('datastore_queue_download')(
-            {},
-            {
-                'query': {
+        with patches.url_for():
+            download_details = toolkit.get_action('datastore_queue_download')(
+                {},
+                {
                     'query': {
-                        'filters': {
-                            'and': [
-                                {
-                                    'string_equals': {
-                                        'fields': ['colour'],
-                                        'value': 'green',
+                        'query': {
+                            'filters': {
+                                'and': [
+                                    {
+                                        'string_equals': {
+                                            'fields': ['colour'],
+                                            'value': 'green',
+                                        }
                                     }
-                                }
-                            ]
-                        },
-                    }
+                                ]
+                            },
+                        }
+                    },
+                    'file': {'format': 'csv'},
+                    'notifier': {'type': 'none'},
                 },
-                'file': {'format': 'csv'},
-                'notifier': {'type': 'none'},
-            },
-        )
+            )
         enqueue_job.assert_called()
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
         download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
         matching_zips = [
             f
             for f in os.listdir(download_dir)
-            if f.startswith(download_details['download_id'])
+            if f.startswith(download_request.derivative_record.download_hash)
         ]
         assert len(matching_zips) == 1
         self.temp_dir = tempfile.mktemp()
         with zipfile.ZipFile(os.path.join(download_dir, matching_zips[0]), 'r') as zf:
             archive_files = zf.namelist()
             assert 'manifest.json' in archive_files
             assert 'resource.csv' in archive_files
@@ -177,45 +187,48 @@
             records = [row for row in reader]
             assert len(records) == 1  # the number of records that should match the q
 
         shutil.rmtree(self.temp_dir)
 
     @patches.enqueue_job()
     def test_run_download_keep_empty(self, enqueue_job, with_vds_resource):
-        download_details = toolkit.get_action('datastore_queue_download')(
-            {},
-            {
-                'query': {
+        with patches.url_for():
+            download_details = toolkit.get_action('datastore_queue_download')(
+                {},
+                {
                     'query': {
-                        'filters': {
-                            'and': [
-                                {
-                                    'string_equals': {
-                                        'fields': ['group'],
-                                        'value': 'b',
+                        'query': {
+                            'filters': {
+                                'and': [
+                                    {
+                                        'string_equals': {
+                                            'fields': ['group'],
+                                            'value': 'b',
+                                        }
                                     }
-                                }
-                            ]
-                        },
-                    }
-                },
-                'file': {
-                    'format': 'csv',
-                    'ignore_empty_fields': False,
-                    'separate_files': False,
+                                ]
+                            },
+                        }
+                    },
+                    'file': {
+                        'format': 'csv',
+                        'ignore_empty_fields': False,
+                        'separate_files': False,
+                    },
+                    'notifier': {'type': 'none'},
                 },
-                'notifier': {'type': 'none'},
-            },
-        )
+            )
         enqueue_job.assert_called()
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
         download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
         matching_zips = [
             f
             for f in os.listdir(download_dir)
-            if f.startswith(download_details['download_id'])
+            if f.startswith(download_request.derivative_record.download_hash)
         ]
         assert len(matching_zips) == 1
         self.temp_dir = tempfile.mktemp()
         with zipfile.ZipFile(os.path.join(download_dir, matching_zips[0]), 'r') as zf:
             archive_files = zf.namelist()
             assert 'manifest.json' in archive_files
             assert 'resource.csv' in archive_files
@@ -226,45 +239,48 @@
             header = [row for row in reader][0]
             assert 'emptyField' in header
 
         shutil.rmtree(self.temp_dir)
 
     @patches.enqueue_job()
     def test_run_download_ignore_empty(self, enqueue_job, with_vds_resource):
-        download_details = toolkit.get_action('datastore_queue_download')(
-            {},
-            {
-                'query': {
+        with patches.url_for():
+            download_details = toolkit.get_action('datastore_queue_download')(
+                {},
+                {
                     'query': {
-                        'filters': {
-                            'and': [
-                                {
-                                    'string_equals': {
-                                        'fields': ['group'],
-                                        'value': 'b',
+                        'query': {
+                            'filters': {
+                                'and': [
+                                    {
+                                        'string_equals': {
+                                            'fields': ['group'],
+                                            'value': 'b',
+                                        }
                                     }
-                                }
-                            ]
-                        },
-                    }
-                },
-                'file': {
-                    'format': 'csv',
-                    'ignore_empty_fields': True,
-                    'separate_files': False,
+                                ]
+                            },
+                        }
+                    },
+                    'file': {
+                        'format': 'csv',
+                        'ignore_empty_fields': True,
+                        'separate_files': False,
+                    },
+                    'notifier': {'type': 'none'},
                 },
-                'notifier': {'type': 'none'},
-            },
-        )
+            )
         enqueue_job.assert_called()
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
         download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
         matching_zips = [
             f
             for f in os.listdir(download_dir)
-            if f.startswith(download_details['download_id'])
+            if f.startswith(download_request.derivative_record.download_hash)
         ]
         assert len(matching_zips) == 1
         self.temp_dir = tempfile.mktemp()
         with zipfile.ZipFile(os.path.join(download_dir, matching_zips[0]), 'r') as zf:
             archive_files = zf.namelist()
             assert 'manifest.json' in archive_files
             assert 'resource.csv' in archive_files
@@ -276,29 +292,31 @@
             assert 'emptyField' not in header
 
         shutil.rmtree(self.temp_dir)
 
     @patches.enqueue_job()
     @pytest.mark.parametrize('transform', [{'id_as_url': {'field': 'urlSlug'}}])
     def test_run_download_with_transform(self, enqueue_job, transform):
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             download_details = toolkit.get_action('datastore_queue_download')(
                 {},
                 {
                     'query': {'query': {}},
                     'file': {'format': 'csv', 'transform': transform},
                     'notifier': {'type': 'none'},
                 },
             )
         enqueue_job.assert_called()
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
         download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
         matching_zips = [
             f
             for f in os.listdir(download_dir)
-            if f.startswith(download_details['download_id'])
+            if f.startswith(download_request.derivative_record.download_hash)
         ]
         assert len(matching_zips) == 1
         self.temp_dir = tempfile.mktemp()
         with zipfile.ZipFile(os.path.join(download_dir, matching_zips[0]), 'r') as zf:
             archive_files = zf.namelist()
             assert 'manifest.json' in archive_files
             assert 'resource.csv' in archive_files
@@ -309,14 +327,69 @@
             records = [row for row in reader]
             assert len(records) == len(test_data.records + test_data.records_addtl)
             for record in records:
                 assert record['urlSlug'].endswith('/banana')
 
         shutil.rmtree(self.temp_dir)
 
+    @patches.enqueue_job()
+    def test_run_download_with_non_vds_resource(self, enqueue_job, with_vds_resource):
+        non_ds_resource = factories.Resource(url_type='upload')
+
+        def _shutil_mock(src, dest):
+            # there's nothing to copy from, so just write the new file
+            with open(dest, 'w') as f:
+                f.write('hello')
+
+        with patch('shutil.copy2', side_effect=_shutil_mock), patches.url_for():
+            download_details = toolkit.get_action('datastore_queue_download')(
+                {},
+                {
+                    'query': {
+                        'query': {},
+                        'resource_ids': [non_ds_resource['id']],
+                    },
+                    'file': {
+                        'format': 'raw',
+                        'format_args': {'allow_non_datastore': True},
+                    },
+                    'notifier': {'type': 'none'},
+                },
+            )
+        enqueue_job.assert_called()
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
+        download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
+        matching_zips = [
+            f
+            for f in os.listdir(download_dir)
+            if f.startswith(download_request.derivative_record.download_hash)
+        ]
+        assert len(matching_zips) == 1
+        self.temp_dir = tempfile.mktemp()
+        with zipfile.ZipFile(os.path.join(download_dir, matching_zips[0]), 'r') as zf:
+            archive_files = zf.namelist()
+            assert 'manifest.json' in archive_files
+            zf.extract('manifest.json', self.temp_dir)
+            assert len(archive_files) == 2
+            # it's easier to do it this way than to predict the url or split it or whatever
+            extless_files = [os.path.splitext(f)[0] for f in archive_files]
+            assert non_ds_resource['id'] in extless_files
+
+        with open(os.path.join(self.temp_dir, 'manifest.json')) as f:
+            manifest = json.load(f)
+            assert manifest['download_id'] == download_details['download_id']
+            assert manifest['file_format'] == 'raw'
+            assert sorted(manifest['files']) == sorted(archive_files)
+            assert not manifest['ignore_empty_fields']
+            assert manifest['separate_files']
+            assert manifest['total_records'] == 1
+
+        shutil.rmtree(self.temp_dir)
+
 
 @pytest.mark.ckan_config('ckan.plugins', 'versioned_datastore query_dois')
 @pytest.mark.ckan_config('ckanext.query_dois.prefix', 'xx.xxxx')
 @pytest.mark.usefixtures(
     'with_plugins',
     'with_versioned_datastore_tables',
     'with_vds_resource',
@@ -336,40 +409,41 @@
     def teardown_class(cls):
         for table in cls.tables:
             if table.exists():
                 table.drop()
 
     @patches.enqueue_job()
     def test_run_download_with_query_dois(self, enqueue_job):
-
         # I cannot get the query_doi endpoints to load for the life of me so we're just
         # going to mock it before I lose my mind
         def _url_for_mock(endpoint, **kwargs):
             if endpoint == 'query_doi.landing_page':
                 return f'/{kwargs["data_centre"]}/{kwargs["identifier"]}'
             else:
-                return toolkit.url_for(endpoint, **kwargs)
+                return '/banana'
 
         with patch(
             'ckanext.query_dois.lib.doi.find_existing_doi',
             return_value=MagicMock(doi='123456'),
         ), patch('ckan.plugins.toolkit.url_for', _url_for_mock):
             download_details = toolkit.get_action('datastore_queue_download')(
                 {},
                 {
                     'query': {'query': {}},
                     'file': {'format': 'dwc'},
                     'notifier': {'type': 'none'},
                 },
             )
         enqueue_job.assert_called()
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
         download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
         assert any(
             [
-                f.startswith(download_details['download_id'])
+                f.startswith(download_request.derivative_record.download_hash)
                 for f in os.listdir(download_dir)
             ]
         )
 
 
 @pytest.mark.ckan_config('ckan.plugins', 'versioned_datastore')
 @pytest.mark.usefixtures(
@@ -382,58 +456,62 @@
 class TestDownloadInterfaces:
     def test_modify_args(self, enqueue_job):
         mock_plugin = ModifyArgsPlugin()
 
         with patch(
             'ckanext.versioned_datastore.lib.downloads.download.PluginImplementations',
             return_value=[mock_plugin],
-        ):
+        ), patches.url_for():
             download_details = toolkit.get_action('datastore_queue_download')(
                 {},
                 {
                     'query': {'query': {}},
                     'file': {'format': 'csv'},
                     'notifier': {'type': 'none'},
                 },
             )
 
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
         download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
         matching_zips = [
             f
             for f in os.listdir(download_dir)
-            if f.startswith(download_details['download_id'])
+            if f.startswith(download_request.derivative_record.download_hash)
         ]
         assert len(matching_zips) == 1
         with zipfile.ZipFile(os.path.join(download_dir, matching_zips[0]), 'r') as zf:
             archive_files = zf.namelist()
             assert 'manifest.json' in archive_files
             assert 'resource.xlsx' in archive_files
             assert len(archive_files) == 2
 
     def test_modify_manifest(self, enqueue_job):
         mock_plugin = ModifyManifestPlugin()
 
         with patch(
             'ckanext.versioned_datastore.lib.downloads.download.PluginImplementations',
             return_value=[mock_plugin],
-        ):
+        ), patches.url_for():
             download_details = toolkit.get_action('datastore_queue_download')(
                 {},
                 {
                     'query': {'query': {}},
                     'file': {'format': 'csv'},
                     'notifier': {'type': 'none'},
                 },
             )
 
+        download_request = DownloadRequest.get(download_details['download_id'])
+        assert download_request is not None
         download_dir = toolkit.config.get('ckanext.versioned_datastore.download_dir')
         matching_zips = [
             f
             for f in os.listdir(download_dir)
-            if f.startswith(download_details['download_id'])
+            if f.startswith(download_request.derivative_record.download_hash)
         ]
         assert len(matching_zips) == 1
         temp_dir = tempfile.mktemp()
         with zipfile.ZipFile(os.path.join(download_dir, matching_zips[0]), 'r') as zf:
             archive_files = zf.namelist()
             assert 'manifest.json' in archive_files
             assert 'resource.csv' in archive_files
```

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_geo.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/basic_query/test_basic_query_geo.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_search.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/basic_query/test_basic_query_search.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/basic_query/test_basic_query_utils.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/basic_query/test_basic_query_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/derivatives/test_derivatives_dwc.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_notifiers.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/test_downloads_notifiers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 from mock import MagicMock, patch
+from tests.helpers import patches
 
 from ckanext.versioned_datastore.lib.downloads.notifiers import (
     EmailNotifier,
     NullNotifier,
     WebhookNotifier,
 )
 
@@ -15,52 +16,52 @@
 
 
 @pytest.mark.parametrize('notifier_type,notifier_args', notifiers)
 class TestNotifierGetText:
     def test_notifier_start_text(self, notifier_type, notifier_args):
         notifier = notifier_type(MagicMock(), **notifier_args)
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             start_text = notifier.start_text()
 
         assert isinstance(start_text, tuple)
         assert len(start_text) == 2
         for t in start_text:
             assert '/banana' in t
 
     def test_notifier_end_text(self, notifier_type, notifier_args):
         notifier = notifier_type(MagicMock(), **notifier_args)
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             end_text = notifier.end_text('/download-url-here')
 
         assert isinstance(end_text, tuple)
         assert len(end_text) == 2
         for t in end_text:
             assert '/download-url-here' in t
 
     def test_notifier_error_text(self, notifier_type, notifier_args):
         notifier = notifier_type(MagicMock(), **notifier_args)
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             error_text = notifier.error_text()
 
         assert isinstance(error_text, tuple)
         assert len(error_text) == 2
         for t in error_text:
             assert '/banana' in t
 
 
 @patch('ckanext.versioned_datastore.lib.downloads.notifiers.email.mailer')
 class TestEmailNotifier:
     def test_email_notifier_start(self, mock_mailer):
         test_email_address = 'test@email.address'
         notifier = EmailNotifier(MagicMock(), emails=[test_email_address])
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             start_text = notifier.start_text()
             notifier.notify_start()
 
         assert mock_mailer.mail_recipient.called
         args, kwargs = mock_mailer.mail_recipient.call_args
         assert kwargs['recipient_email'] == test_email_address
         assert kwargs['recipient_name'] == 'Downloader'
@@ -69,15 +70,15 @@
         assert start_text[1] in kwargs['body_html']
 
     def test_email_notifier_end(self, mock_mailer):
         test_email_address = 'test@email.address'
         test_download_url = '/download-url-here'
         notifier = EmailNotifier(MagicMock(), emails=[test_email_address])
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             end_text = notifier.end_text(test_download_url)
             notifier.notify_end(test_download_url)
 
         assert mock_mailer.mail_recipient.called
         args, kwargs = mock_mailer.mail_recipient.call_args
         assert kwargs['recipient_email'] == test_email_address
         assert kwargs['recipient_name'] == 'Downloader'
@@ -85,15 +86,15 @@
         assert end_text[0] in kwargs['body']
         assert end_text[1] in kwargs['body_html']
 
     def test_email_notifier_error(self, mock_mailer):
         test_email_address = 'test@email.address'
         notifier = EmailNotifier(MagicMock(), emails=[test_email_address])
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             error_text = notifier.error_text()
             notifier.notify_error()
 
         assert mock_mailer.mail_recipient.called
         args, kwargs = mock_mailer.mail_recipient.call_args
         assert kwargs['recipient_email'] == test_email_address
         assert kwargs['recipient_name'] == 'Downloader'
@@ -101,15 +102,15 @@
         assert error_text[0] in kwargs['body']
         assert error_text[1] in kwargs['body_html']
 
     def test_email_notifier_multiple_emails(self, mock_mailer):
         test_email_addresses = ['one@email.address', 'two@email.address']
         notifier = EmailNotifier(MagicMock(), emails=test_email_addresses)
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             start_text = notifier.start_text()
             notifier.notify_start()
 
         assert mock_mailer.mail_recipient.call_count == len(test_email_addresses)
         _, recipient_one = mock_mailer.mail_recipient.call_args_list[0]
         _, recipient_two = mock_mailer.mail_recipient.call_args_list[1]
         for k, v in recipient_one.items():
@@ -122,15 +123,15 @@
 
 @patch('ckanext.versioned_datastore.lib.downloads.notifiers.webhook.requests')
 class TestWebhookNotifier:
     def test_webhook_notifier_start(self, mock_requests):
         test_webhook_url = 'http://webhook-url'
         notifier = WebhookNotifier(MagicMock(), url=test_webhook_url)
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             start_text = notifier.start_text()
             notifier.notify_start()
 
         assert mock_requests.request.called
         args, kwargs = mock_requests.request.call_args
         assert args[0] == 'GET'
         assert args[1] == test_webhook_url
@@ -138,30 +139,30 @@
         assert kwargs['params']['text'] == start_text[0]
 
     def test_webhook_notifier_end(self, mock_requests):
         test_webhook_url = 'http://webhook-url'
         test_download_url = '/download-url-here'
         notifier = WebhookNotifier(MagicMock(), url=test_webhook_url)
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             end_text = notifier.end_text(test_download_url)
             notifier.notify_end(test_download_url)
 
         assert mock_requests.request.called
         args, kwargs = mock_requests.request.call_args
         assert args[0] == 'GET'
         assert args[1] == test_webhook_url
         assert kwargs['params']['url'] == test_download_url
         assert kwargs['params']['text'] == end_text[0]
 
     def test_webhook_notifier_error(self, mock_requests):
         test_webhook_url = 'http://webhook-url'
         notifier = WebhookNotifier(MagicMock(), url=test_webhook_url)
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             error_text = notifier.error_text()
             notifier.notify_error()
 
         assert mock_requests.request.called
         args, kwargs = mock_requests.request.call_args
         assert args[0] == 'GET'
         assert args[1] == test_webhook_url
@@ -174,15 +175,15 @@
             MagicMock(),
             url=test_webhook_url,
             url_param='something-not-url',
             text_param='anything-but-text',
             post=True,
         )
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             start_text = notifier.start_text()
             notifier.notify_start()
 
         assert mock_requests.request.called
         args, kwargs = mock_requests.request.call_args
         assert args[0] == 'POST'
         assert args[1] == test_webhook_url
@@ -193,36 +194,36 @@
 
 
 @patch('ckanext.versioned_datastore.lib.downloads.notifiers.null.logger')
 class TestNullNotifier:
     def test_null_notifier_start(self, mock_logger):
         notifier = NullNotifier(MagicMock())
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             notifier.notify_start()
 
         assert mock_logger.debug.called
         args, kwargs = mock_logger.debug.call_args
         assert args[0] == 'Processing started.'
 
     def test_null_notifier_end(self, mock_logger):
         test_download_url = '/download-url-here'
         notifier = NullNotifier(MagicMock())
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             notifier.notify_end(test_download_url)
 
         assert mock_logger.debug.called
         args, kwargs = mock_logger.debug.call_args
         assert args[0] == 'Processing ended.'
 
     def test_null_notifier_error(self, mock_logger):
         notifier = NullNotifier(MagicMock())
 
-        with patch('ckan.plugins.toolkit.url_for', return_value='/banana'):
+        with patches.url_for():
             notifier.notify_error()
 
         assert mock_logger.debug.called
         args, kwargs = mock_logger.debug.call_args
         assert args[0] == 'Processing failed.'
```

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_query.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/test_downloads_query.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_runmanager.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/test_downloads_runmanager.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/downloads/test_downloads_utils.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/downloads/test_downloads_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/importing/ingestion/test_ingestion_records.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/importing/ingestion/test_ingestion_records.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/test_query_query.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/query/test_query_query.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/query/test_query_v1_0_0.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/query/test_query_v1_0_0.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/lib/test_datastore_utils.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/lib/test_datastore_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/logic/actions/test_actions_downloads.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/logic/actions/test_actions_downloads.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         # instead
         resource_ids = ['test-resource-id']
 
         with patch(
             'ckan.plugins.toolkit.enqueue_job'
         ) as enqueue_mock, patches.rounded_versions(), patches.get_available_resources(
             resource_ids
-        ):
+        ), patches.url_for():
             datastore_queue_download(
                 {},
                 QueryArgs(),
                 DerivativeArgs(format='csv'),
                 notifier=NotifierArgs(type='none'),
             )
             assert enqueue_mock.call_count == 1
```

### Comparing `ckanext-versioned-datastore-4.2.2/tests/unit/test_helpers.py` & `ckanext-versioned-datastore-5.0.0/tests/unit/test_helpers.py`

 * *Files identical despite different names*

