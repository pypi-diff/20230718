# Comparing `tmp/systembridgecli-3.8.0.dev5.tar.gz` & `tmp/systembridgecli-3.8.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgecli-3.8.0.dev5.tar", last modified: Tue Jul 18 09:48:47 2023, max compression
+gzip compressed data, was "systembridgecli-3.8.0.dev6.tar", last modified: Tue Jul 18 10:01:40 2023, max compression
```

## Comparing `systembridgecli-3.8.0.dev5.tar` & `systembridgecli-3.8.0.dev6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:48:47.568033 systembridgecli-3.8.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 09:48:47.568033 systembridgecli-3.8.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 09:48:04.000000 systembridgecli-3.8.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:48:47.568033 systembridgecli-3.8.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-18 09:48:04.000000 systembridgecli-3.8.0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:48:47.568033 systembridgecli-3.8.0.dev5/systembridgecli/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 09:48:04.000000 systembridgecli-3.8.0.dev5/systembridgecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-18 09:48:04.000000 systembridgecli-3.8.0.dev5/systembridgecli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 09:48:45.000000 systembridgecli-3.8.0.dev5/systembridgecli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:48:47.568033 systembridgecli-3.8.0.dev5/systembridgecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 09:48:47.000000 systembridgecli-3.8.0.dev5/systembridgecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-18 09:48:47.000000 systembridgecli-3.8.0.dev5/systembridgecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:48:47.000000 systembridgecli-3.8.0.dev5/systembridgecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 09:48:47.000000 systembridgecli-3.8.0.dev5/systembridgecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 09:48:47.000000 systembridgecli-3.8.0.dev5/systembridgecli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:01:40.326805 systembridgecli-3.8.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 10:01:40.326805 systembridgecli-3.8.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 10:01:04.000000 systembridgecli-3.8.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:01:40.326805 systembridgecli-3.8.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-18 10:01:04.000000 systembridgecli-3.8.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:01:40.326805 systembridgecli-3.8.0.dev6/systembridgecli/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 10:01:04.000000 systembridgecli-3.8.0.dev6/systembridgecli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-18 10:01:04.000000 systembridgecli-3.8.0.dev6/systembridgecli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 10:01:38.000000 systembridgecli-3.8.0.dev6/systembridgecli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:01:40.326805 systembridgecli-3.8.0.dev6/systembridgecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 10:01:40.000000 systembridgecli-3.8.0.dev6/systembridgecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-18 10:01:40.000000 systembridgecli-3.8.0.dev6/systembridgecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:01:40.000000 systembridgecli-3.8.0.dev6/systembridgecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 10:01:40.000000 systembridgecli-3.8.0.dev6/systembridgecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 10:01:40.000000 systembridgecli-3.8.0.dev6/systembridgecli.egg-info/top_level.txt
```

### Comparing `systembridgecli-3.8.0.dev5/pyproject.toml` & `systembridgecli-3.8.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgecli-3.8.0.dev5/setup.py` & `systembridgecli-3.8.0.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgecli-3.8.0.dev5/systembridgecli/__main__.py` & `systembridgecli-3.8.0.dev6/systembridgecli/__main__.py`

 * *Files identical despite different names*

