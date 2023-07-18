# Comparing `tmp/tarn-0.9.3.tar.gz` & `tmp/tarn-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.9.3.tar", last modified: Thu Jul 13 16:25:40 2023, max compression
+gzip compressed data, was "tarn-0.9.4.tar", last modified: Tue Jul 18 13:22:11 2023, max compression
```

## Comparing `tarn-0.9.3.tar` & `tarn-0.9.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-13 16:25:36.000000 tarn-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 16:25:36.000000 tarn-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 16:25:40.056749 tarn-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-13 16:25:36.000000 tarn-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-13 16:25:36.000000 tarn-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-13 16:25:36.000000 tarn-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:25:40.056749 tarn-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-13 16:25:36.000000 tarn-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.052749 tarn-0.9.3/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.056749 tarn-0.9.3/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-13 16:25:36.000000 tarn-0.9.3/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:25:40.052749 tarn-0.9.3/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 16:25:39.000000 tarn-0.9.3/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-13 16:25:40.000000 tarn-0.9.3/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:25:39.000000 tarn-0.9.3/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-13 16:25:39.000000 tarn-0.9.3/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 16:25:40.000000 tarn-0.9.3/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.434451 tarn-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-18 13:22:09.000000 tarn-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 13:22:09.000000 tarn-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-18 13:22:11.434451 tarn-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 13:22:09.000000 tarn-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 13:22:09.000000 tarn-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 13:22:09.000000 tarn-0.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:22:11.434451 tarn-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-18 13:22:09.000000 tarn-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.434451 tarn-0.9.4/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 13:22:09.000000 tarn-0.9.4/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:22:11.430451 tarn-0.9.4/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 13:22:11.000000 tarn-0.9.4/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.9.3/LICENSE` & `tarn-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/PKG-INFO` & `tarn-0.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.9.3
+Version: 0.9.4
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.3.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.4.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.9.3/README.md` & `tarn-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/pyproject.toml` & `tarn-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/setup.py` & `tarn-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/cache/storage.py` & `tarn-0.9.4/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/compat.py` & `tarn-0.9.4/tarn/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/config.py` & `tarn-0.9.4/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/digest.py` & `tarn-0.9.4/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/interface.py` & `tarn-0.9.4/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/local/storage.py` & `tarn-0.9.4/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/location/disk_dict.py` & `tarn-0.9.4/tarn/location/disk_dict.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/location/fanout.py` & `tarn-0.9.4/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/location/interface.py` & `tarn-0.9.4/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/location/levels.py` & `tarn-0.9.4/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/location/nginx.py` & `tarn-0.9.4/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/location/redis.py` & `tarn-0.9.4/tarn/location/redis.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/location/s3.py` & `tarn-0.9.4/tarn/location/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                     yield self._get_buffer(path), self.get_labels(path)
                 else:
                     self.update_usage_date(path)
                     yield self._get_buffer(path)
 
             except ClientError as e:
                 if (
-                    e.response['Error']['Code'] == '404'
+                    e.response['ResponseMetadata']['HTTPStatusCode'] == 404
                     or e.response['Error']['Code'] == 'NoSuchKey'
                 ):  # file doesn't exist
                     yield
                 else:
                     raise
             except ConnectionError:
                 yield
```

### Comparing `tarn-0.9.3/tarn/location/scp.py` & `tarn-0.9.4/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/pickler/compat.py` & `tarn-0.9.4/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/pickler/interface.py` & `tarn-0.9.4/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/pool/hash_key.py` & `tarn-0.9.4/tarn/pool/hash_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/pool/pickle_key.py` & `tarn-0.9.4/tarn/pool/pickle_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/serializers.py` & `tarn-0.9.4/tarn/serializers.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/tools/labels.py` & `tarn-0.9.4/tarn/tools/labels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/tools/locker.py` & `tarn-0.9.4/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/tools/size.py` & `tarn-0.9.4/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/tools/usage.py` & `tarn-0.9.4/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn/utils.py` & `tarn-0.9.4/tarn/utils.py`

 * *Files identical despite different names*

### Comparing `tarn-0.9.3/tarn.egg-info/PKG-INFO` & `tarn-0.9.4/tarn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.9.3
+Version: 0.9.4
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.3.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.9.4.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.9.3/tarn.egg-info/SOURCES.txt` & `tarn-0.9.4/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

