# Comparing `tmp/pycryptographypackageV1-1.0.0.tar.gz` & `tmp/pycryptographypackageV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptographypackageV1-1.0.0.tar", last modified: Tue Jul 18 13:18:54 2023, max compression
+gzip compressed data, was "pycryptographypackageV1-1.1.0.tar", last modified: Tue Jul 18 13:21:00 2023, max compression
```

## Comparing `pycryptographypackageV1-1.0.0.tar` & `pycryptographypackageV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:18:54.810675 pycryptographypackageV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      356 2023-07-18 13:18:54.810675 pycryptographypackageV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:18:54.806675 pycryptographypackageV1-1.0.0/pycryptographypackageV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 13:18:54.000000 pycryptographypackageV1-1.0.0/pycryptographypackageV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:18:54.810675 pycryptographypackageV1-1.0.0/pycryptographypackageV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      356 2023-07-18 13:18:54.000000 pycryptographypackageV1-1.0.0/pycryptographypackageV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2023-07-18 13:18:54.000000 pycryptographypackageV1-1.0.0/pycryptographypackageV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 13:18:54.000000 pycryptographypackageV1-1.0.0/pycryptographypackageV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-18 13:18:54.000000 pycryptographypackageV1-1.0.0/pycryptographypackageV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 13:18:54.810675 pycryptographypackageV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      569 2023-07-18 13:18:54.000000 pycryptographypackageV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:21:00.234262 pycryptographypackageV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-18 13:21:00.234262 pycryptographypackageV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:21:00.230262 pycryptographypackageV1-1.1.0/pycryptographypackageV1/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-18 13:20:59.000000 pycryptographypackageV1-1.1.0/pycryptographypackageV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:21:00.234262 pycryptographypackageV1-1.1.0/pycryptographypackageV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-18 13:21:00.000000 pycryptographypackageV1-1.1.0/pycryptographypackageV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2023-07-18 13:21:00.000000 pycryptographypackageV1-1.1.0/pycryptographypackageV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 13:21:00.000000 pycryptographypackageV1-1.1.0/pycryptographypackageV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-18 13:21:00.000000 pycryptographypackageV1-1.1.0/pycryptographypackageV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 13:21:00.234262 pycryptographypackageV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      569 2023-07-18 13:20:59.000000 pycryptographypackageV1-1.1.0/setup.py
```

### Comparing `pycryptographypackageV1-1.0.0/setup.py` & `pycryptographypackageV1-1.1.0/setup.py`

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
     name="pycryptographypackageV1",
     version=VERSION,
```

