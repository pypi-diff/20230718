# Comparing `tmp/kaskada-0.5.0.tar.gz` & `tmp/kaskada-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.5.0.tar", max compression
+gzip compressed data, was "kaskada-0.5.1.tar", max compression
```

## Comparing `kaskada-0.5.0.tar` & `kaskada-0.5.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1646 2023-07-17 18:54:47.236325 kaskada-0.5.0/README.md
--rw-r--r--   0        0        0     3917 2023-07-17 18:54:47.236325 kaskada-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7632 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/fenlmagic/utils.py
--rw-r--r--   0        0        0       33 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/__init__.py
--rw-r--r--   0        0        0      569 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0        0 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/local_session/__init__.py
--rw-r--r--   0        0        0     3573 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/local_session/local_service.py
--rw-r--r--   0        0        0     3312 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/local_session/local_session_keep_alive.py
--rw-r--r--   0        0        0     6381 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/release.py
--rw-r--r--   0        0        0     1108 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/remote_session/__init__.py
--rw-r--r--   0        0        0    12106 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/api/session.py
--rw-r--r--   0        0        0    11972 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7337 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0    10325 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0        0 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/health/__init__.py
--rw-r--r--   0        0        0     1886 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/health/health_check_client.py
--rw-r--r--   0        0        0     4522 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/health/health_check_servicer.py
--rw-r--r--   0        0        0     2326 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/health/health_check_watcher.py
--rw-r--r--   0        0        0     7352 2023-07-17 18:54:48.012318 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/common_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.012318 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0    13155 2023-07-17 18:54:48.044319 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
--rw-r--r--   0        0        0    12538 2023-07-17 18:54:48.044319 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
--rw-r--r--   0        0        0     4489 2023-07-17 18:54:48.072320 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
--rw-r--r--   0        0        0     2938 2023-07-17 18:54:48.068320 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
--rw-r--r--   0        0        0     4191 2023-07-17 18:54:48.092320 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.120321 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
--rw-r--r--   0        0        0     2718 2023-07-17 18:54:48.124321 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.148322 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
--rw-r--r--   0        0        0     4491 2023-07-17 18:54:48.152322 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py
--rw-r--r--   0        0        0     5054 2023-07-17 18:54:48.180323 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
--rw-r--r--   0        0        0     2222 2023-07-17 18:54:48.184323 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/kafka_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.204323 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/kafka_pb2_grpc.py
--rw-r--r--   0        0        0    10837 2023-07-17 18:54:48.228324 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
--rw-r--r--   0        0        0     9283 2023-07-17 18:54:48.232324 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     1897 2023-07-17 18:54:48.256325 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/options_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.468330 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
--rw-r--r--   0        0        0    13180 2023-07-17 18:54:48.284325 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/plan_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.320326 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
--rw-r--r--   0        0        0     3398 2023-07-17 18:54:48.352327 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
--rw-r--r--   0        0        0     4894 2023-07-17 18:54:48.392328 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
--rw-r--r--   0        0        0     2805 2023-07-17 18:54:48.420329 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.456330 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
--rw-r--r--   0        0        0    11773 2023-07-17 18:54:48.484331 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py
--rw-r--r--   0        0        0     6542 2023-07-17 18:54:48.496331 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     4384 2023-07-17 18:54:48.512332 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/schema_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.528332 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
--rw-r--r--   0        0        0     2827 2023-07-17 18:54:48.540332 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/sources_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.552333 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
--rw-r--r--   0        0        0     2729 2023-07-17 18:54:48.568333 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/spec_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.588334 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
--rw-r--r--   0        0        0    11323 2023-07-17 18:54:48.592334 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py
--rw-r--r--   0        0        0    10053 2023-07-17 18:54:48.612334 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
--rw-r--r--   0        0        0     5157 2023-07-17 18:54:48.624335 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
--rw-r--r--   0        0        0      159 2023-07-17 18:54:48.632335 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
--rw-r--r--   0        0        0     8140 2023-07-17 18:54:48.648336 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py
--rw-r--r--   0        0        0     8153 2023-07-17 18:54:48.668336 kaskada-0.5.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
--rw-r--r--   0        0        0    16491 2023-07-17 18:54:48.680336 kaskada-0.5.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py
--rw-r--r--   0        0        0     8377 2023-07-17 18:54:48.708337 kaskada-0.5.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     8622 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9272 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0    10286 2023-07-17 18:54:47.236325 kaskada-0.5.0/src/kaskada/table.py
--rw-r--r--   0        0        0     7131 2023-07-17 18:54:47.240324 kaskada-0.5.0/src/kaskada/utils.py
--rw-r--r--   0        0        0     4543 2023-07-17 18:54:47.240324 kaskada-0.5.0/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-07-17 18:54:47.240324 kaskada-0.5.0/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-07-17 18:54:47.240324 kaskada-0.5.0/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-07-17 18:54:47.240324 kaskada-0.5.0/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-17 18:54:47.240324 kaskada-0.5.0/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 kaskada-0.5.0/setup.py
--rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 kaskada-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-07-18 17:51:44.071968 kaskada-0.5.1/README.md
+-rw-r--r--   0        0        0     3917 2023-07-18 17:51:44.075968 kaskada-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7253 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0       33 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/api/__init__.py
+-rw-r--r--   0        0        0      569 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0        0 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/api/local_session/__init__.py
+-rw-r--r--   0        0        0     3573 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/api/local_session/local_service.py
+-rw-r--r--   0        0        0     3312 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/api/local_session/local_session_keep_alive.py
+-rw-r--r--   0        0        0     6381 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/api/release.py
+-rw-r--r--   0        0        0     1108 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/api/remote_session/__init__.py
+-rw-r--r--   0        0        0    12106 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/api/session.py
+-rw-r--r--   0        0        0    12059 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7337 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0    10325 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0        0 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/health/__init__.py
+-rw-r--r--   0        0        0     1886 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/health/health_check_client.py
+-rw-r--r--   0        0        0     4522 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/health/health_check_servicer.py
+-rw-r--r--   0        0        0     2326 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/health/health_check_watcher.py
+-rw-r--r--   0        0        0     7352 2023-07-18 17:51:44.767974 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:44.763974 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0    13155 2023-07-18 17:51:44.827975 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
+-rw-r--r--   0        0        0    12538 2023-07-18 17:51:44.831975 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4489 2023-07-18 17:51:44.927976 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
+-rw-r--r--   0        0        0     2938 2023-07-18 17:51:45.007977 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4191 2023-07-18 17:51:44.975976 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/destinations_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:45.027977 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
+-rw-r--r--   0        0        0     2718 2023-07-18 17:51:45.063977 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:45.083977 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
+-rw-r--r--   0        0        0     4491 2023-07-18 17:51:45.147978 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/file_service_pb2.py
+-rw-r--r--   0        0        0     5054 2023-07-18 17:51:45.171978 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2222 2023-07-18 17:51:45.235979 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/kafka_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:45.279979 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/kafka_pb2_grpc.py
+-rw-r--r--   0        0        0    10837 2023-07-18 17:51:45.295979 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
+-rw-r--r--   0        0        0     9283 2023-07-18 17:51:45.343980 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-07-18 17:51:45.371980 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/options_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:45.407981 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
+-rw-r--r--   0        0        0    13235 2023-07-18 17:51:45.531982 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/plan_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:45.467981 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
+-rw-r--r--   0        0        0     3398 2023-07-18 17:51:45.511982 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
+-rw-r--r--   0        0        0     4894 2023-07-18 17:51:45.579982 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2805 2023-07-18 17:51:45.595982 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:45.651983 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
+-rw-r--r--   0        0        0    11773 2023-07-18 17:51:45.651983 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     6542 2023-07-18 17:51:45.727984 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4823 2023-07-18 17:51:45.795984 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/schema_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:45.807984 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     2827 2023-07-18 17:51:45.871985 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/sources_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:45.863985 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
+-rw-r--r--   0        0        0     2729 2023-07-18 17:51:45.967986 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/spec_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:45.967986 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
+-rw-r--r--   0        0        0    11323 2023-07-18 17:51:46.031986 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/table_service_pb2.py
+-rw-r--r--   0        0        0    10053 2023-07-18 17:51:46.031986 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5157 2023-07-18 17:51:46.087987 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:46.087987 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
+-rw-r--r--   0        0        0     8140 2023-07-18 17:51:46.139988 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/view_service_pb2.py
+-rw-r--r--   0        0        0     8153 2023-07-18 17:51:46.143988 kaskada-0.5.1/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16491 2023-07-18 17:51:46.199988 kaskada-0.5.1/src/kaskada/kaskada/v2alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     8377 2023-07-18 17:51:46.243988 kaskada-0.5.1/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8622 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9805 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10286 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/table.py
+-rw-r--r--   0        0        0     7131 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4543 2023-07-18 17:51:44.075968 kaskada-0.5.1/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-07-18 17:51:44.075968 kaskada-0.5.1/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-07-18 17:51:44.075968 kaskada-0.5.1/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-07-18 17:51:44.075968 kaskada-0.5.1/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-18 17:51:44.075968 kaskada-0.5.1/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 kaskada-0.5.1/setup.py
+-rw-r--r--   0        0        0     2742 1970-01-01 00:00:00.000000 kaskada-0.5.1/PKG-INFO
```

### Comparing `kaskada-0.5.0/README.md` & `kaskada-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/pyproject.toml` & `kaskada-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.5.0"
+version = "0.5.1"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
```

### Comparing `kaskada-0.5.0/src/fenlmagic/__init__.py` & `kaskada-0.5.1/src/fenlmagic/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 # pylint: disable=no-member
 from __future__ import print_function
 
 import logging
 import os
 import sys
+from typing import Optional
 
 import IPython
 import pandas
 from google.protobuf import wrappers_pb2 as wrappers
 from IPython.core.error import UsageError
 from IPython.core.magic import Magics, cell_magic, line_cell_magic, magics_class
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
@@ -36,20 +37,18 @@
 
     def set_dataframe(self, dataframe: pandas.DataFrame):
         self.dataframe = dataframe
 
 
 @magics_class
 class FenlMagics(Magics):
-    client = None
-
-    def __init__(self, shell, client):
+    def __init__(self, shell, client: Optional[client.Client]):
         super(FenlMagics, self).__init__(shell)
-        self.client = client
         logger.info("extension loaded")
+        self.client = client
 
     @magic_arguments()
     @argument(
         "--changed-since-time",
         help="Time bound (inclusive) after which results will be produced.",
     )
     @argument(
@@ -170,27 +169,16 @@
                 IPython.get_ipython().push({var: query_result})
 
             return query_result
         except Exception as e:
             raise UsageError(e)
 
 
-def load_ipython_extension(ipython):
-    if client.KASKADA_DEFAULT_CLIENT is None:
-        logger.warn(
-            "No client was initialized. Initializing default client to connect to localhost:50051."
-        )
-        default_client = client.Client(
-            client_id=os.getenv("KASKADA_CLIENT_ID", None),
-            endpoint=client.KASKADA_DEFAULT_ENDPOINT,
-            is_secure=client.KASKADA_IS_SECURE,
-        )
-        client.set_default_client(default_client)
-
-    magics = FenlMagics(ipython, client.get_client())
+def load_ipython_extension(ipython, client: Optional[client.Client] = None):
+    magics = FenlMagics(ipython, client)
     ipython.register_magics(magics)
 
 
 def clean_arg(arg: str) -> str:
     """
     Strips quotes and double-quotes from passed arguments
```

### Comparing `kaskada-0.5.0/src/kaskada/api/api_utils.py` & `kaskada-0.5.1/src/kaskada/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/api/local_session/local_service.py` & `kaskada-0.5.1/src/kaskada/api/local_session/local_service.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/api/local_session/local_session_keep_alive.py` & `kaskada-0.5.1/src/kaskada/api/local_session/local_session_keep_alive.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/api/release.py` & `kaskada-0.5.1/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/api/remote_session/__init__.py` & `kaskada-0.5.1/src/kaskada/api/remote_session/__init__.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/api/session.py` & `kaskada-0.5.1/src/kaskada/api/session.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/client.py` & `kaskada-0.5.1/src/kaskada/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,18 +266,20 @@
 
 def set_default_slice(slice: SliceFilter):
     """Sets the default slice used in every query
 
     Args:
         slice (SliceFilter): SliceFilter to set the default
     """
-    logger.debug(f"Default slice set to type {type(slice)}")
-
     global KASKADA_DEFAULT_SLICE
     KASKADA_DEFAULT_SLICE = slice
+    if KASKADA_DEFAULT_SLICE is None:
+        logger.info("Slicing disabled")
+    else:
+        logger.info(f"Slicing set to: {slice.to_request()}")
 
 
 def set_default_client(client: Client):
     """Sets the default client used in every query
 
     Args:
         client (Client): the target client
```

### Comparing `kaskada-0.5.0/src/kaskada/formatters.css` & `kaskada-0.5.1/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/formatters.js` & `kaskada-0.5.1/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/formatters.py` & `kaskada-0.5.1/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/formatters_helpers.py` & `kaskada-0.5.1/src/kaskada/formatters_helpers.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/formatters_shared.py` & `kaskada-0.5.1/src/kaskada/formatters_shared.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/health/health_check_client.py` & `kaskada-0.5.1/src/kaskada/health/health_check_client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/health/health_check_servicer.py` & `kaskada-0.5.1/src/kaskada/health/health_check_servicer.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/health/health_check_watcher.py` & `kaskada-0.5.1/src/kaskada/health/health_check_watcher.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/common_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/common_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/compute_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/destinations_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/file_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/kafka_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/kafka_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/options_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/options_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/plan_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/plan_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from kaskada.kaskada.v1alpha import common_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_common__pb2
 from kaskada.kaskada.v1alpha import schema_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_schema__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"kaskada/kaskada/v1alpha/plan.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"\xba\x02\n\x0b\x43omputePlan\x12Z\n\x13per_entity_behavior\x18\x01 \x01(\x0e\x32*.kaskada.kaskada.v1alpha.PerEntityBehaviorR\x11perEntityBehavior\x12\x46\n\noperations\x18\x02 \x03(\x0b\x32&.kaskada.kaskada.v1alpha.OperationPlanR\noperations\x12)\n\x10primary_grouping\x18\x03 \x01(\tR\x0fprimaryGrouping\x12\\\n\x19primary_grouping_key_type\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x16primaryGroupingKeyType\"\xc6\x12\n\rOperationPlan\x12I\n\x0b\x65xpressions\x18\x01 \x03(\x0b\x32\'.kaskada.kaskada.v1alpha.ExpressionPlanR\x0b\x65xpressions\x12J\n\x04scan\x18\x02 \x01(\x0b\x32\x34.kaskada.kaskada.v1alpha.OperationPlan.ScanOperationH\x00R\x04scan\x12M\n\x05merge\x18\x03 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.OperationPlan.MergeOperationH\x00R\x05merge\x12P\n\x06select\x18\x04 \x01(\x0b\x32\x36.kaskada.kaskada.v1alpha.OperationPlan.SelectOperationH\x00R\x06select\x12J\n\x04tick\x18\x05 \x01(\x0b\x32\x34.kaskada.kaskada.v1alpha.OperationPlan.TickOperationH\x00R\x04tick\x12T\n\x08with_key\x18\x06 \x01(\x0b\x32\x37.kaskada.kaskada.v1alpha.OperationPlan.WithKeyOperationH\x00R\x07withKey\x12\x66\n\x0elookup_request\x18\x07 \x01(\x0b\x32=.kaskada.kaskada.v1alpha.OperationPlan.LookupRequestOperationH\x00R\rlookupRequest\x12i\n\x0flookup_response\x18\x08 \x01(\x0b\x32>.kaskada.kaskada.v1alpha.OperationPlan.LookupResponseOperationH\x00R\x0elookupResponse\x12T\n\x08shift_to\x18\t \x01(\x0b\x32\x37.kaskada.kaskada.v1alpha.OperationPlan.ShiftToOperationH\x00R\x07shiftTo\x12]\n\x0bshift_until\x18\n \x01(\x0b\x32:.kaskada.kaskada.v1alpha.OperationPlan.ShiftUntilOperationH\x00R\nshiftUntil\x1a\xc5\x01\n\rScanOperation\x12\x38\n\x08table_id\x18\x01 \x01(\x0b\x32\x1d.kaskada.kaskada.v1alpha.UuidR\x07tableId\x12\x37\n\x06schema\x18\x02 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\x12\x41\n\nslice_plan\x18\x03 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\tslicePlan\x1a:\n\x0eMergeOperation\x12\x12\n\x04left\x18\x01 \x01(\rR\x04left\x12\x14\n\x05right\x18\x02 \x01(\rR\x05right\x1aq\n\x0fSelectOperation\x12\x14\n\x05input\x18\x01 \x01(\rR\x05input\x12H\n\tcondition\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\tcondition\x1a\x89\x01\n\x10WithKeyOperation\x12\x14\n\x05input\x18\x01 \x01(\rR\x05input\x12\x43\n\x07new_key\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\x06newKey\x12\x1a\n\x08grouping\x18\x03 \x01(\tR\x08grouping\x1a\xd4\x02\n\rTickOperation\x12]\n\x08\x62\x65havior\x18\x01 \x01(\x0e\x32\x41.kaskada.kaskada.v1alpha.OperationPlan.TickOperation.TickBehaviorR\x08\x62\x65havior\x12\x14\n\x05input\x18\x02 \x01(\rR\x05input\"\xcd\x01\n\x0cTickBehavior\x12\x1d\n\x19TICK_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x1a\n\x16TICK_BEHAVIOR_FINISHED\x10\x01\x12\x18\n\x14TICK_BEHAVIOR_HOURLY\x10\x02\x12\x17\n\x13TICK_BEHAVIOR_DAILY\x10\x03\x12\x19\n\x15TICK_BEHAVIOR_MONTHLY\x10\x04\x12\x18\n\x14TICK_BEHAVIOR_YEARLY\x10\x05\x12\x1a\n\x16TICK_BEHAVIOR_MINUTELY\x10\x06\x1a\x9b\x01\n\x16LookupRequestOperation\x12+\n\x11primary_operation\x18\x01 \x01(\rR\x10primaryOperation\x12T\n\x10\x66oreign_key_hash\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\x0e\x66oreignKeyHash\x1a\xa2\x01\n\x17LookupResponseOperation\x12+\n\x11\x66oreign_operation\x18\x01 \x01(\rR\x10\x66oreignOperation\x12Z\n\x13requesting_key_hash\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\x11requestingKeyHash\x1a\xb2\x01\n\x10ShiftToOperation\x12\x14\n\x05input\x18\x01 \x01(\rR\x05input\x12H\n\x08\x63omputed\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefH\x00R\x08\x63omputed\x12\x36\n\x07literal\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00R\x07literalB\x06\n\x04time\x1au\n\x13ShiftUntilOperation\x12\x14\n\x05input\x18\x01 \x01(\rR\x05input\x12H\n\tcondition\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\tconditionB\n\n\x08operator\"\x86\x03\n\x0e\x45xpressionPlan\x12\x1c\n\targuments\x18\x01 \x03(\rR\targuments\x12\x42\n\x0bresult_type\x18\x02 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\nresultType\x12\x16\n\x06output\x18\x03 \x01(\x08R\x06output\x12\"\n\x0binstruction\x18\x04 \x01(\tH\x00R\x0binstruction\x12\x42\n\x05input\x18\x05 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefH\x00R\x05input\x12<\n\x07literal\x18\x06 \x01(\x0b\x32 .kaskada.kaskada.v1alpha.LiteralH\x00R\x07literal\x12H\n\nlate_bound\x18\x07 \x01(\x0e\x32\'.kaskada.kaskada.v1alpha.LateBoundValueH\x00R\tlateBoundB\n\n\x08operator\"\xb5\n\n\x07Literal\x12\x14\n\x04\x62ool\x18\x08 \x01(\x08H\x00R\x04\x62ool\x12\x14\n\x04int8\x18\t \x01(\x05H\x00R\x04int8\x12\x16\n\x05int16\x18\n \x01(\x05H\x00R\x05int16\x12\x16\n\x05int32\x18\x0b \x01(\x05H\x00R\x05int32\x12\x16\n\x05int64\x18\x0c \x01(\x03H\x00R\x05int64\x12\x16\n\x05uint8\x18\r \x01(\rH\x00R\x05uint8\x12\x18\n\x06uint16\x18\x0e \x01(\rH\x00R\x06uint16\x12\x18\n\x06uint32\x18\x0f \x01(\rH\x00R\x06uint32\x12\x18\n\x06uint64\x18\x10 \x01(\x04H\x00R\x06uint64\x12\x1a\n\x07\x66loat32\x18\x11 \x01(\x02H\x00R\x07\x66loat32\x12\x1a\n\x07\x66loat64\x18\x12 \x01(\x01H\x00R\x07\x66loat64\x12O\n\ttimestamp\x18\x13 \x01(\x0b\x32/.kaskada.kaskada.v1alpha.Literal.TimestampValueH\x00R\ttimestamp\x12\x18\n\x06\x64\x61te32\x18\x14 \x01(\x05H\x00R\x06\x64\x61te32\x12\x18\n\x06\x64\x61te64\x18\x15 \x01(\x03H\x00R\x06\x64\x61te64\x12\x46\n\x06time32\x18\x16 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.Literal.Time32ValueH\x00R\x06time32\x12\x46\n\x06time64\x18\x17 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.Literal.Time64ValueH\x00R\x06time64\x12L\n\x08\x64uration\x18\x18 \x01(\x0b\x32..kaskada.kaskada.v1alpha.Literal.DurationValueH\x00R\x08\x64uration\x12\x63\n\x11interval_day_time\x18\x19 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.Literal.IntervalDayTimeValueH\x00R\x0fintervalDayTime\x12)\n\x0finterval_months\x18\x1a \x01(\x05H\x00R\x0eintervalMonths\x12\x14\n\x04utf8\x18\x1b \x01(\tH\x00R\x04utf8\x12\x46\n\x06record\x18\x1c \x01(\x0b\x32,.kaskada.kaskada.v1alpha.Literal.RecordValueH\x00R\x06record\x1a\x85\x01\n\x0eTimestampValue\x12\x31\n\x05value\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x05value\x12\x12\n\x04unit\x18\x02 \x01(\tR\x04unit\x12,\n\x02tz\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x02tz\x1a\x37\n\x0bTime32Value\x12\x14\n\x05value\x18\x01 \x01(\x05R\x05value\x12\x12\n\x04unit\x18\x02 \x01(\tR\x04unit\x1a\x37\n\x0bTime64Value\x12\x14\n\x05value\x18\x01 \x01(\x03R\x05value\x12\x12\n\x04unit\x18\x02 \x01(\tR\x04unit\x1a\x39\n\rDurationValue\x12\x14\n\x05value\x18\x01 \x01(\x03R\x05value\x12\x12\n\x04unit\x18\x02 \x01(\tR\x04unit\x1a>\n\x14IntervalDayTimeValue\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x1aG\n\x0bRecordValue\x12\x38\n\x06values\x18\x01 \x03(\x0b\x32 .kaskada.kaskada.v1alpha.LiteralR\x06valuesB\t\n\x07literal\"\x94\x05\n\x11OperationInputRef\x12/\n\x13producing_operation\x18\x01 \x01(\rR\x12producingOperation\x12U\n\nkey_column\x18\x02 \x01(\x0e\x32\x34.kaskada.kaskada.v1alpha.OperationInputRef.KeyColumnH\x00R\tkeyColumn\x12\x31\n\x13producer_expression\x18\x03 \x01(\rH\x00R\x12producerExpression\x12\x39\n\x0bscan_record\x18\x04 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\nscanRecord\x12,\n\x04tick\x18\x07 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\x04tick\x12!\n\x0cinput_column\x18\x05 \x01(\rR\x0binputColumn\x12^\n\rinterpolation\x18\x06 \x01(\x0e\x32\x38.kaskada.kaskada.v1alpha.OperationInputRef.InterpolationR\rinterpolation\"m\n\tKeyColumn\x12\x1a\n\x16KEY_COLUMN_UNSPECIFIED\x10\x00\x12\x13\n\x0fKEY_COLUMN_TIME\x10\x01\x12\x16\n\x12KEY_COLUMN_SUBSORT\x10\x02\x12\x17\n\x13KEY_COLUMN_KEY_HASH\x10\x03\"_\n\rInterpolation\x12\x1d\n\x19INTERPOLATION_UNSPECIFIED\x10\x00\x12\x16\n\x12INTERPOLATION_NULL\x10\x01\x12\x17\n\x13INTERPOLATION_AS_OF\x10\x02\x42\x08\n\x06\x63olumn*\x7f\n\x0eLateBoundValue\x12 \n\x1cLATE_BOUND_VALUE_UNSPECIFIED\x10\x00\x12\'\n#LATE_BOUND_VALUE_CHANGED_SINCE_TIME\x10\x01\x12\"\n\x1eLATE_BOUND_VALUE_FINAL_AT_TIME\x10\x02\x42\xf9\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\tPlanProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"kaskada/kaskada/v1alpha/plan.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"\xba\x02\n\x0b\x43omputePlan\x12Z\n\x13per_entity_behavior\x18\x01 \x01(\x0e\x32*.kaskada.kaskada.v1alpha.PerEntityBehaviorR\x11perEntityBehavior\x12\x46\n\noperations\x18\x02 \x03(\x0b\x32&.kaskada.kaskada.v1alpha.OperationPlanR\noperations\x12)\n\x10primary_grouping\x18\x03 \x01(\tR\x0fprimaryGrouping\x12\\\n\x19primary_grouping_key_type\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x16primaryGroupingKeyType\"\xc6\x12\n\rOperationPlan\x12I\n\x0b\x65xpressions\x18\x01 \x03(\x0b\x32\'.kaskada.kaskada.v1alpha.ExpressionPlanR\x0b\x65xpressions\x12J\n\x04scan\x18\x02 \x01(\x0b\x32\x34.kaskada.kaskada.v1alpha.OperationPlan.ScanOperationH\x00R\x04scan\x12M\n\x05merge\x18\x03 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.OperationPlan.MergeOperationH\x00R\x05merge\x12P\n\x06select\x18\x04 \x01(\x0b\x32\x36.kaskada.kaskada.v1alpha.OperationPlan.SelectOperationH\x00R\x06select\x12J\n\x04tick\x18\x05 \x01(\x0b\x32\x34.kaskada.kaskada.v1alpha.OperationPlan.TickOperationH\x00R\x04tick\x12T\n\x08with_key\x18\x06 \x01(\x0b\x32\x37.kaskada.kaskada.v1alpha.OperationPlan.WithKeyOperationH\x00R\x07withKey\x12\x66\n\x0elookup_request\x18\x07 \x01(\x0b\x32=.kaskada.kaskada.v1alpha.OperationPlan.LookupRequestOperationH\x00R\rlookupRequest\x12i\n\x0flookup_response\x18\x08 \x01(\x0b\x32>.kaskada.kaskada.v1alpha.OperationPlan.LookupResponseOperationH\x00R\x0elookupResponse\x12T\n\x08shift_to\x18\t \x01(\x0b\x32\x37.kaskada.kaskada.v1alpha.OperationPlan.ShiftToOperationH\x00R\x07shiftTo\x12]\n\x0bshift_until\x18\n \x01(\x0b\x32:.kaskada.kaskada.v1alpha.OperationPlan.ShiftUntilOperationH\x00R\nshiftUntil\x1a\xc5\x01\n\rScanOperation\x12\x38\n\x08table_id\x18\x01 \x01(\x0b\x32\x1d.kaskada.kaskada.v1alpha.UuidR\x07tableId\x12\x37\n\x06schema\x18\x02 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\x12\x41\n\nslice_plan\x18\x03 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\tslicePlan\x1a:\n\x0eMergeOperation\x12\x12\n\x04left\x18\x01 \x01(\rR\x04left\x12\x14\n\x05right\x18\x02 \x01(\rR\x05right\x1aq\n\x0fSelectOperation\x12\x14\n\x05input\x18\x01 \x01(\rR\x05input\x12H\n\tcondition\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\tcondition\x1a\x89\x01\n\x10WithKeyOperation\x12\x14\n\x05input\x18\x01 \x01(\rR\x05input\x12\x43\n\x07new_key\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\x06newKey\x12\x1a\n\x08grouping\x18\x03 \x01(\tR\x08grouping\x1a\xd4\x02\n\rTickOperation\x12]\n\x08\x62\x65havior\x18\x01 \x01(\x0e\x32\x41.kaskada.kaskada.v1alpha.OperationPlan.TickOperation.TickBehaviorR\x08\x62\x65havior\x12\x14\n\x05input\x18\x02 \x01(\rR\x05input\"\xcd\x01\n\x0cTickBehavior\x12\x1d\n\x19TICK_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x1a\n\x16TICK_BEHAVIOR_FINISHED\x10\x01\x12\x18\n\x14TICK_BEHAVIOR_HOURLY\x10\x02\x12\x17\n\x13TICK_BEHAVIOR_DAILY\x10\x03\x12\x19\n\x15TICK_BEHAVIOR_MONTHLY\x10\x04\x12\x18\n\x14TICK_BEHAVIOR_YEARLY\x10\x05\x12\x1a\n\x16TICK_BEHAVIOR_MINUTELY\x10\x06\x1a\x9b\x01\n\x16LookupRequestOperation\x12+\n\x11primary_operation\x18\x01 \x01(\rR\x10primaryOperation\x12T\n\x10\x66oreign_key_hash\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\x0e\x66oreignKeyHash\x1a\xa2\x01\n\x17LookupResponseOperation\x12+\n\x11\x66oreign_operation\x18\x01 \x01(\rR\x10\x66oreignOperation\x12Z\n\x13requesting_key_hash\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\x11requestingKeyHash\x1a\xb2\x01\n\x10ShiftToOperation\x12\x14\n\x05input\x18\x01 \x01(\rR\x05input\x12H\n\x08\x63omputed\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefH\x00R\x08\x63omputed\x12\x36\n\x07literal\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00R\x07literalB\x06\n\x04time\x1au\n\x13ShiftUntilOperation\x12\x14\n\x05input\x18\x01 \x01(\rR\x05input\x12H\n\tcondition\x18\x02 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefR\tconditionB\n\n\x08operator\"\x86\x03\n\x0e\x45xpressionPlan\x12\x1c\n\targuments\x18\x01 \x03(\rR\targuments\x12\x42\n\x0bresult_type\x18\x02 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\nresultType\x12\x16\n\x06output\x18\x03 \x01(\x08R\x06output\x12\"\n\x0binstruction\x18\x04 \x01(\tH\x00R\x0binstruction\x12\x42\n\x05input\x18\x05 \x01(\x0b\x32*.kaskada.kaskada.v1alpha.OperationInputRefH\x00R\x05input\x12<\n\x07literal\x18\x06 \x01(\x0b\x32 .kaskada.kaskada.v1alpha.LiteralH\x00R\x07literal\x12H\n\nlate_bound\x18\x07 \x01(\x0e\x32\'.kaskada.kaskada.v1alpha.LateBoundValueH\x00R\tlateBoundB\n\n\x08operator\"\xd6\n\n\x07Literal\x12\x14\n\x04\x62ool\x18\x08 \x01(\x08H\x00R\x04\x62ool\x12\x14\n\x04int8\x18\t \x01(\x05H\x00R\x04int8\x12\x16\n\x05int16\x18\n \x01(\x05H\x00R\x05int16\x12\x16\n\x05int32\x18\x0b \x01(\x05H\x00R\x05int32\x12\x16\n\x05int64\x18\x0c \x01(\x03H\x00R\x05int64\x12\x16\n\x05uint8\x18\r \x01(\rH\x00R\x05uint8\x12\x18\n\x06uint16\x18\x0e \x01(\rH\x00R\x06uint16\x12\x18\n\x06uint32\x18\x0f \x01(\rH\x00R\x06uint32\x12\x18\n\x06uint64\x18\x10 \x01(\x04H\x00R\x06uint64\x12\x1a\n\x07\x66loat32\x18\x11 \x01(\x02H\x00R\x07\x66loat32\x12\x1a\n\x07\x66loat64\x18\x12 \x01(\x01H\x00R\x07\x66loat64\x12O\n\ttimestamp\x18\x13 \x01(\x0b\x32/.kaskada.kaskada.v1alpha.Literal.TimestampValueH\x00R\ttimestamp\x12\x18\n\x06\x64\x61te32\x18\x14 \x01(\x05H\x00R\x06\x64\x61te32\x12\x18\n\x06\x64\x61te64\x18\x15 \x01(\x03H\x00R\x06\x64\x61te64\x12\x46\n\x06time32\x18\x16 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.Literal.Time32ValueH\x00R\x06time32\x12\x46\n\x06time64\x18\x17 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.Literal.Time64ValueH\x00R\x06time64\x12L\n\x08\x64uration\x18\x18 \x01(\x0b\x32..kaskada.kaskada.v1alpha.Literal.DurationValueH\x00R\x08\x64uration\x12\x63\n\x11interval_day_time\x18\x19 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.Literal.IntervalDayTimeValueH\x00R\x0fintervalDayTime\x12)\n\x0finterval_months\x18\x1a \x01(\x05H\x00R\x0eintervalMonths\x12\x14\n\x04utf8\x18\x1b \x01(\tH\x00R\x04utf8\x12\x1f\n\nlarge_utf8\x18\x1d \x01(\tH\x00R\tlargeUtf8\x12\x46\n\x06record\x18\x1c \x01(\x0b\x32,.kaskada.kaskada.v1alpha.Literal.RecordValueH\x00R\x06record\x1a\x85\x01\n\x0eTimestampValue\x12\x31\n\x05value\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x05value\x12\x12\n\x04unit\x18\x02 \x01(\tR\x04unit\x12,\n\x02tz\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x02tz\x1a\x37\n\x0bTime32Value\x12\x14\n\x05value\x18\x01 \x01(\x05R\x05value\x12\x12\n\x04unit\x18\x02 \x01(\tR\x04unit\x1a\x37\n\x0bTime64Value\x12\x14\n\x05value\x18\x01 \x01(\x03R\x05value\x12\x12\n\x04unit\x18\x02 \x01(\tR\x04unit\x1a\x39\n\rDurationValue\x12\x14\n\x05value\x18\x01 \x01(\x03R\x05value\x12\x12\n\x04unit\x18\x02 \x01(\tR\x04unit\x1a>\n\x14IntervalDayTimeValue\x12\x14\n\x05start\x18\x01 \x01(\x05R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x05R\x03\x65nd\x1aG\n\x0bRecordValue\x12\x38\n\x06values\x18\x01 \x03(\x0b\x32 .kaskada.kaskada.v1alpha.LiteralR\x06valuesB\t\n\x07literal\"\x94\x05\n\x11OperationInputRef\x12/\n\x13producing_operation\x18\x01 \x01(\rR\x12producingOperation\x12U\n\nkey_column\x18\x02 \x01(\x0e\x32\x34.kaskada.kaskada.v1alpha.OperationInputRef.KeyColumnH\x00R\tkeyColumn\x12\x31\n\x13producer_expression\x18\x03 \x01(\rH\x00R\x12producerExpression\x12\x39\n\x0bscan_record\x18\x04 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\nscanRecord\x12,\n\x04tick\x18\x07 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\x04tick\x12!\n\x0cinput_column\x18\x05 \x01(\rR\x0binputColumn\x12^\n\rinterpolation\x18\x06 \x01(\x0e\x32\x38.kaskada.kaskada.v1alpha.OperationInputRef.InterpolationR\rinterpolation\"m\n\tKeyColumn\x12\x1a\n\x16KEY_COLUMN_UNSPECIFIED\x10\x00\x12\x13\n\x0fKEY_COLUMN_TIME\x10\x01\x12\x16\n\x12KEY_COLUMN_SUBSORT\x10\x02\x12\x17\n\x13KEY_COLUMN_KEY_HASH\x10\x03\"_\n\rInterpolation\x12\x1d\n\x19INTERPOLATION_UNSPECIFIED\x10\x00\x12\x16\n\x12INTERPOLATION_NULL\x10\x01\x12\x17\n\x13INTERPOLATION_AS_OF\x10\x02\x42\x08\n\x06\x63olumn*\x7f\n\x0eLateBoundValue\x12 \n\x1cLATE_BOUND_VALUE_UNSPECIFIED\x10\x00\x12\'\n#LATE_BOUND_VALUE_CHANGED_SINCE_TIME\x10\x01\x12\"\n\x1eLATE_BOUND_VALUE_FINAL_AT_TIME\x10\x02\x42\xf9\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\tPlanProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.plan_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\tPlanProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _globals['_LATEBOUNDVALUE']._serialized_start=5319
-  _globals['_LATEBOUNDVALUE']._serialized_end=5446
+  _globals['_LATEBOUNDVALUE']._serialized_start=5352
+  _globals['_LATEBOUNDVALUE']._serialized_end=5479
   _globals['_COMPUTEPLAN']._serialized_start=234
   _globals['_COMPUTEPLAN']._serialized_end=548
   _globals['_OPERATIONPLAN']._serialized_start=551
   _globals['_OPERATIONPLAN']._serialized_end=2925
   _globals['_OPERATIONPLAN_SCANOPERATION']._serialized_start=1435
   _globals['_OPERATIONPLAN_SCANOPERATION']._serialized_end=1632
   _globals['_OPERATIONPLAN_MERGEOPERATION']._serialized_start=1634
@@ -52,27 +52,27 @@
   _globals['_OPERATIONPLAN_SHIFTTOOPERATION']._serialized_start=2616
   _globals['_OPERATIONPLAN_SHIFTTOOPERATION']._serialized_end=2794
   _globals['_OPERATIONPLAN_SHIFTUNTILOPERATION']._serialized_start=2796
   _globals['_OPERATIONPLAN_SHIFTUNTILOPERATION']._serialized_end=2913
   _globals['_EXPRESSIONPLAN']._serialized_start=2928
   _globals['_EXPRESSIONPLAN']._serialized_end=3318
   _globals['_LITERAL']._serialized_start=3321
-  _globals['_LITERAL']._serialized_end=4654
-  _globals['_LITERAL_TIMESTAMPVALUE']._serialized_start=4200
-  _globals['_LITERAL_TIMESTAMPVALUE']._serialized_end=4333
-  _globals['_LITERAL_TIME32VALUE']._serialized_start=4335
-  _globals['_LITERAL_TIME32VALUE']._serialized_end=4390
-  _globals['_LITERAL_TIME64VALUE']._serialized_start=4392
-  _globals['_LITERAL_TIME64VALUE']._serialized_end=4447
-  _globals['_LITERAL_DURATIONVALUE']._serialized_start=4449
-  _globals['_LITERAL_DURATIONVALUE']._serialized_end=4506
-  _globals['_LITERAL_INTERVALDAYTIMEVALUE']._serialized_start=4508
-  _globals['_LITERAL_INTERVALDAYTIMEVALUE']._serialized_end=4570
-  _globals['_LITERAL_RECORDVALUE']._serialized_start=4572
-  _globals['_LITERAL_RECORDVALUE']._serialized_end=4643
-  _globals['_OPERATIONINPUTREF']._serialized_start=4657
-  _globals['_OPERATIONINPUTREF']._serialized_end=5317
-  _globals['_OPERATIONINPUTREF_KEYCOLUMN']._serialized_start=5101
-  _globals['_OPERATIONINPUTREF_KEYCOLUMN']._serialized_end=5210
-  _globals['_OPERATIONINPUTREF_INTERPOLATION']._serialized_start=5212
-  _globals['_OPERATIONINPUTREF_INTERPOLATION']._serialized_end=5307
+  _globals['_LITERAL']._serialized_end=4687
+  _globals['_LITERAL_TIMESTAMPVALUE']._serialized_start=4233
+  _globals['_LITERAL_TIMESTAMPVALUE']._serialized_end=4366
+  _globals['_LITERAL_TIME32VALUE']._serialized_start=4368
+  _globals['_LITERAL_TIME32VALUE']._serialized_end=4423
+  _globals['_LITERAL_TIME64VALUE']._serialized_start=4425
+  _globals['_LITERAL_TIME64VALUE']._serialized_end=4480
+  _globals['_LITERAL_DURATIONVALUE']._serialized_start=4482
+  _globals['_LITERAL_DURATIONVALUE']._serialized_end=4539
+  _globals['_LITERAL_INTERVALDAYTIMEVALUE']._serialized_start=4541
+  _globals['_LITERAL_INTERVALDAYTIMEVALUE']._serialized_end=4603
+  _globals['_LITERAL_RECORDVALUE']._serialized_start=4605
+  _globals['_LITERAL_RECORDVALUE']._serialized_end=4676
+  _globals['_OPERATIONINPUTREF']._serialized_start=4690
+  _globals['_OPERATIONINPUTREF']._serialized_end=5350
+  _globals['_OPERATIONINPUTREF_KEYCOLUMN']._serialized_start=5134
+  _globals['_OPERATIONINPUTREF_KEYCOLUMN']._serialized_end=5243
+  _globals['_OPERATIONINPUTREF_INTERPOLATION']._serialized_start=5245
+  _globals['_OPERATIONINPUTREF_INTERPOLATION']._serialized_end=5340
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/pulsar_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/schema_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/schema_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/schema.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1bgoogle/protobuf/empty.proto\"\x80\n\n\x08\x44\x61taType\x12O\n\tprimitive\x18\x01 \x01(\x0e\x32/.kaskada.kaskada.v1alpha.DataType.PrimitiveTypeH\x00R\tprimitive\x12\x39\n\x06struct\x18\x02 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaH\x00R\x06struct\x12\x30\n\x06window\x18\x03 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\x06window\x12\x37\n\x04list\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeH\x00R\x04list\x12\x39\n\x03map\x18\x05 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.DataType.MapH\x00R\x03map\x1as\n\x03Map\x12\x33\n\x03key\x18\x01 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x03key\x12\x37\n\x05value\x18\x02 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x05value\"\xc4\x06\n\rPrimitiveType\x12\x1e\n\x1aPRIMITIVE_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13PRIMITIVE_TYPE_NULL\x10\x01\x12\x17\n\x13PRIMITIVE_TYPE_BOOL\x10\x02\x12\x15\n\x11PRIMITIVE_TYPE_I8\x10\x03\x12\x16\n\x12PRIMITIVE_TYPE_I16\x10\x04\x12\x16\n\x12PRIMITIVE_TYPE_I32\x10\x05\x12\x16\n\x12PRIMITIVE_TYPE_I64\x10\x06\x12\x15\n\x11PRIMITIVE_TYPE_U8\x10\x07\x12\x16\n\x12PRIMITIVE_TYPE_U16\x10\x08\x12\x16\n\x12PRIMITIVE_TYPE_U32\x10\t\x12\x16\n\x12PRIMITIVE_TYPE_U64\x10\n\x12\x16\n\x12PRIMITIVE_TYPE_F16\x10\x0b\x12\x16\n\x12PRIMITIVE_TYPE_F32\x10\x0c\x12\x16\n\x12PRIMITIVE_TYPE_F64\x10\r\x12\x19\n\x15PRIMITIVE_TYPE_STRING\x10\x0e\x12$\n PRIMITIVE_TYPE_INTERVAL_DAY_TIME\x10\x0f\x12&\n\"PRIMITIVE_TYPE_INTERVAL_YEAR_MONTH\x10\x10\x12\"\n\x1ePRIMITIVE_TYPE_DURATION_SECOND\x10\x11\x12\'\n#PRIMITIVE_TYPE_DURATION_MILLISECOND\x10\x12\x12\'\n#PRIMITIVE_TYPE_DURATION_MICROSECOND\x10\x13\x12&\n\"PRIMITIVE_TYPE_DURATION_NANOSECOND\x10\x14\x12#\n\x1fPRIMITIVE_TYPE_TIMESTAMP_SECOND\x10\x15\x12(\n$PRIMITIVE_TYPE_TIMESTAMP_MILLISECOND\x10\x16\x12(\n$PRIMITIVE_TYPE_TIMESTAMP_MICROSECOND\x10\x17\x12\'\n#PRIMITIVE_TYPE_TIMESTAMP_NANOSECOND\x10\x18\x12\x17\n\x13PRIMITIVE_TYPE_JSON\x10\x19\x12\x19\n\x15PRIMITIVE_TYPE_DATE32\x10\x1a\x42\x06\n\x04kind\"\xa4\x01\n\x06Schema\x12=\n\x06\x66ields\x18\x01 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.Schema.FieldR\x06\x66ields\x1a[\n\x05\x46ield\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\tdata_type\x18\x02 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x08\x64\x61taTypeB\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0bSchemaProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/schema.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1bgoogle/protobuf/empty.proto\"\xf0\x0b\n\x08\x44\x61taType\x12O\n\tprimitive\x18\x01 \x01(\x0e\x32/.kaskada.kaskada.v1alpha.DataType.PrimitiveTypeH\x00R\tprimitive\x12\x39\n\x06struct\x18\x02 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaH\x00R\x06struct\x12\x30\n\x06window\x18\x03 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\x06window\x12\x37\n\x04list\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeH\x00R\x04list\x12\x39\n\x03map\x18\x05 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.DataType.MapH\x00R\x03map\x1a\xc1\x02\n\x03Map\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07ordered\x18\x02 \x01(\x08R\x07ordered\x12\x19\n\x08key_name\x18\x03 \x01(\tR\x07keyName\x12<\n\x08key_type\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x07keyType\x12&\n\x0fkey_is_nullable\x18\x05 \x01(\x08R\rkeyIsNullable\x12\x1d\n\nvalue_name\x18\x06 \x01(\tR\tvalueName\x12@\n\nvalue_type\x18\x07 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\tvalueType\x12*\n\x11value_is_nullable\x18\x08 \x01(\x08R\x0fvalueIsNullable\"\xe5\x06\n\rPrimitiveType\x12\x1e\n\x1aPRIMITIVE_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13PRIMITIVE_TYPE_NULL\x10\x01\x12\x17\n\x13PRIMITIVE_TYPE_BOOL\x10\x02\x12\x15\n\x11PRIMITIVE_TYPE_I8\x10\x03\x12\x16\n\x12PRIMITIVE_TYPE_I16\x10\x04\x12\x16\n\x12PRIMITIVE_TYPE_I32\x10\x05\x12\x16\n\x12PRIMITIVE_TYPE_I64\x10\x06\x12\x15\n\x11PRIMITIVE_TYPE_U8\x10\x07\x12\x16\n\x12PRIMITIVE_TYPE_U16\x10\x08\x12\x16\n\x12PRIMITIVE_TYPE_U32\x10\t\x12\x16\n\x12PRIMITIVE_TYPE_U64\x10\n\x12\x16\n\x12PRIMITIVE_TYPE_F16\x10\x0b\x12\x16\n\x12PRIMITIVE_TYPE_F32\x10\x0c\x12\x16\n\x12PRIMITIVE_TYPE_F64\x10\r\x12\x19\n\x15PRIMITIVE_TYPE_STRING\x10\x0e\x12\x1f\n\x1bPRIMITIVE_TYPE_LARGE_STRING\x10\x1b\x12$\n PRIMITIVE_TYPE_INTERVAL_DAY_TIME\x10\x0f\x12&\n\"PRIMITIVE_TYPE_INTERVAL_YEAR_MONTH\x10\x10\x12\"\n\x1ePRIMITIVE_TYPE_DURATION_SECOND\x10\x11\x12\'\n#PRIMITIVE_TYPE_DURATION_MILLISECOND\x10\x12\x12\'\n#PRIMITIVE_TYPE_DURATION_MICROSECOND\x10\x13\x12&\n\"PRIMITIVE_TYPE_DURATION_NANOSECOND\x10\x14\x12#\n\x1fPRIMITIVE_TYPE_TIMESTAMP_SECOND\x10\x15\x12(\n$PRIMITIVE_TYPE_TIMESTAMP_MILLISECOND\x10\x16\x12(\n$PRIMITIVE_TYPE_TIMESTAMP_MICROSECOND\x10\x17\x12\'\n#PRIMITIVE_TYPE_TIMESTAMP_NANOSECOND\x10\x18\x12\x17\n\x13PRIMITIVE_TYPE_JSON\x10\x19\x12\x19\n\x15PRIMITIVE_TYPE_DATE32\x10\x1a\x42\x06\n\x04kind\"\xc0\x01\n\x06Schema\x12=\n\x06\x66ields\x18\x01 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.Schema.FieldR\x06\x66ields\x1aw\n\x05\x46ield\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12>\n\tdata_type\x18\x02 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\x08\x64\x61taType\x12\x1a\n\x08nullable\x18\x03 \x01(\x08R\x08nullableB\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0bSchemaProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.schema_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\013SchemaProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
   _globals['_DATATYPE']._serialized_start=95
-  _globals['_DATATYPE']._serialized_end=1375
-  _globals['_DATATYPE_MAP']._serialized_start=413
-  _globals['_DATATYPE_MAP']._serialized_end=528
-  _globals['_DATATYPE_PRIMITIVETYPE']._serialized_start=531
-  _globals['_DATATYPE_PRIMITIVETYPE']._serialized_end=1367
-  _globals['_SCHEMA']._serialized_start=1378
-  _globals['_SCHEMA']._serialized_end=1542
-  _globals['_SCHEMA_FIELD']._serialized_start=1451
-  _globals['_SCHEMA_FIELD']._serialized_end=1542
+  _globals['_DATATYPE']._serialized_end=1615
+  _globals['_DATATYPE_MAP']._serialized_start=414
+  _globals['_DATATYPE_MAP']._serialized_end=735
+  _globals['_DATATYPE_PRIMITIVETYPE']._serialized_start=738
+  _globals['_DATATYPE_PRIMITIVETYPE']._serialized_end=1607
+  _globals['_SCHEMA']._serialized_start=1618
+  _globals['_SCHEMA']._serialized_end=1810
+  _globals['_SCHEMA_FIELD']._serialized_start=1691
+  _globals['_SCHEMA_FIELD']._serialized_end=1810
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/sources_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/sources_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/spec_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/table_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/test_cases_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/view_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py` & `kaskada-0.5.1/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py` & `kaskada-0.5.1/src/kaskada/kaskada/v2alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py` & `kaskada-0.5.1/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/materialization.py` & `kaskada-0.5.1/src/kaskada/materialization.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/query.py` & `kaskada-0.5.1/src/kaskada/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import grpc
 from google.protobuf.message import Message
 
 import kaskada.formatters
 import kaskada.kaskada.v1alpha.destinations_pb2 as destinations_pb
 import kaskada.kaskada.v1alpha.query_service_pb2 as query_pb
-from kaskada.client import KASKADA_DEFAULT_SLICE, Client, get_client
+from kaskada.client import Client, get_client
 from kaskada.slice_filters import SliceFilter
 from kaskada.utils import get_timestamp, handleException, handleGrpcError
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
@@ -130,15 +130,27 @@
         client (Client, optional):
             The Kaskada Client. Defaults to kaskada.KASKADA_DEFAULT_CLIENT.
 
     Returns:
         query_pb.CreateQueryResponse
     """
     if slice_filter is None:
-        slice_filter = KASKADA_DEFAULT_SLICE
+        """
+        Subtle Python Implementation Note:
+
+        The KASKADA_DEFAULT_SLICE is a global variable that varies at runtime. Users can set the default slice at any point.
+        The value of the slice is evaluated at execution time of this method.
+
+        Incorrect: from kaskada.client import KASKADA_DEFAULT_SLICE
+            This value is evaluated once at the import of the query module.
+
+        Correct: import kaskada.client
+            The value is then fetched from the module every time a query is invoked.
+        """
+        slice_filter = kaskada.client.KASKADA_DEFAULT_SLICE
 
     change_since_time = get_timestamp(changed_since_time)
     final_result_time = get_timestamp(final_result_time)
 
     try:
         client = get_client(client)
         query_options = {
```

### Comparing `kaskada-0.5.0/src/kaskada/slice_filters.py` & `kaskada-0.5.1/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/table.py` & `kaskada-0.5.1/src/kaskada/table.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/utils.py` & `kaskada-0.5.1/src/kaskada/utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/src/kaskada/view.py` & `kaskada-0.5.1/src/kaskada/view.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/vendor/validate/validate.proto` & `kaskada-0.5.1/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/vendor/validate/validate_pb2.py` & `kaskada-0.5.1/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/vendor/validate/validate_pb2.pyi` & `kaskada-0.5.1/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.5.0/setup.py` & `kaskada-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'pyarrow>=10.0.1,<11.0.0',
  'pygithub>=1.57,<2.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'kaskada',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'A client library for the Kaskada time travel machine learning service',
     'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n#### Generate documentation \nWe use Sphinx and rely on autogeneration extensions within Sphinx to read docstrings and \ngenerate an HTML formatted version of the codes documentation. \n\n* `poetry run poe docs` : generates and builds the docs \n* `poetry run poe docs-generate` : generates the docs (.rst files)\n* `poetry run poe docs-build` : builds the HTML rendered version of the generated docs (from .rst to .html)\n\nThe generated HTML is located inside `docs/build`. Load `docs/build/index.html` in your browser to see the HTML rendered output. \n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`\n',
     'author': 'Kaskada',
     'author_email': 'maintainers@kaskada.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kaskada-0.5.0/PKG-INFO` & `kaskada-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.5.0
+Version: 0.5.1
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

