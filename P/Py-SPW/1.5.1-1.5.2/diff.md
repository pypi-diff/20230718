# Comparing `tmp/Py-SPW-1.5.1.tar.gz` & `tmp/Py-SPW-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Py-SPW-1.5.1.tar", last modified: Thu Jul 13 13:50:07 2023, max compression
+gzip compressed data, was "Py-SPW-1.5.2.tar", last modified: Mon Jul 17 23:26:22 2023, max compression
```

## Comparing `Py-SPW-1.5.1.tar` & `Py-SPW-1.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/
--rwxrwxr-x   0 stepan    (1000) stepan    (1000)     1085 2023-05-09 10:37:44.000000 Py-SPW-1.5.1/LICENSE
--rw-r--r--   0 stepan    (1000) stepan    (1000)       58 2023-07-13 13:18:30.000000 Py-SPW-1.5.1/MANIFEST.in
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1355 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/PKG-INFO
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/Py_SPW.egg-info/
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1355 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/PKG-INFO
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      285 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/SOURCES.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)        1 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/dependency_links.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       86 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/requires.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)        6 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/top_level.txt
--rw-r--r--   0 stepan    (1000) stepan    (1000)      945 2023-05-09 10:37:44.000000 Py-SPW-1.5.1/README.md
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/pyspw/
--rw-r--r--   0 stepan    (1000) stepan    (1000)     2661 2023-05-09 10:37:42.000000 Py-SPW-1.5.1/pyspw/Parameters.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)     3634 2023-05-09 10:37:42.000000 Py-SPW-1.5.1/pyspw/User.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)       19 2023-07-13 13:19:16.000000 Py-SPW-1.5.1/pyspw/__init__.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)     9956 2023-05-09 10:37:42.000000 Py-SPW-1.5.1/pyspw/api.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)     1728 2023-05-09 10:37:41.000000 Py-SPW-1.5.1/pyspw/errors.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)       85 2023-05-09 10:37:41.000000 Py-SPW-1.5.1/requirements.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       38 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/setup.cfg
--rw-r--r--   0 stepan    (1000) stepan    (1000)      826 2023-07-13 13:50:06.000000 Py-SPW-1.5.1/setup.py
+drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-17 23:26:22.614263 Py-SPW-1.5.2/
+-rwxrwxr-x   0 stepan    (1000) stepan    (1000)     1085 2023-05-09 10:37:44.000000 Py-SPW-1.5.2/LICENSE
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       58 2023-07-13 13:18:30.000000 Py-SPW-1.5.2/MANIFEST.in
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)     1355 2023-07-17 23:26:22.614263 Py-SPW-1.5.2/PKG-INFO
+drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-17 23:26:22.613263 Py-SPW-1.5.2/Py_SPW.egg-info/
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)     1355 2023-07-17 23:26:22.000000 Py-SPW-1.5.2/Py_SPW.egg-info/PKG-INFO
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)      285 2023-07-17 23:26:22.000000 Py-SPW-1.5.2/Py_SPW.egg-info/SOURCES.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)        1 2023-07-17 23:26:22.000000 Py-SPW-1.5.2/Py_SPW.egg-info/dependency_links.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)       86 2023-07-17 23:26:22.000000 Py-SPW-1.5.2/Py_SPW.egg-info/requires.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)        6 2023-07-17 23:26:22.000000 Py-SPW-1.5.2/Py_SPW.egg-info/top_level.txt
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      945 2023-05-09 10:37:44.000000 Py-SPW-1.5.2/README.md
+drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-17 23:26:22.614263 Py-SPW-1.5.2/pyspw/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     2661 2023-05-09 10:37:42.000000 Py-SPW-1.5.2/pyspw/Parameters.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     3634 2023-05-09 10:37:42.000000 Py-SPW-1.5.2/pyspw/User.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       42 2023-07-17 23:26:20.000000 Py-SPW-1.5.2/pyspw/__init__.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     9976 2023-07-17 21:58:25.000000 Py-SPW-1.5.2/pyspw/api.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1728 2023-05-09 10:37:41.000000 Py-SPW-1.5.2/pyspw/errors.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       85 2023-05-09 10:37:41.000000 Py-SPW-1.5.2/requirements.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)       38 2023-07-17 23:26:22.614263 Py-SPW-1.5.2/setup.cfg
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      970 2023-07-17 23:26:07.000000 Py-SPW-1.5.2/setup.py
```

### Comparing `Py-SPW-1.5.1/LICENSE` & `Py-SPW-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.1/PKG-INFO` & `Py-SPW-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Py-SPW
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python library for spworlds API
 Home-page: https://github.com/teleportx/Py-SPW
 Author: Stepan Khozhempo
 Author-email: stepan@xstl.ru
 License: MIT License
 Project-URL: Docs, https://pyspw.xstl.ru/en/latest/
 Project-URL: GitHub, https://github.com/teleport2/Py-SPW/
```

### Comparing `Py-SPW-1.5.1/Py_SPW.egg-info/PKG-INFO` & `Py-SPW-1.5.2/Py_SPW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Py-SPW
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python library for spworlds API
 Home-page: https://github.com/teleportx/Py-SPW
 Author: Stepan Khozhempo
 Author-email: stepan@xstl.ru
 License: MIT License
 Project-URL: Docs, https://pyspw.xstl.ru/en/latest/
 Project-URL: GitHub, https://github.com/teleport2/Py-SPW/
```

### Comparing `Py-SPW-1.5.1/README.md` & `Py-SPW-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.1/pyspw/Parameters.py` & `Py-SPW-1.5.2/pyspw/Parameters.py`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.1/pyspw/User.py` & `Py-SPW-1.5.2/pyspw/User.py`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.1/pyspw/api.py` & `Py-SPW-1.5.2/pyspw/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import platform
 from base64 import b64encode
 from dataclasses import dataclass
 from enum import Enum
 from hashlib import sha256
 import hmac
 import requests as rq
@@ -53,15 +54,18 @@
         }
         try:
             response = rq.request(method.value, url=self._spworlds_api_url + path, headers=headers, json=body)
 
         except rq.exceptions.ConnectionError as error:
             raise err.SpwApiError(error)
 
-        if response.headers.get('Content-Type') != 'application/json':
+        try:
+            response.json()
+
+        except json.JSONDecodeError:
             raise err.SpwApiDDOS()
 
         if response.ok or response.status_code in ignore_codes:
             return response
 
         elif response.status_code == 401:
             raise err.SpwUnauthorized()
```

### Comparing `Py-SPW-1.5.1/pyspw/errors.py` & `Py-SPW-1.5.2/pyspw/errors.py`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.1/setup.py` & `Py-SPW-1.5.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 this_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     description_md = f.read()
 
 requirements = open('requirements.txt', 'r').read().split('\n')
 
+exec(sorted([el if el.startswith('__version__') else 'Z' for el in open('./pyspw/__init__.py', 'r').read().split('\n')], reverse=True)[0])
+
 setup(
     name='Py-SPW',
-    version='1.5.1',
+    version=__version__,
     packages=['pyspw'],
     url='https://github.com/teleportx/Py-SPW',
     license='MIT License',
     author='Stepan Khozhempo',
     author_email='stepan@xstl.ru',
     description='Python library for spworlds API',
     long_description=description_md,
```

