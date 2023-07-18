# Comparing `tmp/covert-ots-1.0.tar.gz` & `tmp/covert-ots-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covert-ots-1.0.tar", last modified: Tue Jul 18 04:59:40 2023, max compression
+gzip compressed data, was "covert-ots-1.0.1.tar", last modified: Tue Jul 18 05:02:30 2023, max compression
```

## Comparing `covert-ots-1.0.tar` & `covert-ots-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 04:59:40.446370 covert-ots-1.0/
--rw-rw-r--   0 om        (1001) om        (1001)      133 2023-07-18 04:59:40.442371 covert-ots-1.0/PKG-INFO
-drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 04:59:40.442371 covert-ots-1.0/covert_ots.egg-info/
--rw-rw-r--   0 om        (1001) om        (1001)      133 2023-07-18 04:59:40.000000 covert-ots-1.0/covert_ots.egg-info/PKG-INFO
--rw-rw-r--   0 om        (1001) om        (1001)      177 2023-07-18 04:59:40.000000 covert-ots-1.0/covert_ots.egg-info/SOURCES.txt
--rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 04:59:40.000000 covert-ots-1.0/covert_ots.egg-info/dependency_links.txt
--rw-rw-r--   0 om        (1001) om        (1001)       40 2023-07-18 04:59:40.000000 covert-ots-1.0/covert_ots.egg-info/requires.txt
--rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 04:59:40.000000 covert-ots-1.0/covert_ots.egg-info/top_level.txt
--rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-18 04:59:40.446370 covert-ots-1.0/setup.cfg
--rw-rw-r--   0 om        (1001) om        (1001)      232 2023-07-18 04:58:52.000000 covert-ots-1.0/setup.py
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 05:02:30.294077 covert-ots-1.0.1/
+-rw-rw-r--   0 om        (1001) om        (1001)      135 2023-07-18 05:02:30.294077 covert-ots-1.0.1/PKG-INFO
+drwxrwxr-x   0 om        (1001) om        (1001)        0 2023-07-18 05:02:30.294077 covert-ots-1.0.1/covert_ots.egg-info/
+-rw-rw-r--   0 om        (1001) om        (1001)      135 2023-07-18 05:02:30.000000 covert-ots-1.0.1/covert_ots.egg-info/PKG-INFO
+-rw-rw-r--   0 om        (1001) om        (1001)      177 2023-07-18 05:02:30.000000 covert-ots-1.0.1/covert_ots.egg-info/SOURCES.txt
+-rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 05:02:30.000000 covert-ots-1.0.1/covert_ots.egg-info/dependency_links.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       33 2023-07-18 05:02:30.000000 covert-ots-1.0.1/covert_ots.egg-info/requires.txt
+-rw-rw-r--   0 om        (1001) om        (1001)        1 2023-07-18 05:02:30.000000 covert-ots-1.0.1/covert_ots.egg-info/top_level.txt
+-rw-rw-r--   0 om        (1001) om        (1001)       38 2023-07-18 05:02:30.294077 covert-ots-1.0.1/setup.cfg
+-rw-rw-r--   0 om        (1001) om        (1001)      218 2023-07-18 05:02:23.000000 covert-ots-1.0.1/setup.py
```

