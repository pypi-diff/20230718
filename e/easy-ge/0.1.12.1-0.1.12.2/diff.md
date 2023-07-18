# Comparing `tmp/easy_ge-0.1.12.1.tar.gz` & `tmp/easy_ge-0.1.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ge-0.1.12.1.tar", max compression
+gzip compressed data, was "easy_ge-0.1.12.2.tar", max compression
```

## Comparing `easy_ge-0.1.12.1.tar` & `easy_ge-0.1.12.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1059 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/LICENSE
--rw-r--r--   0        0        0      550 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/docs/pypi_readme.md
--rw-r--r--   0        0        0       41 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/easy_ge/__init__.py
--rw-r--r--   0        0        0      310 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/easy_ge/entrypoint.py
--rw-r--r--   0        0        0     6421 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/easy_ge/expectation_manager.py
--rw-r--r--   0        0        0     4468 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/easy_ge/helpers.py
--rw-r--r--   0        0        0     2166 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/easy_ge/main.py
--rw-r--r--   0        0        0      908 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/easy_ge/templates/checkpoint.tpl
--rw-r--r--   0        0        0     4535 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/easy_ge/templates/great_expectations.tpl
--rw-r--r--   0        0        0     5091 2023-07-17 19:11:36.648498 easy_ge-0.1.12.1/easy_ge/templates/schema.json
--rw-r--r--   0        0        0     1267 2023-07-17 19:11:36.652498 easy_ge-0.1.12.1/pyproject.toml
--rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 easy_ge-0.1.12.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-18 13:01:19.110034 easy_ge-0.1.12.2/LICENSE
+-rw-r--r--   0        0        0      550 2023-07-18 13:01:19.110034 easy_ge-0.1.12.2/docs/pypi_readme.md
+-rw-r--r--   0        0        0       41 2023-07-18 13:01:19.114034 easy_ge-0.1.12.2/easy_ge/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-18 13:01:19.114034 easy_ge-0.1.12.2/easy_ge/entrypoint.py
+-rw-r--r--   0        0        0     6701 2023-07-18 13:01:19.114034 easy_ge-0.1.12.2/easy_ge/expectation_manager.py
+-rw-r--r--   0        0        0     4468 2023-07-18 13:01:19.114034 easy_ge-0.1.12.2/easy_ge/helpers.py
+-rw-r--r--   0        0        0     2166 2023-07-18 13:01:19.114034 easy_ge-0.1.12.2/easy_ge/main.py
+-rw-r--r--   0        0        0      908 2023-07-18 13:01:19.114034 easy_ge-0.1.12.2/easy_ge/templates/checkpoint.tpl
+-rw-r--r--   0        0        0     4535 2023-07-18 13:01:19.114034 easy_ge-0.1.12.2/easy_ge/templates/great_expectations.tpl
+-rw-r--r--   0        0        0     5091 2023-07-18 13:01:19.114034 easy_ge-0.1.12.2/easy_ge/templates/schema.json
+-rw-r--r--   0        0        0     1291 2023-07-18 13:01:19.114034 easy_ge-0.1.12.2/pyproject.toml
+-rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 easy_ge-0.1.12.2/PKG-INFO
```

### Comparing `easy_ge-0.1.12.1/LICENSE` & `easy_ge-0.1.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.1/docs/pypi_readme.md` & `easy_ge-0.1.12.2/docs/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.1/easy_ge/expectation_manager.py` & `easy_ge-0.1.12.2/easy_ge/expectation_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # great_expectations_wrapper/expectation_manager.py
 
 """
 This module contains a class for managing Great Expectations operations.
 """
 
+import logging
 from typing import Any, Optional
 
 import pandas as pd
 from great_expectations.data_context import (AbstractDataContext,
                                              BaseDataContext)
 from great_expectations.data_context.types.base import DataContextConfig
 
-try:
-    from easy_ge.helpers import TemplateHandler
-except:
-    from helpers import TemplateHandler
-
-import logging
+from easy_ge.helpers import TemplateHandler
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s [%(levelname)s] %(message)s",
     handlers=[
         logging.StreamHandler()
     ]
@@ -43,17 +39,27 @@
 
         Args:
             config: The Great Expectations configuration.
 
         Returns:
             A BaseDataContext object.
         """
+        if not isinstance(config, dict):
+            raise TypeError("config must be a dictionary.")
+        if config == {}:
+            raise Exception("Empty dictionary passed to the function.")
         logging.info("Preparing data context...")
         ge_config = self.ge_template_handler.process_template(config)
-        return BaseDataContext(DataContextConfig(**ge_config))
+        try:
+            return BaseDataContext(DataContextConfig(**ge_config))
+        except Exception as e:
+            logging.error(f'Error while preparing data context: {e}')
+            raise e
+
+
 
     def prepare_checkpoint(self, config: dict[str, Any], data_context: AbstractDataContext):
         """
         Prepare a checkpoint.
 
         Args:
             config: The configuration.
```

### Comparing `easy_ge-0.1.12.1/easy_ge/helpers.py` & `easy_ge-0.1.12.2/easy_ge/helpers.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.1/easy_ge/main.py` & `easy_ge-0.1.12.2/easy_ge/main.py`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.1/easy_ge/templates/checkpoint.tpl` & `easy_ge-0.1.12.2/easy_ge/templates/checkpoint.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.1/easy_ge/templates/great_expectations.tpl` & `easy_ge-0.1.12.2/easy_ge/templates/great_expectations.tpl`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.1/easy_ge/templates/schema.json` & `easy_ge-0.1.12.2/easy_ge/templates/schema.json`

 * *Files identical despite different names*

### Comparing `easy_ge-0.1.12.1/pyproject.toml` & `easy_ge-0.1.12.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "easy_ge"
-version = "0.1.12.1"
+name = "easy-ge"
+version = "0.1.12.2"
 description = "A package that simplifies usage of Great Expectations tool for Data Validation."
 authors = ["Elsayed91 <elsayed.is@outlook.com>"]
 readme = "docs/pypi_readme.md"
 packages = [{include = "easy_ge"}]
 repository = "https://github.com/Elsayed91/easy_ge"
 keywords = ["Great Expectations", "data quality", "data validation"]
 
@@ -29,14 +29,15 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 localstack = "^2.1.0"
 awscli-local = "^0.20"
+pytest-mock = "^3.11.1"
 
 [tool.poetry.extras]
 aws = ["s3fs"]
 google = ["google-cloud-secret-manager", "google-cloud-storage", "gcsfs"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `easy_ge-0.1.12.1/PKG-INFO` & `easy_ge-0.1.12.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ge
-Version: 0.1.12.1
+Version: 0.1.12.2
 Summary: A package that simplifies usage of Great Expectations tool for Data Validation.
 Home-page: https://github.com/Elsayed91/easy_ge
 Keywords: Great Expectations,data quality,data validation
 Author: Elsayed91
 Author-email: elsayed.is@outlook.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
```

