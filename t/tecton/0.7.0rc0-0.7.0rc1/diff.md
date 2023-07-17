# Comparing `tmp/tecton-0.7.0rc0.tar.gz` & `tmp/tecton-0.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecton-0.7.0rc0.tar", last modified: Fri Jul 14 21:47:32 2023, max compression
+gzip compressed data, was "tecton-0.7.0rc1.tar", last modified: Mon Jul 17 21:57:01 2023, max compression
```

## Comparing `tecton-0.7.0rc0.tar` & `tecton-0.7.0rc1.tar`

### file list

```diff
@@ -1,555 +1,555 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.617556 tecton-0.7.0rc0/
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      159 2023-07-14 21:47:27.000000 tecton-0.7.0rc0/MANIFEST.in
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3890 2023-07-14 21:47:32.617556 tecton-0.7.0rc0/PKG-INFO
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2023-07-14 21:47:27.000000 tecton-0.7.0rc0/README.md
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.561551 tecton-0.7.0rc0/protoc_gen_swagger/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/protoc_gen_swagger/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.561551 tecton-0.7.0rc0/protoc_gen_swagger/options/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/protoc_gen_swagger/options/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2657 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/protoc_gen_swagger/options/annotations_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16494 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/protoc_gen_swagger/options/openapiv2_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-07-14 21:47:32.621557 tecton-0.7.0rc0/setup.cfg
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2094 2023-07-14 21:47:27.000000 tecton-0.7.0rc0/setup.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.561551 tecton-0.7.0rc0/tecton/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5361 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.565551 tecton-0.7.0rc0/tecton/_internals/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11143 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/analytics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2259 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/athena_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1169 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/data_frame_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6181 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/delete_keys_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7925 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/display.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      944 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/env_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26511 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/find_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2901 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/ingest_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13125 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/materialization_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      666 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.569552 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      421 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/auth_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/base_stub.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3078 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/error_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3115 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/http_client.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1782 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/request_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/response.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2628 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/service_calls.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      198 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/trace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4147 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/mock_source_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16135 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/query_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.569552 tecton-0.7.0rc0/tecton/_internals/repo/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/repo/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11417 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/repo/function_serialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15439 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/run_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12582 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/sdk_decorators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9019 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/snowflake_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26066 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/spark_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6101 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15669 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4991 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/validations_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       36 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_internals/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      276 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/_stamp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2238 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/aggregation_functions.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.569552 tecton-0.7.0rc0/tecton/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15083 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/access_control.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1574 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/api_key.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34602 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/cli.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4315 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/cli_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6569 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/command.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3009 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14945 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/engine.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25411 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/engine_renderer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3348 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/environment.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/error_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1664 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/printer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5832 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/service_account.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1312 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/user.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6859 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/workspace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      670 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/cli/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/fco_listers.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.573552 tecton-0.7.0rc0/tecton/framework/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7294 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/base_tecton_object.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      810 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/compute_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    89131 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/configs.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20716 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/data_frame.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31660 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10597 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/dataset.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7485 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/entity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34112 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/feature_service.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   165862 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/feature_view.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/filtered_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21844 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/transformation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      673 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/validation_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22879 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/framework/workspace.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.573552 tecton-0.7.0rc0/tecton/identities/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/identities/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/identities/api_keys.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3888 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/identities/credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10498 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/identities/okta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2138 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/pytest_tecton.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/run_api_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3009 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/snowflake_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2730 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/tecton_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3422 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/types.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.573552 tecton-0.7.0rc0/tecton/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.573552 tecton-0.7.0rc0/tecton/vendor/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.573552 tecton-0.7.0rc0/tecton/vendor/dill/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/__diff.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/_objects.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/detect.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/info.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/objtypes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/pointers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/settings.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/dill/dill/temp.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.573552 tecton-0.7.0rc0/tecton/vendor/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.573552 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/clientserver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/finalizer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/java_collections.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/protocol.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/signals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.577552 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/_globals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/accumulators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/broadcast.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.577552 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/cloudpickle/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/daemon.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/files.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/find_spark_home.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/install.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/join.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.581553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/base.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/fpm.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/image.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.581553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.581553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/param/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/param/shared.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/regression.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/stat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/tuning.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/wrapper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.581553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/fpm.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.585553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/random.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/regression.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.585553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/profiler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.585553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/python/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/python/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.585553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/python/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/rdd.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/rddsampler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.585553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resource/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resource/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resource/information.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resource/profile.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resource/requests.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resultiterable.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/shuffle.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.585553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.585553 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/avro/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/catalog.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/column.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/dataframe.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/group.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.589554 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/readwriter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/streaming.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/udf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/window.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/statcounter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/storagelevel.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.589554 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/dstream.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/listener.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/taskcontext.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/traceback_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/worker.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/vendor_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/vendor/vendor_pyspark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1185 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.561551 tecton-0.7.0rc0/tecton.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3890 2023-07-14 21:47:30.000000 tecton-0.7.0rc0/tecton.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19035 2023-07-14 21:47:31.000000 tecton-0.7.0rc0/tecton.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-07-14 21:47:30.000000 tecton-0.7.0rc0/tecton.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2023-07-14 21:47:30.000000 tecton-0.7.0rc0/tecton.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      833 2023-07-14 21:47:31.000000 tecton-0.7.0rc0/tecton.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       95 2023-07-14 21:47:31.000000 tecton-0.7.0rc0/tecton.egg-info/top_level.txt
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.589554 tecton-0.7.0rc0/tecton_athena/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14608 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/athena_session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8482 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/data_catalog_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5747 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/odfv_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6356 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.589554 tecton-0.7.0rc0/tecton_athena/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2291 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17764 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.589554 tecton-0.7.0rc0/tecton_athena/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates/create_table.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3863 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_athena/templates_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.593554 tecton-0.7.0rc0/tecton_core/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13329 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/aggregation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19520 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7206 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/data_types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5415 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4818 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/fco_container.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17300 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/feature_definition_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9765 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/feature_set_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/feature_view_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/filter_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2300 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/function_deserialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      623 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/id_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7393 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/materialization_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6916 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1395 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/online_serving_index.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6304 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/pipeline_common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4393 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/pipeline_sql_builder.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.593554 tecton-0.7.0rc0/tecton_core/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10765 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26314 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8446 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/node_interface.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    66482 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.593554 tecton-0.7.0rc0/tecton_core/query/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2677 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/pandas/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8340 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/pandas/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/pandas/sql.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      610 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9133 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query/sql_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      397 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/query_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4835 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/repo_file_handler.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/request_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1961 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/schema.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5562 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/schema_derivation_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.597554 tecton-0.7.0rc0/tecton_core/specs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      660 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/specs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    38770 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/specs/data_source_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1258 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/specs/entity_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5274 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/specs/feature_service_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30873 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/specs/feature_view_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/specs/tecton_object_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/specs/transformation_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4912 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/specs/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6872 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/time_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.597554 tecton-0.7.0rc0/tecton_core/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.597554 tecton-0.7.0rc0/tecton_core/vendor/treelib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/vendor/treelib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/vendor/treelib/exceptions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/vendor/treelib/misc.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/vendor/treelib/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/vendor/treelib/plugins.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/vendor/treelib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_core/vendor/vendor_treelib.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.597554 tecton-0.7.0rc0/tecton_proto/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.597554 tecton-0.7.0rc0/tecton_proto/amplitude/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/amplitude/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4278 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/amplitude/amplitude_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/amplitude/client_logging_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.597554 tecton-0.7.0rc0/tecton_proto/api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/api/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.597554 tecton-0.7.0rc0/tecton_proto/api/featureservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/api/featureservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    85094 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/api/featureservice/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9207 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/api/featureservice/feature_service_request_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.601555 tecton-0.7.0rc0/tecton_proto/args/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/basic_info_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/data_source_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17760 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3520 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/diff_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/diff_test_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2481 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/fco_args_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4122 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33904 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6463 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/pipeline_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/repo_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4071 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/user_defined_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/version_constraints_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7076 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/args/virtual_data_source_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.601555 tecton-0.7.0rc0/tecton_proto/auth/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/auth/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/auth/acl_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19265 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/auth/authorization_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2935 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/auth/principal_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1922 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/auth/resource_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3027 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/auth/resource_role_assignments_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3544 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/auth/service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.601555 tecton-0.7.0rc0/tecton_proto/canary/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/canary/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/canary/type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/canary/update_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.601555 tecton-0.7.0rc0/tecton_proto/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/cli/repo_diff_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.605555 tecton-0.7.0rc0/tecton_proto/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/aggregation_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/analytics_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/column_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1339 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/container_image_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/data_source_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/data_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/fco_locator_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/framework_version_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1196 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/id_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/pair_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/schema_container_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2070 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/secret_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/common/spark_schema_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.605555 tecton-0.7.0rc0/tecton_proto/consumption/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/consumption/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3289 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/consumption/consumption_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.605555 tecton-0.7.0rc0/tecton_proto/data/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6382 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/batch_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1589 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/data_source_access_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1921 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/fco_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2758 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/fco_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4497 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/feature_store_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15392 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/freshness_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2124 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/fv_materialization_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/hive_metastore_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1971 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/internal_spark_cluster_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5638 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/materialization_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/odfv_compute_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2316 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/onboarding_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1907 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/principal_group_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2696 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/remote_compute_environment_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12187 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/remote_spark_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/saved_feature_data_frame_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4541 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/serving_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9668 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/state_update_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3945 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/stream_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/summary_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2142 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/tecton_api_key_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2358 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9697 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/user_deployment_settings_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/user_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2979 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/virtual_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1743 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/data/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/databricks_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8185 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/dbfs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/execution_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/instance_profiles_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/jobs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/libraries_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1937 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/permissions_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/scim_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/secrets_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/databricks_api/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/dataobs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/dataobs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/dataobs/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/dataobs/expectation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/dataobs/metric_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/dataobs/validation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3569 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/dataobs/validation_task_params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/dataobs/validation_task_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/feature_server/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/feature_server/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/feature_server/configuration/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/feature_server/configuration/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13426 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7654 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/materialization/job_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2598 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/materialization/materialization_states_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13314 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/materialization/materialization_task_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5790 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/materialization/params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2691 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/materialization/spark_cluster_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/materializationjobservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/materializationjobservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14321 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/metadataservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/metadataservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/metadataservice/http_over_grpc_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   107952 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/metadataservice/metadata_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/online_store/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/online_store/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4353 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/online_store/feature_value_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/online_store/status_entry_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/online_store_writer/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/online_store_writer/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/online_store_writer/config_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.609556 tecton-0.7.0rc0/tecton_proto/remoteenvironmentservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/remoteenvironmentservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8041 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.613556 tecton-0.7.0rc0/tecton_proto/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/snowflake/location_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.613556 tecton-0.7.0rc0/tecton_proto/spark_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/spark_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/spark_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7263 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/spark_api/jobs_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.613556 tecton-0.7.0rc0/tecton_proto/spark_common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/spark_common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7339 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/spark_common/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/spark_common/libraries_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.613556 tecton-0.7.0rc0/tecton_proto/validation/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/validation/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_proto/validation/validator_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.613556 tecton-0.7.0rc0/tecton_snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29228 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/pipeline_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7376 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/snowflake_type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32077 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.613556 tecton-0.7.0rc0/tecton_snowflake/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/copier_macro.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/create_temp_table_for_bfv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/delete_orphaned_schemas.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/delete_staged_files.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/historical_features_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/materialized_feature_view.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/offline_materialization_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/online_store_copier.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6695 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/templates_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_snowflake/utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.617556 tecton-0.7.0rc0/tecton_spark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      465 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25652 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2090 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/data_observability.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/data_source_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    35854 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/data_source_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/errors_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      890 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/feature_view_spark_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.617556 tecton-0.7.0rc0/tecton_spark/jars/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/jars/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)  1604241 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/jars/tecton-udfs-spark-3.jar
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4039 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/materialization_plan.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22766 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11048 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/partial_aggregations.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34132 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:32.617556 tecton-0.7.0rc0/tecton_spark/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3054 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/query/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8463 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/query/filter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18310 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/query/join.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1229 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/query/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4229 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/query/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5861 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/query/projection.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5087 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11252 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5410 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/schema_spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2135 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/spark_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1677 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/spark_schema_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4842 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/udf_jar.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2023-07-14 21:47:28.000000 tecton-0.7.0rc0/tecton_spark/udfs.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.870853 tecton-0.7.0rc1/
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      159 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/MANIFEST.in
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3890 2023-07-17 21:57:01.870853 tecton-0.7.0rc1/PKG-INFO
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/README.md
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.810848 tecton-0.7.0rc1/protoc_gen_swagger/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/protoc_gen_swagger/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.810848 tecton-0.7.0rc1/protoc_gen_swagger/options/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/protoc_gen_swagger/options/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2657 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/protoc_gen_swagger/options/annotations_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16494 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/protoc_gen_swagger/options/openapiv2_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-07-17 21:57:01.870853 tecton-0.7.0rc1/setup.cfg
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2094 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.810848 tecton-0.7.0rc1/tecton/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5361 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.814848 tecton-0.7.0rc1/tecton/_internals/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11143 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/analytics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2259 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/athena_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1169 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/data_frame_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6181 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/delete_keys_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7925 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/display.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      944 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/env_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26511 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/find_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2901 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/ingest_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13125 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/materialization_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      666 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.814848 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      421 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/auth_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/base_stub.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3078 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/error_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3115 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/http_client.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1782 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/request_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/response.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2628 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/service_calls.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      198 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/trace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4147 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/mock_source_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16135 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/query_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.818848 tecton-0.7.0rc1/tecton/_internals/repo/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/repo/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11417 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/repo/function_serialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15439 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/run_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12522 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/sdk_decorators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9019 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/snowflake_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26066 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/spark_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6101 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15669 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4991 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/validations_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       36 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_internals/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      274 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/_stamp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2238 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/aggregation_functions.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.818848 tecton-0.7.0rc1/tecton/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15083 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/access_control.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1574 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/api_key.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34602 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/cli.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4315 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/cli_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6569 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/command.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3009 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14945 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/engine.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25411 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/engine_renderer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3348 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/environment.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/error_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1664 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/printer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5832 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/service_account.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1312 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/user.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6859 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/workspace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      670 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/cli/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/fco_listers.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.822849 tecton-0.7.0rc1/tecton/framework/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7294 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/base_tecton_object.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      810 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/compute_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    89131 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/configs.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20716 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/data_frame.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31660 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10597 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/dataset.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7485 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/entity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34112 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/feature_service.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   165862 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/feature_view.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/filtered_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21844 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/transformation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      673 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/validation_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22879 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/framework/workspace.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.822849 tecton-0.7.0rc1/tecton/identities/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/identities/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/identities/api_keys.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3888 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/identities/credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10498 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/identities/okta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2138 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/pytest_tecton.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/run_api_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3009 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/snowflake_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2730 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/tecton_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3422 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/types.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.822849 tecton-0.7.0rc1/tecton/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.822849 tecton-0.7.0rc1/tecton/vendor/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.822849 tecton-0.7.0rc1/tecton/vendor/dill/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/__diff.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/_objects.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/detect.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/info.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/objtypes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/pointers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/settings.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/dill/dill/temp.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.822849 tecton-0.7.0rc1/tecton/vendor/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.822849 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/clientserver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/finalizer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/java_collections.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/protocol.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/signals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.826849 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/_globals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/accumulators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/broadcast.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.826849 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/daemon.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/files.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/find_spark_home.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/install.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/join.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.830850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/base.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/fpm.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/image.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.830850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.834850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/param/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/param/shared.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/regression.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/stat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/tuning.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/wrapper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.834850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/fpm.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.834850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/random.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/regression.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.838850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/profiler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.838850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/python/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/python/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.838850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/python/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/rdd.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/rddsampler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.838850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resource/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resource/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resource/information.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resource/profile.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resource/requests.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resultiterable.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/shuffle.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.838850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.838850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/catalog.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/column.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/dataframe.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/group.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.842850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/readwriter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/streaming.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/udf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/window.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/statcounter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/storagelevel.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.842850 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/dstream.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/listener.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/taskcontext.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/traceback_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/worker.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/vendor_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/vendor/vendor_pyspark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1185 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.814848 tecton-0.7.0rc1/tecton.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3890 2023-07-17 21:57:00.000000 tecton-0.7.0rc1/tecton.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19035 2023-07-17 21:57:00.000000 tecton-0.7.0rc1/tecton.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-07-17 21:57:00.000000 tecton-0.7.0rc1/tecton.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2023-07-17 21:57:00.000000 tecton-0.7.0rc1/tecton.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      833 2023-07-17 21:57:00.000000 tecton-0.7.0rc1/tecton.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       95 2023-07-17 21:57:00.000000 tecton-0.7.0rc1/tecton.egg-info/top_level.txt
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.842850 tecton-0.7.0rc1/tecton_athena/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14608 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/athena_session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8482 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/data_catalog_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5747 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/odfv_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6356 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.842850 tecton-0.7.0rc1/tecton_athena/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2291 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17764 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.842850 tecton-0.7.0rc1/tecton_athena/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates/create_table.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3863 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_athena/templates_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.846851 tecton-0.7.0rc1/tecton_core/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13329 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/aggregation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19520 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7206 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/data_types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5415 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4818 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/fco_container.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17300 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/feature_definition_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9765 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/feature_set_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/feature_view_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/filter_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2300 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/function_deserialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      623 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/id_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7393 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/materialization_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6916 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1395 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/online_serving_index.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6304 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/pipeline_common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4393 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/pipeline_sql_builder.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.846851 tecton-0.7.0rc1/tecton_core/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10765 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26314 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8446 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/node_interface.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    66482 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.846851 tecton-0.7.0rc1/tecton_core/query/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2677 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/pandas/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8340 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/pandas/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/pandas/sql.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      610 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9133 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query/sql_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      397 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/query_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4835 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/repo_file_handler.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/request_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1961 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/schema.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5562 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/schema_derivation_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.846851 tecton-0.7.0rc1/tecton_core/specs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      660 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/specs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    38770 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/specs/data_source_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1258 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/specs/entity_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5274 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/specs/feature_service_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30873 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/specs/feature_view_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/specs/tecton_object_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/specs/transformation_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4912 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/specs/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6872 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/time_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.846851 tecton-0.7.0rc1/tecton_core/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.846851 tecton-0.7.0rc1/tecton_core/vendor/treelib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/vendor/treelib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/vendor/treelib/exceptions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/vendor/treelib/misc.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/vendor/treelib/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/vendor/treelib/plugins.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/vendor/treelib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_core/vendor/vendor_treelib.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.846851 tecton-0.7.0rc1/tecton_proto/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.850851 tecton-0.7.0rc1/tecton_proto/amplitude/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/amplitude/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4278 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/amplitude/amplitude_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/amplitude/client_logging_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.850851 tecton-0.7.0rc1/tecton_proto/api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/api/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.850851 tecton-0.7.0rc1/tecton_proto/api/featureservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/api/featureservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    85094 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/api/featureservice/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9207 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/api/featureservice/feature_service_request_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.850851 tecton-0.7.0rc1/tecton_proto/args/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/basic_info_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/data_source_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17760 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3520 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/diff_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/diff_test_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2481 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/fco_args_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4122 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33904 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6463 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/pipeline_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/repo_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4071 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/user_defined_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/version_constraints_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7076 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/args/virtual_data_source_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.850851 tecton-0.7.0rc1/tecton_proto/auth/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/auth/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/auth/acl_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19265 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/auth/authorization_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2935 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/auth/principal_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1922 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/auth/resource_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3027 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/auth/resource_role_assignments_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3544 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/auth/service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.850851 tecton-0.7.0rc1/tecton_proto/canary/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/canary/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/canary/type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/canary/update_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.850851 tecton-0.7.0rc1/tecton_proto/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/cli/repo_diff_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.854851 tecton-0.7.0rc1/tecton_proto/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/aggregation_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/analytics_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/column_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1339 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/container_image_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/data_source_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/data_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/fco_locator_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/framework_version_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1196 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/id_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/pair_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/schema_container_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2070 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/secret_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/common/spark_schema_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.854851 tecton-0.7.0rc1/tecton_proto/consumption/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/consumption/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3289 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/consumption/consumption_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.858852 tecton-0.7.0rc1/tecton_proto/data/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6382 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/batch_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1589 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/data_source_access_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1921 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/fco_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2758 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/fco_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4497 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/feature_store_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15392 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/freshness_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2124 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/fv_materialization_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/hive_metastore_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1971 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/internal_spark_cluster_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5638 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/materialization_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/odfv_compute_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2316 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/onboarding_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1907 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/principal_group_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2696 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/remote_compute_environment_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12187 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/remote_spark_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/saved_feature_data_frame_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4541 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/serving_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9668 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/state_update_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3945 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/stream_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/summary_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2142 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/tecton_api_key_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2358 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9697 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/user_deployment_settings_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/user_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2979 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/virtual_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1743 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/data/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.858852 tecton-0.7.0rc1/tecton_proto/databricks_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8185 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/dbfs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/execution_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/instance_profiles_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/jobs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/libraries_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1937 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/permissions_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/scim_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/secrets_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/databricks_api/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/dataobs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/dataobs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/dataobs/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/dataobs/expectation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/dataobs/metric_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/dataobs/validation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3569 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/dataobs/validation_task_params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/dataobs/validation_task_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/feature_server/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/feature_server/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/feature_server/configuration/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/feature_server/configuration/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13426 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7654 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/materialization/job_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2598 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/materialization/materialization_states_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13314 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/materialization/materialization_task_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5790 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/materialization/params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2691 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/materialization/spark_cluster_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/materializationjobservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/materializationjobservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14321 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/metadataservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/metadataservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/metadataservice/http_over_grpc_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   107952 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/metadataservice/metadata_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/online_store/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/online_store/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4353 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/online_store/feature_value_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/online_store/status_entry_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/online_store_writer/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/online_store_writer/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/online_store_writer/config_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/remoteenvironmentservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/remoteenvironmentservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8041 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/snowflake/location_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/spark_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/spark_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/spark_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7263 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/spark_api/jobs_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/spark_common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/spark_common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7339 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/spark_common/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/spark_common/libraries_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.862852 tecton-0.7.0rc1/tecton_proto/validation/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/validation/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_proto/validation/validator_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.866852 tecton-0.7.0rc1/tecton_snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29228 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/pipeline_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7376 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/snowflake_type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32077 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.866852 tecton-0.7.0rc1/tecton_snowflake/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/copier_macro.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/create_temp_table_for_bfv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/delete_orphaned_schemas.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/delete_staged_files.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/historical_features_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/materialized_feature_view.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/offline_materialization_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/online_store_copier.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6695 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/templates_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_snowflake/utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.870853 tecton-0.7.0rc1/tecton_spark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      465 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25652 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2090 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/data_observability.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/data_source_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    35854 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/data_source_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/errors_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      890 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/feature_view_spark_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.870853 tecton-0.7.0rc1/tecton_spark/jars/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/jars/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)  1604241 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/jars/tecton-udfs-spark-3.jar
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4039 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/materialization_plan.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22766 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11048 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/partial_aggregations.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34132 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:57:01.870853 tecton-0.7.0rc1/tecton_spark/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3054 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/query/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8463 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/query/filter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18310 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/query/join.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1229 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/query/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4229 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/query/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5861 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/query/projection.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5087 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11252 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5410 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/schema_spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2135 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/spark_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1677 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/spark_schema_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4842 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/udf_jar.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2023-07-17 21:56:58.000000 tecton-0.7.0rc1/tecton_spark/udfs.py
```

### Comparing `tecton-0.7.0rc0/PKG-INFO` & `tecton-0.7.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.7.0rc0
+Version: 0.7.0rc1
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.7.0rc0/README.md` & `tecton-0.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/protoc_gen_swagger/options/annotations_pb2.py` & `tecton-0.7.0rc1/protoc_gen_swagger/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/protoc_gen_swagger/options/openapiv2_pb2.py` & `tecton-0.7.0rc1/protoc_gen_swagger/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/setup.py` & `tecton-0.7.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,14 @@
     author_email='support@tecton.ai',
     url='https://tecton.ai',
     license='Tecton Proprietary',
     include_package_data=True,
     description='Tecton Python SDK',
     entry_points={'console_scripts': ['tecton=tecton.cli.cli:main'], 'pytest11': ['pytest_tecton=tecton.pytest_tecton']},
     name='tecton',
-    version='0.7.0rc0',
+    version='0.7.0rc1',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos~=1.52', 'jinja2~=3.0', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf>=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas~=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version'],
     extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'snowflake': ['snowflake-connector-python[pandas]~=2.8'], 'snowpark': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=2.15']},
     packages=packages,
 )
```

### Comparing `tecton-0.7.0rc0/tecton/__init__.py` & `tecton-0.7.0rc1/tecton/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/analytics.py` & `tecton-0.7.0rc1/tecton/_internals/analytics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/athena_api.py` & `tecton-0.7.0rc1/tecton/_internals/athena_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/data_frame_helper.py` & `tecton-0.7.0rc1/tecton/_internals/data_frame_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/delete_keys_api.py` & `tecton-0.7.0rc1/tecton/_internals/delete_keys_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/display.py` & `tecton-0.7.0rc1/tecton/_internals/display.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/env_utils.py` & `tecton-0.7.0rc1/tecton/_internals/env_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/errors.py` & `tecton-0.7.0rc1/tecton/_internals/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/find_spark.py` & `tecton-0.7.0rc1/tecton/_internals/find_spark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/ingest_utils.py` & `tecton-0.7.0rc1/tecton/_internals/ingest_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/materialization_api.py` & `tecton-0.7.0rc1/tecton/_internals/materialization_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/metadata_service.py` & `tecton-0.7.0rc1/tecton/_internals/metadata_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/error_lib.py` & `tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/error_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/http_client.py` & `tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/http_client.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/request_lib.py` & `tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/request_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/response.py` & `tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/response.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/metadata_service_impl/service_calls.py` & `tecton-0.7.0rc1/tecton/_internals/metadata_service_impl/service_calls.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/mock_source_utils.py` & `tecton-0.7.0rc1/tecton/_internals/mock_source_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/query_helper.py` & `tecton-0.7.0rc1/tecton/_internals/query_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/repo/function_serialization.py` & `tecton-0.7.0rc1/tecton/_internals/repo/function_serialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/rewrite.py` & `tecton-0.7.0rc1/tecton/_internals/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/run_api.py` & `tecton-0.7.0rc1/tecton/_internals/run_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/sdk_decorators.py` & `tecton-0.7.0rc1/tecton/_internals/sdk_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,30 +88,29 @@
         return func(fco_object, *args, **kwargs)
 
     return wrapper
 
 
 @overload
 def assert_remote_object(
-    original_function: Callable[Concatenate[BaseTectonObject, _PT], _RT], /
+    original_function: Callable[Concatenate[BaseTectonObject, _PT], _RT]
 ) -> Callable[Concatenate[BaseTectonObject, _PT], _RT]:
     ...
 
 
 @overload
 def assert_remote_object(
     *, error_message: Callable[[str], Exception] = errors.INVALID_USAGE_FOR_LOCAL_TECTON_OBJECT
 ) -> Callable[[Callable[Concatenate[BaseTectonObject, _PT], _RT]], Callable[Concatenate[BaseTectonObject, _PT], _RT]]:
     ...
 
 
 @typeguard.typeguard_ignore
 def assert_remote_object(
     original_function: Optional[Callable[Concatenate[BaseTectonObject, _PT], _RT]] = None,
-    /,
     *,
     error_message: Callable[[str], Exception] = errors.INVALID_USAGE_FOR_LOCAL_TECTON_OBJECT,
 ) -> Union[
     Callable[Concatenate[BaseTectonObject, _PT], _RT],
     Callable[[Callable[Concatenate[BaseTectonObject, _PT], _RT]], Callable[Concatenate[BaseTectonObject, _PT], _RT]],
 ]:
     """Assert this function is being called on a remote Tecton object, aka an object applied and fetched from the backend, and raise error otherwise.
@@ -123,15 +122,14 @@
     @typeguard.typeguard_ignore
     def inner_decorator(
         target: Callable[Concatenate[BaseTectonObject, _PT], _RT]
     ) -> Callable[Concatenate[BaseTectonObject, _PT], _RT]:
         @wraps(target)
         def wrapper(
             fco_object: BaseTectonObject,
-            /,
             *args: _PT.args,
             **kwargs: _PT.kwargs,
         ) -> _RT:
             if fco_object.info._is_local_object:
                 raise error_message(target.__name__)
             return target(fco_object, *args, **kwargs)
 
@@ -141,15 +139,15 @@
         return inner_decorator(original_function)
 
     return inner_decorator
 
 
 @overload
 def assert_local_object(
-    original_function: Callable[Concatenate[BaseTectonObject, _PT], _RT], /
+    original_function: Callable[Concatenate[BaseTectonObject, _PT], _RT]
 ) -> Callable[Concatenate[BaseTectonObject, _PT], _RT]:
     ...
 
 
 @overload
 def assert_local_object(
     *,
@@ -157,15 +155,14 @@
 ) -> Callable[[Callable[Concatenate[BaseTectonObject, _PT], _RT]], Callable[Concatenate[BaseTectonObject, _PT], _RT]]:
     ...
 
 
 @typeguard.typeguard_ignore
 def assert_local_object(
     original_function: Optional[Callable[Concatenate[BaseTectonObject, _PT], _RT]] = None,
-    /,
     *,
     error_message: Callable[[str], Exception] = errors.INVALID_USAGE_FOR_REMOTE_TECTON_OBJECT,
 ) -> Union[
     Callable[Concatenate[BaseTectonObject, _PT], _RT],
     Callable[[Callable[Concatenate[BaseTectonObject, _PT], _RT]], Callable[Concatenate[BaseTectonObject, _PT], _RT]],
 ]:
     """Assert this function is being called on a local Tecton object, aka an object created locally (as opposed to being fetched from the backend).
@@ -177,15 +174,14 @@
     @typeguard.typeguard_ignore
     def inner_decorator(
         target: Callable[Concatenate[BaseTectonObject, _PT], _RT]
     ) -> Callable[Concatenate[BaseTectonObject, _PT], _RT]:
         @wraps(target)
         def wrapper(
             fco_object: BaseTectonObject,
-            /,
             *args: _PT.args,
             **kwargs: _PT.kwargs,
         ) -> _RT:
             if not fco_object.info._is_local_object:
                 raise error_message(target.__name__)
             return target(fco_object, *args, **kwargs)
 
@@ -194,15 +190,15 @@
     if original_function:
         return inner_decorator(original_function)
 
     return inner_decorator
 
 
 @overload
-def sdk_public_method(original_function: Callable[_PT, _RT], /) -> Callable[_PT, _RT]:
+def sdk_public_method(original_function: Callable[_PT, _RT]) -> Callable[_PT, _RT]:
     ...
 
 
 @overload
 def sdk_public_method(
     *,
     requires_validation: bool = False,
@@ -211,15 +207,14 @@
 ) -> Callable[[Callable[_PT, _RT]], Callable[_PT, _RT]]:
     ...
 
 
 @typeguard.typeguard_ignore
 def sdk_public_method(
     original_function: Optional[Callable[_PT, _RT]] = None,
-    /,
     *,
     requires_validation: bool = False,
     validation_error_message: Callable[[str, str, str], Exception] = errors.TECTON_OBJECT_REQUIRES_VALIDATION,
     supports_skip_validation: Tuple[compute_mode.ComputeMode, ...] = tuple(),
 ) -> Union[Callable[_PT, _RT], Callable[[Callable[_PT, _RT]], Callable[_PT, _RT]]]:
     """Decorator for public SDK methods that should have analytics logging.
```

### Comparing `tecton-0.7.0rc0/tecton/_internals/snowflake_api.py` & `tecton-0.7.0rc1/tecton/_internals/snowflake_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/spark_api.py` & `tecton-0.7.0rc1/tecton/_internals/spark_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/spark_utils.py` & `tecton-0.7.0rc1/tecton/_internals/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/time_utils.py` & `tecton-0.7.0rc1/tecton/_internals/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/type_utils.py` & `tecton-0.7.0rc1/tecton/_internals/type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/utils.py` & `tecton-0.7.0rc1/tecton/_internals/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/_internals/validations_api.py` & `tecton-0.7.0rc1/tecton/_internals/validations_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/aggregation_functions.py` & `tecton-0.7.0rc1/tecton/aggregation_functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/access_control.py` & `tecton-0.7.0rc1/tecton/cli/access_control.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/api_key.py` & `tecton-0.7.0rc1/tecton/cli/api_key.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/cli.py` & `tecton-0.7.0rc1/tecton/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/cli_utils.py` & `tecton-0.7.0rc1/tecton/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/command.py` & `tecton-0.7.0rc1/tecton/cli/command.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/common.py` & `tecton-0.7.0rc1/tecton/cli/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/engine.py` & `tecton-0.7.0rc1/tecton/cli/engine.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/engine_renderer.py` & `tecton-0.7.0rc1/tecton/cli/engine_renderer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/environment.py` & `tecton-0.7.0rc1/tecton/cli/environment.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/error_utils.py` & `tecton-0.7.0rc1/tecton/cli/error_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/printer.py` & `tecton-0.7.0rc1/tecton/cli/printer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/service_account.py` & `tecton-0.7.0rc1/tecton/cli/service_account.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/user.py` & `tecton-0.7.0rc1/tecton/cli/user.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/workspace.py` & `tecton-0.7.0rc1/tecton/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/cli/workspace_utils.py` & `tecton-0.7.0rc1/tecton/cli/workspace_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/fco_listers.py` & `tecton-0.7.0rc1/tecton/fco_listers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/base_tecton_object.py` & `tecton-0.7.0rc1/tecton/framework/base_tecton_object.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/compute_mode.py` & `tecton-0.7.0rc1/tecton/framework/compute_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/configs.py` & `tecton-0.7.0rc1/tecton/framework/configs.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/data_frame.py` & `tecton-0.7.0rc1/tecton/framework/data_frame.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/data_source.py` & `tecton-0.7.0rc1/tecton/framework/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/dataset.py` & `tecton-0.7.0rc1/tecton/framework/dataset.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/entity.py` & `tecton-0.7.0rc1/tecton/framework/entity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/feature_service.py` & `tecton-0.7.0rc1/tecton/framework/feature_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/feature_view.py` & `tecton-0.7.0rc1/tecton/framework/feature_view.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/filtered_source.py` & `tecton-0.7.0rc1/tecton/framework/filtered_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/transformation.py` & `tecton-0.7.0rc1/tecton/framework/transformation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/utils.py` & `tecton-0.7.0rc1/tecton/framework/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/validation_mode.py` & `tecton-0.7.0rc1/tecton/framework/validation_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/framework/workspace.py` & `tecton-0.7.0rc1/tecton/framework/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/identities/api_keys.py` & `tecton-0.7.0rc1/tecton/identities/api_keys.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/identities/credentials.py` & `tecton-0.7.0rc1/tecton/identities/credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/identities/okta.py` & `tecton-0.7.0rc1/tecton/identities/okta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/pytest_tecton.py` & `tecton-0.7.0rc1/tecton/pytest_tecton.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/snowflake_context.py` & `tecton-0.7.0rc1/tecton/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/tecton_context.py` & `tecton-0.7.0rc1/tecton/tecton_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/types.py` & `tecton-0.7.0rc1/tecton/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/__diff.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/__diff.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/_dill.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/_objects.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/_objects.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/detect.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/detect.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/info.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/info.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/objtypes.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/objtypes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/pointers.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/pointers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/settings.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/settings.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/source.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/dill/dill/temp.py` & `tecton-0.7.0rc1/tecton/vendor/dill/dill/temp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/clientserver.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/clientserver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/compat.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/finalizer.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/finalizer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/java_collections.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/java_collections.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/java_gateway.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/protocol.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/protocol.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/py4j/signals.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/py4j/signals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/_globals.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/_globals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/accumulators.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/accumulators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/broadcast.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/broadcast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/conf.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/context.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/daemon.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/daemon.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/files.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/files.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/find_spark_home.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/find_spark_home.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/install.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/install.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/java_gateway.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/join.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/base.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/base.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/classification.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/clustering.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/common.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/evaluation.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/feature.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/fpm.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/functions.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/image.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/image.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/param/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/param/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/param/shared.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/param/shared.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/pipeline.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/recommendation.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/regression.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/stat.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/stat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/tree.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/tuning.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/tuning.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/util.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/ml/wrapper.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/ml/wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/classification.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/clustering.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/common.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/evaluation.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/feature.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/fpm.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/random.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/random.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/recommendation.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/regression.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/stat/test.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/stat/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/tree.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/mllib/util.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/mllib/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/profiler.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/profiler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/rdd.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/rdd.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/rddsampler.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/rddsampler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resource/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resource/information.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resource/information.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resource/profile.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resource/profile.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resource/requests.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resource/requests.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/resultiterable.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/resultiterable.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/serializers.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/shell.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/shuffle.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/shuffle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/avro/functions.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/avro/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/catalog.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/column.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/column.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/conf.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/context.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/dataframe.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/functions.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/group.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/group.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/types.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/readwriter.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/readwriter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/session.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/streaming.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/streaming.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/types.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/udf.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/udf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/utils.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/sql/window.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/sql/window.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/statcounter.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/statcounter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/status.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/storagelevel.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/storagelevel.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/__init__.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/context.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/dstream.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/dstream.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/kinesis.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/kinesis.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/listener.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/listener.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/streaming/util.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/streaming/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/taskcontext.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/taskcontext.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/traceback_utils.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/util.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/pyspark/pyspark/worker.py` & `tecton-0.7.0rc1/tecton/vendor/pyspark/pyspark/worker.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/vendor_dill.py` & `tecton-0.7.0rc1/tecton/vendor/vendor_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/vendor/vendor_pyspark.py` & `tecton-0.7.0rc1/tecton/vendor/vendor_pyspark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton/version.py` & `tecton-0.7.0rc1/tecton/version.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton.egg-info/PKG-INFO` & `tecton-0.7.0rc1/tecton.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.7.0rc0
+Version: 0.7.0rc1
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.7.0rc0/tecton.egg-info/SOURCES.txt` & `tecton-0.7.0rc1/tecton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton.egg-info/requires.txt` & `tecton-0.7.0rc1/tecton.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/athena_session.py` & `tecton-0.7.0rc1/tecton_athena/athena_session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/data_catalog_helper.py` & `tecton-0.7.0rc1/tecton_athena/data_catalog_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/odfv_helper.py` & `tecton-0.7.0rc1/tecton_athena/odfv_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/pipeline_helper.py` & `tecton-0.7.0rc1/tecton_athena/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/query/translate.py` & `tecton-0.7.0rc1/tecton_athena/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/sql_helper.py` & `tecton-0.7.0rc1/tecton_athena/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/templates/create_table.sql` & `tecton-0.7.0rc1/tecton_athena/templates/create_table.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/templates/historical_features.sql` & `tecton-0.7.0rc1/tecton_athena/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/templates/materialization_tile.sql` & `tecton-0.7.0rc1/tecton_athena/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/templates/run_full_aggregation.sql` & `tecton-0.7.0rc1/tecton_athena/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/templates/time_limit.sql` & `tecton-0.7.0rc1/tecton_athena/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_athena/templates_utils.py` & `tecton-0.7.0rc1/tecton_athena/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/aggregation_utils.py` & `tecton-0.7.0rc1/tecton_core/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/conf.py` & `tecton-0.7.0rc1/tecton_core/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/data_types.py` & `tecton-0.7.0rc1/tecton_core/data_types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/errors.py` & `tecton-0.7.0rc1/tecton_core/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/fco_container.py` & `tecton-0.7.0rc1/tecton_core/fco_container.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/feature_definition_wrapper.py` & `tecton-0.7.0rc1/tecton_core/feature_definition_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/feature_set_config.py` & `tecton-0.7.0rc1/tecton_core/feature_set_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/feature_view_utils.py` & `tecton-0.7.0rc1/tecton_core/feature_view_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/function_deserialization.py` & `tecton-0.7.0rc1/tecton_core/function_deserialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/id_helper.py` & `tecton-0.7.0rc1/tecton_core/id_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/materialization_context.py` & `tecton-0.7.0rc1/tecton_core/materialization_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/offline_store.py` & `tecton-0.7.0rc1/tecton_core/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/online_serving_index.py` & `tecton-0.7.0rc1/tecton_core/online_serving_index.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/pipeline_common.py` & `tecton-0.7.0rc1/tecton_core/pipeline_common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/pipeline_sql_builder.py` & `tecton-0.7.0rc1/tecton_core/pipeline_sql_builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/query/aggregation_plans.py` & `tecton-0.7.0rc1/tecton_core/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/query/builder.py` & `tecton-0.7.0rc1/tecton_core/query/builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/query/node_interface.py` & `tecton-0.7.0rc1/tecton_core/query/node_interface.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/query/nodes.py` & `tecton-0.7.0rc1/tecton_core/query/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/query/pandas/node.py` & `tecton-0.7.0rc1/tecton_core/query/pandas/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/query/pandas/nodes.py` & `tecton-0.7.0rc1/tecton_core/query/pandas/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/query/rewrite.py` & `tecton-0.7.0rc1/tecton_core/query/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/query/sql_compat.py` & `tecton-0.7.0rc1/tecton_core/query/sql_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/repo_file_handler.py` & `tecton-0.7.0rc1/tecton_core/repo_file_handler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/request_context.py` & `tecton-0.7.0rc1/tecton_core/request_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/schema.py` & `tecton-0.7.0rc1/tecton_core/schema.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/schema_derivation_utils.py` & `tecton-0.7.0rc1/tecton_core/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/specs/__init__.py` & `tecton-0.7.0rc1/tecton_core/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/specs/data_source_spec.py` & `tecton-0.7.0rc1/tecton_core/specs/data_source_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/specs/entity_spec.py` & `tecton-0.7.0rc1/tecton_core/specs/entity_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/specs/feature_service_spec.py` & `tecton-0.7.0rc1/tecton_core/specs/feature_service_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/specs/feature_view_spec.py` & `tecton-0.7.0rc1/tecton_core/specs/feature_view_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/specs/tecton_object_spec.py` & `tecton-0.7.0rc1/tecton_core/specs/tecton_object_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/specs/transformation_spec.py` & `tecton-0.7.0rc1/tecton_core/specs/transformation_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/specs/utils.py` & `tecton-0.7.0rc1/tecton_core/specs/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/time_utils.py` & `tecton-0.7.0rc1/tecton_core/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/vendor/treelib/__init__.py` & `tecton-0.7.0rc1/tecton_core/vendor/treelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/vendor/treelib/exceptions.py` & `tecton-0.7.0rc1/tecton_core/vendor/treelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/vendor/treelib/misc.py` & `tecton-0.7.0rc1/tecton_core/vendor/treelib/misc.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/vendor/treelib/node.py` & `tecton-0.7.0rc1/tecton_core/vendor/treelib/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/vendor/treelib/plugins.py` & `tecton-0.7.0rc1/tecton_core/vendor/treelib/plugins.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/vendor/treelib/tree.py` & `tecton-0.7.0rc1/tecton_core/vendor/treelib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_core/vendor/vendor_treelib.py` & `tecton-0.7.0rc1/tecton_core/vendor/vendor_treelib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/amplitude/amplitude_pb2.py` & `tecton-0.7.0rc1/tecton_proto/amplitude/amplitude_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/amplitude/client_logging_pb2.py` & `tecton-0.7.0rc1/tecton_proto/amplitude/client_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/api/featureservice/feature_service_pb2.py` & `tecton-0.7.0rc1/tecton_proto/api/featureservice/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/api/featureservice/feature_service_request_pb2.py` & `tecton-0.7.0rc1/tecton_proto/api/featureservice/feature_service_request_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/basic_info_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/basic_info_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/data_source_config_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/data_source_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/data_source_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/diff_options_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/diff_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/diff_test_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/diff_test_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/entity_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/fco_args_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/fco_args_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/feature_service_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/feature_view_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/pipeline_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/repo_metadata_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/repo_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/transformation_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/user_defined_function_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/user_defined_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/version_constraints_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/version_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/args/virtual_data_source_pb2.py` & `tecton-0.7.0rc1/tecton_proto/args/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/auth/acl_pb2.py` & `tecton-0.7.0rc1/tecton_proto/auth/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/auth/authorization_service_pb2.py` & `tecton-0.7.0rc1/tecton_proto/auth/authorization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/auth/principal_pb2.py` & `tecton-0.7.0rc1/tecton_proto/auth/principal_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/auth/resource_pb2.py` & `tecton-0.7.0rc1/tecton_proto/auth/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/auth/resource_role_assignments_pb2.py` & `tecton-0.7.0rc1/tecton_proto/auth/resource_role_assignments_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/auth/service_pb2.py` & `tecton-0.7.0rc1/tecton_proto/auth/service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/canary/type_pb2.py` & `tecton-0.7.0rc1/tecton_proto/canary/type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/canary/update_pb2.py` & `tecton-0.7.0rc1/tecton_proto/canary/update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/cli/repo_diff_pb2.py` & `tecton-0.7.0rc1/tecton_proto/cli/repo_diff_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/aggregation_function_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/aggregation_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/analytics_options_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/analytics_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/column_type_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/column_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/container_image_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/container_image_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/data_source_type_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/data_source_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/data_type_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/fco_locator_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/fco_locator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/framework_version_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/framework_version_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/id_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/id_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/pair_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/schema_container_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/schema_container_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/schema_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/secret_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/common/spark_schema_pb2.py` & `tecton-0.7.0rc1/tecton_proto/common/spark_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/consumption/consumption_pb2.py` & `tecton-0.7.0rc1/tecton_proto/consumption/consumption_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/batch_data_source_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/batch_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/data_source_access_config_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/data_source_access_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/entity_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/fco_metadata_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/fco_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/fco_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/fco_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/feature_service_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/feature_store_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/feature_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/feature_view_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/freshness_status_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/freshness_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/fv_materialization_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/fv_materialization_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/hive_metastore_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/hive_metastore_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/internal_spark_cluster_status_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/internal_spark_cluster_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/materialization_status_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/materialization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/odfv_compute_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/odfv_compute_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/onboarding_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/onboarding_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/principal_group_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/principal_group_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/remote_compute_environment_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/remote_compute_environment_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/remote_spark_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/remote_spark_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/saved_feature_data_frame_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/saved_feature_data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/serving_status_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/serving_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/state_update_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/stream_data_source_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/stream_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/summary_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/tecton_api_key_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/tecton_api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/transformation_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/user_deployment_settings_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/user_deployment_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/user_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/user_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/virtual_data_source_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/data/workspace_pb2.py` & `tecton-0.7.0rc1/tecton_proto/data/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/clusters_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/dbfs_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/dbfs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/error_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/execution_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/instance_profiles_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/instance_profiles_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/jobs_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/libraries_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/permissions_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/permissions_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/scim_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/scim_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/secrets_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/databricks_api/workspace_pb2.py` & `tecton-0.7.0rc1/tecton_proto/databricks_api/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/dataobs/config_pb2.py` & `tecton-0.7.0rc1/tecton_proto/dataobs/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/dataobs/expectation_pb2.py` & `tecton-0.7.0rc1/tecton_proto/dataobs/expectation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/dataobs/metric_pb2.py` & `tecton-0.7.0rc1/tecton_proto/dataobs/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/dataobs/validation_pb2.py` & `tecton-0.7.0rc1/tecton_proto/dataobs/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/dataobs/validation_task_params_pb2.py` & `tecton-0.7.0rc1/tecton_proto/dataobs/validation_task_params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/dataobs/validation_task_pb2.py` & `tecton-0.7.0rc1/tecton_proto/dataobs/validation_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py` & `tecton-0.7.0rc1/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/materialization/job_metadata_pb2.py` & `tecton-0.7.0rc1/tecton_proto/materialization/job_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/materialization/materialization_states_pb2.py` & `tecton-0.7.0rc1/tecton_proto/materialization/materialization_states_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/materialization/materialization_task_pb2.py` & `tecton-0.7.0rc1/tecton_proto/materialization/materialization_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/materialization/params_pb2.py` & `tecton-0.7.0rc1/tecton_proto/materialization/params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/materialization/spark_cluster_pb2.py` & `tecton-0.7.0rc1/tecton_proto/materialization/spark_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/materializationjobservice/materialization_job_service_pb2.py` & `tecton-0.7.0rc1/tecton_proto/materializationjobservice/materialization_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/metadataservice/http_over_grpc_pb2.py` & `tecton-0.7.0rc1/tecton_proto/metadataservice/http_over_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/metadataservice/metadata_service_pb2.py` & `tecton-0.7.0rc1/tecton_proto/metadataservice/metadata_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/online_store/feature_value_pb2.py` & `tecton-0.7.0rc1/tecton_proto/online_store/feature_value_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/online_store/status_entry_pb2.py` & `tecton-0.7.0rc1/tecton_proto/online_store/status_entry_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/online_store_writer/config_pb2.py` & `tecton-0.7.0rc1/tecton_proto/online_store_writer/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py` & `tecton-0.7.0rc1/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/snowflake/location_pb2.py` & `tecton-0.7.0rc1/tecton_proto/snowflake/location_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/spark_api/error_pb2.py` & `tecton-0.7.0rc1/tecton_proto/spark_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/spark_api/jobs_pb2.py` & `tecton-0.7.0rc1/tecton_proto/spark_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/spark_common/clusters_pb2.py` & `tecton-0.7.0rc1/tecton_proto/spark_common/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/spark_common/libraries_pb2.py` & `tecton-0.7.0rc1/tecton_proto/spark_common/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_proto/validation/validator_pb2.py` & `tecton-0.7.0rc1/tecton_proto/validation/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/pipeline_helper.py` & `tecton-0.7.0rc1/tecton_snowflake/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/schema_derivation_utils.py` & `tecton-0.7.0rc1/tecton_snowflake/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/snowflake_type_utils.py` & `tecton-0.7.0rc1/tecton_snowflake/snowflake_type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/sql_helper.py` & `tecton-0.7.0rc1/tecton_snowflake/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/copier_macro.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/copier_macro.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/delete_orphaned_schemas.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/delete_orphaned_schemas.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/delete_staged_files.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/delete_staged_files.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/historical_features.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/historical_features_macros.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/historical_features_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/materialization_tile.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/materialized_feature_view.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/materialized_feature_view.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/offline_materialization_macros.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/offline_materialization_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/run_full_aggregation.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/run_partial_aggregation.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/run_partial_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates/time_limit.sql` & `tecton-0.7.0rc1/tecton_snowflake/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_snowflake/templates_utils.py` & `tecton-0.7.0rc1/tecton_snowflake/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/aggregation_plans.py` & `tecton-0.7.0rc1/tecton_spark/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/data_observability.py` & `tecton-0.7.0rc1/tecton_spark/data_observability.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/data_source_credentials.py` & `tecton-0.7.0rc1/tecton_spark/data_source_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/data_source_helper.py` & `tecton-0.7.0rc1/tecton_spark/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/feature_view_spark_utils.py` & `tecton-0.7.0rc1/tecton_spark/feature_view_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/jars/tecton-udfs-spark-3.jar` & `tecton-0.7.0rc1/tecton_spark/jars/tecton-udfs-spark-3.jar`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/materialization_plan.py` & `tecton-0.7.0rc1/tecton_spark/materialization_plan.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/offline_store.py` & `tecton-0.7.0rc1/tecton_spark/offline_store.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/partial_aggregations.py` & `tecton-0.7.0rc1/tecton_spark/partial_aggregations.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/pipeline_helper.py` & `tecton-0.7.0rc1/tecton_spark/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/query/data_source.py` & `tecton-0.7.0rc1/tecton_spark/query/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/query/filter.py` & `tecton-0.7.0rc1/tecton_spark/query/filter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/query/join.py` & `tecton-0.7.0rc1/tecton_spark/query/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/query/node.py` & `tecton-0.7.0rc1/tecton_spark/query/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/query/pipeline.py` & `tecton-0.7.0rc1/tecton_spark/query/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/query/projection.py` & `tecton-0.7.0rc1/tecton_spark/query/projection.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/query/translate.py` & `tecton-0.7.0rc1/tecton_spark/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/schema_derivation_utils.py` & `tecton-0.7.0rc1/tecton_spark/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/schema_spark_utils.py` & `tecton-0.7.0rc1/tecton_spark/schema_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/spark_helper.py` & `tecton-0.7.0rc1/tecton_spark/spark_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/spark_schema_wrapper.py` & `tecton-0.7.0rc1/tecton_spark/spark_schema_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/time_utils.py` & `tecton-0.7.0rc1/tecton_spark/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.7.0rc0/tecton_spark/udfs.py` & `tecton-0.7.0rc1/tecton_spark/udfs.py`

 * *Files identical despite different names*

