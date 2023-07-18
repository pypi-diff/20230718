# Comparing `tmp/ravityemaillib-0.1.1.2.tar.gz` & `tmp/ravityemaillib-0.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ravityemaillib-0.1.1.2.tar", last modified: Tue Jul 18 10:20:59 2023, max compression
+gzip compressed data, was "ravityemaillib-0.1.1.3.tar", last modified: Tue Jul 18 10:25:43 2023, max compression
```

## Comparing `ravityemaillib-0.1.1.2.tar` & `ravityemaillib-0.1.1.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 10:20:59.286060 ravityemaillib-0.1.1.2/
--rw-rw-rw-   0        0        0      175 2023-07-18 10:20:59.285060 ravityemaillib-0.1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 10:20:59.252009 ravityemaillib-0.1.1.2/ravityemaillib/
--rw-rw-rw-   0        0        0        0 2023-07-18 07:59:36.000000 ravityemaillib-0.1.1.2/ravityemaillib/__init__.py
--rw-rw-rw-   0        0        0     1854 2023-07-18 10:09:12.000000 ravityemaillib-0.1.1.2/ravityemaillib/emaillib.py
-drwxrwxrwx   0        0        0        0 2023-07-18 10:20:59.283057 ravityemaillib-0.1.1.2/ravityemaillib.egg-info/
--rw-rw-rw-   0        0        0      175 2023-07-18 10:20:59.000000 ravityemaillib-0.1.1.2/ravityemaillib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-18 10:20:59.000000 ravityemaillib-0.1.1.2/ravityemaillib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 10:20:59.000000 ravityemaillib-0.1.1.2/ravityemaillib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-18 10:20:59.000000 ravityemaillib-0.1.1.2/ravityemaillib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-18 10:20:59.000000 ravityemaillib-0.1.1.2/ravityemaillib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 10:20:59.286060 ravityemaillib-0.1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-07-18 10:20:53.000000 ravityemaillib-0.1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:25:43.365473 ravityemaillib-0.1.1.3/
+-rw-rw-rw-   0        0        0      175 2023-07-18 10:25:43.364473 ravityemaillib-0.1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 10:25:43.342816 ravityemaillib-0.1.1.3/ravityemaillib/
+-rw-rw-rw-   0        0        0        0 2023-07-18 07:59:36.000000 ravityemaillib-0.1.1.3/ravityemaillib/__init__.py
+-rw-rw-rw-   0        0        0     1854 2023-07-18 10:09:12.000000 ravityemaillib-0.1.1.3/ravityemaillib/emaillib.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:25:43.361960 ravityemaillib-0.1.1.3/ravityemaillib.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-07-18 10:25:43.000000 ravityemaillib-0.1.1.3/ravityemaillib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-07-18 10:25:43.000000 ravityemaillib-0.1.1.3/ravityemaillib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:25:43.000000 ravityemaillib-0.1.1.3/ravityemaillib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-18 10:25:43.000000 ravityemaillib-0.1.1.3/ravityemaillib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:25:43.366473 ravityemaillib-0.1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      219 2023-07-18 10:25:34.000000 ravityemaillib-0.1.1.3/setup.py
```

### Comparing `ravityemaillib-0.1.1.2/ravityemaillib/emaillib.py` & `ravityemaillib-0.1.1.3/ravityemaillib/emaillib.py`

 * *Files identical despite different names*

