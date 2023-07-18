# Comparing `tmp/flask_pypprof-0.1.13.tar.gz` & `tmp/flask_pypprof-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_pypprof-0.1.13.tar", max compression
+gzip compressed data, was "flask_pypprof-0.1.14.tar", max compression
```

## Comparing `flask_pypprof-0.1.13.tar` & `flask_pypprof-0.1.14.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/LICENSE
--rw-r--r--   0        0        0     1788 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/README.md
--rw-r--r--   0        0        0      141 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/flask_pypprof/__init__.py
--rw-r--r--   0        0        0     1408 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/flask_pypprof/handler.py
--rw-r--r--   0        0        0     1919 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/flask_pypprof/routes.py
--rw-r--r--   0        0        0      481 2023-07-17 19:12:30.995417 flask_pypprof-0.1.13/pyproject.toml
--rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 flask_pypprof-0.1.13/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/LICENSE
+-rw-r--r--   0        0        0     1788 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/README.md
+-rw-r--r--   0        0        0      333 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/flask_pypprof/__init__.py
+-rw-r--r--   0        0        0     1408 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/flask_pypprof/handler.py
+-rw-r--r--   0        0        0     1125 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/flask_pypprof/noop_routes.py
+-rw-r--r--   0        0        0     1919 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/flask_pypprof/routes.py
+-rw-r--r--   0        0        0      652 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/pyproject.toml
+-rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 flask_pypprof-0.1.14/PKG-INFO
```

### Comparing `flask_pypprof-0.1.13/LICENSE` & `flask_pypprof-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.13/README.md` & `flask_pypprof-0.1.14/README.md`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.13/flask_pypprof/handler.py` & `flask_pypprof-0.1.14/flask_pypprof/handler.py`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.13/flask_pypprof/routes.py` & `flask_pypprof-0.1.14/flask_pypprof/routes.py`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.13/PKG-INFO` & `flask_pypprof-0.1.14/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flask-pypprof
-Version: 0.1.13
+Version: 0.1.14
 Summary: Pypprof Flask wrapper
 Author: Diego
 Author-email: diegolparra@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: flask (>=2.3.2,<3.0.0)
-Requires-Dist: mprofile (==0.0.15)
-Requires-Dist: protobuf (>=3.20,<4.0)
-Requires-Dist: pypprof (==0.0.1)
-Requires-Dist: zprofile (==1.0.12)
+Requires-Dist: mprofile (==0.0.15) ; sys_platform == "linux"
+Requires-Dist: protobuf (>=3.20,<4.0) ; sys_platform == "linux"
+Requires-Dist: pypprof (==0.0.1) ; sys_platform == "linux"
+Requires-Dist: zprofile (==1.0.12) ; sys_platform == "linux"
 Description-Content-Type: text/markdown
 
 # flask-pypprof
 
 Blueprint for pprof profiling endpoints a la GO's that can be added to python Flask applications. *flask-pypprof* is a wrapper of [pypprof] and based on [django-pypprof] ideas.
 
 ## Installation
```

