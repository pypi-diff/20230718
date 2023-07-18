# Comparing `tmp/pipsqladdV1-1.0.0.tar.gz` & `tmp/pipsqladdV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqladdV1-1.0.0.tar", last modified: Mon Jul 17 23:59:06 2023, max compression
+gzip compressed data, was "pipsqladdV1-1.1.0.tar", last modified: Tue Jul 18 00:01:12 2023, max compression
```

## Comparing `pipsqladdV1-1.0.0.tar` & `pipsqladdV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 23:59:06.944876 pipsqladdV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-17 23:59:06.944876 pipsqladdV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 23:59:06.940876 pipsqladdV1-1.0.0/pipsqladdV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 23:59:06.000000 pipsqladdV1-1.0.0/pipsqladdV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 23:59:06.944876 pipsqladdV1-1.0.0/pipsqladdV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-17 23:59:06.000000 pipsqladdV1-1.0.0/pipsqladdV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-17 23:59:06.000000 pipsqladdV1-1.0.0/pipsqladdV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 23:59:06.000000 pipsqladdV1-1.0.0/pipsqladdV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-17 23:59:06.000000 pipsqladdV1-1.0.0/pipsqladdV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 23:59:06.944876 pipsqladdV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      557 2023-07-17 23:59:06.000000 pipsqladdV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:01:12.752487 pipsqladdV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-18 00:01:12.752487 pipsqladdV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:01:12.752487 pipsqladdV1-1.1.0/pipsqladdV1/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-07-18 00:01:12.000000 pipsqladdV1-1.1.0/pipsqladdV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:01:12.752487 pipsqladdV1-1.1.0/pipsqladdV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-18 00:01:12.000000 pipsqladdV1-1.1.0/pipsqladdV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-18 00:01:12.000000 pipsqladdV1-1.1.0/pipsqladdV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:01:12.000000 pipsqladdV1-1.1.0/pipsqladdV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-18 00:01:12.000000 pipsqladdV1-1.1.0/pipsqladdV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 00:01:12.752487 pipsqladdV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      557 2023-07-18 00:01:12.000000 pipsqladdV1-1.1.0/setup.py
```

### Comparing `pipsqladdV1-1.0.0/setup.py` & `pipsqladdV1-1.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipsqladdV1",
     version=VERSION,
```

