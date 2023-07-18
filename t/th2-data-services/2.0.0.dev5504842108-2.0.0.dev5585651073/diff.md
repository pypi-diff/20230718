# Comparing `tmp/th2_data_services-2.0.0.dev5504842108.tar.gz` & `tmp/th2_data_services-2.0.0.dev5585651073.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev5504842108.tar", last modified: Mon Jul 10 06:33:22 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev5585651073.tar", last modified: Tue Jul 18 09:24:11 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev5504842108.tar` & `th2_data_services-2.0.0.dev5585651073.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23948 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-10 06:33:12.000000 th2_data_services-2.0.0.dev5504842108/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    16098 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5358 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14965 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     7000 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-07-10 06:32:17.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-10 06:33:22.000000 th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23948 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-18 09:24:01.000000 th2_data_services-2.0.0.dev5585651073/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16098 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5425 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14965 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16448 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7000 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-07-18 09:22:46.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-18 09:24:11.000000 th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev5504842108/PKG-INFO` & `th2_data_services-2.0.0.dev5585651073/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3535 3034 3834 3231 3038 0a53 756d 6d61  5504842108.Summa
+00000040: 3535 3835 3635 3130 3733 0a53 756d 6d61  5585651073.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5504842108/README.md` & `th2_data_services-2.0.0.dev5585651073/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/setup.py` & `th2_data_services-2.0.0.dev5585651073/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/data.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/frequencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "Tell DS team if you dont agree or have some ideas."
 )
 def get_category_frequencies(
     events: Iterable[Th2Event],
     categories: List[str],
     categorizer: Callable,
     aggregation_level: str = "seconds",
+    object_expander=None,
 ) -> FrequencyCategoryTable:
     """Returns event frequencies based on event category.
 
     Args:
         events (Iterable[Th2Event]): TH2-Events
         categories (List[str]): Event Categories
         categorizer (Callable): Categorizer Method
@@ -63,14 +64,15 @@
     return misc_utils.get_objects_frequencies2(
         events,
         categories,
         categorizer,
         # TODO -- we shouldn't know internal structure!!! - epochSeconds
         lambda e: options.EVENT_FIELDS_RESOLVER.get_start_timestamp(e)["epochSecond"],
         aggregation_level=aggregation_level,
+        object_expander=object_expander,
     )
 
 
 # Doesn't use category name now. Category values are table header.
 def get_category_frequencies2(
     events: Iterable[Th2Event], category: Category, aggregation_level: str = "seconds"
 ) -> FrequencyCategoryTable:
```

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/frequencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 # NOT STREAMABLE
 def get_category_frequencies(
     messages: Iterable[Th2Message],
     categories: List[str],
     categorizer: Callable,
     aggregation_level: str = "seconds",
     filter_: Callable = None,
+    object_expander=expand_message,
 ) -> FrequencyCategoryTable:  # noqa
     return misc_utils.get_objects_frequencies2(
         messages,
         categories,
         categorizer,
         # TODO -- we shouldn't know internal structure!!! - epochSeconds
-        lambda message: options.MESSAGE_FIELDS_RESOLVER.get_timestamp(message)["epochSecond"],
+        timestamp_function=lambda message: options.MESSAGE_FIELDS_RESOLVER.get_timestamp(message)[
+            "epochSecond"
+        ],
         aggregation_level=aggregation_level,
-        object_expander=expand_message,
+        object_expander=object_expander,
         objects_filter=filter_,
     )
```

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/misc_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+import pprint
 from collections import defaultdict
 from typing import Any, Callable, Dict, Iterable, List, Tuple
 from datetime import datetime, timezone
 
 from deprecated.classic import deprecated
 
 from th2_data_services.utils._types import Th2Event
@@ -63,15 +64,17 @@
                 if not objects_filter(expanded_object):
                     continue
 
             if anchor == 0:
                 anchor = timestamp_function(expanded_object)
 
             if not categories:
-                epoch = timestamp_aggregation_key(anchor, timestamp_function(expanded_object), aggregation_level)
+                epoch = timestamp_aggregation_key(
+                    anchor, timestamp_function(expanded_object), aggregation_level
+                )
                 category = categorizer(expanded_object)
                 categories_set.add(category)
                 if epoch not in frequencies:
                     frequencies[epoch] = {category: 1}
                 elif category not in frequencies[epoch]:
                     frequencies[epoch][category] = 1
                 else:
@@ -96,15 +99,17 @@
     timestamps = list(sorted(frequencies.keys()))
     for timestamp in timestamps:
         line = [datetime.fromtimestamp(timestamp, tz=timezone.utc).strftime("%Y-%m-%dT%H:%M:%S")]
         if categories:
             line.extend(frequencies[timestamp])
         else:
             for category in categories_set:
-                line.append(frequencies[timestamp][category]) if category in frequencies[timestamp] else line.append(0)
+                line.append(frequencies[timestamp][category]) if category in frequencies[
+                    timestamp
+                ] else line.append(0)
 
         results.append(line)
 
     return CategoryFrequencies(results)
 
 
 # STREAMABLE
@@ -133,43 +138,53 @@
 
     Returns:
         List[List]
     """
     frequencies = {}
     anchor = 0
     categories_set = set()
-    for obj in objects_stream:
-        expanded_objects = [obj] if object_expander is None else object_expander(obj)
-        for expanded_object in expanded_objects:
-            if objects_filter is not None:
-                if not objects_filter(expanded_object):
-                    continue
+    obj = None
 
-            if anchor == 0:
-                anchor = timestamp_function(expanded_object)
-
-            if not categories:
-                epoch = timestamp_aggregation_key(anchor, timestamp_function(expanded_object), aggregation_level)
-                category = categorizer(expanded_object)
-                categories_set.add(category)
-                if epoch not in frequencies:
-                    frequencies[epoch] = {category: 1}
-                elif category not in frequencies[epoch]:
-                    frequencies[epoch][category] = 1
+    try:
+        for obj in objects_stream:
+            expanded_objects = [obj] if object_expander is None else object_expander(obj)
+            for expanded_object in expanded_objects:
+                if objects_filter is not None:
+                    if not objects_filter(expanded_object):
+                        continue
+
+                if anchor == 0:
+                    anchor = timestamp_function(expanded_object)
+
+                if not categories:
+                    epoch = timestamp_aggregation_key(
+                        anchor, timestamp_function(expanded_object), aggregation_level
+                    )
+                    category = categorizer(expanded_object)
+                    categories_set.add(category)
+                    if epoch not in frequencies:
+                        frequencies[epoch] = {category: 1}
+                    elif category not in frequencies[epoch]:
+                        frequencies[epoch][category] = 1
+                    else:
+                        frequencies[epoch][category] += 1
                 else:
-                    frequencies[epoch][category] += 1
-            else:
-                for i in range(len(categories)):
-                    if categorizer(expanded_object) == categories[i]:
-                        epoch = timestamp_aggregation_key(
-                            anchor, timestamp_function(expanded_object), aggregation_level
-                        )
-                        if epoch not in frequencies:
-                            frequencies[epoch] = [0] * len(categories)
-                        frequencies[epoch][i] += 1
+                    for i in range(len(categories)):
+                        if categorizer(expanded_object) == categories[i]:
+                            epoch = timestamp_aggregation_key(
+                                anchor, timestamp_function(expanded_object), aggregation_level
+                            )
+                            if epoch not in frequencies:
+                                frequencies[epoch] = [0] * len(categories)
+                            frequencies[epoch][i] += 1
+    except KeyError:
+        # Print the object if a user provided wrong categorizer.
+        if obj is not None:
+            print(f"Problem object: \n" f"{pprint.pformat(obj)}")
+        raise
 
     header = ["timestamp"]
     if categories:
         header.extend(categories)
     else:
         header.extend(categories_set)
 
@@ -177,15 +192,17 @@
     timestamps = list(sorted(frequencies.keys()))
     for timestamp in timestamps:
         line = [datetime.fromtimestamp(timestamp, tz=timezone.utc).strftime("%Y-%m-%dT%H:%M:%S")]
         if categories:
             line.extend(frequencies[timestamp])
         else:
             for category in categories_set:
-                line.append(frequencies[timestamp][category]) if category in frequencies[timestamp] else line.append(0)
+                line.append(frequencies[timestamp][category]) if category in frequencies[
+                    timestamp
+                ] else line.append(0)
 
         results.append(line)
 
     r = FrequencyCategoryTable(header=header, rows=results[1:])
 
     return r
 
@@ -273,15 +290,20 @@
                             "seq_2": curr_seq,
                             "timestamp_1": prev_time,
                             "timestamp_2": curr_time,
                         }
                     )
                 if curr_seq == prev_seq:
                     result.append(
-                        {"type": "duplicate", "seq": prev_seq, "timestamp_1": prev_time, "timestamp_2": curr_time}
+                        {
+                            "type": "duplicate",
+                            "seq": prev_seq,
+                            "timestamp_1": prev_time,
+                            "timestamp_2": curr_time,
+                        }
                     )
             prev_seq = curr_seq
             prev_time = curr_time
 
     return result
 
 
@@ -306,39 +328,53 @@
             for expaned_object in expaned_objects:
                 for processor, params in processors:
                     processor(expaned_object, **params)
 
 
 # TODO: Is this useful?
 #   similar to totals for events, but evenets also have status field
-def get_category_totals_p(obj: Dict, categorizer: Callable, obj_filter: Callable, result) -> Any:  # noqa
+def get_category_totals_p(
+    obj: Dict, categorizer: Callable, obj_filter: Callable, result
+) -> Any:  # noqa
     # TODO: Add docstings
     if obj is None:
-        return get_category_totals_p, {"categorizer": categorizer, "obj_filter": obj_filter, "result": result}
+        return get_category_totals_p, {
+            "categorizer": categorizer,
+            "obj_filter": obj_filter,
+            "result": result,
+        }
 
     if obj_filter is not None and not obj_filter(obj):
         return None
 
     category = categorizer(obj)
     if category not in result:
         result[category] = 1
     else:
         result[category] = result[category] + 1
 
     return None
 
 
-def get_category_examples_p(obj: Dict, categorizer: Callable, obj_filter: Callable, cat_filter: Callable,
-                            max_qty: int, result) -> Any:
+def get_category_examples_p(
+    obj: Dict,
+    categorizer: Callable,
+    obj_filter: Callable,
+    cat_filter: Callable,
+    max_qty: int,
+    result,
+) -> Any:  # noqa
     if obj is None:
-        return get_category_examples_p, {"categorizer": categorizer,
-                                         "obj_filter": obj_filter,
-                                         "cat_filter": cat_filter,
-                                         "max_qty": max_qty,
-                                         "result": result}
+        return get_category_examples_p, {
+            "categorizer": categorizer,
+            "obj_filter": obj_filter,
+            "cat_filter": cat_filter,
+            "max_qty": max_qty,
+            "result": result,
+        }
     if obj_filter is not None and not obj_filter(obj):
         return None
 
     category = categorizer(obj)
     if cat_filter is not None and not cat_filter(category):
         return None
 
@@ -426,15 +462,18 @@
     for key, value in categories.items():
         if category_filter(key):
             result[value] += 1
 
     return result
 
 
-def calc_percentile_in_measurement_dict(d):
+def calc_percentile_in_measurement_dict(d):  # noqa
+    # TODO - something strange ..
+    #   nothing uses it.
+    #   it doesn't return anything
     for item in d.values():
         distr = item["distr"]
         total = item["count"]
         x_series = list(distr.keys())
         x_series.sort()
         sum = 0
         x_prev = 0
```

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev5585651073/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3535 3034 3834 3231 3038 0a53 756d 6d61  5504842108.Summa
+00000040: 3535 3835 3635 3130 3733 0a53 756d 6d61  5585651073.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5504842108/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev5585651073/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

