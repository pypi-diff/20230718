# Comparing `tmp/twyn-2.5.4.tar.gz` & `tmp/twyn-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twyn-2.5.4.tar", max compression
+gzip compressed data, was "twyn-2.5.5.tar", max compression
```

## Comparing `twyn-2.5.4.tar` & `twyn-2.5.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1081 2023-07-14 08:25:28.344167 twyn-2.5.4/LICENSE
--rw-r--r--   0        0        0     3441 2023-07-14 08:25:28.344167 twyn-2.5.4/README.md
--rw-r--r--   0        0        0     3159 2023-07-14 08:25:28.348167 twyn-2.5.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/__init__.py
--rw-r--r--   0        0        0       76 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/__version__.py
--rw-r--r--   0        0        0        0 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/base/__init__.py
--rw-r--r--   0        0        0      942 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/base/constants.py
--rw-r--r--   0        0        0      147 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/base/exceptions.py
--rw-r--r--   0        0        0     2420 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/cli.py
--rw-r--r--   0        0        0        0 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/core/__init__.py
--rw-r--r--   0        0        0     3298 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/core/config_handler.py
--rw-r--r--   0        0        0      513 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/core/exceptions.py
--rw-r--r--   0        0        0      221 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/dependency_parser/__init__.py
--rw-r--r--   0        0        0     1380 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/dependency_parser/abstract_parser.py
--rw-r--r--   0        0        0     2149 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/dependency_parser/dependency_selector.py
--rw-r--r--   0        0        0      554 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/dependency_parser/exceptions.py
--rw-r--r--   0        0        0      561 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/dependency_parser/poetry_lock.py
--rw-r--r--   0        0        0      804 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/dependency_parser/requirements_txt.py
--rw-r--r--   0        0        0     5114 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/main.py
--rw-r--r--   0        0        0        0 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/similarity/__init__.py
--rw-r--r--   0        0        0     2210 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/similarity/algorithm.py
--rw-r--r--   0        0        0      275 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/similarity/exceptions.py
--rw-r--r--   0        0        0      189 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/trusted_packages/__init__.py
--rw-r--r--   0        0        0     1497 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/trusted_packages/constants.py
--rw-r--r--   0        0        0      394 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/trusted_packages/exceptions.py
--rw-r--r--   0        0        0     2009 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/trusted_packages/references.py
--rw-r--r--   0        0        0     1907 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/trusted_packages/selectors.py
--rw-r--r--   0        0        0     2816 2023-07-14 08:25:28.348167 twyn-2.5.4/src/twyn/trusted_packages/trusted_packages.py
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 twyn-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-18 10:37:35.458581 twyn-2.5.5/LICENSE
+-rw-r--r--   0        0        0     3441 2023-07-18 10:37:35.458581 twyn-2.5.5/README.md
+-rw-r--r--   0        0        0     3159 2023-07-18 10:37:35.462581 twyn-2.5.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/base/__init__.py
+-rw-r--r--   0        0        0      942 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/base/constants.py
+-rw-r--r--   0        0        0      147 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/base/exceptions.py
+-rw-r--r--   0        0        0     2420 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/cli.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/core/__init__.py
+-rw-r--r--   0        0        0     3298 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/core/config_handler.py
+-rw-r--r--   0        0        0      513 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/core/exceptions.py
+-rw-r--r--   0        0        0      221 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/dependency_parser/__init__.py
+-rw-r--r--   0        0        0     1380 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/dependency_parser/abstract_parser.py
+-rw-r--r--   0        0        0     2149 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/dependency_parser/dependency_selector.py
+-rw-r--r--   0        0        0      554 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/dependency_parser/exceptions.py
+-rw-r--r--   0        0        0      561 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/dependency_parser/poetry_lock.py
+-rw-r--r--   0        0        0      804 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/dependency_parser/requirements_txt.py
+-rw-r--r--   0        0        0     5114 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/main.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/similarity/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/similarity/algorithm.py
+-rw-r--r--   0        0        0      275 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/similarity/exceptions.py
+-rw-r--r--   0        0        0      189 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/trusted_packages/__init__.py
+-rw-r--r--   0        0        0     1497 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/trusted_packages/constants.py
+-rw-r--r--   0        0        0      394 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/trusted_packages/exceptions.py
+-rw-r--r--   0        0        0     2009 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/trusted_packages/references.py
+-rw-r--r--   0        0        0     1907 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/trusted_packages/selectors.py
+-rw-r--r--   0        0        0     2816 2023-07-18 10:37:35.462581 twyn-2.5.5/src/twyn/trusted_packages/trusted_packages.py
+-rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 twyn-2.5.5/PKG-INFO
```

### Comparing `twyn-2.5.4/LICENSE` & `twyn-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/README.md` & `twyn-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/pyproject.toml` & `twyn-2.5.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twyn"
-version = "2.5.4"
+version = "2.5.5"
 description = ""
 authors = ["Daniel Sanz, Sergio Castillo, Ludo van Orden, Dmitrii Fedotov"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 requests = "^2.28.2"
@@ -18,15 +18,15 @@
 
 [tool.poetry.scripts]
 twyn = "twyn.cli:entry_point"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
-mypy = ">=0.982,<1.4"
+mypy = ">=0.982,<1.5"
 black = ">=22.10,<24.0"
 pytest-cov = "^4.0.0"
 ipdb = "^0.13.9"
 commitizen = "^2.38.0"
 pdbpp = "^0.10.3"
 ruff = ">=0.0.239,<0.0.279"
 types-requests = "^2.28.11.12"
@@ -94,15 +94,15 @@
 [tool.coverage.report]
 fail_under = 95
 exclude_lines = ["if TYPE_CHECKING:", "pragma: no cover"]
 
 
 [tool.commitizen]
 version_files = ["pyproject.toml:version"]
-version = "2.5.4"
+version = "2.5.5"
 tag_format = "v$version"
 name = "cz_customize"
 
 
 [tool.commitizen.customize]
 bump_pattern = "^(break|feat|fix|refactor|perf|ci|docs|style|test|chore|revert|build)(\\(.+\\))?(!)?"
 change_type_order = [
```

### Comparing `twyn-2.5.4/src/twyn/base/constants.py` & `twyn-2.5.5/src/twyn/base/constants.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/cli.py` & `twyn-2.5.5/src/twyn/cli.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/core/config_handler.py` & `twyn-2.5.5/src/twyn/core/config_handler.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/core/exceptions.py` & `twyn-2.5.5/src/twyn/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/dependency_parser/abstract_parser.py` & `twyn-2.5.5/src/twyn/dependency_parser/abstract_parser.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/dependency_parser/dependency_selector.py` & `twyn-2.5.5/src/twyn/dependency_parser/dependency_selector.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/dependency_parser/exceptions.py` & `twyn-2.5.5/src/twyn/dependency_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/dependency_parser/poetry_lock.py` & `twyn-2.5.5/src/twyn/dependency_parser/poetry_lock.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/dependency_parser/requirements_txt.py` & `twyn-2.5.5/src/twyn/dependency_parser/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/main.py` & `twyn-2.5.5/src/twyn/main.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/similarity/algorithm.py` & `twyn-2.5.5/src/twyn/similarity/algorithm.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/trusted_packages/constants.py` & `twyn-2.5.5/src/twyn/trusted_packages/constants.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/trusted_packages/references.py` & `twyn-2.5.5/src/twyn/trusted_packages/references.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/trusted_packages/selectors.py` & `twyn-2.5.5/src/twyn/trusted_packages/selectors.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/src/twyn/trusted_packages/trusted_packages.py` & `twyn-2.5.5/src/twyn/trusted_packages/trusted_packages.py`

 * *Files identical despite different names*

### Comparing `twyn-2.5.4/PKG-INFO` & `twyn-2.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twyn
-Version: 2.5.4
+Version: 2.5.5
 Summary: 
 Author: Daniel Sanz, Sergio Castillo, Ludo van Orden, Dmitrii Fedotov
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

