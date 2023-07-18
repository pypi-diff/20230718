# Comparing `tmp/gen3_util-0.0.4rc3.tar.gz` & `tmp/gen3_util-0.0.4rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.4rc3.tar", last modified: Tue Jul 18 02:32:51 2023, max compression
+gzip compressed data, was "gen3_util-0.0.4rc4.tar", last modified: Tue Jul 18 16:42:42 2023, max compression
```

## Comparing `gen3_util-0.0.4rc3.tar` & `gen3_util-0.0.4rc4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.491107 gen3_util-0.0.4rc3/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.4rc3/LICENSE
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9640 2023-07-18 02:32:51.490781 gen3_util-0.0.4rc3/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8955 2023-07-17 23:27:29.000000 gen3_util-0.0.4rc3/README.md
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.389797 gen3_util-0.0.4rc3/gen3_util/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       71 2023-07-05 18:55:42.000000 gen3_util-0.0.4rc3/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.405052 gen3_util-0.0.4rc3/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4281 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.405539 gen3_util-0.0.4rc3/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5679 2023-07-11 14:24:51.000000 gen3_util-0.0.4rc3/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.407241 gen3_util-0.0.4rc3/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      803 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      629 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc3/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      474 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.408144 gen3_util-0.0.4rc3/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc3/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.408694 gen3_util-0.0.4rc3/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5262 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.422520 gen3_util-0.0.4rc3/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      433 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      503 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.425151 gen3_util-0.0.4rc3/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc3/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2437 2023-07-17 22:26:17.000000 gen3_util-0.0.4rc3/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      938 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      192 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      202 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    12953 2023-07-18 02:31:06.000000 gen3_util-0.0.4rc3/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.440148 gen3_util-0.0.4rc3/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      323 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    11295 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc3/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      329 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      201 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3299 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc3/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.462326 gen3_util-0.0.4rc3/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc3/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.4rc3/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      793 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc3/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.402115 gen3_util-0.0.4rc3/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9640 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1687 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       53 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      155 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       16 2023-07-18 02:32:51.000000 gen3_util-0.0.4rc3/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2023-07-18 02:32:51.491183 gen3_util-0.0.4rc3/setup.cfg
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5579 2023-07-18 02:32:27.000000 gen3_util-0.0.4rc3/setup.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.376731 gen3_util-0.0.4rc3/tests/
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.487563 gen3_util-0.0.4rc3/tests/integration/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      270 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4358 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      454 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      243 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc3/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4318 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc3/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.489866 gen3_util-0.0.4rc3/tests/unit/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      322 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.490195 gen3_util-0.0.4rc3/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 02:32:51.490433 gen3_util-0.0.4rc3/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1450 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc3/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc3/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      565 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      551 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc3/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4616 2023-07-07 18:51:14.000000 gen3_util-0.0.4rc3/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc3/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.830664 gen3_util-0.0.4rc4/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.4rc4/LICENSE
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9640 2023-07-18 16:42:42.830411 gen3_util-0.0.4rc4/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     8955 2023-07-17 23:27:29.000000 gen3_util-0.0.4rc4/README.md
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.803073 gen3_util-0.0.4rc4/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       71 2023-07-05 18:55:42.000000 gen3_util-0.0.4rc4/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.812004 gen3_util-0.0.4rc4/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2321 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4281 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc4/gen3_util/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.812347 gen3_util-0.0.4rc4/gen3_util/access/policies/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5679 2023-07-11 14:24:51.000000 gen3_util-0.0.4rc4/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.815714 gen3_util-0.0.4rc4/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      803 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc4/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      629 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc4/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      474 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc4/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.818013 gen3_util-0.0.4rc4/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4637 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.4rc4/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.818987 gen3_util-0.0.4rc4/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5262 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc4/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.822049 gen3_util-0.0.4rc4/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2824 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      433 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc4/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      503 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc4/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.823619 gen3_util-0.0.4rc4/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc4/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2437 2023-07-17 22:26:17.000000 gen3_util-0.0.4rc4/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      938 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      192 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc4/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      202 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc4/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    13121 2023-07-18 14:08:52.000000 gen3_util-0.0.4rc4/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.825308 gen3_util-0.0.4rc4/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4101 2023-07-07 00:01:20.000000 gen3_util-0.0.4rc4/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2256 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      323 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)    11295 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc4/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      329 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      201 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc4/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3858 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3299 2023-07-11 21:14:30.000000 gen3_util-0.0.4rc4/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.826408 gen3_util-0.0.4rc4/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc4/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2769 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1901 2023-06-30 03:26:36.000000 gen3_util-0.0.4rc4/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      793 2023-06-21 17:42:55.000000 gen3_util-0.0.4rc4/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1078 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc4/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.810885 gen3_util-0.0.4rc4/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     9640 2023-07-18 16:42:42.000000 gen3_util-0.0.4rc4/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1687 2023-07-18 16:42:42.000000 gen3_util-0.0.4rc4/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        1 2023-07-18 16:42:42.000000 gen3_util-0.0.4rc4/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       53 2023-07-18 16:42:42.000000 gen3_util-0.0.4rc4/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      141 2023-07-18 16:42:42.000000 gen3_util-0.0.4rc4/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       16 2023-07-18 16:42:42.000000 gen3_util-0.0.4rc4/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)       38 2023-07-18 16:42:42.830729 gen3_util-0.0.4rc4/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5579 2023-07-18 15:51:28.000000 gen3_util-0.0.4rc4/setup.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.788169 gen3_util-0.0.4rc4/tests/
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.828192 gen3_util-0.0.4rc4/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc4/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      275 2023-07-18 15:42:11.000000 gen3_util-0.0.4rc4/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4358 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc4/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      454 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc4/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      243 2023-06-28 20:29:46.000000 gen3_util-0.0.4rc4/tests/integration/test_config.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2089 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     5134 2023-07-18 15:48:25.000000 gen3_util-0.0.4rc4/tests/integration/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1237 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.829756 gen3_util-0.0.4rc4/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc4/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      322 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc4/tests/unit/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.829961 gen3_util-0.0.4rc4/tests/unit/plugins/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc4/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)        0 2023-07-18 16:42:42.830141 gen3_util-0.0.4rc4/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1450 2023-07-07 00:45:48.000000 gen3_util-0.0.4rc4/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     3380 2023-07-07 00:00:20.000000 gen3_util-0.0.4rc4/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      565 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc4/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)      551 2023-05-05 20:31:25.000000 gen3_util-0.0.4rc4/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     2350 2023-07-18 14:05:51.000000 gen3_util-0.0.4rc4/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     4616 2023-07-07 18:51:14.000000 gen3_util-0.0.4rc4/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) OHSUM01\Domain Users (1971611142)     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.4rc4/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.4rc3/LICENSE` & `gen3_util-0.0.4rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/PKG-INFO` & `gen3_util-0.0.4rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_util
-Version: 0.0.4rc3
+Version: 0.0.4rc4
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.4rc3/README.md` & `gen3_util-0.0.4rc4/README.md`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/access/__init__.py` & `gen3_util-0.0.4rc4/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/access/cli.py` & `gen3_util-0.0.4rc4/gen3_util/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/access/requestor.py` & `gen3_util-0.0.4rc4/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/buckets/__init__.py` & `gen3_util-0.0.4rc4/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/buckets/cli.py` & `gen3_util-0.0.4rc4/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/cli/__init__.py` & `gen3_util-0.0.4rc4/gen3_util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/cli/cli.py` & `gen3_util-0.0.4rc4/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/common/__init__.py` & `gen3_util-0.0.4rc4/gen3_util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/config/__init__.py` & `gen3_util-0.0.4rc4/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/files/__init__.py` & `gen3_util-0.0.4rc4/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/files/cli.py` & `gen3_util-0.0.4rc4/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/files/downloader.py` & `gen3_util-0.0.4rc4/gen3_util/files/downloader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/files/uploader.py` & `gen3_util-0.0.4rc4/gen3_util/files/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 import base64
 import datetime
 import logging
 import pathlib
+import re
 import urllib
 from dataclasses import dataclass
 from multiprocessing import Pool
 from time import sleep
 from typing import List
 from urllib.parse import urlparse, ParseResult
 
@@ -140,30 +141,37 @@
     """The source document reference."""
     elapsed: [datetime.timedelta, None]
     """Amount of time it took to upload."""
     exception: Exception = None
     """On error."""
 
 
+def _normalize_file_url(path: str) -> str:
+    """Strip leading ./ and file:/// from file urls."""
+    path = re.sub(r'^\.\/', '', path)
+    path = re.sub(r'^file:\/\/\/', '', path)
+    return path
+
+
 def _upload_document_reference(config: Config, document_reference: dict, bucket_name: str,
                                program: str, project: str, duplicate_check: bool,
                                source_path: str) -> UploadResult:
     """Write a single document reference to indexd and upload file."""
 
     try:
         start = datetime.datetime.now()
 
         file_client, index_client, user = gen3_services(config=config)
 
         attachment, md5sum, source_path_extension = _extract_extensions(document_reference)
 
         source_path = _extract_source_path(attachment, source_path, source_path_extension)
 
-        file_name = source_path.replace('./', '').replace('file:///', '')
-        object_name = attachment['url'].replace('./', '').replace('file:///', '')
+        file_name = _normalize_file_url(source_path)
+        object_name = _normalize_file_url(attachment['url'])
 
         metadata = _update_indexd(attachment, bucket_name, document_reference, duplicate_check, index_client, md5sum,
                                   object_name, program, project)
 
         # create a record in gen3 using document_reference's id as guid, get a signed url
         # SYNC
```

### Comparing `gen3_util-0.0.4rc3/gen3_util/meta/__init__.py` & `gen3_util-0.0.4rc4/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/meta/cli.py` & `gen3_util-0.0.4rc4/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/meta/importer.py` & `gen3_util-0.0.4rc4/gen3_util/meta/importer.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/meta/uploader.py` & `gen3_util-0.0.4rc4/gen3_util/meta/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/meta/validator.py` & `gen3_util-0.0.4rc4/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/projects/__init__.py` & `gen3_util-0.0.4rc4/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/projects/cli.py` & `gen3_util-0.0.4rc4/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/projects/creator.py` & `gen3_util-0.0.4rc4/gen3_util/projects/creator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/projects/lister.py` & `gen3_util-0.0.4rc4/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util/projects/remover.py` & `gen3_util-0.0.4rc4/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/gen3_util.egg-info/PKG-INFO` & `gen3_util-0.0.4rc4/gen3_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-util
-Version: 0.0.4rc3
+Version: 0.0.4rc4
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.4rc3/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.4rc4/gen3_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/setup.py` & `gen3_util-0.0.4rc4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.4rc3',  # Required
+    version='0.0.4rc4',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.4rc3/tests/integration/test_access.py` & `gen3_util-0.0.4rc4/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/tests/integration/test_files.py` & `gen3_util-0.0.4rc4/tests/integration/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/tests/integration/test_meta.py` & `gen3_util-0.0.4rc4/tests/integration/test_meta.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import pathlib
 import shutil
+import subprocess
 import uuid
 
 from click.testing import CliRunner
 
 from gen3_util.cli.cli import cli
 
 
@@ -45,14 +46,28 @@
     print(result.output)
     assert result.exit_code == 0
     expected_strings = ['Uploaded']
     for expected_string in expected_strings:
         assert expected_string in result.output, f"{expected_string} not found in {result.output}"
 
 
+def run_cmd(command_line) -> str:
+    """Run a command line, return stdout."""
+    try:
+        return subprocess.check_output(command_line, shell=True).decode("utf-8").rstrip()
+    except Exception as exc:
+        raise exc
+
+
+def meta_cp_download_via_gen3(did, tmp_dir_name):
+    params = f'gen3 file download-single --path {tmp_dir_name} {did}'
+    print(params)
+    _ = run_cmd(params)
+
+
 def meta_cp_download(did, tmp_dir_name):
     params = f'--format json meta cp {did} {tmp_dir_name}'.split()
     runner = CliRunner()
     result = runner.invoke(cli, params)
     print(result.output)
     assert result.exit_code == 0
     expected_strings = ['Downloaded']
@@ -105,14 +120,21 @@
 
     create_project(project_id)
     add_policies(project_id)
 
     import_from_directory(tmp_dir_name, project_id)
 
     meta_cp_upload(tmp_dir_name, data_bucket, project_id)
+    program, project = project_id.split('-')
     records = ls()['records']
+    found_our_project = False
     for _ in records:
+        if f"/programs/{program}/projects/{project}" not in _['authz']:
+            continue
+        found_our_project = True
         meta_cp_download(_['did'], tmp_dir_name)
         stat = pathlib.Path(f"{tmp_dir_name}/{_['file_name']}").stat()
         assert stat.st_size == _['size']
-
+        # should also be able to use `gen3 file download-single`
+        meta_cp_download_via_gen3(_['did'], tmp_dir_name)
+    assert found_our_project, f"Did not find our project {project_id} in {records}"
     shutil.rmtree(tmp_dir_name)
```

### Comparing `gen3_util-0.0.4rc3/tests/integration/test_project.py` & `gen3_util-0.0.4rc4/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/tests/unit/plugins/gen3_util_plugin_foo/__init__.py` & `gen3_util-0.0.4rc4/tests/unit/plugins/gen3_util_plugin_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/tests/unit/test_cli.py` & `gen3_util-0.0.4rc4/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.4rc4/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/tests/unit/test_config.py` & `gen3_util-0.0.4rc4/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/tests/unit/test_meta.py` & `gen3_util-0.0.4rc4/tests/unit/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.4rc3/tests/unit/test_validate_directory.py` & `gen3_util-0.0.4rc4/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

