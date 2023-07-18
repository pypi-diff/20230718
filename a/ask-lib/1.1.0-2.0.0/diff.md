# Comparing `tmp/ask_lib-1.1.0.tar.gz` & `tmp/ask_lib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ask_lib-1.1.0.tar", last modified: Sun Aug  1 19:24:18 2021, max compression
+gzip compressed data, was "ask_lib-2.0.0.tar", max compression
```

## Comparing `ask_lib-1.1.0.tar` & `ask_lib-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxrwxrwx   0        0        0        0 2021-08-01 19:24:18.581682 ask_lib-1.1.0/
--rw-rw-rw-   0        0        0     1090 2021-07-31 10:42:40.000000 ask_lib-1.1.0/LICENCE
--rw-rw-rw-   0        0        0     1929 2021-08-01 19:24:18.582176 ask_lib-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1360 2021-08-01 19:23:58.000000 ask_lib-1.1.0/README.md
--rw-rw-rw-   0        0        0      108 2021-07-31 10:35:57.000000 ask_lib-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      666 2021-08-01 19:24:18.584657 ask_lib-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-08-01 19:24:18.537536 ask_lib-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2021-08-01 19:24:18.565809 ask_lib-1.1.0/src/ask_lib/
--rw-rw-rw-   0        0        0       22 2021-07-31 13:28:08.000000 ask_lib-1.1.0/src/ask_lib/__init__.py
--rw-rw-rw-   0        0        0     6367 2021-08-01 19:21:21.000000 ask_lib-1.1.0/src/ask_lib/ask_lib.py
-drwxrwxrwx   0        0        0        0 2021-08-01 19:24:18.578705 ask_lib-1.1.0/src/ask_lib.egg-info/
--rw-rw-rw-   0        0        0     1929 2021-08-01 19:24:18.000000 ask_lib-1.1.0/src/ask_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2021-08-01 19:24:18.000000 ask_lib-1.1.0/src/ask_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-01 19:24:18.000000 ask_lib-1.1.0/src/ask_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2021-08-01 19:24:18.000000 ask_lib-1.1.0/src/ask_lib.egg-info/top_level.txt
+-rw-r--r--   0        0        0      857 2023-07-18 15:00:10.249484 ask_lib-2.0.0/README.md
+-rw-r--r--   0        0        0      199 2023-07-18 18:27:18.028928 ask_lib-2.0.0/ask_lib/__init__.py
+-rw-r--r--   0        0        0     2018 2023-07-18 14:50:41.934893 ask_lib-2.0.0/ask_lib/ask.py
+-rw-r--r--   0        0        0     1084 2023-07-18 18:27:18.032928 ask_lib-2.0.0/ask_lib/ask_flag.py
+-rw-r--r--   0        0        0      591 2023-07-18 18:08:14.143648 ask_lib-2.0.0/ask_lib/ask_result.py
+-rw-r--r--   0        0        0      565 2023-07-18 18:07:20.697294 ask_lib-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 ask_lib-2.0.0/PKG-INFO
```

