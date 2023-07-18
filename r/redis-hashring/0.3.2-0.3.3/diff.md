# Comparing `tmp/redis-hashring-0.3.2.tar.gz` & `tmp/redis-hashring-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/redis-hashring-0.3.2.tar", last modified: Thu Apr 15 19:31:05 2021, max compression
+gzip compressed data, was "redis-hashring-0.3.3.tar", last modified: Tue Jul 18 11:04:19 2023, max compression
```

## Comparing `redis-hashring-0.3.2.tar` & `redis-hashring-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 jpmelos   (1000) jpmelos   (1000)        0 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)       38 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/setup.cfg
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)      969 2021-04-15 19:30:26.000000 redis-hashring-0.3.2/setup.py
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)      809 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/PKG-INFO
-drwxrwxr-x   0 jpmelos   (1000) jpmelos   (1000)        0 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/redis_hashring/
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)    10900 2021-04-15 18:43:58.000000 redis-hashring-0.3.2/redis_hashring/__init__.py
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)     9992 2021-04-13 13:46:19.000000 redis-hashring-0.3.2/README.rst
-drwxrwxr-x   0 jpmelos   (1000) jpmelos   (1000)        0 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/redis_hashring.egg-info/
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)      235 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/redis_hashring.egg-info/SOURCES.txt
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)      809 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/redis_hashring.egg-info/PKG-INFO
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)        1 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/redis_hashring.egg-info/dependency_links.txt
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)       15 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/redis_hashring.egg-info/top_level.txt
--rw-rw-r--   0 jpmelos   (1000) jpmelos   (1000)       12 2021-04-15 19:31:05.000000 redis-hashring-0.3.2/redis_hashring.egg-info/requires.txt
+drwxr-xr-x   0 nsaje      (501) staff       (20)        0 2023-07-18 11:04:19.374493 redis-hashring-0.3.3/
+-rw-r--r--   0 nsaje      (501) staff       (20)     1089 2023-07-17 11:17:29.000000 redis-hashring-0.3.3/LICENSE
+-rw-r--r--   0 nsaje      (501) staff       (20)      810 2023-07-18 11:04:19.374374 redis-hashring-0.3.3/PKG-INFO
+-rw-r--r--   0 nsaje      (501) staff       (20)     9992 2023-07-17 11:17:29.000000 redis-hashring-0.3.3/README.rst
+drwxr-xr-x   0 nsaje      (501) staff       (20)        0 2023-07-18 11:04:19.373617 redis-hashring-0.3.3/redis_hashring/
+-rw-r--r--   0 nsaje      (501) staff       (20)    10900 2023-07-17 11:17:29.000000 redis-hashring-0.3.3/redis_hashring/__init__.py
+drwxr-xr-x   0 nsaje      (501) staff       (20)        0 2023-07-18 11:04:19.374220 redis-hashring-0.3.3/redis_hashring.egg-info/
+-rw-r--r--   0 nsaje      (501) staff       (20)      810 2023-07-18 11:04:19.000000 redis-hashring-0.3.3/redis_hashring.egg-info/PKG-INFO
+-rw-r--r--   0 nsaje      (501) staff       (20)      243 2023-07-18 11:04:19.000000 redis-hashring-0.3.3/redis_hashring.egg-info/SOURCES.txt
+-rw-r--r--   0 nsaje      (501) staff       (20)        1 2023-07-18 11:04:19.000000 redis-hashring-0.3.3/redis_hashring.egg-info/dependency_links.txt
+-rw-r--r--   0 nsaje      (501) staff       (20)       12 2023-07-18 11:04:19.000000 redis-hashring-0.3.3/redis_hashring.egg-info/requires.txt
+-rw-r--r--   0 nsaje      (501) staff       (20)       15 2023-07-18 11:04:19.000000 redis-hashring-0.3.3/redis_hashring.egg-info/top_level.txt
+-rw-r--r--   0 nsaje      (501) staff       (20)       38 2023-07-18 11:04:19.374537 redis-hashring-0.3.3/setup.cfg
+-rw-r--r--   0 nsaje      (501) staff       (20)      969 2023-07-18 11:00:18.000000 redis-hashring-0.3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `redis-hashring-0.3.2/setup.py` & `redis-hashring-0.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name='redis-hashring',
-    version='0.3.2',
+    version='0.3.3',
     author='Close Engineering',
     author_email='engineering@close.com',
     url='http://github.com/closeio/redis-hashring',
     license='MIT',
     description=(
         'Python library for distributed applications using a Redis hash ring'
     ),
-    install_requires=['redis>=3,<4'],
+    install_requires=['redis>=3,<5'],
     platforms='any',
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Programming Language :: Python',
```

### Comparing `redis-hashring-0.3.2/PKG-INFO` & `redis-hashring-0.3.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: redis-hashring
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python library for distributed applications using a Redis hash ring
 Home-page: http://github.com/closeio/redis-hashring
 Author: Close Engineering
 Author-email: engineering@close.com
 License: MIT
-Description: UNKNOWN
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
```

### Comparing `redis-hashring-0.3.2/redis_hashring/__init__.py` & `redis-hashring-0.3.3/redis_hashring/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-hashring-0.3.2/README.rst` & `redis-hashring-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `redis-hashring-0.3.2/redis_hashring.egg-info/PKG-INFO` & `redis-hashring-0.3.3/redis_hashring.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: redis-hashring
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python library for distributed applications using a Redis hash ring
 Home-page: http://github.com/closeio/redis-hashring
 Author: Close Engineering
 Author-email: engineering@close.com
 License: MIT
-Description: UNKNOWN
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
```

