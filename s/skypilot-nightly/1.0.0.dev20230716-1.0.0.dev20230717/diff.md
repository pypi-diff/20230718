# Comparing `tmp/skypilot-nightly-1.0.0.dev20230716.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230717.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230716.tar", last modified: Sun Jul 16 10:40:58 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230717.tar", last modified: Mon Jul 17 10:43:20 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230716.tar` & `skypilot-nightly-1.0.0.dev20230717.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.280852 skypilot-nightly-1.0.0.dev20230716/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-16 10:40:58.280852 skypilot-nightly-1.0.0.dev20230716/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 10:40:58.280852 skypilot-nightly-1.0.0.dev20230716/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-16 10:40:49.000000 skypilot-nightly-1.0.0.dev20230716/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.252852 skypilot-nightly-1.0.0.dev20230716/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-16 10:40:49.000000 skypilot-nightly-1.0.0.dev20230716/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.252852 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.256852 skypilot-nightly-1.0.0.dev20230716/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   112970 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   200283 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.256852 skypilot-nightly-1.0.0.dev20230716/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.256852 skypilot-nightly-1.0.0.dev20230716/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.256852 skypilot-nightly-1.0.0.dev20230716/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41057 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25706 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    42681 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/aws/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.260852 skypilot-nightly-1.0.0.dev20230716/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-16 10:40:49.000000 skypilot-nightly-1.0.0.dev20230716/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.244852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.264852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.268852 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.272852 skypilot-nightly-1.0.0.dev20230716/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.276852 skypilot-nightly-1.0.0.dev20230716/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.276852 skypilot-nightly-1.0.0.dev20230716/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/env_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.276852 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-16 10:40:58.000000 skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:40:58.280852 skypilot-nightly-1.0.0.dev20230716/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   124066 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-16 10:40:44.000000 skypilot-nightly-1.0.0.dev20230716/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.341377 skypilot-nightly-1.0.0.dev20230717/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-17 10:43:20.341377 skypilot-nightly-1.0.0.dev20230717/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 10:43:20.341377 skypilot-nightly-1.0.0.dev20230717/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-17 10:43:10.000000 skypilot-nightly-1.0.0.dev20230717/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.317377 skypilot-nightly-1.0.0.dev20230717/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 10:43:10.000000 skypilot-nightly-1.0.0.dev20230717/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.317377 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112970 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200283 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41057 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26861 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42681 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.321377 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-17 10:43:10.000000 skypilot-nightly-1.0.0.dev20230717/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.325377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.313377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.329377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.333377 skypilot-nightly-1.0.0.dev20230717/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.337377 skypilot-nightly-1.0.0.dev20230717/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.337377 skypilot-nightly-1.0.0.dev20230717/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.337377 skypilot-nightly-1.0.0.dev20230717/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/env_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.337377 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-17 10:43:20.000000 skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 10:43:20.341377 skypilot-nightly-1.0.0.dev20230717/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124066 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 10:43:04.000000 skypilot-nightly-1.0.0.dev20230717/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/LICENSE` & `skypilot-nightly-1.0.0.dev20230717/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230717/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230717/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230716
+Version: 1.0.0.dev20230717
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230716
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230717
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/README.md` & `skypilot-nightly-1.0.0.dev20230717/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230717/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/setup.py` & `skypilot-nightly-1.0.0.dev20230717/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230717/sky/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = '95fdb5b21a87bb3a592bc7178cb508f183daa84e'
-__version__ = '1.0.0-dev20230716'
+__commit__ = '3a8ae21556069e9585bbe9fa0b8fd6641eaf8b00'
+__version__ = '1.0.0-dev20230717'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230717/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230717/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230717/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230717/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230717/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230717/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230717/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/check.py` & `skypilot-nightly-1.0.0.dev20230717/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230717/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230717/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,17 @@
     _MAX_CLUSTER_NAME_LEN_LIMIT = 42
 
     @classmethod
     def _cloud_unsupported_features(
             cls) -> Dict[clouds.CloudImplementationFeatures, str]:
         return {
             clouds.CloudImplementationFeatures.CLONE_DISK_FROM_CLUSTER: f'Migrating disk is not supported in {cls._REPR}.',
+            # TODO(zhwu): our azure subscription offer ID does not support spot.
+            # Need to support it.
+            clouds.CloudImplementationFeatures.SPOT_INSTANCE: f'Spot instances are not supported in {cls._REPR}.',
         }
 
     @classmethod
     def _max_cluster_name_length(cls) -> int:
         return cls._MAX_CLUSTER_NAME_LEN_LIMIT
 
     def instance_type_to_hourly_cost(self,
@@ -278,18 +281,14 @@
                     return (False, None)
                 disk_tier = list(all_tiers)[0]
             if disk_tier != clouds.Cloud._DEFAULT_DISK_TIER:
                 return True, disk_tier
             else:
                 return True, None
 
-        if resources.use_spot:
-            # TODO(zhwu): our azure subscription offer ID does not support spot.
-            # Need to support it.
-            return ([], [])
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             ok, disk_tier = failover_disk_tier(resources.instance_type,
                                                resources.disk_tier)
             if not ok:
                 return ([], [])
             # Treat Resources(Azure, Standard_NC4as_T4_v3, T4) as
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     _cloud_unsupported_features in all clouds to make sure the
     check_features_are_supported() works as expected.
     """
     STOP = 'stop'
     AUTOSTOP = 'autostop'
     MULTI_NODE = 'multi-node'
     CLONE_DISK_FROM_CLUSTER = 'clone_disk_from_cluster'
+    SPOT_INSTANCE = 'spot_instance'
+    CUSTOM_DOSK_TIER = 'custom_disk_tier'
 
 
 class Region(collections.namedtuple('Region', ['name'])):
     """A region."""
     name: str
     zones: Optional[List['Zone']] = None
 
@@ -292,14 +294,19 @@
         requirements.  Currently, this function implements "filtering" the
         cloud's offerings only w.r.t. accelerators constraints.
 
         Launchable resources require a cloud and an instance type be assigned.
         """
         if resources.is_launchable():
             self._check_instance_type_accelerators_combination(resources)
+        resources_required_features = resources.get_required_cloud_features()
+        try:
+            self.check_features_are_supported(resources_required_features)
+        except exceptions.NotSupportedError:
+            return ([], [])
         return self._get_feasible_launchable_resources(resources)
 
     def _get_feasible_launchable_resources(self, resources):
         raise NotImplementedError
 
     @classmethod
     def check_credentials(cls) -> Tuple[bool, Optional[str]]:
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/ibm.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
     @classmethod
     def _cloud_unsupported_features(
             cls) -> Dict[clouds.CloudImplementationFeatures, str]:
         return {
             clouds.CloudImplementationFeatures.CLONE_DISK_FROM_CLUSTER:
                 (f'Migrating disk is not supported in {cls._REPR}.'),
+            clouds.CloudImplementationFeatures.CUSTOM_DOSK_TIER:
+                (f'Custom disk tier is not supported in {cls._REPR}.'),
         }
 
     @classmethod
     def _max_cluster_name_length(cls) -> Optional[int]:
         return cls._MAX_CLUSTER_NAME_LEN_LIMIT
 
     @classmethod
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/lambda_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     # Currently, none of clouds.CloudImplementationFeatures are implemented
     # for Lambda Cloud.
     # STOP/AUTOSTOP: The Lambda cloud provider does not support stopping VMs.
     _CLOUD_UNSUPPORTED_FEATURES = {
         clouds.CloudImplementationFeatures.STOP: 'Lambda cloud does not support stopping VMs.',
         clouds.CloudImplementationFeatures.AUTOSTOP: 'Lambda cloud does not support stopping VMs.',
         clouds.CloudImplementationFeatures.CLONE_DISK_FROM_CLUSTER: f'Migrating disk is not supported in {_REPR}.',
+        clouds.CloudImplementationFeatures.SPOT_INSTANCE: f'Spot instances are not supported in {_REPR}.',
+        clouds.CloudImplementationFeatures.CUSTOM_DOSK_TIER: f'Custom disk tiers are not supported in {_REPR}.',
     }
 
     @classmethod
     def _cloud_unsupported_features(
             cls) -> Dict[clouds.CloudImplementationFeatures, str]:
         return cls._CLOUD_UNSUPPORTED_FEATURES
 
@@ -161,16 +163,14 @@
             'instance_type': resources.instance_type,
             'custom_resources': custom_resources,
             'region': region.name,
         }
 
     def _get_feasible_launchable_resources(
             self, resources: 'resources_lib.Resources'):
-        if resources.use_spot or resources.disk_tier is not None:
-            return ([], [])
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             # Accelerators are part of the instance type in Lambda Cloud
             resources = resources.copy(accelerators=None)
             return ([resources], [])
 
         def _make(instance_list):
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/scp.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,18 @@
     _MAX_CLUSTER_NAME_LEN_LIMIT = 28
     # MULTI_NODE: Multi-node is not supported by the implementation yet.
     _MULTI_NODE = 'Multi-node is not supported by the SCP Cloud yet.'
     _CLOUD_UNSUPPORTED_FEATURES = {
         clouds.CloudImplementationFeatures.MULTI_NODE: _MULTI_NODE,
         clouds.CloudImplementationFeatures.CLONE_DISK_FROM_CLUSTER:
             (f'Migrating disk is not supported in {_REPR}.'),
+        clouds.CloudImplementationFeatures.SPOT_INSTANCE:
+            (f'Spot instances are not supported in {_REPR}.'),
+        clouds.CloudImplementationFeatures.CUSTOM_DOSK_TIER:
+            (f'Custom disk tiers are not supported in {_REPR}.'),
     }
 
     _INDENT_PREFIX = '    '
 
     @classmethod
     def _cloud_unsupported_features(
             cls) -> Dict[clouds.CloudImplementationFeatures, str]:
@@ -226,16 +230,14 @@
         # we need to find a better way to handle this.
         raise exceptions.ResourcesUnavailableError(
             'No image found in catalog for region '
             f'{region_name}. Try setting a valid image_id.')
 
     def _get_feasible_launchable_resources(
             self, resources: 'resources_lib.Resources'):
-        if resources.use_spot or resources.disk_tier is not None:
-            return ([], [])
         # Check if the host VM satisfies the min/max disk size limits.
         is_allowed = self._is_disk_size_allowed(resources)
         if not is_allowed:
             return ([], [])
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             # Accelerators are part of the instance type in SCP Cloud
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230717/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/core.py` & `skypilot-nightly-1.0.0.dev20230717/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230717/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230717/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230717/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230717/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230717/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230717/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230717/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230717/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230717/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230717/sky/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Resources: compute requirements of Tasks."""
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, Set
 from typing_extensions import Literal
 
 import colorama
 
 from sky import clouds
 from sky import global_user_state
 from sky import sky_logging
@@ -887,14 +887,24 @@
         if self.zone is not None and self.zone not in zones:
             return False
         if self.image_id is not None:
             if None not in self.image_id and region not in self.image_id:
                 return False
         return True
 
+    def get_required_cloud_features(
+            self) -> Set[clouds.CloudImplementationFeatures]:
+        """Returns the set of cloud features required by this Resources."""
+        features = set()
+        if self.use_spot:
+            features.add(clouds.CloudImplementationFeatures.SPOT_INSTANCE)
+        if self.disk_tier is not None:
+            features.add(clouds.CloudImplementationFeatures.CUSTOM_DOSK_TIER)
+        return features
+
     @classmethod
     def from_yaml_config(cls, config: Optional[Dict[str, str]]) -> 'Resources':
         if config is None:
             return Resources()
 
         backend_utils.validate_schema(config, schemas.get_resources_schema(),
                                       'Invalid resources YAML: ')
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230717/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230717/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230717/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230717/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230717/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230717/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230717/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230717/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230717/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230717/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230717/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/task.py` & `skypilot-nightly-1.0.0.dev20230717/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230717/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230717/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230717/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230717/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230717/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230717/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230717/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230717/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230717/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230717/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230717/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230717/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230716
+Version: 1.0.0.dev20230717
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230716
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230717
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230717/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230716/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230717/tests/test_wheels.py`

 * *Files identical despite different names*

