# Comparing `tmp/booze-0.1.0.tar.gz` & `tmp/booze-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "booze-0.1.0.tar", max compression
+gzip compressed data, was "booze-0.2.0.tar", max compression
```

## Comparing `booze-0.1.0.tar` & `booze-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-18 04:43:34.768812 booze-0.1.0/README.md
--rw-r--r--   0        0        0      426 2023-07-18 16:05:55.241411 booze-0.1.0/booze/__init__.py
--rw-r--r--   0        0        0     1359 2023-07-18 18:52:22.180647 booze-0.1.0/booze/base.py
--rw-r--r--   0        0        0     3814 2023-07-18 20:56:51.739032 booze-0.1.0/booze/coercer.py
--rw-r--r--   0        0        0      548 2023-07-18 19:20:33.481035 booze-0.1.0/booze/errors.py
--rw-r--r--   0        0        0     2822 2023-07-18 19:03:25.524342 booze-0.1.0/booze/test_coercer.py
--rw-r--r--   0        0        0     2146 2023-07-18 19:26:29.535386 booze-0.1.0/booze/test_errors.py
--rw-r--r--   0        0        0     4478 2023-07-18 19:08:47.403397 booze-0.1.0/booze/validators.py
--rw-r--r--   0        0        0      283 2023-07-18 21:03:31.112213 booze-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 booze-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 04:43:34.768812 booze-0.2.0/README.md
+-rw-r--r--   0        0        0      426 2023-07-18 16:05:55.241411 booze-0.2.0/booze/__init__.py
+-rw-r--r--   0        0        0     1359 2023-07-18 18:52:22.180647 booze-0.2.0/booze/base.py
+-rw-r--r--   0        0        0     3808 2023-07-18 21:04:53.190145 booze-0.2.0/booze/coercer.py
+-rw-r--r--   0        0        0      548 2023-07-18 19:20:33.481035 booze-0.2.0/booze/errors.py
+-rw-r--r--   0        0        0     2822 2023-07-18 19:03:25.524342 booze-0.2.0/booze/test_coercer.py
+-rw-r--r--   0        0        0     2146 2023-07-18 19:26:29.535386 booze-0.2.0/booze/test_errors.py
+-rw-r--r--   0        0        0     4478 2023-07-18 19:08:47.403397 booze-0.2.0/booze/validators.py
+-rw-r--r--   0        0        0      283 2023-07-18 21:05:04.914422 booze-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 booze-0.2.0/PKG-INFO
```

### Comparing `booze-0.1.0/booze/base.py` & `booze-0.2.0/booze/base.py`

 * *Files identical despite different names*

### Comparing `booze-0.1.0/booze/coercer.py` & `booze-0.2.0/booze/coercer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from coercer.errors import *
+from booze.errors import *
 import re
-from coercer import validators
+from booze import validators
 import typing as t
 import uuid
 
 
 class Coerce:
     """
     Coerce class provides a set of validation methods to parse and validate data types.
     Call `parse(value)` after setting the validation rules to parse the value. If the value
     passes all validations, the parsed value is returned; otherwise, a ParsingError is raised.
     """
     def __init__(self, name=str(uuid.uuid4())):
-        from coercer.validators import Validator
+        from booze.validators import Validator
         self.name = name
         self.value = None
         self.validations: t.List[Validator] = []
 
     def __repr__(self):
         if self.value:
             return f"Coerce(name='{self.name}', value={self.value})"
```

### Comparing `booze-0.1.0/booze/errors.py` & `booze-0.2.0/booze/errors.py`

 * *Files identical despite different names*

### Comparing `booze-0.1.0/booze/test_coercer.py` & `booze-0.2.0/booze/test_coercer.py`

 * *Files identical despite different names*

### Comparing `booze-0.1.0/booze/test_errors.py` & `booze-0.2.0/booze/test_errors.py`

 * *Files identical despite different names*

### Comparing `booze-0.1.0/booze/validators.py` & `booze-0.2.0/booze/validators.py`

 * *Files identical despite different names*

