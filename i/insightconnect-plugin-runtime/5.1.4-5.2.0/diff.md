# Comparing `tmp/insightconnect-plugin-runtime-5.1.4.tar.gz` & `tmp/insightconnect-plugin-runtime-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insightconnect-plugin-runtime-5.1.4.tar", last modified: Mon Jun 19 09:16:22 2023, max compression
+gzip compressed data, was "insightconnect-plugin-runtime-5.2.0.tar", last modified: Tue Jul 18 14:37:47 2023, max compression
```

## Comparing `insightconnect-plugin-runtime-5.1.4.tar` & `insightconnect-plugin-runtime-5.2.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.365905 insightconnect-plugin-runtime-5.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-19 09:16:22.365905 insightconnect-plugin-runtime-5.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-06-19 09:15:32.000000 insightconnect-plugin-runtime-5.1.4/insightconnect-plugin-swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.353905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/action.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26847 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/input_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/output_message_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21108 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.353905 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-19 09:16:22.000000 insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 09:16:22.365905 insightconnect-plugin-runtime-5.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
--rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.357905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.361905 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:16:22.365905 insightconnect-plugin-runtime-5.1.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_aws_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_custom_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_server_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-19 09:14:13.000000 insightconnect-plugin-runtime-5.1.4/tests/unit/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.711065 insightconnect-plugin-runtime-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-18 14:37:47.711065 insightconnect-plugin-runtime-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-07-18 14:37:07.000000 insightconnect-plugin-runtime-5.2.0/insightconnect-plugin-swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.703065 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26847 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/clients/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/clients/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/data/input_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/data/output_message_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.703065 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-18 14:37:47.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-18 14:37:47.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:37:47.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-18 14:37:47.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 14:37:47.000000 insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:37:47.711065 insightconnect-plugin-runtime-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      631 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      375 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      944 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.707065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.711065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.711065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.711065 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/test_hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:47.711065 insightconnect-plugin-runtime-5.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_aws_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_custom_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_server_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 14:36:13.000000 insightconnect-plugin-runtime-5.2.0/tests/unit/test_variables.py
```

### Comparing `insightconnect-plugin-runtime-5.1.4/PKG-INFO` & `insightconnect-plugin-runtime-5.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.1.4
+Version: 5.2.0
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.2.0 - Add `status_code` and `exception` properties to task output
 * 5.1.4 - Fix credential masking when connection is null
 * 5.1.3 - Fix credential masking when some input fields are empty
 * 5.1.2 - Add connection credential masking to the plugin's output and log when displayed as plain text | Add new `OutputMasker` class to handle credential masking    
 * 5.1.1 - Updated exception preset messages
 * 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
```

### Comparing `insightconnect-plugin-runtime-5.1.4/README.md` & `insightconnect-plugin-runtime-5.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.2.0 - Add `status_code` and `exception` properties to task output
 * 5.1.4 - Fix credential masking when connection is null
 * 5.1.3 - Fix credential masking when some input fields are empty
 * 5.1.2 - Add connection credential masking to the plugin's output and log when displayed as plain text | Add new `OutputMasker` class to handle credential masking    
 * 5.1.1 - Updated exception preset messages
 * 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
```

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect-plugin-swagger.json` & `insightconnect-plugin-runtime-5.2.0/insightconnect-plugin-swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -450,114 +450,114 @@
     "definitions": {
         "PluginInfo": {
             "type": "object",
             "properties": {
                 "support": {
                     "type": "string"
                 },
-                "version": {
-                    "type": "string"
-                },
-                "vendor": {
-                    "type": "string"
+                "enable_cache": {
+                    "type": "boolean"
                 },
                 "plugin_spec_version": {
                     "type": "string"
                 },
-                "description": {
+                "number_of_workers": {
+                    "type": "integer",
+                    "format": "int32"
+                },
+                "version": {
                     "type": "string"
                 },
                 "tags": {
                     "type": "array",
                     "items": {
                         "type": "string"
                     }
                 },
-                "number_of_workers": {
+                "threads": {
                     "type": "integer",
                     "format": "int32"
                 },
                 "sdk_version": {
                     "type": "string"
                 },
-                "name": {
+                "description": {
                     "type": "string"
                 },
-                "title": {
+                "vendor": {
                     "type": "string"
                 },
-                "threads": {
-                    "type": "integer",
-                    "format": "int32"
+                "name": {
+                    "type": "string"
                 },
-                "enable_cache": {
-                    "type": "boolean"
+                "title": {
+                    "type": "string"
                 }
             }
         },
         "ActionTriggerOutputBody": {
             "type": "object",
             "properties": {
-                "status": {
-                    "type": "string"
-                },
-                "log": {
-                    "type": "string"
-                },
                 "output": {
                     "type": "object"
                 },
                 "meta": {
                     "type": "object"
+                },
+                "log": {
+                    "type": "string"
+                },
+                "status": {
+                    "type": "string"
                 }
             },
             "required": [
                 "log",
                 "meta",
                 "output",
                 "status"
             ]
         },
         "ActionTriggerOutput": {
             "type": "object",
             "properties": {
+                "body": {
+                    "$ref": "#/definitions/ActionTriggerOutputBody"
+                },
+                "version": {
+                    "type": "string"
+                },
                 "type": {
                     "type": "string",
                     "enum": [
                         "action_event",
                         "trigger_event"
                     ]
-                },
-                "version": {
-                    "type": "string"
-                },
-                "body": {
-                    "$ref": "#/definitions/ActionTriggerOutputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "TaskOutputBody": {
             "type": "object",
             "properties": {
-                "state": {
-                    "type": "object"
-                },
                 "output": {
                     "type": "object"
                 },
+                "status": {
+                    "type": "string"
+                },
                 "meta": {
                     "type": "object"
                 },
-                "status": {
-                    "type": "string"
+                "state": {
+                    "type": "object"
                 },
                 "log": {
                     "type": "string"
                 }
             },
             "required": [
                 "log",
@@ -566,183 +566,183 @@
                 "state",
                 "status"
             ]
         },
         "TaskOutput": {
             "type": "object",
             "properties": {
+                "body": {
+                    "$ref": "#/definitions/TaskOutputBody"
+                },
+                "version": {
+                    "type": "string"
+                },
                 "type": {
                     "type": "string",
                     "enum": [
                         "task_event"
                     ]
-                },
-                "version": {
-                    "type": "string"
-                },
-                "body": {
-                    "$ref": "#/definitions/TaskOutputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "ActionTriggerInputBody": {
             "type": "object",
             "properties": {
-                "connection": {
-                    "type": "object"
+                "action": {
+                    "type": "string"
                 },
                 "input": {
                     "type": "object"
                 },
-                "action": {
-                    "type": "string"
+                "connection": {
+                    "type": "object"
                 }
             },
             "required": [
                 "action",
                 "connection",
                 "input"
             ]
         },
         "ActionTriggerInput": {
             "type": "object",
             "properties": {
+                "body": {
+                    "$ref": "#/definitions/ActionTriggerInputBody"
+                },
+                "version": {
+                    "type": "string"
+                },
                 "type": {
                     "type": "string",
                     "enum": [
                         "action_event",
                         "trigger_event"
                     ]
-                },
-                "version": {
-                    "type": "string"
-                },
-                "body": {
-                    "$ref": "#/definitions/ActionTriggerInputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "TaskInputBody": {
             "type": "object",
             "properties": {
-                "connection": {
-                    "type": "object"
-                },
                 "task": {
                     "type": "string"
                 },
+                "state": {
+                    "type": "object"
+                },
                 "input": {
                     "type": "object"
                 },
-                "state": {
+                "connection": {
                     "type": "object"
                 }
             },
             "required": [
                 "connection",
                 "input",
                 "state",
                 "task"
             ]
         },
         "TaskInput": {
             "type": "object",
             "properties": {
+                "body": {
+                    "$ref": "#/definitions/TaskInputBody"
+                },
+                "version": {
+                    "type": "string"
+                },
                 "type": {
                     "type": "string",
                     "enum": [
                         "task_event"
                     ]
-                },
-                "version": {
-                    "type": "string"
-                },
-                "body": {
-                    "$ref": "#/definitions/TaskInputBody"
                 }
             },
             "required": [
                 "body",
                 "type",
                 "version"
             ]
         },
         "ActionTriggerDetails": {
             "type": "object",
             "properties": {
                 "output": {
                     "type": "object"
                 },
-                "description": {
-                    "type": "string"
-                },
                 "title": {
                     "type": "string"
                 },
                 "input": {
                     "type": "object"
+                },
+                "description": {
+                    "type": "string"
                 }
             }
         },
         "ConnectionDetails": {
             "type": "object",
             "properties": {
                 "type": {
                     "type": "string"
                 },
-                "properties": {
-                    "type": "object"
-                },
-                "title": {
-                    "type": "string"
-                },
                 "required": {
                     "type": "array",
                     "items": {
                         "type": "string"
                     }
+                },
+                "title": {
+                    "type": "string"
+                },
+                "properties": {
+                    "type": "object"
                 }
             }
         },
         "ConnectionTestOutput": {
             "type": "object",
             "properties": {
                 "message": {
                     "type": "object"
                 }
             }
         },
         "TaskDetails": {
             "type": "object",
             "properties": {
-                "input": {
+                "output": {
                     "type": "object"
                 },
                 "state": {
                     "type": "object"
                 },
-                "description": {
-                    "type": "string"
-                },
-                "output": {
+                "input": {
                     "type": "object"
                 },
                 "schedule": {
                     "type": "object"
                 },
+                "description": {
+                    "type": "string"
+                },
                 "title": {
                     "type": "string"
                 }
             }
         }
     }
 }
```

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/__init__.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/endpoints.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/api/schemas.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/api/schemas.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/cli.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/aws_client.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/clients/aws_client.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/clients/oauth.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/clients/oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/connection.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/connection.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/input_message_schema.json` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/data/input_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/data/output_message_schema.json` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/data/output_message_schema.json`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/dispatcher.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/dispatcher.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/exceptions.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/helper.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/helper.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/metrics.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/plugin.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,28 +180,32 @@
         input_message,
         log,
         success,
         output,
         error_message,
         state,
         has_more_pages,
+        status_code,
+        error_object,
         ex: None,
         is_test: False,
     ):
         """
         Creates an output message of a step's execution.
 
         :param message_type: The message type
         :param input_message: The input message
         :param log: The log of the step, as a single string
         :param success: whether or not the step was successful
         :param output: The step data output
         :param error_message: An error message if an error was thrown
         :param state: The state of task_event. Only applicable to tasks.
         :param has_more_pages: Whether or not a task_event has more pages to be consumed. Only applicable to tasks.
+        :param status_code: Contains the status code of requests. Only applicable to tasks.
+        :param error_object: Contains the error object if any error occurs. Only applicable to tasks.
         :param ex: An error that was thrown
         :param is_test: whether or not the step is part of a Connection Test
         :return: An output message
         """
 
         output_message = {
             "log": log,
@@ -211,14 +215,24 @@
 
         if state is not None:
             output_message["state"] = state
 
         if has_more_pages is not None:
             output_message["has_more_pages"] = has_more_pages
 
+        if status_code is not None:
+            output_message["status_code"] = status_code
+
+        if error_object is not None and isinstance(error_object, (ConnectionTestException, PluginException)):
+            output_message["exception"] = {
+                "cause": error_object.cause,
+                "assistance": error_object.assistance,
+                "data": error_object.data,
+            }
+
         if success:
             output_message["output"] = output
         else:
             output_message["error"] = error_message
 
             if ex:
                 if isinstance(ex, ConnectionTestException):
@@ -367,14 +381,16 @@
         caught_exception = None
         output = None
         out_type = None
 
         # Properties specific to tasks
         state = None
         has_more_pages = None
+        status_code = None
+        error_object = None
 
         try:
             # Attempt to grab message type first
             message_type = input_message.get("type")
             out_type = message_output_type.get(message_type)
             if message_type not in [
                 "action_start",
@@ -417,15 +433,15 @@
                         "task",
                         logger,
                         log_stream,
                         is_test,
                         is_debug,
                     )
                 else:
-                    output, state, has_more_pages = self.start_step(
+                    output, state, has_more_pages, status_code, error_object = self.start_step(
                         input_message["body"],
                         "task",
                         logger,
                         log_stream,
                         is_test,
                         is_debug,
                     )
@@ -450,14 +466,16 @@
                 input_message,
                 log_stream.getvalue(),
                 success,
                 output,
                 str(caught_exception),
                 state,
                 has_more_pages,
+                status_code,
+                error_object,
                 caught_exception,
                 is_test,
             )
             if not success:
                 raise LoggedException(caught_exception, output)
             return output
 
@@ -528,14 +546,16 @@
                         step.dispatcher = Stdout(message_body["dispatcher"])
                     else:
                         step.dispatcher = Http(message_body["dispatcher"])
 
             params = message_body["input"]
             state = {}
             has_more_pages = None
+            status_code = None
+            error_object = None
 
             if not is_test:
                 # Validate input message
                 try:
                     step.input.validate(params)
                     if step_key == "task":
                         state = message_body["state"]
@@ -575,25 +595,25 @@
 
             # Backward compatibility with steps with missing argument params
             # The SDK has always defined the signature of the run/test methods to include the params dictionary.
             # However, the code generation generates the test method without the params argument.
             parameters = inspect.signature(func)
             if len(parameters.parameters) > 0:
                 if step_key == "task" and not is_test:
-                    output, state, has_more_pages = func(params, state)
+                    output, state, has_more_pages, status_code, error_object = func(params, state)
                 else:
                     output = func(params)
             else:
                 if step_key == "task" and not is_test:
-                    output, state, has_more_pages = func()
+                    output, state, has_more_pages, status_code, error_object = func()
                 else:
                     output = func()
 
             # Don't validate output for any test functions - action/trigger tests shouldn't be validated due to them
             # not providing value and a connection test shouldn't be validated due to it being generic/universal
             if not is_test:
                 step.output.validate(output)
 
             if step_key == "task" and not is_test:
-                return output, state, has_more_pages
+                return output, state, has_more_pages, status_code, error_object
 
             return output
```

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/schema.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/server.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/server.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/step.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/step.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/trigger.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/util.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/util.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime/variables.py` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime/variables.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/PKG-INFO` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-plugin-runtime
-Version: 5.1.4
+Version: 5.2.0
 Summary: InsightConnect Plugin Runtime
 Home-page: https://github.com/rapid7/komand-plugin-sdk-python
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -150,14 +150,15 @@
 Contributions for maintaining and enhancing the InsightConnect Python Plugin Runtime are appreciated. This project uses
 [Black](https://github.com/psf/black) for code formatting and includes a pre-commit hook to auto format code as it is
 contributed. Black is installed as a test dependency and the hook can be initialized by running `pre-commit install` 
 after cloning this repository.
 
 ## Changelog
 
+* 5.2.0 - Add `status_code` and `exception` properties to task output
 * 5.1.4 - Fix credential masking when connection is null
 * 5.1.3 - Fix credential masking when some input fields are empty
 * 5.1.2 - Add connection credential masking to the plugin's output and log when displayed as plain text | Add new `OutputMasker` class to handle credential masking    
 * 5.1.1 - Updated exception preset messages
 * 5.1.0 - Add new helper functions
 * 5.0.0 - Add `has_more_pages` property to task output to indicate task pagination status to output consumers
 * 4.10.1 - Remove raising of exception if request id is not available in header
```

### Comparing `insightconnect-plugin-runtime-5.1.4/insightconnect_plugin_runtime.egg-info/SOURCES.txt` & `insightconnect-plugin-runtime-5.2.0/insightconnect_plugin_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/setup.py` & `insightconnect-plugin-runtime-5.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="insightconnect-plugin-runtime",
-    version="5.1.4",
+    version="5.2.0",
     description="InsightConnect Plugin Runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Rapid7 Integrations Alliance",
     author_email="integrationalliance@rapid7.com",
     url="https://github.com/rapid7/komand-plugin-sdk-python",
     packages=find_packages(),
```

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/__init__.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/__init__.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/hello/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/return_bad_json/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/actions/throw_exception/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/connection/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/hello_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/return_bad_json_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/hello_world/komand_hello_world/triggers/throw_exception_trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/conftest.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_cli.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_hello_world.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/plugin/hello_world/tests/test_server.py` & `insightconnect-plugin-runtime-5.2.0/tests/plugin/hello_world/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_action.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_aws_action.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_aws_action.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_custom_encoder.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_endpoints.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_exceptions.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_helpers.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_metrics.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_oauth.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_oauth.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_plugin.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_schema.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_server_spec.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_server_spec.py`

 * *Files identical despite different names*

### Comparing `insightconnect-plugin-runtime-5.1.4/tests/unit/test_trigger.py` & `insightconnect-plugin-runtime-5.2.0/tests/unit/test_trigger.py`

 * *Files identical despite different names*

