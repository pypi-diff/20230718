# Comparing `tmp/sapphire_config-1.0.1.tar.gz` & `tmp/sapphire_config-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapphire_config-1.0.1.tar", last modified: Thu Jul  6 02:21:37 2023, max compression
+gzip compressed data, was "sapphire_config-1.0.2.tar", last modified: Mon Jul 17 22:45:31 2023, max compression
```

## Comparing `sapphire_config-1.0.1.tar` & `sapphire_config-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1070 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/LICENSE
--rw-rw-r--   0 valentic   (500) valentic   (500)       98 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/MANIFEST.in
--rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      199 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/README.md
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/examples/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/examples/components/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1042 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/examples/components/demo.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     2830 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/examples/components/demo.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/examples/config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      982 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/examples/config/demo.conf
--rwxrwxr-x   0 valentic   (500) valentic   (500)     4932 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/examples/config/demo.py
--rw-rw-r--   0 valentic   (500) valentic   (500)      996 2023-07-06 02:17:33.000000 sapphire_config-1.0.1/pyproject.toml
--rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/setup.cfg
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/src/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/src/sapphire_config/
--rw-rw-r--   0 valentic   (500) valentic   (500)      251 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/src/sapphire_config/__init__.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     5139 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/src/sapphire_config/component.py
--rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-06 02:14:09.000000 sapphire_config-1.0.1/src/sapphire_config/metadata.py
--rw-rw-r--   0 valentic   (500) valentic   (500)     9235 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/src/sapphire_config/parser.py
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/src/sapphire_config.egg-info/
--rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-06 02:21:36.000000 sapphire_config-1.0.1/src/sapphire_config.egg-info/PKG-INFO
--rw-rw-r--   0 valentic   (500) valentic   (500)      588 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/src/sapphire_config.egg-info/SOURCES.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-06 02:21:36.000000 sapphire_config-1.0.1/src/sapphire_config.egg-info/dependency_links.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       92 2023-07-06 02:21:36.000000 sapphire_config-1.0.1/src/sapphire_config.egg-info/requires.txt
--rw-rw-r--   0 valentic   (500) valentic   (500)       16 2023-07-06 02:21:36.000000 sapphire_config-1.0.1/src/sapphire_config.egg-info/top_level.txt
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/tests/
-drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-06 02:21:37.000000 sapphire_config-1.0.1/tests/__pycache__/
--rw-rw-r--   0 valentic   (500) valentic   (500)    26765 2023-07-06 02:17:26.000000 sapphire_config-1.0.1/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc
--rw-rw-r--   0 valentic   (500) valentic   (500)    15474 2023-07-05 19:42:10.000000 sapphire_config-1.0.1/tests/test_sapphireconfig.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1070 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/LICENSE
+-rw-rw-r--   0 valentic   (500) valentic   (500)       98 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/MANIFEST.in
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      199 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/README.md
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/examples/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/examples/components/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1042 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/examples/components/demo.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     2830 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/examples/components/demo.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/examples/config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      982 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/examples/config/demo.conf
+-rwxrwxr-x   0 valentic   (500) valentic   (500)     4932 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/examples/config/demo.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)      996 2023-07-06 02:17:33.000000 sapphire_config-1.0.2/pyproject.toml
+-rw-rw-r--   0 valentic   (500) valentic   (500)       38 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/setup.cfg
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config/
+-rw-rw-r--   0 valentic   (500) valentic   (500)      251 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/src/sapphire_config/__init__.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     5139 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/src/sapphire_config/component.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)       46 2023-07-17 22:41:43.000000 sapphire_config-1.0.2/src/sapphire_config/metadata.py
+-rw-rw-r--   0 valentic   (500) valentic   (500)     9320 2023-07-17 22:43:44.000000 sapphire_config-1.0.2/src/sapphire_config/parser.py
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/
+-rw-rw-r--   0 valentic   (500) valentic   (500)     1920 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/PKG-INFO
+-rw-rw-r--   0 valentic   (500) valentic   (500)      588 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)        1 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       92 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/requires.txt
+-rw-rw-r--   0 valentic   (500) valentic   (500)       16 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/src/sapphire_config.egg-info/top_level.txt
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/tests/
+drwxrwxr-x   0 valentic   (500) valentic   (500)        0 2023-07-17 22:45:31.000000 sapphire_config-1.0.2/tests/__pycache__/
+-rw-rw-r--   0 valentic   (500) valentic   (500)    26765 2023-07-06 02:17:26.000000 sapphire_config-1.0.2/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc
+-rw-rw-r--   0 valentic   (500) valentic   (500)    15474 2023-07-05 19:42:10.000000 sapphire_config-1.0.2/tests/test_sapphireconfig.py
```

### Comparing `sapphire_config-1.0.1/LICENSE` & `sapphire_config-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.1/PKG-INFO` & `sapphire_config-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapphire_config
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sapphire Configuration Parser
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Todd Valentic
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sapphire_config-1.0.1/examples/components/demo.conf` & `sapphire_config-1.0.2/examples/components/demo.conf`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.1/examples/components/demo.py` & `sapphire_config-1.0.2/examples/components/demo.py`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.1/examples/config/demo.conf` & `sapphire_config-1.0.2/examples/config/demo.conf`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.1/examples/config/demo.py` & `sapphire_config-1.0.2/examples/config/demo.py`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.1/pyproject.toml` & `sapphire_config-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.1/src/sapphire_config/component.py` & `sapphire_config-1.0.2/src/sapphire_config/component.py`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.1/src/sapphire_config/parser.py` & `sapphire_config-1.0.2/src/sapphire_config/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 #
 #   2020-12-24  Todd Valentic
 #               Initial implementation
 #
 #   2023-06-17  Todd Valentic
 #               PEP8 compliance
 #
+#   2023-07-17  Todd Valentic
+#               Change Rate offset default to 0 from None
+#
 ##########################################################################
 
 import configparser as cp
 import datetime
 import importlib
 import pathlib
 import re
@@ -30,22 +33,23 @@
 #   Types
 # -------------------------------------------------------------------------
 
 # pylint: disable=protected-access
 
 UNSET = cp._UNSET
 
+
 class Rate:
     """Repeating event specification"""
 
     def __init__(
         self,
         period: datetime.timedelta,
         sync: bool = False,
-        offset: datetime.timedelta = None,
+        offset: datetime.timedelta = 0,
         at_start: bool = False,
     ):
         self.period = period
         self.sync = sync
         self.offset = offset
         self.at_start = at_start
 
@@ -192,15 +196,15 @@
                         option, section, rawval, key
                     ) from None
                 value = value.replace(key, v)
 
         if "%(" in value:
             raise cp.InterpolationDepthError(option, section, rawval)
 
-        value = value.replace('%%', '%')
+        value = value.replace("%%", "%")
 
         return value
 
 
 # -------------------------------------------------------------------------
 #   Sapphire Config Parser
 # -------------------------------------------------------------------------
@@ -283,15 +287,15 @@
             period = fallback.period
             sync = fallback.sync
             offset = fallback.offset
             at_start = fallback.at_start
         else:
             period = fallback
             sync = False
-            offset = None
+            offset = 0
             at_start = False
 
         proxy = self[section]
         period = proxy.get_timedelta(option, fallback=period, **kw)
         period = proxy.get_timedelta(f"{option}.period", fallback=period, **kw)
 
         if period is None:
```

### Comparing `sapphire_config-1.0.1/src/sapphire_config.egg-info/PKG-INFO` & `sapphire_config-1.0.2/src/sapphire_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapphire-config
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sapphire Configuration Parser
 Author-email: Todd Valentic <todd.valentic@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Todd Valentic
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sapphire_config-1.0.1/src/sapphire_config.egg-info/SOURCES.txt` & `sapphire_config-1.0.2/src/sapphire_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.1/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc` & `sapphire_config-1.0.2/tests/__pycache__/test_sapphireconfig.cpython-39-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `sapphire_config-1.0.1/tests/test_sapphireconfig.py` & `sapphire_config-1.0.2/tests/test_sapphireconfig.py`

 * *Files identical despite different names*

