# Comparing `tmp/couchcopy-0.2.0.tar.gz` & `tmp/couchcopy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchcopy-0.2.0.tar", last modified: Thu Jun 22 10:36:35 2023, max compression
+gzip compressed data, was "couchcopy-0.2.1.tar", last modified: Tue Jul 18 08:53:38 2023, max compression
```

## Comparing `couchcopy-0.2.0.tar` & `couchcopy-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2023-06-22 10:36:35.922452 couchcopy-0.2.0/
--rw-r--r--   0 adrien    (1000) adrien    (1000)    35147 2021-11-19 06:19:19.000000 couchcopy-0.2.0/LICENSE
--rw-r--r--   0 adrien    (1000) adrien    (1000)     5990 2023-06-22 10:36:35.922452 couchcopy-0.2.0/PKG-INFO
--rw-r--r--   0 adrien    (1000) adrien    (1000)     5758 2023-06-06 09:37:26.000000 couchcopy-0.2.0/README.rst
--rwxr-xr-x   0 adrien    (1000) adrien    (1000)    24757 2023-06-22 10:33:20.000000 couchcopy-0.2.0/couchcopy
-drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2023-06-22 10:36:35.922452 couchcopy-0.2.0/couchcopy.egg-info/
--rw-r--r--   0 adrien    (1000) adrien    (1000)     5990 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/PKG-INFO
--rw-r--r--   0 adrien    (1000) adrien    (1000)      211 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/SOURCES.txt
--rw-r--r--   0 adrien    (1000) adrien    (1000)        1 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/dependency_links.txt
--rw-r--r--   0 adrien    (1000) adrien    (1000)       29 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/requires.txt
--rw-r--r--   0 adrien    (1000) adrien    (1000)        1 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/top_level.txt
--rw-r--r--   0 adrien    (1000) adrien    (1000)       76 2023-06-22 10:36:35.922452 couchcopy-0.2.0/setup.cfg
--rw-r--r--   0 adrien    (1000) adrien    (1000)      725 2021-11-19 06:19:19.000000 couchcopy-0.2.0/setup.py
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2023-07-18 08:53:38.817871 couchcopy-0.2.1/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    35147 2023-06-07 07:33:16.000000 couchcopy-0.2.1/LICENSE
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5990 2023-07-18 08:53:38.817871 couchcopy-0.2.1/PKG-INFO
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5758 2023-06-07 07:33:16.000000 couchcopy-0.2.1/README.rst
+-rwxr-xr-x   0 adrien    (1000) adrien    (1000)    24829 2023-07-18 08:52:59.000000 couchcopy-0.2.1/couchcopy
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2023-07-18 08:53:38.817871 couchcopy-0.2.1/couchcopy.egg-info/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5990 2023-07-18 08:53:38.000000 couchcopy-0.2.1/couchcopy.egg-info/PKG-INFO
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      211 2023-07-18 08:53:38.000000 couchcopy-0.2.1/couchcopy.egg-info/SOURCES.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)        1 2023-07-18 08:53:38.000000 couchcopy-0.2.1/couchcopy.egg-info/dependency_links.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       29 2023-07-18 08:53:38.000000 couchcopy-0.2.1/couchcopy.egg-info/requires.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)        1 2023-07-18 08:53:38.000000 couchcopy-0.2.1/couchcopy.egg-info/top_level.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       76 2023-07-18 08:53:38.817871 couchcopy-0.2.1/setup.cfg
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      725 2023-06-07 07:33:16.000000 couchcopy-0.2.1/setup.py
```

### Comparing `couchcopy-0.2.0/LICENSE` & `couchcopy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `couchcopy-0.2.0/PKG-INFO` & `couchcopy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchcopy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Backup, load and restore CouchDB clusters
 Home-page: https://github.com/tolteck/couchcopy
 Author: Hoël Iris
 License: GPLv3
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `couchcopy-0.2.0/README.rst` & `couchcopy-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `couchcopy-0.2.0/couchcopy` & `couchcopy-0.2.1/couchcopy`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import sys
 from tempfile import TemporaryDirectory
 
 import aiocouch
 import yaml
 
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 # Tweak this parameter to your needs: From 17 minutes with 16 workers to 28
 # minutes with 8 workers for 10^5 databases on my machine.
 N_WORKERS = 16
 
 
 async def subprocess(*args, shell=False, input=None):
     stdin = None if input is None else asyncio.subprocess.PIPE
@@ -104,15 +104,16 @@
             # tar can exit with return code 1 if files are modified on disk
             # during the archive creation. This is normal behavior when the
             # CouchDB instance is running, so let's filter out these errors and
             # fail only on other ones.
             if returncode1 == 1:
                 stderr1 = '\n'.join(
                     l for l in stderr1.decode().splitlines()
-                    if not l.endswith('file changed as we read it')).encode()
+                    if not l.endswith('File removed before we read it',
+                                      'file changed as we read it')).encode()
                 if not stderr1:
                     returncode1 = 0
 
             if returncode1 != 0:
                 raise Exception(f'Command tar returned code {returncode1}, '
                                 f'stderr: {stderr1.decode()}')
             if returncode2 != 0:
```

### Comparing `couchcopy-0.2.0/couchcopy.egg-info/PKG-INFO` & `couchcopy-0.2.1/couchcopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchcopy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Backup, load and restore CouchDB clusters
 Home-page: https://github.com/tolteck/couchcopy
 Author: Hoël Iris
 License: GPLv3
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `couchcopy-0.2.0/setup.py` & `couchcopy-0.2.1/setup.py`

 * *Files identical despite different names*

