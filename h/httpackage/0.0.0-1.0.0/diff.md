# Comparing `tmp/httpackage-0.0.0.tar.gz` & `tmp/httpackage-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpackage-0.0.0.tar", last modified: Tue Jul 18 01:49:45 2023, max compression
+gzip compressed data, was "httpackage-1.0.0.tar", last modified: Tue Jul 18 02:00:44 2023, max compression
```

## Comparing `httpackage-0.0.0.tar` & `httpackage-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 01:49:45.650000 httpackage-0.0.0/
--rw-rw-rw-   0        0        0     1944 2023-07-18 01:46:21.000000 httpackage-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      411 2023-07-18 01:49:45.647001 httpackage-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 01:49:45.613004 httpackage-0.0.0/httpackage/
--rw-rw-rw-   0        0        0        0 2023-07-17 23:52:32.000000 httpackage-0.0.0/httpackage/__init__.py
--rw-rw-rw-   0        0        0      917 2023-07-18 01:06:22.000000 httpackage-0.0.0/httpackage/httpackage.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:49:45.642997 httpackage-0.0.0/httpackage.egg-info/
--rw-rw-rw-   0        0        0      411 2023-07-18 01:49:45.000000 httpackage-0.0.0/httpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-18 01:49:45.000000 httpackage-0.0.0/httpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 01:49:45.000000 httpackage-0.0.0/httpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-18 01:49:45.000000 httpackage-0.0.0/httpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 01:49:45.650998 httpackage-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-07-18 01:47:41.000000 httpackage-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:00:44.548868 httpackage-1.0.0/
+-rw-rw-rw-   0        0        0     1944 2023-07-18 01:46:21.000000 httpackage-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3928 2023-07-18 02:00:44.544865 httpackage-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 02:00:44.510863 httpackage-1.0.0/httpackage/
+-rw-rw-rw-   0        0        0        0 2023-07-17 23:52:32.000000 httpackage-1.0.0/httpackage/__init__.py
+-rw-rw-rw-   0        0        0      917 2023-07-18 01:06:22.000000 httpackage-1.0.0/httpackage/httpackage.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:00:44.540866 httpackage-1.0.0/httpackage.egg-info/
+-rw-rw-rw-   0        0        0     3928 2023-07-18 02:00:44.000000 httpackage-1.0.0/httpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-18 02:00:44.000000 httpackage-1.0.0/httpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:00:44.000000 httpackage-1.0.0/httpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-18 02:00:44.000000 httpackage-1.0.0/httpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 02:00:44.549874 httpackage-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      628 2023-07-18 02:00:13.000000 httpackage-1.0.0/setup.py
```

### Comparing `httpackage-0.0.0/LICENSE` & `httpackage-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpackage-0.0.0/httpackage/httpackage.py` & `httpackage-1.0.0/httpackage/httpackage.py`

 * *Files identical despite different names*

### Comparing `httpackage-0.0.0/setup.py` & `httpackage-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("quas.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="httpackage",
-    version="0.0.0",
+    version="1.0.0",
     author="PyModuleDev",
     author_email="pxcom@mail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["httpackage"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

