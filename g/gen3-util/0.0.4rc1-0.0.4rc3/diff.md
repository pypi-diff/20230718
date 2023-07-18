# Comparing `tmp/gen3_util-0.0.4rc1.tar.gz` & `tmp/gen3_util-0.0.4rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.4rc1.tar", last modified: Mon Jul 17 22:35:51 2023, max compression
+gzip compressed data, was "gen3_util-0.0.4rc3.tar", last modified: Tue Jul 18 02:32:51 2023, max compression
```

## Comparing `gen3_util-0.0.4rc1.tar` & `gen3_util-0.0.4rc3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.555956 gen3_util-0.0.4rc1/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.4rc1/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     9566 2023-07-17 22:35:51.555703 gen3_util-0.0.4rc1/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     8881 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc1/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.525368 gen3_util-0.0.4rc1/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-07-05 18:55:42.000000 gen3_util-0.0.4rc1/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.530012 gen3_util-0.0.4rc1/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4281 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc1/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.536167 gen3_util-0.0.4rc1/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5679 2023-07-11 14:24:51.000000 gen3_util-0.0.4rc1/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.538919 gen3_util-0.0.4rc1/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc1/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc1/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc1/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.540994 gen3_util-0.0.4rc1/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc1/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.541963 gen3_util-0.0.4rc1/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142     5262 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc1/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.542851 gen3_util-0.0.4rc1/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc1/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc1/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.546043 gen3_util-0.0.4rc1/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc1/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2437 2023-07-17 22:26:17.000000 gen3_util-0.0.4rc1/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      938 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc1/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc1/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    12933 2023-07-17 22:34:16.000000 gen3_util-0.0.4rc1/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.550311 gen3_util-0.0.4rc1/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.4rc1/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      323 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    11295 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc1/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      329 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc1/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3299 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc1/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.551624 gen3_util-0.0.4rc1/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc1/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.4rc1/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc1/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc1/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.528422 gen3_util-0.0.4rc1/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     9566 2023-07-17 22:35:51.000000 gen3_util-0.0.4rc1/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1687 2023-07-17 22:35:51.000000 gen3_util-0.0.4rc1/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-07-17 22:35:51.000000 gen3_util-0.0.4rc1/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-07-17 22:35:51.000000 gen3_util-0.0.4rc1/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-07-17 22:35:51.000000 gen3_util-0.0.4rc1/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-07-17 22:35:51.000000 gen3_util-0.0.4rc1/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-07-17 22:35:51.556018 gen3_util-0.0.4rc1/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5579 2023-07-17 22:34:24.000000 gen3_util-0.0.4rc1/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.518164 gen3_util-0.0.4rc1/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.553416 gen3_util-0.0.4rc1/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc1/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      270 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc1/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4358 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc1/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      454 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc1/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      243 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc1/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4318 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc1/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.555028 gen3_util-0.0.4rc1/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc1/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc1/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.555222 gen3_util-0.0.4rc1/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc1/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-07-17 22:35:51.555417 gen3_util-0.0.4rc1/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc1/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc1/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc1/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc1/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4616 2023-07-07 18:51:14.000000 gen3_util-0.0.4rc1/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc1/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.491107 gen3_util-0.0.4rc3/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.4rc3/LICENSE
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9640 2023-07-18 02:32:51.490781 gen3_util-0.0.4rc3/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8955 2023-07-17 23:27:29.000000 gen3_util-0.0.4rc3/README.md
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.389797 gen3_util-0.0.4rc3/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       71 2023-07-05 18:55:42.000000 gen3_util-0.0.4rc3/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.405052 gen3_util-0.0.4rc3/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4281 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/gen3_util/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.405539 gen3_util-0.0.4rc3/gen3_util/access/policies/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5679 2023-07-11 14:24:51.000000 gen3_util-0.0.4rc3/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.407241 gen3_util-0.0.4rc3/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      803 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      629 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc3/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      474 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.408144 gen3_util-0.0.4rc3/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc3/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.408694 gen3_util-0.0.4rc3/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5262 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.422520 gen3_util-0.0.4rc3/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      433 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      503 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.425151 gen3_util-0.0.4rc3/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc3/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2437 2023-07-17 22:26:17.000000 gen3_util-0.0.4rc3/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      938 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      192 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      202 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    12953 2023-07-18 02:31:06.000000 gen3_util-0.0.4rc3/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.440148 gen3_util-0.0.4rc3/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      323 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    11295 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc3/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      329 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      201 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3299 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc3/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.462326 gen3_util-0.0.4rc3/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc3/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.4rc3/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      793 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc3/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.402115 gen3_util-0.0.4rc3/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9640 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1687 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       53 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      155 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       16 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2023-07-18 02:32:51.491183 gen3_util-0.0.4rc3/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5579 2023-07-18 02:32:27.000000 gen3_util-0.0.4rc3/setup.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.376731 gen3_util-0.0.4rc3/tests/
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.487563 gen3_util-0.0.4rc3/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      270 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4358 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      454 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      243 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/tests/integration/test_config.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4318 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc3/tests/integration/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.489866 gen3_util-0.0.4rc3/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      322 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/unit/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.490195 gen3_util-0.0.4rc3/tests/unit/plugins/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.490433 gen3_util-0.0.4rc3/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1450 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      565 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      551 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4616 2023-07-07 18:51:14.000000 gen3_util-0.0.4rc3/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.4rc1/LICENSE` & `gen3_util-0.0.4rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/PKG-INFO` & `gen3_util-0.0.4rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_util
-Version: 0.0.4rc1
+Version: 0.0.4rc3
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
@@ -29,28 +29,28 @@
 
 # optionally
 $python3 -m venv venv ; source venv/bin/activate
 
 pip install gen3_util
 
 $ gen3_util
-msg: Version 0.0.3
+msg: Version 0.0.4
 
 
 ```
 
 Note: requires [`magic`](https://github.com/ahupp/python-magic#installation) library. If it is not already installed you will see a warning like this:
 
 ```text
 Requires libmagic installed on your system to determine mime-types
 Error: 'failed to find libmagic.  Check your installation'
 For installation instructions see https://github.com/ahupp/python-magic#installation
 ```
 
-
+Note: some environments will get a `_ctypes` error.  Please install 3.9.16
 
 ## Use
 
 ```
 $gen3_util --help
 Usage: gen3_util [OPTIONS] COMMAND [ARGS]...
```

### Comparing `gen3_util-0.0.4rc1/README.md` & `gen3_util-0.0.4rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 # optionally
 $python3 -m venv venv ; source venv/bin/activate
 
 pip install gen3_util
 
 $ gen3_util
-msg: Version 0.0.3
+msg: Version 0.0.4
 
 
 ```
 
 Note: requires [`magic`](https://github.com/ahupp/python-magic#installation) library. If it is not already installed you will see a warning like this:
 
 ```text
 Requires libmagic installed on your system to determine mime-types
 Error: 'failed to find libmagic.  Check your installation'
 For installation instructions see https://github.com/ahupp/python-magic#installation
 ```
 
-
+Note: some environments will get a `_ctypes` error.  Please install 3.9.16
 
 ## Use
 
 ```
 $gen3_util --help
 Usage: gen3_util [OPTIONS] COMMAND [ARGS]...
```

### Comparing `gen3_util-0.0.4rc1/gen3_util/access/__init__.py` & `gen3_util-0.0.4rc3/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/access/cli.py` & `gen3_util-0.0.4rc3/gen3_util/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/access/requestor.py` & `gen3_util-0.0.4rc3/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/buckets/__init__.py` & `gen3_util-0.0.4rc3/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/buckets/cli.py` & `gen3_util-0.0.4rc3/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/cli/__init__.py` & `gen3_util-0.0.4rc3/gen3_util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/cli/cli.py` & `gen3_util-0.0.4rc3/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/common/__init__.py` & `gen3_util-0.0.4rc3/gen3_util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/config/__init__.py` & `gen3_util-0.0.4rc3/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/files/__init__.py` & `gen3_util-0.0.4rc3/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/files/cli.py` & `gen3_util-0.0.4rc3/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/files/downloader.py` & `gen3_util-0.0.4rc3/gen3_util/files/downloader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/files/uploader.py` & `gen3_util-0.0.4rc3/gen3_util/files/uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,16 @@
 
         file_client, index_client, user = gen3_services(config=config)
 
         attachment, md5sum, source_path_extension = _extract_extensions(document_reference)
 
         source_path = _extract_source_path(attachment, source_path, source_path_extension)
 
-        file_name = source_path.lstrip('./').lstrip('file:///')
-        object_name = attachment['url'].lstrip('./').lstrip('file:///')
+        file_name = source_path.replace('./', '').replace('file:///', '')
+        object_name = attachment['url'].replace('./', '').replace('file:///', '')
 
         metadata = _update_indexd(attachment, bucket_name, document_reference, duplicate_check, index_client, md5sum,
                                   object_name, program, project)
 
         # create a record in gen3 using document_reference's id as guid, get a signed url
         # SYNC
```

### Comparing `gen3_util-0.0.4rc1/gen3_util/meta/__init__.py` & `gen3_util-0.0.4rc3/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/meta/cli.py` & `gen3_util-0.0.4rc3/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/meta/importer.py` & `gen3_util-0.0.4rc3/gen3_util/meta/importer.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/meta/uploader.py` & `gen3_util-0.0.4rc3/gen3_util/meta/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/meta/validator.py` & `gen3_util-0.0.4rc3/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/projects/__init__.py` & `gen3_util-0.0.4rc3/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/projects/cli.py` & `gen3_util-0.0.4rc3/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/projects/creator.py` & `gen3_util-0.0.4rc3/gen3_util/projects/creator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/projects/lister.py` & `gen3_util-0.0.4rc3/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util/projects/remover.py` & `gen3_util-0.0.4rc3/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/gen3_util.egg-info/PKG-INFO` & `gen3_util-0.0.4rc3/gen3_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-util
-Version: 0.0.4rc1
+Version: 0.0.4rc3
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
@@ -29,28 +29,28 @@
 
 # optionally
 $python3 -m venv venv ; source venv/bin/activate
 
 pip install gen3_util
 
 $ gen3_util
-msg: Version 0.0.3
+msg: Version 0.0.4
 
 
 ```
 
 Note: requires [`magic`](https://github.com/ahupp/python-magic#installation) library. If it is not already installed you will see a warning like this:
 
 ```text
 Requires libmagic installed on your system to determine mime-types
 Error: 'failed to find libmagic.  Check your installation'
 For installation instructions see https://github.com/ahupp/python-magic#installation
 ```
 
-
+Note: some environments will get a `_ctypes` error.  Please install 3.9.16
 
 ## Use
 
 ```
 $gen3_util --help
 Usage: gen3_util [OPTIONS] COMMAND [ARGS]...
```

### Comparing `gen3_util-0.0.4rc1/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.4rc3/gen3_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/setup.py` & `gen3_util-0.0.4rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.4rc1',  # Required
+    version='0.0.4rc3',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.4rc1/tests/integration/test_access.py` & `gen3_util-0.0.4rc3/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/integration/test_files.py` & `gen3_util-0.0.4rc3/tests/integration/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/integration/test_meta.py` & `gen3_util-0.0.4rc3/tests/integration/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/integration/test_project.py` & `gen3_util-0.0.4rc3/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py` & `gen3_util-0.0.4rc3/tests/unit/plugins/gen3_util_plugin_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/unit/test_cli.py` & `gen3_util-0.0.4rc3/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.4rc3/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/unit/test_config.py` & `gen3_util-0.0.4rc3/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/unit/test_files.py` & `gen3_util-0.0.4rc3/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/unit/test_meta.py` & `gen3_util-0.0.4rc3/tests/unit/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc1/tests/unit/test_validate_directory.py` & `gen3_util-0.0.4rc3/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

