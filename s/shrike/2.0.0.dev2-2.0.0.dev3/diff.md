# Comparing `tmp/shrike-2.0.0.dev2.tar.gz` & `tmp/shrike-2.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrike-2.0.0.dev2.tar", last modified: Wed Jun 28 19:35:05 2023, max compression
+gzip compressed data, was "shrike-2.0.0.dev3.tar", last modified: Mon Jul 17 23:32:09 2023, max compression
```

## Comparing `shrike-2.0.0.dev2.tar` & `shrike-2.0.0.dev3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.690191 shrike-2.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)   252717 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-06-28 19:35:05.690191 shrike-2.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6977 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-28 19:35:05.690191 shrike-2.0.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.678191 shrike-2.0.0.dev2/shrike/
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.682191 shrike-2.0.0.dev2/shrike/_core/
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/_core/eyesoff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/_core/testing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.682191 shrike-2.0.0.dev2/shrike/build/
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.682191 shrike-2.0.0.dev2/shrike/build/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    60232 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/build/commands/prepare.py
--rw-r--r--   0 runner    (1001) docker     (122)     7756 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/build/commands/register.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.682191 shrike-2.0.0.dev2/shrike/build/core/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/build/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14964 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/build/core/command_line.py
--rw-r--r--   0 runner    (1001) docker     (122)     8463 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/build/core/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.682191 shrike-2.0.0.dev2/shrike/build/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/build/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.682191 shrike-2.0.0.dev2/shrike/compliant_logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/compliant_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/compliant_logging/argparser_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/compliant_logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    10327 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/compliant_logging/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    16169 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/compliant_logging/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    41145 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/compliant_logging/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/compliant_logging/progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/compliant_logging/stack_trace_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/compliant_logging/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.682191 shrike-2.0.0.dev2/shrike/distributed/
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/distributed/cluster_auto_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/distributed/dask.py
--rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/distributed/mpi_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/distributed/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.686191 shrike-2.0.0.dev2/shrike/pipeline/
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/argparser_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/canary_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.674191 shrike-2.0.0.dev2/shrike/pipeline/components/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.686191 shrike-2.0.0.dev2/shrike/pipeline/components/fedavg/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/components/fedavg/env.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/components/fedavg/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/components/fedavg/spec.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    35499 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/federated_learning.py
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    20048 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/module_helper_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16294 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/pipeline_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    42898 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/pipeline_helper_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/ray_actor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/telemetry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.686191 shrike-2.0.0.dev2/shrike/pipeline/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24460 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/testing/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/testing/importer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/testing/module_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/testing/pipeline_class_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7520 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/testing/pipeline_class_test_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.686191 shrike-2.0.0.dev2/shrike/pipeline/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/v1/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/v1/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    75640 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/v1/pipeline_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.690191 shrike-2.0.0.dev2/shrike/pipeline/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/v2/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/v2/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    68222 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/pipeline/v2/pipeline_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.690191 shrike-2.0.0.dev2/shrike/spark/
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-06-28 19:29:53.000000 shrike-2.0.0.dev2/shrike/spark/spark_net.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 19:35:05.682191 shrike-2.0.0.dev2/shrike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-06-28 19:35:05.000000 shrike-2.0.0.dev2/shrike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-06-28 19:35:05.000000 shrike-2.0.0.dev2/shrike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-28 19:35:05.000000 shrike-2.0.0.dev2/shrike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-06-28 19:35:05.000000 shrike-2.0.0.dev2/shrike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-28 19:35:05.000000 shrike-2.0.0.dev2/shrike.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)   252717 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6977 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/_core/eyesoff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/_core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/build/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/build/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60232 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/commands/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7756 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/commands/register.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/build/core/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14964 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/core/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8463 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/core/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/build/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/build/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike/compliant_logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10327 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/data_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16169 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41145 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/stack_trace_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/compliant_logging/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/distributed/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/cluster_auto_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/dask.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/mpi_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/distributed/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/canary_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.916048 shrike-2.0.0.dev3/shrike/pipeline/components/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    35499 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/federated_learning.py
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20048 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/module_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16294 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/pipeline_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42859 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/pipeline_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/ray_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/telemetry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/pipeline/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24460 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/components.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/importer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/module_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/pipeline_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7520 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/testing/pipeline_class_test_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.924048 shrike-2.0.0.dev3/shrike/pipeline/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v1/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v1/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75640 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v1/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/shrike/pipeline/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v2/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v2/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67952 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/pipeline/v2/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.928048 shrike-2.0.0.dev3/shrike/spark/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-07-17 23:28:04.000000 shrike-2.0.0.dev3/shrike/spark/spark_net.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 23:32:09.920048 shrike-2.0.0.dev3/shrike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-17 23:32:09.000000 shrike-2.0.0.dev3/shrike.egg-info/top_level.txt
```

### Comparing `shrike-2.0.0.dev2/LICENSE` & `shrike-2.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/NOTICE.txt` & `shrike-2.0.0.dev3/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/PKG-INFO` & `shrike-2.0.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 2.0.0.dev2
+Version: 2.0.0.dev3
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/ai-platform-ml-platform/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: incubation for Azure ML
         
         [![CodeQL](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/codeql-analysis.yml)
         [![docs](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/docs.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/docs.yml)
         [![python](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/python.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/python.yml)
         [![Component Governance](https://dev.azure.com/msdata/Vienna/_apis/build/status/aml-ds/Azure.shrike%20Component%20Governance?branchName=main)](https://dev.azure.com/msdata/Vienna/_build/latest?definitionId=16088&branchName=main)
-        [![Python versions](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/)
+        [![Python versions](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
         [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![codecov](https://codecov.io/gh/ai-platform-ml-platform/shrike/branch/main/graph/badge.svg?token=sSq0BKlfTu)](https://codecov.io/gh/ai-platform-ml-platform/shrike)
         [![PyPI - Downloads](https://img.shields.io/pypi/dm/shrike)](https://pypi.org/project/shrike/)
         [![PyPI version](https://badge.fury.io/py/shrike.svg)](https://badge.fury.io/py/shrike)
         [![license: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](LICENSE)
         
         The `shrike` library is a set of Python utilities for running experiments in the
```

### Comparing `shrike-2.0.0.dev2/README.md` & `shrike-2.0.0.dev3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Shrike: incubation for Azure ML
 
 [![CodeQL](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/codeql-analysis.yml)
 [![docs](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/docs.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/docs.yml)
 [![python](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/python.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/python.yml)
 [![Component Governance](https://dev.azure.com/msdata/Vienna/_apis/build/status/aml-ds/Azure.shrike%20Component%20Governance?branchName=main)](https://dev.azure.com/msdata/Vienna/_build/latest?definitionId=16088&branchName=main)
-[![Python versions](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/)
+[![Python versions](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/ai-platform-ml-platform/shrike/branch/main/graph/badge.svg?token=sSq0BKlfTu)](https://codecov.io/gh/ai-platform-ml-platform/shrike)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/shrike)](https://pypi.org/project/shrike/)
 [![PyPI version](https://badge.fury.io/py/shrike.svg)](https://badge.fury.io/py/shrike)
 [![license: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](LICENSE)
 
 The `shrike` library is a set of Python utilities for running experiments in the
```

### Comparing `shrike-2.0.0.dev2/setup.py` & `shrike-2.0.0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/_core/eyesoff.py` & `shrike-2.0.0.dev3/shrike/_core/eyesoff.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/_core/testing.py` & `shrike-2.0.0.dev3/shrike/_core/testing.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/_core/utils.py` & `shrike-2.0.0.dev3/shrike/_core/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/build/commands/prepare.py` & `shrike-2.0.0.dev3/shrike/build/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/build/commands/register.py` & `shrike-2.0.0.dev3/shrike/build/commands/register.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/build/core/command_line.py` & `shrike-2.0.0.dev3/shrike/build/core/command_line.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/build/core/configuration.py` & `shrike-2.0.0.dev3/shrike/build/core/configuration.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/build/utils/utils.py` & `shrike-2.0.0.dev3/shrike/build/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/compliant_logging/__init__.py` & `shrike-2.0.0.dev3/shrike/compliant_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/compliant_logging/argparser_utils.py` & `shrike-2.0.0.dev3/shrike/compliant_logging/argparser_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/compliant_logging/data_conversions.py` & `shrike-2.0.0.dev3/shrike/compliant_logging/data_conversions.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/compliant_logging/exceptions.py` & `shrike-2.0.0.dev3/shrike/compliant_logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/compliant_logging/logging.py` & `shrike-2.0.0.dev3/shrike/compliant_logging/logging.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/compliant_logging/progress.py` & `shrike-2.0.0.dev3/shrike/compliant_logging/progress.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/compliant_logging/stack_trace_extractor.py` & `shrike-2.0.0.dev3/shrike/compliant_logging/stack_trace_extractor.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/compliant_logging/system_info.py` & `shrike-2.0.0.dev3/shrike/compliant_logging/system_info.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/distributed/cluster_auto_setup.py` & `shrike-2.0.0.dev3/shrike/distributed/cluster_auto_setup.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/distributed/dask.py` & `shrike-2.0.0.dev3/shrike/distributed/dask.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/distributed/mpi_driver.py` & `shrike-2.0.0.dev3/shrike/distributed/mpi_driver.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/distributed/ray.py` & `shrike-2.0.0.dev3/shrike/distributed/ray.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/__init__.py` & `shrike-2.0.0.dev3/shrike/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/canary_helper.py` & `shrike-2.0.0.dev3/shrike/pipeline/canary_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/components/fedavg/run.py` & `shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/run.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/components/fedavg/spec.yaml` & `shrike-2.0.0.dev3/shrike/pipeline/components/fedavg/spec.yaml`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/federated_learning.py` & `shrike-2.0.0.dev3/shrike/pipeline/federated_learning.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/module_helper_base.py` & `shrike-2.0.0.dev3/shrike/pipeline/module_helper_base.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/pipeline_config.py` & `shrike-2.0.0.dev3/shrike/pipeline/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/pipeline_helper_base.py` & `shrike-2.0.0.dev3/shrike/pipeline/pipeline_helper_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -717,15 +717,14 @@
                 if "namespace" in component_manifest_entry:
                     component_entry_name = (
                         component_manifest_entry["namespace"]
                         + "://"
                         + component_manifest_entry["name"]
                     )
                     if component_entry_name == component_name:
-                        print("found")
                         return component_manifest_entry["key"] or component_name
             except ValueError:
                 pass
         raise ValueError(
             f"Could not find component matching {component_name}. Please check your spelling."
         )
```

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/ray_actor.py` & `shrike-2.0.0.dev3/shrike/pipeline/ray_actor.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/telemetry_utils.py` & `shrike-2.0.0.dev3/shrike/pipeline/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/testing/components.py` & `shrike-2.0.0.dev3/shrike/pipeline/testing/components.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/testing/importer.py` & `shrike-2.0.0.dev3/shrike/pipeline/testing/importer.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/testing/module_run_tests.py` & `shrike-2.0.0.dev3/shrike/pipeline/testing/module_run_tests.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/testing/pipeline_class_test.py` & `shrike-2.0.0.dev3/shrike/pipeline/testing/pipeline_class_test.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/testing/pipeline_class_test_v2.py` & `shrike-2.0.0.dev3/shrike/pipeline/testing/pipeline_class_test_v2.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/v1/aml_connect.py` & `shrike-2.0.0.dev3/shrike/pipeline/v1/aml_connect.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/v1/module_helper.py` & `shrike-2.0.0.dev3/shrike/pipeline/v1/module_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/v1/pipeline_helper.py` & `shrike-2.0.0.dev3/shrike/pipeline/v1/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/v2/aml_connect.py` & `shrike-2.0.0.dev3/shrike/pipeline/v2/aml_connect.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/v2/module_helper.py` & `shrike-2.0.0.dev3/shrike/pipeline/v2/module_helper.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike/pipeline/v2/pipeline_helper.py` & `shrike-2.0.0.dev3/shrike/pipeline/v2/pipeline_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,17 +515,14 @@
                 pipeline.display_name = self.config.run.display_name
             if self.config.run.regenerate_outputs:
                 pipeline.settings.force_rerun = True
             if self.config.run.continue_on_failure:
                 pipeline.settings.continue_on_step_failure = True
             ml_client = self.workspace()
 
-            # TODO: this is a temporary workaround to support data access in v2, can this on phase 2
-            pipeline.settings["_dataset_access_mode"] = "DatasetInDpv2"
-
             pipeline_job = ml_client.jobs.create_or_update(
                 job=pipeline,
                 experiment_name=self.config.run.experiment_name,
                 description=self.config.run.experiment_description,
                 tags=pipeline_tags,
                 compute=self.config.compute.default_compute_target,
                 skip_validation=self.config.run.skip_validation,
@@ -901,16 +898,16 @@
         target=None,
         driver_cores=None,
         driver_memory=None,
         executor_memory=None,
         executor_cores=None,
         number_executors=None,
         conf=None,
-        input_mode=None,
-        output_mode=None,
+        input_mode="direct",
+        output_mode="direct",
         datastore_name=None,
         **custom_runtime_arguments,
     ):
         """Applies settings for a Synapse component. Shrike will not set default runsettings except for spark_identity.
 
         Args:
             module_name (str): name of the module from the module manifest (required_modules() method)
@@ -964,16 +961,14 @@
                 new_conf = json.loads(new_conf)
             elif isinstance(new_conf, DictConfig) or isinstance(new_conf, dict):
                 new_conf = flatten(dict(new_conf), reducer="dot")
             else:
                 raise TypeError(
                     f"compute.synapse_conf of type {type(new_conf)} is not a valid json string or a single tested configuration."
                 )
-            if self.module_loader.is_local(module_name):
-                new_conf = json.dumps(new_conf)
             module_instance.conf = new_conf
 
         module_instance.compute = target
         module_instance.identity.type = "managed_identity"
 
         if "synapse_driver_memory" in self.config.compute:
             driver_memory = driver_memory or self.config.compute.synapse_driver_memory
@@ -1000,15 +995,15 @@
                 executor_cores or self.config.compute.synapse_executor_cores
             )
         if executor_cores:
             module_instance.executor_cores = executor_cores
 
         self._set_all_inputs_to(module_instance, input_mode=input_mode)
         self._set_all_outputs_to(
-            module_instance, output_mode=input_mode, datastore_name=datastore_name
+            module_instance, output_mode=output_mode, datastore_name=datastore_name
         )
 
     def _apply_parallel_runsettings(
         self,
         module_name,
         module_instance: Union[InternalParallel, Parallel],
         windows=False,
```

### Comparing `shrike-2.0.0.dev2/shrike/spark/spark_net.py` & `shrike-2.0.0.dev3/shrike/spark/spark_net.py`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike.egg-info/PKG-INFO` & `shrike-2.0.0.dev3/shrike.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: shrike
-Version: 2.0.0.dev2
+Version: 2.0.0.dev3
 Summary: Python utilities for compliant Azure machine learning
 Home-page: https://github.com/ai-platform-ml-platform/shrike
 Author: AML Data Science
 Author-email: aml-ds@microsoft.com
 License: MIT
 Description: # Shrike: incubation for Azure ML
         
         [![CodeQL](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/codeql-analysis.yml)
         [![docs](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/docs.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/docs.yml)
         [![python](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/python.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/python.yml)
         [![Component Governance](https://dev.azure.com/msdata/Vienna/_apis/build/status/aml-ds/Azure.shrike%20Component%20Governance?branchName=main)](https://dev.azure.com/msdata/Vienna/_build/latest?definitionId=16088&branchName=main)
-        [![Python versions](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/)
+        [![Python versions](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
         [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![codecov](https://codecov.io/gh/ai-platform-ml-platform/shrike/branch/main/graph/badge.svg?token=sSq0BKlfTu)](https://codecov.io/gh/ai-platform-ml-platform/shrike)
         [![PyPI - Downloads](https://img.shields.io/pypi/dm/shrike)](https://pypi.org/project/shrike/)
         [![PyPI version](https://badge.fury.io/py/shrike.svg)](https://badge.fury.io/py/shrike)
         [![license: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](LICENSE)
         
         The `shrike` library is a set of Python utilities for running experiments in the
```

### Comparing `shrike-2.0.0.dev2/shrike.egg-info/SOURCES.txt` & `shrike-2.0.0.dev3/shrike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shrike-2.0.0.dev2/shrike.egg-info/requires.txt` & `shrike-2.0.0.dev3/shrike.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 protobuf>=3.19.5
 
 [pipeline]
 azureml-pipeline-core>=1.37.0
 azure-ml-component==0.9.18
 gitpython~=3.1
 hydra-core~=1.0.3
+importlib-resources~=5.9.0
 flatten-dict~=0.4
 jsonpath_ng~=1.5
 coolname~=1.1
 omegaconf~=2.1.0
 toposort~=1.7
 azureml-dataset-runtime~=1.40
 opencensus-ext-azure==1.0.7
```

