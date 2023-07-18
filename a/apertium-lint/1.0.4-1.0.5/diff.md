# Comparing `tmp/apertium_lint-1.0.4.tar.gz` & `tmp/apertium_lint-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apertium_lint-1.0.4.tar", last modified: Mon Jun 26 19:16:25 2023, max compression
+gzip compressed data, was "apertium_lint-1.0.5.tar", last modified: Tue Jul 18 18:57:40 2023, max compression
```

## Comparing `apertium_lint-1.0.4.tar` & `apertium_lint-1.0.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.288689 apertium_lint-1.0.4/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2021-03-01 02:56:44.000000 apertium_lint-1.0.4/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1757 2023-06-26 19:16:25.288689 apertium_lint-1.0.4/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1441 2022-12-27 16:33:47.000000 apertium_lint-1.0.4/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.284689 apertium_lint-1.0.4/apertium_lint/
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)     3381 2022-12-27 16:30:47.000000 apertium_lint-1.0.4/apertium_lint/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9231 2023-03-15 16:13:32.000000 apertium_lint-1.0.4/apertium_lint/file_linter.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.284689 apertium_lint-1.0.4/apertium_lint/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1573 2022-12-23 17:14:07.000000 apertium_lint-1.0.4/apertium_lint/tests/base.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      275 2022-12-23 17:32:13.000000 apertium_lint-1.0.4/apertium_lint/tests/test_cg.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2022-12-23 17:32:06.000000 apertium_lint-1.0.4/apertium_lint/tests/test_lexd.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      460 2022-12-23 17:32:19.000000 apertium_lint-1.0.4/apertium_lint/tests/test_modes.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      444 2022-12-23 17:29:39.000000 apertium_lint-1.0.4/apertium_lint/tests/test_rtx.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1661 2022-12-23 17:32:28.000000 apertium_lint-1.0.4/apertium_lint/tests/test_transfer.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      392 2023-03-15 16:13:16.000000 apertium_lint-1.0.4/apertium_lint/tests/test_twolc.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.284689 apertium_lint-1.0.4/apertium_lint/tree_sitter/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1240 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/cg.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5052 2022-12-27 16:13:50.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/lexc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     5645 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/lexd.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4290 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/rtx.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1904 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/tree_sitter_linter.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6338 2023-03-15 16:13:36.000000 apertium_lint-1.0.4/apertium_lint/tree_sitter/twolc.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.288689 apertium_lint-1.0.4/apertium_lint/xml/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/xml/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10037 2023-04-02 20:54:00.000000 apertium_lint-1.0.4/apertium_lint/xml/dix.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3302 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/xml/lrx.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2839 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/xml/modes.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3249 2023-06-26 19:14:41.000000 apertium_lint-1.0.4/apertium_lint/xml/transfer.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1042 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/apertium_lint/xml/xml.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-26 19:16:25.284689 apertium_lint-1.0.4/apertium_lint.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1757 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1007 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       53 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       33 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-06-26 19:16:25.000000 apertium_lint-1.0.4/apertium_lint.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      546 2023-06-26 19:16:25.288689 apertium_lint-1.0.4/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2022-12-23 16:33:02.000000 apertium_lint-1.0.4/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 18:57:40.067767 apertium_lint-1.0.5/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2021-03-01 02:56:44.000000 apertium_lint-1.0.5/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1757 2023-07-18 18:57:40.067767 apertium_lint-1.0.5/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1441 2022-12-27 16:33:47.000000 apertium_lint-1.0.5/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 18:57:40.055767 apertium_lint-1.0.5/apertium_lint/
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)     3381 2022-12-27 16:30:47.000000 apertium_lint-1.0.5/apertium_lint/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9231 2023-03-15 16:13:32.000000 apertium_lint-1.0.5/apertium_lint/file_linter.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 18:57:40.063767 apertium_lint-1.0.5/apertium_lint/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1573 2022-12-23 17:14:07.000000 apertium_lint-1.0.5/apertium_lint/tests/base.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      275 2022-12-23 17:32:13.000000 apertium_lint-1.0.5/apertium_lint/tests/test_cg.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      336 2023-07-18 18:45:04.000000 apertium_lint-1.0.5/apertium_lint/tests/test_lexc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      293 2022-12-23 17:32:06.000000 apertium_lint-1.0.5/apertium_lint/tests/test_lexd.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      460 2022-12-23 17:32:19.000000 apertium_lint-1.0.5/apertium_lint/tests/test_modes.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      444 2022-12-23 17:29:39.000000 apertium_lint-1.0.5/apertium_lint/tests/test_rtx.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1661 2022-12-23 17:32:28.000000 apertium_lint-1.0.5/apertium_lint/tests/test_transfer.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      392 2023-03-15 16:13:16.000000 apertium_lint-1.0.5/apertium_lint/tests/test_twolc.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 18:57:40.063767 apertium_lint-1.0.5/apertium_lint/tree_sitter/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/tree_sitter/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1240 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/tree_sitter/cg.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6934 2023-07-18 18:56:48.000000 apertium_lint-1.0.5/apertium_lint/tree_sitter/lexc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5645 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/tree_sitter/lexd.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4290 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/tree_sitter/rtx.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1904 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/tree_sitter/tree_sitter_linter.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6338 2023-03-15 16:13:36.000000 apertium_lint-1.0.5/apertium_lint/tree_sitter/twolc.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 18:57:40.067767 apertium_lint-1.0.5/apertium_lint/xml/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       23 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/xml/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10037 2023-04-02 20:54:00.000000 apertium_lint-1.0.5/apertium_lint/xml/dix.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3302 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/xml/lrx.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2839 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/xml/modes.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3249 2023-06-26 19:14:41.000000 apertium_lint-1.0.5/apertium_lint/xml/transfer.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1042 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/apertium_lint/xml/xml.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-18 18:57:40.055767 apertium_lint-1.0.5/apertium_lint.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1757 2023-07-18 18:57:40.000000 apertium_lint-1.0.5/apertium_lint.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1040 2023-07-18 18:57:40.000000 apertium_lint-1.0.5/apertium_lint.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-18 18:57:40.000000 apertium_lint-1.0.5/apertium_lint.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       53 2023-07-18 18:57:40.000000 apertium_lint-1.0.5/apertium_lint.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       33 2023-07-18 18:57:40.000000 apertium_lint-1.0.5/apertium_lint.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-07-18 18:57:40.000000 apertium_lint-1.0.5/apertium_lint.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       96 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      546 2023-07-18 18:57:40.067767 apertium_lint-1.0.5/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2022-12-23 16:33:02.000000 apertium_lint-1.0.5/setup.py
```

### Comparing `apertium_lint-1.0.4/LICENSE` & `apertium_lint-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/PKG-INFO` & `apertium_lint-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium_lint
-Version: 1.0.4
+Version: 1.0.5
 Summary: static analysis of Apertium files
 Home-page: http://github.com/apertium/apertium-lint
 Author: Daniel Swanson
 Author-email: apertium@dangswan.com
 License: GPLv3+
 Keywords: apertium,linter
 Description-Content-Type: text/markdown
```

### Comparing `apertium_lint-1.0.4/README.md` & `apertium_lint-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/__init__.py` & `apertium_lint-1.0.5/apertium_lint/__init__.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/file_linter.py` & `apertium_lint-1.0.5/apertium_lint/file_linter.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/tests/base.py` & `apertium_lint-1.0.5/apertium_lint/tests/base.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/tests/test_transfer.py` & `apertium_lint-1.0.5/apertium_lint/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/tree_sitter/cg.py` & `apertium_lint-1.0.5/apertium_lint/tree_sitter/cg.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/tree_sitter/lexd.py` & `apertium_lint-1.0.5/apertium_lint/tree_sitter/lexd.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/tree_sitter/rtx.py` & `apertium_lint-1.0.5/apertium_lint/tree_sitter/rtx.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/tree_sitter/tree_sitter_linter.py` & `apertium_lint-1.0.5/apertium_lint/tree_sitter/tree_sitter_linter.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/tree_sitter/twolc.py` & `apertium_lint-1.0.5/apertium_lint/tree_sitter/twolc.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/xml/dix.py` & `apertium_lint-1.0.5/apertium_lint/xml/dix.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/xml/lrx.py` & `apertium_lint-1.0.5/apertium_lint/xml/lrx.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/xml/modes.py` & `apertium_lint-1.0.5/apertium_lint/xml/modes.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/xml/transfer.py` & `apertium_lint-1.0.5/apertium_lint/xml/transfer.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint/xml/xml.py` & `apertium_lint-1.0.5/apertium_lint/xml/xml.py`

 * *Files identical despite different names*

### Comparing `apertium_lint-1.0.4/apertium_lint.egg-info/PKG-INFO` & `apertium_lint-1.0.5/apertium_lint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium-lint
-Version: 1.0.4
+Version: 1.0.5
 Summary: static analysis of Apertium files
 Home-page: http://github.com/apertium/apertium-lint
 Author: Daniel Swanson
 Author-email: apertium@dangswan.com
 License: GPLv3+
 Keywords: apertium,linter
 Description-Content-Type: text/markdown
```

### Comparing `apertium_lint-1.0.4/apertium_lint.egg-info/SOURCES.txt` & `apertium_lint-1.0.5/apertium_lint.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 apertium_lint.egg-info/dependency_links.txt
 apertium_lint.egg-info/entry_points.txt
 apertium_lint.egg-info/requires.txt
 apertium_lint.egg-info/top_level.txt
 apertium_lint/tests/__init__.py
 apertium_lint/tests/base.py
 apertium_lint/tests/test_cg.py
+apertium_lint/tests/test_lexc.py
 apertium_lint/tests/test_lexd.py
 apertium_lint/tests/test_modes.py
 apertium_lint/tests/test_rtx.py
 apertium_lint/tests/test_transfer.py
 apertium_lint/tests/test_twolc.py
 apertium_lint/tree_sitter/__init__.py
 apertium_lint/tree_sitter/cg.py
```

### Comparing `apertium_lint-1.0.4/setup.cfg` & `apertium_lint-1.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = apertium_lint
-version = 1.0.4
+version = 1.0.5
 description = static analysis of Apertium files
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = apertium, linter
 license = GPLv3+
 license_files = LICENSE
 author = Daniel Swanson
 author_email = apertium@dangswan.com
 home_page = http://github.com/apertium/apertium-lint
 
 [options]
 install_requires = 
-	tree-sitter-apertium >= 0.1.1
+	tree-sitter-apertium >= 0.1.7
 	lxml
 
 [options.entry_points]
 console_scripts = 
 	apertium-lint = apertium_lint:main
 
 [egg_info]
```

