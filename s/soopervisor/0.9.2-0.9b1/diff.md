# Comparing `tmp/soopervisor-0.9.2.tar.gz` & `tmp/soopervisor-0.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soopervisor-0.9.2.tar", last modified: Tue Jul 18 17:46:26 2023, max compression
+gzip compressed data, was "soopervisor-0.9b1.tar", last modified: Mon Sep 26 21:03:37 2022, max compression
```

## Comparing `soopervisor-0.9.2.tar` & `soopervisor-0.9b1.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.741766 soopervisor-0.9.2/
--rw-r--r--   0 eduardo    (501) staff       (20)     7136 2023-07-18 17:46:23.000000 soopervisor-0.9.2/CHANGELOG.rst
--rw-r--r--   0 eduardo    (501) staff       (20)    11355 2023-07-18 16:46:24.000000 soopervisor-0.9.2/LICENSE
--rw-r--r--   0 eduardo    (501) staff       (20)      121 2022-12-27 00:40:47.000000 soopervisor-0.9.2/MANIFEST.in
--rw-r--r--   0 eduardo    (501) staff       (20)    10930 2023-07-18 17:46:26.741829 soopervisor-0.9.2/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)     2969 2022-12-29 04:29:40.000000 soopervisor-0.9.2/README.rst
--rw-r--r--   0 eduardo    (501) staff       (20)      198 2022-12-27 00:40:47.000000 soopervisor-0.9.2/pyproject.toml
--rw-r--r--   0 eduardo    (501) staff       (20)      201 2023-07-18 17:46:26.742056 soopervisor-0.9.2/setup.cfg
--rw-r--r--   0 eduardo    (501) staff       (20)     3294 2023-07-18 17:45:20.000000 soopervisor-0.9.2/setup.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.735156 soopervisor-0.9.2/src/
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.737634 soopervisor-0.9.2/src/soopervisor/
--rw-r--r--   0 eduardo    (501) staff       (20)       22 2023-07-18 17:46:23.000000 soopervisor-0.9.2/src/soopervisor/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)       77 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/_format.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1047 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/_io.py
--rw-r--r--   0 eduardo    (501) staff       (20)    11714 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/abc.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.738464 soopervisor-0.9.2/src/soopervisor/airflow/
--rw-r--r--   0 eduardo    (501) staff       (20)        0 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/airflow/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      471 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/airflow/config.py
--rw-r--r--   0 eduardo    (501) staff       (20)     4755 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/airflow/export.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.738726 soopervisor-0.9.2/src/soopervisor/argo/
--rw-r--r--   0 eduardo    (501) staff       (20)        0 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/argo/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1904 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/argo/config.py
--rw-r--r--   0 eduardo    (501) staff       (20)     6061 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/argo/export.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.738813 soopervisor-0.9.2/src/soopervisor/assets/
--rw-r--r--   0 eduardo    (501) staff       (20)        0 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/__init__.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.739066 soopervisor-0.9.2/src/soopervisor/assets/airflow/
--rw-r--r--   0 eduardo    (501) staff       (20)      751 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/assets/airflow/bash.py
--rw-r--r--   0 eduardo    (501) staff       (20)      790 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/assets/airflow/docker.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1209 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/assets/airflow/kubernetes.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.739235 soopervisor-0.9.2/src/soopervisor/assets/argo/
--rw-r--r--   0 eduardo    (501) staff       (20)        0 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/argo/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      543 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/argo/template.yaml
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.739739 soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/
--rw-r--r--   0 eduardo    (501) staff       (20)      353 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/Dockerfile
--rw-r--r--   0 eduardo    (501) staff       (20)     1136 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/README.md
--rw-r--r--   0 eduardo    (501) staff       (20)      690 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/app.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1869 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/template.yaml
--rw-r--r--   0 eduardo    (501) staff       (20)     2749 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/test_aws_lambda.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.739834 soopervisor-0.9.2/src/soopervisor/assets/docker/
--rw-r--r--   0 eduardo    (501) staff       (20)      831 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/docker/Dockerfile
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.739928 soopervisor-0.9.2/src/soopervisor/assets/kubeflow/
--rw-r--r--   0 eduardo    (501) staff       (20)      737 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/kubeflow/Dockerfile
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.740026 soopervisor-0.9.2/src/soopervisor/assets/slurm/
--rw-r--r--   0 eduardo    (501) staff       (20)      228 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/assets/slurm/template.sh
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.740519 soopervisor-0.9.2/src/soopervisor/aws/
--rw-r--r--   0 eduardo    (501) staff       (20)        0 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/aws/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)    10305 2023-07-18 17:45:20.000000 soopervisor-0.9.2/src/soopervisor/aws/batch.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1192 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/aws/config.py
--rw-r--r--   0 eduardo    (501) staff       (20)     4777 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/aws/lambda_.py
--rw-r--r--   0 eduardo    (501) staff       (20)      647 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/aws/util.py
--rw-r--r--   0 eduardo    (501) staff       (20)     4467 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/cli.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.741085 soopervisor-0.9.2/src/soopervisor/commons/
--rw-r--r--   0 eduardo    (501) staff       (20)      346 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/commons/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1231 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/commons/conda.py
--rw-r--r--   0 eduardo    (501) staff       (20)     6281 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/commons/dag.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2607 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/commons/dependencies.py
--rw-r--r--   0 eduardo    (501) staff       (20)    11127 2022-12-29 04:09:25.000000 soopervisor-0.9.2/src/soopervisor/commons/docker.py
--rw-r--r--   0 eduardo    (501) staff       (20)     6288 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/commons/source.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1799 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/config.py
--rw-r--r--   0 eduardo    (501) staff       (20)      797 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/enum.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2575 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/exceptions.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1022 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/exporter.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.741365 soopervisor-0.9.2/src/soopervisor/kubeflow/
--rw-r--r--   0 eduardo    (501) staff       (20)        0 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/kubeflow/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      202 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/kubeflow/config.py
--rw-r--r--   0 eduardo    (501) staff       (20)    11384 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/kubeflow/export.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.741668 soopervisor-0.9.2/src/soopervisor/shell/
--rw-r--r--   0 eduardo    (501) staff       (20)       55 2022-12-27 00:40:47.000000 soopervisor-0.9.2/src/soopervisor/shell/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      238 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/shell/config.py
--rw-r--r--   0 eduardo    (501) staff       (20)     5711 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/shell/export.py
--rw-r--r--   0 eduardo    (501) staff       (20)      229 2023-07-18 16:46:24.000000 soopervisor-0.9.2/src/soopervisor/telemetry.py
--rw-r--r--   0 eduardo    (501) staff       (20)      615 2022-12-29 04:29:40.000000 soopervisor-0.9.2/src/soopervisor/validate.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-07-18 17:46:26.738179 soopervisor-0.9.2/src/soopervisor.egg-info/
--rw-r--r--   0 eduardo    (501) staff       (20)    10930 2023-07-18 17:46:26.000000 soopervisor-0.9.2/src/soopervisor.egg-info/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)     1963 2023-07-18 17:46:26.000000 soopervisor-0.9.2/src/soopervisor.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        1 2023-07-18 17:46:26.000000 soopervisor-0.9.2/src/soopervisor.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo    (501) staff       (20)       52 2023-07-18 17:46:26.000000 soopervisor-0.9.2/src/soopervisor.egg-info/entry_points.txt
--rw-r--r--   0 eduardo    (501) staff       (20)      348 2023-07-18 17:46:26.000000 soopervisor-0.9.2/src/soopervisor.egg-info/requires.txt
--rw-r--r--   0 eduardo    (501) staff       (20)       12 2023-07-18 17:46:26.000000 soopervisor-0.9.2/src/soopervisor.egg-info/top_level.txt
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.029235 soopervisor-0.9b1/
+-rw-r--r--   0 Edu        (503) staff       (20)     6891 2022-09-26 20:24:05.000000 soopervisor-0.9b1/CHANGELOG.rst
+-rw-r--r--   0 Edu        (503) staff       (20)    11343 2022-01-30 17:18:36.000000 soopervisor-0.9b1/LICENSE
+-rw-r--r--   0 Edu        (503) staff       (20)      121 2022-02-26 14:10:01.000000 soopervisor-0.9b1/MANIFEST.in
+-rw-r--r--   0 Edu        (503) staff       (20)    10628 2022-09-26 21:03:37.029772 soopervisor-0.9b1/PKG-INFO
+-rw-r--r--   0 Edu        (503) staff       (20)     2858 2022-08-26 03:18:23.000000 soopervisor-0.9b1/README.rst
+-rw-r--r--   0 Edu        (503) staff       (20)      198 2022-01-01 01:49:25.000000 soopervisor-0.9b1/pyproject.toml
+-rw-r--r--   0 Edu        (503) staff       (20)      159 2022-09-26 21:03:37.030889 soopervisor-0.9b1/setup.cfg
+-rw-r--r--   0 Edu        (503) staff       (20)     3268 2022-08-26 03:18:23.000000 soopervisor-0.9b1/setup.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:36.997204 soopervisor-0.9b1/src/
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.007745 soopervisor-0.9b1/src/soopervisor/
+-rw-r--r--   0 Edu        (503) staff       (20)       22 2022-09-26 21:03:26.000000 soopervisor-0.9b1/src/soopervisor/__init__.py
+-rw-r--r--   0 Edu        (503) staff       (20)       77 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/_format.py
+-rw-r--r--   0 Edu        (503) staff       (20)     1106 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/_io.py
+-rw-r--r--   0 Edu        (503) staff       (20)    11985 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/abc.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.011115 soopervisor-0.9b1/src/soopervisor/airflow/
+-rw-r--r--   0 Edu        (503) staff       (20)        0 2020-11-19 06:26:57.000000 soopervisor-0.9b1/src/soopervisor/airflow/__init__.py
+-rw-r--r--   0 Edu        (503) staff       (20)      472 2022-02-11 02:03:35.000000 soopervisor-0.9b1/src/soopervisor/airflow/config.py
+-rw-r--r--   0 Edu        (503) staff       (20)     4742 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/airflow/export.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.012505 soopervisor-0.9b1/src/soopervisor/argo/
+-rw-r--r--   0 Edu        (503) staff       (20)        0 2020-11-19 06:26:57.000000 soopervisor-0.9b1/src/soopervisor/argo/__init__.py
+-rw-r--r--   0 Edu        (503) staff       (20)     1901 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/argo/config.py
+-rw-r--r--   0 Edu        (503) staff       (20)     6268 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/argo/export.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.013429 soopervisor-0.9b1/src/soopervisor/assets/
+-rw-r--r--   0 Edu        (503) staff       (20)    10244 2022-09-22 14:44:18.000000 soopervisor-0.9b1/src/soopervisor/assets/.DS_Store
+-rw-r--r--   0 Edu        (503) staff       (20)        0 2020-08-14 12:00:28.000000 soopervisor-0.9b1/src/soopervisor/assets/__init__.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.015073 soopervisor-0.9b1/src/soopervisor/assets/airflow/
+-rw-r--r--   0 Edu        (503) staff       (20)      751 2022-02-11 02:03:35.000000 soopervisor-0.9b1/src/soopervisor/assets/airflow/bash.py
+-rw-r--r--   0 Edu        (503) staff       (20)      790 2022-02-11 02:03:35.000000 soopervisor-0.9b1/src/soopervisor/assets/airflow/docker.py
+-rw-r--r--   0 Edu        (503) staff       (20)     1206 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/assets/airflow/kubernetes.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.015761 soopervisor-0.9b1/src/soopervisor/assets/argo/
+-rw-r--r--   0 Edu        (503) staff       (20)        0 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/assets/argo/__init__.py
+-rw-r--r--   0 Edu        (503) staff       (20)      543 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/assets/argo/template.yaml
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.016103 soopervisor-0.9b1/src/soopervisor/assets/aws-batch/
+-rw-r--r--   0 Edu        (503) staff       (20)      670 2022-08-26 03:18:23.000000 soopervisor-0.9b1/src/soopervisor/assets/aws-batch/Dockerfile
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.018112 soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/
+-rw-r--r--   0 Edu        (503) staff       (20)      353 2022-08-26 03:18:23.000000 soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/Dockerfile
+-rw-r--r--   0 Edu        (503) staff       (20)     1136 2021-04-18 22:31:31.000000 soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/README.md
+-rw-r--r--   0 Edu        (503) staff       (20)      690 2021-05-22 17:47:14.000000 soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/app.py
+-rw-r--r--   0 Edu        (503) staff       (20)     1869 2021-05-22 17:47:14.000000 soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/template.yaml
+-rw-r--r--   0 Edu        (503) staff       (20)     2848 2021-05-22 17:47:14.000000 soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/test_aws_lambda.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.018730 soopervisor-0.9b1/src/soopervisor/assets/docker/
+-rw-r--r--   0 Edu        (503) staff       (20)      831 2022-09-20 13:16:18.000000 soopervisor-0.9b1/src/soopervisor/assets/docker/Dockerfile
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.019166 soopervisor-0.9b1/src/soopervisor/assets/kubeflow/
+-rw-r--r--   0 Edu        (503) staff       (20)      737 2022-08-26 03:18:23.000000 soopervisor-0.9b1/src/soopervisor/assets/kubeflow/Dockerfile
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.019584 soopervisor-0.9b1/src/soopervisor/assets/slurm/
+-rw-r--r--   0 Edu        (503) staff       (20)      228 2022-02-11 04:26:18.000000 soopervisor-0.9b1/src/soopervisor/assets/slurm/template.sh
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.022459 soopervisor-0.9b1/src/soopervisor/aws/
+-rw-r--r--   0 Edu        (503) staff       (20)        0 2021-04-18 22:31:31.000000 soopervisor-0.9b1/src/soopervisor/aws/__init__.py
+-rw-r--r--   0 Edu        (503) staff       (20)    10581 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/aws/batch.py
+-rw-r--r--   0 Edu        (503) staff       (20)     1217 2022-06-09 08:21:31.000000 soopervisor-0.9b1/src/soopervisor/aws/config.py
+-rw-r--r--   0 Edu        (503) staff       (20)     4866 2022-08-26 03:18:23.000000 soopervisor-0.9b1/src/soopervisor/aws/lambda_.py
+-rw-r--r--   0 Edu        (503) staff       (20)      627 2022-06-09 08:21:31.000000 soopervisor-0.9b1/src/soopervisor/aws/util.py
+-rw-r--r--   0 Edu        (503) staff       (20)     5365 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/cli.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.025694 soopervisor-0.9b1/src/soopervisor/commons/
+-rw-r--r--   0 Edu        (503) staff       (20)      401 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/commons/__init__.py
+-rw-r--r--   0 Edu        (503) staff       (20)     1196 2021-05-22 17:47:14.000000 soopervisor-0.9b1/src/soopervisor/commons/conda.py
+-rw-r--r--   0 Edu        (503) staff       (20)     6535 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/commons/dag.py
+-rw-r--r--   0 Edu        (503) staff       (20)     2567 2022-08-26 03:18:23.000000 soopervisor-0.9b1/src/soopervisor/commons/dependencies.py
+-rw-r--r--   0 Edu        (503) staff       (20)     8770 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/commons/docker.py
+-rw-r--r--   0 Edu        (503) staff       (20)     6509 2022-08-26 03:18:23.000000 soopervisor-0.9b1/src/soopervisor/commons/source.py
+-rw-r--r--   0 Edu        (503) staff       (20)     1776 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/config.py
+-rw-r--r--   0 Edu        (503) staff       (20)      797 2022-06-09 08:21:31.000000 soopervisor-0.9b1/src/soopervisor/enum.py
+-rw-r--r--   0 Edu        (503) staff       (20)     2587 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/exceptions.py
+-rw-r--r--   0 Edu        (503) staff       (20)     1022 2022-06-09 08:21:31.000000 soopervisor-0.9b1/src/soopervisor/exporter.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.027148 soopervisor-0.9b1/src/soopervisor/kubeflow/
+-rw-r--r--   0 Edu        (503) staff       (20)        0 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/kubeflow/__init__.py
+-rw-r--r--   0 Edu        (503) staff       (20)      203 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/kubeflow/config.py
+-rw-r--r--   0 Edu        (503) staff       (20)    11436 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/kubeflow/export.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.028693 soopervisor-0.9b1/src/soopervisor/shell/
+-rw-r--r--   0 Edu        (503) staff       (20)       55 2021-12-20 23:59:39.000000 soopervisor-0.9b1/src/soopervisor/shell/__init__.py
+-rw-r--r--   0 Edu        (503) staff       (20)      243 2022-01-30 17:18:36.000000 soopervisor-0.9b1/src/soopervisor/shell/config.py
+-rw-r--r--   0 Edu        (503) staff       (20)     5751 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/shell/export.py
+-rw-r--r--   0 Edu        (503) staff       (20)      229 2022-08-26 03:18:23.000000 soopervisor-0.9b1/src/soopervisor/telemetry.py
+-rw-r--r--   0 Edu        (503) staff       (20)      628 2022-09-26 20:19:59.000000 soopervisor-0.9b1/src/soopervisor/validate.py
+drwxr-xr-x   0 Edu        (503) staff       (20)        0 2022-09-26 21:03:37.009966 soopervisor-0.9b1/src/soopervisor.egg-info/
+-rw-r--r--   0 Edu        (503) staff       (20)    10628 2022-09-26 21:03:35.000000 soopervisor-0.9b1/src/soopervisor.egg-info/PKG-INFO
+-rw-r--r--   0 Edu        (503) staff       (20)     2040 2022-09-26 21:03:36.000000 soopervisor-0.9b1/src/soopervisor.egg-info/SOURCES.txt
+-rw-r--r--   0 Edu        (503) staff       (20)        1 2022-09-26 21:03:35.000000 soopervisor-0.9b1/src/soopervisor.egg-info/dependency_links.txt
+-rw-r--r--   0 Edu        (503) staff       (20)       52 2022-09-26 21:03:36.000000 soopervisor-0.9b1/src/soopervisor.egg-info/entry_points.txt
+-rw-r--r--   0 Edu        (503) staff       (20)      340 2022-09-26 21:03:36.000000 soopervisor-0.9b1/src/soopervisor.egg-info/requires.txt
+-rw-r--r--   0 Edu        (503) staff       (20)       12 2022-09-26 21:03:36.000000 soopervisor-0.9b1/src/soopervisor.egg-info/top_level.txt
```

### Comparing `soopervisor-0.9.2/CHANGELOG.rst` & `soopervisor-0.9b1/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 CHANGELOG
 =========
 
-0.9.2 (2023-07-18)
-------------------
-* Replaces `@requires` import to use `ploomber_core` instead of `ploomber`
-
-0.9.1 (2022-10-24)
-------------------
-* Adds `--skip-docker` argument in `soopervisor export` to skip docker build (#103)
-* Optimizes the generated AWS Batch ``Dockerfile`` so dependencies are only installed when the requirements are modified
-* Allows using multiple ``requirements.txt`` files, generating one Docker image for each one (#86)
-
-0.9 (2022-10-03)
-----------------
-* Allows execution of single tasks via ``soopervisor export --task {task-name}``
-* Allowing to bundle custom libraries via ``lib/`` in docker image (#87)
-* Fixes DAG loading when passing the ``--lazy`` argument in pipelines with a ``File`` client (#105)
+0.8.1dev
+--------
+* Allos execution of single tasks via `soopervisor export --task {task-name}`
+* Allows using multiple `requirements.txt` files, generating one Docker image for each one (#86)
+* Allowing to bundle custom libraries via `lib/` in docker image (#87)
+* Adding `--skip-docker` argument in `soopervisor export` to skip docker build ([#103](https://github.com/ploomber/soopervisor/issues/103))
+* Fixes DAG loading when passing the `--lazy` argument in pipelines with a `File` client (#105)
 * Display warning if source code contains file over 10MB (#81)
 * Drop support for Python 3.6
 
 0.8 (2022-06-09)
 ----------------
 * Dropping support for Python 3.6
 * Adds ``task_resources`` to AWS Batch
```

### Comparing `soopervisor-0.9.2/LICENSE` & `soopervisor-0.9b1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright (c) 2022-Present Ploomber Inc.
+   Copyright 2022 Ploomber Inc.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `soopervisor-0.9.2/PKG-INFO` & `soopervisor-0.9b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: soopervisor
-Version: 0.9.2
+Version: 0.9b1
+Summary: UNKNOWN
 Home-page: https://github.com/ploomber/soopervisor
 Author: 
 Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
@@ -32,16 +35,14 @@
    :target: https://github.com/ploomber/soopervisor/workflows/CI%20macOS/badge.svg
    :alt: CI macOS badge
 
 .. image:: https://github.com/ploomber/soopervisor/workflows/CI%20Windows/badge.svg
    :target: https://github.com/ploomber/soopervisor/workflows/CI%20Windows/badge.svg
    :alt: CI Windows badge
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
 
 Soopervisor runs `Ploomber <https://github.com/ploomber/ploomber>`_ pipelines
 for batch processing (large-scale training or batch serving) or online
 inference.
 
 .. code-block:: sh
 
@@ -105,29 +106,21 @@
 Whatever your skillset is, you can contribute to our mission. So whether you're a beginner or an experienced professional, you're welcome to join us on this journey!
 
 `Click here to know how you can contribute to Ploomber. <https://github.com/ploomber/contributing/blob/main/README.md>`_
 
 CHANGELOG
 =========
 
-0.9.2 (2023-07-18)
-------------------
-* Replaces `@requires` import to use `ploomber_core` instead of `ploomber`
-
-0.9.1 (2022-10-24)
-------------------
-* Adds `--skip-docker` argument in `soopervisor export` to skip docker build (#103)
-* Optimizes the generated AWS Batch ``Dockerfile`` so dependencies are only installed when the requirements are modified
-* Allows using multiple ``requirements.txt`` files, generating one Docker image for each one (#86)
-
-0.9 (2022-10-03)
-----------------
-* Allows execution of single tasks via ``soopervisor export --task {task-name}``
-* Allowing to bundle custom libraries via ``lib/`` in docker image (#87)
-* Fixes DAG loading when passing the ``--lazy`` argument in pipelines with a ``File`` client (#105)
+0.8.1dev
+--------
+* Allos execution of single tasks via `soopervisor export --task {task-name}`
+* Allows using multiple `requirements.txt` files, generating one Docker image for each one (#86)
+* Allowing to bundle custom libraries via `lib/` in docker image (#87)
+* Adding `--skip-docker` argument in `soopervisor export` to skip docker build ([#103](https://github.com/ploomber/soopervisor/issues/103))
+* Fixes DAG loading when passing the `--lazy` argument in pipelines with a `File` client (#105)
 * Display warning if source code contains file over 10MB (#81)
 * Drop support for Python 3.6
 
 0.8 (2022-06-09)
 ----------------
 * Dropping support for Python 3.6
 * Adds ``task_resources`` to AWS Batch
@@ -284,7 +277,9 @@
 * Conda environments are cached by default
 * Ability to customize arguments to ``ploomber build``
 
 0.1 (2020-08-09)
 -----------------
 
 * First release
+
+
```

### Comparing `soopervisor-0.9.2/README.rst` & `soopervisor-0.9b1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,14 @@
    :target: https://github.com/ploomber/soopervisor/workflows/CI%20macOS/badge.svg
    :alt: CI macOS badge
 
 .. image:: https://github.com/ploomber/soopervisor/workflows/CI%20Windows/badge.svg
    :target: https://github.com/ploomber/soopervisor/workflows/CI%20Windows/badge.svg
    :alt: CI Windows badge
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
 
 Soopervisor runs `Ploomber <https://github.com/ploomber/ploomber>`_ pipelines
 for batch processing (large-scale training or batch serving) or online
 inference.
 
 .. code-block:: sh
```

### Comparing `soopervisor-0.9.2/setup.py` & `soopervisor-0.9b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,121 +6,117 @@
 from os.path import dirname
 from os.path import join
 from os.path import splitext
 
 from setuptools import find_packages
 from setuptools import setup
 
-_version_re = re.compile(r"__version__\s+=\s+(.*)")
+_version_re = re.compile(r'__version__\s+=\s+(.*)')
 
-with open("src/soopervisor/__init__.py", "rb") as f:
+with open('src/soopervisor/__init__.py', 'rb') as f:
     VERSION = str(
-        ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
-    )
+        ast.literal_eval(
+            _version_re.search(f.read().decode('utf-8')).group(1)))
 
 
 def read(*names, **kwargs):
-    return io.open(
-        join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
-    ).read()
+    return io.open(join(dirname(__file__), *names),
+                   encoding=kwargs.get('encoding', 'utf8')).read()
 
 
 REQUIRES = [
-    "click",
-    "tqdm",
-    "pydantic",
-    "Jinja2",
-    "pyyaml",
-    "ploomber>=0.14.6",
-    "ploomber-core>=0.0.11",
+    'click',
+    'tqdm',
+    'pydantic',
+    'Jinja2',
+    'pyyaml',
+    'ploomber>=0.14.6',
+    'ploomber-core',
     # sdist is generated using python -m build, so adding this here.
     # I can remoe it if I change all references to use python setup.py sdist
     # instead
-    "build",
+    'build',
 ]
 
-AWS = ["boto3"]
+AWS = ['boto3']
 
 DEV = [
-    "pkgmt",
-    "invoke",
+    'pkgmt',
+    'invoke',
     # TEST
-    "pytest",
-    "Faker",
-    "yapf",
-    "flake8",
+    'pytest',
+    'Faker',
+    'yapf',
+    'flake8',
     # soopervisor works with airflow 1.X as well but we force the version
     # to prevent pip from installing it (tests will not pass since imports are
     # different)
-    "apache-airflow",
+    'apache-airflow',
     # KubernetesPodOperator
-    "apache-airflow-providers-cncf-kubernetes",
+    'apache-airflow-providers-cncf-kubernetes',
     # DockerOperator
-    "apache-airflow-providers-docker",
+    'apache-airflow-providers-docker',
     # exporting to kubeflow
-    "kfp",
+    'kfp',
     # to validate argo specs
-    "argo-workflows-dsl",
+    'argo-workflows-dsl',
     # for testing aws (newer versions break)
     # see: https://github.com/spulec/moto/issues/1793
-    "moto==1.3.14",
+    'moto==1.3.14',
     # for test_dist.py
-    "wheel",
+    'wheel',
     # to run assets/my_project
-    "scikit-learn",
+    'scikit-learn',
     # DOCS
-    "sphinx",
-    "sphinx-autobuild",
-    "sphinx-inline-tabs",
-    "furo",
+    'sphinx',
+    'sphinx-autobuild',
+    'sphinx-inline-tabs',
+    'furo',
     # RELEASE
-    "twine",
-    "ipython",
+    'twine',
+    'ipython',
 ]
 
-DESCRIPTION = ""
+DESCRIPTION = ''
 
 setup(
-    name="soopervisor",
+    name='soopervisor',
     version=VERSION,
     description=DESCRIPTION,
-    long_description="%s\n%s"
-    % (
-        re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
-            "", read("README.rst")
-        ),
-        re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
-    ),
-    author="",
-    author_email="",
-    url="https://github.com/ploomber/soopervisor",
-    packages=find_packages(where="src"),
-    package_dir={"": "src"},
-    py_modules=[splitext(basename(path))[0] for path in glob("src/*.py")],
+    long_description='%s\n%s' %
+    (re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub(
+        '', read('README.rst')),
+     re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))),
+    author='',
+    author_email='',
+    url='https://github.com/ploomber/soopervisor',
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
+    py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Unix",
-        "Operating System :: POSIX",
-        "Operating System :: Microsoft :: Windows",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: Apache Software License',
+        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: Unix',
+        'Operating System :: POSIX',
+        'Operating System :: Microsoft :: Windows',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     install_requires=REQUIRES,
     extras_require={
         # for users
-        "aws": AWS,
+        'aws': AWS,
         # for development and testing
-        "dev": DEV + AWS,
+        'dev': DEV + AWS,
     },
     setup_requires=[],
     entry_points={
-        "console_scripts": ["soopervisor=soopervisor.cli:cli"],
+        'console_scripts': ['soopervisor=soopervisor.cli:cli'],
     },
 )
```

### Comparing `soopervisor-0.9.2/src/soopervisor/_io.py` & `soopervisor-0.9b1/src/soopervisor/_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 from collections.abc import Mapping
 from pathlib import Path
 
 import yaml
 
-from soopervisor.exceptions import ConfigurationFileTypeError, ConfigurationError
+from soopervisor.exceptions import (ConfigurationFileTypeError,
+                                    ConfigurationError)
 
 
-def load_config_file(path="soopervisor.yaml", expected_env_name=None):
+def load_config_file(path='soopervisor.yaml', expected_env_name=None):
     """
     Load a config file, validates that the returned value is a dictionary,
     optionally validates the existence of certain key
     """
     path = Path(path)
 
     if not path.exists():
-        raise ConfigurationError(
-            f"Error loading {str(path)!r}. File " "does not exist."
-        )
+        raise ConfigurationError(f'Error loading {str(path)!r}. File '
+                                 'does not exist.')
 
     if path.is_dir():
-        raise ConfigurationError(
-            f"Error loading {str(path)!r}. Path " "is a directory."
-        )
+        raise ConfigurationError(f'Error loading {str(path)!r}. Path '
+                                 'is a directory.')
 
     data = yaml.safe_load(Path(path).read_text())
 
     if not isinstance(data, Mapping):
         raise ConfigurationFileTypeError(path, data)
 
     if expected_env_name and expected_env_name not in data:
-        raise ConfigurationError(
-            f"{str(path)!r} does not contain a target "
-            f"environment named {expected_env_name!r}"
-        )
+        raise ConfigurationError(f'{str(path)!r} does not contain a target '
+                                 f'environment named {expected_env_name!r}')
 
     return data
```

### Comparing `soopervisor-0.9.2/src/soopervisor/abc.py` & `soopervisor-0.9b1/src/soopervisor/abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,53 +8,49 @@
 from typing import Optional, List
 from copy import deepcopy
 
 import yaml
 from pydantic import BaseModel
 
 from soopervisor import commons
-from soopervisor.exceptions import (
-    BackendWithoutPresetsError,
-    InvalidPresetForBackendError,
-    ConfigurationError,
-)
+from soopervisor.exceptions import (BackendWithoutPresetsError,
+                                    InvalidPresetForBackendError,
+                                    ConfigurationError)
 from soopervisor._io import load_config_file
 from soopervisor.commons.dag import load_dag_and_spec
 
 
 class AbstractConfig(BaseModel, abc.ABC):
     """Abstract class for configuration objects
 
     Parameters
     ----------
     preset : str
         The preset to use, this determines certain settings and is
         backend-specific
     """
-
     preset: Optional[str] = None
 
     class Config:
-        extra = "forbid"
+        extra = 'forbid'
 
     @classmethod
     def load(cls, path_to_config, env_name):
         """
         Load the target environment configuration from a given YAML config
         file. Creates one if needed.
         """
         data = load_config_file(path_to_config, expected_env_name=env_name)
 
         # check data[env_name] is a dictionary
         if not isinstance(data[env_name], Mapping):
             raise ConfigurationError(
-                f"Expected key {env_name!r} in {str(path_to_config)!r} "
-                "to contain a dictionary, "
-                f"got {type(data[env_name]).__name__}"
-            )
+                f'Expected key {env_name!r} in {str(path_to_config)!r} '
+                'to contain a dictionary, '
+                f'got {type(data[env_name]).__name__}')
 
         return cls._init(env_name, data[env_name], path_to_config)
 
     @classmethod
     def _init(cls, env_name, data, path_to_config):
         """Initialize the Config object and perform validations
 
@@ -68,47 +64,46 @@
 
         path_to_config
             Path to the config file, only used for displaying it in errors
         """
         # check env_name in data, otherwise the env is corrupted
         data = deepcopy(data)
 
-        if "backend" not in data:
+        if 'backend' not in data:
             raise ConfigurationError(
                 f'Missing {"backend"!r} key for '
-                f"section {env_name!r} in {path_to_config!r}. "
-                "Add it and try again."
-            )
+                f'section {env_name!r} in {path_to_config!r}. '
+                'Add it and try again.')
 
-        actual = data["backend"]
+        actual = data['backend']
         backend = cls.get_backend_value()
 
         if actual != backend:
             raise ConfigurationError(
-                f"Invalid backend key for section {env_name!r} in "
-                f"{path_to_config!s}. Expected {backend!r}, "
-                f"actual {actual!r}"
-            )
+                f'Invalid backend key for section {env_name!r} in '
+                f'{path_to_config!s}. Expected {backend!r}, '
+                f'actual {actual!r}')
 
-        del data["backend"]
+        del data['backend']
 
         cfg = cls(**data)
 
         # validate presets is valid
         presets = cls.get_presets()
 
         if presets is None and cfg.preset:
             raise BackendWithoutPresetsError(backend)
 
         if presets:
             if cfg.preset is None:
                 cfg.preset = presets[0]
 
             if cfg.preset not in presets:
-                raise InvalidPresetForBackendError(backend, cfg.preset, presets)
+                raise InvalidPresetForBackendError(backend, cfg.preset,
+                                                   presets)
 
         return cfg
 
     @classmethod
     def new(cls, path_to_config, env_name, preset=None, **defaults):
         """
         Validates, then writes a configuration setting in the selected file
@@ -124,33 +119,33 @@
         preset
             Target environment preset
 
         defaults
             Any other values to store
         """
         if Path(env_name).exists():
-            type_ = "directory" if Path(env_name).is_dir() else "file"
+            type_ = 'directory' if Path(env_name).is_dir() else 'file'
             raise ConfigurationError(
-                f"A {type_} named "
-                f"{env_name!r} already exists in the current working "
-                "directory, select another name for the target environment"
-                " and try again."
-            )
+                f'A {type_} named '
+                f'{env_name!r} already exists in the current working '
+                'directory, select another name for the target environment'
+                ' and try again.')
 
         data = {**cls.hints(), **defaults}
 
         if preset:
-            data["preset"] = preset
+            data['preset'] = preset
 
         # initialize config before storing the yaml to halt execution
         # in case there are any validation errors
         cfg = cls._init(env_name, data, path_to_config)
 
         # pass default_flow_style=None to it serializes lists as [a, b, c]
-        default_data = yaml.safe_dump({env_name: data}, default_flow_style=None)
+        default_data = yaml.safe_dump({env_name: data},
+                                      default_flow_style=None)
 
         # if no config file, write one with env_name section and hints
         if not Path(path_to_config).exists():
             Path(path_to_config).write_text(default_data)
 
         # if config file but missing env_name section, add one with the hints
         else:
@@ -158,28 +153,28 @@
             content = path.read_text()
             env_names = list(load_config_file(path_to_config))
 
             # only update the config file if the section does not exist
             if env_name not in env_names:
                 # append to the text file so we don't delete any existing
                 # comments
-                path.write_text(content + f"\n{default_data}\n")
+                path.write_text(content + f'\n{default_data}\n')
             else:
                 raise ConfigurationError(
-                    "A target environment named "
-                    f"{env_name!r} already exists in {str(path_to_config)!r}, "
-                    "select another name and try again."
-                )
+                    'A target environment named '
+                    f'{env_name!r} already exists in {str(path_to_config)!r}, '
+                    'select another name and try again.')
 
         return cfg
 
     @classmethod
     @abc.abstractmethod
     def get_backend_value(cls):
-        """Returns the string identifier for the given backend"""
+        """Returns the string identifier for the given backend
+        """
         pass
 
     @classmethod
     def get_presets(cls):
         return None
 
     @classmethod
@@ -201,37 +196,36 @@
     def hints(cls):
         """
         Returns a dictiionary with the values to use when a target environment
         is created, it also adds the appropriate backend value. Actual
         hint values must be returned in the _hints() method
         """
         data = cls._hints()
-        data["backend"] = cls.get_backend_value()
+        data['backend'] = cls.get_backend_value()
         return data
 
 
 class AbstractDockerConfig(AbstractConfig):
     """
     An abstract class for docker-based configurations where having a remote
     repository is optional (e.g., can build an image locally)
 
     include : list of str
         Files/directories to include in the Docker image
 
     exclude : list of str
         Files/directories to exclude from the Docker image
     """
-
     include: Optional[List[str]] = None
     exclude: Optional[List[str]] = None
     repository: Optional[str] = None
 
     @classmethod
     def _hints(cls):
-        return dict(repository="your-repository/name")
+        return dict(repository='your-repository/name')
 
 
 class AbstractExporter(abc.ABC):
     """
     Steps:
     1. Initialize configuration object
     2. Perform general validation (applicable to all targets)
@@ -248,15 +242,14 @@
         Environment name
 
     preset : str, default=None
         The backend preset (customizes the configuration). If this isn't
         None and the concrete class does not take a present, it will raise
         an exception
     """
-
     CONFIG_CLASS = None
 
     def __init__(self, cfg, dag, env_name):
         # initialize configuration, write to config file and a few checks on
         # it
         self._cfg = cfg
         self._env_name = env_name
@@ -271,21 +264,23 @@
         Loads an exporter using settings from an existing configuration file
         """
         # run some basic validations
         cls.validate()
 
         dag, _ = load_dag_and_spec(env_name, lazy_import=lazy_import)
 
-        cfg = cls.CONFIG_CLASS.load(path_to_config=path_to_config, env_name=env_name)
+        cfg = cls.CONFIG_CLASS.load(path_to_config=path_to_config,
+                                    env_name=env_name)
 
         return cls(cfg, dag, env_name)
 
     @classmethod
     def new(cls, path_to_config, env_name, preset=None, lazy_import=False):
-        """ """
+        """
+        """
         # run some basic validations
         cls.validate()
 
         dag, spec = load_dag_and_spec(env_name, lazy_import=lazy_import)
 
         if issubclass(cls.CONFIG_CLASS, AbstractDockerConfig):
             # it the spec has products store in relative paths, get them and
@@ -309,67 +304,64 @@
         """
         Verify project has the right structure before running the script.
         This runs as a sanity check in the development machine
         """
         commons.dependencies.check_lock_files_exist()
 
     def add(self):
-        """Create a directory with the env_name and add any necessary files"""
+        """Create a directory with the env_name and add any necessary files
+        """
 
         # check that env_name folder does not exist
         path = Path(self._env_name)
 
         if path.exists():
             Path(self._env_name)
 
-            kind = "file" if path.is_file() else "directory"
+            kind = 'file' if path.is_file() else 'directory'
             raise FileExistsError(
-                f"A {kind} with name {self._env_name!r} "
-                "already exists, delete or rename it and try again"
-            )
+                f'A {kind} with name {self._env_name!r} '
+                'already exists, delete or rename it and try again')
 
         path.mkdir()
 
         return self._add(cfg=self._cfg, env_name=self._env_name)
 
-    def export(
-        self,
-        mode,
-        until=None,
-        skip_tests=False,
-        skip_docker=False,
-        ignore_git=False,
-        lazy_import=False,
-        task_name=None,
-    ):
+    def export(self,
+               mode,
+               until=None,
+               skip_tests=False,
+               skip_docker=False,
+               ignore_git=False,
+               lazy_import=False,
+               task_name=None):
         """
         Exports to the target environment, calls the private ._export()
         method
         """
         # TODO: detect inconsistencies. e.g., environment exists but directory
         # doesnt
         if skip_docker:
-            click.echo("Skipping docker build")
+            click.echo('Skipping docker build')
 
-        return self._export(
-            cfg=self._cfg,
-            env_name=self._env_name,
-            mode=mode,
-            until=until,
-            skip_tests=skip_tests,
-            skip_docker=skip_docker,
-            ignore_git=ignore_git,
-            lazy_import=lazy_import,
-            task_name=task_name,
-        )
+        return self._export(cfg=self._cfg,
+                            env_name=self._env_name,
+                            mode=mode,
+                            until=until,
+                            skip_tests=skip_tests,
+                            skip_docker=skip_docker,
+                            ignore_git=ignore_git,
+                            lazy_import=lazy_import,
+                            task_name=task_name)
 
     @staticmethod
     @abc.abstractmethod
     def _validate(cfg, dag, env_name):
-        """Validate project before generating exported files"""
+        """Validate project before generating exported files
+        """
         pass
 
     @staticmethod
     @abc.abstractmethod
     def _add():
         """
         Private method implementing the backend-specific logic for the add
```

### Comparing `soopervisor-0.9.2/src/soopervisor/airflow/export.py` & `soopervisor-0.9b1/src/soopervisor/airflow/export.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,139 +14,118 @@
 
 
 class AirflowExporter(abc.AbstractExporter):
     """
     Airflow exporter, the generated Airflow DAG can be customized usin
     presets: 'none' (default, KubernetesPodOperator), bash (DockerOperator)
     """
-
     CONFIG_CLASS = AirflowConfig
 
     @staticmethod
     def _add(cfg, env_name):
         """Export Ploomber project to Airflow
 
         Generates a .py file that exposes a dag variable
         """
-        click.echo("Exporting to Airflow...")
-        project_root = Path(".").resolve()
+        click.echo('Exporting to Airflow...')
+        project_root = Path('.').resolve()
         project_name = project_root.name
 
-        name = f"{cfg.preset}.py"
+        name = f'{cfg.preset}.py'
 
         # TODO: modify Dockerfile depending on package or non-package
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as e:
-            e.copy_template(
-                f"airflow/{name}", project_name=project_name, env_name=env_name
-            )
-            path_out = str(Path(env_name, project_name + ".py"))
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as e:
+            e.copy_template(f'airflow/{name}',
+                            project_name=project_name,
+                            env_name=env_name)
+            path_out = str(Path(env_name, project_name + '.py'))
             os.rename(Path(env_name, name), path_out)
 
-            if cfg.preset != "bash":
-                e.copy_template(
-                    "docker/Dockerfile",
-                    conda=Path("environment.lock.yml").exists(),
-                    setup_py=Path("setup.py").exists(),
-                    lib=Path("lib").exists(),
-                    env_name=env_name,
-                )
+            if cfg.preset != 'bash':
+                e.copy_template('docker/Dockerfile',
+                                conda=Path('environment.lock.yml').exists(),
+                                setup_py=Path('setup.py').exists(),
+                                lib=Path('lib').exists(),
+                                env_name=env_name)
 
             click.echo(
-                f"Airflow DAG declaration saved to {path_out!r}, you may "
-                "edit the file to change the configuration if needed, "
-                "(e.g., set the execution period)"
-            )
+                f'Airflow DAG declaration saved to {path_out!r}, you may '
+                'edit the file to change the configuration if needed, '
+                '(e.g., set the execution period)')
 
     @staticmethod
     def _validate(cfg, dag, env_name):
         """
         Validates a project before exporting as an Airflow DAG.
         This runs as a sanity check in the development machine
         """
         pass
 
     @staticmethod
-    def _export(
-        cfg,
-        env_name,
-        mode,
-        until,
-        skip_tests,
-        skip_docker,
-        ignore_git,
-        lazy_import,
-        task_name,
-    ):
+    def _export(cfg, env_name, mode, until, skip_tests, skip_docker,
+                ignore_git, lazy_import, task_name):
         """
         Copies the current source code to the target environment folder.
         The code along with the DAG declaration file can be copied to
         AIRFLOW_HOME for execution
         """
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as e:
-            tasks, args = commons.load_tasks(
-                cmdr=e,
-                name=env_name,
-                mode=mode,
-                lazy_import=lazy_import,
-                task_name=task_name,
-            )
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as e:
+            tasks, args = commons.load_tasks(cmdr=e,
+                                             name=env_name,
+                                             mode=mode,
+                                             lazy_import=lazy_import,
+                                             task_name=task_name)
 
             if not tasks:
-                raise CommanderStop(
-                    f"Loaded DAG in {mode!r} mode has no "
-                    'tasks to submit. Try "--mode force" to '
-                    "submit all tasks regardless of status"
-                )
+                raise CommanderStop(f'Loaded DAG in {mode!r} mode has no '
+                                    'tasks to submit. Try "--mode force" to '
+                                    'submit all tasks regardless of status')
 
             # TODO: throw a warning if non-docker preset but there is a
             # Dockerfile
-            if cfg.preset != "bash" and not skip_docker:
+            if cfg.preset != 'bash' and not skip_docker:
                 pkg_name, target_image = commons.docker.build(
                     e,
                     cfg,
                     env_name,
                     until=until,
                     entry_point=args[1],
                     skip_tests=skip_tests,
-                    ignore_git=ignore_git,
-                )
+                    ignore_git=ignore_git)
                 target_image = target_image[
-                    commons.dependencies.get_default_image_key()
-                ]
+                    commons.dependencies.get_default_image_key()]
                 dag_dict = generate_airflow_spec(tasks, args, target_image)
 
-                path_dag_dict_out = Path(pkg_name + ".json")
+                path_dag_dict_out = Path(pkg_name + '.json')
                 path_dag_dict_out.write_text(json.dumps(dag_dict))
 
             else:
-                (
-                    pkg_name,
-                    target_image,
-                ) = commons.source.find_package_name_and_version()
+                (pkg_name, target_image
+                 ) = commons.source.find_package_name_and_version()
 
                 dag_dict = generate_airflow_spec(tasks, args, target_image)
-                path_dag_dict_out = Path(env_name, pkg_name + ".json")
+                path_dag_dict_out = Path(env_name, pkg_name + '.json')
                 path_dag_dict_out.write_text(json.dumps(dag_dict))
 
 
 def generate_airflow_spec(tasks, args, target_image):
     """
     Generates a dictionary with the spec used by Airflow to construct the
     DAG
     """
     dag_dict = dict(tasks=[], image=target_image)
 
     for name, upstream in tasks.items():
-        command = f"ploomber task {name}"
+        command = f'ploomber task {name}'
 
         if args:
             command = f'{command} {" ".join(args)}'
 
-        dag_dict["tasks"].append(
-            {"name": name, "upstream": upstream, "command": command}
-        )
+        dag_dict['tasks'].append({
+            'name': name,
+            'upstream': upstream,
+            'command': command
+        })
 
     return dag_dict
```

### Comparing `soopervisor-0.9.2/src/soopervisor/argo/config.py` & `soopervisor-0.9b1/src/soopervisor/argo/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,38 +20,37 @@
         ``volumeMounts[*].subPath``). Defaults to the volume's root
 
     spec : dict
         The volume spec, passed directly to the output spec.
         e.g: ``{'persistentVolumeClaim': {'claimName': 'someName'}}``
 
     """
-
     name: str
-    sub_path: str = ""
+    sub_path: str = ''
     spec: dict
 
     class Config:
-        extra = "forbid"
+        extra = 'forbid'
 
     def to_volume(self):
         """
         Generate the entry for the spec.volumes
         """
-        return {"name": self.name, **self.spec}
+        return {'name': self.name, **self.spec}
 
     def to_volume_mount(self):
         """
         Generate the entry for spec.templates[0].volumeMounts
         """
         # reference: https://argoproj.github.io/argo/fields/#volumemount
         return {
-            "name": self.name,
+            'name': self.name,
             # by convention, mount to /mnt/ and use the claim name
-            "mountPath": f"/mnt/{self.name}",
-            "subPath": self.sub_path,
+            'mountPath': f'/mnt/{self.name}',
+            'subPath': self.sub_path
         }
 
 
 class ArgoConfig(abc.AbstractDockerConfig):
     """Configuration for exporting to Argo
 
     Parameters
@@ -64,13 +63,12 @@
             If ``repository`` is ``null``, it sets the ``imagePullPolicy`` in
             the generated spec to ``Never``.
 
     mounted_volumes : list, optional
         List of volumes to mount on each Pod, described with the
         ``ArgoMountedVolumes`` schema.
     """
-
     mounted_volumes: Optional[List[ArgoMountedVolume]] = None
 
     @classmethod
     def get_backend_value(cls):
         return Backend.argo_workflows.value
```

### Comparing `soopervisor-0.9.2/src/soopervisor/argo/export.py` & `soopervisor-0.9b1/src/soopervisor/argo/export.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,180 +27,157 @@
         pass
 
     @staticmethod
     def _add(cfg, env_name):
         """
         Add Dockerfile
         """
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as e:
-            e.copy_template(
-                "docker/Dockerfile",
-                conda=Path("environment.lock.yml").exists(),
-                setup_py=Path("setup.py").exists(),
-                lib=Path("lib").exists(),
-                env_name=env_name,
-            )
-            e.success("Done")
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as e:
+            e.copy_template('docker/Dockerfile',
+                            conda=Path('environment.lock.yml').exists(),
+                            setup_py=Path('setup.py').exists(),
+                            lib=Path('lib').exists(),
+                            env_name=env_name)
+            e.success('Done')
 
     @staticmethod
-    def _export(
-        cfg,
-        env_name,
-        mode,
-        until,
-        skip_tests,
-        skip_docker,
-        ignore_git,
-        lazy_import,
-        task_name,
-    ):
+    def _export(cfg, env_name, mode, until, skip_tests, skip_docker,
+                ignore_git, lazy_import, task_name):
         """
         Build and upload Docker image. Export Argo YAML spec.
         """
 
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as cmdr:
-
-            tasks, args = commons.load_tasks(
-                cmdr=cmdr,
-                name=env_name,
-                mode=mode,
-                lazy_import=lazy_import,
-                task_name=task_name,
-            )
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as cmdr:
+
+            tasks, args = commons.load_tasks(cmdr=cmdr,
+                                             name=env_name,
+                                             mode=mode,
+                                             lazy_import=lazy_import,
+                                             task_name=task_name)
 
             if not tasks:
-                raise CommanderStop(
-                    f"Loaded DAG in {mode!r} mode has no "
-                    'tasks to submit. Try "--mode force" to '
-                    "submit all tasks regardless of status"
-                )
+                raise CommanderStop(f'Loaded DAG in {mode!r} mode has no '
+                                    'tasks to submit. Try "--mode force" to '
+                                    'submit all tasks regardless of status')
             if skip_docker:
                 pkg_name, version = source.find_package_name_and_version()
                 default_image_key = get_default_image_key()
                 if default_image_key:
-                    image_local = f"{pkg_name}:{version}-"
-                    f"{docker.modify_wildcard(default_image_key)}"
+                    image_local = f'{pkg_name}:{version}-'
+                    f'{docker.modify_wildcard(default_image_key)}'
                 target_image = image_local
             else:
-                pkg_name, target_image = docker.build(
-                    cmdr,
-                    cfg,
-                    env_name,
-                    until=until,
-                    entry_point=args[1],
-                    skip_tests=skip_tests,
-                    ignore_git=ignore_git,
-                )
+                pkg_name, target_image = docker.build(cmdr,
+                                                      cfg,
+                                                      env_name,
+                                                      until=until,
+                                                      entry_point=args[1],
+                                                      skip_tests=skip_tests,
+                                                      ignore_git=ignore_git)
                 target_image = target_image[get_default_image_key()]
 
-            cmdr.info("Generating Argo Workflows YAML spec")
-            _make_argo_spec(
-                tasks=tasks,
-                args=args,
-                env_name=env_name,
-                cfg=cfg,
-                pkg_name=pkg_name,
-                target_image=target_image,
-            )
+            cmdr.info('Generating Argo Workflows YAML spec')
+            _make_argo_spec(tasks=tasks,
+                            args=args,
+                            env_name=env_name,
+                            cfg=cfg,
+                            pkg_name=pkg_name,
+                            target_image=target_image)
 
-            cmdr.success("Done.")
+            cmdr.success('Done.')
 
 
 # TODO: delete
 class _literal_str(str):
     """Custom str to represent it in YAML literal style
     Source: https://stackoverflow.com/a/20863889/709975
     """
-
     pass
 
 
 def _change_style(style, representer):
+
     def new_representer(dumper, data):
         scalar = representer(dumper, data)
         scalar.style = style
         return scalar
 
     return new_representer
 
 
 # configure yaml to represent "literal_str" objects in literal style
-represent_literal_str = _change_style("|", SafeRepresenter.represent_str)
+represent_literal_str = _change_style('|', SafeRepresenter.represent_str)
 yaml.add_representer(_literal_str, represent_literal_str)
 
 
 def _make_argo_task(name, dependencies):
-    """Generate an Argo Task spec"""
+    """Generate an Argo Task spec
+    """
     task = {
-        "name": name,
-        "dependencies": dependencies,
-        "template": "run-task",
-        "arguments": {
-            "parameters": [
-                {
-                    "name": "task_name",
-                    "value": name,
-                }
-            ]
-        },
+        'name': name,
+        'dependencies': dependencies,
+        'template': 'run-task',
+        'arguments': {
+            'parameters': [{
+                'name': 'task_name',
+                'value': name,
+            }]
+        }
     }
     return task
 
 
 def _make_argo_spec(tasks, args, env_name, cfg, pkg_name, target_image):
-    """Generate Argo's YAML spec"""
+    """Generate Argo's YAML spec
+    """
     if cfg.mounted_volumes:
-        volumes, volume_mounts = zip(
-            *((mv.to_volume(), mv.to_volume_mount()) for mv in cfg.mounted_volumes)
-        )
+        volumes, volume_mounts = zip(*((mv.to_volume(), mv.to_volume_mount())
+                                       for mv in cfg.mounted_volumes))
         # force them to be lists to prevent "!!python/tuple" to be added
         volumes = list(volumes)
         volume_mounts = list(volume_mounts)
     else:
         volumes = []
         volume_mounts = []
 
-    argo_spec = yaml.safe_load(pkg_resources.read_text(assets_argo, "template.yaml"))
-    argo_spec["spec"]["volumes"] = volumes
+    argo_spec = yaml.safe_load(
+        pkg_resources.read_text(assets_argo, 'template.yaml'))
+    argo_spec['spec']['volumes'] = volumes
 
     tasks_specs = []
 
     for task_name, upstream in tasks.items():
         spec = _make_argo_task(task_name, upstream)
         tasks_specs.append(spec)
 
-    argo_spec["metadata"]["generateName"] = f"{pkg_name}-".replace("_", "-")
-    argo_spec["spec"]["templates"][1]["dag"]["tasks"] = tasks_specs
+    argo_spec['metadata']['generateName'] = f'{pkg_name}-'.replace('_', '-')
+    argo_spec['spec']['templates'][1]['dag']['tasks'] = tasks_specs
 
-    script = argo_spec["spec"]["templates"][0]["script"]
-    script["volumeMounts"] = volume_mounts
-    script["image"] = target_image
+    script = argo_spec['spec']['templates'][0]['script']
+    script['volumeMounts'] = volume_mounts
+    script['image'] = target_image
 
     if cfg.repository is None:
-        click.echo(
-            "null repository found in soopervisor.yaml, "
-            'setting imagePullPolicy to "Never"'
-        )
-        script["imagePullPolicy"] = "Never"
+        click.echo('null repository found in soopervisor.yaml, '
+                   'setting imagePullPolicy to "Never"')
+        script['imagePullPolicy'] = 'Never'
 
-    command = "ploomber task {{inputs.parameters.task_name}}"
+    command = 'ploomber task {{inputs.parameters.task_name}}'
 
     if args:
         command = f'{command} {" ".join(args)}'
 
     # use literal_str to make the script source code be represented in YAML
     # literal style, this makes it readable
-    script["source"] = _literal_str(command)
+    script['source'] = _literal_str(command)
 
     # when we run this the current working directory is env_name/
-    with open("argo.yaml", "w") as f:
+    with open('argo.yaml', 'w') as f:
         yaml.dump(argo_spec, f)
 
-    output_path = f"{env_name}/argo.yaml"
-    click.echo(f"Done. Saved argo spec to {output_path!r}")
-    click.echo(f"Submit your workflow with: argo submit -n argo {output_path}")
+    output_path = f'{env_name}/argo.yaml'
+    click.echo(f'Done. Saved argo spec to {output_path!r}')
+    click.echo(f'Submit your workflow with: argo submit -n argo {output_path}')
 
     return argo_spec
```

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/airflow/bash.py` & `soopervisor-0.9b1/src/soopervisor/assets/airflow/bash.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from pathlib import Path
 
 from airflow import DAG
 from airflow.utils.dates import days_ago
 from airflow.operators.bash import BashOperator
 
 default_args = {
-    "start_date": days_ago(0),
+    'start_date': days_ago(0),
 }
 
 dag = DAG(
-    dag_id="{{project_name}}",
+    dag_id='{{project_name}}',
     default_args=default_args,
-    description="Ploomber DAG ({{project_name}})",
+    description='Ploomber DAG ({{project_name}})',
     schedule_interval=None,
 )
 
-path_to_spec = Path(__file__).parent / "{{project_name}}.json"
+path_to_spec = Path(__file__).parent / '{{project_name}}.json'
 spec = json.loads(path_to_spec.read_text())
 
-for task in spec["tasks"]:
+for task in spec['tasks']:
     BashOperator(
-        bash_command=task["command"],
-        task_id=task["name"],
+        bash_command=task['command'],
+        task_id=task['name'],
         dag=dag,
     )
 
-for task in spec["tasks"]:
-    t = dag.get_task(task["name"])
+for task in spec['tasks']:
+    t = dag.get_task(task['name'])
 
-    for upstream in task["upstream"]:
+    for upstream in task['upstream']:
         t.set_upstream(dag.get_task(upstream))
```

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/airflow/docker.py` & `soopervisor-0.9b1/src/soopervisor/assets/airflow/docker.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 from pathlib import Path
 
 from airflow import DAG
 from airflow.utils.dates import days_ago
 from airflow.operators.docker_operator import DockerOperator
 
 default_args = {
-    "start_date": days_ago(0),
+    'start_date': days_ago(0),
 }
 
 dag = DAG(
-    dag_id="{{project_name}}",
+    dag_id='{{project_name}}',
     default_args=default_args,
-    description="Ploomber DAG ({{project_name}})",
+    description='Ploomber DAG ({{project_name}})',
     schedule_interval=None,
 )
 
-path_to_spec = Path(__file__).parent / "{{project_name}}.json"
+path_to_spec = Path(__file__).parent / '{{project_name}}.json'
 spec = json.loads(path_to_spec.read_text())
 
-for task in spec["tasks"]:
+for task in spec['tasks']:
     DockerOperator(
-        image=spec["image"],
-        command=task["command"],
+        image=spec['image'],
+        command=task['command'],
         dag=dag,
-        task_id=task["name"],
+        task_id=task['name'],
     )
 
-for task in spec["tasks"]:
-    t = dag.get_task(task["name"])
+for task in spec['tasks']:
+    t = dag.get_task(task['name'])
 
-    for upstream in task["upstream"]:
+    for upstream in task['upstream']:
         t.set_upstream(dag.get_task(upstream))
```

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/airflow/kubernetes.py` & `soopervisor-0.9b1/src/soopervisor/assets/airflow/kubernetes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 import json
 from pathlib import Path
 
 from airflow import DAG
 from airflow.utils.dates import days_ago
-from airflow.providers.cncf.kubernetes.operators.kubernetes_pod import (
-    KubernetesPodOperator,
-)
+from airflow.providers.cncf.kubernetes.operators.kubernetes_pod \
+    import KubernetesPodOperator
 
 default_args = {
-    "start_date": days_ago(0),
+    'start_date': days_ago(0),
 }
 
 dag = DAG(
-    dag_id="{{project_name}}",
+    dag_id='{{project_name}}',
     default_args=default_args,
-    description="Ploomber DAG ({{project_name}})",
+    description='Ploomber DAG ({{project_name}})',
     schedule_interval=None,
 )
 
-path_to_spec = Path(__file__).parent / "{{project_name}}.json"
+path_to_spec = Path(__file__).parent / '{{project_name}}.json'
 spec = json.loads(path_to_spec.read_text())
 
-for task in spec["tasks"]:
+for task in spec['tasks']:
     KubernetesPodOperator(
-        image=spec["image"],
-        cmds=["bash", "-cx"],
-        arguments=[task["command"]],
+        image=spec['image'],
+        cmds=['bash', '-cx'],
+        arguments=[task['command']],
         dag=dag,
-        task_id=task["name"],
-        name="{{project_name}}-pod",
+        task_id=task['name'],
+        name='{{project_name}}-pod',
         # if no File.client is configured, you may use volumes and
         # volume_mounts to share data among pods. See the tutorial in our
         # documentation for an example
         in_cluster=False,
         do_xcom_push=False,
         # if pulling a local image, set image_pull_policy='Never'
     )
 
-for task in spec["tasks"]:
-    t = dag.get_task(task["name"])
+for task in spec['tasks']:
+    t = dag.get_task(task['name'])
 
-    for upstream in task["upstream"]:
+    for upstream in task['upstream']:
         t.set_upstream(dag.get_task(upstream))
```

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/argo/template.yaml` & `soopervisor-0.9b1/src/soopervisor/assets/argo/template.yaml`

 * *Files identical despite different names*

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/README.md` & `soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/README.md`

 * *Files identical despite different names*

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/app.py` & `soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/app.py`

 * *Files identical despite different names*

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/template.yaml` & `soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/template.yaml`

 * *Files identical despite different names*

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/aws-lambda/test_aws_lambda.py` & `soopervisor-0.9b1/src/soopervisor/assets/aws-lambda/test_aws_lambda.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 import pytest
 
 import app
 
 
 @pytest.fixture
 def apigw_event():
-    raise NotImplementedError(
-        "Missing implementation in "
-        "{{package_name}}/test_aws_lambda.py. "
-        "Assign an example input to the body variable."
-    )
+    raise NotImplementedError("Missing implementation in "
+                              "{{package_name}}/test_aws_lambda.py. "
+                              "Assign an example input to the body variable.")
 
     # assign a valid sample input here
     body = None
 
     return {
         "body": json.dumps(body),
         "resource": "/{proxy+}",
@@ -37,41 +35,48 @@
                 "cognitoIdentityId": "",
                 "cognitoAuthenticationProvider": "",
                 "sourceIp": "127.0.0.1",
                 "accountId": "",
             },
             "stage": "prod",
         },
-        "queryStringParameters": {"foo": "bar"},
+        "queryStringParameters": {
+            "foo": "bar"
+        },
         "headers": {
-            "Via": "1.1 08f323deadbeefa7af34d5feb414ce27.cloudfront.net (CloudFront)",
+            "Via":
+            "1.1 08f323deadbeefa7af34d5feb414ce27.cloudfront.net (CloudFront)",
             "Accept-Language": "en-US,en;q=0.8",
             "CloudFront-Is-Desktop-Viewer": "true",
             "CloudFront-Is-SmartTV-Viewer": "false",
             "CloudFront-Is-Mobile-Viewer": "false",
             "X-Forwarded-For": "127.0.0.1, 127.0.0.2",
             "CloudFront-Viewer-Country": "US",
-            "Accept": (
-                "text/html,application/xhtml+xml,application/xml;"
-                "q=0.9,image/webp,*/*;q=0.8"
-            ),
+            "Accept":
+            ("text/html,application/xhtml+xml,application/xml;"
+             "q=0.9,image/webp,*/*;q=0.8"),
             "Upgrade-Insecure-Requests": "1",
             "X-Forwarded-Port": "443",
             "Host": "1234567890.execute-api.us-east-1.amazonaws.com",
             "X-Forwarded-Proto": "https",
-            "X-Amz-Cf-Id": "aaaaaaaaaae3VYQb9jd-nvCd-de396Uhbp027Y2JvkCPNLmGJHqlaA==",
+            "X-Amz-Cf-Id":
+            "aaaaaaaaaae3VYQb9jd-nvCd-de396Uhbp027Y2JvkCPNLmGJHqlaA==",
             "CloudFront-Is-Tablet-Viewer": "false",
             "Cache-Control": "max-age=0",
             "User-Agent": "Custom User Agent String",
             "CloudFront-Forwarded-Proto": "https",
             "Accept-Encoding": "gzip, deflate, sdch",
         },
-        "pathParameters": {"proxy": "/examplepath"},
+        "pathParameters": {
+            "proxy": "/examplepath"
+        },
         "httpMethod": "POST",
-        "stageVariables": {"baz": "qux"},
+        "stageVariables": {
+            "baz": "qux"
+        },
         "path": "/examplepath",
     }
 
 
 def test_lambda_handler(apigw_event):
     ret = app.handler(apigw_event, "")
```

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/docker/Dockerfile` & `soopervisor-0.9b1/src/soopervisor/assets/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `soopervisor-0.9.2/src/soopervisor/assets/kubeflow/Dockerfile` & `soopervisor-0.9b1/src/soopervisor/assets/kubeflow/Dockerfile`

 * *Files identical despite different names*

### Comparing `soopervisor-0.9.2/src/soopervisor/aws/batch.py` & `soopervisor-0.9b1/src/soopervisor/aws/batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from uuid import uuid4
 import os
 import json
 from pathlib import Path
 import fnmatch
 
 from ploomber.io._commander import Commander, CommanderStop
-from ploomber_core.dependencies import requires
+from ploomber.util.util import requires
+from ploomber.cloud import api
 
 from soopervisor.aws.config import AWSBatchConfig, CloudConfig
 from soopervisor.aws.util import TaskResources
 from soopervisor.commons import docker, source
 from soopervisor import commons
 from soopervisor import abc
 from soopervisor.commons.dependencies import get_default_image_key
@@ -47,21 +48,24 @@
 
 # FIXME: move this logic to ploomber so we validate it
 # before and after we submit the code
 def _transform_task_resources(resources):
     resources_out = []
 
     if resources.vcpus:
-        resources_out.append({"value": str(resources.vcpus), "type": "VCPU"})
+        resources_out.append({'value': str(resources.vcpus), 'type': 'VCPU'})
 
     if resources.memory:
-        resources_out.append({"value": str(resources.memory), "type": "MEMORY"})
+        resources_out.append({
+            'value': str(resources.memory),
+            'type': 'MEMORY'
+        })
 
     if resources.gpu:
-        resources_out.append({"value": str(resources.gpu), "type": "GPU"})
+        resources_out.append({'value': str(resources.gpu), 'type': 'GPU'})
 
     return resources_out
 
 
 def _validate_keys(task_resources, tasks):
     names = list(tasks)
 
@@ -71,32 +75,31 @@
     for pattern in task_resources:
         matches = fnmatch.filter(names, pattern)
 
         if not matches:
             faulty_keys.append(pattern)
 
     if faulty_keys:
-        faulty_keys_out = "\n* ".join(faulty_keys)
-        raise ValueError(
-            "The following keys in the task_resources section "
-            "did not match any pipeline tasks. Delete them "
-            "or ensure they match at least one task "
-            f"name:\n{faulty_keys_out}"
-        )
+        faulty_keys_out = '\n* '.join(faulty_keys)
+        raise ValueError('The following keys in the task_resources section '
+                         'did not match any pipeline tasks. Delete them '
+                         'or ensure they match at least one task '
+                         f'name:\n{faulty_keys_out}')
 
 
 def _process_task_resources(task_resources, tasks):
     if not task_resources:
         return {}
 
     _validate_keys(task_resources, tasks)
 
-    return TaskResources(
-        {key: _transform_task_resources(value) for key, value in task_resources.items()}
-    )
+    return TaskResources({
+        key: _transform_task_resources(value)
+        for key, value in task_resources.items()
+    })
 
 
 def _submit_dag(
     tasks,
     args,
     job_def,
     image_map,
@@ -106,112 +109,109 @@
     cmdr,
     is_cloud,
     cfg,
 ):
     default_image_key = get_default_image_key()
     remote_name = image_map[default_image_key]
 
-    client = boto3.client("batch", region_name=region_name)
-    container_properties["image"] = remote_name
+    client = boto3.client('batch', region_name=region_name)
+    container_properties['image'] = remote_name
 
     jd_map = {}
 
     task_resources = _process_task_resources(cfg.task_resources, tasks)
 
-    cmdr.info(f"Registering {job_def!r} job definition...")
+    cmdr.info(f'Registering {job_def!r} job definition...')
 
     job_ids = dict()
 
-    cmdr.info("Submitting jobs...")
+    cmdr.info('Submitting jobs...')
 
     if is_cloud:
         # docker.build moves to the env folder
-        params = json.loads(Path("../.ploomber-cloud").read_text())
+        params = json.loads(Path('../.ploomber-cloud').read_text())
 
         # note: this will trigger an error if the user has no quota left
-        from ploomber.cloud.api import PloomberCloudAPI
-
-        out = PloomberCloudAPI().runs_update(params["runid"], tasks)
+        out = api.runs_update(params['runid'], tasks)
     else:
         out, params = None, None
 
     jd = client.register_job_definition(
         jobDefinitionName=job_def,
-        type="container",
-        containerProperties=container_properties,
-    )
+        type='container',
+        containerProperties=container_properties)
     jd_map[default_image_key] = jd
 
     # Register job definitions for task specific images
     for pattern, image in image_map.items():
         if pattern != default_image_key:
             container_props = container_properties.copy()
-            container_props["image"] = image
+            container_props['image'] = image
             task_job_def = f"{job_def}-{docker.modify_wildcard(pattern)}"
-            cmdr.info(f"Registering {task_job_def!r} job definition...")
+            cmdr.info(f'Registering {task_job_def!r} job definition...')
 
             jd = client.register_job_definition(
                 jobDefinitionName=task_job_def,
-                type="container",
-                containerProperties=container_props,
-            )
+                type='container',
+                containerProperties=container_props)
             jd_map[pattern] = jd
 
     for name, upstream in tasks.items():
+
         task_pattern = _find_task_pattern(list(image_map.keys()), name)
         task_pattern = task_pattern if task_pattern else default_image_key
         task_jd = jd_map[task_pattern]
 
         if is_cloud:
             ploomber_task = [
-                "python",
-                "-m",
-                "ploomber.cli.task",
+                'python',
+                '-m',
+                'ploomber.cli.task',
                 name,
-                "--task-id",
-                out["taskids"][name],
+                '--task-id',
+                out['taskids'][name],
             ]
 
             container_overrides = {
-                "command": ploomber_task + args,
+                "command":
+                ploomber_task + args,
                 "environment": [
                     {
                         "name": "PLOOMBER_CLOUD_KEY",
-                        "value": os.environ["PLOOMBER_CLOUD_KEY"],
+                        "value": os.environ["PLOOMBER_CLOUD_KEY"]
                     },
                     {
                         "name": "PLOOMBER_CLOUD_HOST",
-                        "value": os.environ["PLOOMBER_CLOUD_HOST"],
+                        "value": os.environ["PLOOMBER_CLOUD_HOST"]
                     },
-                ],
+                ]
             }
 
         else:
-            ploomber_task = ["ploomber", "task", name]
+            ploomber_task = ['ploomber', 'task', name]
             container_overrides = {"command": ploomber_task + args}
 
         # add requested resources
-        container_overrides["resourceRequirements"] = task_resources.get(name, [])
+        container_overrides['resourceRequirements'] = task_resources.get(
+            name, [])
 
-        response = client.submit_job(
-            jobName=name,
-            jobQueue=job_queue,
-            jobDefinition=task_jd["jobDefinitionArn"],
-            dependsOn=[{"jobId": job_ids[name]} for name in upstream],
-            containerOverrides=container_overrides,
-        )
+        response = client.submit_job(jobName=name,
+                                     jobQueue=job_queue,
+                                     jobDefinition=task_jd['jobDefinitionArn'],
+                                     dependsOn=[{
+                                         "jobId": job_ids[name]
+                                     } for name in upstream],
+                                     containerOverrides=container_overrides)
 
         job_ids[name] = response["jobId"]
 
-        cmdr.print(f"Submitted task {name!r}...")
+        cmdr.print(f'Submitted task {name!r}...')
 
     if is_cloud:
-        from ploomber.cloud.api import PloomberCloudAPI
-
-        PloomberCloudAPI().runs_register_ids(params["runid"], job_ids)
+        api.runs_register_ids(params['runid'], job_ids)
 
 
 class AWSBatchExporter(abc.AbstractExporter):
     CONFIG_CLASS = AWSBatchConfig
 
     @classmethod
     def _submit_dag(cls, *args, **kwargs):
@@ -223,117 +223,93 @@
 
     @classmethod
     def _no_tasks_to_submit(cls):
         pass
 
     @staticmethod
     def _add(cfg, env_name):
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as e:
-            e.copy_template(
-                "docker/Dockerfile",
-                conda=Path("environment.lock.yml").exists(),
-                setup_py=Path("setup.py").exists(),
-                lib=Path("lib").exists(),
-                env_name=env_name,
-            )
-            e.success("Done")
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as e:
+            e.copy_template('aws-batch/Dockerfile',
+                            conda=Path('environment.lock.yml').exists(),
+                            setup_py=Path('setup.py').exists(),
+                            lib=Path('lib').exists(),
+                            env_name=env_name)
+            e.success('Done')
             e.print(
-                f"Fill in the configuration in the {env_name!r} "
-                "section in soopervisor.yaml then submit to AWS Batch with: "
-                f"soopervisor export {env_name}"
-            )
+                f'Fill in the configuration in the {env_name!r} '
+                'section in soopervisor.yaml then submit to AWS Batch with: '
+                f'soopervisor export {env_name}')
 
         # TODO: run dag checks: client configured, ploomber status
 
     @classmethod
-    @requires(["boto3"], name="AWSBatchExporter")
-    def _export(
-        cls,
-        cfg,
-        env_name,
-        mode,
-        until,
-        skip_tests,
-        skip_docker,
-        ignore_git,
-        lazy_import,
-        task_name,
-    ):
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as cmdr:
-            tasks, cli_args = commons.load_tasks(
-                cmdr=cmdr,
-                name=env_name,
-                mode=mode,
-                lazy_import=lazy_import,
-                task_name=task_name,
-            )
+    @requires(['boto3'], name='AWSBatchExporter')
+    def _export(cls, cfg, env_name, mode, until, skip_tests, skip_docker,
+                ignore_git, lazy_import, task_name):
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as cmdr:
+
+            tasks, cli_args = commons.load_tasks(cmdr=cmdr,
+                                                 name=env_name,
+                                                 mode=mode,
+                                                 lazy_import=lazy_import,
+                                                 task_name=task_name)
 
             if not tasks:
                 cls._no_tasks_to_submit()
-                raise CommanderStop(
-                    f"Loaded DAG in {mode!r} mode has no "
-                    'tasks to submit. Try "--mode force" to '
-                    "submit all tasks regardless of status"
-                )
+                raise CommanderStop(f'Loaded DAG in {mode!r} mode has no '
+                                    'tasks to submit. Try "--mode force" to '
+                                    'submit all tasks regardless of status')
             if skip_docker:
                 pkg_name, version = source.find_package_name_and_version()
                 default_image_key = get_default_image_key()
                 if default_image_key:
-                    image_local = f"{pkg_name}:{version}-"
-                    f"{docker.modify_wildcard(default_image_key)}"
+                    image_local = f'{pkg_name}:{version}-'
+                    f'{docker.modify_wildcard(default_image_key)}'
                 image_map = {}
                 image_map[default_image_key] = image_local
             else:
-                pkg_name, image_map = docker.build(
-                    cmdr,
-                    cfg,
-                    env_name,
-                    until=until,
-                    entry_point=cli_args[1],
-                    skip_tests=skip_tests,
-                    ignore_git=ignore_git,
-                )
+                pkg_name, image_map = docker.build(cmdr,
+                                                   cfg,
+                                                   env_name,
+                                                   until=until,
+                                                   entry_point=cli_args[1],
+                                                   skip_tests=skip_tests,
+                                                   ignore_git=ignore_git)
 
-            cmdr.info("Submitting jobs to AWS Batch")
+            cmdr.info('Submitting jobs to AWS Batch')
 
             # add a unique suffix to prevent collisions
             suffix = str(uuid4())[:8]
 
-            cls._submit_dag(
-                tasks=tasks,
-                args=cli_args,
-                job_def=f"{pkg_name}-{suffix}",
-                image_map=image_map,
-                job_queue=cfg.job_queue,
-                container_properties=cfg.container_properties,
-                region_name=cfg.region_name,
-                cmdr=cmdr,
-                cfg=cfg,
-            )
+            cls._submit_dag(tasks=tasks,
+                            args=cli_args,
+                            job_def=f'{pkg_name}-{suffix}',
+                            image_map=image_map,
+                            job_queue=cfg.job_queue,
+                            container_properties=cfg.container_properties,
+                            region_name=cfg.region_name,
+                            cmdr=cmdr,
+                            cfg=cfg)
 
-            cmdr.success("Done. Submitted to AWS Batch")
+            cmdr.success('Done. Submitted to AWS Batch')
 
 
 def _find_task_pattern(task_patterns, current_task):
     for p in [re.compile(t) for t in task_patterns]:
         if p.match(current_task):
             return p.pattern
 
 
 # TODO: add tests
 class CloudExporter(AWSBatchExporter):
     CONFIG_CLASS = CloudConfig
 
     @classmethod
     def _no_tasks_to_submit(cls):
-        from ploomber.cloud.api import PloomberCloudAPI
-
-        params = json.loads(Path(".ploomber-cloud").read_text())
-        PloomberCloudAPI().run_finished(params["runid"])
+        params = json.loads(Path('.ploomber-cloud').read_text())
+        api.run_finished(params['runid'])
 
     @classmethod
     def _submit_dag(cls, *args, **kwargs):
         return _submit_dag(*args, **kwargs, is_cloud=True)
```

### Comparing `soopervisor-0.9.2/src/soopervisor/aws/config.py` & `soopervisor-0.9b1/src/soopervisor/aws/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class TaskResource(BaseModel):
     vcpus: int = None
     memory: int = None
     gpu: int = None
 
     class Config:
-        extra = "forbid"
+        extra = 'forbid'
 
 
 class AWSBatchConfig(AbstractDockerConfig):
     # in AWSBatch, repository cannot be None
     repository: str
 
     container_properties: dict
@@ -27,23 +27,21 @@
 
     @classmethod
     def get_backend_value(cls):
         return Backend.aws_batch.value
 
     @classmethod
     def _hints(cls):
-        return dict(
-            repository="your-repository/name",
-            job_queue="your-job-queue",
-            region_name="your-region-name",
-            container_properties=dict(
-                memory=16384,
-                vcpus=8,
-            ),
-        )
+        return dict(repository='your-repository/name',
+                    job_queue='your-job-queue',
+                    region_name='your-region-name',
+                    container_properties=dict(
+                        memory=16384,
+                        vcpus=8,
+                    ))
 
 
 class CloudConfig(AWSBatchConfig):
     @classmethod
     def get_backend_value(cls):
         return Backend.cloud.value
```

### Comparing `soopervisor-0.9.2/src/soopervisor/aws/lambda_.py` & `soopervisor-0.9b1/src/soopervisor/aws/lambda_.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,52 +18,51 @@
 class AWSLambdaExporter(abc.AbstractExporter):
     CONFIG_CLASS = AWSLambdaConfig
 
     def export(self, mode=None, until=None, skip_tests=False):
         if mode is not None:
             raise ValueError("AWS Lambda does not support 'mode'")
 
-        return self._export(
-            cfg=self._cfg, env_name=self._env_name, until=until, skip_tests=skip_tests
-        )
+        return self._export(cfg=self._cfg,
+                            env_name=self._env_name,
+                            until=until,
+                            skip_tests=skip_tests)
 
     @staticmethod
     def _validate(cfg, dag, env_name):
         pass
 
     @staticmethod
     def _add(cfg, env_name):
         try:
             pkg_name = default.find_package_name()
         except ValueError as e:
             raise ClickException(
-                "AWS Lambda is only supported in packaged projects. "
-                "See the documentation for an example."
-            ) from e
-
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as e:
-            e.copy_template("aws-lambda/README.md")
-            e.copy_template("aws-lambda/Dockerfile", lib=Path("lib").exists())
+                'AWS Lambda is only supported in packaged projects. '
+                'See the documentation for an example.') from e
 
-            e.copy_template("aws-lambda/test_aws_lambda.py", package_name=pkg_name)
-            e.copy_template("aws-lambda/app.py", package_name=pkg_name)
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as e:
+            e.copy_template('aws-lambda/README.md')
+            e.copy_template('aws-lambda/Dockerfile', lib=Path('lib').exists())
+
+            e.copy_template('aws-lambda/test_aws_lambda.py',
+                            package_name=pkg_name)
+            e.copy_template('aws-lambda/app.py', package_name=pkg_name)
 
-            e.copy_template("aws-lambda/template.yaml", package_name=pkg_name)
-            e.success("Done.")
+            e.copy_template('aws-lambda/template.yaml', package_name=pkg_name)
+            e.success('Done.')
             e.print(
-                "Next steps:\n1. Add an input example to "
-                f"{env_name}/test_aws_lambda.py\n"
-                f"2. Add the input parsing logic to {env_name}/app.py\n"
-                f"3. Submit to AWS Lambda with: soopervisor export {env_name}"
-            )
+                'Next steps:\n1. Add an input example to '
+                f'{env_name}/test_aws_lambda.py\n'
+                f'2. Add the input parsing logic to {env_name}/app.py\n'
+                f'3. Submit to AWS Lambda with: soopervisor export {env_name}')
 
             # TODO: use e.warn_on_exit
-            for name in ["docker", "aws", "sam"]:
+            for name in ['docker', 'aws', 'sam']:
                 warn_if_not_installed(name)
 
     @staticmethod
     def _export(cfg, env_name, until, skip_tests):
 
         # TODO: validate project structure: src/*/model.*, etc...
 
@@ -71,67 +70,65 @@
         # bdist?
         # TODO: warn if deploying from a dirty commit, maybe ask for
         # confirmation
         # and show the version?
         # TODO: support for OnlineDAG in app.py
         # TODO: check if OnlineModel can be initialized from the package
 
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as e:
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as e:
 
             commons.dependencies.check_lock_files_exist()
 
-            if (
-                not Path("requirements.lock.txt").exists()
-                and Path("environment.lock.yml").exists()
-            ):
+            if not Path('requirements.lock.txt').exists() and Path(
+                    'environment.lock.yml').exists():
                 e.warn_on_exit(
-                    "Missing requirements.lock.txt file. "
-                    "Once was created from the pip "
-                    "section in the environment.lock.yml file but this "
-                    "may not work if there are missing dependencies. Add "
-                    "one or ensure environment.lock.yml includes all pip "
-                    "dependencies."
-                )
-
-                generate_reqs_txt_from_env_yml(
-                    "environment.lock.yml", output="requirements.lock.txt"
-                )
-                e.rm_on_exit("requirements.lock.txt")
+                    'Missing requirements.lock.txt file. '
+                    'Once was created from the pip '
+                    'section in the environment.lock.yml file but this '
+                    'may not work if there are missing dependencies. Add '
+                    'one or ensure environment.lock.yml includes all pip '
+                    'dependencies.')
+
+                generate_reqs_txt_from_env_yml('environment.lock.yml',
+                                               output='requirements.lock.txt')
+                e.rm_on_exit('requirements.lock.txt')
 
-            e.cp("requirements.lock.txt")
+            e.cp('requirements.lock.txt')
 
             # TODO: ensure user has pytest before running
             if not skip_tests:
-                e.run("pytest", env_name, description="Testing")
+                e.run('pytest', env_name, description='Testing')
 
-            e.rm("dist", "build")
-            e.run("python", "-m", "build", "--wheel", ".", description="Packaging")
-            e.cp("dist")
+            e.rm('dist', 'build')
+            e.run('python',
+                  '-m',
+                  'build',
+                  '--wheel',
+                  '.',
+                  description='Packaging')
+            e.cp('dist')
 
             e.cd(env_name)
 
             # TODO: template.yaml with version number
 
-            e.run("sam", "build", description="Building Docker image")
+            e.run('sam', 'build', description='Building Docker image')
 
-            if until == "build":
+            if until == 'build':
                 e.tw.write(
                     'Done.\nRun "docker images" to see your image.'
-                    '\nRun "sam local start-api" to test your API locally'
-                )
+                    '\nRun "sam local start-api" to test your API locally')
                 return
 
-            args = ["sam", "deploy"]
+            args = ['sam', 'deploy']
 
-            if Path("samconfig.toml").exists():
-                e.warn(
-                    "samconfig.toml already exists. Skipping " "guided deployment..."
-                )
+            if Path('samconfig.toml').exists():
+                e.warn('samconfig.toml already exists. Skipping '
+                       'guided deployment...')
             else:
-                args.append("--guided")
-                e.info("Starting guided deployment...")
+                args.append('--guided')
+                e.info('Starting guided deployment...')
 
-            e.run(*args, description="Deploying")
+            e.run(*args, description='Deploying')
 
-            e.success("Deployed to AWS Lambda")
+            e.success('Deployed to AWS Lambda')
```

### Comparing `soopervisor-0.9.2/src/soopervisor/aws/util.py` & `soopervisor-0.9b1/src/soopervisor/aws/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import fnmatch
 import shutil
 
 
 def warn_if_not_installed(name):
     if not shutil.which(name):
-        print(
-            f"It appears you don't have {name} CLI installed, you need it "
-            'to execute "invoke aws-lambda build"'
-        )
+        print(f'It appears you don\'t have {name} CLI installed, you need it '
+              'to execute "invoke aws-lambda build"')
 
 
 class TaskResources:
     """
     An object to pattern match task names with the task_resources
     section in cloud.yaml
     """
-
     def __init__(self, mapping):
         self._mapping = mapping
 
     def get(self, task_name, default=None):
         for pattern, value in self._mapping.items():
             if fnmatch.fnmatch(task_name, pattern):
                 return value
```

### Comparing `soopervisor-0.9.2/src/soopervisor/cli.py` & `soopervisor-0.9b1/src/soopervisor/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,136 +22,147 @@
     $ soopervisor export training
 
     """
     pass
 
 
 @cli.command()
-@click.argument("env_name")
-@click.option("--backend", "-b", type=click.Choice(Backend.get_values()), required=True)
-@click.option(
-    "--preset", "-p", help="Customizes settings (backend-specific)", default=None
-)
+@click.argument('env_name')
+@click.option('--backend',
+              '-b',
+              type=click.Choice(Backend.get_values()),
+              required=True)
+@click.option('--preset',
+              '-p',
+              help='Customizes settings (backend-specific)',
+              default=None)
 def add(env_name, backend, preset):
     """
     Add a new target platform. Creates a 'soopervisor.yaml' file if needed
 
     Example: soopervisor add cluster-training -b argo-workflows
     """
     backend = Backend(backend)
 
     try:
-        if Path("soopervisor.yaml").exists():
-            cfg = yaml.safe_load(Path("soopervisor.yaml").read_text())
+        if Path('soopervisor.yaml').exists():
+            cfg = yaml.safe_load(Path('soopervisor.yaml').read_text())
             if env_name in cfg:
                 raise click.ClickException(
-                    f"A {env_name!r} section in the "
-                    "soopervisor.yaml configuration file "
-                    "already exists. Choose another name."
-                )
+                    f'A {env_name!r} section in the '
+                    'soopervisor.yaml configuration file '
+                    'already exists. Choose another name.')
         if Path(env_name).exists():
             raise click.ClickException(
-                f"{env_name!r} already exists. Select a different name."
-            )
+                f'{env_name!r} already exists. Select a different name.')
     except Exception as e:
-        telemetry.log_api(
-            "soopervisor_add_error",
-            metadata={"type": backend.value, "env_name": env_name, "error": str(e)},
-        )
+        telemetry.log_api("soopervisor_add_error",
+                          metadata={
+                              'type': backend.value,
+                              'env_name': env_name,
+                              'error': str(e)
+                          })
         raise
 
     Exporter = exporter.for_backend(backend)
-    Exporter.new("soopervisor.yaml", env_name=env_name, preset=preset).add()
+    Exporter.new('soopervisor.yaml', env_name=env_name, preset=preset).add()
 
-    telemetry.log_api(
-        "soopervisor_add_success",
-        metadata={"type": backend.value, "env_name": env_name},
-    )
-
-    click.echo(
-        "Environment added, to export it:\n"
-        f"\t $ soopervisor export {env_name}\n"
-        "To force execution of all tasks:\n"
-        f"\t $ soopervisor export {env_name} "
-        "--mode force\n"
-    )
+    telemetry.log_api("soopervisor_add_success",
+                      metadata={
+                          'type': backend.value,
+                          'env_name': env_name
+                      })
+
+    click.echo('Environment added, to export it:\n'
+               f'\t $ soopervisor export {env_name}\n'
+               'To force execution of all tasks:\n'
+               f'\t $ soopervisor export {env_name} '
+               '--mode force\n')
 
 
 @cli.command()
-@click.argument("env_name")
-@click.option("--until-build", "-u", is_flag=True, help="Only build docker image")
-@click.option("--skip-tests", "-s", is_flag=True, help="Skip docker image tests")
-@click.option("--skip-docker", "-S", is_flag=True, help="Skip docker build")
-@click.option(
-    "--mode", "-m", type=click.Choice(Mode.get_values()), default=Mode.incremental.value
-)
-@click.option(
-    "--ignore-git",
-    "-i",
-    is_flag=True,
-    help="Ignore git tracked files (include everything)",
-)
-@click.option("--lazy", "-l", is_flag=True, help="Lazily load pipeline")
-@click.option(
-    "--task", "-t", type=str, help="Execute a single task with the given name"
-)
-def export(
-    env_name, until_build, mode, skip_tests, skip_docker, ignore_git, lazy, task
-):
+@click.argument('env_name')
+@click.option('--until-build',
+              '-u',
+              is_flag=True,
+              help='Only build docker image')
+@click.option('--skip-tests',
+              '-s',
+              is_flag=True,
+              help='Skip docker image tests')
+@click.option('--skip-docker', '-S', is_flag=True, help='Skip docker build')
+@click.option('--mode',
+              '-m',
+              type=click.Choice(Mode.get_values()),
+              default=Mode.incremental.value)
+@click.option('--ignore-git',
+              '-i',
+              is_flag=True,
+              help='Ignore git tracked files (include everything)')
+@click.option('--lazy', '-l', is_flag=True, help='Lazily load pipeline')
+@click.option('--task',
+              '-t',
+              type=str,
+              help='Execute a single task with the given name')
+def export(env_name, until_build, mode, skip_tests, skip_docker, ignore_git,
+           lazy, task):
     """
     Export a target platform for execution/deployment
     """
     input_args = {
-        "env_name": env_name,
-        "until_build": until_build,
-        "mode": mode,
-        "skip_tests": skip_tests,
-        "skip_docker": skip_docker,
-        "ignore_git": ignore_git,
-        "task": task,
+        'env_name': env_name,
+        'until_build': until_build,
+        'mode': mode,
+        'skip_tests': skip_tests,
+        'skip_docker': skip_docker,
+        'ignore_git': ignore_git,
+        'task': task,
     }
 
     backend = Backend(config.get_backend(env_name))
 
-    telemetry.log_api(
-        "soopervisor_export_started",
-        metadata={"type": backend.value, "input_args": input_args},
-    )
+    telemetry.log_api("soopervisor_export_started",
+                      metadata={
+                          'type': backend.value,
+                          'input_args': input_args
+                      })
 
     until = None
 
     if until_build:
-        until = "build"
+        until = 'build'
 
     # TODO: ignore mode if using aws lambda, raised exception if value
     # is not the default
     if backend == Backend.aws_lambda:
         mode = None
 
     Exporter = exporter.for_backend(backend)
 
     try:
-        Exporter.load("soopervisor.yaml", env_name=env_name, lazy_import=lazy).export(
-            mode=mode,
-            until=until,
-            skip_tests=skip_tests,
-            skip_docker=skip_docker,
-            ignore_git=ignore_git,
-            lazy_import=lazy,
-            task_name=task,
-        )
+        Exporter.load('soopervisor.yaml', env_name=env_name,
+                      lazy_import=lazy).export(mode=mode,
+                                               until=until,
+                                               skip_tests=skip_tests,
+                                               skip_docker=skip_docker,
+                                               ignore_git=ignore_git,
+                                               lazy_import=lazy,
+                                               task_name=task)
 
     except Exception as e:
-        telemetry.log_api(
-            "soopervisor_export_error",
-            metadata={"type": backend.value, "input_args": input_args, "error": str(e)},
-        )
+        telemetry.log_api("soopervisor_export_error",
+                          metadata={
+                              'type': backend.value,
+                              'input_args': input_args,
+                              'error': str(e)
+                          })
         raise
 
-    telemetry.log_api(
-        "soopervisor_export_success",
-        metadata={"type": backend.value, "input_args": input_args},
-    )
+    telemetry.log_api("soopervisor_export_success",
+                      metadata={
+                          'type': backend.value,
+                          'input_args': input_args
+                      })
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     cli()
```

### Comparing `soopervisor-0.9.2/src/soopervisor/commons/conda.py` & `soopervisor-0.9b1/src/soopervisor/commons/conda.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,39 +4,36 @@
 
 import yaml
 
 
 def extract_pip_from_env_yaml(path):
     env = yaml.safe_load(Path(path).read_text())
 
-    if "dependencies" not in env:
+    if 'dependencies' not in env:
         raise ClickException(
-            "Cannot extract pip dependencies from "
-            "environment.lock.yml: missing dependencies section"
-        )
+            'Cannot extract pip dependencies from '
+            'environment.lock.yml: missing dependencies section')
 
-    deps = env["dependencies"]
+    deps = env['dependencies']
 
     for dep in deps:
         if isinstance(dep, Mapping):
-            if "pip" in dep:
-                deps_pip = dep["pip"]
+            if 'pip' in dep:
+                deps_pip = dep['pip']
 
                 if not isinstance(deps_pip, list):
                     raise ClickException(
-                        "Cannot extract pip dependencies "
-                        "from environment.lock.yml: unexpected "
-                        "dependencies.pip value. Expected a "
-                        f"list of dependencies, got: {deps_pip}"
-                    )
+                        'Cannot extract pip dependencies '
+                        'from environment.lock.yml: unexpected '
+                        'dependencies.pip value. Expected a '
+                        f'list of dependencies, got: {deps_pip}')
 
                 return deps_pip
 
     raise ClickException(
-        "Cannot extract pip dependencies from "
-        "environment.lock.yml: missing dependencies.pip section"
-    )
+        'Cannot extract pip dependencies from '
+        'environment.lock.yml: missing dependencies.pip section')
 
 
 def generate_reqs_txt_from_env_yml(path, output):
     reqs = extract_pip_from_env_yaml(path)
-    Path(output).write_text("\n".join(reqs))
+    Path(output).write_text('\n'.join(reqs))
```

### Comparing `soopervisor-0.9.2/src/soopervisor/commons/dag.py` & `soopervisor-0.9b1/src/soopervisor/commons/dag.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def _is_relative_path(path):
     return not Path(path).is_absolute()
 
 
 def _extract_product_parent(task_spec):
-    product_spec = task_spec.data["product"]
+    product_spec = task_spec.data['product']
 
     try:
         # single product
         paths = [Path(product_spec)]
     except TypeError:
         # dictionary
         try:
@@ -34,43 +34,43 @@
             # any other thing
             return []
 
     return [str(path.parent) for path in paths if _is_relative_path(path)]
 
 
 def product_prefixes_from_spec(spec):
-    parents = [_extract_product_parent(t) for t in spec["tasks"]]
+    parents = [_extract_product_parent(t) for t in spec['tasks']]
     parents_flat = [path for sub in parents for path in sub]
     return sorted(set(parents_flat)) or None
 
 
 def find_spec(cmdr, name, lazy_import=False):
     """
     Find spec to use. It first tries to load a file with pipeline.{name}.yaml,
     if that doesn't exist, it tries to load a pipeline.yaml
     """
-    cmdr.info("Loading DAG")
+    cmdr.info('Loading DAG')
 
     try:
-        spec, relative_path = DAGSpec._find_relative(name=name, lazy_import=lazy_import)
-        cmdr.print(f"Found {spec.path!s}. Loading...")
+        spec, relative_path = DAGSpec._find_relative(name=name,
+                                                     lazy_import=lazy_import)
+        cmdr.print(f'Found {spec.path!s}. Loading...')
     except DAGSpecInvalidError:
-        cmdr.print(
-            f"No pipeline.{name}.yaml found, " "looking for pipeline.yaml instead"
-        )
+        cmdr.print(f'No pipeline.{name}.yaml found, '
+                   'looking for pipeline.yaml instead')
         spec = None
 
     if spec is None:
         spec, relative_path = DAGSpec._find_relative(lazy_import=lazy_import)
-        cmdr.print(f"Found {spec.path!s}. Loading...")
+        cmdr.print(f'Found {spec.path!s}. Loading...')
 
     return spec, relative_path
 
 
-def load_dag(cmdr, name=None, mode="incremental", lazy_import=False):
+def load_dag(cmdr, name=None, mode='incremental', lazy_import=False):
     """Load DAG object
 
     Parameters
     ----------
     cmdr : Commander
         Commander instance used to print output
 
@@ -89,21 +89,23 @@
     Returns
     -------
     dag : class
         A DAG class - collection of tasks with dependencies (values)
     relative_path : str
         The relative location of the pipeline.yaml file
     """
-    value_in(name="mode", value=mode, values=Mode.get_values())
+    value_in(name='mode', value=mode, values=Mode.get_values())
 
-    spec, relative_path = find_spec(cmdr=cmdr, name=name, lazy_import=lazy_import)
+    spec, relative_path = find_spec(cmdr=cmdr,
+                                    name=name,
+                                    lazy_import=lazy_import)
     dag = spec.to_dag()
 
-    if mode == "incremental":
-        with add_to_sys_path(".", chdir=False):
+    if mode == 'incremental':
+        with add_to_sys_path('.', chdir=False):
             has_client = dag.clients.get(File) is not None
 
         # what if user has a shared disk but still wants to upload artifacts?
         # maybe add a way to force this
         if has_client:
             dag.render(remote=True)
         else:
@@ -113,15 +115,19 @@
         # force makes rendering faster. we just need this to ensure the
         # pipeline does not have any rendering problems before proceeding
         dag.render(force=True)
 
     return dag, relative_path
 
 
-def load_tasks(cmdr, name=None, mode="incremental", lazy_import=False, task_name=None):
+def load_tasks(cmdr,
+               name=None,
+               mode='incremental',
+               lazy_import=False,
+               task_name=None):
     """Get tasks to execute and their upstream dependencies
 
     Parameters
     ----------
     cmdr : Commander
         Commander instance used to print output
 
@@ -154,24 +160,24 @@
     # user selected a single task
     if task_name:
         task = dag.get(task_name)
 
         if task is None:
             raise NotATaskError(task_name, dag)
 
-        if task.exec_status == TaskStatus.Skipped and mode == "incremental":
+        if task.exec_status == TaskStatus.Skipped and mode == 'incremental':
             # TODO: this will show a "--mode force" message but this only
             # applies when using soopervisor directly, and does not apply
             # when using ploomber cloud
             raise UpToDateTaskError(task_name)
 
         tasks = [task_name]
 
     # if incremental, only get the tasks that are outdated
-    elif mode == "incremental":
+    elif mode == 'incremental':
         tasks = []
 
         for name, task in dag.items():
             if not mode or task.exec_status != TaskStatus.Skipped:
                 tasks.append(name)
 
     # otherwise, get all tasks
@@ -181,25 +187,27 @@
     # get upstream
     out = {}
 
     for t in tasks:
         # add a task as upstream dependency if it's a task that we will execute
         out[t] = [name for name in dag[t].upstream.keys() if name in tasks]
 
-    args = ["--entry-point", relative_path]
+    args = ['--entry-point', relative_path]
 
-    if mode == "force":
-        args.append("--force")
+    if mode == 'force':
+        args.append('--force')
 
     return out, args
 
 
 def load_dag_and_spec(env_name, lazy_import=False):
     # initialize dag (needed for validation)
     # TODO: _export also has to find_spec, maybe load it here and
     # pass it directly to _export?
     with Commander() as cmdr:
-        spec, _ = commons.find_spec(cmdr=cmdr, name=env_name, lazy_import=lazy_import)
+        spec, _ = commons.find_spec(cmdr=cmdr,
+                                    name=env_name,
+                                    lazy_import=lazy_import)
 
     dag = spec.to_dag().render(force=True, show_progress=False)
 
     return dag, spec
```

### Comparing `soopervisor-0.9.2/src/soopervisor/commons/dependencies.py` & `soopervisor-0.9b1/src/soopervisor/commons/dependencies.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import click
 
 from pathlib import Path
 from collections import defaultdict
 
-DEFAULT_IMAGE_NAME = "default"
+DEFAULT_IMAGE_NAME = 'default'
 
 
 def _no_missing_dependencies(prefix, suffix):
     tasks = get_task_dependency_files(prefix, suffix)
     if len(tasks) > 1:
         # If multiple dependency file present, every
         # requirements.task-__.txt/ environment.task-__.yml file
         # should have a corresponding requirements.task-__.lock.txt/
         # environment.-__.lock.yml file
         for task_pattern, paths in tasks.items():
-            if "dependency" not in paths or "lock" not in paths:
+            if 'dependency' not in paths or 'lock' not in paths:
                 return False
     return len(tasks) > 0
 
 
-def get_task_dependency_files(prefix, suffix, lock="lock"):
+def get_task_dependency_files(prefix, suffix, lock='lock'):
     """
     Return all requirements/ environment files
     for each task in the below dict format:
     {
       task_name : { 'dependency' : path,
                  'lock': path of lock file
                }
@@ -37,53 +37,48 @@
         requirements / environment
 
     suffix : str
         txt / yml
 
     """
     task_files = defaultdict(dict)
-    matched_files = [path.name for path in list(Path(".").glob(f"{prefix}*.{suffix}"))]
+    matched_files = [
+        path.name for path in list(Path('.').glob(f"{prefix}*.{suffix}"))
+    ]
     for filename in matched_files:
-        task_name = [s for s in filename.split(".") if s not in (prefix, lock, suffix)]
-        task_name = (
-            DEFAULT_IMAGE_NAME if not task_name else task_name[0].replace("__", "*")
-        )
+        task_name = [
+            s for s in filename.split(".") if s not in (prefix, lock, suffix)
+        ]
+        task_name = DEFAULT_IMAGE_NAME if not task_name else task_name[
+            0].replace('__', '*')
         if lock in filename:
-            task_files[task_name]["lock"] = filename
+            task_files[task_name]['lock'] = filename
         else:
-            task_files[task_name]["dependency"] = filename
+            task_files[task_name]['dependency'] = filename
     return task_files
 
 
 def get_default_image_key():
     return DEFAULT_IMAGE_NAME
 
 
 def check_lock_files_exist():
-    if (
-        not Path("environment.lock.yml").exists()
-        and not Path("requirements.lock.txt").exists()
-    ):
-        raise click.ClickException(
-            """
+    if not Path('environment.lock.yml').exists() and not Path(
+            'requirements.lock.txt').exists():
+        raise click.ClickException("""
 Expected requirements.lock.txt or environment.lock.yml at the root directory, \
 add one and try again.
 
 pip: pip freeze > requirements.lock.txt
 conda: conda env export --no-build --file environment.lock.yml
-"""
-        )
+""")
 
-    if not (
-        _no_missing_dependencies("requirements", "txt")
-        or _no_missing_dependencies("environment", "yml")
-    ):
-        raise click.ClickException(
-            """
+    if not (_no_missing_dependencies('requirements', 'txt')
+            or _no_missing_dependencies('environment', 'yml')):
+        raise click.ClickException("""
         Expected requirements.<task-name>.lock.txt file for \
         each requirements.<task-name>.txt file OR \
         environment.<task-name>.lock.yml for each \
         environment.<task-name>.yml file at the root directory.
         Add relevant files and try again.
 
-        """
-        )
+        """)
```

### Comparing `soopervisor-0.9.2/src/soopervisor/commons/source.py` & `soopervisor-0.9b1/src/soopervisor/commons/source.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,54 +14,53 @@
 
 def find_package_name_and_version():
     # if this is a pkg, get the name
     try:
         pkg_name = default.find_package_name()
     # if not a package, use the parent folder's name
     except ValueError:
-        pkg_name = Path(".").resolve().name
-        version = "latest"
+        pkg_name = Path('.').resolve().name
+        version = 'latest'
     else:
         # if using versioneer, the version may contain "+"
-        version = importlib.import_module(pkg_name).__version__.replace("+", "-plus-")
+        version = importlib.import_module(pkg_name).__version__.replace(
+            '+', '-plus-')
 
     return pkg_name, version
 
 
 def git_tracked_files():
     """
     Returns
     -------
     list or None
         List of tracked files or None if an error happened
     None of str
         None if successfully retrieved tracked files, str if an error happened
     """
-    res = subprocess.run(
-        ["git", "ls-tree", "-r", "HEAD", "--name-only"],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-    )
+    res = subprocess.run(['git', 'ls-tree', '-r', 'HEAD', '--name-only'],
+                         stdout=subprocess.PIPE,
+                         stderr=subprocess.PIPE)
 
     if not res.returncode:
         return res.stdout.decode().splitlines(), None
     else:
         return None, res.stderr.decode().strip()
 
 
 def git_is_dirty():
     """
     Returns True if there are git untracked files (new files that haven't been
     committed yet)
     """
-    res = subprocess.run(
-        ["git", "status", "--short"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
-    )
+    res = subprocess.run(['git', 'status', '--short'],
+                         stdout=subprocess.PIPE,
+                         stderr=subprocess.PIPE)
 
-    return not (res.returncode or "??" not in res.stdout.decode())
+    return not (res.returncode or '??' not in res.stdout.decode())
 
 
 def is_relative_to(path, prefix):
     if prefix is None:
         return False
 
     try:
@@ -73,33 +72,40 @@
 
 
 def is_relative_to_any(path, prefixes):
     return any(is_relative_to(path, prefix) for prefix in prefixes)
 
 
 def glob_all(path, exclude=None):
-    hidden = iglob(str(Path(path) / "**" / ".*"), recursive=True)
-    normal = iglob(str(Path(path) / "**"), recursive=True)
+    hidden = iglob(str(Path(path) / '**' / '.*'), recursive=True)
+    normal = iglob(str(Path(path) / '**'), recursive=True)
 
     for path in chain(hidden, normal):
         if Path(path).is_file() and not is_relative_to(path, exclude):
             yield path
 
 
 def to_posix_str(path):
     return str(PurePosixPath(*Path(path).parts))
 
 
 def size_too_big(path, mb):
-    """Returns true is file is too large"""
+    """Returns true is file is too large
+    """
     total_mb = mb * 1048576
     return os.path.getsize(path) > total_mb
 
 
-def copy(cmdr, src, dst, include=None, exclude=None, ignore_git=False, rename_files={}):
+def copy(cmdr,
+         src,
+         dst,
+         include=None,
+         exclude=None,
+         ignore_git=False,
+         rename_files={}):
     """Copy files
 
     Parameters
     ----------
     cmdr : Commander
         Commander object
 
@@ -127,84 +133,77 @@
     include_dirs = set(p for p in include if Path(p).is_dir())
 
     overlap = set(include) & set(exclude)
 
     big_files = []
 
     if overlap:
-        raise ClickException(
-            "include and exclude must not have " f"overlapping elements: {overlap}"
-        )
+        raise ClickException('include and exclude must not have '
+                             f'overlapping elements: {overlap}')
 
     if git_is_dirty():
-        cmdr.warn_on_exit(
-            "Your git repository contains uncommitted "
-            "files, which will be ignored when building the "
-            "Docker image. Commit them if needed."
-        )
+        cmdr.warn_on_exit('Your git repository contains uncommitted '
+                          'files, which will be ignored when building the '
+                          'Docker image. Commit them if needed.')
 
     tracked, error = git_tracked_files()
 
     if error:
         cmdr.warn_on_exit(
-            f"Unable to get git tracked files: {error}. Everything "
-            "will be included, except for files in the 'exclude' section "
-            "of soopervisor.yaml"
-        )
+            f'Unable to get git tracked files: {error}. Everything '
+            'will be included, except for files in the \'exclude\' section '
+            'of soopervisor.yaml')
 
     if not tracked and not error and not ignore_git:
-        raise ClickException(
-            "Running inside a git repository, but no files "
-            "in the current working directory are tracked "
-            "by git. Commit the files to include them in "
-            "the Docker image or pass the --ignore-git "
-            "flag to soopervisor export"
-        )
+        raise ClickException("Running inside a git repository, but no files "
+                             "in the current working directory are tracked "
+                             "by git. Commit the files to include them in "
+                             "the Docker image or pass the --ignore-git "
+                             "flag to soopervisor export")
 
     for f in glob_all(path=src, exclude=dst):
-        tracked_by_git = tracked is None or ignore_git or to_posix_str(f) in tracked
+        tracked_by_git = (tracked is None or ignore_git
+                          or to_posix_str(f) in tracked)
         excluded = f in exclude or is_relative_to_any(f, exclude_dirs)
         included = f in include or is_relative_to_any(f, include_dirs)
         # never include .git or .gitignore
-        never_include = Path(f).name.startswith(".git") or "__pycache__" in f
-        if (tracked_by_git or included) and not excluded and not never_include:
+        never_include = Path(f).name.startswith('.git') or '__pycache__' in f
+        if ((tracked_by_git or included) and not excluded
+                and not never_include):
             if f in rename_files:
                 target = Path(dst, rename_files[f])
             else:
                 target = Path(dst, f)
             target.parent.mkdir(exist_ok=True, parents=True)
             shutil.copy(f, dst=target)
-            print(f"Copying {f} -> {target}")
+            print(f'Copying {f} -> {target}')
 
             # checking file size
             if size_too_big(f, 10):
                 big_files.append(f)
 
     if len(big_files) > 0:
         click.secho(
-            "\nThe following files are too big. "
-            "this will increase the docker image size "
-            "so ensure this is required to run the pipeline: \n",
-            fg="yellow",
-        )
+            '\nThe following files are too big. '
+            'this will increase the docker image size '
+            'so ensure this is required to run the pipeline: \n',
+            fg='yellow')
 
         for file in big_files:
             # size in MB
             size = "{:.2f}".format(os.path.getsize(f) / 1048576)
-            click.secho(f"Filename: {file} Size:{size} MB", fg="yellow")
+            click.secho(f'Filename: {file} Size:{size} MB', fg='yellow')
 
-        click.secho("\n")
+        click.secho('\n')
 
 
 def compress_dir(cmdr, src, dst):
     print("Compressing directory , src : {}, dst : {}".format(src, dst))
     with tarfile.open(dst, "w:gz") as tar:
         tar.add(src, arcname=os.path.basename(src))
 
     if size_too_big(dst, 5):
-        cmdr.warn_on_exit(
-            f"The project's source code {str(dst)!r} is "
-            "larger than 5MB, there may be some unnecessary "
-            "files (e.g., data files)"
-        )
+        cmdr.warn_on_exit(f"The project's source code {str(dst)!r} is "
+                          "larger than 5MB, there may be some unnecessary "
+                          "files (e.g., data files)")
 
     shutil.rmtree(src)
```

### Comparing `soopervisor-0.9.2/src/soopervisor/config.py` & `soopervisor-0.9b1/src/soopervisor/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,54 +12,51 @@
     """
     Loads soopervisor.yaml and loads the configuration for an env with the
     passed name. Performs validations before returning the configuration
     """
     validate.config_file_exists()
 
     # load soopervisor.yaml
-    cfg = yaml.safe_load(Path("soopervisor.yaml").read_text())
+    cfg = yaml.safe_load(Path('soopervisor.yaml').read_text())
 
     # get section with that name
     if name not in cfg:
         raise exceptions.ConfigurationError(
             f'Missing {name!r} section in {"soopervisor.yaml"!r}. '
-            f"Available ones are: {comma_separated(cfg)}"
-        )
+            f'Available ones are: {comma_separated(cfg)}')
 
     section = cfg[name]
 
     # check if there is a backend key
-    if "backend" not in section:
+    if 'backend' not in section:
         raise exceptions.ConfigurationError(
-            "Misconfigured environment: missing "
-            f"'backend' key in section {name!r} in "
-            "'soopervisor.yaml'"
-        )
+            'Misconfigured environment: missing '
+            f'\'backend\' key in section {name!r} in '
+            '\'soopervisor.yaml\'')
 
-    backend = section["backend"]
+    backend = section['backend']
 
     # check if the value is valid
     if backend not in Backend:
         valid = comma_separated(Backend.__members__.keys())
         raise exceptions.ConfigurationError(
-            f"Misconfigured environment: {backend!r} is "
-            f"not a valid backend. backend must be one of: {valid}"
-        )
+            f'Misconfigured environment: {backend!r} is '
+            f'not a valid backend. backend must be one of: {valid}')
 
     return backend
 
 
 def replace_env(env_name, target_dir):
     """
     For a given target directory, renames env.{env_name}.yaml to env.yaml
     """
-    env = Path(target_dir, f"env.{env_name}.yaml")
+    env = Path(target_dir, f'env.{env_name}.yaml')
 
     if env.exists():
-        env_general = Path(target_dir, "env.yaml")
+        env_general = Path(target_dir, 'env.yaml')
 
         if env_general.exists():
             env_general.unlink()
         else:
-            click.echo(f"No {env} found...")
+            click.echo(f'No {env} found...')
 
         env.rename(env_general)
```

### Comparing `soopervisor-0.9.2/src/soopervisor/enum.py` & `soopervisor-0.9b1/src/soopervisor/enum.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,29 @@
             return False
         else:
             return True
 
 
 @unique
 class Backend(Enum, metaclass=CustomEnum):
-    aws_batch = "aws-batch"
-    aws_lambda = "aws-lambda"
-    argo_workflows = "argo-workflows"
-    airflow = "airflow"
-    kubeflow = "kubeflow"
-    slurm = "slurm"
-    cloud = "cloud"
+    aws_batch = 'aws-batch'
+    aws_lambda = 'aws-lambda'
+    argo_workflows = 'argo-workflows'
+    airflow = 'airflow'
+    kubeflow = 'kubeflow'
+    slurm = 'slurm'
+    cloud = 'cloud'
 
     @classmethod
     def get_values(cls):
         return [v.value for v in cls.__members__.values()]
 
 
 @unique
 class Mode(Enum, metaclass=CustomEnum):
-    incremental = "incremental"
-    regular = "regular"
-    force = "force"
+    incremental = 'incremental'
+    regular = 'regular'
+    force = 'force'
 
     @classmethod
     def get_values(cls):
         return [v.value for v in cls.__members__.values()]
```

### Comparing `soopervisor-0.9.2/src/soopervisor/exceptions.py` & `soopervisor-0.9b1/src/soopervisor/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,90 +2,86 @@
 
 from click import ClickException
 
 from soopervisor._format import comma_separated
 
 
 class BackendWithoutPresetsError(ClickException):
-    """Raises when passing a preset to a backend doesn't have any"""
+    """Raises when passing a preset to a backend doesn't have any
+    """
 
     def __init__(self, backend):
-        super().__init__(
-            f"Backend {str(backend)!r} does not have " "presets. Remove the argument."
-        )
+        super().__init__(f'Backend {str(backend)!r} does not have '
+                         'presets. Remove the argument.')
 
 
 class InvalidPresetForBackendError(ClickException):
-    """Raised if the passed preset is not valid for the passed backend"""
+    """Raised if the passed preset is not valid for the passed backend
+    """
 
     def __init__(self, backend, preset, preset_values):
-        super().__init__(
-            f"Preset {preset!r} is not a valid value for "
-            f"backend {str(backend)!r}. Valid presets are: "
-            f"{comma_separated(preset_values)}"
-        )
+        super().__init__(f'Preset {preset!r} is not a valid value for '
+                         f'backend {str(backend)!r}. Valid presets are: '
+                         f'{comma_separated(preset_values)}')
 
 
 class ConfigurationError(ClickException):
     """
     Raised when there is a misconfiguration. Captured by the CLI to only
     show the error message and not the whole traceback
     """
-
     pass
 
 
 class MissingDockerfileError(ClickException):
     """
     Raised when trying to build a Docker image but the DockerFile is missing
     """
 
     def __init__(self, env_name):
         self.env_name = env_name
-        path = str(Path(env_name, "Dockerfile"))
+        path = str(Path(env_name, 'Dockerfile'))
         message = f"""\
 Expected Dockerfile at {path!r} but it does not exist\
         """
         super().__init__(message)
 
 
 class MissingConfigurationFileError(ClickException):
     """
     Raised if soopervisor.yaml is missing
     """
 
     def __init__(self):
-        name = "soopervisor.yaml"
-        super().__init__(
-            f"Expected a {name!r} file in the current "
-            "working directory, but such files does not exist"
-        )
+        name = 'soopervisor.yaml'
+        super().__init__(f'Expected a {name!r} file in the current '
+                         'working directory, but such files does not exist')
 
 
 class ConfigurationFileTypeError(ClickException):
-    """Raised if the configuration file does not have the right type"""
+    """Raised if the configuration file does not have the right type
+    """
 
     def __init__(self, path, data):
-        super().__init__(
-            f"Expected {str(path)!r} to contain a dictionary "
-            f"but got an object of type: {type(data).__name__}"
-        )
+        super().__init__(f'Expected {str(path)!r} to contain a dictionary '
+                         f'but got an object of type: {type(data).__name__}')
 
 
 class NotATaskError(ClickException):
     """
     Raised when a user passes an invalid task name
     """
 
     def __init__(self, task_name, dag):
         names = comma_separated(dag.keys())
-        super().__init__(f"{task_name!r} is not a valit task name. Tasks are: {names}")
+        super().__init__(
+            f'{task_name!r} is not a valit task name. Tasks are: {names}')
 
 
 class UpToDateTaskError(ClickException):
-    """Raised when a user tries to submit a task that is up-to-date"""
+    """Raised when a user tries to submit a task that is up-to-date
+    """
 
     def __init__(self, task_name):
         super().__init__(
-            f"Task {task_name!r} is up-to-date, to force execution, "
-            "pass: --mode force"
-        )
+            f'Task {task_name!r} is up-to-date, to force execution, '
+            'pass: --mode force')
```

### Comparing `soopervisor-0.9.2/src/soopervisor/exporter.py` & `soopervisor-0.9b1/src/soopervisor/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
         Backend.kubeflow: KubeflowExporter,
         Backend.argo_workflows: ArgoWorkflowsExporter,
         Backend.slurm: SlurmExporter,
         Backend.cloud: CloudExporter,
     }
 
     if backend not in Backend:
-        raise ValueError(f"{backend!r} is not a valid backend")
+        raise ValueError(f'{backend!r} is not a valid backend')
 
     return mapping[backend]
```

### Comparing `soopervisor-0.9.2/src/soopervisor/kubeflow/export.py` & `soopervisor-0.9b1/src/soopervisor/kubeflow/export.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,199 +19,179 @@
 
     @staticmethod
     def _add(cfg, env_name):
         """Export Ploomber project to Kubeflow
 
         Generates a .py file that exposes a dag variable
         """
-        click.echo("Exporting to Kubeflow...")
+        click.echo('Exporting to Kubeflow...')
 
         # TODO: modify Dockerfile depending on package or non-package
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as e:
-            e.copy_template(
-                "kubeflow/Dockerfile",
-                conda=Path("environment.lock.yml").exists(),
-                lib=Path("lib").exists(),
-                setup_py=Path("setup.py").exists(),
-            )
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as e:
+            e.copy_template('kubeflow/Dockerfile',
+                            conda=Path('environment.lock.yml').exists(),
+                            lib=Path('lib').exists(),
+                            setup_py=Path('setup.py').exists())
 
     @staticmethod
     def _validate(cfg, dag, env_name):
         """
         Validates a project before exporting as an Kubeflow DAG.
         This runs as a sanity check in the development machine
         """
         pass
 
     @staticmethod
-    def _export(
-        cfg,
-        env_name,
-        mode,
-        until,
-        skip_tests,
-        skip_docker,
-        ignore_git,
-        lazy_import,
-        task_name,
-    ):
+    def _export(cfg, env_name, mode, until, skip_tests, skip_docker,
+                ignore_git, lazy_import, task_name):
         """
         Copies the current source code to the target environment folder.
         The code along with the DAG declaration file can be copied to
         KUBEFLOW_HOME for execution
         """
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as e:
-            tasks, args = commons.load_tasks(
-                cmdr=e, name=env_name, mode=mode, task_name=task_name
-            )
-            dag, relative_path = commons.load_dag(
-                cmdr=e, name=env_name, mode=mode, lazy_import=lazy_import
-            )
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as e:
+            tasks, args = commons.load_tasks(cmdr=e,
+                                             name=env_name,
+                                             mode=mode,
+                                             task_name=task_name)
+            dag, relative_path = commons.load_dag(cmdr=e,
+                                                  name=env_name,
+                                                  mode=mode,
+                                                  lazy_import=lazy_import)
             products_list = {}
 
             # TODO deal with the second mode.
             for name, task in dag.items():
                 product = task.product
                 products_list[name] = []
                 try:
                     product.items()
                     products = product.products.products
                     for item in products:
                         products_list[name].append(
-                            {item: str(Path(products[item]).resolve())}
-                        )
+                            {item: str(Path(products[item]).resolve())})
                 except AttributeError:  # Single product
                     products_list[name].append(str(Path(product).resolve()))
 
             if not tasks:
-                raise CommanderStop(
-                    f"Loaded DAG in {mode!r} mode has no "
-                    'tasks to submit. Try "--mode force" to '
-                    "submit all tasks regardless of status"
-                )
+                raise CommanderStop(f'Loaded DAG in {mode!r} mode has no '
+                                    'tasks to submit. Try "--mode force" to '
+                                    'submit all tasks regardless of status')
             if skip_docker:
-                click.secho("Skipping docker build")
+                click.secho('Skipping docker build')
                 pkg_name, version = source.find_package_name_and_version()
                 default_image_key = get_default_image_key()
                 if default_image_key:
-                    image_local = f"{pkg_name}:{version}-"
-                    f"{commons.docker.modify_wildcard(default_image_key)}"
+                    image_local = f'{pkg_name}:{version}-'
+                    f'{commons.docker.modify_wildcard(default_image_key)}'
                 target_image = image_local
             else:
                 pkg_name, target_image = commons.docker.build(
                     e,
                     cfg,
                     env_name,
                     until=until,
                     entry_point=args[1],
                     skip_tests=skip_tests,
-                    ignore_git=ignore_git,
-                )
+                    ignore_git=ignore_git)
 
             print("Generating kubeflow script")
-            generate_kubeflow_script(
-                tasks, args, products_list, target_image, pkg_name, env_name
-            )
+            generate_kubeflow_script(tasks, args, products_list, target_image,
+                                     pkg_name, env_name)
 
             print("Compiling to a kubeflow yaml")
-            output_path = f"{env_name}/kubeflow_pipeline.yaml"
+            output_path = f'{env_name}/kubeflow_pipeline.yaml'
             os.system(f"python kubeflow_pipeline.py {output_path}")
 
-            click.echo(f"Done. Saved kubeflow yaml to {output_path!r}")
+            click.echo(f'Done. Saved kubeflow yaml to {output_path!r}')
             click.echo(
-                "Submit your workflow through:\n"
-                "1. Direct upload to cluster\n"
-                "2. Client API call: client.create_run_from_pipeline_package("
-                f"{output_path}, arguments=None)"
-            )
+                'Submit your workflow through:\n'
+                '1. Direct upload to cluster\n'
+                '2. Client API call: client.create_run_from_pipeline_package('
+                f'{output_path}, arguments=None)')
 
 
 def _make_kubeflow_dag(name, dependencies, command):
     dag_task = {
         "name": name,
         "template": name,
     }
 
     if dependencies:
-        dag_task["dependencies"] = dependencies
-        dag_task["arguments"] = {"artifacts": []}
+        dag_task['dependencies'] = dependencies
+        dag_task['arguments'] = {'artifacts': []}
         for dependency in dependencies:
-            dag_task["arguments"]["artifacts"].append(
-                {
-                    "name": f"{dependency}-product",
-                    "from": "{{tasks."
-                    + dependency
-                    + ".outputs.artifacts."
-                    + dependency
-                    + "-product}}",
-                }
-            )
+            dag_task['arguments']['artifacts'].append({
+                'name':
+                f'{dependency}-product',
+                'from':
+                '{{tasks.' + dependency + '.outputs.artifacts.' + dependency +
+                '-product}}'
+            })
 
     return dag_task
 
 
 def _parse_task_dependencies(tasks, dependencies, products, task_name):
     headers = []
     args = []
 
     # Parse task inputs
     if dependencies:
-        headers.append("inputs:\n")
+        headers.append('inputs:\n')
 
         for dependency in dependencies:
-            headers.append("- {name: " + dependency + "}\n")
+            headers.append('- {name: ' + dependency + '}\n')
 
     # Parse task outputs
     task_products = products[task_name]
     if task_products:
-        headers.append("outputs:\n")
-        args.append("        args:\n")
+        headers.append('outputs:\n')
+        args.append('        args:\n')
         if len(task_products) == 1:
-            headers.append("- {name: product}\n")
-            args.append("        - {outputPath: product}\n")
+            headers.append('- {name: product}\n')
+            args.append('        - {outputPath: product}\n')
         else:
             for product in task_products:
                 key = list(product.keys())[0]
-                headers.append("- {name: " + key + "}\n")
-                args.append("        - {outputPath: " + key + "}\n")
+                headers.append('- {name: ' + key + '}\n')
+                args.append('        - {outputPath: ' + key + '}\n')
 
     return args, headers
 
 
 def _parse_pipeline_task(tasks, dependencies, products, task_name):
     pipeline = []
     if dependencies:
-        pipeline.append(f"  {task_name}_step = {task_name}(\n")
+        pipeline.append(f'  {task_name}_step = {task_name}(\n')
 
         if len(dependencies) == 1:  # No ending comma
             item = dependencies[0]
             pipeline.append(f'      {item}_step.outputs["product"]\n')
-            pipeline.append("   )\n\n")
+            pipeline.append('   )\n\n')
         else:
             ctr = 0
             for item in dependencies:
                 item_products = products[item]
                 if len(item_products) == 1:
                     pipeline.append(f'      {item}_step.outputs["product"]')
                 else:
                     for product in item_products:
                         key = list(product.keys())[0]
                         pipeline.append(f'      {item}_step.outputs["{key}"]')
                 if ctr != len(dependencies) - 1:
-                    pipeline.append(",\n")
+                    pipeline.append(',\n')
                 else:
-                    pipeline.append("\n")
+                    pipeline.append('\n')
                 ctr += 1
-            pipeline.append("   )\n\n")
+            pipeline.append('   )\n\n')
     else:
-        pipeline.append(f"  {task_name}_step = {task_name}()\n\n")
+        pipeline.append(f'  {task_name}_step = {task_name}()\n\n')
 
     return pipeline
 
 
 def _parse_pipeline_tasks(tasks, target_image, products, args, pkg_name):
     tasks_lines = []
     pipeline_lines = []
@@ -219,48 +199,49 @@
         # Make sure if the task has an underscore it's converted to dash
         command = f'ploomber task {task_name.replace("_", "-")}'
 
         if args:
             command = f'{command} {" ".join(args)}'
 
         # Write task definition and text content
-        tasks_lines.append(f'{task_name} = comp.load_component_from_text("""\n')
-        tasks_lines.append(f"name: {task_name}\n")
+        tasks_lines.append(
+            f'{task_name} = comp.load_component_from_text("""\n')
+        tasks_lines.append(f'name: {task_name}\n')
 
         # Deal with task inputs outputs
         kubeflow_args, dependency_lines = _parse_task_dependencies(
-            tasks, upstream, products, task_name
-        )
+            tasks, upstream, products, task_name)
         if dependency_lines:
             tasks_lines += dependency_lines
 
-        tasks_lines.append("implementation:\n")
-        tasks_lines.append("    container:\n")
-        tasks_lines.append(f"        image: {target_image}\n")
-        tasks_lines.append("        command:\n")
-        tasks_lines.append("        - sh\n")
-        tasks_lines.append("        - -c\n")
-        tasks_lines.append("        - |\n")
+        tasks_lines.append('implementation:\n')
+        tasks_lines.append('    container:\n')
+        tasks_lines.append(f'        image: {target_image}\n')
+        tasks_lines.append('        command:\n')
+        tasks_lines.append('        - sh\n')
+        tasks_lines.append('        - -c\n')
+        tasks_lines.append('        - |\n')
         for index in range(0, len(kubeflow_args) - 1):
             tasks_lines.append(f'          mkdir -p "$(dirname "${index}")"\n')
-        tasks_lines.append(f"          {command}\n")
+        tasks_lines.append(f'          {command}\n')
 
         # Deal with output/input kubeflow_args
         if kubeflow_args:
             tasks_lines += kubeflow_args
 
         tasks_lines.append('""")\n\n')
 
-        pipeline_lines += _parse_pipeline_task(tasks, upstream, products, task_name)
+        pipeline_lines += _parse_pipeline_task(tasks, upstream, products,
+                                               task_name)
 
     # Create the pipeline
-    tasks_lines.append("# Define your pipeline\n")
-    tasks_lines.append(f"def {pkg_name}():\n")
+    tasks_lines.append('# Define your pipeline\n')
+    tasks_lines.append(f'def {pkg_name}():\n')
     tasks_lines += pipeline_lines
-    tasks_lines.append("\n")
+    tasks_lines.append('\n')
 
     return tasks_lines
 
 
 def filter_dict(tasks, to_replace, replace_with):
     new_tasks = {}
     for k, v in tasks.items():
@@ -276,58 +257,51 @@
             else:
                 new_v.append(key)
         new_tasks[new_k] = new_v
 
     return new_tasks
 
 
-def generate_kubeflow_script(tasks, args, products, target_image, pkg_name, env_name):
+def generate_kubeflow_script(tasks, args, products, target_image, pkg_name,
+                             env_name):
     """
     Generates a dictionary with the spec used by Kubeflow to construct the
     DAG and pipeline.yaml
     """
 
     # Make sure tasks/producs/pkg_name doesn't contain dashes
     tasks = filter_dict(tasks, "-", "_")
-    products = {k.replace("-", "_"): v for k, v in products.items()}
-    pkg_name = pkg_name.replace("-", "_")
-    fname = "kubeflow_pipeline.py"
+    products = {k.replace('-', '_'): v for k, v in products.items()}
+    pkg_name = pkg_name.replace('-', '_')
+    fname = 'kubeflow_pipeline.py'
 
     try:
-        with open(fname, "w") as f:
+        with open(fname, 'w') as f:
 
             # Initialize imports
-            f.write("import kfp\n")
-            f.write("import kfp.components as comp\n")
-            f.write("import kfp.compiler as compiler\n\n")
-            f.write(
-                "# Put your KFP cluster endpoint URL here if working from"
-                " GCP notebooks (or local notebooks). "
-                '("https://xxxxx.notebooks.googleusercontent.com/")\n'
-            )
+            f.write('import kfp\n')
+            f.write('import kfp.components as comp\n')
+            f.write('import kfp.compiler as compiler\n\n')
+            f.write('# Put your KFP cluster endpoint URL here if working from'
+                    ' GCP notebooks (or local notebooks). '
+                    '("https://xxxxx.notebooks.googleusercontent.com/")\n')
             f.write('#kfp_endpoint="YOUR_KFP_ENDPOINT"\n')
-            f.write("#client = kfp.Client(kfp_endpoint)\n\n")
-            f.write(
-                "# This is a sanity check to make sure your notebook and"
-                " cluster can communicate\n"
-            )
-            f.write("#print(client.list_experiments())\n\n")
+            f.write('#client = kfp.Client(kfp_endpoint)\n\n')
+            f.write('# This is a sanity check to make sure your notebook and'
+                    ' cluster can communicate\n')
+            f.write('#print(client.list_experiments())\n\n')
 
             # Parse single pipeline tasks
             f.writelines(
-                _parse_pipeline_tasks(tasks, target_image, products, args, pkg_name)
-            )
+                _parse_pipeline_tasks(tasks, target_image, products, args,
+                                      pkg_name))
 
             # API call to submit the pipeline
-            f.write("# Compile, and submit this pipeline for execution.\n")
+            f.write('# Compile, and submit this pipeline for execution.\n')
             f.write(f'pipeline_name = "{pkg_name}"\n')
-            f.write(
-                f"compiler.Compiler().compile({pkg_name}, "
-                'f"ploomber_pipeline.yaml")\n'
-            )
-            f.write(
-                f"#client.create_run_from_pipeline_func({pkg_name}, " "arguments={})\n"
-            )
+            f.write(f'compiler.Compiler().compile({pkg_name}, '
+                    'f"ploomber_pipeline.yaml")\n')
+            f.write(f'#client.create_run_from_pipeline_func({pkg_name}, '
+                    'arguments={})\n')
     except FileExistsError:
-        print(
-            f"Trying to write to an existing file, please remove" f" {fname} and retry"
-        )
+        print(f"Trying to write to an existing file, please remove"
+              f" {fname} and retry")
```

### Comparing `soopervisor-0.9.2/src/soopervisor/shell/export.py` & `soopervisor-0.9b1/src/soopervisor/shell/export.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,133 +12,114 @@
 from soopervisor import commons
 from soopervisor.shell.config import SlurmConfig
 from soopervisor import validate
 
 
 def _warn_on_exit_if_param(cmdr, param, name):
     if param:
-        cmdr.warn_on_exit(
-            f"{name!r} option has no effect when " "using SLURM, ignoring..."
-        )
+        cmdr.warn_on_exit(f'{name!r} option has no effect when '
+                          'using SLURM, ignoring...')
 
 
 def _check_template_variables(env, source):
     return meta.find_undeclared_variables(env.parse(source))
 
 
 def _validate_template(env, source):
     vars = _check_template_variables(env, source)
-    validate.keys(
-        {"command", "name"}, vars, "Error validating template.sh, missing placeholders"
-    )
+    validate.keys({'command', 'name'}, vars,
+                  'Error validating template.sh, missing placeholders')
 
 
 def _script_name_for_task_name(name, workspace):
     """
     Returns the path to the script to use based on the task name
     """
-    name_sh = f"{name}.sh"
+    name_sh = f'{name}.sh'
     exact_match = Path(workspace, name_sh)
 
     if exact_match.is_file():
         return exact_match
 
     files = sorted(os.listdir(workspace))
 
     for file in files:
-        if fnmatch.fnmatch(name_sh, file.replace("__", "*")):
+        if fnmatch.fnmatch(name_sh, file.replace('__', '*')):
             return Path(workspace, file)
 
-    return Path(workspace, "template.sh")
+    return Path(workspace, 'template.sh')
 
 
 # TODO: check ploomber version
 # TODO: submit all tasks to a single node
 class SlurmExporter(abc.AbstractExporter):
     CONFIG_CLASS = SlurmConfig
 
     @staticmethod
     def _add(cfg, env_name):
         """
         Add sample template
         """
-        with Commander(
-            workspace=env_name,
-            templates_path=("soopervisor", "assets"),
-            environment_kwargs=dict(
-                variable_start_string="[[",
-                variable_end_string="]]",
-            ),
-        ) as e:
-            e.copy_template("slurm/template.sh")
-            e.success("Done")
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets'),
+                       environment_kwargs=dict(
+                           variable_start_string='[[',
+                           variable_end_string=']]',
+                       )) as e:
+            e.copy_template('slurm/template.sh')
+            e.success('Done')
 
     @staticmethod
     def _validate(cfg, dag, env_name):
         pass
 
     @classmethod
     def validate(cls):
         """
         Override method from the abstract class, since it validates lock files
         exist, but we don't need those for SLURM
         """
         pass
 
     @staticmethod
-    def _export(
-        cfg,
-        env_name,
-        mode,
-        until,
-        skip_tests,
-        skip_docker,
-        ignore_git,
-        lazy_import,
-        task_name,
-    ):
+    def _export(cfg, env_name, mode, until, skip_tests, skip_docker,
+                ignore_git, lazy_import, task_name):
         """
         Export and submit jbs
         """
-        with Commander(
-            workspace=env_name, templates_path=("soopervisor", "assets")
-        ) as cmdr:
+        with Commander(workspace=env_name,
+                       templates_path=('soopervisor', 'assets')) as cmdr:
 
             # these do not apply when using SLURM, warn the user
             # TODO: test the warning is shown
-            _warn_on_exit_if_param(cmdr, ignore_git, "ignore_git")
-            _warn_on_exit_if_param(cmdr, until, "until")
-            _warn_on_exit_if_param(cmdr, skip_tests, "skip_tests")
-            _warn_on_exit_if_param(cmdr, skip_docker, "skip_docker")
+            _warn_on_exit_if_param(cmdr, ignore_git, 'ignore_git')
+            _warn_on_exit_if_param(cmdr, until, 'until')
+            _warn_on_exit_if_param(cmdr, skip_tests, 'skip_tests')
+            _warn_on_exit_if_param(cmdr, skip_docker, 'skip_docker')
 
-            template = Path(env_name, "template.sh").read_text()
+            template = Path(env_name, 'template.sh').read_text()
             _validate_template(cmdr._env, template)
 
-            tasks, args = commons.load_tasks(
-                cmdr=cmdr,
-                name=env_name,
-                mode=mode,
-                lazy_import=lazy_import,
-                task_name=task_name,
-            )
+            tasks, args = commons.load_tasks(cmdr=cmdr,
+                                             name=env_name,
+                                             mode=mode,
+                                             lazy_import=lazy_import,
+                                             task_name=task_name)
 
             if not tasks:
-                raise CommanderStop(
-                    f"Loaded DAG in {mode!r} mode has no "
-                    'tasks to submit. Try "--mode force" to '
-                    "submit all tasks regardless of status"
-                )
+                raise CommanderStop(f'Loaded DAG in {mode!r} mode has no '
+                                    'tasks to submit. Try "--mode force" to '
+                                    'submit all tasks regardless of status')
 
             # FIXME: add unit test for this
-            if not shutil.which("sbatch"):
+            if not shutil.which('sbatch'):
                 raise CommanderException(
-                    "sbatch is not installed, but it is "
-                    "required to submit the jobs to the cluster, "
-                    "please install it and try again."
-                )
+                    'sbatch is not installed, but it is '
+                    'required to submit the jobs to the cluster, '
+                    'please install it and try again.')
 
             _submit_to_slurm(tasks, args, env_name)
 
 
 def _submit_to_slurm(tasks, args, workspace):
     """
     Script to submit tasks in a Ploomber pipeline as SLURM jobs.
@@ -159,39 +140,39 @@
     for name, upstream in tasks.items():
 
         # determine which script file to use
         script_sh = _script_name_for_task_name(name, workspace)
         # generate script and save
         job_sh = Template(script_sh.read_text())
 
-        ploomber_command = " ".join(["ploomber", "task", name] + args)
+        ploomber_command = ' '.join(['ploomber', 'task', name] + args)
         script = job_sh.render(name=name, command=ploomber_command)
-        Path("_job.sh").write_text(script)
+        Path('_job.sh').write_text(script)
 
         # does the task have dependencies?
         if upstream:
             # if yes, then use --dependency=afterok:
-            ids = ":".join([name2id[task_name] for task_name in upstream])
+            ids = ':'.join([name2id[task_name] for task_name in upstream])
             # docs: https://hpc.nih.gov/docs/job_dependencies.html
             # https://slurm.schedmd.com/sbatch.html
             # sbatch [options] script [args...]
             cmd = [
-                "sbatch",
-                f"--dependency=afterok:{ids}",
-                "--parsable",
+                'sbatch',
+                f'--dependency=afterok:{ids}',
+                '--parsable',
                 # kill job if upstream dependencies fail
-                "--kill-on-invalid-dep=yes",
-                "_job.sh",
+                '--kill-on-invalid-dep=yes',
+                '_job.sh',
             ]
         else:
             # if no, just submit
-            cmd = ["sbatch", "--parsable", "_job.sh"]
+            cmd = ['sbatch', '--parsable', '_job.sh']
 
         # print the submitted command
         click.echo(f'Running command: {" ".join(cmd)}')
-        click.echo(f"_job.sh content:\n{script}")
+        click.echo(f'_job.sh content:\n{script}')
 
         # submit job
         res = run(cmd, capture_output=True, check=True)
 
         # retrieve the job id, we'll use this to register --dependency
         name2id[name] = res.stdout.decode().strip()
```

### Comparing `soopervisor-0.9.2/src/soopervisor/validate.py` & `soopervisor-0.9b1/src/soopervisor/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from pathlib import Path
 
 from soopervisor.exceptions import MissingConfigurationFileError
 
 
 def value_in(*, name, value, values):
     if value not in values:
-        raise ValueError(f"{name!r} must be one of {pprint(values)}, got: {value!r}")
+        raise ValueError(
+            f"{name!r} must be one of {pprint(values)}, got: {value!r}")
 
 
 def pprint(collection):
-    return ", ".join(f"'{element}'" for element in sorted(collection))
+    return ', '.join(f"'{element}'" for element in sorted(collection))
 
 
 def keys(expected, actual, error):
     missing = set(expected) - set(actual)
 
     if missing:
-        raise ValueError(f"{error}: {pprint(missing)}")
+        raise ValueError(f'{error}: {pprint(missing)}')
 
 
 def config_file_exists():
-    if not Path("soopervisor.yaml").is_file():
+    if not Path('soopervisor.yaml').is_file():
         raise MissingConfigurationFileError()
```

### Comparing `soopervisor-0.9.2/src/soopervisor.egg-info/PKG-INFO` & `soopervisor-0.9b1/src/soopervisor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: soopervisor
-Version: 0.9.2
+Version: 0.9b1
+Summary: UNKNOWN
 Home-page: https://github.com/ploomber/soopervisor
 Author: 
 Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
@@ -32,16 +35,14 @@
    :target: https://github.com/ploomber/soopervisor/workflows/CI%20macOS/badge.svg
    :alt: CI macOS badge
 
 .. image:: https://github.com/ploomber/soopervisor/workflows/CI%20Windows/badge.svg
    :target: https://github.com/ploomber/soopervisor/workflows/CI%20Windows/badge.svg
    :alt: CI Windows badge
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
 
 Soopervisor runs `Ploomber <https://github.com/ploomber/ploomber>`_ pipelines
 for batch processing (large-scale training or batch serving) or online
 inference.
 
 .. code-block:: sh
 
@@ -105,29 +106,21 @@
 Whatever your skillset is, you can contribute to our mission. So whether you're a beginner or an experienced professional, you're welcome to join us on this journey!
 
 `Click here to know how you can contribute to Ploomber. <https://github.com/ploomber/contributing/blob/main/README.md>`_
 
 CHANGELOG
 =========
 
-0.9.2 (2023-07-18)
-------------------
-* Replaces `@requires` import to use `ploomber_core` instead of `ploomber`
-
-0.9.1 (2022-10-24)
-------------------
-* Adds `--skip-docker` argument in `soopervisor export` to skip docker build (#103)
-* Optimizes the generated AWS Batch ``Dockerfile`` so dependencies are only installed when the requirements are modified
-* Allows using multiple ``requirements.txt`` files, generating one Docker image for each one (#86)
-
-0.9 (2022-10-03)
-----------------
-* Allows execution of single tasks via ``soopervisor export --task {task-name}``
-* Allowing to bundle custom libraries via ``lib/`` in docker image (#87)
-* Fixes DAG loading when passing the ``--lazy`` argument in pipelines with a ``File`` client (#105)
+0.8.1dev
+--------
+* Allos execution of single tasks via `soopervisor export --task {task-name}`
+* Allows using multiple `requirements.txt` files, generating one Docker image for each one (#86)
+* Allowing to bundle custom libraries via `lib/` in docker image (#87)
+* Adding `--skip-docker` argument in `soopervisor export` to skip docker build ([#103](https://github.com/ploomber/soopervisor/issues/103))
+* Fixes DAG loading when passing the `--lazy` argument in pipelines with a `File` client (#105)
 * Display warning if source code contains file over 10MB (#81)
 * Drop support for Python 3.6
 
 0.8 (2022-06-09)
 ----------------
 * Dropping support for Python 3.6
 * Adds ``task_resources`` to AWS Batch
@@ -284,7 +277,9 @@
 * Conda environments are cached by default
 * Ability to customize arguments to ``ploomber build``
 
 0.1 (2020-08-09)
 -----------------
 
 * First release
+
+
```

### Comparing `soopervisor-0.9.2/src/soopervisor.egg-info/SOURCES.txt` & `soopervisor-0.9b1/src/soopervisor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 src/soopervisor.egg-info/top_level.txt
 src/soopervisor/airflow/__init__.py
 src/soopervisor/airflow/config.py
 src/soopervisor/airflow/export.py
 src/soopervisor/argo/__init__.py
 src/soopervisor/argo/config.py
 src/soopervisor/argo/export.py
+src/soopervisor/assets/.DS_Store
 src/soopervisor/assets/__init__.py
 src/soopervisor/assets/airflow/bash.py
 src/soopervisor/assets/airflow/docker.py
 src/soopervisor/assets/airflow/kubernetes.py
 src/soopervisor/assets/argo/__init__.py
 src/soopervisor/assets/argo/template.yaml
+src/soopervisor/assets/aws-batch/Dockerfile
 src/soopervisor/assets/aws-lambda/Dockerfile
 src/soopervisor/assets/aws-lambda/README.md
 src/soopervisor/assets/aws-lambda/app.py
 src/soopervisor/assets/aws-lambda/template.yaml
 src/soopervisor/assets/aws-lambda/test_aws_lambda.py
 src/soopervisor/assets/docker/Dockerfile
 src/soopervisor/assets/kubeflow/Dockerfile
```

