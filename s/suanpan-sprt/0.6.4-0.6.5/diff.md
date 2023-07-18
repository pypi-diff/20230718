# Comparing `tmp/suanpan-sprt-0.6.4.tar.gz` & `tmp/suanpan-sprt-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.6.4.tar", last modified: Tue Jul 18 08:32:10 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.6.5.tar", last modified: Tue Jul 18 09:03:50 2023, max compression
```

## Comparing `suanpan-sprt-0.6.4.tar` & `suanpan-sprt-0.6.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4317 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.4/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5737 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.4/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2087 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.4/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6876 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.4/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.4/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4337 2023-07-18 09:03:49.000000 suanpan-sprt-0.6.5/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1251 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5737 2023-07-18 07:58:15.000000 suanpan-sprt-0.6.5/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2087 2023-07-17 07:00:31.000000 suanpan-sprt-0.6.5/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6876 2023-07-18 08:32:10.000000 suanpan-sprt-0.6.5/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6419 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3261 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-07-12 09:08:26.000000 suanpan-sprt-0.6.5/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-07-18 09:03:49.000000 suanpan-sprt-0.6.5/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-07-18 09:03:50.000000 suanpan-sprt-0.6.5/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.6.4/setup.py` & `suanpan-sprt-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.4/sprt/__main__.py` & `suanpan-sprt-0.6.5/sprt/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import sys
 import signal
 import asyncio
 import click
 import pathlib
 from hypercorn.asyncio import serve
 from hypercorn.config import Config
@@ -61,15 +62,15 @@
     signal.signal(signal.SIGINT, receive_signal)
     app = server.create_app(working_dir, log_file, new_log)
     app.logger.info(f'use {log_file} {log_level} {new_log}')
 
     config = Config()
     config.bind = [f'{host}:{port}']
     if log_level.upper() == 'DEBUG':
-        config.accesslog = '-'
+        config.accesslog = log_file
     app.logger.info(f'python runtime running on {host}:{port}')
     asyncio.run(serve(app, config))
 
 
 def receive_signal(signal_number, frame):
     print('receive_signal', signal_number)
     sys.exit(128 + signal_number)
```

### Comparing `suanpan-sprt-0.6.4/sprt/arguments.py` & `suanpan-sprt-0.6.5/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.4/sprt/envs.py` & `suanpan-sprt-0.6.5/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.4/sprt/loader.py` & `suanpan-sprt-0.6.5/sprt/loader.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.4/sprt/log.py` & `suanpan-sprt-0.6.5/sprt/log.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.4/sprt/master.py` & `suanpan-sprt-0.6.5/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.4/sprt/server.py` & `suanpan-sprt-0.6.5/sprt/server.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.4/sprt/storage.py` & `suanpan-sprt-0.6.5/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.4/sprt/testing.py` & `suanpan-sprt-0.6.5/sprt/testing.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.6.4/sprt/utils.py` & `suanpan-sprt-0.6.5/sprt/utils.py`

 * *Files identical despite different names*

