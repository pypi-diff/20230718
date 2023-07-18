# Comparing `tmp/renku_lock-2.6.1-py3-none-any.whl.zip` & `tmp/renku_lock-2.6.1rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 3295 bytes, number of entries: 4
--rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 renku_lock/__init__.py
--rw-r--r--  2.0 unx    11300 b- defN 80-Jan-01 00:00 renku_lock-2.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 renku_lock-2.6.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      293 b- defN 16-Jan-01 00:00 renku_lock-2.6.1.dist-info/RECORD
-4 files, 11703 bytes uncompressed, 2725 bytes compressed:  76.7%
+Zip file size: 3324 bytes, number of entries: 4
+-rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 renku_lock/__init__.py
+-rw-r--r--  2.0 unx    11306 b- defN 80-Jan-01 00:00 renku_lock-2.6.1rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 renku_lock-2.6.1rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      302 b- defN 16-Jan-01 00:00 renku_lock-2.6.1rc1.dist-info/RECORD
+4 files, 11721 bytes uncompressed, 2736 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
 Filename: renku_lock/__init__.py
 Comment: 
 
-Filename: renku_lock-2.6.1.dist-info/METADATA
+Filename: renku_lock-2.6.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: renku_lock-2.6.1.dist-info/WHEEL
+Filename: renku_lock-2.6.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: renku_lock-2.6.1.dist-info/RECORD
+Filename: renku_lock-2.6.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## renku_lock/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "2.6.1"
+__version__ = "2.6.1rc1"
```

## Comparing `renku_lock-2.6.1.dist-info/METADATA` & `renku_lock-2.6.1rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renku-lock
-Version: 2.6.1
+Version: 2.6.1rc1
 Summary: Python SDK and CLI for the Renku platform. lock package
 Home-page: https://github.com/swissdatasciencecenter/renku-python
 License: Apache-2.0
 Keywords: Renku,CLI
 Author: Swiss Data Science Center
 Author-email: contact@datascience.ch
 Requires-Python: >=3.8.1,<3.12
@@ -129,15 +129,15 @@
 Requires-Dist: python-gitlab (==3.8.1) ; python_full_version >= "3.7.0"
 Requires-Dist: pytz (==2023.3)
 Requires-Dist: pywin32 (==227) ; sys_platform == "win32"
 Requires-Dist: pyyaml (==6.0) ; python_version >= "3.6"
 Requires-Dist: pyzmq (==25.1.0) ; python_version >= "3.6"
 Requires-Dist: rdflib (==6.3.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: redis (==4.5.4) ; python_version >= "3.7"
-Requires-Dist: renku (==2.6.1)
+Requires-Dist: renku (==2.6.1rc1)
 Requires-Dist: requests (==2.31.0) ; python_version >= "3.7"
 Requires-Dist: requests-toolbelt (==1.0.0) ; python_version >= "2.7" and python_version < "3.0.dev0" or python_version >= "3.4.dev0"
 Requires-Dist: rich (==13.3.5) ; python_full_version >= "3.7.0"
 Requires-Dist: rq (==1.15.0) ; python_version >= "3.6"
 Requires-Dist: rq-scheduler (==0.13.1)
 Requires-Dist: ruamel.yaml (==0.17.21) ; python_version >= "3.7"
 Requires-Dist: ruamel.yaml.clib (==0.2.7) ; platform_python_implementation == "CPython" and python_version < "3.11" and python_version >= "3.5"
```

