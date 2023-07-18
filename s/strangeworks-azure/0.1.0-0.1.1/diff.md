# Comparing `tmp/strangeworks_azure-0.1.0.tar.gz` & `tmp/strangeworks_azure-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_azure-0.1.0.tar", max compression
+gzip compressed data, was "strangeworks_azure-0.1.1.tar", max compression
```

## Comparing `strangeworks_azure-0.1.0.tar` & `strangeworks_azure-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      723 2023-05-04 15:48:12.000423 strangeworks_azure-0.1.0/README.md
--rw-r--r--   0        0        0     1008 2023-05-04 15:48:27.212036 strangeworks_azure-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      230 2023-05-04 15:48:12.004411 strangeworks_azure-0.1.0/strangeworks_azure/__init__.py
--rw-r--r--   0        0        0     2814 2023-05-04 15:48:12.004411 strangeworks_azure-0.1.0/strangeworks_azure/backend.py
--rw-r--r--   0        0        0     8749 2023-05-04 15:48:12.004411 strangeworks_azure-0.1.0/strangeworks_azure/job.py
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 strangeworks_azure-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      827 2023-07-18 10:42:46.004773 strangeworks_azure-0.1.1/README.md
+-rw-r--r--   0        0        0     1001 2023-07-18 10:43:00.397106 strangeworks_azure-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      230 2023-07-18 10:42:46.008773 strangeworks_azure-0.1.1/strangeworks_azure/__init__.py
+-rw-r--r--   0        0        0     2815 2023-07-18 10:42:46.008773 strangeworks_azure-0.1.1/strangeworks_azure/backend.py
+-rw-r--r--   0        0        0     8749 2023-07-18 10:42:46.008773 strangeworks_azure-0.1.1/strangeworks_azure/job.py
+-rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 strangeworks_azure-0.1.1/PKG-INFO
```

### Comparing `strangeworks_azure-0.1.0/README.md` & `strangeworks_azure-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![Tests](https://github.com/strangeworks/strangeworks-azure/actions/workflows/cron_test.yml/badge.svg)
+
 # Strangeworks Azure Extension
 
 Strangeworks Python SDK extension for Azure.
 
 For more information on using the SDK check out the
 [Strangeworks documentation](https://docs.strangeworks.com/).
```

### Comparing `strangeworks_azure-0.1.0/pyproject.toml` & `strangeworks_azure-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "strangeworks-azure"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_azure"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 azure-quantum = {extras = ["qiskit"], version = "^0.28.263081"}
-strangeworks = "^0.4.1"
-strangeworks-python-core = "^0.1.6"
+strangeworks = "^0.4.4"
+strangeworks-core = "^0.2.3"
 pytest = "^7.3.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 pytest = "^7.0.1"
 Flake8-pyproject = "^1.1.0"
 mdformat = "^0.7.14"
```

### Comparing `strangeworks_azure-0.1.0/strangeworks_azure/backend.py` & `strangeworks_azure-0.1.1/strangeworks_azure/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         name: str,
         status: Optional[str] = None,
         slug: Optional[str] = None,
         **kwargs,
     ):
         self.name = name
         self.slug = slug
+
         self.status = status
 
     def run(
         self,
         task_specification: Union[Dict, str],
         shots: Optional[int],
         *args,
```

### Comparing `strangeworks_azure-0.1.0/strangeworks_azure/job.py` & `strangeworks_azure-0.1.1/strangeworks_azure/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_azure-0.1.0/PKG-INFO` & `strangeworks_azure-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: strangeworks-azure
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-quantum[qiskit] (>=0.28.263081,<0.29.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
-Requires-Dist: strangeworks (>=0.4.1,<0.5.0)
-Requires-Dist: strangeworks-python-core (>=0.1.6,<0.2.0)
+Requires-Dist: strangeworks (>=0.4.4,<0.5.0)
+Requires-Dist: strangeworks-core (>=0.2.3,<0.3.0)
 Description-Content-Type: text/markdown
 
+![Tests](https://github.com/strangeworks/strangeworks-azure/actions/workflows/cron_test.yml/badge.svg)
+
 # Strangeworks Azure Extension
 
 Strangeworks Python SDK extension for Azure.
 
 For more information on using the SDK check out the
 [Strangeworks documentation](https://docs.strangeworks.com/).
```

