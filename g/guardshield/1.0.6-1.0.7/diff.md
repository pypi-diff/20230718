# Comparing `tmp/guardshield-1.0.6.tar.gz` & `tmp/guardshield-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\guardshield-1.0.6.tar", last modified: Sat Jul  8 20:18:25 2023, max compression
+gzip compressed data, was "dist\guardshield-1.0.7.tar", last modified: Tue Jul 18 01:13:01 2023, max compression
```

## Comparing `guardshield-1.0.6.tar` & `guardshield-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 20:18:25.054726 guardshield-1.0.6/
--rw-rw-rw-   0        0        0     1061 2023-05-18 23:20:40.000000 guardshield-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     2681 2023-07-08 20:18:25.053763 guardshield-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2323 2023-05-19 17:02:01.000000 guardshield-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 20:18:25.038768 guardshield-1.0.6/guardshield/
--rw-rw-rw-   0        0        0       89 2023-06-02 21:51:47.000000 guardshield-1.0.6/guardshield/__init__.py
--rw-rw-rw-   0        0        0    58627 2023-07-08 20:13:23.000000 guardshield-1.0.6/guardshield/dll_bytes.py
--rw-rw-rw-   0        0        0     2285 2023-07-08 20:15:56.000000 guardshield-1.0.6/guardshield/main.py
-drwxrwxrwx   0        0        0        0 2023-07-08 20:18:25.051762 guardshield-1.0.6/guardshield.egg-info/
--rw-rw-rw-   0        0        0     2681 2023-07-08 20:18:24.000000 guardshield-1.0.6/guardshield.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-08 20:18:24.000000 guardshield-1.0.6/guardshield.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 20:18:24.000000 guardshield-1.0.6/guardshield.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-08 20:18:24.000000 guardshield-1.0.6/guardshield.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-07-08 20:18:24.000000 guardshield-1.0.6/guardshield.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 20:18:25.055723 guardshield-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      585 2023-07-08 20:16:01.000000 guardshield-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:13:01.020463 guardshield-1.0.7/
+-rw-rw-rw-   0        0        0     1061 2023-05-18 23:20:40.000000 guardshield-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4891 2023-07-18 01:13:01.019466 guardshield-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4464 2023-07-08 20:22:14.000000 guardshield-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 01:13:01.011487 guardshield-1.0.7/guardshield/
+-rw-rw-rw-   0        0        0       89 2023-06-02 21:51:47.000000 guardshield-1.0.7/guardshield/__init__.py
+-rw-rw-rw-   0        0        0    58627 2023-07-08 20:13:23.000000 guardshield-1.0.7/guardshield/dll_bytes.py
+-rw-rw-rw-   0        0        0     3473 2023-07-18 01:11:22.000000 guardshield-1.0.7/guardshield/main.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:13:01.018469 guardshield-1.0.7/guardshield.egg-info/
+-rw-rw-rw-   0        0        0     4891 2023-07-18 01:13:00.000000 guardshield-1.0.7/guardshield.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-07-18 01:13:00.000000 guardshield-1.0.7/guardshield.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 01:13:00.000000 guardshield-1.0.7/guardshield.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 01:13:00.000000 guardshield-1.0.7/guardshield.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-07-18 01:13:00.000000 guardshield-1.0.7/guardshield.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 01:13:01.021460 guardshield-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      585 2023-07-18 01:12:43.000000 guardshield-1.0.7/setup.py
```

### Comparing `guardshield-1.0.6/LICENSE` & `guardshield-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `guardshield-1.0.6/guardshield/dll_bytes.py` & `guardshield-1.0.7/guardshield/dll_bytes.py`

 * *Files identical despite different names*

### Comparing `guardshield-1.0.6/setup.py` & `guardshield-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name="guardshield",
-    version="1.0.6",
+    version="1.0.7",
     author="Oxyn",
     author_email="oxyn.dev@gmail.com",
     description="Security lib",
     keywords = "python anti debugger security exe",
     packages=setuptools.find_packages(),
     include_package_data=True,
     url='https://github.com/OxynDev/ExcerSec',
```

