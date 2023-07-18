# Comparing `tmp/promptquality-0.0.0.tar.gz` & `tmp/promptquality-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptquality-0.0.0.tar", last modified: Fri Apr 14 20:51:58 2023, max compression
+gzip compressed data, was "promptquality-0.1.0.tar", max compression
```

## Comparing `promptquality-0.0.0.tar` & `promptquality-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,22 @@
--rw-r--r--   0        0        0     1799 2023-04-14 20:45:36.908864 promptquality-0.0.0/.gitignore
--rw-r--r--   0        0        0       46 2023-04-14 20:45:36.909163 promptquality-0.0.0/README.md
--rw-r--r--   0        0        0       43 2023-04-14 20:51:38.810657 promptquality-0.0.0/promptquality/__init__.py
--rw-r--r--   0        0        0      958 2023-04-14 20:47:34.625510 promptquality-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 promptquality-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2023-07-18 03:09:10.876506 promptquality-0.1.0/LICENSE
+-rw-r--r--   0        0        0      157 2023-07-18 03:09:10.876506 promptquality-0.1.0/README.md
+-rw-r--r--   0        0        0     1463 2023-07-18 03:09:10.876506 promptquality-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      238 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/constants/__init__.py
+-rw-r--r--   0        0        0      342 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/constants/config.py
+-rw-r--r--   0        0        0      566 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/constants/routes.py
+-rw-r--r--   0        0        0      241 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/constants/run.py
+-rw-r--r--   0        0        0      833 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/get_metrics.py
+-rw-r--r--   0        0        0     4427 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/helpers.py
+-rw-r--r--   0        0        0     1059 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/job_progress.py
+-rw-r--r--   0        0        0      480 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/login.py
+-rw-r--r--   0        0        0     1273 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/run.py
+-rw-r--r--   0        0        0        0 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/types/__init__.py
+-rw-r--r--   0        0        0     7671 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/types/config.py
+-rw-r--r--   0        0        0     2997 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/types/run.py
+-rw-r--r--   0        0        0        0 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/utils/__init__.py
+-rw-r--r--   0        0        0     4043 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/utils/api_client.py
+-rw-r--r--   0        0        0       60 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/utils/logger.py
+-rw-r--r--   0        0        0    24261 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/utils/name.py
+-rw-r--r--   0        0        0     1625 2023-07-18 03:09:10.876506 promptquality-0.1.0/src/promptquality/utils/request.py
+-rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 promptquality-0.1.0/PKG-INFO
```

