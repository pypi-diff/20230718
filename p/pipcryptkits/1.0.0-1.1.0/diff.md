# Comparing `tmp/pipcryptkits-1.0.0.tar.gz` & `tmp/pipcryptkits-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptkits-1.0.0.tar", last modified: Tue Jul 18 00:55:42 2023, max compression
+gzip compressed data, was "pipcryptkits-1.1.0.tar", last modified: Tue Jul 18 00:57:47 2023, max compression
```

## Comparing `pipcryptkits-1.0.0.tar` & `pipcryptkits-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:55:42.648889 pipcryptkits-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-18 00:55:42.648889 pipcryptkits-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:55:42.648889 pipcryptkits-1.0.0/pipcryptkits/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 00:55:42.000000 pipcryptkits-1.0.0/pipcryptkits/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:55:42.648889 pipcryptkits-1.0.0/pipcryptkits.egg-info/
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-18 00:55:42.000000 pipcryptkits-1.0.0/pipcryptkits.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      177 2023-07-18 00:55:42.000000 pipcryptkits-1.0.0/pipcryptkits.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:55:42.000000 pipcryptkits-1.0.0/pipcryptkits.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:55:42.000000 pipcryptkits-1.0.0/pipcryptkits.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 00:55:42.648889 pipcryptkits-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-07-18 00:55:42.000000 pipcryptkits-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:57:47.664457 pipcryptkits-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-18 00:57:47.664457 pipcryptkits-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:57:47.660457 pipcryptkits-1.1.0/pipcryptkits/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-18 00:57:47.000000 pipcryptkits-1.1.0/pipcryptkits/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:57:47.664457 pipcryptkits-1.1.0/pipcryptkits.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-18 00:57:47.000000 pipcryptkits-1.1.0/pipcryptkits.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      177 2023-07-18 00:57:47.000000 pipcryptkits-1.1.0/pipcryptkits.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:57:47.000000 pipcryptkits-1.1.0/pipcryptkits.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:57:47.000000 pipcryptkits-1.1.0/pipcryptkits.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 00:57:47.664457 pipcryptkits-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-18 00:57:47.000000 pipcryptkits-1.1.0/setup.py
```

### Comparing `pipcryptkits-1.0.0/setup.py` & `pipcryptkits-1.1.0/setup.py`

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
     name="pipcryptkits",
     version=VERSION,
```

