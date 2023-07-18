# Comparing `tmp/ubiq-security-2.1.0.tar.gz` & `tmp/ubiq-security-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubiq-security-2.1.0.tar", last modified: Tue Jul 18 15:36:50 2023, max compression
+gzip compressed data, was "ubiq-security-2.1.1.tar", last modified: Tue Jul 18 16:12:35 2023, max compression
```

## Comparing `ubiq-security-2.1.0.tar` & `ubiq-security-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:36:50.486871 ubiq-security-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     1104 2022-11-21 21:22:47.000000 ubiq-security-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9019 2023-07-18 15:36:50.486220 ubiq-security-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8063 2023-05-23 20:56:07.000000 ubiq-security-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 15:36:50.487279 ubiq-security-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1742 2022-11-21 21:22:47.000000 ubiq-security-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:36:50.472869 ubiq-security-2.1.0/ubiq_security/
--rw-r--r--   0 root         (0) root         (0)      226 2022-11-21 21:22:47.000000 ubiq-security-2.1.0/ubiq_security/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3843 2022-11-21 21:22:47.000000 ubiq-security-2.1.0/ubiq_security/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     5455 2023-05-04 23:15:07.000000 ubiq-security-2.1.0/ubiq_security/auth.py
--rw-r--r--   0 root         (0) root         (0)     3607 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5974 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/credentials.py
--rw-r--r--   0 root         (0) root         (0)    13317 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/decrypt.py
--rw-r--r--   0 root         (0) root         (0)     8317 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     5158 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:36:50.484433 ubiq-security-2.1.0/ubiq_security/fpe/
--rw-r--r--   0 root         (0) root         (0)      124 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/fpe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6452 2023-06-21 16:35:33.000000 ubiq-security-2.1.0/ubiq_security/fpe/common.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-06-15 19:59:00.000000 ubiq-security-2.1.0/ubiq_security/fpe/decrypt.py
--rw-r--r--   0 root         (0) root         (0)     3611 2023-06-21 16:35:33.000000 ubiq-security-2.1.0/ubiq_security/fpe/encrypt.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-18 15:05:54.000000 ubiq-security-2.1.0/ubiq_security/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:36:50.479018 ubiq-security-2.1.0/ubiq_security.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9019 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      560 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-18 15:36:50.000000 ubiq-security-2.1.0/ubiq_security.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 16:12:35.220896 ubiq-security-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1104 2022-11-21 21:22:47.000000 ubiq-security-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9019 2023-07-18 16:12:35.220374 ubiq-security-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8063 2023-05-23 20:56:07.000000 ubiq-security-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 16:12:35.221213 ubiq-security-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1742 2022-11-21 21:22:47.000000 ubiq-security-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 16:12:35.203692 ubiq-security-2.1.1/ubiq_security/
+-rw-r--r--   0 root         (0) root         (0)      226 2022-11-21 21:22:47.000000 ubiq-security-2.1.1/ubiq_security/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3843 2022-11-21 21:22:47.000000 ubiq-security-2.1.1/ubiq_security/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2023-05-04 23:15:07.000000 ubiq-security-2.1.1/ubiq_security/auth.py
+-rw-r--r--   0 root         (0) root         (0)     3607 2023-06-15 19:59:00.000000 ubiq-security-2.1.1/ubiq_security/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5974 2023-06-15 19:59:00.000000 ubiq-security-2.1.1/ubiq_security/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2023-06-15 19:59:00.000000 ubiq-security-2.1.1/ubiq_security/decrypt.py
+-rw-r--r--   0 root         (0) root         (0)     8317 2023-06-15 19:59:00.000000 ubiq-security-2.1.1/ubiq_security/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     5158 2023-06-15 19:59:00.000000 ubiq-security-2.1.1/ubiq_security/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 16:12:35.218473 ubiq-security-2.1.1/ubiq_security/fpe/
+-rw-r--r--   0 root         (0) root         (0)      124 2023-06-15 19:59:00.000000 ubiq-security-2.1.1/ubiq_security/fpe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6452 2023-06-21 16:35:33.000000 ubiq-security-2.1.1/ubiq_security/fpe/common.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-06-15 19:59:00.000000 ubiq-security-2.1.1/ubiq_security/fpe/decrypt.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-07-18 16:04:08.000000 ubiq-security-2.1.1/ubiq_security/fpe/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-18 16:11:09.000000 ubiq-security-2.1.1/ubiq_security/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 16:12:35.212040 ubiq-security-2.1.1/ubiq_security.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9019 2023-07-18 16:12:35.000000 ubiq-security-2.1.1/ubiq_security.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      560 2023-07-18 16:12:35.000000 ubiq-security-2.1.1/ubiq_security.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 16:12:35.000000 ubiq-security-2.1.1/ubiq_security.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-18 16:12:35.000000 ubiq-security-2.1.1/ubiq_security.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-18 16:12:35.000000 ubiq-security-2.1.1/ubiq_security.egg-info/top_level.txt
```

### Comparing `ubiq-security-2.1.0/LICENSE` & `ubiq-security-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/PKG-INFO` & `ubiq-security-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiq-security
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python client library for accessing Ubiq Platform
 Home-page: https://gitlab.com/ubiqsecurity/ubiq-python
 Author: Ubiq Security, Inc.
 Author-email: support@ubiqsecurity.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ubiq-security-2.1.0/README.md` & `ubiq-security-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/setup.py` & `ubiq-security-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/algorithm.py` & `ubiq-security-2.1.1/ubiq_security/algorithm.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/auth.py` & `ubiq-security-2.1.1/ubiq_security/auth.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/configuration.py` & `ubiq-security-2.1.1/ubiq_security/configuration.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/credentials.py` & `ubiq-security-2.1.1/ubiq_security/credentials.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/decrypt.py` & `ubiq-security-2.1.1/ubiq_security/decrypt.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/encrypt.py` & `ubiq-security-2.1.1/ubiq_security/encrypt.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/events.py` & `ubiq-security-2.1.1/ubiq_security/events.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/fpe/common.py` & `ubiq-security-2.1.1/ubiq_security/fpe/common.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/fpe/decrypt.py` & `ubiq-security-2.1.1/ubiq_security/fpe/decrypt.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-2.1.0/ubiq_security/fpe/encrypt.py` & `ubiq-security-2.1.1/ubiq_security/fpe/encrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #/usr/bin/env python3
 
 import base64
-from .algo import ff1
+from ubiq_security_fpe import ff1
 
 from ..credentials import credentials
 
 from .common import fmtInput, strConvertRadix, encKeyNumber, fmtOutput
 from .common import fetchFFS, fetchKey, fetchCurrentKeys
 
 class Encryption:
```

### Comparing `ubiq-security-2.1.0/ubiq_security.egg-info/PKG-INFO` & `ubiq-security-2.1.1/ubiq_security.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiq-security
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python client library for accessing Ubiq Platform
 Home-page: https://gitlab.com/ubiqsecurity/ubiq-python
 Author: Ubiq Security, Inc.
 Author-email: support@ubiqsecurity.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ubiq-security-2.1.0/ubiq_security.egg-info/SOURCES.txt` & `ubiq-security-2.1.1/ubiq_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

