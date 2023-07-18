# Comparing `tmp/lavapayments-1.0.2.tar.gz` & `tmp/lavapayments-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavapayments-1.0.2.tar", last modified: Tue Jul 18 13:46:38 2023, max compression
+gzip compressed data, was "lavapayments-1.0.3.tar", last modified: Tue Jul 18 17:18:46 2023, max compression
```

## Comparing `lavapayments-1.0.2.tar` & `lavapayments-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 13:46:38.469788 lavapayments-1.0.2/
--rw-rw-rw-   0        0        0     1189 2023-07-18 13:46:38.468594 lavapayments-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 13:46:38.468594 lavapayments-1.0.2/lavapayments.egg-info/
--rw-rw-rw-   0        0        0     1189 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 13:46:38.469788 lavapayments-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-18 13:45:59.000000 lavapayments-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:18:46.656719 lavapayments-1.0.3/
+-rw-rw-rw-   0        0        0      260 2023-07-18 17:18:46.656719 lavapayments-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 17:18:46.655722 lavapayments-1.0.3/lavapayments.egg-info/
+-rw-rw-rw-   0        0        0      260 2023-07-18 17:18:46.000000 lavapayments-1.0.3/lavapayments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-18 17:18:46.000000 lavapayments-1.0.3/lavapayments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:18:46.000000 lavapayments-1.0.3/lavapayments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 13:46:38.000000 lavapayments-1.0.3/lavapayments.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-07-18 17:18:46.000000 lavapayments-1.0.3/lavapayments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:18:46.657716 lavapayments-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      385 2023-07-18 17:18:26.000000 lavapayments-1.0.3/setup.py
```

