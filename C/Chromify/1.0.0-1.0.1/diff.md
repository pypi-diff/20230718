# Comparing `tmp/Chromify-1.0.0.tar.gz` & `tmp/Chromify-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chromify-1.0.0.tar", last modified: Tue Jul 18 11:09:11 2023, max compression
+gzip compressed data, was "Chromify-1.0.1.tar", last modified: Tue Jul 18 11:28:55 2023, max compression
```

## Comparing `Chromify-1.0.0.tar` & `Chromify-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 11:09:11.186414 Chromify-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-18 11:09:11.175988 Chromify-1.0.0/Chromify.egg-info/
--rw-rw-rw-   0        0        0      448 2023-07-18 11:09:11.000000 Chromify-1.0.0/Chromify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-07-18 11:09:11.000000 Chromify-1.0.0/Chromify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 11:09:11.000000 Chromify-1.0.0/Chromify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-18 11:09:11.000000 Chromify-1.0.0/Chromify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      448 2023-07-18 11:09:11.185414 Chromify-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 11:09:11.183414 Chromify-1.0.0/lib/
--rw-rw-rw-   0        0        0     6542 2023-07-18 10:22:00.000000 Chromify-1.0.0/lib/Chromify.py
--rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.0.0/lib/Color.py
--rw-rw-rw-   0        0        0     7865 2023-07-18 10:07:14.000000 Chromify-1.0.0/lib/Converter.py
--rw-rw-rw-   0        0        0      148 2023-07-17 23:22:11.000000 Chromify-1.0.0/lib/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-18 11:09:11.186414 Chromify-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-07-17 23:48:34.000000 Chromify-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:28:55.057359 Chromify-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-07-18 11:28:55.036574 Chromify-1.0.1/Chromify.egg-info/
+-rw-rw-rw-   0        0        0     5118 2023-07-18 11:28:54.000000 Chromify-1.0.1/Chromify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-07-18 11:28:54.000000 Chromify-1.0.1/Chromify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 11:28:54.000000 Chromify-1.0.1/Chromify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-18 11:28:54.000000 Chromify-1.0.1/Chromify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5118 2023-07-18 11:28:55.055226 Chromify-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 11:28:55.048153 Chromify-1.0.1/lib/
+-rw-rw-rw-   0        0        0     6542 2023-07-18 10:22:00.000000 Chromify-1.0.1/lib/Chromify.py
+-rw-rw-rw-   0        0        0    16090 2023-07-17 14:20:45.000000 Chromify-1.0.1/lib/Color.py
+-rw-rw-rw-   0        0        0     7865 2023-07-18 10:07:14.000000 Chromify-1.0.1/lib/Converter.py
+-rw-rw-rw-   0        0        0      148 2023-07-18 11:28:38.000000 Chromify-1.0.1/lib/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-18 11:28:55.058357 Chromify-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-07-18 11:28:16.000000 Chromify-1.0.1/setup.py
```

### Comparing `Chromify-1.0.0/lib/Chromify.py` & `Chromify-1.0.1/lib/Chromify.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.0/lib/Color.py` & `Chromify-1.0.1/lib/Color.py`

 * *Files identical despite different names*

### Comparing `Chromify-1.0.0/lib/Converter.py` & `Chromify-1.0.1/lib/Converter.py`

 * *Files identical despite different names*

