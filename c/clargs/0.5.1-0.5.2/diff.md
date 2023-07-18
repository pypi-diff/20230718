# Comparing `tmp/clargs-0.5.1.tar.gz` & `tmp/clargs-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clargs-0.5.1.tar", last modified: Mon Jul 17 12:49:42 2023, max compression
+gzip compressed data, was "clargs-0.5.2.tar", last modified: Tue Jul 18 09:59:04 2023, max compression
```

## Comparing `clargs-0.5.1.tar` & `clargs-0.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 12:49:33.000000 clargs-0.5.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-17 12:49:33.000000 clargs-0.5.1/.github/workflows/upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 12:49:33.000000 clargs-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 12:49:33.000000 clargs-0.5.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-17 12:49:42.819741 clargs-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-17 12:49:33.000000 clargs-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/0_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/1_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/2_show_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/3_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/4_parse_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-17 12:49:33.000000 clargs-0.5.1/examples/__generate_example_output__.sh
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-17 12:49:33.000000 clargs-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:49:42.819741 clargs-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/src/clargs/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/aap_from_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/clargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/docsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-17 12:49:33.000000 clargs-0.5.1/src/clargs/helper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/src/clargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-17 12:49:42.000000 clargs-0.5.1/src/clargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-17 12:49:42.000000 clargs-0.5.1/src/clargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:49:42.000000 clargs-0.5.1/src/clargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 12:49:42.000000 clargs-0.5.1/src/clargs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:49:42.819741 clargs-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-17 12:49:33.000000 clargs-0.5.1/test/test_docsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-07-17 12:49:33.000000 clargs-0.5.1/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-17 12:49:33.000000 clargs-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:59:04.770646 clargs-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:59:04.766646 clargs-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:59:04.766646 clargs-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-18 09:58:55.000000 clargs-0.5.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-18 09:58:55.000000 clargs-0.5.2/.github/workflows/upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 09:58:55.000000 clargs-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 09:58:55.000000 clargs-0.5.2/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-18 09:59:04.770646 clargs-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-18 09:58:55.000000 clargs-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:59:04.770646 clargs-0.5.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-18 09:58:55.000000 clargs-0.5.2/examples/0_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-18 09:58:55.000000 clargs-0.5.2/examples/1_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-18 09:58:55.000000 clargs-0.5.2/examples/2_show_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-18 09:58:55.000000 clargs-0.5.2/examples/3_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-18 09:58:55.000000 clargs-0.5.2/examples/4_parse_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-18 09:58:55.000000 clargs-0.5.2/examples/__generate_example_output__.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-18 09:58:55.000000 clargs-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:59:04.770646 clargs-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:59:04.766646 clargs-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:59:04.770646 clargs-0.5.2/src/clargs/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-18 09:58:55.000000 clargs-0.5.2/src/clargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-18 09:58:55.000000 clargs-0.5.2/src/clargs/aap_from_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-18 09:58:55.000000 clargs-0.5.2/src/clargs/clargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-18 09:58:55.000000 clargs-0.5.2/src/clargs/docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-18 09:58:55.000000 clargs-0.5.2/src/clargs/helper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:59:04.770646 clargs-0.5.2/src/clargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-18 09:59:04.000000 clargs-0.5.2/src/clargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-18 09:59:04.000000 clargs-0.5.2/src/clargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:59:04.000000 clargs-0.5.2/src/clargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 09:59:04.000000 clargs-0.5.2/src/clargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:59:04.770646 clargs-0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-18 09:58:55.000000 clargs-0.5.2/test/test_docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-07-18 09:58:55.000000 clargs-0.5.2/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 09:58:55.000000 clargs-0.5.2/tox.ini
```

### Comparing `clargs-0.5.1/.github/workflows/upload.yml` & `clargs-0.5.2/.github/workflows/upload.yml`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/LICENCE.txt` & `clargs-0.5.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/PKG-INFO` & `clargs-0.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clargs
-Version: 0.5.1
+Version: 0.5.2
 Summary: Easily generate commandline apps from your functions, based on type hints
 Author-email: Claude <pypi@claude.nl>
 Project-URL: Homepage, https://github.com/reinhrst/clargs
 Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,25 +12,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # Clargs
 
 The goal of the `clargs` package is to create commandline interfaces from function signatures.
 
-- With a single line, an existing function is turned into a command line program
-- However it also has the flexibility to be the command line interface of a finished product
-- Explicit goal is **Don't Repeat Yourself**. All information is in a single spot (where you define the function)
-- Pure python and no dependencies (except for running test)
-- Support for `int`, `float`, `bool`, `pathlib.Path`, `list` and `typing.Literal` built-in (more coming)
-- Support for flags (`--foo/--no-foo`)
-- Automatic underscore-to-dash conversion (`foo_bar` becomes `--foo-bar`), and creation of short flags (`--foo-bar` and `-f` are both supported)
-- Type of a parameter is set through [PEP 484][2]-style type hints
-- Defaults are taken from the function signature
-- Based on the built-in `argparse` module
-- Function documentation creates command line arguments documentation
+- **Hit the ground running**: With a single line, an existing function is turned into a command line program
+- **Extensible**: It is flexible enough to do everything that `argparse` does, and keeps you in control
+- **No magic**: All the extension does is call commands in `argparse`; you can log and see these commands
+- **Safe**: The built-in python `argparse` module does all the work, so safety guarantees from that module apply
+- **Typing**: Parameter types are set as [PEP 484][2] type hints (e.g. `def foo(bar: int)`)
+- **Standard**: By using `argparse`, you get standard behaviour such as long/short parameters, combine flags, help function
+- **Don't repeat yourself**: Every parameter is defined (changed, added, removed) in one spot and only one spot, the function definition
+- **Rich parameter types**: Support for `str`, `int`, `float`, `bool`, `pathlib.Path` and `typing.Literal` (multiple-choice values)
+- **Richer parameter types**: In addition, lists of these parameters are allowed, default values, boolean-flags (`--foo/--no-foo`), counts
+- **Simple**: Pure python, no dependencies
+- **Documentation**: Function's docstring creates `--help` documentation. Support for `Sphynx`, `GoogleDoc`, `NumpyDoc`, `EpyText`
 
 
 ## Example
 Check out the [list of examples][3] to see the package in action
 
 
 A quick example (just to get you excited):
```

### Comparing `clargs-0.5.1/README.md` & `clargs-0.5.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Clargs
 
 The goal of the `clargs` package is to create commandline interfaces from function signatures.
 
-- With a single line, an existing function is turned into a command line program
-- However it also has the flexibility to be the command line interface of a finished product
-- Explicit goal is **Don't Repeat Yourself**. All information is in a single spot (where you define the function)
-- Pure python and no dependencies (except for running test)
-- Support for `int`, `float`, `bool`, `pathlib.Path`, `list` and `typing.Literal` built-in (more coming)
-- Support for flags (`--foo/--no-foo`)
-- Automatic underscore-to-dash conversion (`foo_bar` becomes `--foo-bar`), and creation of short flags (`--foo-bar` and `-f` are both supported)
-- Type of a parameter is set through [PEP 484][2]-style type hints
-- Defaults are taken from the function signature
-- Based on the built-in `argparse` module
-- Function documentation creates command line arguments documentation
+- **Hit the ground running**: With a single line, an existing function is turned into a command line program
+- **Extensible**: It is flexible enough to do everything that `argparse` does, and keeps you in control
+- **No magic**: All the extension does is call commands in `argparse`; you can log and see these commands
+- **Safe**: The built-in python `argparse` module does all the work, so safety guarantees from that module apply
+- **Typing**: Parameter types are set as [PEP 484][2] type hints (e.g. `def foo(bar: int)`)
+- **Standard**: By using `argparse`, you get standard behaviour such as long/short parameters, combine flags, help function
+- **Don't repeat yourself**: Every parameter is defined (changed, added, removed) in one spot and only one spot, the function definition
+- **Rich parameter types**: Support for `str`, `int`, `float`, `bool`, `pathlib.Path` and `typing.Literal` (multiple-choice values)
+- **Richer parameter types**: In addition, lists of these parameters are allowed, default values, boolean-flags (`--foo/--no-foo`), counts
+- **Simple**: Pure python, no dependencies
+- **Documentation**: Function's docstring creates `--help` documentation. Support for `Sphynx`, `GoogleDoc`, `NumpyDoc`, `EpyText`
 
 
 ## Example
 Check out the [list of examples][3] to see the package in action
 
 
 A quick example (just to get you excited):
```

### Comparing `clargs-0.5.1/examples/0_basic.py` & `clargs-0.5.2/examples/0_basic.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/examples/1_flags.py` & `clargs-0.5.2/examples/1_flags.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/examples/2_show_defaults.py` & `clargs-0.5.2/examples/2_show_defaults.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/examples/3_list.py` & `clargs-0.5.2/examples/3_list.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/examples/4_parse_groups.py` & `clargs-0.5.2/examples/4_parse_groups.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/examples/__generate_example_output__.sh` & `clargs-0.5.2/examples/__generate_example_output__.sh`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/pyproject.toml` & `clargs-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/src/clargs/__init__.py` & `clargs-0.5.2/src/clargs/__init__.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/src/clargs/aap_from_data.py` & `clargs-0.5.2/src/clargs/aap_from_data.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/src/clargs/clargs.py` & `clargs-0.5.2/src/clargs/clargs.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/src/clargs/docsparser.py` & `clargs-0.5.2/src/clargs/docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/src/clargs/helper_types.py` & `clargs-0.5.2/src/clargs/helper_types.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/src/clargs.egg-info/PKG-INFO` & `clargs-0.5.2/src/clargs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clargs
-Version: 0.5.1
+Version: 0.5.2
 Summary: Easily generate commandline apps from your functions, based on type hints
 Author-email: Claude <pypi@claude.nl>
 Project-URL: Homepage, https://github.com/reinhrst/clargs
 Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,25 +12,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # Clargs
 
 The goal of the `clargs` package is to create commandline interfaces from function signatures.
 
-- With a single line, an existing function is turned into a command line program
-- However it also has the flexibility to be the command line interface of a finished product
-- Explicit goal is **Don't Repeat Yourself**. All information is in a single spot (where you define the function)
-- Pure python and no dependencies (except for running test)
-- Support for `int`, `float`, `bool`, `pathlib.Path`, `list` and `typing.Literal` built-in (more coming)
-- Support for flags (`--foo/--no-foo`)
-- Automatic underscore-to-dash conversion (`foo_bar` becomes `--foo-bar`), and creation of short flags (`--foo-bar` and `-f` are both supported)
-- Type of a parameter is set through [PEP 484][2]-style type hints
-- Defaults are taken from the function signature
-- Based on the built-in `argparse` module
-- Function documentation creates command line arguments documentation
+- **Hit the ground running**: With a single line, an existing function is turned into a command line program
+- **Extensible**: It is flexible enough to do everything that `argparse` does, and keeps you in control
+- **No magic**: All the extension does is call commands in `argparse`; you can log and see these commands
+- **Safe**: The built-in python `argparse` module does all the work, so safety guarantees from that module apply
+- **Typing**: Parameter types are set as [PEP 484][2] type hints (e.g. `def foo(bar: int)`)
+- **Standard**: By using `argparse`, you get standard behaviour such as long/short parameters, combine flags, help function
+- **Don't repeat yourself**: Every parameter is defined (changed, added, removed) in one spot and only one spot, the function definition
+- **Rich parameter types**: Support for `str`, `int`, `float`, `bool`, `pathlib.Path` and `typing.Literal` (multiple-choice values)
+- **Richer parameter types**: In addition, lists of these parameters are allowed, default values, boolean-flags (`--foo/--no-foo`), counts
+- **Simple**: Pure python, no dependencies
+- **Documentation**: Function's docstring creates `--help` documentation. Support for `Sphynx`, `GoogleDoc`, `NumpyDoc`, `EpyText`
 
 
 ## Example
 Check out the [list of examples][3] to see the package in action
 
 
 A quick example (just to get you excited):
```

### Comparing `clargs-0.5.1/src/clargs.egg-info/SOURCES.txt` & `clargs-0.5.2/src/clargs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/test/test_docsparser.py` & `clargs-0.5.2/test/test_docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.1/test/test_simple.py` & `clargs-0.5.2/test/test_simple.py`

 * *Files identical despite different names*

