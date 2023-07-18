# Comparing `tmp/lesscode_utils-0.0.0.tar.gz` & `tmp/lesscode_utils-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_utils-0.0.0.tar", last modified: Thu Jun 15 09:23:47 2023, max compression
+gzip compressed data, was "dist/lesscode_utils-0.0.1.tar", last modified: Tue Jul 18 07:10:41 2023, max compression
```

## Comparing `lesscode_utils-0.0.0.tar` & `lesscode_utils-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,28 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/
--rw-r--r--   0 baai       (501) staff       (20)      375 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       50 2023-06-15 08:16:15.000000 lesscode_utils-0.0.0/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/lesscode_utils/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-06-15 07:55:10.000000 lesscode_utils-0.0.0/lesscode_utils/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     2777 2023-06-15 09:20:19.000000 lesscode_utils-0.0.0/lesscode_utils/date_time_utils.py
--rw-r--r--   0 baai       (501) staff       (20)      786 2023-06-15 08:16:15.000000 lesscode_utils-0.0.0/lesscode_utils/json_utils.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-06-15 07:56:59.000000 lesscode_utils-0.0.0/lesscode_utils/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/lesscode_utils.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      375 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/lesscode_utils.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      323 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/lesscode_utils.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/lesscode_utils.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       16 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/lesscode_utils.egg-info/requires.txt
--rw-r--r--   0 baai       (501) staff       (20)       15 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/lesscode_utils.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-06-15 09:23:47.000000 lesscode_utils-0.0.0/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1267 2023-06-15 08:17:20.000000 lesscode_utils-0.0.0/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/
+-rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       50 2023-06-15 08:16:15.000000 lesscode_utils-0.0.1/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/lesscode_utils/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-06-15 07:55:10.000000 lesscode_utils-0.0.1/lesscode_utils/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     2777 2023-06-15 09:20:19.000000 lesscode_utils-0.0.1/lesscode_utils/date_time_utils.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/
+-rw-r--r--   0 baai       (501) staff       (20)      226 2022-04-19 02:49:20.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1817 2023-07-18 06:03:34.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/aes.py
+-rw-r--r--   0 baai       (501) staff       (20)      621 2023-07-18 07:00:16.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/base64.py
+-rw-r--r--   0 baai       (501) staff       (20)     1722 2023-07-18 07:00:16.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/des.py
+-rw-r--r--   0 baai       (501) staff       (20)      609 2023-07-18 07:00:16.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/hmac.py
+-rw-r--r--   0 baai       (501) staff       (20)      289 2023-07-18 07:00:16.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/md5.py
+-rw-r--r--   0 baai       (501) staff       (20)     2264 2023-07-18 07:00:16.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/rsa.py
+-rw-r--r--   0 baai       (501) staff       (20)      288 2023-07-18 07:00:16.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/sha1.py
+-rw-r--r--   0 baai       (501) staff       (20)      292 2023-07-18 07:00:16.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/sha256.py
+-rw-r--r--   0 baai       (501) staff       (20)     3896 2023-07-18 07:00:16.000000 lesscode_utils-0.0.1/lesscode_utils/encryption_algorithm/smx.py
+-rw-r--r--   0 baai       (501) staff       (20)     9626 2023-07-18 07:09:19.000000 lesscode_utils-0.0.1/lesscode_utils/es_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)      786 2023-06-15 08:16:15.000000 lesscode_utils-0.0.1/lesscode_utils/json_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-18 07:02:54.000000 lesscode_utils-0.0.1/lesscode_utils/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/lesscode_utils.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/lesscode_utils.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      793 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/lesscode_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/lesscode_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       16 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/lesscode_utils.egg-info/requires.txt
+-rw-r--r--   0 baai       (501) staff       (20)       15 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/lesscode_utils.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-07-18 07:10:41.000000 lesscode_utils-0.0.1/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1267 2023-06-15 08:17:20.000000 lesscode_utils-0.0.1/setup.py
```

### Comparing `lesscode_utils-0.0.0/lesscode_utils/date_time_utils.py` & `lesscode_utils-0.0.1/lesscode_utils/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.0/lesscode_utils/json_utils.py` & `lesscode_utils-0.0.1/lesscode_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.0/setup.py` & `lesscode_utils-0.0.1/setup.py`

 * *Files identical despite different names*

