# Comparing `tmp/ravityemaillib-0.1.1.0.tar.gz` & `tmp/ravityemaillib-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ravityemaillib-0.1.1.0.tar", last modified: Tue Jul 18 08:04:04 2023, max compression
+gzip compressed data, was "ravityemaillib-0.1.1.1.tar", last modified: Tue Jul 18 10:14:37 2023, max compression
```

## Comparing `ravityemaillib-0.1.1.0.tar` & `ravityemaillib-0.1.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 08:04:04.393993 ravityemaillib-0.1.1.0/
--rw-rw-rw-   0        0        0      175 2023-07-18 08:04:04.392991 ravityemaillib-0.1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 08:04:04.382193 ravityemaillib-0.1.1.0/ravityemaillib/
--rw-rw-rw-   0        0        0        0 2023-07-18 07:59:36.000000 ravityemaillib-0.1.1.0/ravityemaillib/__init__.py
--rw-rw-rw-   0        0        0       39 2023-07-18 06:46:02.000000 ravityemaillib-0.1.1.0/ravityemaillib/emaillib.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:04:04.392488 ravityemaillib-0.1.1.0/ravityemaillib.egg-info/
--rw-rw-rw-   0        0        0      175 2023-07-18 08:04:04.000000 ravityemaillib-0.1.1.0/ravityemaillib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-07-18 08:04:04.000000 ravityemaillib-0.1.1.0/ravityemaillib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 08:04:04.000000 ravityemaillib-0.1.1.0/ravityemaillib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-18 08:04:04.000000 ravityemaillib-0.1.1.0/ravityemaillib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 08:04:04.393993 ravityemaillib-0.1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      219 2023-07-18 08:03:56.000000 ravityemaillib-0.1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:14:37.266730 ravityemaillib-0.1.1.1/
+-rw-rw-rw-   0        0        0      175 2023-07-18 10:14:37.265255 ravityemaillib-0.1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 10:14:37.226244 ravityemaillib-0.1.1.1/ravityemaillib/
+-rw-rw-rw-   0        0        0        0 2023-07-18 07:59:36.000000 ravityemaillib-0.1.1.1/ravityemaillib/__init__.py
+-rw-rw-rw-   0        0        0     1854 2023-07-18 10:09:12.000000 ravityemaillib-0.1.1.1/ravityemaillib/emaillib.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:14:37.263255 ravityemaillib-0.1.1.1/ravityemaillib.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-07-18 10:14:37.000000 ravityemaillib-0.1.1.1/ravityemaillib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-18 10:14:37.000000 ravityemaillib-0.1.1.1/ravityemaillib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:14:37.000000 ravityemaillib-0.1.1.1/ravityemaillib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-18 10:14:37.000000 ravityemaillib-0.1.1.1/ravityemaillib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-18 10:14:37.000000 ravityemaillib-0.1.1.1/ravityemaillib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:14:37.266730 ravityemaillib-0.1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      272 2023-07-18 10:14:04.000000 ravityemaillib-0.1.1.1/setup.py
```

