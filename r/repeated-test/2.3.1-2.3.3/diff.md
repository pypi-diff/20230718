# Comparing `tmp/repeated_test-2.3.1.tar.gz` & `tmp/repeated_test-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repeated_test-2.3.1.tar", last modified: Thu Oct 13 06:56:25 2022, max compression
+gzip compressed data, was "repeated_test-2.3.3.tar", last modified: Tue Jul 18 07:01:53 2023, max compression
```

## Comparing `repeated_test-2.3.1.tar` & `repeated_test-2.3.3.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-13 06:56:25.947856 repeated_test-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (116)      209 2022-10-13 06:56:13.000000 repeated_test-2.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-13 06:56:25.943856 repeated_test-2.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-13 06:56:25.943856 repeated_test-2.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      398 2022-10-13 06:56:13.000000 repeated_test-2.3.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1197 2022-10-13 06:56:13.000000 repeated_test-2.3.1/.github/workflows/deploy-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       93 2022-10-13 06:56:13.000000 repeated_test-2.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      126 2022-10-13 06:56:13.000000 repeated_test-2.3.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (116)      262 2022-10-13 06:56:13.000000 repeated_test-2.3.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)     1191 2022-10-13 06:56:13.000000 repeated_test-2.3.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (116)     1066 2022-10-13 06:56:13.000000 repeated_test-2.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       95 2022-10-13 06:56:13.000000 repeated_test-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    16641 2022-10-13 06:56:25.947856 repeated_test-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    15630 2022-10-13 06:56:13.000000 repeated_test-2.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      140 2022-10-13 06:56:13.000000 repeated_test-2.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-13 06:56:25.943856 repeated_test-2.3.1/repeated_test/
--rw-r--r--   0 runner    (1001) docker     (116)      546 2022-10-13 06:56:13.000000 repeated_test-2.3.1/repeated_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      626 2022-10-13 06:56:13.000000 repeated_test-2.3.1/repeated_test/_evaluated.py
--rw-r--r--   0 runner    (1001) docker     (116)     6648 2022-10-13 06:56:13.000000 repeated_test-2.3.1/repeated_test/core.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-13 06:56:25.947856 repeated_test-2.3.1/repeated_test/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      167 2022-10-13 06:56:13.000000 repeated_test-2.3.1/repeated_test/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22194 2022-10-13 06:56:13.000000 repeated_test-2.3.1/repeated_test/tests/test_rt.py
--rw-r--r--   0 runner    (1001) docker     (116)     1857 2022-10-13 06:56:13.000000 repeated_test-2.3.1/repeated_test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-13 06:56:25.947856 repeated_test-2.3.1/repeated_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    16641 2022-10-13 06:56:25.000000 repeated_test-2.3.1/repeated_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      533 2022-10-13 06:56:25.000000 repeated_test-2.3.1/repeated_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-13 06:56:25.000000 repeated_test-2.3.1/repeated_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-10-13 06:56:25.000000 repeated_test-2.3.1/repeated_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-10-13 06:56:25.000000 repeated_test-2.3.1/repeated_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-10-13 06:56:25.947856 repeated_test-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1355 2022-10-13 06:56:13.000000 repeated_test-2.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      361 2022-10-13 06:56:13.000000 repeated_test-2.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:53.303763 repeated_test-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-18 07:01:44.000000 repeated_test-2.3.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:53.295763 repeated_test-2.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:53.299764 repeated_test-2.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 07:01:44.000000 repeated_test-2.3.3/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-18 07:01:44.000000 repeated_test-2.3.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 07:01:44.000000 repeated_test-2.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-18 07:01:44.000000 repeated_test-2.3.3/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 07:01:44.000000 repeated_test-2.3.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-18 07:01:44.000000 repeated_test-2.3.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-18 07:01:44.000000 repeated_test-2.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 07:01:44.000000 repeated_test-2.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16641 2023-07-18 07:01:53.303763 repeated_test-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15630 2023-07-18 07:01:44.000000 repeated_test-2.3.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-18 07:01:44.000000 repeated_test-2.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:53.299764 repeated_test-2.3.3/repeated_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-18 07:01:44.000000 repeated_test-2.3.3/repeated_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-18 07:01:44.000000 repeated_test-2.3.3/repeated_test/_evaluated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-18 07:01:44.000000 repeated_test-2.3.3/repeated_test/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:53.303763 repeated_test-2.3.3/repeated_test/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-18 07:01:44.000000 repeated_test-2.3.3/repeated_test/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22194 2023-07-18 07:01:44.000000 repeated_test-2.3.3/repeated_test/tests/test_rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 07:01:44.000000 repeated_test-2.3.3/repeated_test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:53.299764 repeated_test-2.3.3/repeated_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16641 2023-07-18 07:01:53.000000 repeated_test-2.3.3/repeated_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-18 07:01:53.000000 repeated_test-2.3.3/repeated_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:01:53.000000 repeated_test-2.3.3/repeated_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 07:01:53.000000 repeated_test-2.3.3/repeated_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 07:01:53.303763 repeated_test-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-18 07:01:44.000000 repeated_test-2.3.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-18 07:01:44.000000 repeated_test-2.3.3/tox.ini
```

### Comparing `repeated_test-2.3.1/COPYING` & `repeated_test-2.3.3/COPYING`

 * *Files identical despite different names*

### Comparing `repeated_test-2.3.1/LICENSE.txt` & `repeated_test-2.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repeated_test-2.3.1/PKG-INFO` & `repeated_test-2.3.3/repeated_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: repeated_test
-Version: 2.3.1
+Name: repeated-test
+Version: 2.3.3
 Summary: A quick unittest-compatible framework for repeating a test function over many fixtures
 Home-page: https://github.com/epsy/repeated_test
 Author: Yann Kaiser
 Author-email: kaiser.yann@gmail.com
 License: MIT
 Keywords: test,testing,unittest,fixtures
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `repeated_test-2.3.1/README.rst` & `repeated_test-2.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `repeated_test-2.3.1/repeated_test/__init__.py` & `repeated_test-2.3.3/repeated_test/__init__.py`

 * *Files identical despite different names*

### Comparing `repeated_test-2.3.1/repeated_test/_evaluated.py` & `repeated_test-2.3.3/repeated_test/_evaluated.py`

 * *Files identical despite different names*

### Comparing `repeated_test-2.3.1/repeated_test/core.py` & `repeated_test-2.3.3/repeated_test/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # COPYING for details.
 
 import itertools
 import sys
 import traceback
 import unittest
 
-import six
 import collections
 
 from repeated_test.utils import options, options_to_kwargs
 from repeated_test import _evaluated
 
 
 __unittest = True # hides frames from this file from unittest output
@@ -178,15 +177,15 @@
 
     return _run_test_matrix
 
 
 def _raise_at_custom_line(filename, lineno, funcname):
     funcname = funcname.strip('<>')
     d = {}
-    six.exec_(compile(_make_raiser(lineno, funcname), filename, 'exec'), d)
+    exec(compile(_make_raiser(lineno, funcname), filename, 'exec'), d)
     ret = d[funcname]
     return ret
 
 
 def _make_raiser(lineno, funcname):
     padding = '\n'*(lineno-1) + 'def '+funcname+'(typ, exc, tb):'
     return padding+'raise exc.with_traceback(tb)'
```

### Comparing `repeated_test-2.3.1/repeated_test/tests/test_rt.py` & `repeated_test-2.3.3/repeated_test/tests/test_rt.py`

 * *Files identical despite different names*

### Comparing `repeated_test-2.3.1/repeated_test/utils.py` & `repeated_test-2.3.3/repeated_test/utils.py`

 * *Files identical despite different names*

### Comparing `repeated_test-2.3.1/repeated_test.egg-info/PKG-INFO` & `repeated_test-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: repeated-test
-Version: 2.3.1
+Name: repeated_test
+Version: 2.3.3
 Summary: A quick unittest-compatible framework for repeating a test function over many fixtures
 Home-page: https://github.com/epsy/repeated_test
 Author: Yann Kaiser
 Author-email: kaiser.yann@gmail.com
 License: MIT
 Keywords: test,testing,unittest,fixtures
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `repeated_test-2.3.1/setup.py` & `repeated_test-2.3.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description_content_type='text/x-rst',
     license="MIT",
     author="Yann Kaiser",
     author_email="kaiser.yann@gmail.com",
     url="https://github.com/epsy/repeated_test",
     tests_require=[],
     python_requires=">=3.5",
-    install_requires=['six>=1.7'],
+    install_requires=[],
     test_suite="repeated_test.tests",
     keywords=['test', 'testing', 'unittest', 'fixtures'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.5",
```

