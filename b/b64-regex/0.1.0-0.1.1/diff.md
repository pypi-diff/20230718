# Comparing `tmp/b64_regex-0.1.0.tar.gz` & `tmp/b64_regex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b64_regex-0.1.0.tar", max compression
+gzip compressed data, was "b64_regex-0.1.1.tar", max compression
```

## Comparing `b64_regex-0.1.0.tar` & `b64_regex-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-18 00:22:50.034018 b64_regex-0.1.0/b64_regex/__init__.py
--rw-r--r--   0        0        0      854 2023-07-18 00:53:48.566522 b64_regex-0.1.0/b64_regex/generate_test.py
--rw-r--r--   0        0        0     6804 2023-07-18 10:08:40.594786 b64_regex-0.1.0/b64_regex/recoder.py
--rw-r--r--   0        0        0        0 2023-07-18 01:07:21.729803 b64_regex-0.1.0/b64_regex/tests/__init__.py
--rw-r--r--   0        0        0   150857 2023-07-18 01:02:29.509338 b64_regex-0.1.0/b64_regex/tests/data/test.csv
--rw-r--r--   0        0        0    65028 2023-07-18 07:52:58.538597 b64_regex-0.1.0/b64_regex/tests/data/test.txt
--rw-r--r--   0        0        0     1158 2023-07-18 08:35:40.944539 b64_regex-0.1.0/b64_regex/tests/test_compiler.py
--rw-r--r--   0        0        0      424 2023-07-18 10:19:30.017280 b64_regex-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2234 2023-07-18 10:13:29.713408 b64_regex-0.1.0/README.md
--rw-r--r--   0        0        0     2632 1970-01-01 00:00:00.000000 b64_regex-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2716 2023-07-18 10:40:13.424550 b64_regex-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 10:40:13.424550 b64_regex-0.1.1/b64_regex/__init__.py
+-rw-r--r--   0        0        0      854 2023-07-18 10:40:13.424550 b64_regex-0.1.1/b64_regex/generate_test.py
+-rw-r--r--   0        0        0     6804 2023-07-18 10:40:13.424550 b64_regex-0.1.1/b64_regex/recoder.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:40:13.424550 b64_regex-0.1.1/b64_regex/tests/__init__.py
+-rw-r--r--   0        0        0   150857 2023-07-18 10:40:13.424550 b64_regex-0.1.1/b64_regex/tests/data/test.csv
+-rw-r--r--   0        0        0    65028 2023-07-18 10:40:13.424550 b64_regex-0.1.1/b64_regex/tests/data/test.txt
+-rw-r--r--   0        0        0     1158 2023-07-18 10:40:13.424550 b64_regex-0.1.1/b64_regex/tests/test_compiler.py
+-rw-r--r--   0        0        0      620 2023-07-18 10:40:13.424550 b64_regex-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3409 1970-01-01 00:00:00.000000 b64_regex-0.1.1/PKG-INFO
```

### Comparing `b64_regex-0.1.0/b64_regex/generate_test.py` & `b64_regex-0.1.1/b64_regex/generate_test.py`

 * *Files identical despite different names*

### Comparing `b64_regex-0.1.0/b64_regex/recoder.py` & `b64_regex-0.1.1/b64_regex/recoder.py`

 * *Files identical despite different names*

### Comparing `b64_regex-0.1.0/b64_regex/tests/data/test.csv` & `b64_regex-0.1.1/b64_regex/tests/data/test.csv`

 * *Files identical despite different names*

### Comparing `b64_regex-0.1.0/b64_regex/tests/data/test.txt` & `b64_regex-0.1.1/b64_regex/tests/data/test.txt`

 * *Files identical despite different names*

### Comparing `b64_regex-0.1.0/b64_regex/tests/test_compiler.py` & `b64_regex-0.1.1/b64_regex/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `b64_regex-0.1.0/README.md` & `b64_regex-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Base64 Regex
 
+[![pypi](https://img.shields.io/pypi/v/b64-regex)](https://pypi.org/project/b64-regex/)
+[![test](https://github.com/MythicManiac/b64-regex/workflows/Test/badge.svg)](https://github.com/MythicManiac/b64-regex/actions)
+[![codecov](https://codecov.io/gh/MythicManiac/b64-regex/branch/master/graph/badge.svg?token=D1IB10WPT7)](https://codecov.io/gh/MythicManiac/b64-regex)
+[![python-versions](https://img.shields.io/pypi/pyversions/b64-regex.svg)](https://pypi.org/project/b64-regex/)
+
 Search through base64 encoding without decoding.
 
 ## Usage
 
 ### Building a regex
 
 To build a regex pattern for matching a specific string through base64, use the
```

### Comparing `b64_regex-0.1.0/PKG-INFO` & `b64_regex-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: b64-regex
-Version: 0.1.0
-Summary: Search through b64 encoded text without decoding.
+Version: 0.1.1
+Summary: Build regex patterns for search through b64 encoded text without decoding.
+Home-page: https://github.com/MythicManiac/b64-regex
 License: MIT
 Author: Mythic
-Author-email: mythicmaniac@gmail.com
-Requires-Python: >=3.11,<4.0
+Author-email: mythic@thunderstore.io
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/MythicManiac/b64-regex
 Description-Content-Type: text/markdown
 
 # Base64 Regex
 
+[![pypi](https://img.shields.io/pypi/v/b64-regex)](https://pypi.org/project/b64-regex/)
+[![test](https://github.com/MythicManiac/b64-regex/workflows/Test/badge.svg)](https://github.com/MythicManiac/b64-regex/actions)
+[![codecov](https://codecov.io/gh/MythicManiac/b64-regex/branch/master/graph/badge.svg?token=D1IB10WPT7)](https://codecov.io/gh/MythicManiac/b64-regex)
+[![python-versions](https://img.shields.io/pypi/pyversions/b64-regex.svg)](https://pypi.org/project/b64-regex/)
+
 Search through base64 encoding without decoding.
 
 ## Usage
 
 ### Building a regex
 
 To build a regex pattern for matching a specific string through base64, use the
```

