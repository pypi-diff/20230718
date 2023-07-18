# Comparing `tmp/ExtractEmailAttachments-0.1.2.tar.gz` & `tmp/ExtractEmailAttachments-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExtractEmailAttachments-0.1.2.tar", last modified: Wed Jul 12 06:23:56 2023, max compression
+gzip compressed data, was "ExtractEmailAttachments-0.1.3.tar", last modified: Tue Jul 18 08:41:26 2023, max compression
```

## Comparing `ExtractEmailAttachments-0.1.2.tar` & `ExtractEmailAttachments-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 06:23:56.361085 ExtractEmailAttachments-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-12 06:23:56.338084 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments/
--rw-rw-rw-   0        0        0   106496 2023-07-12 06:21:41.000000 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments/ExtractEmailAttachments.pyd
--rw-rw-rw-   0        0        0        0 2023-07-12 01:20:14.000000 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments/__init__.py
--rw-rw-rw-   0        0        0    67072 2023-07-12 06:21:25.000000 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments/eml_demo.pyd
--rw-rw-rw-   0        0        0    49664 2023-07-12 06:21:33.000000 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments/eml_function.pyd
-drwxrwxrwx   0        0        0        0 2023-07-12 06:23:56.357088 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments.egg-info/
--rw-rw-rw-   0        0        0      418 2023-07-12 06:23:56.000000 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-07-12 06:23:56.000000 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 06:23:56.000000 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-12 06:23:56.000000 ExtractEmailAttachments-0.1.2/ExtractEmailAttachments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       21 2023-07-12 02:38:13.000000 ExtractEmailAttachments-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 ExtractEmailAttachments-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      418 2023-07-12 06:23:56.362076 ExtractEmailAttachments-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 ExtractEmailAttachments-0.1.2/README.md
--rw-rw-rw-   0        0        0      136 2023-07-12 06:23:56.365075 ExtractEmailAttachments-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1033 2023-07-12 06:23:28.000000 ExtractEmailAttachments-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:41:26.782018 ExtractEmailAttachments-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-18 08:41:26.767018 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments/
+-rw-rw-rw-   0        0        0   106496 2023-07-18 08:39:06.000000 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments/ExtractEmailAttachments.pyd
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:20:14.000000 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments/__init__.py
+-rw-rw-rw-   0        0        0    67072 2023-07-12 06:21:25.000000 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments/eml_demo.pyd
+-rw-rw-rw-   0        0        0    49664 2023-07-12 06:21:33.000000 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments/eml_function.pyd
+drwxrwxrwx   0        0        0        0 2023-07-18 08:41:26.780022 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-07-18 08:41:26.000000 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-07-18 08:41:26.000000 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:41:26.000000 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-18 08:41:26.000000 ExtractEmailAttachments-0.1.3/ExtractEmailAttachments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       21 2023-07-12 02:38:13.000000 ExtractEmailAttachments-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 ExtractEmailAttachments-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      418 2023-07-18 08:41:26.782018 ExtractEmailAttachments-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 ExtractEmailAttachments-0.1.3/README.md
+-rw-rw-rw-   0        0        0      136 2023-07-18 08:41:26.784019 ExtractEmailAttachments-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-07-18 08:41:00.000000 ExtractEmailAttachments-0.1.3/setup.py
```

### Comparing `ExtractEmailAttachments-0.1.2/setup.py` & `ExtractEmailAttachments-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 2
+PATCH = 3
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "ExtractEmailAttachments",
```

