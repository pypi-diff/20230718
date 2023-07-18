# Comparing `tmp/pyxnat-1.5.tar.gz` & `tmp/pyxnat-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyxnat-1.5.tar", last modified: Mon Sep 19 14:25:55 2022, max compression
+gzip compressed data, was "pyxnat-1.6.tar", last modified: Tue Jul 18 06:32:10 2023, max compression
```

## Comparing `pyxnat-1.5.tar` & `pyxnat-1.6.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2022-09-19 14:25:55.000000 pyxnat-1.5/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1631 2022-09-19 13:58:21.000000 pyxnat-1.5/LICENSE
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5064 2022-09-19 14:25:55.000000 pyxnat-1.5/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4268 2022-09-19 13:58:21.000000 pyxnat-1.5/README.rst
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2022-09-19 14:25:55.000000 pyxnat-1.5/bin/
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)    24501 2022-09-19 13:58:21.000000 pyxnat-1.5/bin/sessionmirror.py
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      666 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/__init__.py
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat/core/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      148 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/__init__.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     9682 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/array.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6184 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/attributes.py
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat/core/derivatives/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1719 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/derivatives/__init__.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1022 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/derivatives/ashs.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     7751 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/downloadutils.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3431 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/errors.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21861 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/help.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      576 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/httputil.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    18504 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/interfaces.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     9953 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/jsonutil.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    10565 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/manage.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      745 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/pathutil.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14510 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/pipelines.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     9708 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/provenance.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    87349 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/resources.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5191 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/schema.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26029 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/search.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    11517 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/select.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3509 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/tags.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4113 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/uriutil.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2424 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/users.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2018 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/xpass.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4876 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/core/xpath_store.py
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat/tests/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      671 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/__init__.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2677 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/array_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3545 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/attributes_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1118 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/custom_variables_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      508 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/downloadutils_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      467 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/experiments_tests.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      532 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/graphdata_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      308 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/inspector_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1849 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/interfaces_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1384 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/jsonutil_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      788 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/manage_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      119 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/pathutil_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1785 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/pipelines_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      548 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/prearchive_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      228 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/project_manager_tests.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1098 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/provenance_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4627 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/repr_tests.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    11398 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/resources_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      503 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/scans_tests.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2911 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/search_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3199 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/select_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1680 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/sessionmirror_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      360 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/test_resource_functions.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1731 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/uriutil_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5679 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/user_and_project_management_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1425 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/xpass_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      982 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/tests/xpath_test.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       16 2022-09-19 13:58:21.000000 pyxnat-1.5/pyxnat/version.py
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat.egg-info/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5064 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat.egg-info/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1683 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat.egg-info/SOURCES.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat.egg-info/dependency_links.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       61 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat.egg-info/requires.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        7 2022-09-19 14:25:55.000000 pyxnat-1.5/pyxnat.egg-info/top_level.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      126 2022-09-19 14:25:55.000000 pyxnat-1.5/setup.cfg
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2253 2022-09-19 13:58:21.000000 pyxnat-1.5/setup.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 06:32:10.714742 pyxnat-1.6/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6065 2023-07-18 06:32:10.714742 pyxnat-1.6/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4302 2023-06-07 10:48:44.000000 pyxnat-1.6/README.rst
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 06:32:10.704743 pyxnat-1.6/bin/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)    24499 2023-07-18 06:30:45.000000 pyxnat-1.6/bin/sessionmirror.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 06:32:10.704743 pyxnat-1.6/pyxnat/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      666 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/__init__.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 06:32:10.714742 pyxnat-1.6/pyxnat/core/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      148 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     9682 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/array.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6184 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/attributes.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 06:32:10.714742 pyxnat-1.6/pyxnat/core/derivatives/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1719 2023-06-07 10:48:41.000000 pyxnat-1.6/pyxnat/core/derivatives/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1022 2023-06-07 10:48:41.000000 pyxnat-1.6/pyxnat/core/derivatives/ashs.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     7751 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/downloadutils.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3431 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/errors.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21861 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/help.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      576 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/httputil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    18504 2023-06-07 10:48:41.000000 pyxnat-1.6/pyxnat/core/interfaces.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     9953 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/jsonutil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    10565 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/manage.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      745 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/pathutil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14510 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/pipelines.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     9708 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/provenance.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    87421 2023-07-18 06:30:45.000000 pyxnat-1.6/pyxnat/core/resources.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5191 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/schema.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26029 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/search.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    11517 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/select.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3509 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/tags.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4113 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/uriutil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2424 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/users.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2018 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/xpass.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4876 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/core/xpath_store.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 06:32:10.714742 pyxnat-1.6/pyxnat/tests/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      583 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2699 2023-07-18 06:30:45.000000 pyxnat-1.6/pyxnat/tests/array_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3556 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/attributes_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1129 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/custom_variables_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      519 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/downloadutils_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      478 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/experiments_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      543 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/graphdata_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      308 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/tests/inspector_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1860 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/interfaces_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1384 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/tests/jsonutil_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      799 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/manage_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      119 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/tests/pathutil_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1785 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/tests/pipelines_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      559 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/prearchive_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      228 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/project_manager_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1109 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/provenance_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     4638 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/repr_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    11394 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/resources_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      514 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/scans_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2911 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/tests/search_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3199 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/tests/select_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1691 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/sessionmirror_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      360 2023-06-07 10:48:41.000000 pyxnat-1.6/pyxnat/tests/test_resource_functions.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1731 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/tests/uriutil_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5564 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/user_and_project_management_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1425 2022-11-10 14:41:27.000000 pyxnat-1.6/pyxnat/tests/xpass_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      993 2023-06-07 10:48:44.000000 pyxnat-1.6/pyxnat/tests/xpath_test.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       16 2023-07-18 06:30:45.000000 pyxnat-1.6/pyxnat/version.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-18 06:32:10.704743 pyxnat-1.6/pyxnat.egg-info/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6065 2023-07-18 06:32:10.000000 pyxnat-1.6/pyxnat.egg-info/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1671 2023-07-18 06:32:10.000000 pyxnat-1.6/pyxnat.egg-info/SOURCES.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2023-07-18 06:32:10.000000 pyxnat-1.6/pyxnat.egg-info/dependency_links.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       61 2023-07-18 06:32:10.000000 pyxnat-1.6/pyxnat.egg-info/requires.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        7 2023-07-18 06:32:10.000000 pyxnat-1.6/pyxnat.egg-info/top_level.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      276 2023-07-18 06:32:10.714742 pyxnat-1.6/setup.cfg
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2253 2023-07-18 06:30:45.000000 pyxnat-1.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyxnat-1.5/README.rst` & `pyxnat-1.6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 using ``pip`` with the following command::
 
     pip install pyxnat
 
 Dependencies
 ============
 
-- `requests <https://2.python-requests.org/en/master/>`_ v2.20 or higher
+- `requests <https://requests.readthedocs.io/>`_ v2.20 or higher
 - `python-lxml <https://lxml.de/>`_ v4.3.2 or higher recommended, earlier versions may work.
 
 For development purposes:
 
-- *python-nose* v1.2.1 or higher
-- *coverage* v3.6 or higher
+- `pytest <https://pytest.org/>`_ v7.1 or higher
+- `coverage <https://coverage.readthedocs.io/>`_ v3.6 or higher
 
 See the `full installation instructions <https://pyxnat.github.io/pyxnat/installing.html>`_
 for recommended and optional dependencies.
 
 Installation from sources
 =========================
 
@@ -64,15 +64,15 @@
 In v1.1, tests were restructured and were directed to two independent XNAT
 instances based on permission level. Hence `XNAT Central <http://central.xnat.org>`_
 is still used for most tests with read access whereas other tests requiring
 write permissions are run on a local XNAT instance in a Docker container.
 
 Consequently, running the test suite now requires the following:
 
-  - *python-nose* v1.2.1+
+  - *pytest* v7.1+
   - *coverage* v3.6+
   - *docker* v18+
 
 Setting up a local Docker-powered XNAT instance may be achieved easily using
 ``docker-compose`` and any available recipe. We recommend the one from the
 `following repository <https://github.com/NrgXnat/xnat-docker-compose>`_
 (maintained by the XNAT team). Once the repository cloned, run the following
@@ -84,15 +84,15 @@
 You may check it out visiting http://localhost.
 
 The script ``tests/setup_xnat.py`` may then be executed to populate the local
 instance before running the tests.
 
 Finally run the tests with the following command (from the root of the project)::
 
-    nosetests pyxnat/tests
+    pytest --cov pyxnat
 
 The file ``.github/workflows/ci.yml`` (used for CI) features these described
 steps and may be referred to for further information.
 
 
 Building the documentation
 ==========================
```

### Comparing `pyxnat-1.5/bin/sessionmirror.py` & `pyxnat-1.6/bin/sessionmirror.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,19 +467,19 @@
         # dst_assr = dst_sess.assessor(assr_label)
         # assr_cache_dir = op.join(sess_cache_dir, assr_label)
         # copy_assr(src_assr, dst_assr, assr_cache_dir)
 
     for src_res in src_sess.resources().fetchall('obj'):
         res_label = src_res.label()
 
-        print('INFO:Processing resource:%s...' % (res_label))
+        print('INFO:Processing resource:%s...' % res_label)
 
         dst_res = dst_sess.resource(res_label)
 
-        res_cache_dir = op.join(scan_cache_dir, res_label)
+        res_cache_dir = op.join(sess_cache_dir, res_label)
 
         copy_res(src_res, dst_res, res_cache_dir, use_zip=True)
 
 
 def copy_scan(src_scan, dst_scan, scan_cache_dir):
     '''Copy scan from source XNAT to destination XNAT'''
```

### Comparing `pyxnat-1.5/pyxnat/__init__.py` & `pyxnat-1.6/pyxnat/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/array.py` & `pyxnat-1.6/pyxnat/core/array.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/attributes.py` & `pyxnat-1.6/pyxnat/core/attributes.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/derivatives/__init__.py` & `pyxnat-1.6/pyxnat/core/derivatives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/derivatives/ashs.py` & `pyxnat-1.6/pyxnat/core/derivatives/ashs.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/downloadutils.py` & `pyxnat-1.6/pyxnat/core/downloadutils.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/errors.py` & `pyxnat-1.6/pyxnat/core/errors.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/help.py` & `pyxnat-1.6/pyxnat/core/help.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/httputil.py` & `pyxnat-1.6/pyxnat/core/httputil.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/interfaces.py` & `pyxnat-1.6/pyxnat/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/jsonutil.py` & `pyxnat-1.6/pyxnat/core/jsonutil.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/manage.py` & `pyxnat-1.6/pyxnat/core/manage.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/pathutil.py` & `pyxnat-1.6/pyxnat/core/pathutil.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/pipelines.py` & `pyxnat-1.6/pyxnat/core/pipelines.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/provenance.py` & `pyxnat-1.6/pyxnat/core/provenance.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/resources.py` & `pyxnat-1.6/pyxnat/core/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1842,15 +1842,17 @@
         # Check if resource exists
         if self.exists():
             resource_id = self.id()
             base_url = uri_parent(self._uri)
             resources = self._intf._get_json(base_url)
             res_info = [r for r in resources
                         if r['xnat_abstractresource_id'] == resource_id][0]
-            fs = sizeof_fmt(float(res_info['file_size']))
+            fs = '0.0 B'
+            if res_info['file_size'] != '':
+                fs = sizeof_fmt(float(res_info['file_size']))
 
             # Creating the output string
             output = '<{cl} Object> {id} `{label}` ({fc} files {fs})'
             output = output.format(label=self.label(),
                                    cl=self.__class__.__name__,
                                    id=resource_id,
                                    fc=res_info['file_count'],
@@ -2075,28 +2077,27 @@
 
     def datatype(self):
         return (super(Resource, self).datatype()
                 or 'xnat:abstractResource'
                 )
 
     def attributes(self):
-        """ Files attributes include:
-                - URI
-                - Name
-                - Size in bytes
-                - path (relative to the parent resource)
+        """ Resource attributes include:
+                - label
+                - file_count
+                - file_size in bytes
                 - tags
                 - format
                 - content
             Returns
             -------
             dict : a dictionary with the resource attributes
         """
 
-        return self._getcells(['URI', 'Name', 'Size', 'path',
+        return self._getcells(['label', 'file_count', 'file_size',
                                'tags', 'format', 'content'])
 
 
 class In_Resource(Resource):
 
     def parent(self):
         uri = uri_grandparent(self._uri)
@@ -2140,21 +2141,22 @@
                 - URI
                 - Name
                 - Size in bytes
                 - path (relative to the parent resource)
                 - file_tags
                 - file_format
                 - file_content
+                - digest
 
             Returns
             -------
             dict : a dictionary with the file attributes
         """
 
-        return self._getcells(['URI', 'Name', 'Size', 'path',
+        return self._getcells(['URI', 'Name', 'Size', 'path', 'digest',
                                'file_tags', 'file_format', 'file_content'])
 
     def get(self, dest=None):
         """ Downloads the file.
 
             Parameters
             ----------
```

### Comparing `pyxnat-1.5/pyxnat/core/schema.py` & `pyxnat-1.6/pyxnat/core/schema.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/search.py` & `pyxnat-1.6/pyxnat/core/search.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/select.py` & `pyxnat-1.6/pyxnat/core/select.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/tags.py` & `pyxnat-1.6/pyxnat/core/tags.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/uriutil.py` & `pyxnat-1.6/pyxnat/core/uriutil.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/users.py` & `pyxnat-1.6/pyxnat/core/users.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/xpass.py` & `pyxnat-1.6/pyxnat/core/xpass.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/core/xpath_store.py` & `pyxnat-1.6/pyxnat/core/xpath_store.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/tests/__init__.py` & `pyxnat-1.6/pyxnat/tests/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from functools import wraps
-from nose import SkipTest
-from nose.plugins.attrib import attr
+import pytest
 import os
 
 
 def skip_if_no_network(func=None):
     """Skip test completely in NONETWORK settings
     If not used as a decorator, and just a function, could be used at the module level
     """
 
     def check_and_raise():
         if os.environ.get('PYXNAT_SKIP_NETWORK_TESTS'):
-            raise SkipTest("Skipping since no network settings")
+            pytest.skip("Skipping since no network settings")
 
     if func:
         @wraps(func)
-        @attr('skip_if_no_network')
         def newfunc(*args, **kwargs):
             check_and_raise()
             return func(*args, **kwargs)
         return newfunc
     else:
         check_and_raise()
```

### Comparing `pyxnat-1.5/pyxnat/tests/array_test.py` & `pyxnat-1.6/pyxnat/tests/array_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import os.path as op
 from pyxnat import Interface
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 import logging as log
 log.basicConfig(level=log.INFO)
 
 
 class ArrayTests(unittest.TestCase):
     ''' Resource-related XNAT connectivity test cases '''
 
@@ -16,49 +16,49 @@
     @skip_if_no_network
     def test_array_experiments(self):
         '''
         Get a list of experiments from a given subject which has multiple types
         of experiments (i.e. MRSessions and PETSessions) and assert it gathers
         them all.
         '''
-        e = self._intf.array.experiments(subject_id='CENTRAL_S06242').data
+        e = self._intf.array.experiments(subject_id='CENTRAL02_S01346').data
         self.assertGreaterEqual(len(e), 3)
 
     @skip_if_no_network
     def test_array_mrsessions(self):
         '''
         From a given subject which has multiple types of experiments, get a
         list of MRI sessions and assert its length matches the list of
         experiments of type 'xnat:mrSessionData'
         '''
-        mris = self._intf.array.mrsessions(subject_id='CENTRAL_S06242').data
-        e = self._intf.array.experiments(subject_id='CENTRAL_S06242',
+        mris = self._intf.array.mrsessions(subject_id='CENTRAL02_S01346').data
+        e = self._intf.array.experiments(subject_id='CENTRAL02_S01346',
                                          experiment_type='xnat:mrSessionData')
         exps = e.data
         self.assertListEqual(mris, exps)
 
     @skip_if_no_network
     def test_array_scans(self):
         '''
         Get a list of scans from a given experiment which has multiple types
         of scans (i.e. PETScans and CTScans) and assert it gathers them all.
         '''
-        s = self._intf.array.scans(experiment_id='CENTRAL_E72012').data
-        self.assertEqual(len(s), 16)
+        s = self._intf.array.scans(experiment_id='CENTRAL03_E05157').data
+        self.assertEqual(len(s), 4)
 
     @skip_if_no_network
     def test_array_mrscans(self):
         '''
         Get a list of MRI scans from a given experiment which has multiple
         scans mixed (i.e. MRScans and MRSpectroscopies, aka OtherDicomScans)
         and assert its length matches the list of scans filtered by type
         'xnat:mrScanData'
         '''
-        mris = self._intf.array.mrscans(experiment_id='CENTRAL_E72012').data
-        exps = self._intf.array.scans(experiment_id='CENTRAL_E72012',
+        mris = self._intf.array.mrscans(experiment_id='CENTRAL02_E01892').data
+        exps = self._intf.array.scans(experiment_id='CENTRAL02_E01892',
                                       scan_type='xnat:mrScanData').data
         self.assertListEqual([i['xnat:mrscandata/id'] for i in mris],
                              [i['xnat:mrscandata/id'] for i in exps])
 
     @skip_if_no_network
     def test_search_experiments(self):
         et = 'xnat:subjectData'
```

### Comparing `pyxnat-1.5/pyxnat/tests/attributes_test.py` & `pyxnat-1.6/pyxnat/tests/attributes_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os.path as op
 from uuid import uuid1
 import time
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 from pyxnat import Interface
 from pyxnat.core import interfaces
 
 
 _modulepath = op.dirname(op.abspath(__file__))
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
```

### Comparing `pyxnat-1.5/pyxnat/tests/custom_variables_test.py` & `pyxnat-1.6/pyxnat/tests/custom_variables_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from uuid import uuid1
 from pyxnat import Interface
 import os.path as op
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 central = Interface(config=fp)
 project = central.select.project('nosetests5')
 
 variables = {'Subjects': {'newgroup': {'foo': 'string', 'bar': 'int'}}}
```

### Comparing `pyxnat-1.5/pyxnat/tests/graphdata_test.py` & `pyxnat-1.6/pyxnat/tests/graphdata_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyxnat.core.help import GraphData, PaintGraph, SchemasInspector
 from pyxnat import Interface
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 import os.path as op
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 central = Interface(config=fp)
 
 
 @skip_if_no_network
```

### Comparing `pyxnat-1.5/pyxnat/tests/interfaces_test.py` & `pyxnat-1.6/pyxnat/tests/interfaces_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os.path as op
 from pyxnat import Interface
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 central = Interface(config=fp)
 central_anon = Interface('https://central.xnat.org', anonymous=True)
 
 
 def test_simple_object_listing():
```

### Comparing `pyxnat-1.5/pyxnat/tests/jsonutil_test.py` & `pyxnat-1.6/pyxnat/tests/jsonutil_test.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/tests/manage_test.py` & `pyxnat-1.6/pyxnat/tests/manage_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os.path as op
 from pyxnat import Interface
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 central = Interface(config=fp)
 
 notified = []
```

### Comparing `pyxnat-1.5/pyxnat/tests/pipelines_test.py` & `pyxnat-1.6/pyxnat/tests/pipelines_test.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/tests/prearchive_test.py` & `pyxnat-1.6/pyxnat/tests/prearchive_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyxnat import Interface
 import os.path as op
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 central = Interface(config=fp)
 
 
 @skip_if_no_network
 def test_prearchive_get():
```

### Comparing `pyxnat-1.5/pyxnat/tests/provenance_test.py` & `pyxnat-1.6/pyxnat/tests/provenance_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from uuid import uuid1
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 from pyxnat import Interface
 import os.path as op
 
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 central = Interface(config=fp)
 project = central.select.project('nosetests5')
```

### Comparing `pyxnat-1.5/pyxnat/tests/repr_tests.py` & `pyxnat-1.6/pyxnat/tests/repr_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyxnat import Interface
 import os.path as op
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 
 _modulepath = op.dirname(op.abspath(__file__))
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 print(fp)
 central = Interface(config=fp)
```

### Comparing `pyxnat-1.5/pyxnat/tests/resources_test.py` & `pyxnat-1.6/pyxnat/tests/resources_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tempfile
 from uuid import uuid1
 from six import string_types
 import os.path as op
 import os
 from pyxnat import Interface
-from . import skip_if_no_network
-from nose import SkipTest
+from pyxnat.tests import skip_if_no_network
+import pytest
 from pyxnat.core import interfaces
 
 _modulepath = op.dirname(op.abspath(__file__))
 
 central = Interface(config=op.join(op.dirname(op.abspath(__file__)),
                                    'central.cfg'))
 interfaces.STUBBORN = True
@@ -240,15 +240,15 @@
     try:
         assert project.quarantine_code() == 0
         assert project.prearchive_code() == 4, project.prearchive_code()
     except DatabaseError:
         if version['version'] == '1.7.5.2-SNAPSHOT':
             msg = 'Version 1.7.5.2-SNAPSHOT gives trouble on some machines. \
                    Skipping it'
-            raise SkipTest(msg)
+            pytest.skip(msg)
 
     if version['version'] != '1.7.5.2-SNAPSHOT':
         try:
             assert project.current_arc() == b'arc001'
         except DatabaseError:
             msg = 'Check if current_arc is supported in XNAT version %s.' \
                   % version['version']
```

### Comparing `pyxnat-1.5/pyxnat/tests/search_test.py` & `pyxnat-1.6/pyxnat/tests/search_test.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/tests/select_test.py` & `pyxnat-1.6/pyxnat/tests/select_test.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/tests/sessionmirror_test.py` & `pyxnat-1.6/pyxnat/tests/sessionmirror_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import os.path as op
 import pyxnat
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 
 _modulepath = op.dirname(op.abspath(pyxnat.__file__))
 dd = op.join(op.split(_modulepath)[0], 'bin')
 sys.path.append(dd)
 
 cfg = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 central = pyxnat.Interface(config=cfg)
```

### Comparing `pyxnat-1.5/pyxnat/tests/uriutil_test.py` & `pyxnat-1.6/pyxnat/tests/uriutil_test.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/tests/user_and_project_management_test.py` & `pyxnat-1.6/pyxnat/tests/user_and_project_management_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from pyxnat import Interface
 from requests.exceptions import ConnectionError
 import os.path as op
-from nose import SkipTest
 from functools import wraps
-from nose.plugins.attrib import attr
+import pytest
 
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 
 
 def docker_available(func=None):
-    '''Skip test completely if no Docker-based XNAT instance available
-    '''
+    """Skip test completely if no Docker-based XNAT instance available
+    """
 
     def check_and_raise():
         if 'setup_docker_xnat' in func.__name__:
             print('Initializing XNAT.')
             return
         fp = op.abspath('.xnat.cfg')
         print(fp, op.isfile(fp))
@@ -24,20 +23,18 @@
 
         try:
             x.head('')
             list(x.select.projects())
             print('Docker instance found.')
         except (ConnectionError, KeyError):
             print('Skipping it.')
-            raise SkipTest('Docker-based XNAT instance unavailable')
+            pytest.skip('Docker-based XNAT instance unavailable')
 
     if func:
         @wraps(func)
-        @attr('network')
-        @attr('docker_available')
         def newfunc(*args, **kwargs):
             check_and_raise()
             return func(*args, **kwargs)
         return newfunc
     else:
         check_and_raise()
 
@@ -73,28 +70,27 @@
         print(cmd2)
         os.system(cmd2)
 
         cmd2 = cmd % '{"initialized":true}'
         print(cmd2)
         os.system(cmd2)
 
-
         p = x.select.project('nosetests')
         p.create()
         for i in range(3, 10):
             p = x.select.project('nosetests%s' % i)
             p.create()
 
         uri = '/data/projects/nosetests'
         options = {'alias': 'nosetests2'}
         data = x.put(uri, params=options).text
 
     except Exception:
         print('Skipping initialization.')
-        raise SkipTest('Docker-based XNAT initialization failed.')
+        pytest.skip('Docker-based XNAT initialization failed.')
 
 
 @docker_available
 def test_users():
     x = Interface(config='.xnat.cfg')
     assert isinstance(x.manage.users(), list)
```

### Comparing `pyxnat-1.5/pyxnat/tests/xpass_test.py` & `pyxnat-1.6/pyxnat/tests/xpass_test.py`

 * *Files identical despite different names*

### Comparing `pyxnat-1.5/pyxnat/tests/xpath_test.py` & `pyxnat-1.6/pyxnat/tests/xpath_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os.path as op
 from pyxnat import Interface
-from . import skip_if_no_network
+from pyxnat.tests import skip_if_no_network
 
 fp = op.join(op.dirname(op.abspath(__file__)), 'central.cfg')
 central = Interface(config=fp)
 
 
 @skip_if_no_network
 def test_001_xpath_checkout():
```

### Comparing `pyxnat-1.5/pyxnat.egg-info/SOURCES.txt` & `pyxnat-1.6/pyxnat.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.rst
 setup.cfg
 setup.py
 bin/sessionmirror.py
 pyxnat/__init__.py
 pyxnat/version.py
 pyxnat.egg-info/PKG-INFO
@@ -35,28 +34,28 @@
 pyxnat/core/derivatives/__init__.py
 pyxnat/core/derivatives/ashs.py
 pyxnat/tests/__init__.py
 pyxnat/tests/array_test.py
 pyxnat/tests/attributes_test.py
 pyxnat/tests/custom_variables_test.py
 pyxnat/tests/downloadutils_test.py
-pyxnat/tests/experiments_tests.py
+pyxnat/tests/experiments_test.py
 pyxnat/tests/graphdata_test.py
 pyxnat/tests/inspector_test.py
 pyxnat/tests/interfaces_test.py
 pyxnat/tests/jsonutil_test.py
 pyxnat/tests/manage_test.py
 pyxnat/tests/pathutil_test.py
 pyxnat/tests/pipelines_test.py
 pyxnat/tests/prearchive_test.py
-pyxnat/tests/project_manager_tests.py
+pyxnat/tests/project_manager_test.py
 pyxnat/tests/provenance_test.py
-pyxnat/tests/repr_tests.py
+pyxnat/tests/repr_test.py
 pyxnat/tests/resources_test.py
-pyxnat/tests/scans_tests.py
+pyxnat/tests/scans_test.py
 pyxnat/tests/search_test.py
 pyxnat/tests/select_test.py
 pyxnat/tests/sessionmirror_test.py
 pyxnat/tests/test_resource_functions.py
 pyxnat/tests/uriutil_test.py
 pyxnat/tests/user_and_project_management_test.py
 pyxnat/tests/xpass_test.py
```

### Comparing `pyxnat-1.5/setup.py` & `pyxnat-1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,16 @@
                       'Intended Audience :: Science/Research',
                       'Intended Audience :: Education',
                       'License :: OSI Approved :: BSD License',
                       'Operating System :: OS Independent',
                       'Topic :: Scientific/Engineering',
                       'Topic :: Utilities',
                       'Topic :: Internet :: WWW/HTTP',
-                      'Programming Language :: Python :: 3.7',
                       'Programming Language :: Python :: 3.8',
+                      'Programming Language :: Python :: 3.9',
                  ],
 
                  platforms='any',
                  scripts=['bin/sessionmirror.py'],
                  install_requires=['lxml>=4.3',
                                    'requests>=2.20',
                                    'pathlib>=1.0',
```

