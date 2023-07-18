# Comparing `tmp/sphinx-markdown-builder-0.6.2.tar.gz` & `tmp/sphinx-markdown-builder-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-markdown-builder-0.6.2.tar", last modified: Mon Jul  3 23:22:37 2023, max compression
+gzip compressed data, was "sphinx-markdown-builder-0.6.3.tar", last modified: Tue Jul 18 10:11:31 2023, max compression
```

## Comparing `sphinx-markdown-builder-0.6.2.tar` & `sphinx-markdown-builder-0.6.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/
--rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     2159 2023-06-14 19:10:47.000000 sphinx-markdown-builder-0.6.2/CONTRIBUTING.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     1086 2023-07-03 23:20:14.000000 sphinx-markdown-builder-0.6.2/LICENSE
--rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.2/MANIFEST.in
--rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)     2089 2023-07-03 23:20:14.000000 sphinx-markdown-builder-0.6.2/README.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     2060 2023-07-03 23:20:14.000000 sphinx-markdown-builder-0.6.2/pyproject.toml
--rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/setup.cfg
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/
--rw-rw-r--   0 liran     (1000) liran     (1000)      555 2023-07-03 23:20:14.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/__init__.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     2941 2023-07-03 22:00:20.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/builder.py
--rw-rw-r--   0 liran     (1000) liran     (1000)    10540 2023-07-03 22:00:36.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/contexts.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     1786 2023-07-03 22:00:54.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/escape.py
--rw-rw-r--   0 liran     (1000) liran     (1000)    23049 2023-07-03 23:15:09.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/translator.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     1412 2023-07-03 22:00:09.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/writer.py
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/
--rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)      567 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)      111 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/requires.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       24 2023-07-03 23:22:37.000000 sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/top_level.txt
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-03 23:22:37.856375 sphinx-markdown-builder-0.6.2/tests/
--rw-rw-r--   0 liran     (1000) liran     (1000)     2598 2023-06-30 11:36:10.000000 sphinx-markdown-builder-0.6.2/tests/test_builder.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     1994 2023-06-30 12:43:08.000000 sphinx-markdown-builder-0.6.2/tests/test_unit.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-18 10:11:31.735752 sphinx-markdown-builder-0.6.3/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.3/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2159 2023-06-14 19:10:47.000000 sphinx-markdown-builder-0.6.3/CONTRIBUTING.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1086 2023-07-18 10:09:35.000000 sphinx-markdown-builder-0.6.3/LICENSE
+-rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-06-22 13:05:55.000000 sphinx-markdown-builder-0.6.3/MANIFEST.in
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-18 10:11:31.735752 sphinx-markdown-builder-0.6.3/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2089 2023-07-18 10:09:35.000000 sphinx-markdown-builder-0.6.3/README.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2060 2023-07-18 10:09:35.000000 sphinx-markdown-builder-0.6.3/pyproject.toml
+-rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-07-18 10:11:31.735752 sphinx-markdown-builder-0.6.3/setup.cfg
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-18 10:11:31.735752 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/
+-rw-rw-r--   0 liran     (1000) liran     (1000)      555 2023-07-18 10:09:35.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/__init__.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2941 2023-07-03 22:00:20.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/builder.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)    10540 2023-07-03 22:00:36.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/contexts.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1786 2023-07-03 22:00:54.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/escape.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)    23076 2023-07-18 10:03:35.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/translator.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1412 2023-07-03 22:00:09.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/writer.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-18 10:11:31.735752 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder.egg-info/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2802 2023-07-18 10:11:31.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)      567 2023-07-18 10:11:31.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-07-18 10:11:31.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)      111 2023-07-18 10:11:31.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder.egg-info/requires.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       24 2023-07-18 10:11:31.000000 sphinx-markdown-builder-0.6.3/sphinx_markdown_builder.egg-info/top_level.txt
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-07-18 10:11:31.735752 sphinx-markdown-builder-0.6.3/tests/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     2598 2023-06-30 11:36:10.000000 sphinx-markdown-builder-0.6.3/tests/test_builder.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1994 2023-06-30 12:43:08.000000 sphinx-markdown-builder-0.6.3/tests/test_unit.py
```

### Comparing `sphinx-markdown-builder-0.6.2/CODE_OF_CONDUCT.md` & `sphinx-markdown-builder-0.6.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.2/CONTRIBUTING.md` & `sphinx-markdown-builder-0.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.2/LICENSE` & `sphinx-markdown-builder-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.2/PKG-INFO` & `sphinx-markdown-builder-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-markdown-builder
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Sphinx extension to add markdown generation support.
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/liran-funaro/sphinx-markdown-builder
 Keywords: sphinx,sphinx-extention,markdown,docs,documentation,builder
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/liran-funaro/sphinx-markdown-builder/badge.svg?branch=main)](https://coveralls.io/github/liran-funaro/sphinx-markdown-builder?branch=main)
 
 A Sphinx extension to add markdown generation support.
 
 ## Install
 
 ```sh
-pip3 install sphinx-markdown-builder==0.6.2
+pip3 install sphinx-markdown-builder==0.6.3
 ```
 
 ## Usage
 
 Add the extension to your `conf.py` file:
 ```python
 extensions = [
```

### Comparing `sphinx-markdown-builder-0.6.2/README.md` & `sphinx-markdown-builder-0.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/liran-funaro/sphinx-markdown-builder/badge.svg?branch=main)](https://coveralls.io/github/liran-funaro/sphinx-markdown-builder?branch=main)
 
 A Sphinx extension to add markdown generation support.
 
 ## Install
 
 ```sh
-pip3 install sphinx-markdown-builder==0.6.2
+pip3 install sphinx-markdown-builder==0.6.3
 ```
 
 ## Usage
 
 Add the extension to your `conf.py` file:
 ```python
 extensions = [
```

### Comparing `sphinx-markdown-builder-0.6.2/pyproject.toml` & `sphinx-markdown-builder-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sphinx-markdown-builder"
-version = "0.6.2"
+version = "0.6.3"
 description = "A Sphinx extension to add markdown generation support."
 readme = "README.md"
 authors = [{ name = "Liran Funaro", email = "liran.funaro@gmail.com" }]
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -32,15 +32,15 @@
     "bumpver", "black", "isort", "flake8", "pylint", "pip-tools", "pytest", "pytest-cov", "coveralls",
 ]
 
 [project.urls]
 Homepage = "https://github.com/liran-funaro/sphinx-markdown-builder"
 
 [tool.bumpver]
-current_version = "0.6.2"
+current_version = "0.6.3"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/__init__.py` & `sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A Sphinx extension to add markdown generation support.
 """
 from sphinx_markdown_builder.builder import MarkdownBuilder
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 __docformat__ = "reStructuredText"
 
 
 def setup(app):
     app.add_builder(MarkdownBuilder)
     app.add_config_value("markdown_http_base", "", False)
     app.add_config_value("markdown_uri_doc_suffix", ".md", False)
```

### Comparing `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/builder.py` & `sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/builder.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/contexts.py` & `sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/contexts.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/escape.py` & `sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/escape.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/translator.py` & `sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     emphasis=ItalicContext,
     strong=StrongContext,
     subscript=SubscriptContext,
     superscript=SubscriptContext,
     desc_annotation=ItalicContext,
     literal_strong=StrongContext,
     literal_emphasis=ItalicContext,
-    field_name=StrongContext,  # e.g 'returns', 'parameters'
+    field_name=PushContext(WrappedContext, "**", ":**"),  # e.g 'returns', 'parameters'
     # Doc info elements
     docinfo=DocInfoContext,
     docinfo_item=DocInfoContext,
     **dict.fromkeys(DOC_INFO_FIELDS, DocInfoContext),
     authors=None,  # not used: visit_author is called anyway for each author.
     # Doctree elements to skip subtree
     autosummary_toc=SKIP,
```

### Comparing `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder/writer.py` & `sphinx-markdown-builder-0.6.3/sphinx_markdown_builder/writer.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/PKG-INFO` & `sphinx-markdown-builder-0.6.3/sphinx_markdown_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-markdown-builder
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Sphinx extension to add markdown generation support.
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/liran-funaro/sphinx-markdown-builder
 Keywords: sphinx,sphinx-extention,markdown,docs,documentation,builder
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/liran-funaro/sphinx-markdown-builder/badge.svg?branch=main)](https://coveralls.io/github/liran-funaro/sphinx-markdown-builder?branch=main)
 
 A Sphinx extension to add markdown generation support.
 
 ## Install
 
 ```sh
-pip3 install sphinx-markdown-builder==0.6.2
+pip3 install sphinx-markdown-builder==0.6.3
 ```
 
 ## Usage
 
 Add the extension to your `conf.py` file:
 ```python
 extensions = [
```

### Comparing `sphinx-markdown-builder-0.6.2/sphinx_markdown_builder.egg-info/SOURCES.txt` & `sphinx-markdown-builder-0.6.3/sphinx_markdown_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.2/tests/test_builder.py` & `sphinx-markdown-builder-0.6.3/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `sphinx-markdown-builder-0.6.2/tests/test_unit.py` & `sphinx-markdown-builder-0.6.3/tests/test_unit.py`

 * *Files identical despite different names*

