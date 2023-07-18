# Comparing `tmp/domino-py-0.3.0.tar.gz` & `tmp/domino-py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.3.0.tar", last modified: Thu May 18 06:57:42 2023, max compression
+gzip compressed data, was "domino-py-0.4.0.tar", last modified: Tue Jul 18 13:46:28 2023, max compression
```

## Comparing `domino-py-0.3.0.tar` & `domino-py-0.4.0.tar`

### file list

```diff
@@ -1,72 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.772395 domino-py-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-18 06:57:28.000000 domino-py-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-18 06:57:42.772395 domino-py-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-18 06:57:28.000000 domino-py-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.752395 domino-py-0.3.0/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.752395 domino-py-0.3.0/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.756395 domino-py-0.3.0/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    24061 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.760395 domino-py-0.3.0/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.760395 domino-py-0.3.0/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/docker_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/external_python_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.760395 domino-py-0.3.0/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/custom_operators/sidecar/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.764395 domino-py-0.3.0/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.764395 domino-py-0.3.0/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/deploy_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/display_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.768395 domino-py-0.3.0/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/piece_dry_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/run_piece_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.768395 domino-py-0.3.0/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/utils/piece_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 06:57:29.000000 domino-py-0.3.0/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:57:42.772395 domino-py-0.3.0/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 06:57:42.000000 domino-py-0.3.0/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:57:42.772395 domino-py-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-18 06:57:29.000000 domino-py-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.593134 domino-py-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 13:46:17.000000 domino-py-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-18 13:46:28.593134 domino-py-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-18 13:46:17.000000 domino-py-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.585134 domino-py-0.4.0/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.585134 domino-py-0.4.0/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.585134 domino-py-0.4.0/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18294 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24061 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.589135 domino-py-0.4.0/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.589135 domino-py-0.4.0/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/custom_operators/docker_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/custom_operators/external_python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16979 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.589135 domino-py-0.4.0/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/custom_operators/sidecar/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.589135 domino-py-0.4.0/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.589135 domino-py-0.4.0/domino/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/models/output_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.589135 domino-py-0.4.0/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/schemas/deploy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/schemas/display_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.589135 domino-py-0.4.0/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/scripts/deprecated_piece_dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/scripts/run_piece_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.589135 domino-py-0.4.0/domino/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/testing/dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/testing/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/testing/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.589135 domino-py-0.4.0/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/utils/piece_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 13:46:17.000000 domino-py-0.4.0/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:46:28.593134 domino-py-0.4.0/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-18 13:46:28.000000 domino-py-0.4.0/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-18 13:46:28.000000 domino-py-0.4.0/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:46:28.000000 domino-py-0.4.0/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 13:46:28.000000 domino-py-0.4.0/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-18 13:46:28.000000 domino-py-0.4.0/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 13:46:28.000000 domino-py-0.4.0/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:46:28.593134 domino-py-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-18 13:46:17.000000 domino-py-0.4.0/setup.py
```

### Comparing `domino-py-0.3.0/LICENSE` & `domino-py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/PKG-INFO` & `domino-py-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,193 +1,205 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python package for the Domino platform
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
-Description: 
-        
-        <p align="center">
+Description: <p align="center">
           <img src="https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/logo.png" width="450" title="Domino">
         </p>
+        <p align="center"><i>Build amazing ideas, piece by piece.</i></p>
         <p align="center">
           <a href="https://pypi.org/project/domino-py">
             <img src="https://img.shields.io/pypi/v/domino-py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">
           </a>
           <a href="https://artifacthub.io/packages/helm/domino/domino">
             <img src="https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino">
           </a>
           <a href="https://domino-py.readthedocs.io/en/latest/">
             <img alt="Read the Docs" src="https://img.shields.io/readthedocs/domino-py?label=Docs&logo=Read%20the%20Docs&logoColor=white">
           </a>
         </p>
         
+        <br>
+        
+        ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/7_create_workflow.gif)
         
         # Table of contents
         - [About](#about)
         - [Quick start](#quick-start)
         - [GUI](#gui)
-        - [REST](#rest)
         - [Pieces](#pieces)
+        - [REST](#rest)
+        - [Credits](#credits)
         
         <br>
         
         # About
         Domino is an open source workflow management platform, with:
         
-        - an intuitive [Graphical User Interface](#gui) that facilitates creating, editing and monitoring any type of Workflow, from data processing to machine learning
-        - a [REST API](#rest) that controls a running Apache Airflow instance
-        - a standard way of writing and publishing functional [Pieces](#pieces), which follows good practices for data modeling, documentation and distribution
+        - :desktop_computer: an intuitive [Graphical User Interface](#gui) that facilitates creating, editing and monitoring any type of Workflow, from data processing to machine learning
+        - :package: a standard way of writing and publishing functional [Pieces](#pieces), which follows good practices for data modeling, documentation and distribution
+        - :gear: a [REST API](#rest) that controls a running Apache Airflow instance
         
         
         Creating Workflows in the GUI is as simple as dragging and dropping Pieces to the canvas, and connecting them. The user can also schedule the Workflow to run periodically, at a specific date/time, or trigger it manually. The monitoring page shows the status of each Workflow Piece in real time, including the logs and results of each run.
         
+        Pieces are functional units that can be reused in multiple Workflows. Pieces can execute anything that can be written in Python, and can be easily distributed and installed directly from Github repositories to be used in Domino Workflows.
+        
         Every Domino Workflow corresponds to an Apache Airflow DAG, and each Piece corresponds to an Airflow task. Domino controls an Airflow instance, which is responsible for executing, scheduling and monitoring the Workflows (DAGs).
         
-        Pieces are functional units that can be reused in multiple Workflows. Pieces can execute anything that can be written in Python, and can be easily distributed and installed directly from Github repositories to be used in Domino Workflows.
+        You can think of Domino as Airflow with superpowers:
+        
+        - :desktop_computer: create highly complex Workflows with simple point-and-click and drag-and-drop operations, in an user-friendly GUI
+        - :package: make use of Pieces developed by other people, share and reuse your own Pieces
+        - :busts_in_silhouette: collaborate in groups to edit and monitor Workflows
+        - :chart_with_upwards_trend: experience a cleaner and more intuitive GUI for viewing Workflows results, including logs and richer reports with images and tables
+        - :minidisc: shared storage for tasks in the same workflow
+        - :arrows_counterclockwise: use gitSync to sync DAGs from files stored in a Git repository
+        - :wheel_of_dharma: scalable, Kubernetes-native platform
+        - :battery: powered by Apache Airflow for top-tier workflows scheduling and monitoring
         
         <br>
         
         # Quick start
         
         The Domino Python package can be installed via pip. We reccommend you install Domino in a separate Python environment.
         
         ```bash
         pip install domino-py
         ```
         
-        You can then use Domino command line interface to easily run the Domino platform locally. Go to a new, empty directory and run the following command:
+        You can then use Domino command line interface to easily run the Domino platform locally (requires Docker compose). Go to a new, empty directory and run the following command:
         
         ```bash
         domino platform run-compose
         ```
         
-        This is a convenience command that will:
-        - Create the necessary folder structure for Domino and Airflow processes
-        - Create a docker-compose.yaml file
-        - Run the docker compose up command
-        
-        This command might take up to a few minutes to execute, since it will download and run all the necessary docker images. If everything worked as expected, after all processes started successfully you should be able to navigate to `localhost:3000` to access the Domino frontend service.
+        After all processes started successfully, navigate to `localhost:3000` to access the Domino frontend service.
         
         Running the Domino platform locally with Docker compose is useful for development and testing purposes. For production environments, we recommend you install Domino in a Kubernetes cluster:
         - Running Domino in a [local Kubernetes cluster with Kind](https://domino-py.readthedocs.io/en/latest/pages/platform.html)
         - Running Domino in a [remote Kubernetes cluster](https://domino-py.readthedocs.io/en/latest/pages/deployment_cloud.html)
         
         <br>
         
         # GUI
         The Domino frontend service is a React application that provides the GUI for easily creating, editing and monitoring Workflows. Here are some of its features:
         
         <details>
           <summary>
+            <strong>Access authentication</strong>
+          </summary>
+          Sign up and login to use the Domino platform. <br></br>
+        
+          ![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/1_sign_up.gif)
+        
+        </details>
+        
+        <details>
+          <summary>
+            <strong>Create Workspaces</strong>
+          </summary>
+          Create new Workspaces and add your github access token. <br></br>
+        
+          ![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/2_create_workspace_and_token.gif)
+        
+        </details>
+        
+        <details>
+          <summary>
             <strong>Install Pieces repositories</strong>
           </summary>
           Install bundles of Pieces to your Domino Workspaces direclty from Github repositories, and use them in your Workflows. <br></br>
         
-          ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/3_install_pieces.gif)
+          ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_install_pieces.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Create Workflows</strong>
           </summary>
           Create Workflows by dragging and dropping Pieces to the canvas, and connecting them. <br></br>
         
-          ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/4_create_workflow.gif)
+          ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/7_create_workflow.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Edit Pieces</strong>
           </summary>
           Edit Pieces by changing their input. Outputs from upstream Pieces are automatically available as inputs for downstream Pieces. Pieces can pass forward any type of data, from simple strings to heavy files, all automatically handled by Domino shared storage system. <br></br>
         
-          ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/5_edit_pieces.gif)
+          ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/8_edit_pieces.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Schedule Workflows</strong>
           </summary>
           Schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
         
-          ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_edit_workflow.gif)
+          ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/9_edit_workflow.gif)
         </details>
         
         <details>
           <summary>
             <strong>Monitor Workflows</strong>
           </summary>
           Monitor Workflows in real time, including the status of each Piece, the logs and results of each run. <br></br>
         
-          ![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/7_monitor_workflow.gif)
+          ![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/10_monitor_workflow.gif)
         
         </details>
         
         <br>
         
-        # REST
-        The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
-        
-        - executing operations requested by the frontend service
-        - interacting with the Airflow instance, including triggering, creating, editing and deleting Workflows (DAGs)
-        - interacting with the Domino Database
-        
-        The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://domino-py.readthedocs.io/en/latest/pages/rest.html).
-        
-        <br>
-        
         # Pieces
         Pieces are the secret sauce of Domino, they are functional units that can be distributed and reused in multiple Workflows. Domino Pieces are special because they:
         
-        - can execute anything written in Python, heavy-weight (e.g. Machine Learning) as well as light-weight (e.g. sending emails) tasks
-        - have well defined data models for inputs, outputs and secrets
-        - run in isolated execution environments (Docker containers)
-        - are organized in repositories, for easy distribution and installation
+        - :snake: can execute anything written in Python, heavy-weight (e.g. Machine Learning) as well as light-weight (e.g. sending emails) tasks
+        - :traffic_light: have well defined data models for inputs, outputs and secrets
+        - :package: run in self-contained and isolated execution environments (Docker containers)
+        - :gear: are immutable, guaranteeing reproducibility of your workflows
+        - :octocat: are organized in git repositories, for easy packaging, distribution and installation
+        - :bookmark_tabs: are properly versioned, tested and documented
+        - :zap: are plug-and-play and versatile, can be easily incorporated in any workflow
+        
+        It is very easy to create and share your own Pieces:
+        
+        - :one: write your Python function
+        - :two: define its data types (input, output and secrets)
+        - :three: define its dependencies (requirements.txt or Dockerfile)
+        - :four: publish it in a repository (public or private)
         
-        To facilitate the creation of Pieces, we provide a [template repository](https://github.com/Tauffer-Consulting/domino_pieces_repository_template) with the basic file structure and examples for data models, metadata, source code and dependencies.
+        The [Pieces repository template](https://github.com/Tauffer-Consulting/domino_pieces_repository_template) provides the basic structure, example files and automatic actions for a seamless Pieces creation experience.
         
-        In short, each Piece is a folder containing the following files:
-        - A `piece.py` file with the source code to be executed
-        - A `models.py` file containing the Pydantic models that define the input, output and secrets for the Piece
-        - A `metadata.json` file containing the Piece's metadata, including dependencies and GUI style
+        Read more in the [Pieces documentation](https://domino-py.readthedocs.io/en/latest/pages/pieces.html).
         
-        A repository contains multiples Pieces. Pieces with the same dependencies are automatically grouped together in a dependency group, and each dependency group is built into a Docker image. The Docker images are the self contained execution environments containing the Piece's source code and with all the necessary dependencies installed.
         
-        The Docker images are automatically built and published in the same Github repository as the Pieces. This organization makes it straightforward to install Pieces respositories in Domino Workspaces, to be used in Workflows.
-        
-        Read more about Pieces and how to create them in the [Pieces documentation](https://domino-py.readthedocs.io/en/latest/pages/pieces.html).
+        <br>
         
+        # REST
+        The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
         
-        <br>
+        - executing operations requested by the frontend service
+        - interacting with the Airflow instance, including triggering, creating, editing and deleting Workflows (DAGs)
+        - interacting with the Domino Database
         
-        # Platform
+        The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://domino-py.readthedocs.io/en/latest/pages/rest.html).
         
-        ## GitSync
-        A good practice when running Airflow in a Kubernetes cluster is to use a GitSync container to sync DAGs from a Git repository to the Airflow services. 
+        <br>
         
-        ## Shared storage structure
-        Shared workflow data could be stored in a remote source (e.g. S3 bucket) or locally (for dev and tests only).
+        # Credits
+        Domino is developed and maintained by [Tauffer Consulting](https://www.taufferconsulting.com/).
         
-        ```
-        /shared_storage
-        ..../{workflow-id}
-        ......../{run-id}
-        ............/{task-id}
-        ................/results
-        ..................../log.txt
-        ..................../result.npy
-        ..................../result.html
-        ................/report
-        ................/xcom_out
-        ..................../xcom_out.json
-        ```
 Keywords: domino,airflow,gui
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: airflow
```

#### html2text {}

```diff
@@ -1,110 +1,117 @@
-Metadata-Version: 2.1 Name: domino-py Version: 0.3.0 Summary: Python package
+Metadata-Version: 2.1 Name: domino-py Version: 0.4.0 Summary: Python package
 for the Domino platform Home-page: UNKNOWN Author: Luiz Tauffer and Vinicius
 Vaz Author-email: luiz@taufferconsulting.com License: UNKNOWN Description:
    [https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/
                                    logo.png]
+                     Build amazing ideas, piece by piece.
                     [https://img.shields.io/pypi/v/domino-
   py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20] [https://
  img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino]
                                 [Read_the_Docs]
-# Table of contents - [About](#about) - [Quick start](#quick-start) - [GUI]
-(#gui) - [REST](#rest) - [Pieces](#pieces)
-# About Domino is an open source workflow management platform, with: - an
-intuitive [Graphical User Interface](#gui) that facilitates creating, editing
-and monitoring any type of Workflow, from data processing to machine learning -
-a [REST API](#rest) that controls a running Apache Airflow instance - a
-standard way of writing and publishing functional [Pieces](#pieces), which
-follows good practices for data modeling, documentation and distribution
-Creating Workflows in the GUI is as simple as dragging and dropping Pieces to
-the canvas, and connecting them. The user can also schedule the Workflow to run
-periodically, at a specific date/time, or trigger it manually. The monitoring
-page shows the status of each Workflow Piece in real time, including the logs
-and results of each run. Every Domino Workflow corresponds to an Apache Airflow
-DAG, and each Piece corresponds to an Airflow task. Domino controls an Airflow
-instance, which is responsible for executing, scheduling and monitoring the
-Workflows (DAGs). Pieces are functional units that can be reused in multiple
-Workflows. Pieces can execute anything that can be written in Python, and can
-be easily distributed and installed directly from Github repositories to be
-used in Domino Workflows.
+
+![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/7_create_workflow.gif) # Table of contents -
+[About](#about) - [Quick start](#quick-start) - [GUI](#gui) - [Pieces](#pieces)
+- [REST](#rest) - [Credits](#credits)
+# About Domino is an open source workflow management platform, with: - :
+desktop_computer: an intuitive [Graphical User Interface](#gui) that
+facilitates creating, editing and monitoring any type of Workflow, from data
+processing to machine learning - :package: a standard way of writing and
+publishing functional [Pieces](#pieces), which follows good practices for data
+modeling, documentation and distribution - :gear: a [REST API](#rest) that
+controls a running Apache Airflow instance Creating Workflows in the GUI is as
+simple as dragging and dropping Pieces to the canvas, and connecting them. The
+user can also schedule the Workflow to run periodically, at a specific date/
+time, or trigger it manually. The monitoring page shows the status of each
+Workflow Piece in real time, including the logs and results of each run. Pieces
+are functional units that can be reused in multiple Workflows. Pieces can
+execute anything that can be written in Python, and can be easily distributed
+and installed directly from Github repositories to be used in Domino Workflows.
+Every Domino Workflow corresponds to an Apache Airflow DAG, and each Piece
+corresponds to an Airflow task. Domino controls an Airflow instance, which is
+responsible for executing, scheduling and monitoring the Workflows (DAGs). You
+can think of Domino as Airflow with superpowers: - :desktop_computer: create
+highly complex Workflows with simple point-and-click and drag-and-drop
+operations, in an user-friendly GUI - :package: make use of Pieces developed by
+other people, share and reuse your own Pieces - :busts_in_silhouette:
+collaborate in groups to edit and monitor Workflows - :
+chart_with_upwards_trend: experience a cleaner and more intuitive GUI for
+viewing Workflows results, including logs and richer reports with images and
+tables - :minidisc: shared storage for tasks in the same workflow - :
+arrows_counterclockwise: use gitSync to sync DAGs from files stored in a Git
+repository - :wheel_of_dharma: scalable, Kubernetes-native platform - :battery:
+powered by Apache Airflow for top-tier workflows scheduling and monitoring
 # Quick start The Domino Python package can be installed via pip. We reccommend
 you install Domino in a separate Python environment. ```bash pip install
 domino-py ``` You can then use Domino command line interface to easily run the
-Domino platform locally. Go to a new, empty directory and run the following
-command: ```bash domino platform run-compose ``` This is a convenience command
-that will: - Create the necessary folder structure for Domino and Airflow
-processes - Create a docker-compose.yaml file - Run the docker compose up
-command This command might take up to a few minutes to execute, since it will
-download and run all the necessary docker images. If everything worked as
-expected, after all processes started successfully you should be able to
-navigate to `localhost:3000` to access the Domino frontend service. Running the
-Domino platform locally with Docker compose is useful for development and
-testing purposes. For production environments, we recommend you install Domino
-in a Kubernetes cluster: - Running Domino in a [local Kubernetes cluster with
-Kind](https://domino-py.readthedocs.io/en/latest/pages/platform.html) - Running
-Domino in a [remote Kubernetes cluster](https://domino-py.readthedocs.io/en/
-latest/pages/deployment_cloud.html)
+Domino platform locally (requires Docker compose). Go to a new, empty directory
+and run the following command: ```bash domino platform run-compose ``` After
+all processes started successfully, navigate to `localhost:3000` to access the
+Domino frontend service. Running the Domino platform locally with Docker
+compose is useful for development and testing purposes. For production
+environments, we recommend you install Domino in a Kubernetes cluster: -
+Running Domino in a [local Kubernetes cluster with Kind](https://domino-
+py.readthedocs.io/en/latest/pages/platform.html) - Running Domino in a [remote
+Kubernetes cluster](https://domino-py.readthedocs.io/en/latest/pages/
+deployment_cloud.html)
 # GUI The Domino frontend service is a React application that provides the GUI
 for easily creating, editing and monitoring Workflows. Here are some of its
-features:   Install Pieces repositories  Install bundles of Pieces to your
-Domino Workspaces direclty from Github repositories, and use them in your
-Workflows.
+features:   Access authentication  Sign up and login to use the Domino
+platform.
+![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/1_sign_up.gif)    Create Workspaces
+Create new Workspaces and add your github access token.
+![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/2_create_workspace_and_token.gif)
+Install Pieces repositories  Install bundles of Pieces to your Domino
+Workspaces direclty from Github repositories, and use them in your Workflows.
 ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
-main/docs/source/_static/media/3_install_pieces.gif)    Create Workflows
+main/docs/source/_static/media/6_install_pieces.gif)    Create Workflows
 Create Workflows by dragging and dropping Pieces to the canvas, and connecting
 them.
 ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
-main/docs/source/_static/media/4_create_workflow.gif)    Edit Pieces  Edit
+main/docs/source/_static/media/7_create_workflow.gif)    Edit Pieces  Edit
 Pieces by changing their input. Outputs from upstream Pieces are automatically
 available as inputs for downstream Pieces. Pieces can pass forward any type of
 data, from simple strings to heavy files, all automatically handled by Domino
 shared storage system.
 ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
-main/docs/source/_static/media/5_edit_pieces.gif)    Schedule Workflows
+main/docs/source/_static/media/8_edit_pieces.gif)    Schedule Workflows
 Schedule Workflows to run periodically, at a specific date/time, or trigger
 them manually.
 ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/
-domino/main/docs/source/_static/media/6_edit_workflow.gif)    Monitor Workflows
+domino/main/docs/source/_static/media/9_edit_workflow.gif)    Monitor Workflows
 Monitor Workflows in real time, including the status of each Piece, the logs
 and results of each run.
 ![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/
-domino/main/docs/source/_static/media/7_monitor_workflow.gif)
+domino/main/docs/source/_static/media/10_monitor_workflow.gif)
+# Pieces Pieces are the secret sauce of Domino, they are functional units that
+can be distributed and reused in multiple Workflows. Domino Pieces are special
+because they: - :snake: can execute anything written in Python, heavy-weight
+(e.g. Machine Learning) as well as light-weight (e.g. sending emails) tasks - :
+traffic_light: have well defined data models for inputs, outputs and secrets -
+:package: run in self-contained and isolated execution environments (Docker
+containers) - :gear: are immutable, guaranteeing reproducibility of your
+workflows - :octocat: are organized in git repositories, for easy packaging,
+distribution and installation - :bookmark_tabs: are properly versioned, tested
+and documented - :zap: are plug-and-play and versatile, can be easily
+incorporated in any workflow It is very easy to create and share your own
+Pieces: - :one: write your Python function - :two: define its data types
+(input, output and secrets) - :three: define its dependencies (requirements.txt
+or Dockerfile) - :four: publish it in a repository (public or private) The
+[Pieces repository template](https://github.com/Tauffer-Consulting/
+domino_pieces_repository_template) provides the basic structure, example files
+and automatic actions for a seamless Pieces creation experience. Read more in
+the [Pieces documentation](https://domino-py.readthedocs.io/en/latest/pages/
+pieces.html).
 # REST The Backend service is a REST API that controls a running Apache Airflow
 instance. It is responsible for: - executing operations requested by the
 frontend service - interacting with the Airflow instance, including triggering,
 creating, editing and deleting Workflows (DAGs) - interacting with the Domino
 Database The REST service is written in Python, using the FastAPI framework.
 Read more about it in the [REST documentation](https://domino-
 py.readthedocs.io/en/latest/pages/rest.html).
-# Pieces Pieces are the secret sauce of Domino, they are functional units that
-can be distributed and reused in multiple Workflows. Domino Pieces are special
-because they: - can execute anything written in Python, heavy-weight (e.g.
-Machine Learning) as well as light-weight (e.g. sending emails) tasks - have
-well defined data models for inputs, outputs and secrets - run in isolated
-execution environments (Docker containers) - are organized in repositories, for
-easy distribution and installation To facilitate the creation of Pieces, we
-provide a [template repository](https://github.com/Tauffer-Consulting/
-domino_pieces_repository_template) with the basic file structure and examples
-for data models, metadata, source code and dependencies. In short, each Piece
-is a folder containing the following files: - A `piece.py` file with the source
-code to be executed - A `models.py` file containing the Pydantic models that
-define the input, output and secrets for the Piece - A `metadata.json` file
-containing the Piece's metadata, including dependencies and GUI style A
-repository contains multiples Pieces. Pieces with the same dependencies are
-automatically grouped together in a dependency group, and each dependency group
-is built into a Docker image. The Docker images are the self contained
-execution environments containing the Piece's source code and with all the
-necessary dependencies installed. The Docker images are automatically built and
-published in the same Github repository as the Pieces. This organization makes
-it straightforward to install Pieces respositories in Domino Workspaces, to be
-used in Workflows. Read more about Pieces and how to create them in the [Pieces
-documentation](https://domino-py.readthedocs.io/en/latest/pages/pieces.html).
-# Platform ## GitSync A good practice when running Airflow in a Kubernetes
-cluster is to use a GitSync container to sync DAGs from a Git repository to the
-Airflow services. ## Shared storage structure Shared workflow data could be
-stored in a remote source (e.g. S3 bucket) or locally (for dev and tests only).
-``` /shared_storage ..../{workflow-id} ......../{run-id} ............/{task-id}
-................/results ..................../log.txt ..................../
-result.npy ..................../result.html ................/report
-................/xcom_out ..................../xcom_out.json ``` Keywords:
-domino,airflow,gui Platform: UNKNOWN Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: airflow
+# Credits Domino is developed and maintained by [Tauffer Consulting](https://
+www.taufferconsulting.com/). Keywords: domino,airflow,gui Platform: UNKNOWN
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+airflow
```

### Comparing `domino-py-0.3.0/domino/base_piece.py` & `domino-py-0.4.0/domino/base_piece.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 from typing import Union
 import pydantic
 import pickle
 import time
 import subprocess
 import base64
+from typing import Optional
 
 from domino.logger import get_configured_logger
 from domino.schemas.deploy_mode import DeployModeType
 from domino.schemas.display_result import DisplayResultFileType
 from domino.exceptions.exceptions import InvalidPieceOutputError
 
 
@@ -121,40 +122,26 @@
                 self.upstream_tasks_data[tid]["results"] = self.workflow_shared_storage + f"/{tid}/results"
                 with open(f"{self.workflow_shared_storage}/{tid}/xcom/return.json") as f:
                     self.upstream_tasks_data[tid]["xcom"] = json.load(f)
         else:
             raise NotImplementedError(f"Get upstream XCOM not implemented for deploy_mode=={self.deploy_mode}")
 
     
-    def validate_and_get_env_secrets(self, piece_secrets_model: pydantic.BaseModel = None, secrets_values=None):
+    def validate_and_get_env_secrets(self, piece_secrets_model: pydantic.BaseModel = None):
         """
         Get secret variables for this Piece from ENV. The necessary secret variables to run the Piece should be defined in the Piece's SecretsModel.
-        The secrets can then be retrieved and used in the Piece's `piece_function` method as such:
-        ```
-        my_secret = self.secrets.my_secret
-        ```
+        The secrets can then be retrieved and used in the Piece's `piece_function` method.
 
         Args:
             piece_secrets_model (pydantic.BaseModel): _description_
         """
-        self.secrets = None
-        if piece_secrets_model and self.deploy_mode in ['local-k8s', 'local-k8s-dev', 'prod']:
-            secrets_names = list(piece_secrets_model.schema()["properties"].keys())
-            secrets = dict()
-            secrets_values = ast.literal_eval(os.environ.get('DOMINO_K8S_PIECE_SECRETS', '{}'))
-            if not secrets_values:
-                secrets_values = {}
-            for s in secrets_names:
-                secrets[s] = secrets_values.get(s, None)
-            self.secrets = piece_secrets_model(**secrets)
-        elif piece_secrets_model and self.deploy_mode == 'local-compose':
-            secrets_names = list(piece_secrets_model.schema()["properties"].keys())
-            secrets = dict()
-            secrets_values = ast.literal_eval(os.environ.get('DOMINO_DOCKER_PIECE_SECRETS', '{}'))
-            self.secrets = piece_secrets_model(**secrets_values)
+        if piece_secrets_model:
+            secrets_values = ast.literal_eval(os.environ.get('DOMINO_PIECE_SECRETS', '{}'))
+            return piece_secrets_model(**secrets_values)
+        return None
 
 
     def format_xcom(self, output_obj: pydantic.BaseModel) -> dict:
         """
         Formats and adds extra metadata to XCOM dictionary content.
 
         Args:
@@ -251,48 +238,50 @@
 
         else:
             raise NotImplementedError("deploy mode not accepted for xcom push")
     
 
     def run_piece_function(
         self, 
-        airflow_context: dict,
-        op_kwargs: dict,
+        piece_input_data: dict,
         piece_input_model: pydantic.BaseModel,
         piece_output_model: pydantic.BaseModel, 
-        piece_secrets_model: pydantic.BaseModel = None,
-        secrets_values: dict = None
+        piece_secrets_model: Optional[pydantic.BaseModel] = None,
+        airflow_context: Optional[dict] = None
     ):
         """
         _summary_
 
         Args:
-            airflow_context (dict): Dictionary containing Airflow context information
-            op_kwargs (dict): Dictionary containing Piece's kwargs
+            piece_input_data (dict): Dictionary containing Piece's Input kwargs
             piece_input_model (pydantic.BaseModel): Piece's InputModel
             piece_output_model (pydantic.BaseModel): Piece's OutputModel
             piece_secrets_model (pydantic.BaseModel, optional): Piece's SecretsModel. Defaults to None.
+            airflow_context (dict, optional): Airflow context dictionary. Defaults to None.
 
         Raises:
             InvalidPieceOutputError: _description_
         """
         # Start logger
         self.start_logger()
 
         self.piece_input_model = piece_input_model
         self.piece_output_model = piece_output_model
         self.piece_secrets_model = piece_secrets_model
 
         # Airflow context dictionary: https://composed.blog/airflow/execute-context
         # For local-bash and kubernetes deploy modes, we assemble this ourselves and the context data is more limited
-        self.airflow_context = airflow_context
-        self.dag_run_id = airflow_context.get("dag_run_id")
+        if airflow_context is None:
+            self.airflow_context = {
+                "execution_datetime": os.getenv('AIRFLOW_CONTEXT_EXECUTION_DATETIME', "123456789"),
+                "dag_run_id": os.getenv('AIRFLOW_CONTEXT_DAG_RUN_ID', "123456789"),
+            }
 
         # Check if Piece's necessary secrets are present in ENV
-        self.validate_and_get_env_secrets(piece_secrets_model=piece_secrets_model, secrets_values=secrets_values)
+        secrets_model_obj =self.validate_and_get_env_secrets(piece_secrets_model=piece_secrets_model)
 
         # Generate paths
         workflow_run_subpath = os.environ.get('DOMINO_WORKFLOW_RUN_SUBPATH', '')
         self.workflow_shared_storage = Path("/home/shared_storage") 
         if self.deploy_mode == 'local-compose':
             self.workflow_shared_storage = str(self.workflow_shared_storage / workflow_run_subpath)
         self.results_path = f"{self.workflow_shared_storage}/{self.task_id}/results"
@@ -301,55 +290,70 @@
         shared_storage_source = os.environ.get('DOMINO_WORKFLOW_SHARED_STORAGE', None)
         if not shared_storage_source or shared_storage_source == "none" or self.deploy_mode == "local-compose":
             self.generate_paths()
         else:
             self._wait_for_sidecar_paths()
             
         # Using pydantic to validate input data
-        input_model_obj = piece_input_model(**op_kwargs)
+        input_model_obj = piece_input_model(**piece_input_data)
 
         # Run piece function
-        output_obj = self.piece_function(input_model=input_model_obj)
+        call_piece_func_dict = {"input_data": input_model_obj}
+        if piece_secrets_model:
+            call_piece_func_dict['secrets_data'] = secrets_model_obj
+        output_obj = self.piece_function(**call_piece_func_dict)
 
         # Validate output data
+        if isinstance(output_obj, dict):
+            output_obj = piece_output_model(**output_obj)
         if not isinstance(output_obj, piece_output_model):
             raise InvalidPieceOutputError(piece_name=self.__class__.__name__)
 
         # Push XCom
         xcom_obj = self.format_xcom(output_obj=output_obj)
         self.push_xcom(xcom_obj=xcom_obj)
 
 
     @classmethod
     def dry_run(
         cls,
-        piece_input: dict, 
+        input_data: dict, 
         piece_input_model: pydantic.BaseModel,
-        piece_output_model: pydantic.BaseModel, 
+        piece_output_model: pydantic.BaseModel,
         piece_secrets_model: pydantic.BaseModel = None,
-        secrets_input: dict = None,
+        secrets_data: dict = None,
         results_path: str = None,
     ):
-        # Instantiate 
-        input_model_obj = piece_input_model(**piece_input)
-        secrets_model_obj = piece_secrets_model(**secrets_input) if piece_secrets_model else None
+        # Instantiate models
+        input_model_obj = piece_input_model(**input_data)
+        secrets_model_obj = piece_secrets_model(**secrets_data) if piece_secrets_model else None
 
         class DryPiece(cls):
-            def __init__(self, secrets, results_path):
+            def __init__(self, results_path):
                 self.results_path = results_path
-                self.secrets = secrets
                 self.logger = get_configured_logger(f"{self.__class__.__name__ }-dry-run")
 
-        dry_instance = DryPiece(
-            secrets=secrets_model_obj,
-            results_path=results_path
-        )
+        dry_instance = DryPiece(results_path=results_path)
 
         # Run piece function
-        return cls.piece_function(self=dry_instance, input_model=input_model_obj)
+        call_piece_func_dict = {
+            "self": dry_instance, 
+            "input_data": input_model_obj
+        }
+        if piece_secrets_model:
+            call_piece_func_dict['secrets_data'] = secrets_model_obj
+        output_obj = cls.piece_function(**call_piece_func_dict)
+        
+        # Validate output data
+        if isinstance(output_obj, dict):
+            output_obj = piece_output_model(**output_obj)
+        if not isinstance(output_obj, piece_output_model):
+            raise InvalidPieceOutputError(piece_name=cls.__name__)
+        
+        return output_obj
 
 
     @staticmethod
     def get_container_cpu_limit() -> float:
         """
         Get the CPU limit of the container in millicores.
         reference: https://stackoverflow.com/questions/65551215/get-docker-cpu-memory-limit-inside-container/65554131#65554131
```

### Comparing `domino-py-0.3.0/domino/cli/cli.py` & `domino-py-0.4.0/domino/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -227,41 +227,37 @@
     is_flag=True,
     prompt='Build Docker images?',
     expose_value=True,
     default=False,
     help='If True (default), builds Docker images.'
 )
 @click.option(
-    '--publish-images', 
-    is_flag=True,
-    prompt='Publish Docker images?',
-    expose_value=True,
-    default=False,
-    help='If True (default), publishes Docker images to github container registry.'
+    '--source-url',
+    prompt='Url of source repository',
+    default="",
+    help='The base url for this Pieces repository.'
 )
+def cli_organize_pieces_repository(build_images, source_url):
+    """Organize Pieces repository."""
+    pieces_repository.organize_pieces_repository(build_images, source_url)
+
+@click.command()
 @click.option(
     '--registry-token',
     prompt='Github Container Registry token',
     default=get_registry_token_from_env,
     help='Your Github Container Registry token with access to where the image will be published.'
 )
-@click.option(
-    '--source-url',
-    prompt='Url of source repository',
-    default="",
-    help='The base url for this Pieces repository.'
-)
-def cli_organize_pieces_repository(build_images, publish_images, registry_token, source_url):
-    """Prepare local folder for running a Domino platform."""
+def cli_publish_images(registry_token):
+    """Publish images to github container registry from mapping."""
     if registry_token:
         os.environ['GHCR_PASSWORD'] = registry_token
     console.print(f"Using registry token to publish images")
-    pieces_repository.organize_pieces_repository(build_images, publish_images, source_url)
-
-
+    pieces_repository.publish_docker_images()
+    
 @click.command()
 def cli_create_release():
     """
     Get release version for the Pieces repository in github stdout format.
     Used by github actions to set the release version.
     Needs the following env vars:
         - GITHUB_TOKEN
@@ -279,31 +275,32 @@
     elif ctx.invoked_subcommand == "create":
         pass
 
 
 cli_piece.add_command(cli_organize_pieces_repository, name="organize")
 cli_piece.add_command(cli_create_piece_repository, name="create")
 cli_piece.add_command(cli_create_release, name="release")
+cli_piece.add_command(cli_publish_images, name="publish-images")
 
 
 ###############################################################################
 # PARENT GROUP
 ###############################################################################
 
 @click.command()
 def cli_run_piece_k8s():
     """Run Piece on Kubernetes Pod"""
-    from domino.scripts.run_piece_k8s import run_piece as run_piece_in_k8s
-    
+    from domino.scripts.run_piece_docker import run_piece as run_piece_in_docker    
     console.print("Running Piece inside K8s pod...")
-    run_piece_in_k8s()
+    run_piece_in_docker()
 
 
 @click.command()
 def cli_run_piece_docker():
+    """Run Piece on Docker container"""
     from domino.scripts.run_piece_docker import run_piece as run_piece_in_docker
     console.print('Running Piece inside Docker container...')
     run_piece_in_docker()
 
 
 @click.command()
 def cli_run_piece_bash():
```

### Comparing `domino-py-0.3.0/domino/cli/utils/pieces_repository.py` & `domino-py-0.4.0/domino/cli/utils/pieces_repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -341,36 +341,55 @@
 
     if save_map_as_file:
         map_file_path = organized_domino_path / "dependencies_map.json"
         with open(map_file_path, "w") as outfile:
             json.dump(pieces_images_map, outfile, indent=4, cls=SetEncoder)
 
 
-def build_docker_images(publish_images: bool) -> None:
+def build_docker_images() -> None:
     """
     Convenience function to build Docker images from the repository dependencies and publish them to Docker Hub
     """
     from domino.scripts.build_docker_images_pieces import build_images_from_pieces_repository
 
     console.print("Building Docker images and generating map file...")
-    updated_dependencies_map = build_images_from_pieces_repository(publish=publish_images)
+    updated_dependencies_map = build_images_from_pieces_repository()
     return updated_dependencies_map
 
+def publish_docker_images() -> None:
+    """
+    Load pieces to docker image map from environment variable and publish them to Container Registry.
+    This is used in the CI/CD pipeline to publish images to Container Registry after they are built and the tests pass.
+    """
+    from domino.scripts.build_docker_images_pieces import publish_image
+
+    pieces_images_map = json.loads(os.environ.get('PIECES_IMAGES_MAP', '{}'))
+    if not pieces_images_map:
+        raise ValueError("No images found to publish.")
+    
+    console.print("Publishing Docker images...")
+    all_images = set([e for e in pieces_images_map.values()])
+    for image in all_images:
+        console.print(f"Publishing image {image}...")
+        publish_image(source_image_name=image)
+    
+
+
 
 def validate_repo_name(repo_name: str) -> None:
     """
     Validate repository name
     """
     if any([a.isspace() for a in repo_name]):
         raise ValueError("Repository name should not contain blank spaces")
     if any([a in repo_name for a in ["!", "@", "#", "$", "%", "^", "&", "*", "(", ")", "+", "=", "{", "}", "[", "]", ":", ";", "'", '"', "<", ">", "?", "/", "\\", "|", "~", "`"]]):
         raise ValueError("Repository name should not contain special characters")
 
 
-def organize_pieces_repository(build_images: bool, publish_images: bool, source_url: str) -> None:
+def organize_pieces_repository(build_images: bool, source_url: str) -> None:
     """
     Organize Piece's repository for Domino. This will: 
     - validate the folder structure, and create the pieces compiled_metadata.json and dependencies_map.json files
     - build Docker images for the Pieces
     - publish images at github container registry
     """        
     # Validate repository
@@ -390,15 +409,15 @@
     
     # Generate dependencies_map.json file
     create_dependencies_map(save_map_as_file=True)
     console.print("Metadata and dependencies organized successfully!", style=f"bold {COLOR_PALETTE.get('success')}")
 
     # Build and publish the images
     if build_images:
-        updated_dependencies_map = build_docker_images(publish_images=publish_images)
+        updated_dependencies_map = build_docker_images()
         map_file_path = Path(".") / ".domino/dependencies_map.json"
         with open(map_file_path, "w") as outfile:
             json.dump(updated_dependencies_map, outfile, indent=4)
 
 
 
 def create_release():
```

### Comparing `domino-py-0.3.0/domino/cli/utils/platform.py` & `domino-py-0.4.0/domino/cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/client/airflow_client.py` & `domino-py-0.4.0/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/client/domino_backend_client.py` & `domino-py-0.4.0/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/client/fs_client.py` & `domino-py-0.4.0/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/client/github_rest_client.py` & `domino-py-0.4.0/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/client/local_files_client.py` & `domino-py-0.4.0/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/client/s3_client.py` & `domino-py-0.4.0/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/custom_operators/docker_operator.py` & `domino-py-0.4.0/domino/custom_operators/docker_operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,35 +56,35 @@
                 *mounts,
             ],
             environment=self.environment,
         )
     
     def _set_base_env_vars(self):
         self.environment = {
-            "DOMINO_DOCKER_PIECE": self.running_piece_name,
-            "DOMINO_DOCKER_INSTANTIATE_PIECE_KWARGS": str({
+            "DOMINO_PIECE": self.running_piece_name,
+            "DOMINO_INSTANTIATE_PIECE_KWARGS": str({
                 "deploy_mode": self.deploy_mode,
                 "task_id": self.task_id,
                 "dag_id": self.running_dag_id,
             }),
-            "DOMINO_DOCKER_RUN_PIECE_KWARGS": str(self.piece_input_kwargs),
+            "DOMINO_RUN_PIECE_KWARGS": str(self.piece_input_kwargs),
             "DOMINO_WORKFLOW_SHARED_STORAGE": self.workflow_shared_storage.json() if self.workflow_shared_storage else "",
             "AIRFLOW_CONTEXT_EXECUTION_DATETIME": "{{ dag_run.logical_date | ts_nodash }}",
             "AIRFLOW_CONTEXT_DAG_RUN_ID": "{{ run_id }}",
         }
 
     @staticmethod
     def _get_upstream_xcom_data_from_task_ids(task_ids: list, context: 'Context'):
         upstream_xcoms_data = dict()
         for tid in task_ids:
             upstream_xcoms_data[tid] = context['ti'].xcom_pull(task_ids=tid)
         return upstream_xcoms_data
 
     def _update_piece_kwargs_with_upstream_xcom(self, upstream_xcoms_data: dict):
-        #domino_docker_run_piece_kwargs = self.environment.get('DOMINO_DOCKER_RUN_PIECE_KWARGS')
+        #domino_run_piece_kwargs = self.environment.get('DOMINO_RUN_PIECE_KWARGS')
         if not self.piece_input_kwargs:
             self.piece_input_kwargs = dict()
         
         updated_op_kwargs = dict()
         for k, v in self.piece_input_kwargs.items():
             if isinstance(v, dict) and v.get("type", None) == "fromUpstream":
                 upstream_task_id = v.get("upstream_task_id")
@@ -93,15 +93,15 @@
                 updated_op_kwargs[k] = output_value
                 if upstream_task_id not in self.shared_storage_upstream_ids_list:
                     self.shared_storage_upstream_ids_list.append(upstream_task_id)
                 continue
             updated_op_kwargs[k] = v
         self.piece_input_kwargs = updated_op_kwargs
         self.environment['AIRFLOW_UPSTREAM_TASKS_IDS_SHARED_STORAGE'] = str(self.shared_storage_upstream_ids_list)
-        self.environment['DOMINO_DOCKER_RUN_PIECE_KWARGS'] = str(self.piece_input_kwargs)
+        self.environment['DOMINO_RUN_PIECE_KWARGS'] = str(self.piece_input_kwargs)
     
 
     def _prepare_execute_environment(self, context: Context):
         """ 
         Prepare execution with the following configurations:
         - pass extra arguments and configuration as environment variables to the pod
         - add shared storage sidecar container to the pod - if shared storage is FUSE based
@@ -112,15 +112,15 @@
         self.environment['AIRFLOW_UPSTREAM_TASKS_IDS'] = str(upstream_task_ids)
         self.environment['DOMINO_WORKFLOW_SHARED_STORAGE'] = str(self.workflow_shared_storage.source.name) if self.workflow_shared_storage else None
     
         # Save updated piece input kwargs with upstream data to environment variable
         upstream_xcoms_data = self._get_upstream_xcom_data_from_task_ids(task_ids=upstream_task_ids, context=context)
         self._update_piece_kwargs_with_upstream_xcom(upstream_xcoms_data=upstream_xcoms_data)
         piece_secrets = self._get_piece_secrets(piece_repository_id=self.repository_id, piece_name=self.running_piece_name)
-        self.environment['DOMINO_DOCKER_PIECE_SECRETS'] = str(piece_secrets)
+        self.environment['DOMINO_PIECE_SECRETS'] = str(piece_secrets)
         dag_id = context["dag_run"].dag_id
         dag_run_id = context['run_id']
         dag_run_id_path = dag_run_id.replace("-", "_").replace(".", "_").replace(" ", "_").replace(":", "_").replace("+", "_")
         self.workflow_run_subpath = f"{dag_id}/{dag_run_id_path}"
         self.environment['DOMINO_WORKFLOW_RUN_SUBPATH'] = self.workflow_run_subpath
```

### Comparing `domino-py-0.3.0/domino/custom_operators/external_python_operator.py` & `domino-py-0.4.0/domino/custom_operators/external_python_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         piece_secrets = {
             e.get('name'): e.get('value') 
             for e in secrets_response.json()
         }
         return piece_secrets
 
     def _update_piece_kwargs_with_upstream_xcom(self, upstream_xcoms_data: dict):
-        #domino_k8s_run_op_kwargs = [var for var in self.env_vars if getattr(var, 'name', None) == 'DOMINO_K8S_RUN_PIECE_KWARGS']
-        #domino_k8s_run_piece_kwargs = self.piece_kwargs
+        #domino_run_op_kwargs = [var for var in self.env_vars if getattr(var, 'name', None) == 'DOMINO_RUN_PIECE_KWARGS']
+        #domino_run_piece_kwargs = self.piece_kwargs
         if not self.piece_kwargs:
             self.piece_kwargs = dict()
 
         # Update Operator kwargs with upstream tasks XCOM data
         # Also updates the list of upstream tasks for which we need to mount the results path
         updated_op_kwargs = dict()
         for k, v in self.piece_kwargs.items():
```

### Comparing `domino-py-0.3.0/domino/custom_operators/k8s_operator.py` & `domino-py-0.4.0/domino/custom_operators/k8s_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                 piece_name=self.workflow_shared_storage.default_piece_name,
             )
 
         self.workflow_shared_storage.source = self.workflow_shared_storage.source.name
         env_vars = {
             'DOMINO_WORKFLOW_SHARED_STORAGE': self.workflow_shared_storage.json() if self.workflow_shared_storage else "",
             'DOMINO_WORKFLOW_SHARED_STORAGE_SECRETS': str(storage_piece_secrets),
-            'DOMINO_K8S_INSTANTIATE_PIECE_KWARGS': str(self.task_env_vars.get('DOMINO_K8S_INSTANTIATE_PIECE_KWARGS')),
+            'DOMINO_INSTANTIATE_PIECE_KWARGS': str(self.task_env_vars.get('DOMINO_INSTANTIATE_PIECE_KWARGS')),
             'DOMINO_WORKFLOW_RUN_SUBPATH': self.workflow_run_subpath,
             'AIRFLOW_UPSTREAM_TASKS_IDS_SHARED_STORAGE': str(self.shared_storage_upstream_ids_list),
         }
 
         self.shared_storage_sidecar_container_name = f"domino-shared-storage-sidecar-{self.task_id_replaced}"
         sidecar_container = k8s.V1Container(
             name=self.shared_storage_sidecar_container_name,
@@ -200,24 +200,24 @@
         piece_secrets = {
             e.get('name'): e.get('value') 
             for e in secrets_response.json()
         }
         return piece_secrets
 
     def _get_piece_kwargs_with_upstream_xcom(self, upstream_xcoms_data: dict):
-        domino_k8s_run_op_kwargs = [var for var in self.env_vars if getattr(var, 'name', None) == 'DOMINO_K8S_RUN_PIECE_KWARGS']
+        domino_k8s_run_op_kwargs = [var for var in self.env_vars if getattr(var, 'name', None) == 'DOMINO_RUN_PIECE_KWARGS']
         if not domino_k8s_run_op_kwargs:
             domino_k8s_run_op_kwargs = {
-                "name": "DOMINO_K8S_RUN_PIECE_KWARGS",
+                "name": "DOMINO_RUN_PIECE_KWARGS",
                 "value": {}
             }
         else:
             domino_k8s_run_op_kwargs = domino_k8s_run_op_kwargs[0]
             domino_k8s_run_op_kwargs = {
-                "name": "DOMINO_K8S_RUN_PIECE_KWARGS",
+                "name": "DOMINO_RUN_PIECE_KWARGS",
                 "value": ast.literal_eval(domino_k8s_run_op_kwargs.value)
             }
         
         # Update Operator kwargs with upstream tasks XCOM data
         # Also updates the list of upstream tasks for which we need to mount the results path
         updated_op_kwargs = dict()
         for k, v in domino_k8s_run_op_kwargs.get('value').items():
@@ -318,20 +318,20 @@
             'value': str(self.workflow_shared_storage.source.name) if self.workflow_shared_storage else None,
             'value_from': None
         })
 
         # Save updated piece input kwargs with upstream data to environment variable
         upstream_xcoms_data = self._get_upstream_xcom_data_from_task_ids(task_ids=upstream_task_ids, context=context)
         domino_k8s_run_op_kwargs = self._get_piece_kwargs_with_upstream_xcom(upstream_xcoms_data=upstream_xcoms_data)        
-        self._update_env_var_value_from_name(name='DOMINO_K8S_RUN_PIECE_KWARGS', value=str(domino_k8s_run_op_kwargs))
+        self._update_env_var_value_from_name(name='DOMINO_RUN_PIECE_KWARGS', value=str(domino_k8s_run_op_kwargs))
         
         # Add pieces secrets to environment variables
         piece_secrets = self._get_piece_secrets(piece_repository_id=self.repository_id, piece_name=self.running_piece_name)
         self.env_vars.append({
-            "name": "DOMINO_K8S_PIECE_SECRETS",
+            "name": "DOMINO_PIECE_SECRETS",
             "value": str(piece_secrets),
             "value_from": None
         })
 
         # Include workflow run subpath from dag run id, taken from context
         dag_id = context["dag_run"].dag_id
         dag_run_id = context['run_id']
```

### Comparing `domino-py-0.3.0/domino/custom_operators/python_operator.py` & `domino-py-0.4.0/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/custom_operators/sidecar/logger.py` & `domino-py-0.4.0/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/custom_operators/sidecar/mount.py` & `domino-py-0.4.0/domino/custom_operators/sidecar/mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self):
         self.logger = get_configured_logger(self.__class__.__name__)
         self.mount_base_path = "/home/shared_storage"
         self.config_file_path = "/.config/rclone/rclone.conf"
         self.parser = self._get_parser()
         self._set_shared_storage()
         self._set_remote_base_folder_path()
-        self.task_id = ast.literal_eval(os.environ.get("DOMINO_K8S_INSTANTIATE_PIECE_KWARGS"))["task_id"]
+        self.task_id = ast.literal_eval(os.environ.get("DOMINO_INSTANTIATE_PIECE_KWARGS"))["task_id"]
         self.workflow_run_subpath = os.environ.get("DOMINO_WORKFLOW_RUN_SUBPATH")
 
         self.shared_storage_function_map = {
             "gcs": self._setup_gcs_shared_storage_config,
             "aws_s3": self._setup_aws_s3_shared_storage_config,
             "local": self._setup_local_shared_storage_config
         }
```

### Comparing `domino-py-0.3.0/domino/exceptions/exceptions.py` & `domino-py-0.4.0/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/logger.py` & `domino-py-0.4.0/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/schemas/piece_metadata.py` & `domino-py-0.4.0/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/schemas/shared_storage.py` & `domino-py-0.4.0/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/scripts/create_docker_compose_file.py` & `domino-py-0.4.0/domino/scripts/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/scripts/docker_compose_constants.py` & `domino-py-0.4.0/domino/scripts/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/scripts/docker_compose_scripts.py` & `domino-py-0.4.0/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/scripts/load_piece.py` & `domino-py-0.4.0/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/scripts/piece_dry_run.py` & `domino-py-0.4.0/domino/scripts/deprecated_piece_dry_run.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/scripts/run_piece_bash.py` & `domino-py-0.4.0/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino/scripts/run_piece_docker.py` & `domino-py-0.4.0/domino/scripts/run_piece_docker.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import ast
 import json
 
 
 def run_piece():
      # Import Operator from File System, already configured with metadata
-    piece_name = os.getenv("DOMINO_DOCKER_PIECE")
+    piece_name = os.getenv("DOMINO_PIECE")
 
     pieces_repository_copy_path = Path("domino/pieces_repository").resolve()
     pieces_folder_path = pieces_repository_copy_path / "pieces"
     compiled_metadata_path = pieces_repository_copy_path / ".domino/compiled_metadata.json"
 
     with open(str(compiled_metadata_path), "r") as f:
         compiled_metadata = json.load(f)
@@ -24,27 +24,20 @@
 
     piece_input_model_class, piece_output_model_class, piece_secrets_model_class = load_piece_models_from_path(
         pieces_folder_path=pieces_folder_path,
         piece_name=piece_name
     )
 
     # Instantiate Operator
-    instantiate_op_dict = ast.literal_eval(os.getenv("DOMINO_DOCKER_INSTANTIATE_PIECE_KWARGS"))
+    instantiate_op_dict = ast.literal_eval(os.getenv("DOMINO_INSTANTIATE_PIECE_KWARGS"))
     piece_object = piece_class(**instantiate_op_dict)
 
-    # Get relevant airflow context from ENV
-    airflow_context = {
-        "execution_datetime": os.getenv('AIRFLOW_CONTEXT_EXECUTION_DATETIME', "123456789"),
-        "dag_run_id": os.getenv('AIRFLOW_CONTEXT_DAG_RUN_ID', "123456789"),
-    }
-
     # Run Operator
-    run_piece_input_kwargs = ast.literal_eval(os.getenv("DOMINO_DOCKER_RUN_PIECE_KWARGS"))
+    run_piece_input_kwargs = ast.literal_eval(os.getenv("DOMINO_RUN_PIECE_KWARGS"))
     piece_object.run_piece_function(
-        airflow_context=airflow_context,
-        op_kwargs=run_piece_input_kwargs,        
+        piece_input_data=run_piece_input_kwargs,        
         piece_input_model=piece_input_model_class, 
         piece_output_model=piece_output_model_class, 
         piece_secrets_model=piece_secrets_model_class,
     )
 
     return None
```

### Comparing `domino-py-0.3.0/domino/task.py` & `domino-py-0.4.0/domino/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,21 +84,21 @@
         # - https://airflow.apache.org/docs/apache-airflow/1.10.14/_api/airflow/contrib/operators/kubernetes_pod_operator/index.html
         # - https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html
         # - https://www.astronomer.io/guides/templating/
         # - good example: https://github.com/apache/airflow/blob/main/tests/system/providers/cncf/kubernetes/example_kubernetes.py
         # - commands HAVE to go in a list object: https://stackoverflow.com/a/55149915/11483674
         elif self.deploy_mode in ["local-k8s", "local-k8s-dev", "prod"]:
             container_env_vars = {
-                "DOMINO_K8S_PIECE": self.piece["name"],
-                "DOMINO_K8S_INSTANTIATE_PIECE_KWARGS": str({
+                "DOMINO_PIECE": self.piece["name"],
+                "DOMINO_INSTANTIATE_PIECE_KWARGS": str({
                     "deploy_mode": self.deploy_mode,
                     "task_id": self.task_id,
                     "dag_id": self.dag_id,
                 }),
-                "DOMINO_K8S_RUN_PIECE_KWARGS": str(piece_input_kwargs),
+                "DOMINO_RUN_PIECE_KWARGS": str(piece_input_kwargs),
                 "DOMINO_WORKFLOW_SHARED_STORAGE": self.workflow_shared_storage.json() if self.workflow_shared_storage else "",
                 "AIRFLOW_CONTEXT_EXECUTION_DATETIME": "{{ dag_run.logical_date | ts_nodash }}",
                 "AIRFLOW_CONTEXT_DAG_RUN_ID": "{{ run_id }}",
             }
             base_container_resources_model = ContainerResourcesModel(
                 requests={
                     "cpu": "100m",
```

### Comparing `domino-py-0.3.0/domino/utils/piece_generator.py` & `domino-py-0.4.0/domino/utils/piece_generator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.3.0/domino_py.egg-info/PKG-INFO` & `domino-py-0.4.0/domino_py.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,193 +1,205 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python package for the Domino platform
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
-Description: 
-        
-        <p align="center">
+Description: <p align="center">
           <img src="https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/logo.png" width="450" title="Domino">
         </p>
+        <p align="center"><i>Build amazing ideas, piece by piece.</i></p>
         <p align="center">
           <a href="https://pypi.org/project/domino-py">
             <img src="https://img.shields.io/pypi/v/domino-py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">
           </a>
           <a href="https://artifacthub.io/packages/helm/domino/domino">
             <img src="https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino">
           </a>
           <a href="https://domino-py.readthedocs.io/en/latest/">
             <img alt="Read the Docs" src="https://img.shields.io/readthedocs/domino-py?label=Docs&logo=Read%20the%20Docs&logoColor=white">
           </a>
         </p>
         
+        <br>
+        
+        ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/7_create_workflow.gif)
         
         # Table of contents
         - [About](#about)
         - [Quick start](#quick-start)
         - [GUI](#gui)
-        - [REST](#rest)
         - [Pieces](#pieces)
+        - [REST](#rest)
+        - [Credits](#credits)
         
         <br>
         
         # About
         Domino is an open source workflow management platform, with:
         
-        - an intuitive [Graphical User Interface](#gui) that facilitates creating, editing and monitoring any type of Workflow, from data processing to machine learning
-        - a [REST API](#rest) that controls a running Apache Airflow instance
-        - a standard way of writing and publishing functional [Pieces](#pieces), which follows good practices for data modeling, documentation and distribution
+        - :desktop_computer: an intuitive [Graphical User Interface](#gui) that facilitates creating, editing and monitoring any type of Workflow, from data processing to machine learning
+        - :package: a standard way of writing and publishing functional [Pieces](#pieces), which follows good practices for data modeling, documentation and distribution
+        - :gear: a [REST API](#rest) that controls a running Apache Airflow instance
         
         
         Creating Workflows in the GUI is as simple as dragging and dropping Pieces to the canvas, and connecting them. The user can also schedule the Workflow to run periodically, at a specific date/time, or trigger it manually. The monitoring page shows the status of each Workflow Piece in real time, including the logs and results of each run.
         
+        Pieces are functional units that can be reused in multiple Workflows. Pieces can execute anything that can be written in Python, and can be easily distributed and installed directly from Github repositories to be used in Domino Workflows.
+        
         Every Domino Workflow corresponds to an Apache Airflow DAG, and each Piece corresponds to an Airflow task. Domino controls an Airflow instance, which is responsible for executing, scheduling and monitoring the Workflows (DAGs).
         
-        Pieces are functional units that can be reused in multiple Workflows. Pieces can execute anything that can be written in Python, and can be easily distributed and installed directly from Github repositories to be used in Domino Workflows.
+        You can think of Domino as Airflow with superpowers:
+        
+        - :desktop_computer: create highly complex Workflows with simple point-and-click and drag-and-drop operations, in an user-friendly GUI
+        - :package: make use of Pieces developed by other people, share and reuse your own Pieces
+        - :busts_in_silhouette: collaborate in groups to edit and monitor Workflows
+        - :chart_with_upwards_trend: experience a cleaner and more intuitive GUI for viewing Workflows results, including logs and richer reports with images and tables
+        - :minidisc: shared storage for tasks in the same workflow
+        - :arrows_counterclockwise: use gitSync to sync DAGs from files stored in a Git repository
+        - :wheel_of_dharma: scalable, Kubernetes-native platform
+        - :battery: powered by Apache Airflow for top-tier workflows scheduling and monitoring
         
         <br>
         
         # Quick start
         
         The Domino Python package can be installed via pip. We reccommend you install Domino in a separate Python environment.
         
         ```bash
         pip install domino-py
         ```
         
-        You can then use Domino command line interface to easily run the Domino platform locally. Go to a new, empty directory and run the following command:
+        You can then use Domino command line interface to easily run the Domino platform locally (requires Docker compose). Go to a new, empty directory and run the following command:
         
         ```bash
         domino platform run-compose
         ```
         
-        This is a convenience command that will:
-        - Create the necessary folder structure for Domino and Airflow processes
-        - Create a docker-compose.yaml file
-        - Run the docker compose up command
-        
-        This command might take up to a few minutes to execute, since it will download and run all the necessary docker images. If everything worked as expected, after all processes started successfully you should be able to navigate to `localhost:3000` to access the Domino frontend service.
+        After all processes started successfully, navigate to `localhost:3000` to access the Domino frontend service.
         
         Running the Domino platform locally with Docker compose is useful for development and testing purposes. For production environments, we recommend you install Domino in a Kubernetes cluster:
         - Running Domino in a [local Kubernetes cluster with Kind](https://domino-py.readthedocs.io/en/latest/pages/platform.html)
         - Running Domino in a [remote Kubernetes cluster](https://domino-py.readthedocs.io/en/latest/pages/deployment_cloud.html)
         
         <br>
         
         # GUI
         The Domino frontend service is a React application that provides the GUI for easily creating, editing and monitoring Workflows. Here are some of its features:
         
         <details>
           <summary>
+            <strong>Access authentication</strong>
+          </summary>
+          Sign up and login to use the Domino platform. <br></br>
+        
+          ![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/1_sign_up.gif)
+        
+        </details>
+        
+        <details>
+          <summary>
+            <strong>Create Workspaces</strong>
+          </summary>
+          Create new Workspaces and add your github access token. <br></br>
+        
+          ![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/2_create_workspace_and_token.gif)
+        
+        </details>
+        
+        <details>
+          <summary>
             <strong>Install Pieces repositories</strong>
           </summary>
           Install bundles of Pieces to your Domino Workspaces direclty from Github repositories, and use them in your Workflows. <br></br>
         
-          ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/3_install_pieces.gif)
+          ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_install_pieces.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Create Workflows</strong>
           </summary>
           Create Workflows by dragging and dropping Pieces to the canvas, and connecting them. <br></br>
         
-          ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/4_create_workflow.gif)
+          ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/7_create_workflow.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Edit Pieces</strong>
           </summary>
           Edit Pieces by changing their input. Outputs from upstream Pieces are automatically available as inputs for downstream Pieces. Pieces can pass forward any type of data, from simple strings to heavy files, all automatically handled by Domino shared storage system. <br></br>
         
-          ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/5_edit_pieces.gif)
+          ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/8_edit_pieces.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Schedule Workflows</strong>
           </summary>
           Schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
         
-          ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_edit_workflow.gif)
+          ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/9_edit_workflow.gif)
         </details>
         
         <details>
           <summary>
             <strong>Monitor Workflows</strong>
           </summary>
           Monitor Workflows in real time, including the status of each Piece, the logs and results of each run. <br></br>
         
-          ![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/7_monitor_workflow.gif)
+          ![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/10_monitor_workflow.gif)
         
         </details>
         
         <br>
         
-        # REST
-        The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
-        
-        - executing operations requested by the frontend service
-        - interacting with the Airflow instance, including triggering, creating, editing and deleting Workflows (DAGs)
-        - interacting with the Domino Database
-        
-        The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://domino-py.readthedocs.io/en/latest/pages/rest.html).
-        
-        <br>
-        
         # Pieces
         Pieces are the secret sauce of Domino, they are functional units that can be distributed and reused in multiple Workflows. Domino Pieces are special because they:
         
-        - can execute anything written in Python, heavy-weight (e.g. Machine Learning) as well as light-weight (e.g. sending emails) tasks
-        - have well defined data models for inputs, outputs and secrets
-        - run in isolated execution environments (Docker containers)
-        - are organized in repositories, for easy distribution and installation
+        - :snake: can execute anything written in Python, heavy-weight (e.g. Machine Learning) as well as light-weight (e.g. sending emails) tasks
+        - :traffic_light: have well defined data models for inputs, outputs and secrets
+        - :package: run in self-contained and isolated execution environments (Docker containers)
+        - :gear: are immutable, guaranteeing reproducibility of your workflows
+        - :octocat: are organized in git repositories, for easy packaging, distribution and installation
+        - :bookmark_tabs: are properly versioned, tested and documented
+        - :zap: are plug-and-play and versatile, can be easily incorporated in any workflow
+        
+        It is very easy to create and share your own Pieces:
+        
+        - :one: write your Python function
+        - :two: define its data types (input, output and secrets)
+        - :three: define its dependencies (requirements.txt or Dockerfile)
+        - :four: publish it in a repository (public or private)
         
-        To facilitate the creation of Pieces, we provide a [template repository](https://github.com/Tauffer-Consulting/domino_pieces_repository_template) with the basic file structure and examples for data models, metadata, source code and dependencies.
+        The [Pieces repository template](https://github.com/Tauffer-Consulting/domino_pieces_repository_template) provides the basic structure, example files and automatic actions for a seamless Pieces creation experience.
         
-        In short, each Piece is a folder containing the following files:
-        - A `piece.py` file with the source code to be executed
-        - A `models.py` file containing the Pydantic models that define the input, output and secrets for the Piece
-        - A `metadata.json` file containing the Piece's metadata, including dependencies and GUI style
+        Read more in the [Pieces documentation](https://domino-py.readthedocs.io/en/latest/pages/pieces.html).
         
-        A repository contains multiples Pieces. Pieces with the same dependencies are automatically grouped together in a dependency group, and each dependency group is built into a Docker image. The Docker images are the self contained execution environments containing the Piece's source code and with all the necessary dependencies installed.
         
-        The Docker images are automatically built and published in the same Github repository as the Pieces. This organization makes it straightforward to install Pieces respositories in Domino Workspaces, to be used in Workflows.
-        
-        Read more about Pieces and how to create them in the [Pieces documentation](https://domino-py.readthedocs.io/en/latest/pages/pieces.html).
+        <br>
         
+        # REST
+        The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
         
-        <br>
+        - executing operations requested by the frontend service
+        - interacting with the Airflow instance, including triggering, creating, editing and deleting Workflows (DAGs)
+        - interacting with the Domino Database
         
-        # Platform
+        The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://domino-py.readthedocs.io/en/latest/pages/rest.html).
         
-        ## GitSync
-        A good practice when running Airflow in a Kubernetes cluster is to use a GitSync container to sync DAGs from a Git repository to the Airflow services. 
+        <br>
         
-        ## Shared storage structure
-        Shared workflow data could be stored in a remote source (e.g. S3 bucket) or locally (for dev and tests only).
+        # Credits
+        Domino is developed and maintained by [Tauffer Consulting](https://www.taufferconsulting.com/).
         
-        ```
-        /shared_storage
-        ..../{workflow-id}
-        ......../{run-id}
-        ............/{task-id}
-        ................/results
-        ..................../log.txt
-        ..................../result.npy
-        ..................../result.html
-        ................/report
-        ................/xcom_out
-        ..................../xcom_out.json
-        ```
 Keywords: domino,airflow,gui
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: airflow
```

#### html2text {}

```diff
@@ -1,110 +1,117 @@
-Metadata-Version: 2.1 Name: domino-py Version: 0.3.0 Summary: Python package
+Metadata-Version: 2.1 Name: domino-py Version: 0.4.0 Summary: Python package
 for the Domino platform Home-page: UNKNOWN Author: Luiz Tauffer and Vinicius
 Vaz Author-email: luiz@taufferconsulting.com License: UNKNOWN Description:
    [https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/
                                    logo.png]
+                     Build amazing ideas, piece by piece.
                     [https://img.shields.io/pypi/v/domino-
   py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20] [https://
  img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino]
                                 [Read_the_Docs]
-# Table of contents - [About](#about) - [Quick start](#quick-start) - [GUI]
-(#gui) - [REST](#rest) - [Pieces](#pieces)
-# About Domino is an open source workflow management platform, with: - an
-intuitive [Graphical User Interface](#gui) that facilitates creating, editing
-and monitoring any type of Workflow, from data processing to machine learning -
-a [REST API](#rest) that controls a running Apache Airflow instance - a
-standard way of writing and publishing functional [Pieces](#pieces), which
-follows good practices for data modeling, documentation and distribution
-Creating Workflows in the GUI is as simple as dragging and dropping Pieces to
-the canvas, and connecting them. The user can also schedule the Workflow to run
-periodically, at a specific date/time, or trigger it manually. The monitoring
-page shows the status of each Workflow Piece in real time, including the logs
-and results of each run. Every Domino Workflow corresponds to an Apache Airflow
-DAG, and each Piece corresponds to an Airflow task. Domino controls an Airflow
-instance, which is responsible for executing, scheduling and monitoring the
-Workflows (DAGs). Pieces are functional units that can be reused in multiple
-Workflows. Pieces can execute anything that can be written in Python, and can
-be easily distributed and installed directly from Github repositories to be
-used in Domino Workflows.
+
+![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/7_create_workflow.gif) # Table of contents -
+[About](#about) - [Quick start](#quick-start) - [GUI](#gui) - [Pieces](#pieces)
+- [REST](#rest) - [Credits](#credits)
+# About Domino is an open source workflow management platform, with: - :
+desktop_computer: an intuitive [Graphical User Interface](#gui) that
+facilitates creating, editing and monitoring any type of Workflow, from data
+processing to machine learning - :package: a standard way of writing and
+publishing functional [Pieces](#pieces), which follows good practices for data
+modeling, documentation and distribution - :gear: a [REST API](#rest) that
+controls a running Apache Airflow instance Creating Workflows in the GUI is as
+simple as dragging and dropping Pieces to the canvas, and connecting them. The
+user can also schedule the Workflow to run periodically, at a specific date/
+time, or trigger it manually. The monitoring page shows the status of each
+Workflow Piece in real time, including the logs and results of each run. Pieces
+are functional units that can be reused in multiple Workflows. Pieces can
+execute anything that can be written in Python, and can be easily distributed
+and installed directly from Github repositories to be used in Domino Workflows.
+Every Domino Workflow corresponds to an Apache Airflow DAG, and each Piece
+corresponds to an Airflow task. Domino controls an Airflow instance, which is
+responsible for executing, scheduling and monitoring the Workflows (DAGs). You
+can think of Domino as Airflow with superpowers: - :desktop_computer: create
+highly complex Workflows with simple point-and-click and drag-and-drop
+operations, in an user-friendly GUI - :package: make use of Pieces developed by
+other people, share and reuse your own Pieces - :busts_in_silhouette:
+collaborate in groups to edit and monitor Workflows - :
+chart_with_upwards_trend: experience a cleaner and more intuitive GUI for
+viewing Workflows results, including logs and richer reports with images and
+tables - :minidisc: shared storage for tasks in the same workflow - :
+arrows_counterclockwise: use gitSync to sync DAGs from files stored in a Git
+repository - :wheel_of_dharma: scalable, Kubernetes-native platform - :battery:
+powered by Apache Airflow for top-tier workflows scheduling and monitoring
 # Quick start The Domino Python package can be installed via pip. We reccommend
 you install Domino in a separate Python environment. ```bash pip install
 domino-py ``` You can then use Domino command line interface to easily run the
-Domino platform locally. Go to a new, empty directory and run the following
-command: ```bash domino platform run-compose ``` This is a convenience command
-that will: - Create the necessary folder structure for Domino and Airflow
-processes - Create a docker-compose.yaml file - Run the docker compose up
-command This command might take up to a few minutes to execute, since it will
-download and run all the necessary docker images. If everything worked as
-expected, after all processes started successfully you should be able to
-navigate to `localhost:3000` to access the Domino frontend service. Running the
-Domino platform locally with Docker compose is useful for development and
-testing purposes. For production environments, we recommend you install Domino
-in a Kubernetes cluster: - Running Domino in a [local Kubernetes cluster with
-Kind](https://domino-py.readthedocs.io/en/latest/pages/platform.html) - Running
-Domino in a [remote Kubernetes cluster](https://domino-py.readthedocs.io/en/
-latest/pages/deployment_cloud.html)
+Domino platform locally (requires Docker compose). Go to a new, empty directory
+and run the following command: ```bash domino platform run-compose ``` After
+all processes started successfully, navigate to `localhost:3000` to access the
+Domino frontend service. Running the Domino platform locally with Docker
+compose is useful for development and testing purposes. For production
+environments, we recommend you install Domino in a Kubernetes cluster: -
+Running Domino in a [local Kubernetes cluster with Kind](https://domino-
+py.readthedocs.io/en/latest/pages/platform.html) - Running Domino in a [remote
+Kubernetes cluster](https://domino-py.readthedocs.io/en/latest/pages/
+deployment_cloud.html)
 # GUI The Domino frontend service is a React application that provides the GUI
 for easily creating, editing and monitoring Workflows. Here are some of its
-features:   Install Pieces repositories  Install bundles of Pieces to your
-Domino Workspaces direclty from Github repositories, and use them in your
-Workflows.
+features:   Access authentication  Sign up and login to use the Domino
+platform.
+![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/1_sign_up.gif)    Create Workspaces
+Create new Workspaces and add your github access token.
+![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/2_create_workspace_and_token.gif)
+Install Pieces repositories  Install bundles of Pieces to your Domino
+Workspaces direclty from Github repositories, and use them in your Workflows.
 ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
-main/docs/source/_static/media/3_install_pieces.gif)    Create Workflows
+main/docs/source/_static/media/6_install_pieces.gif)    Create Workflows
 Create Workflows by dragging and dropping Pieces to the canvas, and connecting
 them.
 ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
-main/docs/source/_static/media/4_create_workflow.gif)    Edit Pieces  Edit
+main/docs/source/_static/media/7_create_workflow.gif)    Edit Pieces  Edit
 Pieces by changing their input. Outputs from upstream Pieces are automatically
 available as inputs for downstream Pieces. Pieces can pass forward any type of
 data, from simple strings to heavy files, all automatically handled by Domino
 shared storage system.
 ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
-main/docs/source/_static/media/5_edit_pieces.gif)    Schedule Workflows
+main/docs/source/_static/media/8_edit_pieces.gif)    Schedule Workflows
 Schedule Workflows to run periodically, at a specific date/time, or trigger
 them manually.
 ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/
-domino/main/docs/source/_static/media/6_edit_workflow.gif)    Monitor Workflows
+domino/main/docs/source/_static/media/9_edit_workflow.gif)    Monitor Workflows
 Monitor Workflows in real time, including the status of each Piece, the logs
 and results of each run.
 ![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/
-domino/main/docs/source/_static/media/7_monitor_workflow.gif)
+domino/main/docs/source/_static/media/10_monitor_workflow.gif)
+# Pieces Pieces are the secret sauce of Domino, they are functional units that
+can be distributed and reused in multiple Workflows. Domino Pieces are special
+because they: - :snake: can execute anything written in Python, heavy-weight
+(e.g. Machine Learning) as well as light-weight (e.g. sending emails) tasks - :
+traffic_light: have well defined data models for inputs, outputs and secrets -
+:package: run in self-contained and isolated execution environments (Docker
+containers) - :gear: are immutable, guaranteeing reproducibility of your
+workflows - :octocat: are organized in git repositories, for easy packaging,
+distribution and installation - :bookmark_tabs: are properly versioned, tested
+and documented - :zap: are plug-and-play and versatile, can be easily
+incorporated in any workflow It is very easy to create and share your own
+Pieces: - :one: write your Python function - :two: define its data types
+(input, output and secrets) - :three: define its dependencies (requirements.txt
+or Dockerfile) - :four: publish it in a repository (public or private) The
+[Pieces repository template](https://github.com/Tauffer-Consulting/
+domino_pieces_repository_template) provides the basic structure, example files
+and automatic actions for a seamless Pieces creation experience. Read more in
+the [Pieces documentation](https://domino-py.readthedocs.io/en/latest/pages/
+pieces.html).
 # REST The Backend service is a REST API that controls a running Apache Airflow
 instance. It is responsible for: - executing operations requested by the
 frontend service - interacting with the Airflow instance, including triggering,
 creating, editing and deleting Workflows (DAGs) - interacting with the Domino
 Database The REST service is written in Python, using the FastAPI framework.
 Read more about it in the [REST documentation](https://domino-
 py.readthedocs.io/en/latest/pages/rest.html).
-# Pieces Pieces are the secret sauce of Domino, they are functional units that
-can be distributed and reused in multiple Workflows. Domino Pieces are special
-because they: - can execute anything written in Python, heavy-weight (e.g.
-Machine Learning) as well as light-weight (e.g. sending emails) tasks - have
-well defined data models for inputs, outputs and secrets - run in isolated
-execution environments (Docker containers) - are organized in repositories, for
-easy distribution and installation To facilitate the creation of Pieces, we
-provide a [template repository](https://github.com/Tauffer-Consulting/
-domino_pieces_repository_template) with the basic file structure and examples
-for data models, metadata, source code and dependencies. In short, each Piece
-is a folder containing the following files: - A `piece.py` file with the source
-code to be executed - A `models.py` file containing the Pydantic models that
-define the input, output and secrets for the Piece - A `metadata.json` file
-containing the Piece's metadata, including dependencies and GUI style A
-repository contains multiples Pieces. Pieces with the same dependencies are
-automatically grouped together in a dependency group, and each dependency group
-is built into a Docker image. The Docker images are the self contained
-execution environments containing the Piece's source code and with all the
-necessary dependencies installed. The Docker images are automatically built and
-published in the same Github repository as the Pieces. This organization makes
-it straightforward to install Pieces respositories in Domino Workspaces, to be
-used in Workflows. Read more about Pieces and how to create them in the [Pieces
-documentation](https://domino-py.readthedocs.io/en/latest/pages/pieces.html).
-# Platform ## GitSync A good practice when running Airflow in a Kubernetes
-cluster is to use a GitSync container to sync DAGs from a Git repository to the
-Airflow services. ## Shared storage structure Shared workflow data could be
-stored in a remote source (e.g. S3 bucket) or locally (for dev and tests only).
-``` /shared_storage ..../{workflow-id} ......../{run-id} ............/{task-id}
-................/results ..................../log.txt ..................../
-result.npy ..................../result.html ................/report
-................/xcom_out ..................../xcom_out.json ``` Keywords:
-domino,airflow,gui Platform: UNKNOWN Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: airflow
+# Credits Domino is developed and maintained by [Tauffer Consulting](https://
+www.taufferconsulting.com/). Keywords: domino,airflow,gui Platform: UNKNOWN
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+airflow
```

### Comparing `domino-py-0.3.0/domino_py.egg-info/SOURCES.txt` & `domino-py-0.4.0/domino_py.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -25,31 +25,36 @@
 domino/custom_operators/k8s_operator.py
 domino/custom_operators/python_operator.py
 domino/custom_operators/sidecar/__init__.py
 domino/custom_operators/sidecar/logger.py
 domino/custom_operators/sidecar/mount.py
 domino/exceptions/__init__.py
 domino/exceptions/exceptions.py
+domino/models/__init__.py
+domino/models/output_modifier.py
 domino/schemas/__init__.py
 domino/schemas/container_resources.py
 domino/schemas/deploy_mode.py
 domino/schemas/display_result.py
 domino/schemas/from_upstream.py
 domino/schemas/piece_metadata.py
 domino/schemas/shared_storage.py
 domino/scripts/__init__.py
 domino/scripts/build_docker_images_pieces.py
 domino/scripts/create_docker_compose_file.py
+domino/scripts/deprecated_piece_dry_run.py
 domino/scripts/docker_compose_constants.py
 domino/scripts/docker_compose_scripts.py
 domino/scripts/load_piece.py
-domino/scripts/piece_dry_run.py
 domino/scripts/run_piece_bash.py
 domino/scripts/run_piece_docker.py
-domino/scripts/run_piece_k8s.py
+domino/testing/__init__.py
+domino/testing/dry_run.py
+domino/testing/http_client.py
+domino/testing/http_server.py
 domino/utils/__init__.py
 domino/utils/metadata_default.py
 domino/utils/piece_generator.py
 domino/utils/workflow_shared_storage.py
 domino_py.egg-info/PKG-INFO
 domino_py.egg-info/SOURCES.txt
 domino_py.egg-info/dependency_links.txt
```

### Comparing `domino-py-0.3.0/setup.py` & `domino-py-0.4.0/setup.py`

 * *Files identical despite different names*

