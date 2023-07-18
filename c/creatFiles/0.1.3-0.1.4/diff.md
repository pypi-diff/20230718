# Comparing `tmp/creatFiles-0.1.3.tar.gz` & `tmp/creatFiles-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creatFiles-0.1.3.tar", last modified: Thu Jul 13 01:26:26 2023, max compression
+gzip compressed data, was "creatFiles-0.1.4.tar", last modified: Tue Jul 18 08:29:44 2023, max compression
```

## Comparing `creatFiles-0.1.3.tar` & `creatFiles-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 01:26:25.990639 creatFiles-0.1.3/
--rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 creatFiles-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 creatFiles-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      402 2023-07-13 01:26:25.990639 creatFiles-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-05 02:45:05.000000 creatFiles-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 01:26:25.969589 creatFiles-0.1.3/creatFiles/
--rw-rw-rw-   0        0        0        0 2023-02-28 07:01:01.000000 creatFiles-0.1.3/creatFiles/__init__.py
--rw-rw-rw-   0        0        0   122368 2023-07-13 01:14:01.000000 creatFiles-0.1.3/creatFiles/creatFiles.pyd
--rw-rw-rw-   0        0        0    54272 2023-07-06 02:12:32.000000 creatFiles-0.1.3/creatFiles/function_refer.pyd
--rw-rw-rw-   0        0        0    81920 2023-07-06 02:12:42.000000 creatFiles-0.1.3/creatFiles/function_refer_ui.pyd
-drwxrwxrwx   0        0        0        0 2023-07-13 01:26:25.986591 creatFiles-0.1.3/creatFiles.egg-info/
--rw-rw-rw-   0        0        0      402 2023-07-13 01:26:25.000000 creatFiles-0.1.3/creatFiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-07-13 01:26:25.000000 creatFiles-0.1.3/creatFiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 01:26:25.000000 creatFiles-0.1.3/creatFiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-13 01:26:25.000000 creatFiles-0.1.3/creatFiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-07-13 01:26:25.993589 creatFiles-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-13 01:25:52.000000 creatFiles-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:29:44.657740 creatFiles-0.1.4/
+-rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 creatFiles-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 creatFiles-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      402 2023-07-18 08:29:44.657740 creatFiles-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-05 02:45:05.000000 creatFiles-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 08:29:44.642742 creatFiles-0.1.4/creatFiles/
+-rw-rw-rw-   0        0        0        0 2023-02-28 07:01:01.000000 creatFiles-0.1.4/creatFiles/__init__.py
+-rw-rw-rw-   0        0        0   122368 2023-07-18 08:26:28.000000 creatFiles-0.1.4/creatFiles/creatFiles.pyd
+-rw-rw-rw-   0        0        0    54272 2023-07-06 02:12:32.000000 creatFiles-0.1.4/creatFiles/function_refer.pyd
+-rw-rw-rw-   0        0        0    81920 2023-07-06 02:12:42.000000 creatFiles-0.1.4/creatFiles/function_refer_ui.pyd
+drwxrwxrwx   0        0        0        0 2023-07-18 08:29:44.653817 creatFiles-0.1.4/creatFiles.egg-info/
+-rw-rw-rw-   0        0        0      402 2023-07-18 08:29:44.000000 creatFiles-0.1.4/creatFiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-07-18 08:29:44.000000 creatFiles-0.1.4/creatFiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:29:44.000000 creatFiles-0.1.4/creatFiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-18 08:29:44.000000 creatFiles-0.1.4/creatFiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-07-18 08:29:44.659742 creatFiles-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-18 08:28:29.000000 creatFiles-0.1.4/setup.py
```

### Comparing `creatFiles-0.1.3/setup.py` & `creatFiles-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 3
+PATCH = 4
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "creatFiles",
```

