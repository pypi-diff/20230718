# Comparing `tmp/real-brasileiro-0.2.5.tar.gz` & `tmp/real-brasileiro-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real-brasileiro-0.2.5.tar", last modified: Tue Jul 18 03:56:51 2023, max compression
+gzip compressed data, was "real-brasileiro-0.2.7.tar", last modified: Tue Jul 18 04:02:07 2023, max compression
```

## Comparing `real-brasileiro-0.2.5.tar` & `real-brasileiro-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1073 2023-07-18 03:36:07.000000 real-brasileiro-0.2.5/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      966 2023-07-18 03:51:31.000000 real-brasileiro-0.2.5/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/real_br/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       32 2023-07-18 03:36:07.000000 real-brasileiro-0.2.5/real_br/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4501 2023-07-18 03:51:31.000000 real-brasileiro-0.2.5/real_br/real_br.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/real_brasileiro.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 03:56:51.000000 real-brasileiro-0.2.5/real_brasileiro.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      221 2023-07-18 03:56:51.000000 real-brasileiro-0.2.5/real_brasileiro.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-18 03:56:51.000000 real-brasileiro-0.2.5/real_brasileiro.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-07-18 03:56:51.000000 real-brasileiro-0.2.5/real_brasileiro.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-18 03:56:51.923476 real-brasileiro-0.2.5/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      403 2023-07-18 03:56:48.000000 real-brasileiro-0.2.5/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 04:02:07.173477 real-brasileiro-0.2.7/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1073 2023-07-18 03:36:07.000000 real-brasileiro-0.2.7/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 04:02:07.173477 real-brasileiro-0.2.7/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      966 2023-07-18 03:51:31.000000 real-brasileiro-0.2.7/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 04:02:07.163477 real-brasileiro-0.2.7/real_br/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       32 2023-07-18 03:36:07.000000 real-brasileiro-0.2.7/real_br/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4488 2023-07-18 04:01:49.000000 real-brasileiro-0.2.7/real_br/real_br.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 04:02:07.173477 real-brasileiro-0.2.7/real_brasileiro.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1270 2023-07-18 04:02:07.000000 real-brasileiro-0.2.7/real_brasileiro.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      221 2023-07-18 04:02:07.000000 real-brasileiro-0.2.7/real_brasileiro.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-18 04:02:07.000000 real-brasileiro-0.2.7/real_brasileiro.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        8 2023-07-18 04:02:07.000000 real-brasileiro-0.2.7/real_brasileiro.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-18 04:02:07.173477 real-brasileiro-0.2.7/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      403 2023-07-18 04:02:06.000000 real-brasileiro-0.2.7/setup.py
```

### Comparing `real-brasileiro-0.2.5/LICENSE` & `real-brasileiro-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `real-brasileiro-0.2.5/PKG-INFO` & `real-brasileiro-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real-brasileiro
-Version: 0.2.5
+Version: 0.2.7
 Summary: UNKNOWN
 Home-page: https://github.com/MikalROn/Real_br
 Author: Daniel Coêlho
 Author-email: heromon.9010@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `real-brasileiro-0.2.5/README.md` & `real-brasileiro-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `real-brasileiro-0.2.5/real_br/real_br.py` & `real-brasileiro-0.2.7/real_br/real_br.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     # <>
 
     def __str__(self):
         return self.reais
 
     def __float__(self):
-        return float(f'{self._sinal}{self.centavos / 100}')
+        return float(f'{self.centavos / 100}')
 
     def __int__(self):
         return self.centavos
 
     # Operações
 
     def __add__(self, other: object) -> object:
```

### Comparing `real-brasileiro-0.2.5/real_brasileiro.egg-info/PKG-INFO` & `real-brasileiro-0.2.7/real_brasileiro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real-brasileiro
-Version: 0.2.5
+Version: 0.2.7
 Summary: UNKNOWN
 Home-page: https://github.com/MikalROn/Real_br
 Author: Daniel Coêlho
 Author-email: heromon.9010@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3
```

