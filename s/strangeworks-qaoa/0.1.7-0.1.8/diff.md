# Comparing `tmp/strangeworks_qaoa-0.1.7.tar.gz` & `tmp/strangeworks_qaoa-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qaoa-0.1.7.tar", max compression
+gzip compressed data, was "strangeworks_qaoa-0.1.8.tar", max compression
```

## Comparing `strangeworks_qaoa-0.1.7.tar` & `strangeworks_qaoa-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-06-14 14:07:05.162877 strangeworks_qaoa-0.1.7/LICENSE
--rw-r--r--   0        0        0      679 2023-06-14 14:07:05.162877 strangeworks_qaoa-0.1.7/README.md
--rw-r--r--   0        0        0      791 2023-06-14 14:07:18.331063 strangeworks_qaoa-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      194 2023-06-14 14:07:05.162877 strangeworks_qaoa-0.1.7/strangeworks_qaoa/__init__.py
--rw-r--r--   0        0        0    17637 2023-06-14 14:07:05.162877 strangeworks_qaoa-0.1.7/strangeworks_qaoa/sdk.py
--rw-r--r--   0        0        0      691 2023-06-14 14:07:05.162877 strangeworks_qaoa-0.1.7/strangeworks_qaoa/serializer.py
--rw-r--r--   0        0        0    12428 2023-06-14 14:07:05.162877 strangeworks_qaoa-0.1.7/strangeworks_qaoa/utils.py
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/LICENSE
+-rw-r--r--   0        0        0      679 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/README.md
+-rw-r--r--   0        0        0      791 2023-07-18 10:42:11.867814 strangeworks_qaoa-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/strangeworks_qaoa/__init__.py
+-rw-r--r--   0        0        0    17638 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/strangeworks_qaoa/sdk.py
+-rw-r--r--   0        0        0      691 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/strangeworks_qaoa/serializer.py
+-rw-r--r--   0        0        0    12428 2023-07-18 10:41:55.939644 strangeworks_qaoa-0.1.8/strangeworks_qaoa/utils.py
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.8/PKG-INFO
```

### Comparing `strangeworks_qaoa-0.1.7/LICENSE` & `strangeworks_qaoa-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.7/README.md` & `strangeworks_qaoa-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.7/pyproject.toml` & `strangeworks_qaoa-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "strangeworks-qaoa"
-version = "0.1.7"
+version = "0.1.8"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qaoa"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 networkx = "^3.0"
 numpy = "1.23.2"
 qiskit = "^0.41.0"
-strangeworks = "^0.4.0"
+strangeworks = "^0.4.4"
 dimod = "^0.12.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "22.10.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.2.1"
```

### Comparing `strangeworks_qaoa-0.1.7/strangeworks_qaoa/sdk.py` & `strangeworks_qaoa-0.1.8/strangeworks_qaoa/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,15 @@
         """
 
         if self.backend_list == " ":
             self.backends()
 
         aws = False
         ibm = False
+
         for nn in range(len(self.backend_list["AWS"])):
             if (
                 self.backend_list["AWS"][nn]["name"] == backend
                 or self.backend_list["AWS"][nn]["arn"] == backend
             ):
                 aws = True
                 backend_id = self.backend_list["AWS"][nn]["arn"]
```

### Comparing `strangeworks_qaoa-0.1.7/strangeworks_qaoa/serializer.py` & `strangeworks_qaoa-0.1.8/strangeworks_qaoa/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.7/strangeworks_qaoa/utils.py` & `strangeworks_qaoa-0.1.8/strangeworks_qaoa/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.7/PKG-INFO` & `strangeworks_qaoa-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strangeworks-qaoa
-Version: 0.1.7
+Version: 0.1.8
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dimod (>=0.12.4,<0.13.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (==1.23.2)
 Requires-Dist: qiskit (>=0.41.0,<0.42.0)
-Requires-Dist: strangeworks (>=0.4.0,<0.5.0)
+Requires-Dist: strangeworks (>=0.4.4,<0.5.0)
 Description-Content-Type: text/markdown
 
 ![Tests](https://github.com/strangeworks/strangeworks-qaoa/actions/workflows/cron_test.yml/badge.svg)
 
 # Strangeworks QAOA SDK Extension
 
 This extension provides access to the Strangeworks QAOA service through the SDK.
```

