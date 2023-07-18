# Comparing `tmp/QRcodeTracking-0.1.4.tar.gz` & `tmp/QRcodeTracking-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QRcodeTracking-0.1.4.tar", last modified: Fri Jul 14 07:43:17 2023, max compression
+gzip compressed data, was "QRcodeTracking-0.1.5.tar", last modified: Tue Jul 18 09:45:32 2023, max compression
```

## Comparing `QRcodeTracking-0.1.4.tar` & `QRcodeTracking-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:43:17.311180 QRcodeTracking-0.1.4/
--rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 QRcodeTracking-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 QRcodeTracking-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      373 2023-07-14 07:43:17.312201 QRcodeTracking-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 07:43:17.291171 QRcodeTracking-0.1.4/QRcodeTracking/
--rw-rw-rw-   0        0        0    76800 2023-07-14 07:41:54.000000 QRcodeTracking-0.1.4/QRcodeTracking/QR_codefunction.pyd
--rw-rw-rw-   0        0        0   115712 2023-07-14 07:41:45.000000 QRcodeTracking-0.1.4/QRcodeTracking/QRcodeTracking.pyd
--rw-rw-rw-   0        0        0        0 2023-07-13 02:44:59.000000 QRcodeTracking-0.1.4/QRcodeTracking/__init__.py
--rw-rw-rw-   0        0        0    64000 2023-07-14 07:41:35.000000 QRcodeTracking-0.1.4/QRcodeTracking/erwewima_ui.pyd
-drwxrwxrwx   0        0        0        0 2023-07-14 07:43:17.308175 QRcodeTracking-0.1.4/QRcodeTracking.egg-info/
--rw-rw-rw-   0        0        0      373 2023-07-14 07:43:17.000000 QRcodeTracking-0.1.4/QRcodeTracking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-07-14 07:43:17.000000 QRcodeTracking-0.1.4/QRcodeTracking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:43:17.000000 QRcodeTracking-0.1.4/QRcodeTracking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-14 07:43:17.000000 QRcodeTracking-0.1.4/QRcodeTracking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       15 2023-07-14 03:40:50.000000 QRcodeTracking-0.1.4/README.md
--rw-rw-rw-   0        0        0      136 2023-07-14 07:43:17.314176 QRcodeTracking-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1006 2023-07-14 07:42:58.000000 QRcodeTracking-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 09:45:32.311054 QRcodeTracking-0.1.5/
+-rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 QRcodeTracking-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 QRcodeTracking-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      373 2023-07-18 09:45:32.311054 QRcodeTracking-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 09:45:32.297054 QRcodeTracking-0.1.5/QRcodeTracking/
+-rw-rw-rw-   0        0        0    76800 2023-07-14 07:41:54.000000 QRcodeTracking-0.1.5/QRcodeTracking/QR_codefunction.pyd
+-rw-rw-rw-   0        0        0   115712 2023-07-18 09:44:27.000000 QRcodeTracking-0.1.5/QRcodeTracking/QRcodeTracking.pyd
+-rw-rw-rw-   0        0        0        0 2023-07-13 02:44:59.000000 QRcodeTracking-0.1.5/QRcodeTracking/__init__.py
+-rw-rw-rw-   0        0        0    64000 2023-07-14 07:41:35.000000 QRcodeTracking-0.1.5/QRcodeTracking/erwewima_ui.pyd
+drwxrwxrwx   0        0        0        0 2023-07-18 09:45:32.309054 QRcodeTracking-0.1.5/QRcodeTracking.egg-info/
+-rw-rw-rw-   0        0        0      373 2023-07-18 09:45:32.000000 QRcodeTracking-0.1.5/QRcodeTracking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-07-18 09:45:32.000000 QRcodeTracking-0.1.5/QRcodeTracking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 09:45:32.000000 QRcodeTracking-0.1.5/QRcodeTracking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-18 09:45:32.000000 QRcodeTracking-0.1.5/QRcodeTracking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       15 2023-07-14 03:40:50.000000 QRcodeTracking-0.1.5/README.md
+-rw-rw-rw-   0        0        0      136 2023-07-18 09:45:32.313055 QRcodeTracking-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2023-07-18 09:45:26.000000 QRcodeTracking-0.1.5/setup.py
```

### Comparing `QRcodeTracking-0.1.4/setup.py` & `QRcodeTracking-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 4
+PATCH = 5
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "QRcodeTracking",
```

