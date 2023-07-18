# Comparing `tmp/ghga_connector-0.3.8.tar.gz` & `tmp/ghga_connector-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_connector-0.3.8.tar", last modified: Mon Jul 17 14:17:11 2023, max compression
+gzip compressed data, was "ghga_connector-0.3.9.tar", last modified: Tue Jul 18 15:02:04 2023, max compression
```

## Comparing `ghga_connector-0.3.8.tar` & `ghga_connector-0.3.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.603518 ghga_connector-0.3.8/ghga_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.603518 ghga_connector-0.3.8/ghga_connector/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.607518 ghga_connector-0.3.8/ghga_connector/core/api_calls/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/well_knowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/api_calls/work_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/batch_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/http_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/ghga_connector/core/message_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.603518 ghga_connector-0.3.8/ghga_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 14:17:11.000000 ghga_connector-0.3.8/ghga_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.607518 ghga_connector-0.3.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/get_package_name.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/license_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.607518 ghga_connector-0.3.8/scripts/script_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/script_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/script_utils/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/update_config_docs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/update_readme.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/scripts/update_template_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-17 14:17:11.615518 ghga_connector-0.3.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.599518 ghga_connector-0.3.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/endpoints_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/fixtures/mock_api/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/mock_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/mock_api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/integration/test_file_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:17:11.611518 ghga_connector-0.3.8/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/test_api_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-17 14:16:50.000000 ghga_connector-0.3.8/tests/unit/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.835165 ghga_connector-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-07-18 15:02:04.835165 ghga_connector-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.827165 ghga_connector-0.3.9/ghga_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.831165 ghga_connector-0.3.9/ghga_connector/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.831165 ghga_connector-0.3.9/ghga_connector/core/api_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/api_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/api_calls/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/api_calls/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/api_calls/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/api_calls/well_knowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/api_calls/work_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/batch_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/http_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/ghga_connector/core/message_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.827165 ghga_connector-0.3.9/ghga_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-07-18 15:02:04.000000 ghga_connector-0.3.9/ghga_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-18 15:02:04.000000 ghga_connector-0.3.9/ghga_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:02:04.000000 ghga_connector-0.3.9/ghga_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 15:02:04.000000 ghga_connector-0.3.9/ghga_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:02:04.000000 ghga_connector-0.3.9/ghga_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 15:02:04.000000 ghga_connector-0.3.9/ghga_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 15:02:04.000000 ghga_connector-0.3.9/ghga_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.831165 ghga_connector-0.3.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/scripts/get_package_name.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/scripts/license_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.831165 ghga_connector-0.3.9/scripts/script_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/scripts/script_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/scripts/script_utils/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/scripts/update_config_docs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/scripts/update_readme.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/scripts/update_template_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-18 15:02:04.835165 ghga_connector-0.3.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.827165 ghga_connector-0.3.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.831165 ghga_connector-0.3.9/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/fixtures/endpoints_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.831165 ghga_connector-0.3.9/tests/fixtures/mock_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/fixtures/mock_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/fixtures/mock_api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/fixtures/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/fixtures/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.831165 ghga_connector-0.3.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.831165 ghga_connector-0.3.9/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/integration/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.835165 ghga_connector-0.3.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:02:04.835165 ghga_connector-0.3.9/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/unit/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/unit/test_api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-18 15:01:54.000000 ghga_connector-0.3.9/tests/unit/test_file_operations.py
```

### Comparing `ghga_connector-0.3.8/LICENSE` & `ghga_connector-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/PKG-INFO` & `ghga_connector-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_connector
-Version: 0.3.8
+Version: 0.3.9
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.8
+docker pull ghga/ghga-connector:0.3.9
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.8 .
+docker build -t ghga/ghga-connector:0.3.9 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.8 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.9 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_connector-0.3.8/README.md` & `ghga_connector-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,29 +24,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.8
+docker pull ghga/ghga-connector:0.3.9
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.8 .
+docker build -t ghga/ghga-connector:0.3.9 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.8 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.9 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_connector-0.3.8/ghga_connector/__init__.py` & `ghga_connector-0.3.9/ghga_connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 CLI - Client to perform up- and download operations to and from a local ghga instance
 """
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `ghga_connector-0.3.8/ghga_connector/__main__.py` & `ghga_connector-0.3.9/ghga_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/cli.py` & `ghga_connector-0.3.9/ghga_connector/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 #
 
 """ CLI-specific wrappers around core functions."""
 
 import os
 import sys
 from distutils.util import strtobool
+from functools import partial
 from pathlib import Path
+from types import TracebackType
+from typing import Union
 
 import crypt4gh.keys
 import typer
 from ghga_service_commons.utils import crypt
 
 from ghga_connector import core
 from ghga_connector.config import Config
@@ -52,14 +55,33 @@
     def failure(self, message: str):
         """
         Write message to stderr representing information about a failed operation
         """
         typer.secho(message, fg=core.MessageColors.FAILURE, err=True)
 
 
+def exception_hook(
+    type_: BaseException,  # pylint: disable=unused-argument
+    value: BaseException,
+    traceback: Union[TracebackType, None],  # pylint: disable=unused-argument
+    message_display: CLIMessageDisplay,
+):
+    """When debug mode is NOT enabled, gets called to perform final error handling
+    before program exits"""
+    message = (
+        "An error occurred. Rerun command"
+        + " with --debug at the end to see more information."
+    )
+
+    if value.args:
+        message = value.args[0]
+
+    message_display.failure(message)
+
+
 cli = typer.Typer(no_args_is_help=True)
 
 
 def upload(  # noqa C901
     *,
     file_id: str = typer.Option(..., help="The id of the file to upload"),
     file_path: Path = typer.Option(..., help="The path to the file to upload"),
@@ -76,16 +98,18 @@
     debug: bool = typer.Option(
         False, help="Set this option in order to view traceback for errors."
     ),
 ):
     """
     Command to upload a file
     """
+    message_display = CLIMessageDisplay()
+
     if not debug:
-        sys.excepthook = lambda x, y, z: None
+        sys.excepthook = partial(exception_hook, message_display=message_display)
 
     core.HttpxClientState.configure(CONFIG.max_retries)
 
     wkvs_caller = core.WKVSCaller(CONFIG.wkvs_api_url)
     server_pubkey = wkvs_caller.get_server_pubkey()
     ucs_api_url = wkvs_caller.get_ucs_api_url()
 
@@ -124,41 +148,41 @@
     debug: bool = typer.Option(
         False, help="Set this option in order to view traceback for errors."
     ),
 ):
     """
     Command to download files
     """
-    if not debug:
-        sys.excepthook = lambda x, y, z: None
 
     core.HttpxClientState.configure(CONFIG.max_retries)
     message_display = CLIMessageDisplay()
 
+    if not debug:
+        sys.excepthook = partial(exception_hook, message_display=message_display)
+
     if not my_public_key_path.is_file():
-        message_display.failure(f"The file '{my_public_key_path}' does not exist.")
         raise core.exceptions.PubKeyFileDoesNotExistError(
             pubkey_path=my_public_key_path
         )
 
     if not output_dir.is_dir():
-        message_display.failure(f"The directory '{output_dir}' does not exist.")
-        raise core.exceptions.DirectoryDoesNotExistError(output_dir=output_dir)
+        raise core.exceptions.DirectoryDoesNotExistError(directory=output_dir)
 
     my_public_key = crypt4gh.keys.get_public_key(filepath=my_public_key_path)
     my_private_key = crypt4gh.keys.get_private_key(
         filepath=my_private_key_path, callback=None
     )
 
     # get work package access token and id from user input, will be used in later PR
     work_package_id, work_package_token = core.main.get_wps_token(
         max_tries=3, message_display=message_display
     )
     decrypted_token = crypt.decrypt(data=work_package_token, key=my_private_key)
 
+    message_display.display("Retrieving API configuration information...")
     wkvs_caller = core.WKVSCaller(CONFIG.wkvs_api_url)
     wps_api_url = wkvs_caller.get_wps_api_url()
     dcs_api_url = wkvs_caller.get_dcs_api_url()
 
     work_package_accessor = core.WorkPackageAccessor(
         access_token=decrypted_token,
         api_url=wps_api_url,
@@ -181,14 +205,15 @@
         staging_parameters=staging_parameters,
         work_package_accessor=work_package_accessor,
     )
     file_stager.check_and_stage(output_dir=output_dir)
 
     while file_stager.file_ids_remain():
         for file_id in file_stager.get_staged():
+            message_display.display(f"Downloading file with id '{file_id}'...")
             core.download(
                 api_url=dcs_api_url,
                 file_id=file_id,
                 file_extension=file_ids_with_extension[file_id],
                 output_dir=output_dir,
                 max_wait_time=CONFIG.max_wait_time,
                 part_size=CONFIG.part_size,
@@ -218,66 +243,72 @@
     ),
     debug: bool = typer.Option(
         False, help="Set this option in order to view traceback for errors."
     ),
 ):
     """Command to decrypt a downloaded file"""
 
-    if not debug:
-        sys.excepthook = lambda x, y, z: None
-
     message_display = CLIMessageDisplay()
 
+    if not debug:
+        sys.excepthook = partial(exception_hook, message_display=message_display)
+
     if not input_dir.is_dir():
-        message_display.failure(
-            f"Input directory '{input_dir}' does not exist or is not a directory."
-        )
+        raise core.exceptions.DirectoryDoesNotExistError(directory=input_dir)
 
     if not output_dir:
         output_dir = Path(os.getcwd())
 
     if output_dir.exists() and not output_dir.is_dir():
-        message_display.failure(
-            f"Output directory location '{input_dir}' exists, but is not a directory."
-        )
+        raise core.exceptions.OutputPathIsNotDirectory(directory=output_dir)
 
     if not output_dir.exists():
+        message_display.display(f"Creating output directory '{output_dir}'")
         output_dir.mkdir(parents=True)
 
     errors = {}
     skipped_files = []
+    file_count = 0
     for input_file in input_dir.iterdir():
         if not input_file.is_file() or not input_file.suffix == ".c4gh":
             skipped_files.append((str(input_file)))
             continue
 
+        file_count += 1
+
         # strip the .c4gh extension for the output file
         output_file = output_dir / input_file.with_suffix("")
 
         if output_file.exists():
             errors[
                 str(input_file)
             ] = f"File already exists at '{output_file}', will not overwrite."
             continue
 
         try:
+            message_display.display(f"Decrypting file with id '{input_file}'...")
             core.decrypt_file(
                 input_file=input_file,
                 output_file=output_file,
                 decryption_private_key_path=decryption_private_key_path,
             )
         except ValueError as error:
             errors[
                 str(input_file)
             ] = f"Could not decrypt the provided file with the given key.\nError: {str(error)}"
             continue
 
         message_display.success(
             f"Successfully decrypted file '{input_file}' to location '{output_dir}'."
         )
+    if file_count == 0:
+        message_display.display(
+            f"No files were processed because the directory '{input_dir}' contains no "
+            + "applicable files."
+        )
 
     if skipped_files:
         message_display.display(
             "The following files were skipped as they are not .c4gh files:"
         )
         for file in skipped_files:
             message_display.display(f"- {file}")
```

### Comparing `ghga_connector-0.3.8/ghga_connector/config.py` & `ghga_connector-0.3.9/ghga_connector/config.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/__init__.py` & `ghga_connector-0.3.9/ghga_connector/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/api_calls/__init__.py` & `ghga_connector-0.3.9/ghga_connector/core/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/api_calls/download.py` & `ghga_connector-0.3.9/ghga_connector/core/api_calls/download.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/api_calls/upload.py` & `ghga_connector-0.3.9/ghga_connector/core/api_calls/upload.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/api_calls/utils.py` & `ghga_connector-0.3.9/ghga_connector/core/api_calls/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/api_calls/well_knowns.py` & `ghga_connector-0.3.9/ghga_connector/core/api_calls/well_knowns.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/api_calls/work_package.py` & `ghga_connector-0.3.9/ghga_connector/core/api_calls/work_package.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/batch_processing.py` & `ghga_connector-0.3.9/ghga_connector/core/batch_processing.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/client.py` & `ghga_connector-0.3.9/ghga_connector/core/client.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/constants.py` & `ghga_connector-0.3.9/ghga_connector/core/constants.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/exceptions.py` & `ghga_connector-0.3.9/ghga_connector/core/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,104 +30,113 @@
         message = "Aborting batch process"
         super().__init__(message)
 
 
 class DirectoryDoesNotExistError(RuntimeError):
     """Thrown, when the specified directory does not exist."""
 
-    def __init__(self, *, output_dir: Path):
-        message = f"The directory {output_dir} does not exist."
+    def __init__(self, *, directory: Path):
+        message = f"The directory '{directory}' does not exist."
+        super().__init__(message)
+
+
+class OutputPathIsNotDirectory(RuntimeError):
+    """Thrown when specified output path is not a directory"""
+
+    def __init__(self, *, directory: Path):
+        message = (
+            f"Path of output directory '{directory}' exists, but is not a directory."
+        )
         super().__init__(message)
 
 
 class FileAlreadyExistsError(RuntimeError):
     """Thrown, when the specified file already exists."""
 
     def __init__(self, *, output_file: str):
-        message = f"The file {output_file} already exists."
+        message = f"The file '{output_file}' already exists."
         super().__init__(message)
 
 
 class FileAlreadyEncryptedError(RuntimeError):
     """Thrown, when the specified file is already encrypted."""
 
     def __init__(self, *, file_path: Path):
-        message = f"The file {file_path} is already Crypt4GH encrypted."
+        message = (
+            f"The file '{file_path}' is already Crypt4GH encrypted. Provide data "
+            + "without Crypt4GH encryption."
+        )
         super().__init__(message)
 
 
 class FileDoesNotExistError(RuntimeError):
     """Thrown, when the specified file does not exist."""
 
     def __init__(self, *, file_path: Path):
-        message = f"The file {file_path} does not exist."
+        message = f"The file '{file_path}' does not exist."
         super().__init__(message)
 
 
 class PubKeyFileDoesNotExistError(RuntimeError):
     """Thrown, when the specified public key file does not exist."""
 
     def __init__(self, *, pubkey_path: Path):
-        message = f"The public key file {pubkey_path} does not exist."
+        message = f"The public key file '{pubkey_path}' does not exist."
         super().__init__(message)
 
 
 class PubKeyMismatchError(RuntimeError):
     """
     Thrown when the user public key announced in the submission metadata retrieved from
     the work package service does not match the user public key provided to the connector
     """
 
     def __init__(self):
-        message = (
-            "Provided user public key does not match the announced user public key."
-        )
+        message = "Provided public key does not match the public key from the metadata."
         super().__init__(message)
 
 
 class PrivateKeyFileDoesNotExistError(RuntimeError):
     """Thrown, when the specified private key file does exist."""
 
     def __init__(self, *, private_key_path: Path):
-        message = f"The private key file {private_key_path} does not exist."
+        message = f"The private key file '{private_key_path}' does not exist."
         super().__init__(message)
 
 
 class ApiNotReachableError(RuntimeError):
     """Thrown, when the api is not reachable."""
 
     def __init__(self, *, api_url: str):
-        message = f"The url {api_url} is currently not reachable."
+        message = f"The url '{api_url}' is currently not reachable."
         super().__init__(message)
 
 
 class RetryTimeExpectedError(RuntimeError):
     """Thrown, when a request didn't contain a retry time even though it was expected."""
 
     def __init__(self, *, url: str):
-        message = (
-            f"No `Retry-After` header in response from server following the url: {url}"
-        )
+        message = f"No `Retry-After` header in response from server following the url: '{url}'"
         super().__init__(message)
 
 
 class RequestFailedError(RuntimeError):
     """Thrown, when a request fails without returning a response code"""
 
     def __init__(self, *, url: str):
-        message = f"The request to {url} failed."
+        message = f"The request to '{url}' failed."
         super().__init__(message)
 
 
 class NoS3AccessMethodError(RuntimeError):
     """Thrown, when a request returns the desired response code, but no S3 Access
     Method"""
 
     def __init__(self, *, url: str):
-        message = f"The request to {url} did not return an S3 Access Method."
+        message = f"The request to '{url}' did not return an S3 Access Method."
         super().__init__(message)
 
 
 class FileNotRegisteredError(RuntimeError):
     """Thrown, when a request for a file returns a 404 error."""
 
     def __init__(self, *, file_id: str):
@@ -150,68 +159,68 @@
 
 
 class BadResponseCodeError(RuntimeError):
     """Thrown, when a request returns an unexpected response code (e.g. 500)"""
 
     def __init__(self, *, url: str, response_code: int):
         self.response_code = response_code
-        message = f"The request to {url} failed with response code {response_code}."
+        message = f"The request to '{url}' failed with response code {response_code}."
         super().__init__(message)
 
 
 class NoUploadPossibleError(RuntimeError):
     """Thrown, when a multipart upload currently can't be started (response code 400)"""
 
     def __init__(self, *, file_id: str):
         message = (
             "It is not possible to start a multipart upload for file with id "
-            + f"'{file_id}', because this download is already pending or has been "
+            + f"'{file_id}' because this download is already pending or has been "
             + "accepted."
         )
         super().__init__(message)
 
 
 class DownloadFinalizationError(RuntimeError):
     """
     Thrown when a downloaded file cannot be moved to its final location, as another file
     already exists at that location that was not present at the beginning of the batch process
     """
 
     def __init__(self, *, file_path: Path):
         message = (
             "Cannot move downloaded file to its final location as another file "
-            + f"unexpectedly exists at {file_path}"
+            + f"unexpectedly exists at '{file_path}'"
         )
         super().__init__(message)
 
 
 class UserHasNoUploadAccessError(RuntimeError):
     """
     Thrown when a user does not have the credentials to get or change
     details of an ongoing upload with a specific upload id
     (response code 403)
     """
 
     def __init__(self, *, upload_id: str):
         message = (
-            "This user is not registered as the data submitter "
+            "You are not registered as a Data Submitter "
             f"for the file corresponding to the upload_id '{upload_id}'."
         )
         super().__init__(message)
 
 
 class UserHasNoFileAccessError(RuntimeError):
     """
     Thrown when a user does not have the credentials for
     a specific file id (response code 403)
     """
 
     def __init__(self, *, file_id: str):
         message = (
-            "This user is not registered as the data submitter "
+            "You are not registered as the data submitter "
             f"for the file with the id '{file_id}'."
         )
         super().__init__(message)
 
 
 class CantChangeUploadStatusError(RuntimeError):
     """
@@ -225,23 +234,23 @@
 
 
 class MaxWaitTimeExceededError(RuntimeError):
     """Thrown, when the specified wait time for getting a download url has been
     exceeded."""
 
     def __init__(self, *, max_wait_time: int):
-        message = f"Exceeded maximum wait time of {max_wait_time} seconds."
+        message = f"Exceeded maximum wait time of ({max_wait_time}) seconds."
         super().__init__(message)
 
 
 class ConnectionFailedError(RuntimeError):
     """Thrown, when a ConnectError or ConnectTimeout error is raised by httpx"""
 
     def __init__(self, *, url: str, reason: str):
-        message = f"Request to {url} failed to connect. Reason: {reason}"
+        message = f"Request to '{url}' failed to connect. Reason: {reason}"
         super().__init__(message)
 
 
 class MaxPartNoExceededError(RuntimeError):
     """
     Thrown requesting a part number larger than the maximally possible number of parts.
 
@@ -280,15 +289,15 @@
         super().__init__(message)
 
 
 class InvalidWorkPackageToken(RuntimeError):
     """Thrown, when the work package string pasted by the user could not be parsed"""
 
     def __init__(self, *, tries: int):
-        message = f"Parsing of the work package string failed {tries} times."
+        message = f"Parsing of the work package string failed ({tries}) times."
         super().__init__(message)
 
 
 class NoWorkPackageAccessError(RuntimeError):
     """
     Thrown when the given auth token does not provide access for
     a specific work package id (response code 403)
@@ -307,27 +316,27 @@
     Thrown when communication with the Work Package Service returns an unexpected response.
     This should be used instead of BadResponseError when handling WPS results to differentiate.
     """
 
     def __init__(self, *, url: str, response_code: int):
         self.response_code = response_code
         message = (
-            f"The request to the WPS at {url} failed with an unexpected response code "
+            f"The request to the WPS at '{url}' failed with an unexpected response code "
             + f"of {response_code}."
         )
         super().__init__(message)
 
 
 class UnauthorizedAPICallError(RuntimeError):
     """
     Thrown when a 403 is returned from a call requiring a work order token for authorization
     """
 
     def __init__(self, *, url: str, cause: str):
-        message = f"Could not authorize call to {url}: {cause}"
+        message = f"Could not authorize call to '{url}': {cause}"
         super().__init__(message)
 
 
 class WellKnownValueNotFound(RuntimeError):
     """
     Thrown when a 404 is returned from a call to the well-known-value-service for a
     specific value name.
```

### Comparing `ghga_connector-0.3.8/ghga_connector/core/file_operations.py` & `ghga_connector-0.3.9/ghga_connector/core/file_operations.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/http_translation.py` & `ghga_connector-0.3.9/ghga_connector/core/http_translation.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector/core/message_display.py` & `ghga_connector-0.3.9/ghga_connector/core/message_display.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/ghga_connector.egg-info/PKG-INFO` & `ghga_connector-0.3.9/ghga_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-connector
-Version: 0.3.8
+Version: 0.3.9
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.8
+docker pull ghga/ghga-connector:0.3.9
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.8 .
+docker build -t ghga/ghga-connector:0.3.9 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.8 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.9 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_connector-0.3.8/ghga_connector.egg-info/SOURCES.txt` & `ghga_connector-0.3.9/ghga_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/scripts/__init__.py` & `ghga_connector-0.3.9/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/scripts/get_package_name.py` & `ghga_connector-0.3.9/scripts/get_package_name.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/scripts/license_checker.py` & `ghga_connector-0.3.9/scripts/license_checker.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/scripts/script_utils/__init__.py` & `ghga_connector-0.3.9/scripts/script_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/scripts/script_utils/cli.py` & `ghga_connector-0.3.9/scripts/script_utils/cli.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/scripts/update_config_docs.py` & `ghga_connector-0.3.9/scripts/update_config_docs.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/scripts/update_readme.py` & `ghga_connector-0.3.9/scripts/update_readme.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/scripts/update_template_files.py` & `ghga_connector-0.3.9/scripts/update_template_files.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/setup.cfg` & `ghga_connector-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/setup.py` & `ghga_connector-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/fixtures/__init__.py` & `ghga_connector-0.3.9/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/fixtures/config.py` & `ghga_connector-0.3.9/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/fixtures/endpoints_handler.py` & `ghga_connector-0.3.9/tests/fixtures/endpoints_handler.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/fixtures/mock_api/__init__.py` & `ghga_connector-0.3.9/tests/fixtures/mock_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/fixtures/mock_api/app.py` & `ghga_connector-0.3.9/tests/fixtures/mock_api/app.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/fixtures/s3.py` & `ghga_connector-0.3.9/tests/fixtures/s3.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/fixtures/state.py` & `ghga_connector-0.3.9/tests/fixtures/state.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/fixtures/utils.py` & `ghga_connector-0.3.9/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/integration/__init__.py` & `ghga_connector-0.3.9/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/integration/fixtures/__init__.py` & `ghga_connector-0.3.9/tests/integration/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/integration/fixtures/utils.py` & `ghga_connector-0.3.9/tests/integration/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/integration/test_cli.py` & `ghga_connector-0.3.9/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/integration/test_file_operations.py` & `ghga_connector-0.3.9/tests/integration/test_file_operations.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/unit/__init__.py` & `ghga_connector-0.3.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/unit/fixtures/__init__.py` & `ghga_connector-0.3.9/tests/unit/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/unit/fixtures/utils.py` & `ghga_connector-0.3.9/tests/unit/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/unit/test_api_calls.py` & `ghga_connector-0.3.9/tests/unit/test_api_calls.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/unit/test_core.py` & `ghga_connector-0.3.9/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.8/tests/unit/test_file_operations.py` & `ghga_connector-0.3.9/tests/unit/test_file_operations.py`

 * *Files identical despite different names*

