# Comparing `tmp/randog-0.6.0.tar.gz` & `tmp/randog-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randog-0.6.0.tar", last modified: Mon Jul 17 07:03:47 2023, max compression
+gzip compressed data, was "randog-0.7.0.tar", last modified: Tue Jul 18 15:18:09 2023, max compression
```

## Comparing `randog-0.6.0.tar` & `randog-0.7.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.608795 randog-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 07:03:36.000000 randog-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-17 07:03:47.608795 randog-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-17 07:03:36.000000 randog-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-17 07:03:36.000000 randog-0.6.0/randog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-17 07:03:36.000000 randog-0.6.0/randog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog/_main/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_main_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog/_main/_subcmd_def/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_byfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_main/_subcmd_def/_timedelta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_utils/nullsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-17 07:03:36.000000 randog-0.6.0/randog/_utils/type.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-17 07:03:36.000000 randog-0.6.0/randog/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.608795 randog-0.6.0/randog/factory/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_by_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_by_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_float.py
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_from_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_from_pyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_increment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-17 07:03:36.000000 randog-0.6.0/randog/factory/_union.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.608795 randog-0.6.0/randog/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-17 07:03:36.000000 randog-0.6.0/randog/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-07-17 07:03:36.000000 randog-0.6.0/randog/sqlalchemy/_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-17 07:03:36.000000 randog-0.6.0/randog/sqlalchemy/_custom_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-17 07:03:36.000000 randog-0.6.0/randog/timedelta_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 07:03:47.604795 randog-0.6.0/randog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-17 07:03:47.000000 randog-0.6.0/randog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-17 07:03:47.000000 randog-0.6.0/randog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 07:03:47.000000 randog-0.6.0/randog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 07:03:47.000000 randog-0.6.0/randog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 07:03:47.608795 randog-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-17 07:03:36.000000 randog-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:18:09.731652 randog-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 15:17:57.000000 randog-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-18 15:18:09.731652 randog-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-18 15:17:57.000000 randog-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:18:09.719652 randog-0.7.0/randog/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-18 15:17:57.000000 randog-0.7.0/randog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-18 15:17:57.000000 randog-0.7.0/randog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:18:09.723652 randog-0.7.0/randog/_main/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_main_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:18:09.727652 randog-0.7.0/randog/_main/_subcmd_def/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_byfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_main/_subcmd_def/_timedelta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:18:09.727652 randog-0.7.0/randog/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_utils/nullsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-18 15:17:57.000000 randog-0.7.0/randog/_utils/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-18 15:17:57.000000 randog-0.7.0/randog/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:18:09.731652 randog-0.7.0/randog/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_by_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_by_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_from_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_from_pyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_increment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-18 15:17:57.000000 randog-0.7.0/randog/factory/_union.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:18:09.731652 randog-0.7.0/randog/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-18 15:17:57.000000 randog-0.7.0/randog/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-07-18 15:17:57.000000 randog-0.7.0/randog/sqlalchemy/_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-18 15:17:57.000000 randog-0.7.0/randog/sqlalchemy/_custom_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-18 15:17:57.000000 randog-0.7.0/randog/timedelta_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:18:09.723652 randog-0.7.0/randog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-18 15:18:09.000000 randog-0.7.0/randog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-18 15:18:09.000000 randog-0.7.0/randog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:18:09.000000 randog-0.7.0/randog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 15:18:09.000000 randog-0.7.0/randog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:18:09.731652 randog-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-18 15:17:57.000000 randog-0.7.0/setup.py
```

### Comparing `randog-0.6.0/LICENSE` & `randog-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/PKG-INFO` & `randog-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: randog
-Version: 0.6.0
+Version: 0.7.0
 Summary: Generate data randomly
 Home-page: UNKNOWN
 Author: k-izumi
 Author-email: k.izumi.ysk@gmail.com
 Maintainer: k-izumi
 Maintainer-email: k.izumi.ysk@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/unaguna/random-obj-generator/issues
 Project-URL: Documentation, https://unaguna.github.io/random-obj-generator/
 Project-URL: Source Code, https://github.com/unaguna/random-obj-generator
-Description: **randog 0.6.0 — Randomly object generator**
+Description: **randog 0.7.0 — Randomly object generator**
         
         **randog** is a package which helps to generate data randomly.
         
         ## Install
         
         You can install from PyPI.
```

### Comparing `randog-0.6.0/README.md` & `randog-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-**randog 0.6.0 — Randomly object generator**
+**randog 0.7.0 — Randomly object generator**
 
 **randog** is a package which helps to generate data randomly.
 
 ## Install
 
 You can install from PyPI.
```

### Comparing `randog-0.6.0/randog/_examples.py` & `randog-0.7.0/randog/_examples.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_main_args.py` & `randog-0.7.0/randog/_main/_main_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,21 @@
     @property
     def format(self) -> t.Optional[str]:
         if hasattr(self._args, "format"):
             return self._args.format
         else:
             return None
 
+    @property
+    def csv(self) -> t.Optional[int]:
+        if hasattr(self._args, "csv"):
+            return self._args.csv
+        else:
+            return None
+
     def output_path_for(self, number: int) -> t.Optional[str]:
         if self._args.output is None:
             return None
         else:
             return self._args.output.format(number)
 
     def get(self, key: str, default: t.Any = None) -> t.Any:
```

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/__init__.py` & `randog-0.7.0/randog/_main/_subcmd_def/__init__.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_base.py` & `randog-0.7.0/randog/_main/_subcmd_def/_base.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_bool.py` & `randog-0.7.0/randog/_main/_subcmd_def/_bool.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_date.py` & `randog-0.7.0/randog/_main/_subcmd_def/_date.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_datetime.py` & `randog-0.7.0/randog/_main/_subcmd_def/_datetime.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_decimal.py` & `randog-0.7.0/randog/_main/_subcmd_def/_decimal.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_float.py` & `randog-0.7.0/randog/_main/_subcmd_def/_float.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_int.py` & `randog-0.7.0/randog/_main/_subcmd_def/_int.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_str.py` & `randog-0.7.0/randog/_main/_subcmd_def/_str.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_time.py` & `randog-0.7.0/randog/_main/_subcmd_def/_time.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_main/_subcmd_def/_timedelta.py` & `randog-0.7.0/randog/_main/_subcmd_def/_timedelta.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/_utils/type.py` & `randog-0.7.0/randog/_utils/type.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/__init__.py` & `randog-0.7.0/randog/factory/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ._list import randlist
 from ._dict import DictItem, DictRandomFactory, randdict
 from ._by_callable import ByCallableFactory, by_callable
 from ._by_iterator import ByIteratorFactory, by_iterator
 from ._increment import increment
 from ._union import UnionRandomFactory, union
 from ._from_example import from_example, FromExampleContext
-from ._from_pyfile import from_pyfile
+from ._from_pyfile import from_pyfile, FactoryDef
 
 __all__ = [
     "from_example",
     "FromExampleContext",
     "from_pyfile",
     "Factory",
     "randchoice",
@@ -39,8 +39,9 @@
     "randlist",
     "randdict",
     "by_callable",
     "by_iterator",
     "increment",
     "union",
     "DictItem",
+    "FactoryDef",
 ]
```

### Comparing `randog-0.6.0/randog/factory/_base.py` & `randog-0.7.0/randog/factory/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         """
         pass
 
     def or_none(
         self,
         prob: float = 0.1,
         *,
+        lazy_choice: bool = False,
         rnd: t.Optional[Random] = None,
     ) -> "Factory[t.Union[T, None]]":
         """Returns a factory whose result may be None with the specified probability.
 
         Examples
         --------
         >>> import randog
@@ -35,28 +36,34 @@
         >>> generated = factory.next()
         >>> assert generated is None or isinstance(generated, str)
 
         Parameters
         ----------
         prob : float, default=0.1
             Probability that the result is None
+        lazy_choice : bool, optional
+            If it is True, when generating a value,
+            first generate value with the base factory and then decides whether to adopt it or None.
+            Otherwise, it first decides whether to return None or generate a value and return it,
+            and then generates a value only if it is returned.
         rnd : Random, optional
             random number generator to be used
 
         Returns
         -------
         Factory[T|None]
             A factory whose result may be None with the specified probability.
         """
         import randog.factory
 
         return randog.factory.union(
             self,
             randog.factory.const(None),
             weights=[1 - prob, prob],
+            lazy_choice=lazy_choice,
             rnd=rnd,
         )
 
     def post_process(self, post_process: t.Callable[[T], R]) -> "Factory[R]":
         """Returns a factory whose result will be modified by `post_process`
 
         Examples
```

### Comparing `randog-0.6.0/randog/factory/_bool.py` & `randog-0.7.0/randog/factory/_bool.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_by_callable.py` & `randog-0.7.0/randog/factory/_by_callable.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_by_iterator.py` & `randog-0.7.0/randog/factory/_by_iterator.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_choice.py` & `randog-0.7.0/randog/factory/_choice.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_date.py` & `randog-0.7.0/randog/factory/_date.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_datetime.py` & `randog-0.7.0/randog/factory/_datetime.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_decimal.py` & `randog-0.7.0/randog/factory/_decimal.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_dict.py` & `randog-0.7.0/randog/factory/_dict.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_float.py` & `randog-0.7.0/randog/factory/_float.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_from_example.py` & `randog-0.7.0/randog/factory/_from_example.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_increment.py` & `randog-0.7.0/randog/factory/_increment.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_int.py` & `randog-0.7.0/randog/factory/_int.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_list.py` & `randog-0.7.0/randog/factory/_list.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_str.py` & `randog-0.7.0/randog/factory/_str.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_time.py` & `randog-0.7.0/randog/factory/_time.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/factory/_timedelta.py` & `randog-0.7.0/randog/factory/_timedelta.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/sqlalchemy/_construct.py` & `randog-0.7.0/randog/sqlalchemy/_construct.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/sqlalchemy/_custom_func.py` & `randog-0.7.0/randog/sqlalchemy/_custom_func.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog/timedelta_util.py` & `randog-0.7.0/randog/timedelta_util.py`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/randog.egg-info/PKG-INFO` & `randog-0.7.0/randog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: randog
-Version: 0.6.0
+Version: 0.7.0
 Summary: Generate data randomly
 Home-page: UNKNOWN
 Author: k-izumi
 Author-email: k.izumi.ysk@gmail.com
 Maintainer: k-izumi
 Maintainer-email: k.izumi.ysk@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/unaguna/random-obj-generator/issues
 Project-URL: Documentation, https://unaguna.github.io/random-obj-generator/
 Project-URL: Source Code, https://github.com/unaguna/random-obj-generator
-Description: **randog 0.6.0 — Randomly object generator**
+Description: **randog 0.7.0 — Randomly object generator**
         
         **randog** is a package which helps to generate data randomly.
         
         ## Install
         
         You can install from PyPI.
```

### Comparing `randog-0.6.0/randog.egg-info/SOURCES.txt` & `randog-0.7.0/randog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `randog-0.6.0/setup.py` & `randog-0.7.0/setup.py`

 * *Files identical despite different names*

