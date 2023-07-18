# Comparing `tmp/pkgNipun-0.0.1.tar.gz` & `tmp/pkgNipun-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgNipun-0.0.1.tar", last modified: Fri Jul 14 12:56:00 2023, max compression
+gzip compressed data, was "pkgNipun-1.1.0.tar", last modified: Tue Jul 18 15:58:46 2023, max compression
```

## Comparing `pkgNipun-0.0.1.tar` & `pkgNipun-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 12:56:00.476952 pkgNipun-0.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)     1066 2023-07-14 10:08:16.000000 pkgNipun-0.0.1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)      335 2023-07-14 12:56:00.476952 pkgNipun-0.0.1/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 12:56:00.476952 pkgNipun-0.0.1/pkgNipun/
--rw-rw-r--   0 user      (1000) user      (1000)      621 2023-07-14 12:39:18.000000 pkgNipun-0.0.1/pkgNipun/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-14 12:56:00.476952 pkgNipun-0.0.1/pkgNipun.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      335 2023-07-14 12:56:00.000000 pkgNipun-0.0.1/pkgNipun.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      169 2023-07-14 12:56:00.000000 pkgNipun-0.0.1/pkgNipun.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-14 12:56:00.000000 pkgNipun-0.0.1/pkgNipun.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       21 2023-07-14 12:56:00.000000 pkgNipun-0.0.1/pkgNipun.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-14 12:56:00.476952 pkgNipun-0.0.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      957 2023-07-14 12:55:29.000000 pkgNipun-0.0.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-18 15:58:46.228964 pkgNipun-1.1.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1066 2023-07-14 10:08:16.000000 pkgNipun-1.1.0/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      335 2023-07-18 15:58:46.228964 pkgNipun-1.1.0/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-18 15:58:46.224964 pkgNipun-1.1.0/pkgNipun/
+-rw-rw-r--   0 user      (1000) user      (1000)     1032 2023-07-18 15:51:41.000000 pkgNipun-1.1.0/pkgNipun/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-18 15:58:46.228964 pkgNipun-1.1.0/pkgNipun.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      335 2023-07-18 15:58:45.000000 pkgNipun-1.1.0/pkgNipun.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      169 2023-07-18 15:58:45.000000 pkgNipun-1.1.0/pkgNipun.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-18 15:58:45.000000 pkgNipun-1.1.0/pkgNipun.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       21 2023-07-18 15:58:45.000000 pkgNipun-1.1.0/pkgNipun.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-18 15:58:46.228964 pkgNipun-1.1.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      957 2023-07-18 10:41:52.000000 pkgNipun-1.1.0/setup.py
```

### Comparing `pkgNipun-0.0.1/LICENSE.txt` & `pkgNipun-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkgNipun-0.0.1/setup.py` & `pkgNipun-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="pkgNipun",                     # This is the name of the package
-    version="0.0.1",                        # The initial release version
+    version="1.1.0",                        # The initial release version
     author="Nipun Dogra",                     # Full name of the author
     description="sample description",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

