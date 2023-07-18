# Comparing `tmp/myfuncs-1.0.0.tar.gz` & `tmp/myfuncs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfuncs-1.0.0.tar", last modified: Sat Jul  1 04:55:09 2023, max compression
+gzip compressed data, was "myfuncs-1.1.0.tar", last modified: Tue Jul 18 02:51:55 2023, max compression
```

## Comparing `myfuncs-1.0.0.tar` & `myfuncs-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-01 04:55:09.318271 myfuncs-1.0.0/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-05-13 16:42:37.000000 myfuncs-1.0.0/LICENSE
--rw-r--r--   0 work       (501) staff       (20)     2728 2023-07-01 04:55:09.318161 myfuncs-1.0.0/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     1989 2023-07-01 04:54:48.000000 myfuncs-1.0.0/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-01 04:55:09.317033 myfuncs-1.0.0/myfuncs/
--rw-r--r--   0 work       (501) staff       (20)     1153 2023-07-01 04:37:50.000000 myfuncs-1.0.0/myfuncs/__init__.py
--rw-r--r--   0 work       (501) staff       (20)     4470 2023-07-01 03:35:53.000000 myfuncs-1.0.0/myfuncs/funcs.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-01 04:55:09.317535 myfuncs-1.0.0/myfuncs.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     2728 2023-07-01 04:55:09.000000 myfuncs-1.0.0/myfuncs.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      248 2023-07-01 04:55:09.000000 myfuncs-1.0.0/myfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-07-01 04:55:09.000000 myfuncs-1.0.0/myfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)       14 2023-07-01 04:55:09.000000 myfuncs-1.0.0/myfuncs.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-07-01 04:55:09.318307 myfuncs-1.0.0/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)      916 2023-07-01 04:33:42.000000 myfuncs-1.0.0/setup.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-01 04:55:09.317904 myfuncs-1.0.0/tests/
--rw-r--r--   0 work       (501) staff       (20)        0 2023-07-01 04:44:58.000000 myfuncs-1.0.0/tests/__init__.py
--rwxr-xr-x   0 work       (501) staff       (20)     4015 2023-07-01 03:41:29.000000 myfuncs-1.0.0/tests/funcspy_tests.py
--rw-r--r--   0 work       (501) staff       (20)      985 2023-07-01 04:40:15.000000 myfuncs-1.0.0/tests/main_tests.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-18 02:51:55.448936 myfuncs-1.1.0/
+-rw-r--r--   0 work       (501) staff       (20)     1068 2023-05-13 16:42:37.000000 myfuncs-1.1.0/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)     2878 2023-07-18 02:51:55.448826 myfuncs-1.1.0/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     2139 2023-07-18 02:28:31.000000 myfuncs-1.1.0/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-18 02:51:55.447444 myfuncs-1.1.0/myfuncs/
+-rw-r--r--   0 work       (501) staff       (20)     3776 2023-07-18 02:26:29.000000 myfuncs-1.1.0/myfuncs/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)     4470 2023-07-01 03:35:53.000000 myfuncs-1.1.0/myfuncs/funcs.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-18 02:51:55.448161 myfuncs-1.1.0/myfuncs.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     2878 2023-07-18 02:51:55.000000 myfuncs-1.1.0/myfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      278 2023-07-18 02:51:55.000000 myfuncs-1.1.0/myfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-07-18 02:51:55.000000 myfuncs-1.1.0/myfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)       15 2023-07-18 02:51:55.000000 myfuncs-1.1.0/myfuncs.egg-info/requires.txt
+-rw-r--r--   0 work       (501) staff       (20)       14 2023-07-18 02:51:55.000000 myfuncs-1.1.0/myfuncs.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       38 2023-07-18 02:51:55.448971 myfuncs-1.1.0/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)      932 2023-07-18 02:49:46.000000 myfuncs-1.1.0/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-07-18 02:51:55.448570 myfuncs-1.1.0/tests/
+-rw-r--r--   0 work       (501) staff       (20)        0 2023-07-01 04:44:58.000000 myfuncs-1.1.0/tests/__init__.py
+-rwxr-xr-x   0 work       (501) staff       (20)     4170 2023-07-18 02:33:50.000000 myfuncs-1.1.0/tests/funcspy_tests.py
+-rw-r--r--   0 work       (501) staff       (20)     2258 2023-07-18 02:49:18.000000 myfuncs-1.1.0/tests/main_tests.py
```

### Comparing `myfuncs-1.0.0/LICENSE` & `myfuncs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myfuncs-1.0.0/PKG-INFO` & `myfuncs-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfuncs
-Version: 1.0.0
+Version: 1.1.0
 Summary: Personal utility functions that I use across different codebases.
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -52,14 +52,22 @@
 The `runcmd` function's parameters are:
 
 - `cmd` (str): The command to be executed.
 - `output` (bool, optional): Specifies whether to capture and return the output of the command. Defaults to True.
 - `*args`: Additional positional arguments passed to `subprocess.run()`.
 - `**kwargs`: Additional keyword arguments passed to `subprocess.run()`.
 
+## `is_jwt_str()`
+
+Returns True if a str is a valid encoded jwt string else False
+
+## `nlprint()`
+
+Identical to print but with an additional print()
+
 ----
 
 ## Running Tests
 
 The `myfuncs` package includes a test suite to verify the operation of its functions. To run the tests:
 
 ```bash
```

### Comparing `myfuncs-1.0.0/README.md` & `myfuncs-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 The `runcmd` function's parameters are:
 
 - `cmd` (str): The command to be executed.
 - `output` (bool, optional): Specifies whether to capture and return the output of the command. Defaults to True.
 - `*args`: Additional positional arguments passed to `subprocess.run()`.
 - `**kwargs`: Additional keyword arguments passed to `subprocess.run()`.
 
+## `is_jwt_str()`
+
+Returns True if a str is a valid encoded jwt string else False
+
+## `nlprint()`
+
+Identical to print but with an additional print()
+
 ----
 
 ## Running Tests
 
 The `myfuncs` package includes a test suite to verify the operation of its functions. To run the tests:
 
 ```bash
```

### Comparing `myfuncs-1.0.0/myfuncs/funcs.py` & `myfuncs-1.1.0/myfuncs/funcs.py`

 * *Files identical despite different names*

### Comparing `myfuncs-1.0.0/myfuncs.egg-info/PKG-INFO` & `myfuncs-1.1.0/myfuncs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfuncs
-Version: 1.0.0
+Version: 1.1.0
 Summary: Personal utility functions that I use across different codebases.
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -52,14 +52,22 @@
 The `runcmd` function's parameters are:
 
 - `cmd` (str): The command to be executed.
 - `output` (bool, optional): Specifies whether to capture and return the output of the command. Defaults to True.
 - `*args`: Additional positional arguments passed to `subprocess.run()`.
 - `**kwargs`: Additional keyword arguments passed to `subprocess.run()`.
 
+## `is_jwt_str()`
+
+Returns True if a str is a valid encoded jwt string else False
+
+## `nlprint()`
+
+Identical to print but with an additional print()
+
 ----
 
 ## Running Tests
 
 The `myfuncs` package includes a test suite to verify the operation of its functions. To run the tests:
 
 ```bash
```

### Comparing `myfuncs-1.0.0/setup.py` & `myfuncs-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfuncs',
-    version='1.0.0',
+    version='1.1.0',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=['logfunc==1.4.1'],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='Personal utility functions that I use across different codebases.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/cc-d/myfuncs',
     license='MIT',
```

### Comparing `myfuncs-1.0.0/tests/funcspy_tests.py` & `myfuncs-1.1.0/tests/funcspy_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #!/usr/bin/env python3
 import logging
 import unittest
 import sys
 from pathlib import Path
 from unittest.mock import MagicMock
 
-sys.path.insert(0, str(Path(__file__).parent.parent))  # Add the parent directory of tests to the system path
+sys.path.insert(
+    0, str(Path(__file__).parent.parent)
+)  # Add the parent directory of tests to the system path
 
-from myfuncs.funcs import *
+from myfuncs.funcs import logf, get_asctime, valid_uuid, trunc_str, ran_str
 
 logging.basicConfig(level=logging.DEBUG)
 
+
 class TestMyFuncs(unittest.TestCase):
     @logf()
     def test_get_asctime(self):
         asctime = get_asctime()
         self.assertIsNotNone(asctime)
         self.assertIsInstance(asctime, str)
 
@@ -59,15 +62,14 @@
         self.assertEqual(result, 3)
         self.assertEqual(logger_mock.log.call_count, 2)
         logger_mock.log.assert_any_call(logging.DEBUG, "example_func() | (1, 2) {}")
         log_message = logger_mock.log.call_args_list[1][0][1]
         self.assertTrue(log_message.startswith("example_func()"))
         self.assertTrue(log_message.endswith(" | 3"))
 
-
     @logf()
     def test_logf_no_args_no_return_no_time(self):
         logger_mock = MagicMock()
 
         @logf(level=logging.DEBUG, log_args=False, log_return=False, measure_time=False)
         def example_func(a, b):
             return a + b
@@ -78,20 +80,28 @@
         self.assertEqual(result, 3)
         self.assertEqual(logger_mock.log.call_count, 1)
 
     @logf()
     def test_logf_max_str_len(self):
         logger_mock = MagicMock()
 
-        @logf(level=logging.DEBUG, log_args=True, log_return=True, max_str_len=10, measure_time=True)
+        @logf(
+            level=logging.DEBUG,
+            log_args=True,
+            log_return=True,
+            max_str_len=10,
+            measure_time=True,
+        )
         def example_func(a, b):
             return "abcde" * 1000  # Return a very long string
 
         with unittest.mock.patch('myfuncs.funcs.logger', logger_mock):
-            result = example_func("abcde" * 1000, 2)  # Pass a very long string as an argument
+            result = example_func(
+                "abcde" * 1000, 2
+            )  # Pass a very long string as an argument
 
         self.assertEqual(result, "abcde" * 1000)
         self.assertEqual(logger_mock.log.call_count, 2)
         log_message = logger_mock.log.call_args_list[1][0][1]
         self.assertTrue(log_message.startswith("example_func()"))
         self.assertTrue("..." in log_message)  # Log message should be truncated
```

