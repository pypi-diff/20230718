# Comparing `tmp/robocorp-0.8.0.tar.gz` & `tmp/robocorp-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp-0.8.0.tar", max compression
+gzip compressed data, was "robocorp-0.8.1.tar", max compression
```

## Comparing `robocorp-0.8.0.tar` & `robocorp-0.8.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      599 2023-07-14 16:12:45.874605 robocorp-0.8.0/README.md
--rw-r--r--   0        0        0      776 2023-07-14 16:12:45.874605 robocorp-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-07-14 16:12:45.874605 robocorp-0.8.0/src/robocorp/_meta/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 16:12:45.874605 robocorp-0.8.0/src/robocorp/_meta/py.typed
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 robocorp-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      599 2023-07-18 11:54:37.083345 robocorp-0.8.1/README.md
+-rw-r--r--   0        0        0      776 2023-07-18 11:54:37.083345 robocorp-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-18 11:54:37.087345 robocorp-0.8.1/src/robocorp/_meta/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:54:37.087345 robocorp-0.8.1/src/robocorp/_meta/py.typed
+-rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 robocorp-0.8.1/PKG-INFO
```

### Comparing `robocorp-0.8.0/README.md` & `robocorp-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `robocorp-0.8.0/pyproject.toml` & `robocorp-0.8.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp"
-version = "0.8.0"
+version = "0.8.1"
 description = "Robocorp core libraries for Python automation"
 authors = [
 	"Ossi Rajuvaara <ossi@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
 license = "Apache-2.0"
@@ -12,15 +12,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 robocorp-tasks = "2.1.2"
 robocorp-log = "2.3.0"
 robocorp-workitems = "1.2.1"
 robocorp-vault = "1.2.0"
-robocorp-storage = "0.3.0"
+robocorp-storage = "0.3.1"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [tool.black]
 skip-string-normalization = false
 skip-magic-trailing-comma = false
```

### Comparing `robocorp-0.8.0/PKG-INFO` & `robocorp-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: robocorp
-Version: 0.8.0
+Version: 0.8.1
 Summary: Robocorp core libraries for Python automation
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Ossi Rajuvaara
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: robocorp-log (==2.3.0)
-Requires-Dist: robocorp-storage (==0.3.0)
+Requires-Dist: robocorp-storage (==0.3.1)
 Requires-Dist: robocorp-tasks (==2.1.2)
 Requires-Dist: robocorp-vault (==1.2.0)
 Requires-Dist: robocorp-workitems (==1.2.1)
 Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
 # robocorp (metapackage)
```

