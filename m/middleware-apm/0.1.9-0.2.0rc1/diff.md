# Comparing `tmp/middleware-apm-0.1.9.tar.gz` & `tmp/middleware-apm-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-apm-0.1.9.tar", last modified: Sat Oct 29 04:32:40 2022, max compression
+gzip compressed data, was "middleware-apm-0.2.0rc1.tar", last modified: Tue Jul 18 10:13:43 2023, max compression
```

## Comparing `middleware-apm-0.1.9.tar` & `middleware-apm-0.2.0rc1.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/apmpythonpackage/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/apmpythonpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/apmpythonpackage/apmpythonpackage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/middleware_apm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-29 04:32:40.000000 middleware-apm-0.1.9/middleware_apm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-29 04:32:40.000000 middleware-apm-0.1.9/middleware_apm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 04:32:40.000000 middleware-apm-0.1.9/middleware_apm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-29 04:32:40.000000 middleware-apm-0.1.9/middleware_apm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-29 04:32:40.938949 middleware-apm-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-29 04:32:33.000000 middleware-apm-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:13:43.174430 middleware-apm-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 10:13:14.000000 middleware-apm-0.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-18 10:13:43.174430 middleware-apm-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 10:13:14.000000 middleware-apm-0.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:13:43.174430 middleware-apm-0.2.0rc1/middleware_apm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-18 10:13:43.000000 middleware-apm-0.2.0rc1/middleware_apm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-18 10:13:43.000000 middleware-apm-0.2.0rc1/middleware_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:13:43.000000 middleware-apm-0.2.0rc1/middleware_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 10:13:43.000000 middleware-apm-0.2.0rc1/middleware_apm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-18 10:13:43.000000 middleware-apm-0.2.0rc1/middleware_apm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 10:13:43.000000 middleware-apm-0.2.0rc1/middleware_apm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:13:43.174430 middleware-apm-0.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-18 10:13:14.000000 middleware-apm-0.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:13:43.174430 middleware-apm-0.2.0rc1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-18 10:13:14.000000 middleware-apm-0.2.0rc1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-18 10:13:14.000000 middleware-apm-0.2.0rc1/src/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-18 10:13:14.000000 middleware-apm-0.2.0rc1/src/_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-18 10:13:14.000000 middleware-apm-0.2.0rc1/src/_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-18 10:13:14.000000 middleware-apm-0.2.0rc1/src/mw_tracker.py
```

### Comparing `middleware-apm-0.1.9/LICENSE` & `middleware-apm-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

