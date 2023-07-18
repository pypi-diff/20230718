# Comparing `tmp/kfp-tekton-server-api-1.8.0rc6.tar.gz` & `tmp/kfp-tekton-server-api-1.8.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-tekton-server-api-1.8.0rc6.tar", last modified: Mon Jul 17 19:06:14 2023, max compression
+gzip compressed data, was "kfp-tekton-server-api-1.8.0rc7.tar", last modified: Tue Jul 18 18:25:33 2023, max compression
```

## Comparing `kfp-tekton-server-api-1.8.0rc6.tar` & `kfp-tekton-server-api-1.8.0rc7.tar`

### file list

```diff
@@ -1,113 +1,111 @@
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.687806 kfp-tekton-server-api-1.8.0rc6/
--rw-r--r--   0 tommyli    (501) staff       (20)    11357 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/LICENSE
--rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-17 19:06:14.688012 kfp-tekton-server-api-1.8.0rc6/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)    13066 2023-07-13 21:54:41.000000 kfp-tekton-server-api-1.8.0rc6/README.md
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.625437 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/
--rw-r--r--   0 tommyli    (501) staff       (20)     4398 2023-07-17 19:05:22.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/__init__.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.632904 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/
--rw-r--r--   0 tommyli    (501) staff       (20)      550 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    36823 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/experiment_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5448 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/healthz_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    35425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/job_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    69047 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/pipeline_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13674 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/pipeline_upload_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    59741 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/run_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    26288 2023-07-17 19:05:28.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api_client.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13322 2023-07-17 19:05:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/configuration.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3795 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/exceptions.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.654093 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/
--rw-r--r--   0 tommyli    (501) staff       (20)     3447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4658 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/googlerpc_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/inline_object.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2873 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/job_mode.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4643 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
--rw-r--r--   0 tommyli    (501) staff       (20)    10425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/protobuf_any.py
--rw-r--r--   0 tommyli    (501) staff       (20)     6709 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2896 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/run_metric_format.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4712 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_cron_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     7846 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_experiment.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2983 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_experiment_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3470 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_get_healthz_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3762 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_get_template_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)    14740 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_job.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5594 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_experiments_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5272 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_jobs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5542 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5398 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_pipelines_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_runs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3869 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_parameter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5006 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_periodic_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)    10909 2023-07-17 19:04:24.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5052 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_runtime.py
--rw-r--r--   0 tommyli    (501) staff       (20)     8397 2023-07-13 21:54:18.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_spec.py
--rw-r--r--   0 tommyli    (501) staff       (20)    10094 2023-07-17 19:04:20.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_version.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3868 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_read_artifact_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2916 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_relationship.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3597 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3989 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_key.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4894 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_reference.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3057 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_type.py
--rw-r--r--   0 tommyli    (501) staff       (20)    14091 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4126 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_detail.py
--rw-r--r--   0 tommyli    (501) staff       (20)     6333 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_metric.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2897 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4504 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4362 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_trigger.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3609 2023-07-17 19:05:04.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_url.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4806 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_value.py
--rw-r--r--   0 tommyli    (501) staff       (20)    12334 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/rest.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.627891 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/
--rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)     4343 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/SOURCES.txt
--rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/dependency_links.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       48 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/requires.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       22 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/top_level.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       69 2023-07-17 19:06:14.688735 kfp-tekton-server-api-1.8.0rc6/setup.cfg
--rw-r--r--   0 tommyli    (501) staff       (20)     1247 2023-07-17 19:05:39.000000 kfp-tekton-server-api-1.8.0rc6/setup.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.687068 kfp-tekton-server-api-1.8.0rc6/test/
--rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_experiment_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1622 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_googlerpc_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)      971 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_healthz_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1694 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_inline_object.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1339 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_job_mode.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1848 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_job_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3721 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1842 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_spec_runtime_config.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1071 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_upload_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1476 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_protobuf_any.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1915 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1837 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1429 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_run_metric_format.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2682 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_run_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1659 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_cron_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2104 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_experiment.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1530 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_experiment_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1520 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_get_healthz_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1528 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_get_template_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4344 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_job.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2563 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_experiments_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5054 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_jobs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3607 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_pipeline_versions_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4513 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_pipelines_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4306 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_runs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1440 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_parameter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1714 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_periodic_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4295 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1533 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_runtime.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2232 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_spec.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3261 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_version.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1538 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_read_artifact_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1416 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_relationship.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1934 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_report_run_metrics_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_key.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1725 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_reference.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1418 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_type.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3628 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_run.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4134 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_detail.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1524 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_metric.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1453 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1543 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_trigger.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1389 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_url.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_value.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-18 18:25:33.807936 kfp-tekton-server-api-1.8.0rc7/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11357 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/LICENSE
+-rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-18 18:25:33.808160 kfp-tekton-server-api-1.8.0rc7/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)    13102 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/README.md
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-18 18:25:33.752294 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/
+-rw-r--r--   0 tommyli    (501) staff       (20)     4338 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/__init__.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-18 18:25:33.757879 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/
+-rw-r--r--   0 tommyli    (501) staff       (20)      550 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    36823 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5448 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    35425 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    69047 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13980 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    59741 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    26288 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api_client.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13322 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/configuration.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3795 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/exceptions.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-18 18:25:33.779384 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/
+-rw-r--r--   0 tommyli    (501) staff       (20)     3387 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4658 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3481 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2873 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4643 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5979 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6709 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3178 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2896 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4712 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     7846 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2983 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3470 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3762 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14740 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5594 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5272 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5542 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5398 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5178 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3869 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5006 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    10871 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5052 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     8397 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     9786 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3868 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2916 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3597 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3989 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4894 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3057 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14091 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4126 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6333 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2897 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4362 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3567 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4806 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_value.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    12334 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/rest.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-18 18:25:33.754404 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api.egg-info/
+-rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-18 18:25:33.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api.egg-info/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)     4278 2023-07-18 18:25:33.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api.egg-info/SOURCES.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-07-18 18:25:33.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api.egg-info/dependency_links.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       48 2023-07-18 18:25:33.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api.egg-info/requires.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       22 2023-07-18 18:25:33.000000 kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api.egg-info/top_level.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       69 2023-07-18 18:25:33.809006 kfp-tekton-server-api-1.8.0rc7/setup.cfg
+-rw-r--r--   0 tommyli    (501) staff       (20)     1247 2023-07-18 18:24:13.000000 kfp-tekton-server-api-1.8.0rc7/setup.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-18 18:25:33.807350 kfp-tekton-server-api-1.8.0rc7/test/
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1622 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)      971 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1694 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1339 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1848 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3721 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1842 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1139 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1410 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1915 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1837 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1429 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2682 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1659 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2104 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1530 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1520 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1528 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4344 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2563 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5054 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2986 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3687 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4306 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1440 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1714 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3565 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1533 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2232 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2463 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1538 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1416 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1934 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1481 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1725 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1418 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3628 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4134 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1524 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1453 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1352 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1447 2023-07-18 18:19:48.000000 kfp-tekton-server-api-1.8.0rc7/test/test_v1_value.py
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/LICENSE` & `kfp-tekton-server-api-1.8.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/README.md` & `kfp-tekton-server-api-1.8.0rc7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # kfp-tekton-server-api
 This file contains REST API specification for Kubeflow Pipelines. The file is autogenerated from the swagger definition.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.8.0rc4
-- Package version: 1.8.0rc4
+- API version: 1.8.0rc7
+- Package version: 1.8.0rc7
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.google.com](https://www.google.com)
 
 ## Requirements.
 
-Python 2.7 and 3.7+
+Python 2.7 and 3.4+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
@@ -116,16 +116,16 @@
 *PipelineServiceApi* | [**pipeline_service_get_pipeline**](docs/PipelineServiceApi.md#pipeline_service_get_pipeline) | **GET** /apis/v1/pipelines/{id} | Finds a specific pipeline by ID.
 *PipelineServiceApi* | [**pipeline_service_get_pipeline_version**](docs/PipelineServiceApi.md#pipeline_service_get_pipeline_version) | **GET** /apis/v1/pipeline_versions/{versionId} | Gets a pipeline version by pipeline version ID.
 *PipelineServiceApi* | [**pipeline_service_get_pipeline_version_template**](docs/PipelineServiceApi.md#pipeline_service_get_pipeline_version_template) | **GET** /apis/v1/pipeline_versions/{versionId}/templates | Returns a YAML template that contains the specified pipeline version&#39;s description, parameters and metadata.
 *PipelineServiceApi* | [**pipeline_service_get_template**](docs/PipelineServiceApi.md#pipeline_service_get_template) | **GET** /apis/v1/pipelines/{id}/templates | Returns a single YAML template that contains the description, parameters, and metadata associated with the pipeline provided.
 *PipelineServiceApi* | [**pipeline_service_list_pipeline_versions**](docs/PipelineServiceApi.md#pipeline_service_list_pipeline_versions) | **GET** /apis/v1/pipeline_versions | Lists all pipeline versions of a given pipeline.
 *PipelineServiceApi* | [**pipeline_service_list_pipelines**](docs/PipelineServiceApi.md#pipeline_service_list_pipelines) | **GET** /apis/v1/pipelines | Finds all pipelines.
 *PipelineServiceApi* | [**pipeline_service_update_pipeline_default_version**](docs/PipelineServiceApi.md#pipeline_service_update_pipeline_default_version) | **POST** /apis/v1/pipelines/{pipelineId}/default_version/{versionId} | Update the default pipeline version of a specific pipeline.
-*PipelineUploadServiceApi* | [**upload_pipeline**](docs/PipelineUploadServiceApi.md#upload_pipeline) | **POST** /apis/v1/pipelines/upload | 
-*PipelineUploadServiceApi* | [**upload_pipeline_version**](docs/PipelineUploadServiceApi.md#upload_pipeline_version) | **POST** /apis/v1/pipelines/upload_version | 
+*PipelineUploadServiceApi* | [**pipeline_service_upload_pipeline**](docs/PipelineUploadServiceApi.md#pipeline_service_upload_pipeline) | **POST** /apis/v1/pipelines/upload | 
+*PipelineUploadServiceApi* | [**pipeline_service_upload_pipeline_version**](docs/PipelineUploadServiceApi.md#pipeline_service_upload_pipeline_version) | **POST** /apis/v1/pipelines/upload_version | 
 *RunServiceApi* | [**run_service_archive_run**](docs/RunServiceApi.md#run_service_archive_run) | **POST** /apis/v1/runs/{id}:archive | Archives a run.
 *RunServiceApi* | [**run_service_create_run**](docs/RunServiceApi.md#run_service_create_run) | **POST** /apis/v1/runs | Creates a new run.
 *RunServiceApi* | [**run_service_delete_run**](docs/RunServiceApi.md#run_service_delete_run) | **DELETE** /apis/v1/runs/{id} | Deletes a run.
 *RunServiceApi* | [**run_service_get_run**](docs/RunServiceApi.md#run_service_get_run) | **GET** /apis/v1/runs/{runId} | Finds a specific run by ID.
 *RunServiceApi* | [**run_service_list_runs**](docs/RunServiceApi.md#run_service_list_runs) | **GET** /apis/v1/runs | Finds all runs.
 *RunServiceApi* | [**run_service_read_artifact**](docs/RunServiceApi.md#run_service_read_artifact) | **GET** /apis/v1/runs/{runId}/nodes/{nodeId}/artifacts/{artifactName}:read | Finds a run&#39;s artifact data.
 *RunServiceApi* | [**run_service_report_run_metrics**](docs/RunServiceApi.md#run_service_report_run_metrics) | **POST** /apis/v1/runs/{runId}:reportMetrics | ReportRunMetrics reports metrics of a run. Each metric is reported in its own transaction, so this API accepts partial failures. Metric can be uniquely identified by (run_id, node_id, name). Duplicate reporting will be ignored by the API. First reporting wins.
@@ -167,15 +167,14 @@
  - [V1ResourceKey](docs/V1ResourceKey.md)
  - [V1ResourceReference](docs/V1ResourceReference.md)
  - [V1ResourceType](docs/V1ResourceType.md)
  - [V1Run](docs/V1Run.md)
  - [V1RunDetail](docs/V1RunDetail.md)
  - [V1RunMetric](docs/V1RunMetric.md)
  - [V1RunStorageState](docs/V1RunStorageState.md)
- - [V1Status](docs/V1Status.md)
  - [V1Trigger](docs/V1Trigger.md)
  - [V1Url](docs/V1Url.md)
  - [V1Value](docs/V1Value.md)
 
 
 ## Documentation For Authorization
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/__init__.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.8.0rc6"
+__version__ = "1.8.0rc7"
 
 # import apis into sdk package
 from kfp_tekton_server_api.api.experiment_service_api import ExperimentServiceApi
 from kfp_tekton_server_api.api.healthz_service_api import HealthzServiceApi
 from kfp_tekton_server_api.api.job_service_api import JobServiceApi
 from kfp_tekton_server_api.api.pipeline_service_api import PipelineServiceApi
 from kfp_tekton_server_api.api.pipeline_upload_service_api import PipelineUploadServiceApi
@@ -64,12 +64,11 @@
 from kfp_tekton_server_api.models.v1_resource_key import V1ResourceKey
 from kfp_tekton_server_api.models.v1_resource_reference import V1ResourceReference
 from kfp_tekton_server_api.models.v1_resource_type import V1ResourceType
 from kfp_tekton_server_api.models.v1_run import V1Run
 from kfp_tekton_server_api.models.v1_run_detail import V1RunDetail
 from kfp_tekton_server_api.models.v1_run_metric import V1RunMetric
 from kfp_tekton_server_api.models.v1_run_storage_state import V1RunStorageState
-from kfp_tekton_server_api.models.v1_status import V1Status
 from kfp_tekton_server_api.models.v1_trigger import V1Trigger
 from kfp_tekton_server_api.models.v1_url import V1Url
 from kfp_tekton_server_api.models.v1_value import V1Value
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/__init__.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/job_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/job_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/pipeline_upload_service_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,21 +32,21 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def upload_pipeline(self, uploadfile, **kwargs):  # noqa: E501
-        """upload_pipeline  # noqa: E501
+    def pipeline_service_upload_pipeline(self, uploadfile, **kwargs):  # noqa: E501
+        """pipeline_service_upload_pipeline  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.upload_pipeline(uploadfile, async_req=True)
+        >>> thread = api.pipeline_service_upload_pipeline(uploadfile, async_req=True)
         >>> result = thread.get()
 
         :param uploadfile: The pipeline to upload. Maximum size of 32MB is supported. (required)
         :type uploadfile: file
         :param name:
         :type name: str
         :param description:
@@ -62,23 +62,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1Pipeline
         """
         kwargs['_return_http_data_only'] = True
-        return self.upload_pipeline_with_http_info(uploadfile, **kwargs)  # noqa: E501
+        return self.pipeline_service_upload_pipeline_with_http_info(uploadfile, **kwargs)  # noqa: E501
 
-    def upload_pipeline_with_http_info(self, uploadfile, **kwargs):  # noqa: E501
-        """upload_pipeline  # noqa: E501
+    def pipeline_service_upload_pipeline_with_http_info(self, uploadfile, **kwargs):  # noqa: E501
+        """pipeline_service_upload_pipeline  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.upload_pipeline_with_http_info(uploadfile, async_req=True)
+        >>> thread = api.pipeline_service_upload_pipeline_with_http_info(uploadfile, async_req=True)
         >>> result = thread.get()
 
         :param uploadfile: The pipeline to upload. Maximum size of 32MB is supported. (required)
         :type uploadfile: file
         :param name:
         :type name: str
         :param description:
@@ -118,22 +118,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method upload_pipeline" % key
+                    " to method pipeline_service_upload_pipeline" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'uploadfile' is set
         if self.api_client.client_side_validation and ('uploadfile' not in local_var_params or  # noqa: E501
                                                         local_var_params['uploadfile'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `uploadfile` when calling `upload_pipeline`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `uploadfile` when calling `pipeline_service_upload_pipeline`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'name' in local_var_params and local_var_params['name'] is not None:  # noqa: E501
@@ -172,21 +172,21 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def upload_pipeline_version(self, uploadfile, **kwargs):  # noqa: E501
-        """upload_pipeline_version  # noqa: E501
+    def pipeline_service_upload_pipeline_version(self, uploadfile, **kwargs):  # noqa: E501
+        """pipeline_service_upload_pipeline_version  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.upload_pipeline_version(uploadfile, async_req=True)
+        >>> thread = api.pipeline_service_upload_pipeline_version(uploadfile, async_req=True)
         >>> result = thread.get()
 
         :param uploadfile: The pipeline to upload. Maximum size of 32MB is supported. (required)
         :type uploadfile: file
         :param name:
         :type name: str
         :param pipelineid:
@@ -204,23 +204,23 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1PipelineVersion
         """
         kwargs['_return_http_data_only'] = True
-        return self.upload_pipeline_version_with_http_info(uploadfile, **kwargs)  # noqa: E501
+        return self.pipeline_service_upload_pipeline_version_with_http_info(uploadfile, **kwargs)  # noqa: E501
 
-    def upload_pipeline_version_with_http_info(self, uploadfile, **kwargs):  # noqa: E501
-        """upload_pipeline_version  # noqa: E501
+    def pipeline_service_upload_pipeline_version_with_http_info(self, uploadfile, **kwargs):  # noqa: E501
+        """pipeline_service_upload_pipeline_version  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.upload_pipeline_version_with_http_info(uploadfile, async_req=True)
+        >>> thread = api.pipeline_service_upload_pipeline_version_with_http_info(uploadfile, async_req=True)
         >>> result = thread.get()
 
         :param uploadfile: The pipeline to upload. Maximum size of 32MB is supported. (required)
         :type uploadfile: file
         :param name:
         :type name: str
         :param pipelineid:
@@ -263,22 +263,22 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method upload_pipeline_version" % key
+                    " to method pipeline_service_upload_pipeline_version" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'uploadfile' is set
         if self.api_client.client_side_validation and ('uploadfile' not in local_var_params or  # noqa: E501
                                                         local_var_params['uploadfile'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `uploadfile` when calling `upload_pipeline_version`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `uploadfile` when calling `pipeline_service_upload_pipeline_version`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'name' in local_var_params and local_var_params['name'] is not None:  # noqa: E501
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/run_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api/run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api_client.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.8.0rc6/python'
+        self.user_agent = 'OpenAPI-Generator/1.8.0rc7/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/configuration.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,16 +347,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.8.0rc6\n"\
-               "SDK Package Version: 1.8.0rc6".\
+               "Version of the API: 1.8.0rc7\n"\
+               "SDK Package Version: 1.8.0rc7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/exceptions.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/__init__.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,11 +45,10 @@
 from kfp_tekton_server_api.models.v1_resource_key import V1ResourceKey
 from kfp_tekton_server_api.models.v1_resource_reference import V1ResourceReference
 from kfp_tekton_server_api.models.v1_resource_type import V1ResourceType
 from kfp_tekton_server_api.models.v1_run import V1Run
 from kfp_tekton_server_api.models.v1_run_detail import V1RunDetail
 from kfp_tekton_server_api.models.v1_run_metric import V1RunMetric
 from kfp_tekton_server_api.models.v1_run_storage_state import V1RunStorageState
-from kfp_tekton_server_api.models.v1_status import V1Status
 from kfp_tekton_server_api.models.v1_trigger import V1Trigger
 from kfp_tekton_server_api.models.v1_url import V1Url
 from kfp_tekton_server_api.models.v1_value import V1Value
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/googlerpc_status.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/inline_object.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/job_mode.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/job_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/run_metric_format.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_get_template_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_job.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_job.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_parameter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,23 +42,22 @@
         'error': 'str',
         'default_version': 'V1PipelineVersion',
         'resource_references': 'list[V1ResourceReference]'
     }
 
     attribute_map = {
         'id': 'id',
-        # 'created_at': 'createdAt',
+        'created_at': 'createdAt',
         'name': 'name',
         'description': 'description',
         'parameters': 'parameters',
         'url': 'url',
         'error': 'error',
         'default_version': 'defaultVersion',
-        'resource_references': 'resourceReferences',
-        'created_at': 'created_at'
+        'resource_references': 'resourceReferences'
     }
 
     def __init__(self, id=None, created_at=None, name=None, description=None, parameters=None, url=None, error=None, default_version=None, resource_references=None, local_vars_configuration=None):  # noqa: E501
         """V1Pipeline - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_pipeline_runtime.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_version.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_pipeline_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,24 +42,20 @@
         'resource_references': 'list[V1ResourceReference]',
         'description': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
-        # 'created_at': 'createdAt',
+        'created_at': 'createdAt',
         'parameters': 'parameters',
-        # 'code_source_url': 'codeSourceUrl',
-        # 'package_url': 'packageUrl',
-        # 'resource_references': 'resourceReferences',
-        'description': 'description',
-        'created_at': 'created_at',
-        'code_source_url': 'code_source_url',
-        'package_url': 'package_url',
-        'resource_references': 'resource_references'
+        'code_source_url': 'codeSourceUrl',
+        'package_url': 'packageUrl',
+        'resource_references': 'resourceReferences',
+        'description': 'description'
     }
 
     def __init__(self, id=None, name=None, created_at=None, parameters=None, code_source_url=None, package_url=None, resource_references=None, description=None, local_vars_configuration=None):  # noqa: E501
         """V1PipelineVersion - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
@@ -227,26 +223,26 @@
 
         self._package_url = package_url
 
     @property
     def resource_references(self):
         """Gets the resource_references of this V1PipelineVersion.  # noqa: E501
 
-        Input field. Specify which resource this pipeline version belongs to. For Experiment, the only valid resource reference is a single Namespace.  # noqa: E501
+        Input. Required. E.g., specify which pipeline this pipeline version belongs to.  # noqa: E501
 
         :return: The resource_references of this V1PipelineVersion.  # noqa: E501
         :rtype: list[V1ResourceReference]
         """
         return self._resource_references
 
     @resource_references.setter
     def resource_references(self, resource_references):
         """Sets the resource_references of this V1PipelineVersion.
 
-        Input field. Specify which resource this pipeline version belongs to. For Experiment, the only valid resource reference is a single Namespace.  # noqa: E501
+        Input. Required. E.g., specify which pipeline this pipeline version belongs to.  # noqa: E501
 
         :param resource_references: The resource_references of this V1PipelineVersion.  # noqa: E501
         :type resource_references: list[V1ResourceReference]
         """
 
         self._resource_references = resource_references
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_read_artifact_response.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_relationship.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_report_run_metrics_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_resource_key.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_resource_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_resource_type.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_detail.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_run_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_run_metric.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_url.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'pipeline_url': 'str'
     }
 
     attribute_map = {
-        # 'pipeline_url': 'pipelineUrl',
-        'pipeline_url': 'pipeline_url'
+        'pipeline_url': 'pipelineUrl'
     }
 
     def __init__(self, pipeline_url=None, local_vars_configuration=None):  # noqa: E501
         """V1Url - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_value.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/models/v1_value.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/rest.py` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api/rest.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/SOURCES.txt` & `kfp-tekton-server-api-1.8.0rc7/kfp_tekton_server_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 kfp_tekton_server_api/models/v1_resource_key.py
 kfp_tekton_server_api/models/v1_resource_reference.py
 kfp_tekton_server_api/models/v1_resource_type.py
 kfp_tekton_server_api/models/v1_run.py
 kfp_tekton_server_api/models/v1_run_detail.py
 kfp_tekton_server_api/models/v1_run_metric.py
 kfp_tekton_server_api/models/v1_run_storage_state.py
-kfp_tekton_server_api/models/v1_status.py
 kfp_tekton_server_api/models/v1_trigger.py
 kfp_tekton_server_api/models/v1_url.py
 kfp_tekton_server_api/models/v1_value.py
 test/test_experiment_service_api.py
 test/test_googlerpc_status.py
 test/test_healthz_service_api.py
 test/test_inline_object.py
@@ -96,11 +95,10 @@
 test/test_v1_resource_key.py
 test/test_v1_resource_reference.py
 test/test_v1_resource_type.py
 test/test_v1_run.py
 test/test_v1_run_detail.py
 test/test_v1_run_metric.py
 test/test_v1_run_storage_state.py
-test/test_v1_status.py
 test/test_v1_trigger.py
 test/test_v1_url.py
 test/test_v1_value.py
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/setup.py` & `kfp-tekton-server-api-1.8.0rc7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kfp-tekton-server-api"
-VERSION = "1.8.0rc6"
+VERSION = "1.8.0rc7"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_googlerpc_status.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_inline_object.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_job_mode.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_job_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_job_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_job_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_pipeline_spec_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_parameter.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,37 +9,45 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
+import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.api.pipeline_upload_service_api import PipelineUploadServiceApi  # noqa: E501
+from kfp_tekton_server_api.models.v1_parameter import V1Parameter  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-
-class TestPipelineUploadServiceApi(unittest.TestCase):
-    """PipelineUploadServiceApi unit test stubs"""
+class TestV1Parameter(unittest.TestCase):
+    """V1Parameter unit test stubs"""
 
     def setUp(self):
-        self.api = kfp_tekton_server_api.api.pipeline_upload_service_api.PipelineUploadServiceApi()  # noqa: E501
-
-    def tearDown(self):
         pass
 
-    def test_upload_pipeline(self):
-        """Test case for upload_pipeline
-
-        """
+    def tearDown(self):
         pass
 
-    def test_upload_pipeline_version(self):
-        """Test case for upload_pipeline_version
-
-        """
-        pass
+    def make_instance(self, include_optional):
+        """Test V1Parameter
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = kfp_tekton_server_api.models.v1_parameter.V1Parameter()  # noqa: E501
+        if include_optional :
+            return V1Parameter(
+                name = '0', 
+                value = '0'
+            )
+        else :
+            return V1Parameter(
+        )
+
+    def testV1Parameter(self):
+        """Test V1Parameter"""
+        inst_req_only = self.make_instance(include_optional=False)
+        inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_protobuf_any.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_protobuf_any.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,15 @@
         """Test ProtobufAny
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = kfp_tekton_server_api.models.protobuf_any.ProtobufAny()  # noqa: E501
         if include_optional :
             return ProtobufAny(
-                type = '0', 
-                type_url = '0', 
-                value = 'YQ=='
+                type = '0'
             )
         else :
             return ProtobufAny(
         )
 
     def testProtobufAny(self):
         """Test ProtobufAny"""
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_report_run_metrics_response_report_run_metric_result.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_report_run_metrics_response_report_run_metric_result_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_run_metric_format.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_run_service_api.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_get_template_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_job.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_job.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_pipelines_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,75 +12,77 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.models.v1_list_pipeline_versions_response import V1ListPipelineVersionsResponse  # noqa: E501
+from kfp_tekton_server_api.models.v1_list_pipelines_response import V1ListPipelinesResponse  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-class TestV1ListPipelineVersionsResponse(unittest.TestCase):
-    """V1ListPipelineVersionsResponse unit test stubs"""
+class TestV1ListPipelinesResponse(unittest.TestCase):
+    """V1ListPipelinesResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1ListPipelineVersionsResponse
+        """Test V1ListPipelinesResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_tekton_server_api.models.v1_list_pipeline_versions_response.V1ListPipelineVersionsResponse()  # noqa: E501
+        # model = kfp_tekton_server_api.models.v1_list_pipelines_response.V1ListPipelinesResponse()  # noqa: E501
         if include_optional :
-            return V1ListPipelineVersionsResponse(
-                versions = [
-                    kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
+            return V1ListPipelinesResponse(
+                pipelines = [
+                    kfp_tekton_server_api.models.v1_pipeline.v1Pipeline(
                         id = '0', 
-                        name = '0', 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        name = '0', 
+                        description = '0', 
                         parameters = [
                             kfp_tekton_server_api.models.v1_parameter.v1Parameter(
                                 name = '0', 
                                 value = '0', )
                             ], 
-                        code_source_url = '0', 
-                        package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                            pipeline_url = '0', 
-                            pipeline_url = '0', ), 
-                        resource_references = [
-                            kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                                key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
-                                    type = 'UNKNOWN_RESOURCE_TYPE', 
-                                    id = '0', ), 
-                                name = '0', 
-                                relationship = 'UNKNOWN_RELATIONSHIP', )
-                            ], 
-                        description = '0', 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        code_source_url = '0', 
-                        package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                            pipeline_url = '0', 
+                        url = kfp_tekton_server_api.models.v1_url.v1Url(
                             pipeline_url = '0', ), 
+                        error = '0', 
+                        default_version = kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
+                            id = '0', 
+                            name = '0', 
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            code_source_url = '0', 
+                            package_url = kfp_tekton_server_api.models.v1_url.v1Url(
+                                pipeline_url = '0', ), 
+                            resource_references = [
+                                kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
+                                    key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
+                                        type = 'UNKNOWN_RESOURCE_TYPE', 
+                                        id = '0', ), 
+                                    name = '0', 
+                                    relationship = 'UNKNOWN_RELATIONSHIP', )
+                                ], 
+                            description = '0', ), 
                         resource_references = [
                             kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
                                 name = '0', )
                             ], )
                     ], 
-                next_page_token = '0', 
-                total_size = 56
+                total_size = 56, 
+                next_page_token = '0'
             )
         else :
-            return V1ListPipelineVersionsResponse(
+            return V1ListPipelinesResponse(
         )
 
-    def testV1ListPipelineVersionsResponse(self):
-        """Test V1ListPipelineVersionsResponse"""
+    def testV1ListPipelinesResponse(self):
+        """Test V1ListPipelinesResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,89 +12,81 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.models.v1_list_pipelines_response import V1ListPipelinesResponse  # noqa: E501
+from kfp_tekton_server_api.models.v1_pipeline import V1Pipeline  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-class TestV1ListPipelinesResponse(unittest.TestCase):
-    """V1ListPipelinesResponse unit test stubs"""
+class TestV1Pipeline(unittest.TestCase):
+    """V1Pipeline unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1ListPipelinesResponse
+        """Test V1Pipeline
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_tekton_server_api.models.v1_list_pipelines_response.V1ListPipelinesResponse()  # noqa: E501
+        # model = kfp_tekton_server_api.models.v1_pipeline.V1Pipeline()  # noqa: E501
         if include_optional :
-            return V1ListPipelinesResponse(
-                pipelines = [
-                    kfp_tekton_server_api.models.v1_pipeline.v1Pipeline(
-                        id = '0', 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+            return V1Pipeline(
+                id = '0', 
+                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                name = '0', 
+                description = '0', 
+                parameters = [
+                    kfp_tekton_server_api.models.v1_parameter.v1Parameter(
                         name = '0', 
-                        description = '0', 
-                        parameters = [
-                            kfp_tekton_server_api.models.v1_parameter.v1Parameter(
-                                name = '0', 
-                                value = '0', )
-                            ], 
-                        url = kfp_tekton_server_api.models.v1_url.v1Url(
-                            pipeline_url = '0', 
-                            pipeline_url = '0', ), 
-                        error = '0', 
-                        default_version = kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
-                            id = '0', 
-                            name = '0', 
-                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            code_source_url = '0', 
-                            package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                                pipeline_url = '0', 
-                                pipeline_url = '0', ), 
-                            resource_references = [
-                                kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                                    key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
-                                        type = 'UNKNOWN_RESOURCE_TYPE', 
-                                        id = '0', ), 
-                                    name = '0', 
-                                    relationship = 'UNKNOWN_RELATIONSHIP', )
-                                ], 
-                            description = '0', 
-                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            code_source_url = '0', 
-                            package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                                pipeline_url = '0', 
-                                pipeline_url = '0', ), 
-                            resource_references = [
-                                kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                                    name = '0', )
-                                ], ), 
-                        resource_references = [
-                            kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                                name = '0', )
-                            ], 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                        value = '0', )
                     ], 
-                total_size = 56, 
-                next_page_token = '0'
+                url = kfp_tekton_server_api.models.v1_url.v1Url(
+                    pipeline_url = '0', ), 
+                error = '0', 
+                default_version = kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
+                    id = '0', 
+                    name = '0', 
+                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    parameters = [
+                        kfp_tekton_server_api.models.v1_parameter.v1Parameter(
+                            name = '0', 
+                            value = '0', )
+                        ], 
+                    code_source_url = '0', 
+                    package_url = kfp_tekton_server_api.models.v1_url.v1Url(
+                        pipeline_url = '0', ), 
+                    resource_references = [
+                        kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
+                            key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
+                                type = 'UNKNOWN_RESOURCE_TYPE', 
+                                id = '0', ), 
+                            name = '0', 
+                            relationship = 'UNKNOWN_RELATIONSHIP', )
+                        ], 
+                    description = '0', ), 
+                resource_references = [
+                    kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
+                        key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
+                            type = 'UNKNOWN_RESOURCE_TYPE', 
+                            id = '0', ), 
+                        name = '0', 
+                        relationship = 'UNKNOWN_RELATIONSHIP', )
+                    ]
             )
         else :
-            return V1ListPipelinesResponse(
+            return V1Pipeline(
         )
 
-    def testV1ListPipelinesResponse(self):
-        """Test V1ListPipelinesResponse"""
+    def testV1Pipeline(self):
+        """Test V1Pipeline"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_read_artifact_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,42 +12,41 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.models.v1_parameter import V1Parameter  # noqa: E501
+from kfp_tekton_server_api.models.v1_read_artifact_response import V1ReadArtifactResponse  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-class TestV1Parameter(unittest.TestCase):
-    """V1Parameter unit test stubs"""
+class TestV1ReadArtifactResponse(unittest.TestCase):
+    """V1ReadArtifactResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1Parameter
+        """Test V1ReadArtifactResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_tekton_server_api.models.v1_parameter.V1Parameter()  # noqa: E501
+        # model = kfp_tekton_server_api.models.v1_read_artifact_response.V1ReadArtifactResponse()  # noqa: E501
         if include_optional :
-            return V1Parameter(
-                name = '0', 
-                value = '0'
+            return V1ReadArtifactResponse(
+                data = 'YQ=='
             )
         else :
-            return V1Parameter(
+            return V1ReadArtifactResponse(
         )
 
-    def testV1Parameter(self):
-        """Test V1Parameter"""
+    def testV1ReadArtifactResponse(self):
+        """Test V1ReadArtifactResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_run_detail.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,93 +12,87 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.models.v1_pipeline import V1Pipeline  # noqa: E501
+from kfp_tekton_server_api.models.v1_run_detail import V1RunDetail  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-class TestV1Pipeline(unittest.TestCase):
-    """V1Pipeline unit test stubs"""
+class TestV1RunDetail(unittest.TestCase):
+    """V1RunDetail unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1Pipeline
+        """Test V1RunDetail
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_tekton_server_api.models.v1_pipeline.V1Pipeline()  # noqa: E501
+        # model = kfp_tekton_server_api.models.v1_run_detail.V1RunDetail()  # noqa: E501
         if include_optional :
-            return V1Pipeline(
-                id = '0', 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                name = '0', 
-                description = '0', 
-                parameters = [
-                    kfp_tekton_server_api.models.v1_parameter.v1Parameter(
-                        name = '0', 
-                        value = '0', )
-                    ], 
-                url = kfp_tekton_server_api.models.v1_url.v1Url(
-                    pipeline_url = '0', 
-                    pipeline_url = '0', ), 
-                error = '0', 
-                default_version = kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
+            return V1RunDetail(
+                run = kfp_tekton_server_api.models.v1_run.v1Run(
                     id = '0', 
                     name = '0', 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    parameters = [
-                        kfp_tekton_server_api.models.v1_parameter.v1Parameter(
-                            name = '0', 
-                            value = '0', )
-                        ], 
-                    code_source_url = '0', 
-                    package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                        pipeline_url = '0', 
-                        pipeline_url = '0', ), 
+                    storage_state = 'STORAGESTATE_AVAILABLE', 
+                    description = '0', 
+                    pipeline_spec = kfp_tekton_server_api.models.v1_pipeline_spec.v1PipelineSpec(
+                        pipeline_id = '0', 
+                        pipeline_name = '0', 
+                        workflow_manifest = '0', 
+                        pipeline_manifest = '0', 
+                        parameters = [
+                            kfp_tekton_server_api.models.v1_parameter.v1Parameter(
+                                name = '0', 
+                                value = '0', )
+                            ], 
+                        runtime_config = kfp_tekton_server_api.models.pipeline_spec_runtime_config.PipelineSpecRuntimeConfig(
+                            parameters = {
+                                'key' : kfp_tekton_server_api.models.v1_value.v1Value(
+                                    int_value = '0', 
+                                    double_value = 1.337, 
+                                    string_value = '0', )
+                                }, 
+                            pipeline_root = '0', ), ), 
                     resource_references = [
                         kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
                             key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
                                 type = 'UNKNOWN_RESOURCE_TYPE', 
                                 id = '0', ), 
                             name = '0', 
                             relationship = 'UNKNOWN_RELATIONSHIP', )
                         ], 
-                    description = '0', 
+                    service_account = '0', 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    code_source_url = '0', 
-                    package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                        pipeline_url = '0', 
-                        pipeline_url = '0', ), 
-                    resource_references = [
-                        kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                            name = '0', )
+                    scheduled_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    finished_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    status = '0', 
+                    error = '0', 
+                    metrics = [
+                        kfp_tekton_server_api.models.v1_run_metric.v1RunMetric(
+                            name = '0', 
+                            node_id = '0', 
+                            number_value = 1.337, 
+                            format = 'UNSPECIFIED', )
                         ], ), 
-                resource_references = [
-                    kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                        key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
-                            type = 'UNKNOWN_RESOURCE_TYPE', 
-                            id = '0', ), 
-                        name = '0', 
-                        relationship = 'UNKNOWN_RELATIONSHIP', )
-                    ], 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
+                pipeline_runtime = kfp_tekton_server_api.models.v1_pipeline_runtime.v1PipelineRuntime(
+                    pipeline_manifest = '0', 
+                    workflow_manifest = '0', )
             )
         else :
-            return V1Pipeline(
+            return V1RunDetail(
         )
 
-    def testV1Pipeline(self):
-        """Test V1Pipeline"""
+    def testV1RunDetail(self):
+        """Test V1RunDetail"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_pipeline_runtime.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_version.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_list_pipeline_versions_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,74 +12,65 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kfp_tekton_server_api
-from kfp_tekton_server_api.models.v1_pipeline_version import V1PipelineVersion  # noqa: E501
+from kfp_tekton_server_api.models.v1_list_pipeline_versions_response import V1ListPipelineVersionsResponse  # noqa: E501
 from kfp_tekton_server_api.rest import ApiException
 
-class TestV1PipelineVersion(unittest.TestCase):
-    """V1PipelineVersion unit test stubs"""
+class TestV1ListPipelineVersionsResponse(unittest.TestCase):
+    """V1ListPipelineVersionsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1PipelineVersion
+        """Test V1ListPipelineVersionsResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kfp_tekton_server_api.models.v1_pipeline_version.V1PipelineVersion()  # noqa: E501
+        # model = kfp_tekton_server_api.models.v1_list_pipeline_versions_response.V1ListPipelineVersionsResponse()  # noqa: E501
         if include_optional :
-            return V1PipelineVersion(
-                id = '0', 
-                name = '0', 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                parameters = [
-                    kfp_tekton_server_api.models.v1_parameter.v1Parameter(
+            return V1ListPipelineVersionsResponse(
+                versions = [
+                    kfp_tekton_server_api.models.v1_pipeline_version.v1PipelineVersion(
+                        id = '0', 
                         name = '0', 
-                        value = '0', )
+                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        parameters = [
+                            kfp_tekton_server_api.models.v1_parameter.v1Parameter(
+                                name = '0', 
+                                value = '0', )
+                            ], 
+                        code_source_url = '0', 
+                        package_url = kfp_tekton_server_api.models.v1_url.v1Url(
+                            pipeline_url = '0', ), 
+                        resource_references = [
+                            kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
+                                key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
+                                    type = 'UNKNOWN_RESOURCE_TYPE', 
+                                    id = '0', ), 
+                                name = '0', 
+                                relationship = 'UNKNOWN_RELATIONSHIP', )
+                            ], 
+                        description = '0', )
                     ], 
-                code_source_url = '0', 
-                package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                    pipeline_url = '0', 
-                    pipeline_url = '0', ), 
-                resource_references = [
-                    kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                        key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
-                            type = 'UNKNOWN_RESOURCE_TYPE', 
-                            id = '0', ), 
-                        name = '0', 
-                        relationship = 'UNKNOWN_RELATIONSHIP', )
-                    ], 
-                description = '0', 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                code_source_url = '0', 
-                package_url = kfp_tekton_server_api.models.v1_url.v1Url(
-                    pipeline_url = '0', 
-                    pipeline_url = '0', ), 
-                resource_references = [
-                    kfp_tekton_server_api.models.v1_resource_reference.v1ResourceReference(
-                        key = kfp_tekton_server_api.models.v1_resource_key.v1ResourceKey(
-                            type = 'UNKNOWN_RESOURCE_TYPE', 
-                            id = '0', ), 
-                        name = '0', 
-                        relationship = 'UNKNOWN_RELATIONSHIP', )
-                    ]
+                next_page_token = '0', 
+                total_size = 56
             )
         else :
-            return V1PipelineVersion(
+            return V1ListPipelineVersionsResponse(
         )
 
-    def testV1PipelineVersion(self):
-        """Test V1PipelineVersion"""
+    def testV1ListPipelineVersionsResponse(self):
+        """Test V1ListPipelineVersionsResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_relationship.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_report_run_metrics_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_resource_key.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_resource_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_resource_type.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_run.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_run_metric.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_url.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_url.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         """Test V1Url
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = kfp_tekton_server_api.models.v1_url.V1Url()  # noqa: E501
         if include_optional :
             return V1Url(
-                pipeline_url = '0', 
                 pipeline_url = '0'
             )
         else :
             return V1Url(
         )
 
     def testV1Url(self):
```

### Comparing `kfp-tekton-server-api-1.8.0rc6/test/test_v1_value.py` & `kfp-tekton-server-api-1.8.0rc7/test/test_v1_value.py`

 * *Files identical despite different names*

