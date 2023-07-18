# Comparing `tmp/sfdc-test-1.0.10.tar.gz` & `tmp/sfdc-test-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfdc-test-1.0.10.tar", last modified: Tue Jul 18 10:46:29 2023, max compression
+gzip compressed data, was "sfdc-test-1.0.9.tar", last modified: Tue Jul 18 10:12:51 2023, max compression
```

## Comparing `sfdc-test-1.0.10.tar` & `sfdc-test-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nlemouton   (503) staff       (20)        0 2023-07-18 10:46:29.493073 sfdc-test-1.0.10/
--rw-r--r--   0 nlemouton   (503) staff       (20)      253 2023-07-18 10:46:29.493210 sfdc-test-1.0.10/PKG-INFO
--rw-r--r--   0 nlemouton   (503) staff       (20)       12 2023-07-18 05:22:34.000000 sfdc-test-1.0.10/README.md
--rw-r--r--   0 nlemouton   (503) staff       (20)       38 2023-07-18 10:46:29.493733 sfdc-test-1.0.10/setup.cfg
--rw-r--r--   0 nlemouton   (503) staff       (20)      392 2023-07-18 10:46:04.000000 sfdc-test-1.0.10/setup.py
-drwxr-xr-x   0 nlemouton   (503) staff       (20)        0 2023-07-18 10:46:29.490561 sfdc-test-1.0.10/sfdc_test.egg-info/
--rw-r--r--   0 nlemouton   (503) staff       (20)      253 2023-07-18 10:46:29.000000 sfdc-test-1.0.10/sfdc_test.egg-info/PKG-INFO
--rw-r--r--   0 nlemouton   (503) staff       (20)      232 2023-07-18 10:46:29.000000 sfdc-test-1.0.10/sfdc_test.egg-info/SOURCES.txt
--rw-r--r--   0 nlemouton   (503) staff       (20)        1 2023-07-18 10:46:29.000000 sfdc-test-1.0.10/sfdc_test.egg-info/dependency_links.txt
--rw-r--r--   0 nlemouton   (503) staff       (20)       11 2023-07-18 10:46:29.000000 sfdc-test-1.0.10/sfdc_test.egg-info/top_level.txt
-drwxr-xr-x   0 nlemouton   (503) staff       (20)        0 2023-07-18 10:46:29.491159 sfdc-test-1.0.10/test_utils/
--rw-r--r--   0 nlemouton   (503) staff       (20)        0 2023-07-18 05:22:34.000000 sfdc-test-1.0.10/test_utils/__init__.py
-drwxr-xr-x   0 nlemouton   (503) staff       (20)        0 2023-07-18 10:46:29.492566 sfdc-test-1.0.10/test_utils/api/
--rw-r--r--   0 nlemouton   (503) staff       (20)       30 2023-07-18 05:22:34.000000 sfdc-test-1.0.10/test_utils/api/__init__.py
--rw-r--r--   0 nlemouton   (503) staff       (20)       61 2023-07-18 05:22:34.000000 sfdc-test-1.0.10/test_utils/api/api.py
+drwxr-xr-x   0 nlemouton   (503) staff       (20)        0 2023-07-18 10:12:51.276051 sfdc-test-1.0.9/
+-rw-r--r--   0 nlemouton   (503) staff       (20)      252 2023-07-18 10:12:51.276181 sfdc-test-1.0.9/PKG-INFO
+-rw-r--r--   0 nlemouton   (503) staff       (20)       12 2023-07-18 05:22:34.000000 sfdc-test-1.0.9/README.md
+-rw-r--r--   0 nlemouton   (503) staff       (20)       38 2023-07-18 10:12:51.276771 sfdc-test-1.0.9/setup.cfg
+-rw-r--r--   0 nlemouton   (503) staff       (20)      391 2023-07-18 10:12:44.000000 sfdc-test-1.0.9/setup.py
+drwxr-xr-x   0 nlemouton   (503) staff       (20)        0 2023-07-18 10:12:51.274010 sfdc-test-1.0.9/sfdc_test.egg-info/
+-rw-r--r--   0 nlemouton   (503) staff       (20)      252 2023-07-18 10:12:51.000000 sfdc-test-1.0.9/sfdc_test.egg-info/PKG-INFO
+-rw-r--r--   0 nlemouton   (503) staff       (20)      232 2023-07-18 10:12:51.000000 sfdc-test-1.0.9/sfdc_test.egg-info/SOURCES.txt
+-rw-r--r--   0 nlemouton   (503) staff       (20)        1 2023-07-18 10:12:51.000000 sfdc-test-1.0.9/sfdc_test.egg-info/dependency_links.txt
+-rw-r--r--   0 nlemouton   (503) staff       (20)       11 2023-07-18 10:12:51.000000 sfdc-test-1.0.9/sfdc_test.egg-info/top_level.txt
+drwxr-xr-x   0 nlemouton   (503) staff       (20)        0 2023-07-18 10:12:51.274596 sfdc-test-1.0.9/test_utils/
+-rw-r--r--   0 nlemouton   (503) staff       (20)        0 2023-07-18 05:22:34.000000 sfdc-test-1.0.9/test_utils/__init__.py
+drwxr-xr-x   0 nlemouton   (503) staff       (20)        0 2023-07-18 10:12:51.275611 sfdc-test-1.0.9/test_utils/api/
+-rw-r--r--   0 nlemouton   (503) staff       (20)       30 2023-07-18 05:22:34.000000 sfdc-test-1.0.9/test_utils/api/__init__.py
+-rw-r--r--   0 nlemouton   (503) staff       (20)       61 2023-07-18 05:22:34.000000 sfdc-test-1.0.9/test_utils/api/api.py
```

