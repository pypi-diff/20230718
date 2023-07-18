# Comparing `tmp/dlt-0.3.4.tar.gz` & `tmp/dlt-0.3.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.3.4.tar", max compression
+gzip compressed data, was "dlt-0.3.5a0.tar", max compression
```

## Comparing `dlt-0.3.4.tar` & `dlt-0.3.5a0.tar`

### file list

```diff
@@ -1,224 +1,224 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.4/LICENSE.txt
--rw-r--r--   0        0        0     4144 2023-07-08 12:23:15.759697 dlt-0.3.4/README.md
--rw-r--r--   0        0        0     1708 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/__init__.py
--rw-r--r--   0        0        0    17127 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3974 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    15046 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    14849 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1853 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18756 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10508 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9588 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4505 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     2308 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.4/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      480 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     6741 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-07-08 12:23:15.759697 dlt-0.3.4/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      344 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      664 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     3662 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    12880 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    18788 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1002 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     2128 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0    14214 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5476 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3387 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12537 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2712 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6559 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-07-15 10:14:14.845022 dlt-0.3.4/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     6203 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2727 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     8426 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      189 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     3158 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    11909 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     8111 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-07-15 10:57:51.195021 dlt-0.3.4/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/jsonpath.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/libs/__init__.py
--rw-r--r--   0        0        0     1657 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/libs/pyarrow.py
--rw-r--r--   0        0        0      232 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/pendulum.py
--rw-r--r--   0        0        0    19531 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13923 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4501 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      771 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7234 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2492 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0     2798 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25164 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23295 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     1906 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     3107 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    11872 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8600 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9506 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2525 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/typing.py
--rw-r--r--   0        0        0    14285 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     2136 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    14030 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10509 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     2257 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7342 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     4135 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6635 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1761 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4989 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4184 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     1270 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/filesystem/__init__.py
--rw-r--r--   0        0        0     2260 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/filesystem/configuration.py
--rw-r--r--   0        0        0     5918 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/filesystem/filesystem.py
--rw-r--r--   0        0        0     1419 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/filesystem/filesystem_client.py
--rw-r--r--   0        0        0     5046 2023-07-15 19:51:36.170686 dlt-0.3.4/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    17153 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     2057 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0     2201 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/motherduck/__init__.py
--rw-r--r--   0        0        0     1807 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/motherduck/configuration.py
--rw-r--r--   0        0        0      968 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/motherduck/motherduck.py
--rw-r--r--   0        0        0     1391 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/motherduck/sql_client.py
--rw-r--r--   0        0        0      251 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     2312 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1377 2023-07-13 15:13:56.520313 dlt-0.3.4/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3176 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     5781 2023-07-15 10:59:55.545022 dlt-0.3.4/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     2237 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      623 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     8620 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     2255 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/snowflake/__init__.py
--rw-r--r--   0        0        0     4075 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/snowflake/configuration.py
--rw-r--r--   0        0        0     9021 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/snowflake/snowflake.py
--rw-r--r--   0        0        0     7069 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/destinations/snowflake/sql_client.py
--rw-r--r--   0        0        0     7776 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10489 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.4/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26516 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12995 2023-07-15 16:23:33.345022 dlt-0.3.4/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8312 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/extract.py
--rw-r--r--   0        0        0    18469 2023-07-15 16:23:33.345022 dlt-0.3.4/dlt/extract/incremental.py
--rw-r--r--   0        0        0    35605 2023-07-15 16:23:33.345022 dlt-0.3.4/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/schema.py
--rw-r--r--   0        0        0    38391 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.4/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    13867 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     3167 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6669 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     5220 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13214 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/helpers/pandas_helper.py
--rw-r--r--   0        0        0    13378 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/helpers/streamlit_helper.py
--rw-r--r--   0        0        0       31 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/load/exceptions.py
--rw-r--r--   0        0        0    22228 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-07-08 12:23:15.769697 dlt-0.3.4/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.4/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16488 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    13633 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     2009 2023-07-15 19:51:36.180686 dlt-0.3.4/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     3100 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8711 2023-07-17 05:20:41.255677 dlt-0.3.4/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    64550 2023-07-17 05:20:41.265677 dlt-0.3.4/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4186 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     9132 2023-07-17 05:20:41.265677 dlt-0.3.4/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4894 2023-07-17 05:20:41.265677 dlt-0.3.4/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.4/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      832 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0    10837 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      234 2023-07-13 09:09:29.104259 dlt-0.3.4/dlt/sources/helpers/requests/typing.py
--rw-r--r--   0        0        0      679 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-07-08 12:23:15.779697 dlt-0.3.4/dlt/version.py
--rw-r--r--   0        0        0     4459 2023-07-17 05:20:41.265677 dlt-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     7760 1970-01-01 00:00:00.000000 dlt-0.3.4/setup.py
--rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 dlt-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.5a0/LICENSE.txt
+-rw-r--r--   0        0        0     4144 2023-07-08 12:23:15.759697 dlt-0.3.5a0/README.md
+-rw-r--r--   0        0        0     1708 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    17127 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3974 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    15046 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    14849 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1853 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18756 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10508 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9588 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4505 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     2308 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.5a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      480 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     6741 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-07-08 12:23:15.759697 dlt-0.3.5a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      344 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      664 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     3662 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    12880 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18788 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1002 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     2128 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0    14214 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5476 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3387 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12537 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2712 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6559 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-07-15 10:14:14.845022 dlt-0.3.5a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     6203 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2727 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     8426 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      189 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     3158 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    11909 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     8111 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-07-15 10:57:51.195021 dlt-0.3.5a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0      232 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    19531 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      771 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7234 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2492 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0     2798 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25164 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23295 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     1906 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     3107 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    11872 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8600 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9506 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2525 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    14285 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     2136 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    14030 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10509 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     2257 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7342 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     4135 2023-07-18 11:51:55.317911 dlt-0.3.5a0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6635 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1761 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4989 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4184 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     1270 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/filesystem/__init__.py
+-rw-r--r--   0        0        0     2260 2023-07-15 19:51:36.170686 dlt-0.3.5a0/dlt/destinations/filesystem/configuration.py
+-rw-r--r--   0        0        0     5918 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1419 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/filesystem/filesystem_client.py
+-rw-r--r--   0        0        0     5046 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    17153 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     2057 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0     2201 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/motherduck/__init__.py
+-rw-r--r--   0        0        0     1807 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/motherduck/configuration.py
+-rw-r--r--   0        0        0      968 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/motherduck/motherduck.py
+-rw-r--r--   0        0        0     1391 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/motherduck/sql_client.py
+-rw-r--r--   0        0        0      251 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     2312 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1377 2023-07-13 15:13:56.520313 dlt-0.3.5a0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3176 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     5781 2023-07-15 10:59:55.545022 dlt-0.3.5a0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     2237 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      623 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     8620 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     2255 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/snowflake/__init__.py
+-rw-r--r--   0        0        0     4075 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/snowflake/configuration.py
+-rw-r--r--   0        0        0     9021 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/snowflake/snowflake.py
+-rw-r--r--   0        0        0     7069 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/destinations/snowflake/sql_client.py
+-rw-r--r--   0        0        0     7776 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10489 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.5a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26516 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12995 2023-07-15 16:23:33.345022 dlt-0.3.5a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8312 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    19337 2023-07-18 12:05:27.467911 dlt-0.3.5a0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    35424 2023-07-18 12:05:27.467911 dlt-0.3.5a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    38391 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.5a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    13867 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3167 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6669 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     5220 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13214 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/helpers/pandas_helper.py
+-rw-r--r--   0        0        0    13378 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/helpers/streamlit_helper.py
+-rw-r--r--   0        0        0       31 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    22228 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-07-08 12:23:15.769697 dlt-0.3.5a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.5a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16488 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    13633 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-15 19:51:36.180686 dlt-0.3.5a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     3100 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8711 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    64550 2023-07-18 11:51:55.327911 dlt-0.3.5a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4186 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     9132 2023-07-18 11:51:55.337911 dlt-0.3.5a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4894 2023-07-18 11:51:55.337911 dlt-0.3.5a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.5a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0    10837 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1757 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      234 2023-07-13 09:09:29.104259 dlt-0.3.5a0/dlt/sources/helpers/requests/typing.py
+-rw-r--r--   0        0        0      679 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-07-08 12:23:15.779697 dlt-0.3.5a0/dlt/version.py
+-rw-r--r--   0        0        0     4461 2023-07-18 12:05:37.647911 dlt-0.3.5a0/pyproject.toml
+-rw-r--r--   0        0        0     7762 1970-01-01 00:00:00.000000 dlt-0.3.5a0/setup.py
+-rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 dlt-0.3.5a0/PKG-INFO
```

### Comparing `dlt-0.3.4/LICENSE.txt` & `dlt-0.3.5a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/README.md` & `dlt-0.3.5a0/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/__init__.py` & `dlt-0.3.5a0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/_dlt.py` & `dlt-0.3.5a0/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/config_toml_writer.py` & `dlt-0.3.5a0/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/deploy_command.py` & `dlt-0.3.5a0/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/deploy_command_helpers.py` & `dlt-0.3.5a0/dlt/cli/deploy_command_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/echo.py` & `dlt-0.3.5a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/init_command.py` & `dlt-0.3.5a0/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/pipeline_command.py` & `dlt-0.3.5a0/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/pipeline_files.py` & `dlt-0.3.5a0/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/source_detection.py` & `dlt-0.3.5a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/telemetry_command.py` & `dlt-0.3.5a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/cli/utils.py` & `dlt-0.3.5a0/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/arithmetics.py` & `dlt-0.3.5a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/accessors.py` & `dlt-0.3.5a0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/container.py` & `dlt-0.3.5a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/exceptions.py` & `dlt-0.3.5a0/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/inject.py` & `dlt-0.3.5a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/paths.py` & `dlt-0.3.5a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/providers/airflow.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/providers/context.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/providers/dictionary.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/providers/environ.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/providers/provider.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/providers/toml.py` & `dlt-0.3.5a0/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/resolve.py` & `dlt-0.3.5a0/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/__init__.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/exceptions.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/known_sections.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.3.5a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/configuration/utils.py` & `dlt-0.3.5a0/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/data_types/type_helpers.py` & `dlt-0.3.5a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/data_writers/buffered.py` & `dlt-0.3.5a0/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/data_writers/escape.py` & `dlt-0.3.5a0/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/data_writers/exceptions.py` & `dlt-0.3.5a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/data_writers/writers.py` & `dlt-0.3.5a0/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/destination/capabilities.py` & `dlt-0.3.5a0/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/destination/reference.py` & `dlt-0.3.5a0/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/exceptions.py` & `dlt-0.3.5a0/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/git.py` & `dlt-0.3.5a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/json/__init__.py` & `dlt-0.3.5a0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/json/_orjson.py` & `dlt-0.3.5a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/json/_simplejson.py` & `dlt-0.3.5a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/jsonpath.py` & `dlt-0.3.5a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/libs/pyarrow.py` & `dlt-0.3.5a0/dlt/common/libs/pyarrow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/normalizers/configuration.py` & `dlt-0.3.5a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/normalizers/json/__init__.py` & `dlt-0.3.5a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/normalizers/json/relational.py` & `dlt-0.3.5a0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/normalizers/naming/direct.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/normalizers/naming/naming.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.3.5a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/normalizers/utils.py` & `dlt-0.3.5a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/pipeline.py` & `dlt-0.3.5a0/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/reflection/spec.py` & `dlt-0.3.5a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/reflection/utils.py` & `dlt-0.3.5a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runners/configuration.py` & `dlt-0.3.5a0/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runners/pool_runner.py` & `dlt-0.3.5a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runners/runnable.py` & `dlt-0.3.5a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runners/stdout.py` & `dlt-0.3.5a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runners/synth_pickle.py` & `dlt-0.3.5a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runners/venv.py` & `dlt-0.3.5a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/collector.py` & `dlt-0.3.5a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/exec_info.py` & `dlt-0.3.5a0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/init.py` & `dlt-0.3.5a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/logger.py` & `dlt-0.3.5a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/prometheus.py` & `dlt-0.3.5a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/segment.py` & `dlt-0.3.5a0/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/sentry.py` & `dlt-0.3.5a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/signals.py` & `dlt-0.3.5a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/slack.py` & `dlt-0.3.5a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/runtime/telemetry.py` & `dlt-0.3.5a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/schema/detections.py` & `dlt-0.3.5a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/schema/exceptions.py` & `dlt-0.3.5a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/schema/schema.py` & `dlt-0.3.5a0/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/schema/typing.py` & `dlt-0.3.5a0/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/schema/utils.py` & `dlt-0.3.5a0/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/source.py` & `dlt-0.3.5a0/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/__init__.py` & `dlt-0.3.5a0/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/configuration.py` & `dlt-0.3.5a0/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/data_item_storage.py` & `dlt-0.3.5a0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/exceptions.py` & `dlt-0.3.5a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/file_storage.py` & `dlt-0.3.5a0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/live_schema_storage.py` & `dlt-0.3.5a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/load_storage.py` & `dlt-0.3.5a0/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/normalize_storage.py` & `dlt-0.3.5a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/schema_storage.py` & `dlt-0.3.5a0/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/transactional_file.py` & `dlt-0.3.5a0/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/storages/versioned_storage.py` & `dlt-0.3.5a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/time.py` & `dlt-0.3.5a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/typing.py` & `dlt-0.3.5a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/utils.py` & `dlt-0.3.5a0/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/validation.py` & `dlt-0.3.5a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/common/wei.py` & `dlt-0.3.5a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/bigquery/__init__.py` & `dlt-0.3.5a0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/bigquery/bigquery.py` & `dlt-0.3.5a0/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/bigquery/configuration.py` & `dlt-0.3.5a0/dlt/destinations/bigquery/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/bigquery/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/duckdb/__init__.py` & `dlt-0.3.5a0/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/duckdb/configuration.py` & `dlt-0.3.5a0/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/duckdb/duck.py` & `dlt-0.3.5a0/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/duckdb/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/dummy/__init__.py` & `dlt-0.3.5a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/dummy/configuration.py` & `dlt-0.3.5a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/dummy/dummy.py` & `dlt-0.3.5a0/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/exceptions.py` & `dlt-0.3.5a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/filesystem/__init__.py` & `dlt-0.3.5a0/dlt/destinations/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/filesystem/configuration.py` & `dlt-0.3.5a0/dlt/destinations/filesystem/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/filesystem/filesystem.py` & `dlt-0.3.5a0/dlt/destinations/filesystem/filesystem.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/filesystem/filesystem_client.py` & `dlt-0.3.5a0/dlt/destinations/filesystem/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/insert_job_client.py` & `dlt-0.3.5a0/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/job_client_impl.py` & `dlt-0.3.5a0/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/job_impl.py` & `dlt-0.3.5a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/motherduck/__init__.py` & `dlt-0.3.5a0/dlt/destinations/motherduck/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/motherduck/configuration.py` & `dlt-0.3.5a0/dlt/destinations/motherduck/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/motherduck/motherduck.py` & `dlt-0.3.5a0/dlt/destinations/motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/motherduck/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/motherduck/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/postgres/__init__.py` & `dlt-0.3.5a0/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/postgres/configuration.py` & `dlt-0.3.5a0/dlt/destinations/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/postgres/postgres.py` & `dlt-0.3.5a0/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/postgres/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/redshift/README.md` & `dlt-0.3.5a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/redshift/__init__.py` & `dlt-0.3.5a0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/redshift/configuration.py` & `dlt-0.3.5a0/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/redshift/redshift.py` & `dlt-0.3.5a0/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/snowflake/__init__.py` & `dlt-0.3.5a0/dlt/destinations/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/snowflake/configuration.py` & `dlt-0.3.5a0/dlt/destinations/snowflake/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/snowflake/snowflake.py` & `dlt-0.3.5a0/dlt/destinations/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/snowflake/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/snowflake/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/sql_client.py` & `dlt-0.3.5a0/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/sql_merge_job.py` & `dlt-0.3.5a0/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/destinations/typing.py` & `dlt-0.3.5a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/extract/decorators.py` & `dlt-0.3.5a0/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/extract/exceptions.py` & `dlt-0.3.5a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/extract/extract.py` & `dlt-0.3.5a0/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/extract/incremental.py` & `dlt-0.3.5a0/dlt/extract/incremental.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,16 +71,17 @@
     >>> info = p.run(r, destination="duckdb")
 
     Args:
         cursor_path: The name or a JSON path to an cursor field. Uses the same names of fields as in your JSON document, before they are normalized to store in the database.
         initial_value: Optional value used for `last_value` when no state is available, e.g. on the first run of the pipeline. If not provided `last_value` will be `None` on the first run.
         last_value_func: Callable used to determine which cursor value to save in state. It is called with a list of the stored state value and all cursor vals from currently processing items. Default is `max`
         primary_key: Optional primary key used to deduplicate data. If not provided, a primary key defined by the resource will be used. Pass a tuple to define a compound key. Pass empty tuple to disable unique checks
-        end_value: Optional value used to load a limited range of records between `initial_value` and `end_value`. The resource generator is stopped when this value is reached.
+        end_value: Optional value used to load a limited range of records between `initial_value` and `end_value`.
             Use in conjunction with `initial_value`, e.g. load records from given month `incremental(initial_value="2022-01-01T00:00:00Z", end_value="2022-02-01T00:00:00Z")`
+            Note, when this is set the incremental filtering is stateless and `initial_value` always supersedes any previous incremental value in state.
     """
     cursor_path: str = None
     # TODO: Support typevar here
     initial_value: Optional[Any] = None
     end_value: Optional[Any] = None
 
     def __init__(
@@ -102,14 +103,19 @@
         """Value of last_value at the beginning of current pipeline run"""
         self.resource_name: Optional[str] = None
         self.primary_key: Optional[TTableHintTemplate[TColumnKey]] = primary_key
         self._cached_state: IncrementalColumnState = None
         """State dictionary cached on first access"""
         super().__init__(self.transform)
 
+        self.end_out_of_range: bool = False
+        """Becomes true on the first item that is out of range of `end_value`. I.e. when using `max` function this means a value that is equal or higher"""
+        self.start_out_of_range: bool = False
+        """Becomes true on the first item that is out of range of `initial_value`. I.e. when using `max` this is a value that is lower than `initial_value`"""
+
     @classmethod
     def from_existing_state(cls, resource_name: str, cursor_path: str) -> "Incremental[TCursorValue]":
         """Create Incremental instance from existing state."""
         state = Incremental._get_state(resource_name, cursor_path)
         i = cls(cursor_path, state["initial_value"])
         i.resource_name = resource_name
         return i
@@ -217,56 +223,62 @@
     def transform(self, row: TDataItem) -> bool:
         if row is None:
             return True
 
         row_values = find_values(self.cursor_path_p, row)
         if not row_values:
             raise IncrementalCursorPathMissing(self.resource_name, self.cursor_path, row)
-
-        incremental_state = self._cached_state
-        last_value = incremental_state['last_value']
-
         row_value = row_values[0]
 
         # For datetime cursor, ensure the value is a timezone aware datetime.
         # The object saved in state will always be a tz aware pendulum datetime so this ensures values are comparable
         if isinstance(row_value, datetime):
             row_value = pendulum.instance(row_value)
 
+        incremental_state = self._cached_state
+        last_value = incremental_state['last_value']
+        last_value_func = self.last_value_func
+
         # Check whether end_value has been reached
+        # Filter end value ranges exclusively, so in case of "max" function we remove values >= end_value
         if self.end_value is not None and (
-            row_value == self.end_value or self.last_value_func((row_value, self.end_value)) != self.end_value
+            last_value_func((row_value, self.end_value)) != self.end_value or last_value_func((row_value, )) == self.end_value
         ):
-            raise StopIteration()
+            self.end_out_of_range = True
+            return False
 
         check_values = (row_value,) + ((last_value, ) if last_value is not None else ())
-        new_value = self.last_value_func(check_values)
+        new_value = last_value_func(check_values)
         if last_value == new_value:
+            processed_row_value = last_value_func((row_value, ))
             # we store row id for all records with the current "last_value" in state and use it to deduplicate
-            if self.last_value_func((row_value, )) == last_value:
+            if processed_row_value == last_value:
                 unique_value = self.unique_value(row)
                 # if unique value exists then use it to deduplicate
                 if unique_value:
                     if unique_value in incremental_state['unique_hashes']:
                         return False
                     # add new hash only if the record row id is same as current last value
                     incremental_state['unique_hashes'].append(unique_value)
                 return True
             # skip the record that is not a last_value or new_value: that record was already processed
             check_values = (row_value,) + ((self.start_value,) if self.start_value is not None else ())
-            new_value = self.last_value_func(check_values)
-            if new_value == self.start_value:
+            new_value = last_value_func(check_values)
+            # Include rows == start_value but exclude "lower"
+            if new_value == self.start_value and processed_row_value != self.start_value:
+                self.start_out_of_range = True
                 return False
             else:
                 return True
-        if new_value != last_value:
+        else:
             incremental_state["last_value"] = new_value
             unique_value = self.unique_value(row)
             if unique_value:
                 incremental_state["unique_hashes"] = [unique_value]
+
         return True
 
     def bind(self, pipe: SupportsPipe) -> "Incremental[TCursorValue]":
         "Called by pipe just before evaluation"
         # bind the resource/pipe name
         if self.is_partial():
             raise IncrementalCursorPathMissing(pipe.name, None, None)
```

### Comparing `dlt-0.3.4/dlt/extract/pipe.py` & `dlt-0.3.5a0/dlt/extract/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,17 +577,14 @@
                     next_meta = next_item.meta
                     next_item = next_item.data
             except TypeError as ty_ex:
                 assert callable(step)
                 raise InvalidStepFunctionArguments(pipe_item.pipe.name, get_callable_name(step), inspect.signature(step), str(ty_ex))
             except (PipelineException, ExtractorException, DltSourceException, PipeException):
                 raise
-            except StopIteration:
-                # To avoid catching StopIteration in the general Exception handler below, we just want to stop the generator
-                raise
             except Exception as ex:
                 raise ResourceExtractionError(pipe_item.pipe.name, step, str(ex), "transform") from ex
             # create next pipe item if a value was returned. A None means that item was consumed/filtered out and should not be further processed
             if next_item is not None:
                 pipe_item = ResolvablePipeItem(next_item, pipe_item.step + 1, pipe_item.pipe, next_meta)
             else:
                 pipe_item = None
```

### Comparing `dlt-0.3.4/dlt/extract/schema.py` & `dlt-0.3.5a0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/extract/source.py` & `dlt-0.3.5a0/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/extract/typing.py` & `dlt-0.3.5a0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/extract/utils.py` & `dlt-0.3.5a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/helpers/airflow_helper.py` & `dlt-0.3.5a0/dlt/helpers/airflow_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/helpers/dbt/__init__.py` & `dlt-0.3.5a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/helpers/dbt/configuration.py` & `dlt-0.3.5a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.3.5a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/helpers/dbt/exceptions.py` & `dlt-0.3.5a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/helpers/dbt/profiles.yml` & `dlt-0.3.5a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/helpers/dbt/runner.py` & `dlt-0.3.5a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/helpers/pandas_helper.py` & `dlt-0.3.5a0/dlt/helpers/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/helpers/streamlit_helper.py` & `dlt-0.3.5a0/dlt/helpers/streamlit_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/load/configuration.py` & `dlt-0.3.5a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/load/exceptions.py` & `dlt-0.3.5a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/load/load.py` & `dlt-0.3.5a0/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/normalize/configuration.py` & `dlt-0.3.5a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/normalize/normalize.py` & `dlt-0.3.5a0/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/__init__.py` & `dlt-0.3.5a0/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/configuration.py` & `dlt-0.3.5a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/dbt.py` & `dlt-0.3.5a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/exceptions.py` & `dlt-0.3.5a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/helpers.py` & `dlt-0.3.5a0/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/pipeline.py` & `dlt-0.3.5a0/dlt/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/progress.py` & `dlt-0.3.5a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/state_sync.py` & `dlt-0.3.5a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/trace.py` & `dlt-0.3.5a0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/pipeline/track.py` & `dlt-0.3.5a0/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/reflection/names.py` & `dlt-0.3.5a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/reflection/script_inspector.py` & `dlt-0.3.5a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/reflection/script_visitor.py` & `dlt-0.3.5a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/sources/helpers/requests/__init__.py` & `dlt-0.3.5a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/sources/helpers/requests/retry.py` & `dlt-0.3.5a0/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/sources/helpers/requests/session.py` & `dlt-0.3.5a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/sources/helpers/transform.py` & `dlt-0.3.5a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/dlt/version.py` & `dlt-0.3.5a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.4/pyproject.toml` & `dlt-0.3.5a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.3.4"
+version = "0.3.5a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `dlt-0.3.4/setup.py` & `dlt-0.3.5a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
  'snowflake': ['snowflake-connector-python[pandas]>=3.0.4,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.3.4',
+    'version': '0.3.5a0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `dlt-0.3.4/PKG-INFO` & `dlt-0.3.5a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.3.4
+Version: 0.3.5a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

