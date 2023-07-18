# Comparing `tmp/pipsqlite3mod-1.0.0.tar.gz` & `tmp/pipsqlite3mod-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlite3mod-1.0.0.tar", last modified: Tue Jul 18 01:34:24 2023, max compression
+gzip compressed data, was "pipsqlite3mod-1.1.0.tar", last modified: Tue Jul 18 01:36:29 2023, max compression
```

## Comparing `pipsqlite3mod-1.0.0.tar` & `pipsqlite3mod-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:34:24.544520 pipsqlite3mod-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      346 2023-07-18 01:34:24.544520 pipsqlite3mod-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:34:24.544520 pipsqlite3mod-1.0.0/pipsqlite3mod/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 01:34:23.000000 pipsqlite3mod-1.0.0/pipsqlite3mod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:34:24.544520 pipsqlite3mod-1.0.0/pipsqlite3mod.egg-info/
--rw-r--r--   0 root         (0) root         (0)      346 2023-07-18 01:34:24.000000 pipsqlite3mod-1.0.0/pipsqlite3mod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-18 01:34:24.000000 pipsqlite3mod-1.0.0/pipsqlite3mod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 01:34:24.000000 pipsqlite3mod-1.0.0/pipsqlite3mod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-18 01:34:24.000000 pipsqlite3mod-1.0.0/pipsqlite3mod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 01:34:24.548520 pipsqlite3mod-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-18 01:34:23.000000 pipsqlite3mod-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:36:29.336080 pipsqlite3mod-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-07-18 01:36:29.332080 pipsqlite3mod-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:36:29.332080 pipsqlite3mod-1.1.0/pipsqlite3mod/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-18 01:36:28.000000 pipsqlite3mod-1.1.0/pipsqlite3mod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:36:29.332080 pipsqlite3mod-1.1.0/pipsqlite3mod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      346 2023-07-18 01:36:29.000000 pipsqlite3mod-1.1.0/pipsqlite3mod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-18 01:36:29.000000 pipsqlite3mod-1.1.0/pipsqlite3mod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 01:36:29.000000 pipsqlite3mod-1.1.0/pipsqlite3mod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-18 01:36:29.000000 pipsqlite3mod-1.1.0/pipsqlite3mod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 01:36:29.336080 pipsqlite3mod-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-18 01:36:28.000000 pipsqlite3mod-1.1.0/setup.py
```

### Comparing `pipsqlite3mod-1.0.0/setup.py` & `pipsqlite3mod-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipsqlite3mod",
     version=VERSION,
```

