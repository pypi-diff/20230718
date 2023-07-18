# Comparing `tmp/tested_package-0.0.1.tar.gz` & `tmp/tested_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tested_package-0.0.1.tar", last modified: Tue Jul 18 14:14:49 2023, max compression
+gzip compressed data, was "tested_package-0.0.2.tar", last modified: Tue Jul 18 14:22:01 2023, max compression
```

## Comparing `tested_package-0.0.1.tar` & `tested_package-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 14:14:49.590321 tested_package-0.0.1/
--rw-rw-rw-   0        0        0      455 2023-07-18 14:14:49.589329 tested_package-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 14:14:49.590321 tested_package-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      882 2023-07-18 14:13:33.000000 tested_package-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:14:49.586335 tested_package-0.0.1/tested_package/
--rw-rw-rw-   0        0        0        0 2023-07-18 14:11:06.000000 tested_package-0.0.1/tested_package/__init__.py
--rw-rw-rw-   0        0        0       60 2023-07-18 14:12:18.000000 tested_package-0.0.1/tested_package/fileA.py
--rw-rw-rw-   0        0        0       60 2023-07-18 14:12:18.000000 tested_package-0.0.1/tested_package/fileB.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:14:49.588329 tested_package-0.0.1/tested_package.egg-info/
--rw-rw-rw-   0        0        0      455 2023-07-18 14:14:49.000000 tested_package-0.0.1/tested_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-18 14:14:49.000000 tested_package-0.0.1/tested_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 14:14:49.000000 tested_package-0.0.1/tested_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-18 14:14:49.000000 tested_package-0.0.1/tested_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 14:22:01.778665 tested_package-0.0.2/
+-rw-rw-rw-   0        0        0      455 2023-07-18 14:22:01.777675 tested_package-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 14:22:01.778665 tested_package-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      882 2023-07-18 14:21:57.000000 tested_package-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:22:01.774682 tested_package-0.0.2/tested_package/
+-rw-rw-rw-   0        0        0       40 2023-07-18 14:21:50.000000 tested_package-0.0.2/tested_package/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-07-18 14:12:18.000000 tested_package-0.0.2/tested_package/fileA.py
+-rw-rw-rw-   0        0        0       60 2023-07-18 14:12:18.000000 tested_package-0.0.2/tested_package/fileB.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:22:01.777675 tested_package-0.0.2/tested_package.egg-info/
+-rw-rw-rw-   0        0        0      455 2023-07-18 14:22:01.000000 tested_package-0.0.2/tested_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-18 14:22:01.000000 tested_package-0.0.2/tested_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 14:22:01.000000 tested_package-0.0.2/tested_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-18 14:22:01.000000 tested_package-0.0.2/tested_package.egg-info/top_level.txt
```

### Comparing `tested_package-0.0.1/setup.py` & `tested_package-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Package for testing'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     # the name must match the folder name 'LatticeGeometryLib'
     name="tested_package",
```

