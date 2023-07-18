# Comparing `tmp/flask_protobuf-0.1.1.tar.gz` & `tmp/flask_protobuf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_protobuf-0.1.1.tar", last modified: Mon Jul 17 23:58:09 2023, max compression
+gzip compressed data, was "flask_protobuf-0.1.2.tar", last modified: Mon Jul 17 23:59:15 2023, max compression
```

## Comparing `flask_protobuf-0.1.1.tar` & `flask_protobuf-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-17 23:58:09.700968 flask_protobuf-0.1.1/
--rw-r--r--   0 jgutierrez   (503) staff       (20)     1068 2023-07-17 03:34:07.000000 flask_protobuf-0.1.1/LICENSE.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)      431 2023-07-17 23:58:09.701129 flask_protobuf-0.1.1/PKG-INFO
--rw-r--r--   0 jgutierrez   (503) staff       (20)     2819 2023-07-17 23:58:05.000000 flask_protobuf-0.1.1/README.md
-drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-17 23:58:09.696711 flask_protobuf-0.1.1/flask_protobuf/
--rw-r--r--   0 jgutierrez   (503) staff       (20)      136 2023-07-16 10:00:26.000000 flask_protobuf-0.1.1/flask_protobuf/__init__.py
--rw-r--r--   0 jgutierrez   (503) staff       (20)     6346 2023-07-17 23:29:04.000000 flask_protobuf-0.1.1/flask_protobuf/extension.py
-drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-17 23:58:09.700524 flask_protobuf-0.1.1/flask_protobuf.egg-info/
--rw-r--r--   0 jgutierrez   (503) staff       (20)      431 2023-07-17 23:58:09.000000 flask_protobuf-0.1.1/flask_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 jgutierrez   (503) staff       (20)      284 2023-07-17 23:58:09.000000 flask_protobuf-0.1.1/flask_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)        1 2023-07-17 23:58:09.000000 flask_protobuf-0.1.1/flask_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)       30 2023-07-17 23:58:09.000000 flask_protobuf-0.1.1/flask_protobuf.egg-info/requires.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)       15 2023-07-17 23:58:09.000000 flask_protobuf-0.1.1/flask_protobuf.egg-info/top_level.txt
--rw-r--r--   0 jgutierrez   (503) staff       (20)       38 2023-07-17 23:58:09.701648 flask_protobuf-0.1.1/setup.cfg
--rw-r--r--   0 jgutierrez   (503) staff       (20)      587 2023-07-17 23:56:58.000000 flask_protobuf-0.1.1/setup.py
+drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-17 23:59:15.966436 flask_protobuf-0.1.2/
+-rw-r--r--   0 jgutierrez   (503) staff       (20)     1068 2023-07-17 03:34:07.000000 flask_protobuf-0.1.2/LICENSE.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      431 2023-07-17 23:59:15.966699 flask_protobuf-0.1.2/PKG-INFO
+-rw-r--r--   0 jgutierrez   (503) staff       (20)     2819 2023-07-17 23:58:05.000000 flask_protobuf-0.1.2/README.md
+drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-17 23:59:15.961335 flask_protobuf-0.1.2/flask_protobuf/
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      136 2023-07-16 10:00:26.000000 flask_protobuf-0.1.2/flask_protobuf/__init__.py
+-rw-r--r--   0 jgutierrez   (503) staff       (20)     6346 2023-07-17 23:29:04.000000 flask_protobuf-0.1.2/flask_protobuf/extension.py
+drwxr-xr-x   0 jgutierrez   (503) staff       (20)        0 2023-07-17 23:59:15.965532 flask_protobuf-0.1.2/flask_protobuf.egg-info/
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      431 2023-07-17 23:59:15.000000 flask_protobuf-0.1.2/flask_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      284 2023-07-17 23:59:15.000000 flask_protobuf-0.1.2/flask_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)        1 2023-07-17 23:59:15.000000 flask_protobuf-0.1.2/flask_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)       30 2023-07-17 23:59:15.000000 flask_protobuf-0.1.2/flask_protobuf.egg-info/requires.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)       15 2023-07-17 23:59:15.000000 flask_protobuf-0.1.2/flask_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 jgutierrez   (503) staff       (20)       79 2023-07-17 23:59:15.967690 flask_protobuf-0.1.2/setup.cfg
+-rw-r--r--   0 jgutierrez   (503) staff       (20)      587 2023-07-17 23:59:13.000000 flask_protobuf-0.1.2/setup.py
```

### Comparing `flask_protobuf-0.1.1/LICENSE.txt` & `flask_protobuf-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flask_protobuf-0.1.1/README.md` & `flask_protobuf-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_protobuf-0.1.1/flask_protobuf/extension.py` & `flask_protobuf-0.1.2/flask_protobuf/extension.py`

 * *Files identical despite different names*

### Comparing `flask_protobuf-0.1.1/setup.py` & `flask_protobuf-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='flask_protobuf',
     license='MIT',
-    version='0.1.1',
+    version='0.1.2',
     description='Flask-Protobuf is a Python package that provides integration between Flask and Protocol Buffers (protobuf). It allows you to easily handle incoming protobuf messages in your Flask application.',
     author='Jerick Gutierrez',
     packages=['flask_protobuf'],
     url='https://github.com/Mackhintoshi/Flask-Protobuf',
     keywords=['flask', 'protobuf', 'google', 'protocol buffers'],
     install_requires=[
         'Flask>=2.3.2',
```

