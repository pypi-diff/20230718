# Comparing `tmp/examon_core-1.0.6.tar.gz` & `tmp/examon_core-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.0.6.tar", max compression
+gzip compressed data, was "examon_core-1.0.7.tar", max compression
```

## Comparing `examon_core-1.0.6.tar` & `examon_core-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.6/examon_core/__init__.py
--rw-r--r--   0        0        0     1039 2023-07-16 08:19:13.878728 examon_core-1.0.6/examon_core/code_metrics.py
--rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.0.6/examon_core/examon_item.py
--rwxr-xr-x   0        0        0     1531 2023-07-18 13:36:47.779723 examon_core-1.0.6/examon_core/examon_item_registry.py
--rwxr-xr-x   0        0        0     1697 2023-07-16 08:20:56.019327 examon_core-1.0.6/examon_core/function_raw_code.py
--rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.0.6/examon_core/multi_choice_factory.py
--rw-r--r--   0        0        0      980 2023-07-16 08:19:13.846489 examon_core-1.0.6/examon_core/print_ext.py
--rwxr-xr-x   0        0        0      620 2023-07-16 08:19:13.933636 examon_core-1.0.6/examon_core/question.py
--rw-r--r--   0        0        0     2591 2023-07-16 08:19:13.826878 examon_core-1.0.6/examon_core/question_factory.py
--rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.6/examon_core/question_response.py
--rw-r--r--   0        0        0      107 2023-07-17 15:48:04.895960 examon_core-1.0.6/examon_core/todo.md
--rw-r--r--   0        0        0      517 2023-07-18 14:19:53.482392 examon_core-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.7/examon_core/__init__.py
+-rw-r--r--   0        0        0     1039 2023-07-16 08:19:13.878728 examon_core-1.0.7/examon_core/code_metrics.py
+-rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.0.7/examon_core/examon_item.py
+-rwxr-xr-x   0        0        0     1531 2023-07-18 13:36:47.779723 examon_core-1.0.7/examon_core/examon_item_registry.py
+-rwxr-xr-x   0        0        0     1697 2023-07-16 08:20:56.019327 examon_core-1.0.7/examon_core/function_raw_code.py
+-rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.0.7/examon_core/multi_choice_factory.py
+-rw-r--r--   0        0        0      980 2023-07-16 08:19:13.846489 examon_core-1.0.7/examon_core/print_ext.py
+-rwxr-xr-x   0        0        0      620 2023-07-16 08:19:13.933636 examon_core-1.0.7/examon_core/question.py
+-rw-r--r--   0        0        0     2850 2023-07-18 20:38:10.761164 examon_core-1.0.7/examon_core/question_factory.py
+-rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.7/examon_core/question_response.py
+-rw-r--r--   0        0        0      107 2023-07-17 15:48:04.895960 examon_core-1.0.7/examon_core/todo.md
+-rw-r--r--   0        0        0      517 2023-07-18 20:40:27.926998 examon_core-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.7/PKG-INFO
```

### Comparing `examon_core-1.0.6/examon_core/code_metrics.py` & `examon_core-1.0.7/examon_core/code_metrics.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.6/examon_core/examon_item.py` & `examon_core-1.0.7/examon_core/examon_item.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.6/examon_core/examon_item_registry.py` & `examon_core-1.0.7/examon_core/examon_item_registry.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.6/examon_core/function_raw_code.py` & `examon_core-1.0.7/examon_core/function_raw_code.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.6/examon_core/print_ext.py` & `examon_core-1.0.7/examon_core/print_ext.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.6/examon_core/question.py` & `examon_core-1.0.7/examon_core/question.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.6/examon_core/question_factory.py` & `examon_core-1.0.7/examon_core/question_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,32 @@
 from .print_ext import PrintLog
 from .code_metrics import CodeMetricsFactory
 
 import random
 import logging
 
 
+class InvalidChoiceException(Exception):
+    pass
+
+
 class QuestionFactory:
     @staticmethod
     def build(**kwargs):
         function = kwargs['function']
         tags = kwargs['tags']
-        hints = kwargs['hints']
+        hints = kwargs['hints'] if 'hints' in kwargs.keys() else []
         param1 = kwargs['param1'] if 'param1' in kwargs else None
         choice_list = kwargs['choice_list']
         fn_string = function_raw_code(function, hints)
         first_line_no = function.__code__.co_firstlineno
 
+        if choice_list is not None and any(type(choice) is tuple for choice in choice_list):
+            raise InvalidChoiceException('Cannot use a <tuple> as a choice')
+
         # Code Metrics
         metrics = CodeMetricsFactory.build(fn_string)
 
         # Build
         if param1 is not None:
             selected_input_param = random.choice(param1)
             PrintLog.reset()
```

### Comparing `examon_core-1.0.6/pyproject.toml` & `examon_core-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "examon_core"
-version = "1.0.6"
+version = "1.0.7"
 description = "Examon Core Libs"
 authors = ["Jarrod Folino <jdfolino@icloud.com>"]
 packages = [{include = "examon_core"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 radon = "^6.0.1"
```

