# Comparing `tmp/infoworkssdk-3.0a3.tar.gz` & `tmp/infoworkssdk-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoworkssdk-3.0a3.tar", last modified: Thu Jun  1 10:07:50 2023, max compression
+gzip compressed data, was "infoworkssdk-3.0b0.tar", last modified: Thu Apr 13 12:48:00 2023, max compression
```

## Comparing `infoworkssdk-3.0a3.tar` & `infoworkssdk-3.0b0.tar`

### file list

```diff
@@ -1,69 +1,67 @@
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-06-01 10:07:50.603539 infoworkssdk-3.0a3/
--rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-3.0a3/LICENSE
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-06-01 10:07:50.603402 infoworkssdk-3.0a3/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     1806 2023-01-25 13:55:47.000000 infoworkssdk-3.0a3/README.md
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-06-01 10:07:50.584027 infoworkssdk-3.0a3/infoworks/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/__init__.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-06-01 10:07:50.584460 infoworkssdk-3.0a3/infoworks/core/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/core/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     3057 2023-04-11 06:44:19.000000 infoworkssdk-3.0a3/infoworks/core/iw_authentication.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1234 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/error.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-06-01 10:07:50.594815 infoworkssdk-3.0a3/infoworks/sdk/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)    89421 2023-04-08 13:06:20.000000 infoworkssdk-3.0a3/infoworks/sdk/admin_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    11222 2023-04-11 06:44:19.000000 infoworkssdk-3.0a3/infoworks/sdk/base_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-06-01 10:07:50.595287 infoworkssdk-3.0a3/infoworks/sdk/cicd/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-08 16:36:18.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/cicd_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-06-01 10:07:50.597818 infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-02-07 06:46:50.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
--rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-02-07 06:47:32.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2979 2023-05-11 08:03:43.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1929 2023-04-11 06:44:19.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1986 2023-02-07 06:52:34.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
--rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/lineage.py
--rw-r--r--   0 infoworks   (501) staff       (20)    29459 2023-05-11 08:03:43.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/utils.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-06-01 10:07:50.602090 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/
--rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)    14064 2023-05-18 09:49:52.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/cdata_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    20083 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/csv_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    13654 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/domains.py
--rw-r--r--   0 infoworks   (501) staff       (20)      185 2023-05-16 04:42:59.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/local_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/misc.py
--rw-r--r--   0 infoworks   (501) staff       (20)     7857 2023-05-16 04:42:59.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/pipeline_group.py
--rw-r--r--   0 infoworks   (501) staff       (20)    19020 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/pipelines.py
--rw-r--r--   0 infoworks   (501) staff       (20)    19988 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)    13060 2023-05-18 09:49:52.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1982 2023-05-18 09:49:52.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/update_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    14896 2023-05-18 09:49:52.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/workflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)    22704 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
--rw-r--r--   0 infoworks   (501) staff       (20)    27048 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/wrappersource.py
--rw-r--r--   0 infoworks   (501) staff       (20)    12333 2023-05-16 04:42:59.000000 infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
--rw-r--r--   0 infoworks   (501) staff       (20)     1729 2023-05-08 06:11:43.000000 infoworkssdk-3.0a3/infoworks/sdk/client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    31762 2023-04-10 04:34:31.000000 infoworkssdk-3.0a3/infoworks/sdk/domain_client.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-06-01 10:07:50.602355 infoworkssdk-3.0a3/infoworks/sdk/ejson/
--rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-3.0a3/infoworks/sdk/ejson/__init__.py
--rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-3.0a3/infoworks/sdk/generic_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    53262 2023-04-11 06:43:28.000000 infoworkssdk-3.0a3/infoworks/sdk/jobmetrics.py
--rw-r--r--   0 infoworks   (501) staff       (20)    32432 2023-04-11 04:32:34.000000 infoworkssdk-3.0a3/infoworks/sdk/jobs_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-3.0a3/infoworks/sdk/jobs_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)     2216 2023-05-08 06:08:31.000000 infoworkssdk-3.0a3/infoworks/sdk/local_configurations.py
--rw-r--r--   0 infoworks   (501) staff       (20)    49406 2023-05-14 10:55:59.000000 infoworkssdk-3.0a3/infoworks/sdk/pipeline_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)    47562 2023-04-13 12:30:16.000000 infoworkssdk-3.0a3/infoworks/sdk/pipeline_group_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/pipeline_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    41346 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/replicator_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)   177790 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/source_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/source_response.py
--rw-r--r--   0 infoworks   (501) staff       (20)    70492 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/url_builder.py
--rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/utils.py
--rw-r--r--   0 infoworks   (501) staff       (20)    65998 2023-06-01 10:05:48.000000 infoworkssdk-3.0a3/infoworks/sdk/workflow_client.py
--rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-3.0a3/infoworks/sdk/workflow_response.py
-drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-06-01 10:07:50.603179 infoworkssdk-3.0a3/infoworkssdk.egg-info/
--rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-06-01 10:07:50.000000 infoworkssdk-3.0a3/infoworkssdk.egg-info/PKG-INFO
--rw-r--r--   0 infoworks   (501) staff       (20)     2425 2023-06-01 10:07:50.000000 infoworkssdk-3.0a3/infoworkssdk.egg-info/SOURCES.txt
--rw-r--r--   0 infoworks   (501) staff       (20)        1 2023-06-01 10:07:50.000000 infoworkssdk-3.0a3/infoworkssdk.egg-info/dependency_links.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       45 2023-06-01 10:07:50.000000 infoworkssdk-3.0a3/infoworkssdk.egg-info/requires.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       10 2023-06-01 10:07:50.000000 infoworkssdk-3.0a3/infoworkssdk.egg-info/top_level.txt
--rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-06-01 10:07:50.603596 infoworkssdk-3.0a3/setup.cfg
--rw-r--r--   0 infoworks   (501) staff       (20)      908 2023-06-01 10:05:58.000000 infoworkssdk-3.0a3/setup.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.619391 infoworkssdk-3.0b0/
+-rw-r--r--   0 infoworks   (501) staff       (20)    35149 2022-12-08 16:36:18.000000 infoworkssdk-3.0b0/LICENSE
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-04-13 12:48:00.619240 infoworkssdk-3.0b0/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     1806 2023-01-25 13:55:47.000000 infoworkssdk-3.0b0/README.md
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.599722 infoworkssdk-3.0b0/infoworks/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/__init__.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.600163 infoworkssdk-3.0b0/infoworks/core/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/core/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     3057 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/core/iw_authentication.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1080 2023-01-09 10:04:48.000000 infoworkssdk-3.0b0/infoworks/error.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.610072 infoworkssdk-3.0b0/infoworks/sdk/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    89421 2023-04-08 13:06:20.000000 infoworkssdk-3.0b0/infoworks/sdk/admin_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    11222 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/base_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.610480 infoworkssdk-3.0b0/infoworks/sdk/cicd/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      544 2022-12-08 16:36:18.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/cicd_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.612923 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     5276 2023-02-07 06:46:50.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     7337 2023-02-07 06:47:32.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     2784 2023-04-12 13:53:13.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1929 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_source_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1986 2023-02-07 06:52:34.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      987 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/lineage.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    28608 2023-04-12 13:53:13.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/utils.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.617829 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/
+-rw-r--r--   0 infoworks   (501) staff       (20)        0 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    12629 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/cdata_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    18649 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/csv_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    13421 2022-12-08 16:37:10.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/domains.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      517 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/misc.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     7881 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipeline_group.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    16611 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipelines.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    18556 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/rdbms_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    10283 2023-04-11 06:44:19.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/salesforce_source.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      963 2022-12-19 09:42:17.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/update_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    12796 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/workflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    21402 2023-04-13 04:12:24.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    26631 2023-04-13 04:12:24.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrappersource.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    11434 2023-04-13 04:12:24.000000 infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1650 2023-04-04 12:20:53.000000 infoworkssdk-3.0b0/infoworks/sdk/client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    31762 2023-04-10 04:34:31.000000 infoworkssdk-3.0b0/infoworks/sdk/domain_client.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.618051 infoworkssdk-3.0b0/infoworks/sdk/ejson/
+-rw-r--r--   0 infoworks   (501) staff       (20)     4435 2022-12-08 16:36:18.000000 infoworkssdk-3.0b0/infoworks/sdk/ejson/__init__.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      547 2023-01-23 12:36:52.000000 infoworkssdk-3.0b0/infoworks/sdk/generic_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    53262 2023-04-11 06:43:28.000000 infoworkssdk-3.0b0/infoworks/sdk/jobmetrics.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    32432 2023-04-11 04:32:34.000000 infoworkssdk-3.0b0/infoworks/sdk/jobs_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      487 2023-01-10 05:44:03.000000 infoworkssdk-3.0b0/infoworks/sdk/jobs_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     1911 2023-01-27 06:24:03.000000 infoworkssdk-3.0b0/infoworks/sdk/local_configurations.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    36765 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/pipeline_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    47562 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/pipeline_group_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      593 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/pipeline_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)   176960 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/source_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      584 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/source_response.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    60128 2023-04-11 06:45:26.000000 infoworkssdk-3.0b0/infoworks/sdk/url_builder.py
+-rw-r--r--   0 infoworks   (501) staff       (20)     4479 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/utils.py
+-rw-r--r--   0 infoworks   (501) staff       (20)    65766 2023-04-13 12:30:16.000000 infoworkssdk-3.0b0/infoworks/sdk/workflow_client.py
+-rw-r--r--   0 infoworks   (501) staff       (20)      594 2022-12-08 16:35:08.000000 infoworkssdk-3.0b0/infoworks/sdk/workflow_response.py
+drwxr-xr-x   0 infoworks   (501) staff       (20)        0 2023-04-13 12:48:00.619020 infoworkssdk-3.0b0/infoworkssdk.egg-info/
+-rw-r--r--   0 infoworks   (501) staff       (20)     2441 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/PKG-INFO
+-rw-r--r--   0 infoworks   (501) staff       (20)     2325 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)        1 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/requires.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       10 2023-04-13 12:48:00.000000 infoworkssdk-3.0b0/infoworkssdk.egg-info/top_level.txt
+-rw-r--r--   0 infoworks   (501) staff       (20)       38 2023-04-13 12:48:00.619438 infoworkssdk-3.0b0/setup.cfg
+-rw-r--r--   0 infoworks   (501) staff       (20)      896 2023-04-13 12:47:53.000000 infoworkssdk-3.0b0/setup.py
```

### Comparing `infoworkssdk-3.0a3/LICENSE` & `infoworkssdk-3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/PKG-INFO` & `infoworkssdk-3.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 3.0a3
+Version: 3.0b0
 Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
 Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infoworkssdk-3.0a3/README.md` & `infoworkssdk-3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/core/iw_authentication.py` & `infoworkssdk-3.0b0/infoworks/core/iw_authentication.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/error.py` & `infoworkssdk-3.0b0/infoworks/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,13 +34,7 @@
         super(AdminError, self).__init__(self.message)
 
 
 class JobsError(Exception):
     def __init__(self, message):
         self.message = message
         super(JobsError, self).__init__(self.message)
-
-
-class GenericError(Exception):
-    def __init__(self, message):
-        self.message = message
-        super(GenericError, self).__init__(self.message)
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/admin_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/admin_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/base_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/base_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/cicd_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/cicd_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_all_configs_from_domain.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_entity_configuration_lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_pipeline_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,17 +36,14 @@
                         f.write(filename)
                         f.write("\n")
             except Exception as e:
                 self.logger.error(f"Unable to export configurations for pipeline {pipeline_id} due to {str(e)}")
                 print(f"Unable to export configurations for pipeline {pipeline_id} due to {str(e)}")
         if pipeline_grp_config is not None:
             pipeline_group_id = pipeline_grp_config["id"]
-            json_obj = {"entity_id": pipeline_group_id, "entity_type": "pipeline_group"}
-            domain_id = utils_obj.get_domain_id(self, json_obj)
-            if domain_id:
-                filename, configuration_obj = utils_obj.dump_to_file(self, "pipeline_group", domain_id, pipeline_group_id,
+            filename, configuration_obj = utils_obj.dump_to_file(self, "pipeline_group", domain_id, pipeline_group_id,
                                                                  replace_words, config_file_dump_path)
-                if filename is not None:
-                    f_pipeline_group.write(filename)
-                    f_pipeline_group.write("\n")
+            if filename is not None:
+                f_pipeline_group.write(filename)
+                f_pipeline_group.write("\n")
         f.close()
         f_pipeline_group.close()
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_source_configuration.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_source_configuration.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/lineage.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/lineage.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/download_configurations/utils.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/download_configurations/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import copy
 import os
-import traceback
-
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.url_builder import get_parent_entity_url, list_domains_url, configure_pipeline_url, \
     configure_workflow_url, \
     configure_source_url, get_environment_details, get_environment_storage_details, get_environment_compute_details, \
     get_environment_interactive_compute_details, get_source_configurations_url, get_pipeline_url, \
     get_data_connection, source_info, list_users_url, list_secrets_url, get_pipeline_group_base_url,list_pipelines_url
 from infoworks.sdk.cicd.cicd_response import CICDResponse
@@ -300,15 +298,14 @@
                                                                 cicd_client.client_config['bearer_token']))
                             parsed_response = IWUtils.ejson_deserialize(response.content)
                             if response.status_code == 200:
                                 status = "SUCCESS"
                             else:
                                 status = "FAILED"
                                 print("Get Data Connection Details failed " + json.dumps(response))
-                                cicd_client.logger.error("Get Data Connection Details failed " + json.dumps(response))
 
                             response_to_return["get_data_connection_details_response"] = CICDResponse.parse_result(
                                 status=status,
                                 entity_id=entity_id,
                                 response=parsed_response)
                             if response.status_code == 200 and len(parsed_response.get("result", [])) > 0:
                                 result = parsed_response.get("result", [])
@@ -317,26 +314,19 @@
                                                                                               result["properties"])
                                 for key in ['name', 'type', 'sub_type', 'properties']:
                                     dataconnection_obj[key] = result[key]
                                 configuration_obj["dataconnection_configurations"].append(
                                     copy.deepcopy(dataconnection_obj))
                 elif entity_type == "pipeline_group":
                     list_pipelines_under_domain_url = list_pipelines_url(cicd_client.client_config,domain_id=domain_id)
-                    cicd_client.logger.info(f"Calling the api: {list_pipelines_under_domain_url}")
                     pipeline_name_lookup={}
                     pipelines_under_domain_response = cicd_client.call_api("GET", list_pipelines_under_domain_url, IWUtils.get_default_header_for_v3(
             cicd_client.client_config[
                 'bearer_token']))
                     pipelines_under_domain_parsed_response = IWUtils.ejson_deserialize(pipelines_under_domain_response.content)
-                    if pipelines_under_domain_parsed_response.get("result","")=="":
-                        cicd_client.logger.error(f"Failed to list the pipelines under domain {domain_id}")
-                        cicd_client.logger.error(pipelines_under_domain_parsed_response)
-                        print(f"Failed to list the pipelines under domain {domain_id}")
-                        print(pipelines_under_domain_parsed_response)
-                        raise Exception(f"Failed to list the pipelines under domain {domain_id}")
                     for pipeline in pipelines_under_domain_parsed_response["result"]:
                         pipeline_name_lookup[pipeline["id"]]=pipeline["name"]
                     for index,pipeline in enumerate(configuration_obj["pipelines"]):
                         pipeline["name"]=pipeline_name_lookup.get(pipeline["pipeline_id"],None)
                     environment_id = configuration_obj["environment_id"]
                 domains_url_base = list_domains_url(cicd_client.client_config)
                 filter_condition = IWUtils.ejson_serialize({"_id": domain_id})
@@ -344,15 +334,14 @@
                     filter_condition=filter_condition)
                 response = cicd_client.call_api("GET", domains_url,
                                                 IWUtils.get_default_header_for_v3(
                                                     cicd_client.client_config['bearer_token']))
                 parsed_response = IWUtils.ejson_deserialize(response.content)
                 if response.status_code == 200:
                     status = "SUCCESS"
-                    cicd_client.logger.info("Got domain details successfully")
                 else:
                     status = "FAILED"
                     print("Get Domains Details failed " + json.dumps(response))
                 response_to_return["get_domain_details_response"] = CICDResponse.parse_result(status=status,
                                                                                               entity_id=entity_id,
                                                                                               response=parsed_response)
                 existing_domain_name = None
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/cdata_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/cdata_source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import copy
 import json
 
 import requests
 import yaml
-import configparser
+
 from infoworks.sdk.url_builder import get_source_details_url
 from infoworks.sdk.utils import IWUtils
-from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
-from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
+
 
 class CdataSource:
     def __init__(self):
         self.configuration_obj = None
         self.source_config_path = None
         self.environment_id = None
         self.storage_id = None
@@ -25,34 +24,14 @@
             json_string = file.read()
             if replace_words != "":
                 for key, value in [item.split("->") for item in replace_words.split(";")]:
                     json_string = json_string.replace(key, value)
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
         self.secrets = secrets
 
-    def update_mappings_for_configurations(self, mappings):
-        config = configparser.ConfigParser()
-        config.read_dict(mappings)
-        d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
-        for section in config.sections():
-            if section in PRE_DEFINED_MAPPINGS:
-                continue
-            print("section:", section)
-            try:
-                final = d.setval(section.split("$"), dict(config.items(section)))
-            except KeyError as e:
-                pass
-        self.configuration_obj = d.data
-        if "configuration$source_configs$data_lake_schema" in config.sections():
-            self.update_table_schema_and_database("target_schema",dict(config.items("configuration$source_configs$data_lake_schema")))
-        if "configuration$source_configs$staging_schema_name" in config.sections():
-            self.update_table_schema_and_database("stage_schema",dict(config.items("configuration$source_configs$staging_schema_name")))
-        if "configuration$source_configs$target_database_name" in config.sections():
-            self.update_table_schema_and_database("database",dict(config.items("configuration$source_configs$target_database_name")))
-
     def create_cdata_source(self, src_client_obj):
         data = self.configuration_obj["configuration"]["source_configs"]
         create_cdata_source_payload = data.copy()
         create_cdata_source_payload["data_lake_schema"]= data["data_lake_schema"] if "data_lake_schema" in data else ""
         create_cdata_source_payload["environment_id"] = self.environment_id
         create_cdata_source_payload["storage_id"] = self.storage_id
         create_cdata_source_payload["is_source_ingested"]= True
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/csv_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/csv_source.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import requests
 import yaml
 from infoworks.sdk.url_builder import get_source_details_url, list_secrets_url
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.source_response import SourceResponse
 from infoworks.sdk.local_configurations import Response
 from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
-from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
 import configparser
 
 class CSVSource:
     def __init__(self, environment_id, storage_id, source_config_path, secrets=None, replace_words=""):
         self.storage_id = storage_id
         self.environment_id = environment_id
         self.source_config_path = source_config_path
@@ -18,51 +17,25 @@
         with open(self.source_config_path, 'r') as file:
             json_string = file.read()
             if replace_words != "":
                 for key, value in [item.split("->") for item in replace_words.split(";")]:
                     json_string = json_string.replace(key, value)
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
 
-    def update_table_schema_and_database(self,type,mappings):
-        data=self.configuration_obj
-        for table in data.get("configuration",{}).get("table_configs",[]):
-            if type=="target_schema":
-                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("target_schema_name","")
-                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["target_schema_name"]=mappings.get(schema_from_config.lower())
-            elif type=="stage_schema":
-                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("staging_schema_name","")
-                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["staging_schema_name"]=mappings.get(schema_from_config.lower())
-            elif type=="database":
-                database_from_config=table.get("configuration",{}).get("configuration",{}).get("target_database_name","")
-                if database_from_config!="" and database_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["target_database_name"]=mappings.get(database_from_config.lower())
-            else:
-                pass
-
     def update_mappings_for_configurations(self, mappings):
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
         for section in config.sections():
-            if section in PRE_DEFINED_MAPPINGS:
+            if section in ["environment_mappings","storage_mappings","compute_mappings","table_group_compute_mappings","api_mappings","azure_keyvault","aws_secrets"]:
                 continue
             print("section:", section)
-            try:
-                final = d.setval(section.split("$"), dict(config.items(section)))
-            except KeyError as e:
-                pass
+            final = d.setval(section.split("$"), dict(config.items(section)))
+            print(f"section replacement:{d.getval(section.split('$'))}")
         self.configuration_obj = d.data
-        if "configuration$source_configs$data_lake_schema" in config.sections():
-            self.update_table_schema_and_database("target_schema",dict(config.items("configuration$source_configs$data_lake_schema")))
-        if "configuration$source_configs$staging_schema_name" in config.sections():
-            self.update_table_schema_and_database("stage_schema",dict(config.items("configuration$source_configs$staging_schema_name")))
-        if "configuration$source_configs$target_database_name" in config.sections():
-            self.update_table_schema_and_database("database",dict(config.items("configuration$source_configs$target_database_name")))
 
     def get_secret_id_from_name(self,cicd_client,secret_name):
         secret_id = None
         get_secret_details_url = list_secrets_url(cicd_client.client_config)+'?filter={"name":"'+secret_name+'"}'
         response = cicd_client.call_api("GET", get_secret_details_url,
                                         IWUtils.get_default_header_for_v3(cicd_client.client_config['bearer_token']))
         parsed_response = IWUtils.ejson_deserialize(response.content)
@@ -224,27 +197,34 @@
 
     def import_source_configuration(self, src_client_obj, source_id,
                                     mappings, export_configuration_file=None, export_config_lookup=True,
                                     read_passwords_from_secrets=False,dont_skip_step=True):
         if not dont_skip_step:
             return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
         src_name = self.configuration_obj["configuration"]["source_configs"]["name"]
+        table_group_compute_mappings = mappings.get("table_group_compute_mappings", {})
         source_import_payload = {"configuration": self.configuration_obj["configuration"]}
         modified_table_configs = self.configuration_obj["configuration"]["table_configs"]
         index = 0
         for table_config in self.configuration_obj["configuration"]["table_configs"]:
             modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
             if not table_config["configuration"].get("meta_crawl_performed", False):
                 modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
                 index = index + 1
             else:
                 if not table_config["configuration"]["meta_crawl_performed"]:
                     modified_table_configs[index]["configuration"]["meta_crawl_performed"] = True
                 index = index + 1
         source_import_payload["configuration"]["table_configs"] = modified_table_configs
+        iw_mappings = source_import_payload["configuration"]["iw_mappings"]
+        for item in iw_mappings:
+            if item.get("entity_type", "") == "environment_compute_template":
+                item["recommendation"]["compute_name"] = table_group_compute_mappings.get(
+                    item["recommendation"]["compute_name"], item["recommendation"]["compute_name"])
+        source_import_payload["configuration"]["iw_mappings"] = iw_mappings
         if export_config_lookup and (export_configuration_file is not None or read_passwords_from_secrets):
             for table in source_import_payload.get("configuration")["table_configs"]:
                 # Check if there are any export configurations and passwords to replace
                 if table.get("configuration", {}).get("export_configuration", None) is not None:
                     export_configs = table.get("configuration", {}).get("export_configuration")
                     target_type = export_configs.get("target_type", "").upper()
                     table_name = table["configuration"]["name"].upper()
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/domains.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 
 from infoworks.sdk import url_builder
 from infoworks.sdk.url_builder import list_domains_url, list_users_url, add_user_to_domain_url, \
     add_sources_to_domain_url
 from infoworks.sdk.utils import IWUtils
 from infoworks.core.iw_authentication import get_bearer_token
-from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
+
 
 class Domain:
     def __init__(self, environment_id):
         self.environment_id = environment_id
 
     def create(self, client, domain_name):
         new_domain_id = ''
@@ -21,18 +21,16 @@
         try:
             create_domain_url = url_builder.create_domain_url(client.client_config)
             response = client.call_api("POST", create_domain_url,
                                        IWUtils.get_default_header_for_v3(client.client_config['bearer_token']),
                                        domain_json_object)
             parsed_response = IWUtils.ejson_deserialize(
                 response.content)
-            if response.status_code!=200:
+            if response.status_code != 200:
                 client.logger.info('Cant create domain')
-                client.logger.info(parsed_response.get("message",""))
-                client.logger.info(parsed_response.get("details", ""))
                 client.logger.info('Getting the existing domain_id with given name.')
                 domains_url_base = list_domains_url(client.client_config)
                 filter_condition = str({"name": domain_name})
                 domains_url = domains_url_base + f"?filter={{filter_condition}}".format(
                     filter_condition=filter_condition)
                 response = client.call_api("GET", domains_url, headers={
                     'Authorization': 'Bearer ' + client.client_config["bearer_token"],
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/misc.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/misc.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/pipeline_group.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipeline_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import configparser
 import requests
 import yaml
 from infoworks.core.iw_authentication import get_bearer_token
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.url_builder import get_pipeline_group_base_url,list_domains_url,list_pipelines_url
 from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
-from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
 
 class PipelineGroup:
     def __init__(self, pipeline_group_config_path, environment_id, storage_id, interactive_id,
                  replace_words="", secrets=None):
         self.storage_id = storage_id
         self.interactive_id = interactive_id
         self.environment_id = environment_id
@@ -25,15 +24,15 @@
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
 
     def update_mappings_for_configurations(self, mappings):
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
         for section in config.sections():
-            if section in PRE_DEFINED_MAPPINGS:
+            if section in ["environment_mappings","storage_mappings","compute_mappings","table_group_compute_mappings","api_mappings","azure_keyvault","aws_secrets"]:
                 continue
             print("section:", section)
             try:
                 final = d.setval(section.split("$"), dict(config.items(section)))
                 print(f"section replacement:{d.getval(section.split('$'))}")
             except KeyError as e:
                 pass
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/pipelines.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/pipelines.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import yaml
 from infoworks.core.iw_authentication import get_bearer_token
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.url_builder import list_sources_url, list_domains_url, create_pipeline_url, create_data_connection, \
     configure_pipeline_url
 from infoworks.sdk.cicd.upload_configurations.domains import Domain
 from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
-from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
 
 class Pipeline:
     def __init__(self, pipeline_config_path, environment_id, storage_id, interactive_id,
                  replace_words="", secrets=None):
         self.storage_id = storage_id
         self.interactive_id = interactive_id
         self.environment_id = environment_id
@@ -26,58 +25,23 @@
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
 
     def update_mappings_for_configurations(self, mappings):
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
         for section in config.sections():
-            if section in PRE_DEFINED_MAPPINGS:
+            if section in ["environment_mappings","storage_mappings","compute_mappings","table_group_compute_mappings","api_mappings","azure_keyvault","aws_secrets"]:
                 continue
+            print("section:", section)
             try:
                 final = d.setval(section.split("$"), dict(config.items(section)))
+                print(f"section replacement:{d.getval(section.split('$'))}")
             except KeyError as e:
                 pass
         self.configuration_obj = d.data
-        #handle domain name mappings
-        iw_mappings = self.configuration_obj.get("configuration", {}).get("iw_mappings", [])
-        try:
-            if "domain_name_mappings" in config.sections():
-                domain_mappings = dict(config.items("domain_name_mappings"))
-                if domain_mappings != {}:
-                    for mapping in iw_mappings:
-                        domain_name=mapping.get("recommendation",{}).get("domain_name","")
-                        if domain_name!="" and domain_mappings!={}:
-                            mapping["recommendation"]["domain_name"]=domain_mappings.get(domain_name.lower(),domain_name)
-                    self.configuration_obj["configuration"]["iw_mappings"] = iw_mappings
-        except Exception as e:
-            print("Failed while doing the domain mappings")
-            print(str(e))
-            print(traceback.format_exc())
-        # handle any other generic name mappings like iw_mappings$recommendation$source_name
-        try:
-            generic_mappings = [i for i in config.sections() if i.lower().startswith("iw_mappings$")]
-            for mapping in generic_mappings:
-                lineage_list = mapping.split("$")
-                lineage_list.remove("iw_mappings")
-                if "recommendation" in lineage_list:
-                    lineage_list.remove("recommendation")
-                artifact_type = lineage_list[0]
-                artifact_mappings = dict(config.items(f"iw_mappings$recommendation${artifact_type}"))
-                if artifact_mappings != {}:
-                    for mapping in iw_mappings:
-                        artifact_name = mapping.get("recommendation", {}).get(artifact_type, "")
-                        if artifact_name != "" and artifact_mappings != {}:
-                            mapping["recommendation"][artifact_type] = artifact_mappings.get(
-                                artifact_name.lower(),
-                                artifact_name)
-                    self.configuration_obj["configuration"]["iw_mappings"] = iw_mappings
-        except Exception as e:
-            print("Failed while doing the generic mappings")
-            print(str(e))
-            print(traceback.format_exc())
 
     def create(self, pipeline_client_obj, domain_id, domain_name):
         pipeline_name = self.configuration_obj["configuration"]["entity"]["entity_name"]
         sources_in_pipelines = []
         for item in self.configuration_obj["configuration"]["iw_mappings"]:
             if item["entity_type"] == "table" and "source_name" in item["recommendation"]:
                 sources_in_pipelines.append(item["recommendation"].get("source_name"))
@@ -264,22 +228,20 @@
                     headers = IWUtils.get_default_header_for_v3(pipeline_client_obj.client_config['bearer_token'])
                     response = requests.post(create_data_connection_url, headers=headers, data=data, verify=False)
                 response = IWUtils.ejson_deserialize(response.content)
                 pipeline_client_obj.logger.info(response)
                 print(response)
 
         import_configs = {
-            "run_pipeline_metadata_build": True,
+            "run_pipeline_metadata_build": False,
             "is_pipeline_version_active": True,
             "import_data_connection": True,
             "include_optional_properties": True
         }
         url_for_importing_pipeline = configure_pipeline_url(pipeline_client_obj.client_config, domain_id, pipeline_id)
-        pipeline_client_obj.logger.info(f"URL to configure pipeline: {url_for_importing_pipeline}")
-        print(f"URL to configure pipeline: {url_for_importing_pipeline}")
         del self.configuration_obj["environment_configurations"]
         del self.configuration_obj["user_email"]
         json_string = IWUtils.ejson_serialize(
             {"configuration": self.configuration_obj["configuration"], "import_configs": import_configs})
 
         response = requests.post(url_for_importing_pipeline, data=json_string,
                                  headers={
@@ -291,14 +253,9 @@
                 pipeline_client_obj.client_config["ip"], pipeline_client_obj.client_config["port"],
                 pipeline_client_obj.client_config["refresh_token"])
             headers = IWUtils.get_default_header_for_v3(pipeline_client_obj.client_config['bearer_token'])
             response = requests.post(url_for_importing_pipeline, data=json_string, headers=headers, verify=False)
         response = IWUtils.ejson_deserialize(response.content)
         if response is not None:
             pipeline_client_obj.logger.info(response.get("message", "") + " Done")
-            pipeline_client_obj.logger.info(response)
             print(f'{response.get("message", "")} Done')
-            print(response)
             return "SUCCESS"
-        else:
-            print(response)
-            return "FAILED"
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/rdbms_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/rdbms_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from infoworks.sdk.url_builder import get_source_details_url,list_secrets_url
 from infoworks.sdk.utils import IWUtils
 from infoworks.sdk.source_response import SourceResponse
 from infoworks.sdk.local_configurations import Response
 import configparser
 from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
-from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
 
 class RDBMSSource:
     def __init__(self):
         self.configuration_obj = None
         self.source_config_path = None
         self.environment_id = None
         self.storage_id = None
@@ -45,51 +44,25 @@
                 secret_id = result[0]["id"]
                 cicd_client.logger.info("Found secret id {} ".format(secret_id))
                 return secret_id
             else:
                 cicd_client.logger.info("Secret id is {} ".format(None))
                 return None
 
-    def update_table_schema_and_database(self,type,mappings):
-        data=self.configuration_obj
-        for table in data.get("configuration",{}).get("table_configs",[]):
-            if type=="target_schema":
-                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("target_schema_name","")
-                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["target_schema_name"]=mappings.get(schema_from_config.lower())
-            elif type=="stage_schema":
-                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("staging_schema_name","")
-                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["staging_schema_name"]=mappings.get(schema_from_config.lower())
-            elif type=="database":
-                database_from_config=table.get("configuration",{}).get("configuration",{}).get("target_database_name","")
-                if database_from_config!="" and database_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["target_database_name"]=mappings.get(database_from_config.lower())
-            else:
-                pass
-
     def update_mappings_for_configurations(self, mappings):
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
         for section in config.sections():
-            if section in PRE_DEFINED_MAPPINGS:
+            if section in ["environment_mappings","storage_mappings","compute_mappings","table_group_compute_mappings","api_mappings","azure_keyvault","aws_secrets"]:
                 continue
             print("section:", section)
-            try:
-                final = d.setval(section.split("$"), dict(config.items(section)))
-            except KeyError as e:
-                pass
+            final = d.setval(section.split("$"), dict(config.items(section)))
+            print(f"section replacement:{d.getval(section.split('$'))}")
         self.configuration_obj = d.data
-        if "configuration$source_configs$data_lake_schema" in config.sections():
-            self.update_table_schema_and_database("target_schema",dict(config.items("configuration$source_configs$data_lake_schema")))
-        if "configuration$source_configs$staging_schema_name" in config.sections():
-            self.update_table_schema_and_database("stage_schema",dict(config.items("configuration$source_configs$staging_schema_name")))
-        if "configuration$source_configs$target_database_name" in config.sections():
-            self.update_table_schema_and_database("database",dict(config.items("configuration$source_configs$target_database_name")))
 
     def create_rdbms_source(self, src_client_obj):
         data = self.configuration_obj["configuration"]["source_configs"]
         create_rdbms_source_payload = {
             "name": data["name"],
             "type": "rdbms",
             "sub_type": data["sub_type"],
@@ -241,16 +214,23 @@
     def configure_tables_and_tablegroups(self, src_client_obj, source_id, export_configuration_file=None,
                                          export_config_lookup=True, mappings=None, read_passwords_from_secrets=False,
                                          env_tag="", secret_type="",dont_skip_step=True):
         if not dont_skip_step:
             return SourceResponse.parse_result(status="SKIPPED", source_id=source_id)
         if mappings is None:
             mappings = {}
+        iw_mappings = self.configuration_obj["configuration"]["iw_mappings"]
+        table_group_compute_mappings = mappings.get("table_group_compute_mappings", {})
         source_configs = self.configuration_obj["configuration"]["source_configs"]
         src_name = str(source_configs["name"])
+        for item in iw_mappings:
+            if item.get("entity_type", "") == "environment_compute_template":
+                item["recommendation"]["compute_name"] = table_group_compute_mappings.get(
+                    item["recommendation"]["compute_name"], item["recommendation"]["compute_name"])
+        self.configuration_obj["configuration"]["iw_mappings"] = iw_mappings
         # Update the service account json file mappings if any
         if export_config_lookup and (export_configuration_file is not None or read_passwords_from_secrets):
             for table in self.configuration_obj["configuration"]["table_configs"]:
                 # Check if there are any export configurations and passwords to replace
                 if table.get("configuration", {}).get("export_configuration", None) is not None:
                     export_configs = table.get("configuration", {}).get("export_configuration")
                     target_type = export_configs.get("target_type", "").upper()
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/salesforce_source.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/salesforce_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import json
 
 import requests
 import yaml
 
 from infoworks.sdk.url_builder import get_source_details_url
 from infoworks.sdk.utils import IWUtils
-import configparser
-from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
-from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
+
 
 class SalesforceSource:
     def __init__(self):
         self.configuration_obj = None
         self.source_config_path = None
         self.environment_id = None
         self.storage_id = None
@@ -25,52 +23,14 @@
             json_string = file.read()
             if replace_words != "":
                 for key, value in [item.split("->") for item in replace_words.split(";")]:
                     json_string = json_string.replace(key, value)
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
         self.secrets = secrets
 
-    def update_table_schema_and_database(self,type,mappings):
-        data=self.configuration_obj
-        for table in data.get("configuration",{}).get("table_configs",[]):
-            if type=="target_schema":
-                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("target_schema_name","")
-                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["target_schema_name"]=mappings.get(schema_from_config.lower())
-            elif type=="stage_schema":
-                schema_from_config=table.get("configuration",{}).get("configuration",{}).get("staging_schema_name","")
-                if schema_from_config!="" and schema_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["staging_schema_name"]=mappings.get(schema_from_config.lower())
-            elif type=="database":
-                database_from_config=table.get("configuration",{}).get("configuration",{}).get("target_database_name","")
-                if database_from_config!="" and database_from_config.lower() in mappings.keys():
-                    table["configuration"]["configuration"]["target_database_name"]=mappings.get(database_from_config.lower())
-            else:
-                pass
-
-    def update_mappings_for_configurations(self, mappings):
-        config = configparser.ConfigParser()
-        config.read_dict(mappings)
-        d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
-        for section in config.sections():
-            if section in PRE_DEFINED_MAPPINGS:
-                continue
-            print("section:", section)
-            try:
-                final = d.setval(section.split("$"), dict(config.items(section)))
-            except KeyError as e:
-                pass
-        self.configuration_obj = d.data
-        if "configuration$source_configs$data_lake_schema" in config.sections():
-            self.update_table_schema_and_database("target_schema",dict(config.items("configuration$source_configs$data_lake_schema")))
-        if "configuration$source_configs$staging_schema_name" in config.sections():
-            self.update_table_schema_and_database("stage_schema",dict(config.items("configuration$source_configs$staging_schema_name")))
-        if "configuration$source_configs$target_database_name" in config.sections():
-            self.update_table_schema_and_database("database",dict(config.items("configuration$source_configs$target_database_name")))
-
     def create_salesforce_source(self, src_client_obj):
         data = self.configuration_obj["configuration"]["source_configs"]
         create_salesforce_source_payload = {
             "name": data["name"],
             "type": "crm",
             "sub_type": data["sub_type"],
             "data_lake_path": data["data_lake_path"],
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/workflow.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/workflow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import traceback
-
 from infoworks.sdk.url_builder import list_sources_url, create_workflow_url, list_domains_url, configure_workflow_url
 from infoworks.sdk.utils import IWUtils
 import sys
 import configparser
 import requests
 from infoworks.sdk.cicd.upload_configurations.domains import Domain
 from infoworks.core.iw_authentication import get_bearer_token
 from infoworks.sdk.cicd.upload_configurations.update_configurations import InfoworksDynamicAccessNestedDict
-from infoworks.sdk.cicd.upload_configurations.local_configurations import PRE_DEFINED_MAPPINGS
 
 class Workflow:
     def __init__(self, workflow_configuration_path, replace_words=""):
         with open(workflow_configuration_path, 'r') as file:
             json_string = file.read()
             if replace_words != "":
                 for key, value in [item.split("->") for item in replace_words.split(";")]:
@@ -20,56 +17,23 @@
         self.configuration_obj = IWUtils.ejson_deserialize(json_string)
 
     def update_mappings_for_configurations(self, mappings):
         config = configparser.ConfigParser()
         config.read_dict(mappings)
         d = InfoworksDynamicAccessNestedDict(self.configuration_obj)
         for section in config.sections():
-            if section in PRE_DEFINED_MAPPINGS:
+            if section in ["environment_mappings","storage_mappings","compute_mappings","table_group_compute_mappings","api_mappings","azure_keyvault","aws_secrets"]:
                 continue
+            print("section:", section)
             try:
                 final = d.setval(section.split("$"), dict(config.items(section)))
+                print(f"section replacement:{d.getval(section.split('$'))}")
             except KeyError as e:
                 pass
         self.configuration_obj = d.data
-        iw_mappings = self.configuration_obj.get("configuration", {}).get("iw_mappings", [])
-        try:
-            if "domain_name_mappings" in config.sections():
-                domain_mappings = dict(config.items("domain_name_mappings"))
-                if domain_mappings!={}:
-                    for mapping in iw_mappings:
-                        domain_name = mapping.get("recommendation", {}).get("domain_name", "")
-                        if domain_name != "" and domain_mappings != {}:
-                            mapping["recommendation"]["domain_name"] = domain_mappings.get(domain_name.lower(), domain_name)
-                    self.configuration_obj["configuration"]["iw_mappings"]=iw_mappings
-        except Exception as e:
-            print("Failed while doing the domain mappings")
-            print(str(e))
-            print(traceback.format_exc())
-        # handle any other generic name mappings like iw_mappings$recommendation$source_name
-        try:
-            generic_mappings = [i for i in config.sections() if i.lower().startswith("iw_mappings$")]
-            for mapping in generic_mappings:
-                lineage_list = mapping.split("$")
-                lineage_list.remove("iw_mappings")
-                if "recommendation" in lineage_list:
-                    lineage_list.remove("recommendation")
-                artifact_type = lineage_list[0]
-                artifact_mappings = dict(config.items(f"iw_mappings$recommendation${artifact_type}"))
-                if artifact_mappings != {}:
-                    for mapping in iw_mappings:
-                        artifact_name = mapping.get("recommendation", {}).get(artifact_type, "")
-                        if artifact_name != "" and artifact_mappings != {}:
-                            mapping["recommendation"][artifact_type] = artifact_mappings.get(artifact_name.lower(),
-                                                                                             artifact_name)
-                    self.configuration_obj["configuration"]["iw_mappings"] = iw_mappings
-        except Exception as e:
-            print("Failed while doing the generic mappings")
-            print(str(e))
-            print(traceback.format_exc())
 
     def create(self, wf_client_obj, domain_id, domain_name):
         sources_in_wfs = []
         workflow_name = self.configuration_obj["configuration"]["entity"]["entity_name"]
         for item in self.configuration_obj["configuration"]["iw_mappings"]:
             if item["entity_type"] == "table_group" and "source_name" in item["recommendation"]:
                 sources_in_wfs.append(item["recommendation"].get("source_name"))
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperpipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,18 +127,14 @@
         :param override_configuration_file: Path of the file with override keys for dataconnection properties
         :param replace_words: Pass the strings to be replaced in the configuration file. Example: DEV->PROD;dev->prod
         :param read_passwords_from_secrets: True/False. If True all the pipeline related passwords are read from encrypted file name passed
         """
         try:
             if domain_id is None and domain_name is None:
                 domain_name = Path(configuration_file_path).name.split("#")[0]
-                domain_mappings = self.mappings.get("domain_name_mappings", {})
-                if domain_mappings != {}:
-                    if domain_name.lower() in domain_mappings.keys():
-                        domain_name = domain_mappings.get(domain_name.lower(), domain_name)
             env_id = self.client_config.get("default_environment_id", None)
             storage_id = self.client_config.get("default_storage_id", None)
             compute_id = self.client_config.get("default_compute_id", None)
             with open(configuration_file_path, 'r') as file:
                 json_string = file.read()
             configuration_obj = IWUtils.ejson_deserialize(json_string)
             environment_configurations = configuration_obj["environment_configurations"]
@@ -170,15 +166,14 @@
                                                                              params={"filter": {"name": compute_name}})
                         if len(result["result"]["response"]) != 0:
                             compute_id = result["result"]["response"][0]["id"]
             if env_id is None:
                 print("No env id and no mapping found")
                 raise Exception("No env id and no mapping found")
             pl_obj = Pipeline(configuration_file_path, env_id, storage_id, compute_id, replace_words, self.secrets_config)
-            pl_obj.configuration_obj = configuration_obj
             pl_obj.update_mappings_for_configurations(self.mappings)
             pipeline_id, domain_id = pl_obj.create(self, domain_id, domain_name)
             if pipeline_id is not None:
                 status = pl_obj.configure(self, pipeline_id, domain_id, override_configuration_file, self.mappings, read_passwords_from_secrets,env_tag=env_tag, secret_type=secret_type)
         except Exception as e:
             self.logger.error(str(e))
             print(str(e))
@@ -197,18 +192,14 @@
         :param override_configuration_file: Path of the file with override keys for dataconnection properties
         :param replace_words: Pass the strings to be replaced in the configuration file. Example: DEV->PROD;dev->prod
         :param read_passwords_from_secrets: True/False. If True all the pipeline related passwords are read from encrypted file name passed
         """
         try:
             if domain_id is None and domain_name is None:
                 domain_name = Path(configuration_file_path).name.split("#")[0]
-                domain_mappings = self.mappings.get("domain_name_mappings", {})
-                if domain_mappings != {}:
-                    if domain_name.lower() in domain_mappings.keys():
-                        domain_name = domain_mappings.get(domain_name.lower(), domain_name)
             env_id = self.client_config.get("default_environment_id", None)
             storage_id = self.client_config.get("default_storage_id", None)
             compute_id = self.client_config.get("default_compute_id", None)
             with open(configuration_file_path, 'r') as file:
                 json_string = file.read()
             configuration_obj = IWUtils.ejson_deserialize(json_string)
             environment_configurations = configuration_obj["environment_configurations"]
@@ -240,15 +231,14 @@
                                                                              params={"filter": {"name": compute_name}})
                         if len(result["result"]["response"]) != 0:
                             compute_id = result["result"]["response"][0]["id"]
             if env_id is None:
                 print("No env id and no mapping found")
                 raise Exception("No env id and no mapping found")
             pl_grp_obj = PipelineGroup(configuration_file_path, env_id, storage_id, compute_id, replace_words, self.secrets_config)
-            pl_grp_obj.configuration_obj = configuration_obj
             pl_grp_obj.update_mappings_for_configurations(self.mappings)
             pipeline_group_id, domain_id = pl_grp_obj.create(self, domain_id, domain_name)
         except Exception as e:
             self.logger.error(str(e))
             print(str(e))
             self.logger.error(traceback.format_exc())
             print(traceback.format_exc())
@@ -299,18 +289,14 @@
                 path = pipeline_gexf_lineage_file
             graph = nx.read_gexf(path)
             for item in self._topological_sort_grouping(graph):
                 for i in item:
                     if i != "root":
                         pipeline_file = graph._node[i]['filename'].strip()
                         domain_name = pipeline_file.split("#")[0]
-                        domain_mappings = self.mappings.get("domain_name_mappings", {})
-                        if domain_mappings != {}:
-                            if domain_name.lower() in domain_mappings.keys():
-                                domain_name = domain_mappings.get(domain_name.lower(), domain_name)
                         pipeline_args = {"entity_type": "pipeline",
                                          "pipeline_config_path": os.path.join(configurations_base_path, "pipeline",
                                                                               pipeline_file.strip()),
                                          "domain_name": domain_name, "replace_words": pl_replace_words,
                                          "override_configuration_file": override_configuration_file, "read_passwords_from_secrets": read_passwords_from_secrets}
                         job_queue.put(pipeline_args)
                 print('*** Main thread waiting to complete all pending pipeline creation/configuration requests ***')
@@ -318,18 +304,14 @@
                 print('*** Done with All Tasks ***')
         else:
             with open(os.path.join(configurations_base_path, "modified_files", "pipeline.csv"),
                       "r") as pipeline_files_fp:
                 for pipeline_file in pipeline_files_fp.readlines():
                     pl_name = pipeline_file.strip()
                     domain_name = pl_name.split("#")[0]
-                    domain_mappings = self.mappings.get("domain_name_mappings", {})
-                    if domain_mappings != {}:
-                        if domain_name.lower() in domain_mappings.keys():
-                            domain_name = domain_mappings.get(domain_name.lower(), domain_name)
                     pipeline_args = {"entity_type": "pipeline",
                                      "pipeline_config_path": os.path.join(configurations_base_path, "pipeline",
                                                                           pipeline_file.strip()),
                                      "domain_name": domain_name, "replace_words": pl_replace_words,
                                      "override_configuration_file": override_configuration_file}
                     job_queue.put(pipeline_args)
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/wrappersource.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrappersource.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,18 +124,16 @@
                         mapping["recommendation"]["compute_name"]=compute_mappings_from_config.get(mapping["recommendation"]["compute_name"],mapping["recommendation"]["compute_name"])
             if env_id is None or storage_id is None:
                 print("No env id or storage id found")
                 raise Exception("No env id or storage id found")
 
             source_type = configuration_obj["configuration"]["source_configs"]["type"]
             source_sub_type = configuration_obj["configuration"]["source_configs"]["sub_type"]
-            if source_type == "file" and (source_sub_type == "structured" or source_sub_type == "fixedwidth"):
+            if source_type == "file" and source_sub_type == "structured":
                 source_obj = CSVSource(env_id, storage_id, configuration_file_path, self.secrets_config, replace_words)
-                # adding below line to prevent missing out mappings done above (compute_mappings,environment_mappings etc
-                source_obj.configuration_obj=configuration_obj
                 source_obj.update_mappings_for_configurations(self.mappings)
                 create_source_response = source_obj.create_csv_source(self)
                 source_id=create_source_response["result"]["source_id"]
                 if source_id is not None:
                     # Proceed to configure the source connection details
                     source_connection_configurations_response = source_obj.configure_csv_source(self, source_id, self.mappings,
                                                     read_passwords_from_secrets=read_passwords_from_secrets,
@@ -172,15 +170,14 @@
                     self.logger.error("Failed to create source")
                     raise Exception("Failed to create source")
                 response_to_return["create_source_response"] = create_source_response
             elif source_type == "rdbms" and source_sub_type!="snowflake":
                 source_obj = RDBMSSource()
                 source_obj.set_variables(env_id, storage_id, configuration_file_path, self.secrets_config,
                                          replace_words)
-                source_obj.configuration_obj = configuration_obj
                 source_obj.update_mappings_for_configurations(self.mappings)
                 source_creation_response = source_obj.create_rdbms_source(self)
                 source_id = source_creation_response["result"]["source_id"]
                 if source_id is not None:
                     # Proceed to configure the source connection details
                     source_connection_configurations_response = source_obj.configure_rdbms_source_connection(self, source_id, override_configuration_file,
                                                                     read_passwords_from_secrets=read_passwords_from_secrets,
@@ -241,15 +238,14 @@
                     print(source_creation_response)
                     self.logger.error(source_creation_response)
                     raise Exception("Failed to create source")
             elif source_type == "crm" and source_sub_type == "salesforce":
                 source_obj = SalesforceSource()
                 source_obj.set_variables(env_id, storage_id, configuration_file_path, self.secrets_config,
                                          replace_words)
-                source_obj.configuration_obj = configuration_obj
                 source_obj.update_mappings_for_configurations(self.mappings)
                 source_id = source_obj.create_salesforce_source(self)
                 if source_id is not None:
                     # Proceed to configure the source connection details
                     if source_obj.configure_salesforce_source_connection(self, source_id, override_configuration_file,
                                                                     read_passwords_from_secrets=read_passwords_from_secrets,
                                                                     env_tag=env_tag,
@@ -273,18 +269,17 @@
                             print("Failed to launch source test connection")
                             raise Exception("Failed to launch source test connection")
                 else:
                     self.logger.error("Failed to create source")
                     raise Exception("Failed to create source")
             else:    #assumes to be cdata source
                 source_obj = CdataSource()
+                source_obj.update_mappings_for_configurations(self.mappings)
                 source_obj.set_variables(env_id, storage_id, configuration_file_path, self.secrets_config,
                                          replace_words)
-                source_obj.update_mappings_for_configurations(self.mappings)
-                source_obj.configuration_obj = configuration_obj
                 source_id = source_obj.create_cdata_source(self)
                 if source_id is not None:
                     # Proceed to configure the source connection details
                     if source_obj.configure_cdata_source_connection(self, source_id, override_configuration_file,
                                                                     read_passwords_from_secrets=read_passwords_from_secrets,
                                                                     env_tag=env_tag,
                                                                     secret_type=secret_type) == "SUCCESS":
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py` & `infoworkssdk-3.0b0/infoworks/sdk/cicd/upload_configurations/wrapperworkflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -126,18 +126,14 @@
         :param domain_id: Domain id to which the pipeline belongs to.
         :param domain_name: Domain name to which the pipeline belongs to
         :param replace_words: Pass the strings to be replaced in the configuration file. Example: DEV->PROD;dev->prod
         """
         try:
             if domain_id is None and domain_name is None:
                 domain_name = Path(configuration_file_path).name.split("#")[0]
-                domain_mappings = self.mappings.get("domain_name_mappings", {})
-                if domain_mappings != {}:
-                    if domain_name.lower() in domain_mappings.keys():
-                        domain_name = domain_mappings.get(domain_name.lower(),domain_name)
             wf_obj = Workflow(configuration_file_path, replace_words)
             wf_obj.update_mappings_for_configurations(self.mappings)
             wf_id, domain_id = wf_obj.create(self, domain_id, domain_name)
             if wf_id is not None:
                 status = wf_obj.configure(self, wf_id, domain_id)
         except Exception as e:
             self.logger.error(str(e))
@@ -178,34 +174,26 @@
                 path = workflow_gexf_lineage_file
             graph = nx.read_gexf(path)
             for item in self._topological_sort_grouping(graph):
                 for i in item:
                     if i != "root":
                         wf_name = graph._node[i]['filename'].strip()
                         domain_name = wf_name.split("#")[0]
-                        domain_mappings = self.mappings.get("domain_name_mappings", {})
-                        if domain_mappings != {}:
-                            if domain_name.lower() in domain_mappings.keys():
-                                domain_name = domain_mappings.get(domain_name.lower(), domain_name)
                         wf_args = {"entity_type": "workflow",
                                    "workflow_config_path": os.path.join("configurations/workflow", wf_name),
                                    "domain_name": domain_name}
                         job_queue.put(wf_args)
                 print('*** Main thread waiting to complete all pending pipeline creation/configuration requests ***')
                 job_queue.join()
                 print('*** Done with All Tasks ***')
         else:
             with open(os.path.join("configurations/modified_files", "workflow.csv"), "r") as workflow_file_fp:
                 for workflow_file in workflow_file_fp.readlines():
                     wf_name = workflow_file.strip()
                     domain_name = wf_name.split("#")[0]
-                    domain_mappings = self.mappings.get("domain_name_mappings", {})
-                    if domain_mappings != {}:
-                        if domain_name.lower() in domain_mappings.keys():
-                            domain_name = domain_mappings.get(domain_name.lower(), domain_name)
                     wf_args = {"entity_type": "workflow",
                                "workflow_config_path": os.path.join("configurations/workflow", wf_name),
                                "domain_name": domain_name, "replace_words": wf_replace_words, }
                     job_queue.put(wf_args)
 
             print('*** Main thread waiting to complete all workflow configuration requests ***')
             job_queue.join()
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/client.py` & `infoworkssdk-3.0b0/infoworks/sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from infoworks.sdk.pipeline_client import PipelineClient
 from infoworks.sdk.workflow_client import WorkflowClient
 from infoworks.sdk.domain_client import DomainClient
 from infoworks.sdk.jobmetrics import JobMetricsClient
 from infoworks.sdk.admin_client import AdminClient
 from infoworks.sdk.jobs_client import JobsClient
 from infoworks.sdk.pipeline_group_client import PipelineGroupClient
-from infoworks.sdk.replicator_client import ReplicatorClient
 
 
 class InfoworksClientSDK(SourceClient, PipelineClient, WorkflowClient, DomainClient, AdminClient, JobMetricsClient,
                          DownloadSource, DownloadPipeline, DownloadWorkflow, DownloadEntityWithLineage,
                          DownloadAllEntitiesFromDomain, WrapperSource, WrapperPipeline, WrapperWorkflow, JobsClient,
-                         PipelineGroupClient, ReplicatorClient):
+                         PipelineGroupClient):
     def __init__(self):
         super().__init__()
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/domain_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/domain_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/ejson/__init__.py` & `infoworkssdk-3.0b0/infoworks/sdk/ejson/__init__.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/generic_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/generic_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/jobmetrics.py` & `infoworkssdk-3.0b0/infoworks/sdk/jobmetrics.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/jobs_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/jobs_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/pipeline_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/pipeline_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import time
 
 from infoworks.error import PipelineError
 from infoworks.sdk import url_builder, local_configurations
 from infoworks.sdk.base_client import BaseClient
-from infoworks.sdk.generic_response import GenericResponse
 from infoworks.sdk.local_configurations import Response, ErrorCode
 from infoworks.sdk.pipeline_response import PipelineResponse
 from infoworks.sdk.utils import IWUtils
 
 
 class PipelineClient(BaseClient):
     def __init__(self):
@@ -640,218 +639,7 @@
                                                      error_code=ErrorCode.USER_ERROR,
                                                      response=response)
         except Exception as e:
             self.logger.error(
                 f"Failed to get pipeline lineage for pipeline {pipeline_id} and column {column_name} " + str(e))
             raise PipelineError(
                 f"Failed to get pipeline lineage for pipeline {pipeline_id} and column {column_name} " + str(e))
-
-    def create_pipeline_version(self, domain_id, pipeline_id, body=None):
-        """
-        Create a new Pipeline Version
-        :param body: a JSON object containing pipeline version
-        :type body: JSON Object
-        :param domain_id: Entity identifier of domain
-        :param pipeline_id: Entity identifier of pipeline_id
-        :return: response dict
-        """
-        try:
-            response = IWUtils.ejson_deserialize(self.call_api("POST", url_builder.pipeline_version_base_url(
-                self.client_config, domain_id, pipeline_id), IWUtils.get_default_header_for_v3(
-                self.client_config['bearer_token']),
-                                                               body).content)
-            result = response.get('result', {})
-            pipeline_version_id = result.get('id', None)
-            if pipeline_version_id is None:
-                self.logger.error('Pipeline version failed to create.')
-                return PipelineResponse.parse_result(status=Response.Status.FAILED,
-                                                     error_code=ErrorCode.USER_ERROR,
-                                                     error_desc='Pipeline version failed to create.',
-                                                     response=response)
-
-            pipeline_version_id = str(pipeline_version_id)
-            self.logger.info(
-                'Pipeline version {id} has been created under domain {domain_id}.'.format(id=pipeline_version_id,
-                                                                                          domain_id=domain_id))
-            return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=pipeline_version_id,
-                                                response=response)
-
-        except Exception as e:
-            self.logger.error('Response from server: ' + str(e))
-            self.logger.exception('Error occurred while trying to create a new pipeline version.')
-            raise PipelineError('Error occurred while trying to create a new pipeline version.')
-
-    def update_pipeline_version(self, domain_id, pipeline_id, pipeline_version_id, body=None):
-        """
-        Updates the Pipeline Version
-        :param body: a JSON object containing pipeline version
-        :type body: JSON Object
-        :param domain_id: Entity identifier of domain
-        :param pipeline_id: Entity identifier of pipeline_id
-        :param pipeline_version_id: Entity identifier of pipeline_version_id
-        :return: response dict
-        """
-        try:
-            response = IWUtils.ejson_deserialize(self.call_api("PATCH", url_builder.pipeline_version_base_url(
-                self.client_config, domain_id, pipeline_id) + f"/{pipeline_version_id}",
-                                                               IWUtils.get_default_header_for_v3(
-                                                                   self.client_config['bearer_token']), body).content)
-            message = response.get('message', "")
-            if message != "Pipeline Version Updated Successfully":
-                self.logger.error('Pipeline version failed to update.')
-                return PipelineResponse.parse_result(status=Response.Status.FAILED,
-                                                     error_code=ErrorCode.USER_ERROR,
-                                                     error_desc='Pipeline version failed to update.',
-                                                     response=response)
-
-            else:
-                self.logger.info(
-                    'Pipeline version {id} has been updated.'.format(id=pipeline_version_id))
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=pipeline_version_id,
-                                                    response=response)
-
-        except Exception as e:
-            self.logger.error('Response from server: ' + str(e))
-            self.logger.exception('Error occurred while trying to update a pipeline version.')
-            raise PipelineError('Error occurred while trying to update a pipeline version.')
-
-    def set_pipeline_version_as_active(self, domain_id, pipeline_id, pipeline_version_id):
-        """
-        Sets the pipeline version as active
-        :param domain_id: Entity identifier of domain
-        :param pipeline_id: Entity identifier of pipeline_id
-        :param pipeline_version_id: Entity identifier of pipeline_version_id
-        :return: response dict
-        """
-        try:
-            response = IWUtils.ejson_deserialize(self.call_api("POST", url_builder.pipeline_version_base_url(
-                self.client_config, domain_id, pipeline_id) + f"/{pipeline_version_id}/set-active",
-                                                               IWUtils.get_default_header_for_v3(
-                                                                   self.client_config['bearer_token'])).content)
-            message = response.get('message', "")
-            if message != "Successfully set active version":
-                self.logger.error('Pipeline version failed to be set active.')
-                return PipelineResponse.parse_result(status=Response.Status.FAILED,
-                                                     error_code=ErrorCode.USER_ERROR,
-                                                     error_desc='Pipeline version failed to be set active.',
-                                                     response=response)
-
-            else:
-                self.logger.info(
-                    'Pipeline version {id} has been set as active.'.format(id=pipeline_version_id))
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=pipeline_version_id,
-                                                    response=response)
-
-        except Exception as e:
-            self.logger.error('Response from server: ' + str(e))
-            self.logger.exception('Error occurred while trying to set a pipeline version as active.')
-            raise PipelineError('Error occurred while trying to set a pipeline version as active.')
-
-    def modify_advanced_config_for_pipeline(self, domain_id, pipeline_id, adv_config_body,
-                                            action_type="update", key=None):
-        """
-        Function to add/update the adv config for the pipeline
-        :param pipeline_id: id of the pipeline
-        :type pipeline_id: String
-        :param domain_id: Domain id to which the pipeline belongs to
-        :type domain_id: String
-        :param action_type: values can be either create/update. default update
-        :type action_type: String
-        :param adv_config_body: JSON dict
-        adv_config_body_example = {
-            "key" : "",
-            "value": "",
-            "description": "",
-            "is_active": True
-            }
-        :param key: In case of update, name of the adv config to update
-        :return: response dict
-        """
-        if None in {pipeline_id, domain_id} or adv_config_body is None:
-            raise Exception(f"pipeline_id, domain_id and adv_config_body cannot be None")
-        try:
-            if action_type.lower() == "create":
-                request_type = "POST"
-                request_url = url_builder.advanced_config_pipeline_url(self.client_config, domain_id,
-                                                                       pipeline_id)
-            else:
-                request_type = "PUT"
-                request_url = url_builder.advanced_config_pipeline_url(self.client_config, domain_id,
-                                                                       pipeline_id) + f"{key}"
-            response = IWUtils.ejson_deserialize(
-                self.call_api(request_type, request_url,
-                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
-                              adv_config_body).content)
-            result = response.get('result', {})
-            message = response.get('message', "")
-            adv_config_id = result.get('id', None)
-            if adv_config_id is not None:
-                adv_config_id = str(adv_config_id)
-                self.logger.info(
-                    'Advanced Config has been created {id}.'.format(id=adv_config_id))
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, entity_id=adv_config_id,
-                                                    response=response)
-            elif message == "Successfully updated Advance configuration":
-                self.logger.info('Advanced Config has been updated')
-                return GenericResponse.parse_result(status=Response.Status.SUCCESS, response=response)
-            else:
-                self.logger.error(f'Failed to {action_type} advanced config for pipeline.')
-                return GenericResponse.parse_result(status=Response.Status.FAILED,
-                                                    error_code=ErrorCode.USER_ERROR,
-                                                    error_desc=f'Failed to {action_type} advanced config for pipeline',
-                                                    response=response)
-
-        except Exception as e:
-            self.logger.error('Response from server: ' + str(e))
-            self.logger.exception('Error occurred while trying to add/update adv config pipeline.')
-            raise PipelineError('Error occurred while trying to add/update adv config pipeline.')
-
-    def list_pipeline_versions(self, domain_id=None, pipeline_id=None, params=None):
-        """
-        Function to list the pipeline versions
-        :param domain_id: Entity identified for domain
-        :type domain_id: String
-        :param pipeline_id: Entity identified for pipeline
-        :param params: Pass the parameters like limit, filter, offset, sort_by, order_by as a dictionary
-        :type: JSON dict
-        :return: response list
-        """
-        if None in {domain_id, pipeline_id}:
-            self.logger.error("domain_id and pipeline_id cannot be None")
-            raise Exception("omain_id and pipeline_id cannot be None")
-        if params is None:
-            params = {"limit": 20, "offset": 0}
-        url_to_list_pipeline_versions = url_builder.pipeline_version_base_url(self.client_config, domain_id, pipeline_id) \
-                                + IWUtils.get_query_params_string_from_dict(params=params)
-
-        pipelines_list = []
-        try:
-            response = IWUtils.ejson_deserialize(
-                self.call_api("GET", url_to_list_pipeline_versions,
-                              IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
-            if response is not None:
-                result = response.get("result", [])
-                initial_msg = response.get("message", "")
-                while len(result) > 0:
-                    pipelines_list.extend(result)
-                    nextUrl = '{protocol}://{ip}:{port}{next}'.format(next=response.get('links')['next'],
-                                                                      ip=self.client_config['ip'],
-                                                                      port=self.client_config['port'],
-                                                                      protocol=self.client_config['protocol'],
-                                                                      )
-                    response = IWUtils.ejson_deserialize(
-                        self.call_api("GET", nextUrl, IWUtils.get_default_header_for_v3(
-                            self.client_config['bearer_token'])).content)
-                    result = response.get("result", None)
-                    if result is None:
-                        return PipelineResponse.parse_result(status=Response.Status.FAILED,
-                                                             error_code=ErrorCode.GENERIC_ERROR,
-                                                             error_desc="Error in listing pipeline version",
-                                                             response=response
-                                                             )
-
-                response["result"] = pipelines_list
-                response["message"] = initial_msg
-            return PipelineResponse.parse_result(status=Response.Status.SUCCESS, response=response)
-        except Exception as e:
-            self.logger.error("Error in listing pipeline version")
-            raise PipelineError("Error in listing pipeline version" + str(e))
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/pipeline_group_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/pipeline_group_client.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/pipeline_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/pipeline_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/source_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/source_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         """
         if None in {source_id}:
             self.logger.error("source id cannot be None")
             raise Exception("source id cannot be None")
         try:
             url_for_browse_source = url_builder.browse_source_tables_url(self.client_config, source_id)
             if filter_tables_properties is not None:
-                filter_condition = f"?is_filter_enabled=true&tables_filter={filter_tables_properties.get('tables_filter','')}&catalogs_filter={filter_tables_properties.get('catalogs_filter','')}&schemas_filter={filter_tables_properties.get('schemas_filter','')}"
+                filter_condition = f"?is_filter_enabled=true&tables_filter={filter_tables_properties['tables_filter']}&catalogs_filter={filter_tables_properties['catalogs_filter']}&schemas_filter={filter_tables_properties['schemas_filter']}"
                 url_for_browse_source = url_for_browse_source + filter_condition
             response = IWUtils.ejson_deserialize(
                 self.call_api("GET", url_for_browse_source,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token'])).content)
             result = response.get('result', {})
             if result.get("message","")=="Interactive Cluster is not running. Please bring up cluster and retry":
                 return SourceResponse.parse_result(status=Response.Status.FAILED,
@@ -1637,33 +1637,22 @@
             return None
         if src_type.lower() == "oracle":
             sub_type = SourceMappings.oracle.get("sub_type")
             driver_name = SourceMappings.oracle.get("driver_name")
             driver_version = SourceMappings.oracle.get("driver_version")
             database = SourceMappings.oracle.get("database")
         elif src_type.lower() == "sqlserver":
-            sub_type = SourceMappings.sqlserver.get("sub_type")
-            driver_name = SourceMappings.sqlserver.get("driver_name")
-            driver_version = SourceMappings.sqlserver.get("driver_version")
-            database = SourceMappings.sqlserver.get("database")
+            pass
         elif src_type.lower() == "teradata":
             sub_type = SourceMappings.teradata.get("sub_type")
             driver_name = SourceMappings.teradata.get("driver_name")
             driver_version = SourceMappings.teradata.get("driver_version")
             database = SourceMappings.teradata.get("database")
         elif src_type.lower() == "mysql":
-            sub_type = SourceMappings.mysql.get("sub_type")
-            driver_name = SourceMappings.mysql.get("driver_name")
-            driver_version = SourceMappings.mysql.get("driver_version")
-            database = SourceMappings.mysql.get("database")
-        elif src_type.lower() == "netezza":
-            sub_type = SourceMappings.netezza.get("sub_type")
-            driver_name = SourceMappings.netezza.get("driver_name")
-            driver_version = SourceMappings.netezza.get("driver_version")
-            database = SourceMappings.netezza.get("database")
+            pass
         else:
             sub_type = SourceMappings.oracle.get("sub_type")
             driver_name = SourceMappings.oracle.get("driver_name")
             driver_version = SourceMappings.oracle.get("driver_version")
             database = SourceMappings.oracle.get("database")
         src_create_response = self.create_source(source_config={
             "name": src_name,
@@ -2801,15 +2790,15 @@
             if action_type.lower() == "create":
                 request_type = "POST"
                 request_url = url_builder.table_advanced_base_url(self.client_config, source_id,
                                                                   table_id)
             else:
                 request_type = "PUT"
                 request_url = url_builder.table_advanced_base_url(self.client_config, source_id,
-                                                                  table_id) + f"/{key}"
+                                                                  table_id) + f"{key}"
             response = IWUtils.ejson_deserialize(
                 self.call_api(request_type, request_url,
                               IWUtils.get_default_header_for_v3(self.client_config['bearer_token']),
                               adv_config_body).content)
             result = response.get('result', {})
             message = response.get('message', "")
             adv_config_id = result.get('id', None)
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/source_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/source_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/url_builder.py` & `infoworkssdk-3.0b0/infoworks/sdk/url_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1538,32 +1538,21 @@
     return request
 
 
 def advanced_config_domain_url(config, domain_id):
     """
     returns url to work with adv config of the domain
     """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/configurations/advance'.format(
+    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/accessible-pipeline-extensions'.format(
         domain_id=domain_id,
         ip=config['ip'], port=config['port'],
         protocol=config['protocol'])
     return request
 
 
-def advanced_config_pipeline_url(config, domain_id, pipeline_id):
-    """
-    returns url to work with adv config of the pipeline
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/pipelines/{pipeline_id}/configurations/advance'.format(
-        domain_id=domain_id, pipeline_id=pipeline_id,
-        ip=config['ip'], port=config['port'],
-        protocol=config['protocol'])
-    return request
-
-
 def table_advanced_base_url(config, source_id, table_id):
     """
     returns url to work with table level advanced configuration
     """
     request = '{protocol}://{ip}:{port}/v3/sources/{source_id}/tables/{table_id}/configurations/advance'.format(
         source_id=source_id,
         table_id=table_id,
@@ -1620,252 +1609,7 @@
     """
         returns url to get secret details in Infoworks
         """
     request = '{protocol}://{ip}:{port}/v3/admin/manage-secrets/secrets'.format(
         ip=config['ip'], port=config['port'],
         protocol=config['protocol'])
     return request
-
-
-def list_replicator_sources_url(config):
-    """
-    returns URL to list replicator sources using v3 api
-    :param config: client configurations
-    :type config: dict
-    :return: url to list sources
-    """
-    request = '{protocol}://{ip}:{port}/v3/replicator/sources'.format(ip=config['ip'], port=config['port'],
-                                                                      protocol=config['protocol'])
-    return request
-
-
-def get_replicator_source_url(config, source_id):
-    """
-    returns URL to the details of a specific replicator source using v3 api
-    :param config: client configurations
-    :type config: dict
-    :param source_id: Identifier of Source
-    :type source_id: str
-    :return: url to the details of a specific replicator source
-    """
-    request = '{protocol}://{ip}:{port}/v3/replicator/sources/{source_id}'.format(
-        ip=config['ip'], port=config['port'], protocol=config['protocol'], source_id=source_id)
-    return request
-
-
-def create_replicator_source_url(config):
-    """
-    returns URL to create a replicator source using v3 api
-    :param config: client configurations
-    :type config: dict
-    :return: url for the replicator source creation
-    """
-    request = '{protocol}://{ip}:{port}/v3/replicator/sources'.format(ip=config['ip'], port=config['port'],
-                                                                      protocol=config['protocol'])
-    return request
-
-
-def list_replicator_destinations_url(config):
-    """
-    returns URL to list replicator destinations using v3 api
-    :param config: client configurations
-    :type config: dict
-    :return: url to list destinations
-    """
-    request = '{protocol}://{ip}:{port}/v3/replicator/destinations'.format(ip=config['ip'], port=config['port'],
-                                                                           protocol=config['protocol'])
-    return request
-
-
-def get_replicator_destination_url(config, destination_id):
-    """
-    returns URL to the details of a specific replicator destination using v3 api
-    :param config: client configurations
-    :type config: dict
-    :param destination_id: Identifier of Destination
-    :type destination_id: str
-    :return: url to the details of a specific replicator destination
-    """
-    request = '{protocol}://{ip}:{port}/v3/replicator/destinations/{destination_id}'.format(
-        ip=config['ip'], port=config['port'], protocol=config['protocol'], destination_id=destination_id)
-    return request
-
-
-def create_replicator_destination_url(config):
-    """
-    returns URL to create a replicator destination using v3 api
-    :param config: client configurations
-    :type config: dict
-    :return: url for the replicator destination creation
-    """
-    request = '{protocol}://{ip}:{port}/v3/replicator/destinations'.format(ip=config['ip'], port=config['port'],
-                                                                           protocol=config['protocol'])
-    return request
-
-
-def list_replicator_definitions_url(config, domain_id):
-    """
-    returns URL to list replicator definitions using v3 api
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier of Domain
-    :type domain_id: String
-    :return: url to list definitions
-    """
-
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/definitions' \
-        .format(ip=config['ip'], port=config['port'], domain_id=domain_id,
-                protocol=config['protocol'])
-    return request
-
-
-def create_replicator_definition_url(config, domain_id):
-    """
-    returns URL to create a replicator definition using v3 api
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier for domain
-    :type domain_id: string
-    :return: url for the replicator definition creation
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/definitions'.format(ip=config['ip'],
-                                                                                   port=config['port'],
-                                                                                   protocol=config['protocol'],
-                                                                                   domain_id=domain_id)
-    return request
-
-
-def add_replicator_definition_tables_url(config, domain_id, definition_id):
-    """
-    returns URL to add tables to replicator definition using v3 api
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier for domain
-    :type domain_id: string
-    :param definition_id: Identifier for Replicator definition
-    :type definition_id: string
-    :return: url to add tables to replicator definition
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/definitions/{definition_id}/tables' \
-        .format(ip=config['ip'], port=config['port'], protocol=config['protocol'], domain_id=domain_id,
-                definition_id=definition_id)
-
-    return request
-
-
-def submit_replication_metacrawl_job_url(config, domain_id, replicator_source_id):
-    """
-    returns URL to add tables to replicator definition using v3 api
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier for domain
-    :type domain_id: string
-    :param replicator_source_id: Identifier for Source
-    :type replicator_source_id: string
-    :return: url to submit replication metacrawl job
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/replicator-sources/{replicator_source_id}/jobs' \
-        .format(ip=config['ip'], port=config['port'], protocol=config['protocol'], domain_id=domain_id,
-                replicator_source_id=replicator_source_id)
-
-    return request
-
-
-def submit_replication_data_job_url(config, domain_id, definition_id):
-    """
-    returns URL to add tables to replicator definition using v3 api
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier for domain
-    :type domain_id: string
-    :param definition_id: Identifier for Definition
-    :type definition_id: string
-    :return: url to submit replication data job
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/definitions/{definition_id}/jobs' \
-        .format(ip=config['ip'], port=config['port'], protocol=config['protocol'], domain_id=domain_id,
-                definition_id=definition_id)
-
-    return request
-
-
-def add_replicator_sources_to_domain_url(config, domain_id):
-    """
-    returns URL to add replicator sources to domains
-
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier for domain
-    :type domain_id: string
-    :return: url to add replicator sources to domains
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/accessible-replicator-sources' \
-        .format(ip=config['ip'], port=config['port'], domain_id=domain_id, protocol=config['protocol'])
-    return request
-
-
-def add_replicator_destinations_to_domain_url(config, domain_id):
-    """
-    returns URL to add replicator destinations to domains
-
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier for domain
-    :type domain_id: string
-    :return: url to add replicator destinations to domains
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/accessible-replicator-destinations' \
-        .format(ip=config['ip'], port=config['port'], domain_id=domain_id, protocol=config['protocol'])
-    return request
-
-
-def get_replication_schedules_url(config, domain_id, definition_id):
-    """
-    returns replication schedules URL
-
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier for domain
-    :type domain_id: string
-    :param definition_id : Identifier for Replicator definition
-    :type definition_id: string
-    :return: replication schedules URL
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/definitions/{definition_id}/schedules' \
-        .format(ip=config['ip'], port=config['port'], domain_id=domain_id, protocol=config['protocol'],
-                definition_id=definition_id)
-    return request
-
-
-def get_replicator_source_tables_url(config, source_id):
-    """
-    returns replicator source tables URL
-
-    :param config: client configurations
-    :type config: dict
-    :param source_id: Identifier for replicator source
-    :type source_id: string
-    :return: replicator source tables url
-    """
-    request = '{protocol}://{ip}:{port}/v3//replicator/sources/{source_id}/tables' \
-        .format(ip=config['ip'], port=config['port'], source_id=source_id, protocol=config['protocol'])
-    return request
-
-
-def pipeline_version_base_url(config, domain_id, pipeline_id):
-    """
-    returns URL to work on pipeline versions using v3 api
-    :param config: client configurations
-    :type config: dict
-    :param domain_id: Identifier for domain
-    :type domain_id: string
-    :param pipeline_id: Identifier for pipeline
-    :return: url to work on pipeline version
-    """
-    request = '{protocol}://{ip}:{port}/v3/domains/{domain_id}/pipelines/{pipeline_id}/versions'.format(ip=config['ip'],
-                                                                                                        port=config[
-                                                                                                            'port'],
-                                                                                                        protocol=config[
-                                                                                                            'protocol'],
-                                                                                                        domain_id=domain_id,
-                                                                                                        pipeline_id=pipeline_id)
-    return request
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/utils.py` & `infoworkssdk-3.0b0/infoworks/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/workflow_client.py` & `infoworkssdk-3.0b0/infoworks/sdk/workflow_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,44 +476,40 @@
             self.logger.error("workflow_id or workflow_run_id cannot be None")
             raise Exception("workflow_id or workflow_run_id cannot be None")
         try:
             response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_status_url(
                 self.client_config, workflow_id, workflow_run_id), IWUtils.get_default_header_for_v3(
                 self.client_config['bearer_token'])).content)
             result = response.get('result', {})
-            if result:
+            workflow_status = result['workflow_status']["state"]
+            while workflow_status.lower() not in ['success', 'completed', 'failed', 'aborted', 'canceled']:
+                response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_status_url(
+                    self.client_config, workflow_id, workflow_run_id), IWUtils.get_default_header_for_v3(
+                    self.client_config['bearer_token'])).content)
+                result = response.get('result', {})
                 workflow_status = result['workflow_status']["state"]
-                while workflow_status.lower() not in ['success', 'completed', 'failed', 'aborted', 'canceled']:
-                    response = IWUtils.ejson_deserialize(self.call_api("GET", url_builder.get_workflow_status_url(
-                        self.client_config, workflow_id, workflow_run_id), IWUtils.get_default_header_for_v3(
-                        self.client_config['bearer_token'])).content)
-                    result = response.get('result', {})
-                    workflow_status = result['workflow_status']["state"]
-                    if workflow_status.lower() in ['success', 'completed', 'failed', 'aborted', 'canceled']:
-                        break
-                    print(f"workflow_status : {workflow_status}.Sleeping for {poll_interval} seconds")
-                    time.sleep(poll_interval)
+                if workflow_status.lower() in ['success', 'completed', 'failed', 'aborted', 'canceled']:
+                    break
+                print(f"workflow_status : {workflow_status}.Sleeping for {poll_interval} seconds")
+                time.sleep(poll_interval)
 
-                run_id = result.get('id', None)
-                if result.get('id', None) is None:
-                    self.logger.error(f'Failed to poll status of the workflow {workflow_id}')
-                    return WorkflowResponse.parse_result(status=Response.Status.FAILED,
-                                                         error_code=ErrorCode.USER_ERROR,
-                                                         error_desc=f'Failed to poll status of the workflow {workflow_id}',
-                                                         response=response)
-
-                workflow_id = str(workflow_id)
-                self.logger.info(
-                    'Successfully polled status of the workflow {id} with run id {run_id}.'.format(id=workflow_id,
-                                                                                                   run_id=run_id))
-                return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+            run_id = result.get('id', None)
+            if result.get('id', None) is None:
+                self.logger.error(f'Failed to poll status of the workflow {workflow_id}')
+                return WorkflowResponse.parse_result(status=Response.Status.FAILED,
+                                                     error_code=ErrorCode.USER_ERROR,
+                                                     error_desc=f'Failed to poll status of the workflow {workflow_id}',
                                                      response=response)
-            else:
-                print(response)
-                raise Exception("Returned API Result is None")
+
+            workflow_id = str(workflow_id)
+            self.logger.info(
+                'Successfully polled status of the workflow {id} with run id {run_id}.'.format(id=workflow_id,
+                                                                                               run_id=run_id))
+            return WorkflowResponse.parse_result(status=Response.Status.SUCCESS, workflow_id=workflow_id,
+                                                 response=response)
 
         except Exception as e:
             self.logger.error('Response from server: ' + str(response))
             self.logger.exception('Error occurred while trying to poll status of workflow.')
             raise WorkflowError('Error occurred while trying to poll status of workflow.')
 
     def get_workflow_configuration_json_export(self, workflow_id=None, domain_id=None):
```

### Comparing `infoworkssdk-3.0a3/infoworks/sdk/workflow_response.py` & `infoworkssdk-3.0b0/infoworks/sdk/workflow_response.py`

 * *Files identical despite different names*

### Comparing `infoworkssdk-3.0a3/infoworkssdk.egg-info/PKG-INFO` & `infoworkssdk-3.0b0/infoworkssdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infoworkssdk
-Version: 3.0a3
+Version: 3.0b0
 Summary: A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0
 Home-page: https://github.com/Infoworks/InfoworksPythonSDK
 Author: Infoworks CE Team
 Author-email: abhishek.raviprasad@infoworks.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `infoworkssdk-3.0a3/infoworkssdk.egg-info/SOURCES.txt` & `infoworkssdk-3.0b0/infoworkssdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 infoworks/sdk/jobmetrics.py
 infoworks/sdk/jobs_client.py
 infoworks/sdk/jobs_response.py
 infoworks/sdk/local_configurations.py
 infoworks/sdk/pipeline_client.py
 infoworks/sdk/pipeline_group_client.py
 infoworks/sdk/pipeline_response.py
-infoworks/sdk/replicator_client.py
 infoworks/sdk/source_client.py
 infoworks/sdk/source_response.py
 infoworks/sdk/url_builder.py
 infoworks/sdk/utils.py
 infoworks/sdk/workflow_client.py
 infoworks/sdk/workflow_response.py
 infoworks/sdk/cicd/__init__.py
@@ -35,15 +34,14 @@
 infoworks/sdk/cicd/download_configurations/get_workflow_configuration.py
 infoworks/sdk/cicd/download_configurations/lineage.py
 infoworks/sdk/cicd/download_configurations/utils.py
 infoworks/sdk/cicd/upload_configurations/__init__.py
 infoworks/sdk/cicd/upload_configurations/cdata_source.py
 infoworks/sdk/cicd/upload_configurations/csv_source.py
 infoworks/sdk/cicd/upload_configurations/domains.py
-infoworks/sdk/cicd/upload_configurations/local_configurations.py
 infoworks/sdk/cicd/upload_configurations/misc.py
 infoworks/sdk/cicd/upload_configurations/pipeline_group.py
 infoworks/sdk/cicd/upload_configurations/pipelines.py
 infoworks/sdk/cicd/upload_configurations/rdbms_source.py
 infoworks/sdk/cicd/upload_configurations/salesforce_source.py
 infoworks/sdk/cicd/upload_configurations/update_configurations.py
 infoworks/sdk/cicd/upload_configurations/workflow.py
```

### Comparing `infoworkssdk-3.0a3/setup.py` & `infoworkssdk-3.0b0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="infoworkssdk",
-    version="3.0-alpha3",
+    version="3.0-beta",
     author="Infoworks CE Team",
     author_email="abhishek.raviprasad@infoworks.io",
     description="A package to work with Infoworks via SDK. This library is compatible with Infoworks v5.34 onwards. Code can be found in https://github.com/Infoworks/InfoworksPythonSDK branch: release/sdk-3.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Infoworks/InfoworksPythonSDK",
     packages=setuptools.find_packages(),
     install_requires=[
-        'requests', 'bson', 'urllib3', 'pandas', 'networkx', 'pyyaml'],
+        'requests', 'bson', 'urllib3', 'pandas', 'networkx'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

