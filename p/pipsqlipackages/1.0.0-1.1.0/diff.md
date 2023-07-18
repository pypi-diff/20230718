# Comparing `tmp/pipsqlipackages-1.0.0.tar.gz` & `tmp/pipsqlipackages-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlipackages-1.0.0.tar", last modified: Tue Jul 18 13:21:59 2023, max compression
+gzip compressed data, was "pipsqlipackages-1.1.0.tar", last modified: Tue Jul 18 13:24:04 2023, max compression
```

## Comparing `pipsqlipackages-1.0.0.tar` & `pipsqlipackages-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:21:59.458065 pipsqlipackages-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-18 13:21:59.454065 pipsqlipackages-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:21:59.454065 pipsqlipackages-1.0.0/pipsqlipackages/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 13:21:58.000000 pipsqlipackages-1.0.0/pipsqlipackages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:21:59.454065 pipsqlipackages-1.0.0/pipsqlipackages.egg-info/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-18 13:21:59.000000 pipsqlipackages-1.0.0/pipsqlipackages.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-18 13:21:59.000000 pipsqlipackages-1.0.0/pipsqlipackages.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 13:21:59.000000 pipsqlipackages-1.0.0/pipsqlipackages.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-18 13:21:59.000000 pipsqlipackages-1.0.0/pipsqlipackages.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 13:21:59.458065 pipsqlipackages-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      561 2023-07-18 13:21:58.000000 pipsqlipackages-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:24:04.613649 pipsqlipackages-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-18 13:24:04.613649 pipsqlipackages-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:24:04.613649 pipsqlipackages-1.1.0/pipsqlipackages/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-18 13:24:04.000000 pipsqlipackages-1.1.0/pipsqlipackages/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 13:24:04.613649 pipsqlipackages-1.1.0/pipsqlipackages.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-18 13:24:04.000000 pipsqlipackages-1.1.0/pipsqlipackages.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-18 13:24:04.000000 pipsqlipackages-1.1.0/pipsqlipackages.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 13:24:04.000000 pipsqlipackages-1.1.0/pipsqlipackages.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-18 13:24:04.000000 pipsqlipackages-1.1.0/pipsqlipackages.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 13:24:04.613649 pipsqlipackages-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      561 2023-07-18 13:24:04.000000 pipsqlipackages-1.1.0/setup.py
```

### Comparing `pipsqlipackages-1.0.0/setup.py` & `pipsqlipackages-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipsqlipackages",
     version=VERSION,
```

