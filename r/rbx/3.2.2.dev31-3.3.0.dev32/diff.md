# Comparing `tmp/rbx-3.2.2.dev31.tar.gz` & `tmp/rbx-3.3.0.dev32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbx-3.2.2.dev31.tar", last modified: Thu Jul  6 14:05:10 2023, max compression
+gzip compressed data, was "rbx-3.3.0.dev32.tar", last modified: Tue Jul 18 13:52:11 2023, max compression
```

## Comparing `rbx-3.2.2.dev31.tar` & `rbx-3.3.0.dev32.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.351750 rbx-3.2.2.dev31/rbx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.351750 rbx-3.2.2.dev31/rbx/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/auth/keystore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.351750 rbx-3.2.2.dev31/rbx/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/aws/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.351750 rbx-3.2.2.dev31/rbx/buildtools/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/buildtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-06 14:05:09.000000 rbx-3.2.2.dev31/rbx/buildtools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/rbx/buildtools/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/buildtools/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/buildtools/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/buildtools/tasks/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/buildtools/tasks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/buildtools/tasks/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/rbx/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/clients/adsquare.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/clients/broadsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/clients/oxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/clients/panels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/clients/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/clients/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/clients/uslicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/rbx/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/gcp/cloud_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/gcp/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/rbx/geo/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/geo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/geo/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/geo/packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/rbx/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/manifest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/manifest/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/manifest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/rbx/queues/
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/queues/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/queues/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/rbx/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/utils/mdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/rbx/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-06 14:04:55.000000 rbx-3.2.2.dev31/rbx/web/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:05:10.351750 rbx-3.2.2.dev31/rbx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-06 14:05:10.000000 rbx-3.2.2.dev31/rbx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-06 14:05:10.000000 rbx-3.2.2.dev31/rbx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:05:10.000000 rbx-3.2.2.dev31/rbx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-06 14:05:10.000000 rbx-3.2.2.dev31/rbx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 14:05:10.000000 rbx-3.2.2.dev31/rbx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 14:05:10.000000 rbx-3.2.2.dev31/rbx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:05:10.355751 rbx-3.2.2.dev31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-06 14:05:09.000000 rbx-3.2.2.dev31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.818238 rbx-3.3.0.dev32/rbx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/auth/keystore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/aws/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx/buildtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 13:52:10.000000 rbx-3.3.0.dev32/rbx/buildtools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx/buildtools/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/buildtools/tasks/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/adsquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/broadsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/oxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/clients/uslicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/gcp/cloud_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/gcp/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/geo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/geo/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/geo/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/manifest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/manifest/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/manifest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/queues/
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/queues/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/queues/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/utils/mdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/rbx/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-18 13:51:54.000000 rbx-3.3.0.dev32/rbx/web/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:11.822238 rbx-3.3.0.dev32/rbx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 13:52:11.000000 rbx-3.3.0.dev32/rbx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:52:11.826238 rbx-3.3.0.dev32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-18 13:52:10.000000 rbx-3.3.0.dev32/setup.py
```

### Comparing `rbx-3.2.2.dev31/LICENSE` & `rbx-3.3.0.dev32/LICENSE`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/PKG-INFO` & `rbx-3.3.0.dev32/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.2.2.dev31
+Version: 3.3.0.dev32
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,12 +23,13 @@
 Provides-Extra: geo
 Provides-Extra: manifest
 Provides-Extra: notifications
 Provides-Extra: platform
 Provides-Extra: queues
 Provides-Extra: storage
 Provides-Extra: tasks
+Provides-Extra: web
 Provides-Extra: test
 License-File: LICENSE
 
 A collection of common tools for Scoota services.
```

### Comparing `rbx-3.2.2.dev31/rbx/auth/decorators.py` & `rbx-3.3.0.dev32/rbx/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/auth/keystore.py` & `rbx-3.3.0.dev32/rbx/auth/keystore.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/aws/s3.py` & `rbx-3.3.0.dev32/rbx/aws/s3.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/buildtools/tasks/deploy.py` & `rbx-3.3.0.dev32/rbx/buildtools/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/buildtools/tasks/image.py` & `rbx-3.3.0.dev32/rbx/buildtools/tasks/image.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/buildtools/tasks/misc.py` & `rbx-3.3.0.dev32/rbx/buildtools/tasks/misc.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/clients/__init__.py` & `rbx-3.3.0.dev32/rbx/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/clients/adsquare.py` & `rbx-3.3.0.dev32/rbx/clients/adsquare.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/clients/broadsign.py` & `rbx-3.3.0.dev32/rbx/clients/broadsign.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/clients/oxr.py` & `rbx-3.3.0.dev32/rbx/clients/oxr.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/clients/panels.py` & `rbx-3.3.0.dev32/rbx/clients/panels.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/clients/reporting.py` & `rbx-3.3.0.dev32/rbx/clients/reporting.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/clients/retry.py` & `rbx-3.3.0.dev32/rbx/clients/retry.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/clients/uslicer.py` & `rbx-3.3.0.dev32/rbx/clients/uslicer.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/exceptions.py` & `rbx-3.3.0.dev32/rbx/exceptions.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/gcp/cloud_tasks.py` & `rbx-3.3.0.dev32/rbx/gcp/cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/gcp/pubsub.py` & `rbx-3.3.0.dev32/rbx/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/gcp/storage.py` & `rbx-3.3.0.dev32/rbx/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/geo/__init__.py` & `rbx-3.3.0.dev32/rbx/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/geo/cli.py` & `rbx-3.3.0.dev32/rbx/geo/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/geo/maps.py` & `rbx-3.3.0.dev32/rbx/geo/maps.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/geo/packer.py` & `rbx-3.3.0.dev32/rbx/geo/packer.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/logging.py` & `rbx-3.3.0.dev32/rbx/logging.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/manifest/cli.py` & `rbx-3.3.0.dev32/rbx/manifest/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/manifest/processor.py` & `rbx-3.3.0.dev32/rbx/manifest/processor.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/manifest/utils.py` & `rbx-3.3.0.dev32/rbx/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/queues/__init__.py` & `rbx-3.3.0.dev32/rbx/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/queues/jobs.py` & `rbx-3.3.0.dev32/rbx/queues/jobs.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/queues/scheduler.py` & `rbx-3.3.0.dev32/rbx/queues/scheduler.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx/utils/__init__.py` & `rbx-3.3.0.dev32/rbx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx.egg-info/PKG-INFO` & `rbx-3.3.0.dev32/rbx.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.2.2.dev31
+Version: 3.3.0.dev32
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,12 +23,13 @@
 Provides-Extra: geo
 Provides-Extra: manifest
 Provides-Extra: notifications
 Provides-Extra: platform
 Provides-Extra: queues
 Provides-Extra: storage
 Provides-Extra: tasks
+Provides-Extra: web
 Provides-Extra: test
 License-File: LICENSE
 
 A collection of common tools for Scoota services.
```

### Comparing `rbx-3.2.2.dev31/rbx.egg-info/SOURCES.txt` & `rbx-3.3.0.dev32/rbx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbx-3.2.2.dev31/rbx.egg-info/requires.txt` & `rbx-3.3.0.dev32/rbx.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -55,7 +55,11 @@
 google-cloud-pubsub<3,>=2.9
 redis<4.2,>3.5
 hiredis==2.0.0
 rq==1.10.1
 rq-scheduler==0.11.0
 google-cloud-storage<3,>=2.1
 google-cloud-tasks<3,>=2.7
+google-cloud-error-reporting<2,>=1.9.2
+
+[web]
+google-cloud-error-reporting<2,>=1.9.2
```

### Comparing `rbx-3.2.2.dev31/setup.py` & `rbx-3.3.0.dev32/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,20 @@
     "redis>3.5,<4.2",
     "hiredis==2.0.0",
     "rq==1.10.1",
     "rq-scheduler==0.11.0",
 ]
 STORAGE = ["google-cloud-storage>=2.1,<3"]
 TASKS = ["google-cloud-tasks>=2.7,<3"]
+WEB = ["google-cloud-error-reporting>=1.9.2,<2"]
 
 
 setup(
     name="rbx",
-    version="3.2.2.dev31",
+    version="3.3.0.dev32",
     license="Apache 2.0",
     description="Scoota Platform utilities",
     long_description="A collection of common tools for Scoota services.",
     url="http://scoota.com/",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
@@ -74,16 +75,17 @@
         "geo": MAPS,
         "manifest": MANIFEST,
         "notifications": NOTIFICATIONS,
         "platform": AUTH + MANIFEST + MAPS + NOTIFICATIONS + QUEUES,
         "queues": QUEUES,
         "storage": STORAGE,
         "tasks": TASKS,
+        "web": WEB,
         # Include them all for the test suite.
-        "test": AUTH + MANIFEST + MAPS + NOTIFICATIONS + QUEUES + STORAGE + TASKS,
+        "test": AUTH + MANIFEST + MAPS + NOTIFICATIONS + QUEUES + STORAGE + TASKS + WEB,
     },
     entry_points={
         "console_scripts": [
             "buildtools = rbx.buildtools.cli:program.run [buildtools]",
             "buildcreative = rbx.manifest.cli:build_creative [manifest]",
             "geocode = rbx.geo.cli:geocode [geo]",
             "reverse_geocode = rbx.geo.cli:reverse_geocode [geo]",
```

