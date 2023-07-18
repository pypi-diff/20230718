# Comparing `tmp/real-brasileiro-0.2.1.tar.gz` & `tmp/real-brasileiro-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real-brasileiro-0.2.1.tar", last modified: Tue Jul 18 03:46:00 2023, max compression
+gzip compressed data, was "real-brasileiro-0.2.5.tar", last modified: Tue Jul 18 03:56:51 2023, max compression
```

## Comparing `real-brasileiro-0.2.1.tar` & `real-brasileiro-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:46:00.523476 real-brasileiro-0.2.1/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1073 2023-07-18 03:36:07.000000 real-brasileiro-0.2.1/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 03:46:00.523476 real-brasileiro-0.2.1/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      966 2023-07-18 03:42:42.000000 real-brasileiro-0.2.1/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:46:00.523476 real-brasileiro-0.2.1/real_brasileiro.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 03:46:00.000000 real-brasileiro-0.2.1/real_brasileiro.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      182 2023-07-18 03:46:00.000000 real-brasileiro-0.2.1/real_brasileiro.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-18 03:46:00.000000 real-brasileiro-0.2.1/real_brasileiro.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-18 03:46:00.000000 real-brasileiro-0.2.1/real_brasileiro.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-18 03:46:00.523476 real-brasileiro-0.2.1/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      377 2023-07-18 03:45:16.000000 real-brasileiro-0.2.1/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1073 2023-07-18 03:36:07.000000 real-brasileiro-0.2.5/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      966 2023-07-18 03:51:31.000000 real-brasileiro-0.2.5/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/real_br/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       32 2023-07-18 03:36:07.000000 real-brasileiro-0.2.5/real_br/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4501 2023-07-18 03:51:31.000000 real-brasileiro-0.2.5/real_br/real_br.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/real_brasileiro.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 03:56:51.000000 real-brasileiro-0.2.5/real_brasileiro.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      221 2023-07-18 03:56:51.000000 real-brasileiro-0.2.5/real_brasileiro.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-18 03:56:51.000000 real-brasileiro-0.2.5/real_brasileiro.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-07-18 03:56:51.000000 real-brasileiro-0.2.5/real_brasileiro.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      403 2023-07-18 03:56:48.000000 real-brasileiro-0.2.5/setup.py
```

### Comparing `real-brasileiro-0.2.1/LICENSE` & `real-brasileiro-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `real-brasileiro-0.2.1/PKG-INFO` & `real-brasileiro-0.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real-brasileiro
-Version: 0.2.1
+Version: 0.2.5
 Summary: UNKNOWN
 Home-page: https://github.com/MikalROn/Real_br
 Author: Daniel Coêlho
 Author-email: heromon.9010@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `real-brasileiro-0.2.1/README.md` & `real-brasileiro-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `real-brasileiro-0.2.1/real_brasileiro.egg-info/PKG-INFO` & `real-brasileiro-0.2.5/real_brasileiro.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real-brasileiro
-Version: 0.2.1
+Version: 0.2.5
 Summary: UNKNOWN
 Home-page: https://github.com/MikalROn/Real_br
 Author: Daniel Coêlho
 Author-email: heromon.9010@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3
```

