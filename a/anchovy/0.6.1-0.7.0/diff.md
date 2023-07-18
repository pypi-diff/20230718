# Comparing `tmp/anchovy-0.6.1.tar.gz` & `tmp/anchovy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anchovy-0.6.1.tar", last modified: Wed Aug 24 10:01:39 2022, max compression
+gzip compressed data, was "anchovy-0.7.0.tar", last modified: Mon Jul 17 23:57:59 2023, max compression
```

## Comparing `anchovy-0.6.1.tar` & `anchovy-0.7.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.284264 anchovy-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.276264 anchovy-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.276264 anchovy-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-08-24 10:01:28.000000 anchovy-0.6.1/.github/workflows/python-cq.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-08-24 10:01:28.000000 anchovy-0.6.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-24 10:01:28.000000 anchovy-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-08-24 10:01:28.000000 anchovy-0.6.1/.tokeignore
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-24 10:01:28.000000 anchovy-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5947 2022-08-24 10:01:39.284264 anchovy-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-08-24 10:01:31.000000 anchovy-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.276264 anchovy-0.6.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.280264 anchovy-0.6.1/examples/_images/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/_images/.credits.md
--rw-r--r--   0 runner    (1001) docker     (121)   890709 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/_images/anchovy-nypl.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   706821 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/_images/home-sweet-home-cdk.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   679302 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/_images/nice-wheels-cdk.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   482152 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/_images/quayside-newcastle.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   447542 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/_images/stormy-cdk.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.280264 anchovy-0.6.1/examples/basic_site/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/basic_site/base.jinja.html
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/basic_site/index.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.280264 anchovy-0.6.1/examples/basic_site/static/
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/basic_site/static/core.css
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/basic_site.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/css_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.280264 anchovy-0.6.1/examples/gallery/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/gallery/base.jinja.html
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/gallery/index.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.280264 anchovy-0.6.1/examples/gallery/static/
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/gallery/static/core.css
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-08-24 10:01:28.000000 anchovy-0.6.1/examples/gallery.py
--rw-r--r--   0 runner    (1001) docker     (121)    10831 2022-08-24 10:01:28.000000 anchovy-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-24 10:01:39.284264 anchovy-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-24 10:01:28.000000 anchovy-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.276264 anchovy-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.284264 anchovy-0.6.1/src/anchovy/
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7601 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     8683 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.284264 anchovy-0.6.1/src/anchovy/css/
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8741 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/css/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4129 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     5445 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/images.py
--rw-r--r--   0 runner    (1001) docker     (121)     4162 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/jinja.py
--rw-r--r--   0 runner    (1001) docker     (121)     3834 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/pretty_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-08-24 10:01:28.000000 anchovy-0.6.1/src/anchovy/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:01:39.284264 anchovy-0.6.1/src/anchovy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5947 2022-08-24 10:01:39.000000 anchovy-0.6.1/src/anchovy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-08-24 10:01:39.000000 anchovy-0.6.1/src/anchovy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 10:01:39.000000 anchovy-0.6.1/src/anchovy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-24 10:01:39.000000 anchovy-0.6.1/src/anchovy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-08-24 10:01:39.000000 anchovy-0.6.1/src/anchovy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-24 10:01:39.000000 anchovy-0.6.1/src/anchovy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.236470 anchovy-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.216470 anchovy-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.220470 anchovy-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 23:57:45.000000 anchovy-0.7.0/.github/workflows/python-cq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-17 23:57:45.000000 anchovy-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-17 23:57:45.000000 anchovy-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 23:57:45.000000 anchovy-0.7.0/.tokeignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 23:57:45.000000 anchovy-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-17 23:57:59.236470 anchovy-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-17 23:57:50.000000 anchovy-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.224470 anchovy-0.7.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.228470 anchovy-0.7.0/examples/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/_images/.credits.md
+-rw-r--r--   0 runner    (1001) docker     (123)   890709 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/_images/anchovy-nypl.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   706821 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/_images/home-sweet-home-cdk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   679302 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/_images/nice-wheels-cdk.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   482152 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/_images/quayside-newcastle.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   447542 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/_images/stormy-cdk.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.228470 anchovy-0.7.0/examples/basic_site/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/basic_site/base.jinja.html
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/basic_site/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.228470 anchovy-0.7.0/examples/basic_site/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/basic_site/static/core.css
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/basic_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/css_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.232470 anchovy-0.7.0/examples/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/gallery/base.jinja.html
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/gallery/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.232470 anchovy-0.7.0/examples/gallery/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/gallery/static/core.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-17 23:57:45.000000 anchovy-0.7.0/examples/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-17 23:57:45.000000 anchovy-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:57:59.236470 anchovy-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:57:45.000000 anchovy-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.220470 anchovy-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.232470 anchovy-0.7.0/src/anchovy/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.236470 anchovy-0.7.0/src/anchovy/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/css/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/pretty_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-17 23:57:45.000000 anchovy-0.7.0/src/anchovy/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:57:59.232470 anchovy-0.7.0/src/anchovy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-17 23:57:59.000000 anchovy-0.7.0/src/anchovy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-17 23:57:59.000000 anchovy-0.7.0/src/anchovy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:57:59.000000 anchovy-0.7.0/src/anchovy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 23:57:59.000000 anchovy-0.7.0/src/anchovy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-17 23:57:59.000000 anchovy-0.7.0/src/anchovy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 23:57:59.000000 anchovy-0.7.0/src/anchovy.egg-info/top_level.txt
```

### Comparing `anchovy-0.6.1/.github/workflows/python-cq.yml` & `anchovy-0.7.0/.github/workflows/python-cq.yml`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: true
       matrix:
-        python-version: ['3.10', '3.11.0-alpha - 3.11']
+        python-version: ['3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install .[all] pylint pyright
+        python -m pip install .[cq] pylint pyright
     - name: Lint with pylint
       run: pylint src/anchovy
     - name: Typecheck with pyright
       run: pyright src/anchovy
```

### Comparing `anchovy-0.6.1/.github/workflows/python-publish.yml` & `anchovy-0.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/LICENSE` & `anchovy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/PKG-INFO` & `anchovy-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchovy
-Version: 0.6.1
+Version: 0.7.0
 Summary: A minimal, unopinionated file processing engine intended for static website generation.
 Author-email: Daniel Foerster <pydsigner@gmail.com>
 License: Apache-2.0
 Keywords: static,website,generation,html,css,template
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,14 +22,15 @@
 Provides-Extra: markdown
 Provides-Extra: css
 Provides-Extra: pretty
 Provides-Extra: pillow
 Provides-Extra: web
 Provides-Extra: base
 Provides-Extra: all
+Provides-Extra: cq
 License-File: LICENSE
 
 [![PyPI - Project Version](https://img.shields.io/pypi/v/anchovy)](https://pypi.org/project/anchovy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/anchovy)](https://pypi.org/project/anchovy)
 [![GitHub - Project License](https://img.shields.io/github/license/pydsigner/anchovy)](https://github.com/pydsigner/anchovy)
 [![GitHub - Code Size](https://img.shields.io/github/languages/code-size/pydsigner/anchovy)](https://github.com/pydsigner/anchovy)
 
@@ -90,28 +91,28 @@
     input_dir=Path('site'),
     output_dir=Path('build'),
 )
 RULES = [
     # Ignore dotfiles found in either the input_dir or the working dir.
     Rule(
         (
-            REMatcher(r'(.*/)*\..*', dir='input_dir')
-            | REMatcher(r'(.*/)*\..*', dir='working_dir')
+            REMatcher(r'(.*/)*\..*', parent_dir='input_dir')
+            | REMatcher(r'(.*/)*\..*', parent_dir='working_dir')
         ),
         None
     ),
     # Render markdown files, then stop processing them.
     Rule(
         REMatcher(r'.*\.md'),
         [OutputDirPathCalc('.html'), None],
         JinjaMarkdownStep()
     ),
     # Copy everything else in static/ directories through.
     Rule(
-        REMatcher(r'(.*/)*static/.*', dir='input_dir'),
+        REMatcher(r'(.*/)*static/.*', parent_dir='input_dir'),
         OutputDirPathCalc(),
         DirectCopyStep()
     ),
 ]
 ```
 
 This example is very simple, but is legitimately enough for a small website.
```

### Comparing `anchovy-0.6.1/README.md` & `anchovy-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,28 +60,28 @@
     input_dir=Path('site'),
     output_dir=Path('build'),
 )
 RULES = [
     # Ignore dotfiles found in either the input_dir or the working dir.
     Rule(
         (
-            REMatcher(r'(.*/)*\..*', dir='input_dir')
-            | REMatcher(r'(.*/)*\..*', dir='working_dir')
+            REMatcher(r'(.*/)*\..*', parent_dir='input_dir')
+            | REMatcher(r'(.*/)*\..*', parent_dir='working_dir')
         ),
         None
     ),
     # Render markdown files, then stop processing them.
     Rule(
         REMatcher(r'.*\.md'),
         [OutputDirPathCalc('.html'), None],
         JinjaMarkdownStep()
     ),
     # Copy everything else in static/ directories through.
     Rule(
-        REMatcher(r'(.*/)*static/.*', dir='input_dir'),
+        REMatcher(r'(.*/)*static/.*', parent_dir='input_dir'),
         OutputDirPathCalc(),
         DirectCopyStep()
     ),
 ]
 ```
 
 This example is very simple, but is legitimately enough for a small website.
```

### Comparing `anchovy-0.6.1/examples/_images/.credits.md` & `anchovy-0.7.0/examples/_images/.credits.md`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/examples/_images/anchovy-nypl.jpg` & `anchovy-0.7.0/examples/_images/anchovy-nypl.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/examples/_images/home-sweet-home-cdk.jpg` & `anchovy-0.7.0/examples/_images/home-sweet-home-cdk.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/examples/_images/nice-wheels-cdk.jpg` & `anchovy-0.7.0/examples/_images/nice-wheels-cdk.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/examples/_images/quayside-newcastle.jpg` & `anchovy-0.7.0/examples/_images/quayside-newcastle.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/examples/_images/stormy-cdk.jpg` & `anchovy-0.7.0/examples/_images/stormy-cdk.jpg`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/examples/basic_site.py` & `anchovy-0.7.0/examples/basic_site.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,25 @@
     input_dir=Path(__file__).parent / 'basic_site',
     output_dir=Path('output/basic_site'),
 )
 RULES = [
     # Ignore dotfiles found in either the input_dir or the working dir.
     Rule(
         (
-            REMatcher(r'(.*/)*\..*', dir='input_dir')
-            | REMatcher(r'(.*/)*\..*', dir='working_dir')
+            REMatcher(r'(.*/)*\..*', parent_dir='input_dir')
+            | REMatcher(r'(.*/)*\..*', parent_dir='working_dir')
         ),
         None
     ),
     # Render markdown files, then stop processing them.
     Rule(
         REMatcher(r'.*\.md'),
         [OutputDirPathCalc('.html'), None],
         JinjaMarkdownStep()
     ),
     # Copy everything else in static/ directories through.
     Rule(
-        REMatcher(r'(.*/)*static/.*', dir='input_dir'),
+        REMatcher(r'(.*/)*static/.*', parent_dir='input_dir'),
         OutputDirPathCalc(),
         DirectCopyStep()
     ),
 ]
```

### Comparing `anchovy-0.6.1/examples/css_transformer.py` & `anchovy-0.7.0/examples/css_transformer.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/examples/gallery/index.md` & `anchovy-0.7.0/examples/gallery/index.md`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/examples/gallery/static/core.css` & `anchovy-0.7.0/examples/gallery/static/core.css`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/examples/gallery.py` & `anchovy-0.7.0/examples/gallery.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     input_dir=Path(__file__).parent / 'gallery',
     output_dir=Path('output/gallery'),
 )
 RULES = [
     # Ignore dotfiles found in either the input_dir or the working dir.
     Rule(
         (
-            REMatcher(r'(.*/)*\..*', dir='input_dir')
-            | REMatcher(r'(.*/)*\..*', dir='working_dir')
+            REMatcher(r'(.*/)*\..*', parent_dir='input_dir')
+            | REMatcher(r'(.*/)*\..*', parent_dir='working_dir')
         ),
         None
     ),
     # Render markdown files, then stop processing them.
     Rule(
         REMatcher(r'.*\.md'),
         [OutputDirPathCalc('.html'), None],
@@ -49,12 +49,12 @@
     Rule(
         REMatcher(r'.*\.png'),
         [OutputDirPathCalc(), None],
         OptipngStep()
     ),
     # Copy everything else in static/ directories through.
     Rule(
-        REMatcher(r'(.*/)*static/.*', dir='input_dir'),
+        REMatcher(r'(.*/)*static/.*', parent_dir='input_dir'),
         OutputDirPathCalc(),
         DirectCopyStep()
     ),
 ]
```

### Comparing `anchovy-0.6.1/pyproject.toml` & `anchovy-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,27 @@
     "Topic :: Text Processing :: Markup",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 jinja = ["Jinja2>=3.1.2"]
-markdown = ["anchovy[jinja]", "commonmark>=0.9.1"]
+markdown = ["anchovy[jinja]", "markdown_it_py>=3.0.0"]
 css = ["tinycss2>=1.1.1"]
 pretty = ["rich>=12.5.1"]
 pillow = ["Pillow>=9.2.0"]
 web = ["anchovy[markdown]", "anchovy[css]", "anchovy[pillow]"]
 base = ["anchovy[web]", "anchovy[pretty]"]
 # Currently, [all] is the same as [base]; this will change in the future if
 # heavy dependencies for non-core Steps are added.
 all = ["anchovy[base]"]
+# Includes all possible dependencies, including fallbacks that will not be used
+# under normal circumstances, for linting purposes. End users are intended to
+# ignore this option.
+cq = ["anchovy[all]", "commonmark>=0.9.1", "markdown>=3.4.3", "mistletoe>=1.1.0", "tqdm>=4.65.0"]
 
 [project.scripts]
 anchovy = "anchovy.cli:main"
 
 [tool.setuptools_scm]
 
 [tool.pylint.main]
```

### Comparing `anchovy-0.6.1/src/anchovy/cli.py` & `anchovy-0.7.0/src/anchovy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 
 def pprint_step(step: t.Type[Step]):
     """
     Prettily display dependency information for the given Step class.
     """
     missing = [
-        d.name for d in step.get_dependencies()
+        str(d) for d in step.get_dependencies()
         if d.needed and not d.satisfied
 
     ]
     if missing:
         text = ', '.join(missing)
         print_with_style(f'✗ {step.__name__} (missing: {text})', style='red')
     else:
```

### Comparing `anchovy-0.6.1/src/anchovy/core.py` & `anchovy-0.7.0/src/anchovy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,17 @@
     A context and configuration class for building Anchovy projects.
     """
     def __init__(self,
                  settings: BuildSettings,
                  rules: list[Rule]):
         self.settings = settings
         self.rules: list[Rule] = []
-        for r in rules:
-            self.rules.append(r)
-            self.bind(r.step)
+        for rule in rules:
+            self.rules.append(rule)
+            self.bind(rule.step)
 
     @t.overload
     def __getitem__(self, key: ContextDir) -> Path: ...
     @t.overload
     def __getitem__(self, key: t.Literal['purge_dirs']) -> bool: ...
     def __getitem__(self, key):
         return self.settings[key]
```

### Comparing `anchovy-0.6.1/src/anchovy/css/__init__.py` & `anchovy-0.7.0/src/anchovy/css/__init__.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/src/anchovy/css/parser.py` & `anchovy-0.7.0/src/anchovy/css/parser.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/src/anchovy/dependencies.py` & `anchovy-0.7.0/src/anchovy/dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,40 +24,57 @@
 
 
 def import_install_check(dependency: Dependency):
     """
     An install checker which tries to import a Python module.
     """
     try:
-        importlib.import_module(dependency.name)
+        importlib.import_module(dependency.check_name)
     except ImportError:
         return False
     return True
 
 
 def which_install_check(dependency: Dependency):
     """
     An install checker using `shutil.which()` to look for an executable.
     """
-    return bool(shutil.which(dependency.name))
+    return bool(shutil.which(dependency.check_name))
+
+
+def pip_dependency(name: str, source: str | None = None, check_name: str | None = None):
+    """
+    A shortcut function for creating typical pip-based Dependencys.
+    """
+    return Dependency(name, 'pip', import_install_check, source, check_name)
+
+
+def web_exec_dependency(name: str, source: str | None = None, check_name: str | None = None):
+    """
+    A shortcut function for creating typical Dependencys for general
+    internet-sourced executables.
+    """
+    return Dependency(name, 'web', which_install_check, source, check_name)
 
 
 class Dependency:
     """
     A class for tracking and evaluating dependencies.
     """
     def __init__(self,
                  name: str,
                  type: str,
                  install_check: t.Callable[[Dependency], bool],
-                 source: str | None = None):
+                 source: str | None = None,
+                 check_name: str | None = None):
         self.name = name
         self.type = type
         self.install_check = install_check
         self.source = source or name
+        self.check_name = check_name or name
 
     @property
     def satisfied(self):
         """
         A bool indicating if this dependency is met.
         """
         return self.install_check(self)
@@ -75,14 +92,17 @@
         A string giving help on how to install this dependency.
         """
         return DEPENDENCY_TYPES[self.type][0].format(name=self.name, source=self.source)
 
     def __repr__(self):
         return f'Dependency(name={self.name}, needed={self.needed}, satisfied={self.satisfied})'
 
+    def __str__(self):
+        return self.name
+
     def __or__(self, other: Dependency):
         return _OrDependency(self, other)
 
     def __and__(self, other: Dependency):
         return _AndDependency(self, other)
 
 
@@ -90,14 +110,17 @@
     def __init__(self, left: Dependency, right: Dependency):
         self.left = left
         self.right = right
 
     def __repr__(self):
         return f'{self.left} | {self.right}'
 
+    def __str__(self):
+        return repr(self)
+
     @property
     def satisfied(self):
         """
         A bool indicating whether either of these dependencies are met.
         """
         return self.left.satisfied or self.right.satisfied
 
@@ -125,14 +148,17 @@
     def __init__(self, left: Dependency, right: Dependency):
         self.left = left
         self.right = right
 
     def __repr__(self):
         return f'{self.left} & {self.right}'
 
+    def __str__(self):
+        return repr(self)
+
     @property
     def satisfied(self):
         """
         A bool indicating whether both of these dependencies are met.
         """
         return self.left.satisfied and self.right.satisfied
```

### Comparing `anchovy-0.6.1/src/anchovy/images.py` & `anchovy-0.7.0/src/anchovy/images.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import shutil
 import typing as t
 from pathlib import Path
 
 from .core import Step
-from .dependencies import Dependency, import_install_check, which_install_check
+from .dependencies import pip_dependency, web_exec_dependency
 from .simple import BaseCommandStep
 
 if t.TYPE_CHECKING:
     from _typeshed import StrOrBytesPath
 
 
 class CWebPStep(BaseCommandStep):
@@ -29,22 +29,17 @@
         """
         self.options = ['-q', str(quality)]
         if lossless:
             self.options.append('-lossless')
         self.options.extend(options)
 
     @classmethod
-    def get_dependencies(cls) -> set[Dependency]:
+    def get_dependencies(cls):
         return super().get_dependencies() | {
-            Dependency(
-                'cwebp',
-                'web',
-                which_install_check,
-                'https://developers.google.com/speed/webp/download'
-            ),
+            web_exec_dependency('cwebp', 'https://developers.google.com/speed/webp/download'),
         }
 
     def get_command(self, input_path: Path, output_path: Path) -> list[StrOrBytesPath]:
         return ['cwebp', input_path, *self.options, '-o', output_path]
 
 
 class ImageMagickStep(BaseCommandStep):
@@ -56,21 +51,20 @@
         If simple image conversion is desired, @options can be left empty.
         Otherwise, see https://imagemagick.org/script/command-line-options.php,
         or perhaps use `IMThumbnailStep()` instead.
         """
         self.options = options
 
     @classmethod
-    def get_dependencies(cls) -> set[Dependency]:
+    def get_dependencies(cls):
         return super().get_dependencies() | {
-            Dependency(
-                'magick',
-                'web',
-                which_install_check,
-                'https://imagemagick.org/script/download.php'
+            web_exec_dependency(
+                'imagemagick',
+                'https://imagemagick.org/script/download.php',
+                'magick'
             ),
         }
 
     def get_command(self, input_path: Path, output_path: Path) -> list[StrOrBytesPath]:
         return ['magick', input_path, *self.options, output_path]
 
 
@@ -105,21 +99,19 @@
     """
     A simple Pillow step which can convert and/or thumbnail images.
     """
     def __init__(self, thumbnail: tuple[int, int] | None = None):
         self.thumbnail = thumbnail
 
     @classmethod
-    def get_dependencies(cls) -> set[Dependency]:
+    def get_dependencies(cls):
         return super().get_dependencies() | {
-            Dependency(
-                'PIL',
-                'pip',
-                import_install_check,
-                'Pillow'
+            pip_dependency(
+                'Pillow',
+                check_name='PIL'
             ),
         }
 
     def __call__(self, path: Path, output_paths: list[Path]):
         from PIL import Image
 
         with Image.open(path) as img:
@@ -144,14 +136,14 @@
         The default @optimization_level may vary based on your build of optipng
         but is probably 2. Extra flags may be supplied using @extra_options.
         """
         self.options = ['-o', str(optimization_level)] if optimization_level is not None else []
         self.options.extend(extra_options)
 
     @classmethod
-    def get_dependencies(cls) -> set[Dependency]:
+    def get_dependencies(cls):
         return super().get_dependencies() | {
-            Dependency('optipng', 'web', which_install_check, 'http://optipng.sourceforge.net'),
+            web_exec_dependency('optipng', 'http://optipng.sourceforge.net'),
         }
 
     def get_command(self, input_path: Path, output_path: Path) -> list[StrOrBytesPath]:
         return ['optipng', *self.options, input_path, '-out', output_path]
```

### Comparing `anchovy-0.6.1/src/anchovy/jinja.py` & `anchovy-0.7.0/src/anchovy/jinja.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from __future__ import annotations
 
 import shutil
 import typing as t
+from functools import reduce
 from pathlib import Path
 
 from .core import Context, Step
-from .dependencies import Dependency, import_install_check
+from .dependencies import pip_dependency, Dependency
 
 if t.TYPE_CHECKING:
     import commonmark
     import commonmark.render.renderer
     from jinja2 import Environment
 
 
+MDProcessor = t.Callable[[str], str]
+
+
 class JinjaRenderStep(Step):
     """
     Abstract base class for Steps using Jinja rendering.
     """
     env: Environment
 
     @classmethod
-    def get_dependencies(cls) -> set[Dependency]:
+    def get_dependencies(cls):
         return super().get_dependencies() | {
-            Dependency('jinja2', 'pip', import_install_check),
+            pip_dependency('jinja2'),
         }
 
     def __init__(self,
                  env: Environment | None = None,
                  extra_globals: dict[str, t.Any] | None = None):
         self._temporary_env = env
         self._extra_globals = extra_globals
@@ -69,43 +73,94 @@
     """
     A Step for rendering Markdown using Jinja templates. Parses according to
     CommonMark and Renders to HTML by default.
     """
     encoding = 'utf-8'
 
     @classmethod
-    def get_dependencies(cls) -> set[Dependency]:
-        return super().get_dependencies() | {
-            Dependency('commonmark', 'pip', import_install_check),
-        }
+    def _build_markdownit(cls):
+        import markdown_it
+        processor = markdown_it.MarkdownIt()
+
+        def convert(md_string: str) -> str:
+            return processor.render(md_string)
+
+        return convert
+
+    @classmethod
+    def _build_mistletoe(cls):
+        import mistletoe
+        processor = mistletoe.HTMLRenderer()
+
+        def convert(md_string: str) -> str:
+            return processor.render(mistletoe.Document(md_string))
+
+        return convert
+
+    @classmethod
+    def _build_markdown(cls):
+        import markdown
+        processor = markdown.Markdown()
+
+        def convert(md_string: str):
+            return processor.convert(md_string)
+
+        return convert
+
+    @classmethod
+    def _build_commonmark(cls):
+        import commonmark
+        parser = commonmark.Parser()
+        renderer = commonmark.HtmlRenderer()
+
+        def convert(md_string: str) -> str:
+            return renderer.render(parser.parse(md_string))
+
+        return convert
+
+    @classmethod
+    def get_options(cls):
+        return [
+            (pip_dependency('markdown-it-py', None, 'markdown_it'), cls._build_markdownit),
+            (pip_dependency('mistletoe'), cls._build_mistletoe),
+            (pip_dependency('markdown'), cls._build_markdown),
+            (pip_dependency('commonmark'), cls._build_commonmark),
+        ]
+
+    @classmethod
+    def get_dependencies(cls):
+        deps = [option[0] for option in cls.get_options()]
+        dep_set = {reduce(lambda x, y: x | y, deps)} if deps else set[Dependency]()
+
+        return super().get_dependencies() | dep_set
 
     def __init__(self,
                  default_template: str | None = None,
-                 md_parser: commonmark.Parser | None = None,
-                 md_renderer: commonmark.render.renderer.Renderer | None = None,
+                 md_processor: MDProcessor | None = None,
                  jinja_env: Environment | None = None,
                  jinja_globals: dict[str, t.Any] | None = None):
         super().__init__(jinja_env, jinja_globals)
         self.default_template = default_template
+        self._md_processor = md_processor
+
+    @property
+    def md_processor(self):
+        if not self._md_processor:
+            for dep, factory in self.get_options():
+                if dep.satisfied:
+                    self._md_processor = factory()
+                    break
+            else:
+                raise RuntimeError('Markdown processor could not be initialized!')
+        return self._md_processor
 
-        if md_parser:
-            self.md_parser = md_parser
-        else:
-            import commonmark
-            self.md_parser = commonmark.Parser()
-        if md_renderer:
-            self.md_renderer = md_renderer
-        else:
-            import commonmark
-            self.md_renderer = commonmark.HtmlRenderer()
 
     def __call__(self, path: Path, output_paths: list[Path]):
         meta, content = self.extract_metadata(path.read_text(self.encoding))
-        ast = self.md_parser.parse(content.strip())
-        meta |= {'rendered_markdown': self.md_renderer.render(ast).strip()}
+        meta |= {'rendered_markdown': self.md_processor(content.strip()).strip()}
 
         self.render_template(
             meta.get('template', self.default_template),
             meta,
             output_paths
         )
```

### Comparing `anchovy-0.6.1/src/anchovy/paths.py` & `anchovy-0.7.0/src/anchovy/paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,23 +80,23 @@
     def __call__(self, context: Context, path: Path, match: T) -> Path:
         return _to_dir_inner(context['working_dir'], self.ext, context, path, match)
 
 
 class REMatcher(Matcher[re.Match | None]):
     """
     Path Matcher using regular expressions. @re_flags will be passed to
-    `re.compile()`. @dir, if specified, should be a key to a configured
+    `re.compile()`. @parent_dir, if specified, should be a key to a configured
     directory, not a Path, and will be used to handle matching the beginning of
     Paths; this can be used to avoid pitfalls with unexpected characters in
     input or working directories.
     """
-    def __init__(self, re_string: str, re_flags: int = 0, dir: ContextDir | None = None):
+    def __init__(self, re_string: str, re_flags: int = 0, parent_dir: ContextDir | None = None):
         self.regex = re.compile(re_string, re_flags)
-        self.root_dir: ContextDir | None = dir
+        self.parent_dir: ContextDir | None = parent_dir
 
     def __call__(self, context: Context, path: Path):
-        if self.root_dir:
+        if self.parent_dir:
             # Handle this part of matching outside the regex.
-            if not path.is_relative_to(context[self.root_dir]):
+            if not path.is_relative_to(context[self.parent_dir]):
                 return None
-            path = path.relative_to(context[self.root_dir])
+            path = path.relative_to(context[self.parent_dir])
         return self.regex.match(path.as_posix())
```

### Comparing `anchovy-0.6.1/src/anchovy/pretty_utils.py` & `anchovy-0.7.0/src/anchovy/pretty_utils.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/src/anchovy/simple.py` & `anchovy-0.7.0/src/anchovy/simple.py`

 * *Files identical despite different names*

### Comparing `anchovy-0.6.1/src/anchovy.egg-info/PKG-INFO` & `anchovy-0.7.0/src/anchovy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchovy
-Version: 0.6.1
+Version: 0.7.0
 Summary: A minimal, unopinionated file processing engine intended for static website generation.
 Author-email: Daniel Foerster <pydsigner@gmail.com>
 License: Apache-2.0
 Keywords: static,website,generation,html,css,template
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,14 +22,15 @@
 Provides-Extra: markdown
 Provides-Extra: css
 Provides-Extra: pretty
 Provides-Extra: pillow
 Provides-Extra: web
 Provides-Extra: base
 Provides-Extra: all
+Provides-Extra: cq
 License-File: LICENSE
 
 [![PyPI - Project Version](https://img.shields.io/pypi/v/anchovy)](https://pypi.org/project/anchovy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/anchovy)](https://pypi.org/project/anchovy)
 [![GitHub - Project License](https://img.shields.io/github/license/pydsigner/anchovy)](https://github.com/pydsigner/anchovy)
 [![GitHub - Code Size](https://img.shields.io/github/languages/code-size/pydsigner/anchovy)](https://github.com/pydsigner/anchovy)
 
@@ -90,28 +91,28 @@
     input_dir=Path('site'),
     output_dir=Path('build'),
 )
 RULES = [
     # Ignore dotfiles found in either the input_dir or the working dir.
     Rule(
         (
-            REMatcher(r'(.*/)*\..*', dir='input_dir')
-            | REMatcher(r'(.*/)*\..*', dir='working_dir')
+            REMatcher(r'(.*/)*\..*', parent_dir='input_dir')
+            | REMatcher(r'(.*/)*\..*', parent_dir='working_dir')
         ),
         None
     ),
     # Render markdown files, then stop processing them.
     Rule(
         REMatcher(r'.*\.md'),
         [OutputDirPathCalc('.html'), None],
         JinjaMarkdownStep()
     ),
     # Copy everything else in static/ directories through.
     Rule(
-        REMatcher(r'(.*/)*static/.*', dir='input_dir'),
+        REMatcher(r'(.*/)*static/.*', parent_dir='input_dir'),
         OutputDirPathCalc(),
         DirectCopyStep()
     ),
 ]
 ```
 
 This example is very simple, but is legitimately enough for a small website.
```

### Comparing `anchovy-0.6.1/src/anchovy.egg-info/SOURCES.txt` & `anchovy-0.7.0/src/anchovy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 examples/_images/home-sweet-home-cdk.jpg
 examples/_images/nice-wheels-cdk.jpg
 examples/_images/quayside-newcastle.jpg
 examples/_images/stormy-cdk.jpg
 examples/basic_site/base.jinja.html
 examples/basic_site/index.md
 examples/basic_site/static/core.css
+examples/basic_site/static/images
 examples/gallery/base.jinja.html
 examples/gallery/index.md
 examples/gallery/static/core.css
+examples/gallery/static/images
 src/anchovy/__init__.py
 src/anchovy/__main__.py
 src/anchovy/cli.py
 src/anchovy/core.py
 src/anchovy/dependencies.py
 src/anchovy/images.py
 src/anchovy/jinja.py
```

