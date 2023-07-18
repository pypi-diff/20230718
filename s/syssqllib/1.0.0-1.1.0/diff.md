# Comparing `tmp/syssqllib-1.0.0.tar.gz` & `tmp/syssqllib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqllib-1.0.0.tar", last modified: Tue Jul 18 01:48:25 2023, max compression
+gzip compressed data, was "syssqllib-1.1.0.tar", last modified: Tue Jul 18 01:50:30 2023, max compression
```

## Comparing `syssqllib-1.0.0.tar` & `syssqllib-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:48:25.577650 syssqllib-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-18 01:48:25.577650 syssqllib-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 01:48:25.577650 syssqllib-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      555 2023-07-18 01:48:25.000000 syssqllib-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:48:25.577650 syssqllib-1.0.0/syssqllib/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 01:48:25.000000 syssqllib-1.0.0/syssqllib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:48:25.577650 syssqllib-1.0.0/syssqllib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-18 01:48:25.000000 syssqllib-1.0.0/syssqllib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-18 01:48:25.000000 syssqllib-1.0.0/syssqllib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 01:48:25.000000 syssqllib-1.0.0/syssqllib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-18 01:48:25.000000 syssqllib-1.0.0/syssqllib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:50:30.645297 syssqllib-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-18 01:50:30.645297 syssqllib-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 01:50:30.645297 syssqllib-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      555 2023-07-18 01:50:30.000000 syssqllib-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:50:30.645297 syssqllib-1.1.0/syssqllib/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-18 01:50:30.000000 syssqllib-1.1.0/syssqllib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:50:30.645297 syssqllib-1.1.0/syssqllib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-18 01:50:30.000000 syssqllib-1.1.0/syssqllib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-18 01:50:30.000000 syssqllib-1.1.0/syssqllib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 01:50:30.000000 syssqllib-1.1.0/syssqllib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-18 01:50:30.000000 syssqllib-1.1.0/syssqllib.egg-info/top_level.txt
```

### Comparing `syssqllib-1.0.0/setup.py` & `syssqllib-1.1.0/setup.py`

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
     name="syssqllib",
     version=VERSION,
```

