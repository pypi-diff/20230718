# Comparing `tmp/spam_analyzer-0.2.0b1.tar.gz` & `tmp/spam_analyzer-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spam_analyzer-0.2.0b1.tar", max compression
+gzip compressed data, was "spam_analyzer-0.2.1b0.tar", max compression
```

## Comparing `spam_analyzer-0.2.0b1.tar` & `spam_analyzer-0.2.1b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        4 2023-07-16 17:37:10.362472 spam_analyzer-0.2.0b1/.github/python-version.txt
--rw-r--r--   0        0        0    35149 2023-07-16 17:37:10.362472 spam_analyzer-0.2.0b1/LICENSE
--rw-r--r--   0        0        0     7841 2023-07-16 21:26:37.359742 spam_analyzer-0.2.0b1/README.md
--rw-r--r--   0        0        0      285 2023-07-16 21:26:37.359742 spam_analyzer-0.2.0b1/conf/config.yaml
--rw-r--r--   0        0        0     6770 2023-07-16 17:37:10.506471 spam_analyzer-0.2.0b1/conf/word_blacklist.txt
--rw-r--r--   0        0        0     1912 2023-07-18 15:29:07.945312 spam_analyzer-0.2.0b1/pyproject.toml
--rw-r--r--   0        0        0      974 2023-07-18 15:28:22.945317 spam_analyzer-0.2.0b1/spamanalyzer/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 17:37:10.518472 spam_analyzer-0.2.0b1/spamanalyzer/__main__.py
--rw-r--r--   0        0        0     1322 2023-07-17 22:51:24.740954 spam_analyzer-0.2.0b1/spamanalyzer/analyzer/__init__.py
--rw-r--r--   0        0        0      984 2023-07-17 22:51:24.740954 spam_analyzer-0.2.0b1/spamanalyzer/analyzer/classifier.py
--rw-r--r--   0        0        0    14029 2023-07-17 22:51:24.740954 spam_analyzer-0.2.0b1/spamanalyzer/analyzer/data_structures.py
--rw-r--r--   0        0        0    11867 2023-07-17 22:51:24.740954 spam_analyzer-0.2.0b1/spamanalyzer/analyzer/utils.py
--rw-r--r--   0        0        0       58 2023-07-17 22:51:24.740954 spam_analyzer-0.2.0b1/spamanalyzer/cli/__init__.py
--rw-r--r--   0        0        0     2028 2023-07-17 22:51:24.740954 spam_analyzer-0.2.0b1/spamanalyzer/cli/parser.py
--rw-r--r--   0        0        0     1732 2023-07-17 22:51:24.740954 spam_analyzer-0.2.0b1/spamanalyzer/cli/run.py
--rw-r--r--   0        0        0     4794 2023-07-17 22:51:24.740954 spam_analyzer-0.2.0b1/spamanalyzer/display.py
--rw-r--r--   0        0        0     3171 2023-07-17 22:51:24.740954 spam_analyzer-0.2.0b1/spamanalyzer/files.py
--rw-r--r--   0        0        0     9109 1970-01-01 00:00:00.000000 spam_analyzer-0.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-07-18 15:37:16.810585 spam_analyzer-0.2.1b0/.github/python-version.txt
+-rw-r--r--   0        0        0    35149 2023-07-18 15:37:16.814585 spam_analyzer-0.2.1b0/LICENSE
+-rw-r--r--   0        0        0     7841 2023-07-18 15:37:16.814585 spam_analyzer-0.2.1b0/README.md
+-rw-r--r--   0        0        0      285 2023-07-18 15:37:17.086584 spam_analyzer-0.2.1b0/conf/config.yaml
+-rw-r--r--   0        0        0     6770 2023-07-18 15:37:17.086584 spam_analyzer-0.2.1b0/conf/word_blacklist.txt
+-rw-r--r--   0        0        0     1911 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/pyproject.toml
+-rw-r--r--   0        0        0      974 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/__main__.py
+-rw-r--r--   0        0        0     1322 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/analyzer/__init__.py
+-rw-r--r--   0        0        0      984 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/analyzer/classifier.py
+-rw-r--r--   0        0        0    14029 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/analyzer/data_structures.py
+-rw-r--r--   0        0        0    11867 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/analyzer/utils.py
+-rw-r--r--   0        0        0       58 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/cli/__init__.py
+-rw-r--r--   0        0        0     2028 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/cli/parser.py
+-rw-r--r--   0        0        0     1732 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/cli/run.py
+-rw-r--r--   0        0        0     4794 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/display.py
+-rw-r--r--   0        0        0     3171 2023-07-18 15:37:17.110584 spam_analyzer-0.2.1b0/spamanalyzer/files.py
+-rw-r--r--   0        0        0     9109 1970-01-01 00:00:00.000000 spam_analyzer-0.2.1b0/PKG-INFO
```

### Comparing `spam_analyzer-0.2.0b1/LICENSE` & `spam_analyzer-0.2.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/README.md` & `spam_analyzer-0.2.1b0/README.md`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/conf/word_blacklist.txt` & `spam_analyzer-0.2.1b0/conf/word_blacklist.txt`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/pyproject.toml` & `spam_analyzer-0.2.1b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spam-analyzer"
-version = "0.2.0b1"
+version = "0.2.1b"
 description = "A simple email analyzer"
 authors = ["Matteo Spanio <matteo.spanio97@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "spamanalyzer"}]
 homepage = "http://matteospanio.me/spam-analyzer/"
 repository = "https://github.com/matteospanio/spam-analyzer"
```

### Comparing `spam_analyzer-0.2.0b1/spamanalyzer/__init__.py` & `spam_analyzer-0.2.1b0/spamanalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/spamanalyzer/analyzer/__init__.py` & `spam_analyzer-0.2.1b0/spamanalyzer/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/spamanalyzer/analyzer/classifier.py` & `spam_analyzer-0.2.1b0/spamanalyzer/analyzer/classifier.py`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/spamanalyzer/analyzer/data_structures.py` & `spam_analyzer-0.2.1b0/spamanalyzer/analyzer/data_structures.py`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/spamanalyzer/analyzer/utils.py` & `spam_analyzer-0.2.1b0/spamanalyzer/analyzer/utils.py`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/spamanalyzer/cli/parser.py` & `spam_analyzer-0.2.1b0/spamanalyzer/cli/parser.py`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/spamanalyzer/cli/run.py` & `spam_analyzer-0.2.1b0/spamanalyzer/cli/run.py`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/spamanalyzer/display.py` & `spam_analyzer-0.2.1b0/spamanalyzer/display.py`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/spamanalyzer/files.py` & `spam_analyzer-0.2.1b0/spamanalyzer/files.py`

 * *Files identical despite different names*

### Comparing `spam_analyzer-0.2.0b1/PKG-INFO` & `spam_analyzer-0.2.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spam-analyzer
-Version: 0.2.0b1
+Version: 0.2.1b0
 Summary: A simple email analyzer
 Home-page: http://matteospanio.me/spam-analyzer/
 License: GPLv3
 Keywords: spam,spam-analyzer,cybersecurity
 Author: Matteo Spanio
 Author-email: matteo.spanio97@gmail.com
 Requires-Python: >=3.10,<4.0
```

