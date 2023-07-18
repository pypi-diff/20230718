# Comparing `tmp/covert-ots-1.0.2.tar.gz` & `tmp/covert-ots-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covert-ots-1.0.2.tar", last modified: Tue Jul 18 05:05:25 2023, max compression
+gzip compressed data, was "covert-ots-1.0.3.tar", last modified: Tue Jul 18 05:08:10 2023, max compression
```

## Comparing `covert-ots-1.0.2.tar` & `covert-ots-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 05:05:25.000429 covert-ots-1.0.2/
--rw-rw-r--   0 om        (1001) om        (1001)      135 2023-07-18 05:05:25.000429 covert-ots-1.0.2/PKG-INFO
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 05:05:25.000429 covert-ots-1.0.2/covert_ots.egg-info/
--rw-rw-r--   0 om        (1001) om        (1001)      135 2023-07-18 05:05:24.000000 covert-ots-1.0.2/covert_ots.egg-info/PKG-INFO
--rw-rw-r--   0 om        (1001) om        (1001)      177 2023-07-18 05:05:24.000000 covert-ots-1.0.2/covert_ots.egg-info/SOURCES.txt
--rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 05:05:24.000000 covert-ots-1.0.2/covert_ots.egg-info/dependency_links.txt
--rw-rw-r--   0 om        (1001) om        (1001)       33 2023-07-18 05:05:24.000000 covert-ots-1.0.2/covert_ots.egg-info/requires.txt
--rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 05:05:24.000000 covert-ots-1.0.2/covert_ots.egg-info/top_level.txt
--rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-18 05:05:25.000429 covert-ots-1.0.2/setup.cfg
--rw-rw-r--   0 om        (1001) om        (1001)      218 2023-07-18 05:05:22.000000 covert-ots-1.0.2/setup.py
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 05:08:10.867042 covert-ots-1.0.3/
+-rw-rw-r--   0 om        (1001) om        (1001)      135 2023-07-18 05:08:10.867042 covert-ots-1.0.3/PKG-INFO
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 05:08:10.867042 covert-ots-1.0.3/covert_ots.egg-info/
+-rw-rw-r--   0 om        (1001) om        (1001)      135 2023-07-18 05:08:10.000000 covert-ots-1.0.3/covert_ots.egg-info/PKG-INFO
+-rw-rw-r--   0 om        (1001) om        (1001)      214 2023-07-18 05:08:10.000000 covert-ots-1.0.3/covert_ots.egg-info/SOURCES.txt
+-rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 05:08:10.000000 covert-ots-1.0.3/covert_ots.egg-info/dependency_links.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       62 2023-07-18 05:08:10.000000 covert-ots-1.0.3/covert_ots.egg-info/entry_points.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       33 2023-07-18 05:08:10.000000 covert-ots-1.0.3/covert_ots.egg-info/requires.txt
+-rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 05:08:10.000000 covert-ots-1.0.3/covert_ots.egg-info/top_level.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-18 05:08:10.867042 covert-ots-1.0.3/setup.cfg
+-rw-rw-r--   0 om        (1001) om        (1001)      305 2023-07-18 05:08:09.000000 covert-ots-1.0.3/setup.py
```

