# Comparing `tmp/pythonfontingadds-1.0.0.tar.gz` & `tmp/pythonfontingadds-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonfontingadds-1.0.0.tar", last modified: Tue Jul 18 12:46:24 2023, max compression
+gzip compressed data, was "pythonfontingadds-1.1.0.tar", last modified: Tue Jul 18 12:48:28 2023, max compression
```

## Comparing `pythonfontingadds-1.0.0.tar` & `pythonfontingadds-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:46:24.765568 pythonfontingadds-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-18 12:46:24.765568 pythonfontingadds-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:46:24.765568 pythonfontingadds-1.0.0/pythonfontingadds/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 12:46:24.000000 pythonfontingadds-1.0.0/pythonfontingadds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:46:24.765568 pythonfontingadds-1.0.0/pythonfontingadds.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-07-18 12:46:24.000000 pythonfontingadds-1.0.0/pythonfontingadds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-18 12:46:24.000000 pythonfontingadds-1.0.0/pythonfontingadds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 12:46:24.000000 pythonfontingadds-1.0.0/pythonfontingadds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-18 12:46:24.000000 pythonfontingadds-1.0.0/pythonfontingadds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 12:46:24.765568 pythonfontingadds-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-07-18 12:46:24.000000 pythonfontingadds-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:48:28.961068 pythonfontingadds-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-18 12:48:28.961068 pythonfontingadds-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:48:28.957068 pythonfontingadds-1.1.0/pythonfontingadds/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-18 12:48:28.000000 pythonfontingadds-1.1.0/pythonfontingadds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:48:28.961068 pythonfontingadds-1.1.0/pythonfontingadds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-18 12:48:28.000000 pythonfontingadds-1.1.0/pythonfontingadds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-18 12:48:28.000000 pythonfontingadds-1.1.0/pythonfontingadds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 12:48:28.000000 pythonfontingadds-1.1.0/pythonfontingadds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-18 12:48:28.000000 pythonfontingadds-1.1.0/pythonfontingadds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 12:48:28.961068 pythonfontingadds-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-07-18 12:48:28.000000 pythonfontingadds-1.1.0/setup.py
```

### Comparing `pythonfontingadds-1.0.0/setup.py` & `pythonfontingadds-1.1.0/setup.py`

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
     name="pythonfontingadds",
     version=VERSION,
```

