# Comparing `tmp/llm-0.4.1.tar.gz` & `tmp/llm-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-0.4.1.tar", last modified: Sat Jun 17 21:41:31 2023, max compression
+gzip compressed data, was "llm-0.5.tar", last modified: Wed Jul 12 14:24:21 2023, max compression
```

## Comparing `llm-0.4.1.tar` & `llm-0.5.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:41:31.631900 llm-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-17 21:41:16.000000 llm-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-17 21:41:31.631900 llm-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-17 21:41:16.000000 llm-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:41:31.631900 llm-0.4.1/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 21:41:16.000000 llm-0.4.1/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 21:41:16.000000 llm-0.4.1/llm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-17 21:41:16.000000 llm-0.4.1/llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-17 21:41:16.000000 llm-0.4.1/llm/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:41:31.631900 llm-0.4.1/llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-17 21:41:31.000000 llm-0.4.1/llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 21:41:31.631900 llm-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-17 21:41:16.000000 llm-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:41:31.631900 llm-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-17 21:41:16.000000 llm-0.4.1/tests/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-17 21:41:16.000000 llm-0.4.1/tests/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-17 21:41:16.000000 llm-0.4.1/tests/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-17 21:41:16.000000 llm-0.4.1/tests/test_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:21.158298 llm-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 14:24:05.000000 llm-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 14:24:05.000000 llm-0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-12 14:24:21.158298 llm-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-12 14:24:05.000000 llm-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:21.150298 llm-0.5/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-12 14:24:05.000000 llm-0.5/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 14:24:05.000000 llm-0.5/llm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-07-12 14:24:05.000000 llm-0.5/llm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:21.158298 llm-0.5/llm/default_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:05.000000 llm-0.5/llm/default_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-07-12 14:24:05.000000 llm-0.5/llm/default_plugins/openai_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-12 14:24:05.000000 llm-0.5/llm/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-12 14:24:05.000000 llm-0.5/llm/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-12 14:24:05.000000 llm-0.5/llm/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-07-12 14:24:05.000000 llm-0.5/llm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-12 14:24:05.000000 llm-0.5/llm/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-12 14:24:05.000000 llm-0.5/llm/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-12 14:24:05.000000 llm-0.5/llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:24:21.158298 llm-0.5/llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-12 14:24:21.000000 llm-0.5/llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 14:24:21.000000 llm-0.5/llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:24:21.000000 llm-0.5/llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-12 14:24:21.000000 llm-0.5/llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 14:24:21.000000 llm-0.5/llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 14:24:21.000000 llm-0.5/llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:24:21.158298 llm-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-12 14:24:05.000000 llm-0.5/setup.py
```

### Comparing `llm-0.4.1/LICENSE` & `llm-0.5/LICENSE`

 * *Files identical despite different names*

