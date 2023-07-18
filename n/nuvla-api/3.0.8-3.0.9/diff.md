# Comparing `tmp/nuvla-api-3.0.8.tar.gz` & `tmp/nuvla-api-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvla-api-3.0.8.tar", last modified: Tue May 10 14:17:17 2022, max compression
+gzip compressed data, was "nuvla-api-3.0.9.tar", last modified: Tue Jul 18 09:44:23 2023, max compression
```

## Comparing `nuvla-api-3.0.8.tar` & `nuvla-api-3.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 khaledbasbous   (501) staff       (20)        0 2022-05-10 14:17:17.311210 nuvla-api-3.0.8/
--rw-r--r--   0 khaledbasbous   (501) staff       (20)       26 2022-03-08 13:29:46.000000 nuvla-api-3.0.8/MANIFEST.in
--rw-r--r--   0 khaledbasbous   (501) staff       (20)      968 2022-05-10 14:17:17.311274 nuvla-api-3.0.8/PKG-INFO
--rw-r--r--   0 khaledbasbous   (501) staff       (20)       86 2022-05-10 12:59:59.000000 nuvla-api-3.0.8/pyproject.toml
--rw-r--r--   0 khaledbasbous   (501) staff       (20)       30 2022-03-21 07:21:56.000000 nuvla-api-3.0.8/requirements.txt
--rw-r--r--   0 khaledbasbous   (501) staff       (20)       67 2022-05-10 14:17:17.311458 nuvla-api-3.0.8/setup.cfg
--rwxr-xr-x   0 khaledbasbous   (501) staff       (20)     1443 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/setup.py
-drwxr-xr-x   0 khaledbasbous   (501) staff       (20)        0 2022-05-10 14:17:17.308030 nuvla-api-3.0.8/src/
-drwxr-xr-x   0 khaledbasbous   (501) staff       (20)        0 2022-05-10 14:17:17.308612 nuvla-api-3.0.8/src/nuvla/
--rw-r--r--   0 khaledbasbous   (501) staff       (20)       81 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/__init__.py
-drwxr-xr-x   0 khaledbasbous   (501) staff       (20)        0 2022-05-10 14:17:17.308957 nuvla-api-3.0.8/src/nuvla/api/
--rw-r--r--   0 khaledbasbous   (501) staff       (20)      112 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/__init__.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)    24118 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/api.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)     2406 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/models.py
-drwxr-xr-x   0 khaledbasbous   (501) staff       (20)        0 2022-05-10 14:17:17.310132 nuvla-api-3.0.8/src/nuvla/api/resources/
--rw-r--r--   0 khaledbasbous   (501) staff       (20)      222 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/__init__.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)     2351 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/base.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)      734 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/callback.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)     6410 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/credential.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)     3777 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/data.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)    19472 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/deployment.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)     1624 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/deployment_parameter.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)     2942 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/infra_service.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)     7345 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/module.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)     1421 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/notification.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)     1190 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/resources/user.py
-drwxr-xr-x   0 khaledbasbous   (501) staff       (20)        0 2022-05-10 14:17:17.310434 nuvla-api-3.0.8/src/nuvla/api/util/
--rw-r--r--   0 khaledbasbous   (501) staff       (20)       24 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/util/__init__.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)      731 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/util/date.py
--rw-r--r--   0 khaledbasbous   (501) staff       (20)      688 2022-05-10 14:17:12.000000 nuvla-api-3.0.8/src/nuvla/api/util/filter.py
-drwxr-xr-x   0 khaledbasbous   (501) staff       (20)        0 2022-05-10 14:17:17.311100 nuvla-api-3.0.8/src/nuvla_api.egg-info/
--rw-r--r--   0 khaledbasbous   (501) staff       (20)      968 2022-05-10 14:17:17.000000 nuvla-api-3.0.8/src/nuvla_api.egg-info/PKG-INFO
--rw-r--r--   0 khaledbasbous   (501) staff       (20)      915 2022-05-10 14:17:17.000000 nuvla-api-3.0.8/src/nuvla_api.egg-info/SOURCES.txt
--rw-r--r--   0 khaledbasbous   (501) staff       (20)        1 2022-05-10 14:17:17.000000 nuvla-api-3.0.8/src/nuvla_api.egg-info/dependency_links.txt
--rw-r--r--   0 khaledbasbous   (501) staff       (20)        6 2022-05-10 14:17:17.000000 nuvla-api-3.0.8/src/nuvla_api.egg-info/namespace_packages.txt
--rw-r--r--   0 khaledbasbous   (501) staff       (20)        1 2022-05-10 14:17:16.000000 nuvla-api-3.0.8/src/nuvla_api.egg-info/not-zip-safe
--rw-r--r--   0 khaledbasbous   (501) staff       (20)       29 2022-05-10 14:17:17.000000 nuvla-api-3.0.8/src/nuvla_api.egg-info/requires.txt
--rw-r--r--   0 khaledbasbous   (501) staff       (20)        6 2022-05-10 14:17:17.000000 nuvla-api-3.0.8/src/nuvla_api.egg-info/top_level.txt
+drwxr-xr-x   0 lionel     (501) staff       (20)        0 2023-07-18 09:44:23.320388 nuvla-api-3.0.9/
+-rw-r--r--   0 lionel     (501) staff       (20)       26 2021-12-14 10:54:10.000000 nuvla-api-3.0.9/MANIFEST.in
+-rw-r--r--   0 lionel     (501) staff       (20)      940 2023-07-18 09:44:23.320491 nuvla-api-3.0.9/PKG-INFO
+-rw-r--r--   0 lionel     (501) staff       (20)       86 2023-07-18 09:24:29.000000 nuvla-api-3.0.9/pyproject.toml
+-rw-r--r--   0 lionel     (501) staff       (20)       32 2023-07-18 09:24:29.000000 nuvla-api-3.0.9/requirements.txt
+-rw-r--r--   0 lionel     (501) staff       (20)       67 2023-07-18 09:44:23.320821 nuvla-api-3.0.9/setup.cfg
+-rwxr-xr-x   0 lionel     (501) staff       (20)     1443 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/setup.py
+drwxr-xr-x   0 lionel     (501) staff       (20)        0 2023-07-18 09:44:23.312000 nuvla-api-3.0.9/src/
+drwxr-xr-x   0 lionel     (501) staff       (20)        0 2023-07-18 09:44:23.316481 nuvla-api-3.0.9/src/nuvla/
+-rw-r--r--   0 lionel     (501) staff       (20)       81 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/__init__.py
+drwxr-xr-x   0 lionel     (501) staff       (20)        0 2023-07-18 09:44:23.317102 nuvla-api-3.0.9/src/nuvla/api/
+-rw-r--r--   0 lionel     (501) staff       (20)      112 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/__init__.py
+-rw-r--r--   0 lionel     (501) staff       (20)    24118 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/api.py
+-rw-r--r--   0 lionel     (501) staff       (20)     2406 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/models.py
+drwxr-xr-x   0 lionel     (501) staff       (20)        0 2023-07-18 09:44:23.318879 nuvla-api-3.0.9/src/nuvla/api/resources/
+-rw-r--r--   0 lionel     (501) staff       (20)      222 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/__init__.py
+-rw-r--r--   0 lionel     (501) staff       (20)     2351 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/base.py
+-rw-r--r--   0 lionel     (501) staff       (20)      734 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/callback.py
+-rw-r--r--   0 lionel     (501) staff       (20)     6410 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/credential.py
+-rw-r--r--   0 lionel     (501) staff       (20)     3777 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/data.py
+-rw-r--r--   0 lionel     (501) staff       (20)    19472 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/deployment.py
+-rw-r--r--   0 lionel     (501) staff       (20)     1624 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/deployment_parameter.py
+-rw-r--r--   0 lionel     (501) staff       (20)     2942 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/infra_service.py
+-rw-r--r--   0 lionel     (501) staff       (20)     7345 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/module.py
+-rw-r--r--   0 lionel     (501) staff       (20)     1421 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/notification.py
+-rw-r--r--   0 lionel     (501) staff       (20)     1190 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/resources/user.py
+drwxr-xr-x   0 lionel     (501) staff       (20)        0 2023-07-18 09:44:23.319291 nuvla-api-3.0.9/src/nuvla/api/util/
+-rw-r--r--   0 lionel     (501) staff       (20)       24 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/util/__init__.py
+-rw-r--r--   0 lionel     (501) staff       (20)      731 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/util/date.py
+-rw-r--r--   0 lionel     (501) staff       (20)      688 2023-07-18 09:44:19.000000 nuvla-api-3.0.9/src/nuvla/api/util/filter.py
+drwxr-xr-x   0 lionel     (501) staff       (20)        0 2023-07-18 09:44:23.320258 nuvla-api-3.0.9/src/nuvla_api.egg-info/
+-rw-r--r--   0 lionel     (501) staff       (20)      940 2023-07-18 09:44:23.000000 nuvla-api-3.0.9/src/nuvla_api.egg-info/PKG-INFO
+-rw-r--r--   0 lionel     (501) staff       (20)      915 2023-07-18 09:44:23.000000 nuvla-api-3.0.9/src/nuvla_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lionel     (501) staff       (20)        1 2023-07-18 09:44:23.000000 nuvla-api-3.0.9/src/nuvla_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lionel     (501) staff       (20)        6 2023-07-18 09:44:23.000000 nuvla-api-3.0.9/src/nuvla_api.egg-info/namespace_packages.txt
+-rw-r--r--   0 lionel     (501) staff       (20)        1 2023-07-18 09:44:23.000000 nuvla-api-3.0.9/src/nuvla_api.egg-info/not-zip-safe
+-rw-r--r--   0 lionel     (501) staff       (20)       31 2023-07-18 09:44:23.000000 nuvla-api-3.0.9/src/nuvla_api.egg-info/requires.txt
+-rw-r--r--   0 lionel     (501) staff       (20)        6 2023-07-18 09:44:23.000000 nuvla-api-3.0.9/src/nuvla_api.egg-info/top_level.txt
```

### Comparing `nuvla-api-3.0.8/PKG-INFO` & `nuvla-api-3.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: nuvla-api
-Version: 3.0.8
+Version: 3.0.9
 Summary: A wrapper to use Nuvla from Python programs.
 Home-page: https://sixsq.com/nuvla
 Author: SixSq SA
 Author-email: support@sixsq.com
 License: Apache License, Version 2.0
 Keywords: nuvla devops api
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
-
-UNKNOWN
-
```

### Comparing `nuvla-api-3.0.8/setup.py` & `nuvla-api-3.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('requirements.txt') as f:
     install_requires = []
     for line in f.readlines():
         if not line.startswith('mock'):
             install_requires.append(line)
 
-version = '3.0.8'
+version = '3.0.9'
 
 setup(
     name='nuvla-api',
     version=version,
     author="SixSq SA",
     author_email='support@sixsq.com',
     url='https://sixsq.com/nuvla',
```

### Comparing `nuvla-api-3.0.8/src/nuvla/api/api.py` & `nuvla-api-3.0.9/src/nuvla/api/api.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/models.py` & `nuvla-api-3.0.9/src/nuvla/api/models.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/base.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/base.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/callback.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/callback.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/credential.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/credential.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/data.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/data.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/deployment.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/deployment_parameter.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/deployment_parameter.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/infra_service.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/infra_service.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/module.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/module.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/notification.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/notification.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/resources/user.py` & `nuvla-api-3.0.9/src/nuvla/api/resources/user.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/util/date.py` & `nuvla-api-3.0.9/src/nuvla/api/util/date.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla/api/util/filter.py` & `nuvla-api-3.0.9/src/nuvla/api/util/filter.py`

 * *Files identical despite different names*

### Comparing `nuvla-api-3.0.8/src/nuvla_api.egg-info/PKG-INFO` & `nuvla-api-3.0.9/src/nuvla_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: nuvla-api
-Version: 3.0.8
+Version: 3.0.9
 Summary: A wrapper to use Nuvla from Python programs.
 Home-page: https://sixsq.com/nuvla
 Author: SixSq SA
 Author-email: support@sixsq.com
 License: Apache License, Version 2.0
 Keywords: nuvla devops api
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
-
-UNKNOWN
-
```

### Comparing `nuvla-api-3.0.8/src/nuvla_api.egg-info/SOURCES.txt` & `nuvla-api-3.0.9/src/nuvla_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

