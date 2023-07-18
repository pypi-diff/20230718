# Comparing `tmp/urlybird-0.0.1a3.tar.gz` & `tmp/urlybird-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlybird-0.0.1a3.tar", last modified: Sun Oct 31 07:44:24 2021, max compression
+gzip compressed data, was "urlybird-0.0.2.tar", last modified: Tue Jan 25 19:06:08 2022, max compression
```

## Comparing `urlybird-0.0.1a3.tar` & `urlybird-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2021-10-31 07:44:24.020135 urlybird-0.0.1a3/
--rw-r--r--   0 lash      (1000) lash      (1000)      498 2012-12-28 03:21:09.000000 urlybird-0.0.1a3/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       32 2021-10-31 06:54:38.000000 urlybird-0.0.1a3/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      682 2021-10-31 07:44:24.020135 urlybird-0.0.1a3/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      868 2021-10-31 06:38:03.000000 urlybird-0.0.1a3/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)      326 2021-10-31 06:38:03.000000 urlybird-0.0.1a3/WARRANTY
--rw-r--r--   0 lash      (1000) lash      (1000)      685 2021-10-31 07:44:24.023468 urlybird-0.0.1a3/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      494 2021-10-31 06:53:27.000000 urlybird-0.0.1a3/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2021-10-31 07:44:24.020135 urlybird-0.0.1a3/urlybird/
--rw-r--r--   0 lash      (1000) lash      (1000)     1024 2021-10-31 06:26:32.000000 urlybird-0.0.1a3/urlybird/merge.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2021-10-31 07:44:24.020135 urlybird-0.0.1a3/urlybird.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      682 2021-10-31 07:44:23.000000 urlybird-0.0.1a3/urlybird.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      200 2021-10-31 07:44:23.000000 urlybird-0.0.1a3/urlybird.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2021-10-31 07:44:23.000000 urlybird-0.0.1a3/urlybird.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        9 2021-10-31 07:44:23.000000 urlybird-0.0.1a3/urlybird.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-01-25 19:06:08.565420 urlybird-0.0.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)      498 2012-12-28 03:21:09.000000 urlybird-0.0.2/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       32 2021-10-31 06:54:38.000000 urlybird-0.0.2/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      680 2022-01-25 19:06:08.565420 urlybird-0.0.2/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      868 2021-10-31 06:38:03.000000 urlybird-0.0.2/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)      326 2021-10-31 06:38:03.000000 urlybird-0.0.2/WARRANTY
+-rw-r--r--   0 lash      (1000) lash      (1000)      683 2022-01-25 19:06:08.565420 urlybird-0.0.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      494 2021-10-31 06:53:27.000000 urlybird-0.0.2/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-01-25 19:06:08.565420 urlybird-0.0.2/urlybird/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1020 2022-01-25 18:57:47.000000 urlybird-0.0.2/urlybird/host.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1024 2022-01-25 18:15:12.000000 urlybird-0.0.2/urlybird/merge.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-01-25 19:06:08.565420 urlybird-0.0.2/urlybird.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      680 2022-01-25 19:06:08.000000 urlybird-0.0.2/urlybird.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      217 2022-01-25 19:06:08.000000 urlybird-0.0.2/urlybird.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2022-01-25 19:06:08.000000 urlybird-0.0.2/urlybird.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2022-01-25 19:06:08.000000 urlybird-0.0.2/urlybird.egg-info/top_level.txt
```

### Comparing `urlybird-0.0.1a3/PKG-INFO` & `urlybird-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlybird
-Version: 0.0.1a3
+Version: 0.0.2
 Summary: Common url operations not covered by the standard library urllib
 Home-page: https://gitlab.com/chaintools/chainlib
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: WTFPL
 Keywords: url,internet
 Platform: UNKNOWN
```

### Comparing `urlybird-0.0.1a3/WAIVER` & `urlybird-0.0.2/WAIVER`

 * *Files identical despite different names*

### Comparing `urlybird-0.0.1a3/setup.cfg` & `urlybird-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = urlybird
-version = 0.0.1a3
+version = 0.0.2
 description = Common url operations not covered by the standard library urllib
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://gitlab.com/chaintools/chainlib
 keywords = 
 	url
 	internet
```

### Comparing `urlybird-0.0.1a3/urlybird/merge.py` & `urlybird-0.0.2/urlybird/merge.py`

 * *Files identical despite different names*

### Comparing `urlybird-0.0.1a3/urlybird.egg-info/PKG-INFO` & `urlybird-0.0.2/urlybird.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlybird
-Version: 0.0.1a3
+Version: 0.0.2
 Summary: Common url operations not covered by the standard library urllib
 Home-page: https://gitlab.com/chaintools/chainlib
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: WTFPL
 Keywords: url,internet
 Platform: UNKNOWN
```

