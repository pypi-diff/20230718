# Comparing `tmp/python-define-1.0.0.tar.gz` & `tmp/python-define-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-define-1.0.0.tar", last modified: Tue Jul 18 02:51:16 2023, max compression
+gzip compressed data, was "python-define-1.0.1.tar", last modified: Tue Jul 18 02:54:50 2023, max compression
```

## Comparing `python-define-1.0.0.tar` & `python-define-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-18 02:51:16.840229 python-define-1.0.0/
--rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.0.0/LICENSE
--rw-r--r--   0 grant     (1000) grant     (1000)    44853 2023-07-18 02:51:16.840229 python-define-1.0.0/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)     4374 2023-07-18 02:49:27.000000 python-define-1.0.0/README.md
--rwxr-xr-x   0 grant     (1000) grant     (1000)     5452 2023-07-18 01:50:22.000000 python-define-1.0.0/define.py
--rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-07-18 02:50:19.000000 python-define-1.0.0/pyproject.toml
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-18 02:51:16.840229 python-define-1.0.0/python_define.egg-info/
--rw-r--r--   0 grant     (1000) grant     (1000)    44853 2023-07-18 02:51:16.000000 python-define-1.0.0/python_define.egg-info/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-07-18 02:51:16.000000 python-define-1.0.0/python_define.egg-info/SOURCES.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-07-18 02:51:16.000000 python-define-1.0.0/python_define.egg-info/dependency_links.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-18 02:51:16.000000 python-define-1.0.0/python_define.egg-info/entry_points.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-07-18 02:51:16.000000 python-define-1.0.0/python_define.egg-info/requires.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-07-18 02:51:16.000000 python-define-1.0.0/python_define.egg-info/top_level.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-18 02:51:16.840229 python-define-1.0.0/setup.cfg
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-18 02:54:50.429218 python-define-1.0.1/
+-rw-r--r--   0 grant     (1000) grant     (1000)    34523 2023-06-29 07:50:39.000000 python-define-1.0.1/LICENSE
+-rw-r--r--   0 grant     (1000) grant     (1000)    44853 2023-07-18 02:54:50.429218 python-define-1.0.1/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)     4374 2023-07-18 02:49:27.000000 python-define-1.0.1/README.md
+-rwxr-xr-x   0 grant     (1000) grant     (1000)     5452 2023-07-18 01:50:22.000000 python-define-1.0.1/define.py
+-rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-07-18 02:53:16.000000 python-define-1.0.1/pyproject.toml
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-07-18 02:54:50.429218 python-define-1.0.1/python_define.egg-info/
+-rw-r--r--   0 grant     (1000) grant     (1000)    44853 2023-07-18 02:54:50.000000 python-define-1.0.1/python_define.egg-info/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-07-18 02:54:50.000000 python-define-1.0.1/python_define.egg-info/SOURCES.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-07-18 02:54:50.000000 python-define-1.0.1/python_define.egg-info/dependency_links.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-18 02:54:50.000000 python-define-1.0.1/python_define.egg-info/entry_points.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-07-18 02:54:50.000000 python-define-1.0.1/python_define.egg-info/requires.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-07-18 02:54:50.000000 python-define-1.0.1/python_define.egg-info/top_level.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-07-18 02:54:50.429218 python-define-1.0.1/setup.cfg
```

### Comparing `python-define-1.0.0/LICENSE` & `python-define-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-define-1.0.0/PKG-INFO` & `python-define-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.0.0
+Version: 1.0.1
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `python-define-1.0.0/README.md` & `python-define-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python-define-1.0.0/define.py` & `python-define-1.0.1/define.py`

 * *Files identical despite different names*

### Comparing `python-define-1.0.0/pyproject.toml` & `python-define-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-define"
-version = "1.0.0"
+version = "1.0.1"
 description = "An OpenAI powered command-line linguistics assistant"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Grant Carthew", email = "grant@carthew.net"},
 ]
```

### Comparing `python-define-1.0.0/python_define.egg-info/PKG-INFO` & `python-define-1.0.1/python_define.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.0.0
+Version: 1.0.1
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

