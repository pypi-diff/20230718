# Comparing `tmp/pythoncolouringsliberyV1-1.0.0.tar.gz` & `tmp/pythoncolouringsliberyV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncolouringsliberyV1-1.0.0.tar", last modified: Tue Jul 18 19:22:18 2023, max compression
+gzip compressed data, was "pythoncolouringsliberyV1-1.1.0.tar", last modified: Tue Jul 18 19:24:23 2023, max compression
```

## Comparing `pythoncolouringsliberyV1-1.0.0.tar` & `pythoncolouringsliberyV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:22:18.497978 pythoncolouringsliberyV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      357 2023-07-18 19:22:18.497978 pythoncolouringsliberyV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:22:18.497978 pythoncolouringsliberyV1-1.0.0/pythoncolouringsliberyV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 19:22:18.000000 pythoncolouringsliberyV1-1.0.0/pythoncolouringsliberyV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:22:18.497978 pythoncolouringsliberyV1-1.0.0/pythoncolouringsliberyV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      357 2023-07-18 19:22:18.000000 pythoncolouringsliberyV1-1.0.0/pythoncolouringsliberyV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-18 19:22:18.000000 pythoncolouringsliberyV1-1.0.0/pythoncolouringsliberyV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 19:22:18.000000 pythoncolouringsliberyV1-1.0.0/pythoncolouringsliberyV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-18 19:22:18.000000 pythoncolouringsliberyV1-1.0.0/pythoncolouringsliberyV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 19:22:18.497978 pythoncolouringsliberyV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      570 2023-07-18 19:22:18.000000 pythoncolouringsliberyV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:24:23.485602 pythoncolouringsliberyV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-07-18 19:24:23.485602 pythoncolouringsliberyV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:24:23.485602 pythoncolouringsliberyV1-1.1.0/pythoncolouringsliberyV1/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-18 19:24:22.000000 pythoncolouringsliberyV1-1.1.0/pythoncolouringsliberyV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:24:23.485602 pythoncolouringsliberyV1-1.1.0/pythoncolouringsliberyV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-07-18 19:24:23.000000 pythoncolouringsliberyV1-1.1.0/pythoncolouringsliberyV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-18 19:24:23.000000 pythoncolouringsliberyV1-1.1.0/pythoncolouringsliberyV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 19:24:23.000000 pythoncolouringsliberyV1-1.1.0/pythoncolouringsliberyV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-18 19:24:23.000000 pythoncolouringsliberyV1-1.1.0/pythoncolouringsliberyV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 19:24:23.485602 pythoncolouringsliberyV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      570 2023-07-18 19:24:22.000000 pythoncolouringsliberyV1-1.1.0/setup.py
```

### Comparing `pythoncolouringsliberyV1-1.0.0/setup.py` & `pythoncolouringsliberyV1-1.1.0/setup.py`

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
     name="pythoncolouringsliberyV1",
     version=VERSION,
```

