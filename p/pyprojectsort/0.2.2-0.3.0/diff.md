# Comparing `tmp/pyprojectsort-0.2.2.tar.gz` & `tmp/pyprojectsort-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectsort-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprojectsort-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprojectsort-0.2.2.tar` & `pyprojectsort-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3200 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/README.md
--rw-r--r--   0        0        0     2022 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      203 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyprojectsort/__init__.py
--rw-r--r--   0        0        0      138 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyprojectsort/__main__.py
--rw-r--r--   0        0        0      197 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyprojectsort/__version__.py
--rw-r--r--   0        0        0     3099 2023-07-07 23:35:34.349272 pyprojectsort-0.2.2/pyprojectsort/main.py
--rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 pyprojectsort-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3977 2023-07-18 19:07:00.152661 pyprojectsort-0.3.0/README.md
+-rw-r--r--   0        0        0     2225 2023-07-18 19:07:00.156661 pyprojectsort-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-07-18 19:07:00.156661 pyprojectsort-0.3.0/pyprojectsort/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-18 19:07:00.156661 pyprojectsort-0.3.0/pyprojectsort/__main__.py
+-rw-r--r--   0        0        0      197 2023-07-18 19:07:00.156661 pyprojectsort-0.3.0/pyprojectsort/__version__.py
+-rw-r--r--   0        0        0     6172 2023-07-18 19:07:00.156661 pyprojectsort-0.3.0/pyprojectsort/main.py
+-rw-r--r--   0        0        0     4982 1970-01-01 00:00:00.000000 pyprojectsort-0.3.0/PKG-INFO
```

### Comparing `pyprojectsort-0.2.2/README.md` & `pyprojectsort-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # pyprojectsort
 
-[![image](https://badge.fury.io/py/pyprojectsort.svg)](https://pypi.org/project/pyprojectsort/)
-![image](https://img.shields.io/badge/license-MIT-blue)
-[![image](https://img.shields.io/pypi/pyversions/pyprojectsort.svg)](https://pypi.python.org/pypi/pyprojectsort)
+[![PyPI Version](https://badge.fury.io/py/pyprojectsort.svg)](https://pypi.org/project/pyprojectsort/)
+![LICENSE](https://img.shields.io/badge/license-MIT-blue)
+[![Python versions](https://img.shields.io/pypi/pyversions/pyprojectsort.svg)](https://pypi.org/pypi/pyprojectsort)
 ![Supported platforms](https://img.shields.io/badge/platforms-macOS%20%7C%20Windows%20%7C%20Linux-green)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![Pipeline status](https://github.com/kieran-ryan/python-package-template/actions/workflows/main.yml/badge.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kieran-ryan/pyprojectsort/main.svg)](https://results.pre-commit.ci/latest/github/kieran-ryan/pyprojectsort/main)
 
 Formatter for pyproject.toml files.
 
-This package enforces consistent formatting of pyproject.toml files, reducing merge request conflicts and saving time otherwise spent to format manually. It also contributes to a cleaner git history and more readable code; enhancing overall project organisation and maintainability. Experience a streamlined workflow, reduced errors, and improved code readability with `pyprojectsort`.
+This package enforces consistent formatting of pyproject.toml files, reducing merge request conflicts and saving time otherwise spent on manual formatting. It also contributes to a cleaner git history and more readable code; enhancing overall project organisation and maintainability. Experience a streamlined workflow, reduced errors, and improved code readability with `pyprojectsort`.
 
 ## Features
 
-- Alphabetically sorts pyproject.toml by:
+- Alphanumerically sorts pyproject.toml by:
   - section
   - section key
   - list value
 - Reformats pyproject.toml to a standardised style
   - line per list value
   - double quotations
   - trailing commas
@@ -35,15 +36,15 @@
 
 ### Using pyprojectsort with [pre-commit](https://pre-commit.com)
 
 To use as an automated git hook, add this to your `.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/kieran-ryan/pyprojectsort
-  rev: v0.2.1
+  rev: v0.2.2
   hooks:
     - id: pyprojectsort
 ```
 
 ## Examples
 
 With the following `pyproject.toml`:
@@ -53,14 +54,19 @@
 ignore = ["G004",
 "T201",
     "ANN"
 ]
 
 [project]
 name = 'pyprojectsort'
+authors = [
+    { name = "Kieran Ryan" },
+    "Author Name <author@email.com>",
+    {name="Author name"}
+]
 
 [tool.radon]
 show_mi = true
 exclude = "tests/*,venv/*"
 total_average = true
 show_complexity = true
 
@@ -81,14 +87,19 @@
 [build-system]
 build-backend = "flit.buildapi"
 requires = [
     "flit",
 ]
 
 [project]
+authors = [
+    "Author Name <author@email.com>",
+    { name = "Author Name" },
+    { name = "Kieran Ryan" },
+]
 name = "pyprojectsort"
 
 [tool.radon]
 exclude = "tests/*,venv/*"
 show_complexity = true
 show_mi = true
 total_average = true
@@ -111,12 +122,30 @@
 
 The **--check** option can be used to determine whether your file would be reformatted.
 
 ```console
 pyprojectsort --check
 ```
 
-If the file needs reformatting, the program exits with code 1. This is useful for [pipeline integration](https://github.com/kieran-ryan/pyprojectsort/blob/d9cf5e1e646e1e5260f7cf0168ecd0a05ce8ed11/.github/workflows/main.yml#L30) as it prevents writing back changes so a clean repository is maintained for subsequent jobs.
+If the file needs reformatting, the program exits with an error code. This is useful for [pipeline integration](https://github.com/kieran-ryan/pyprojectsort/blob/d9cf5e1e646e1e5260f7cf0168ecd0a05ce8ed11/.github/workflows/main.yml#L30) as it prevents writing back changes so that a clean repository is maintained for subsequent jobs.
+
+The **--diff** option provides similar functionality but also displays any changes that would be made.
+
+```console
+pyprojectsort --diff
+```
+
+The diff of an alphabetically reordered array will appear as follows:
+
+```diff
+@@ -6,8 +6,8 @@
+[project]
+authors = [
++ { name = "Author Name" },
+  { name = "Kieran Ryan" },
+- { name = "Author Name" },
+]
+```
 
 ## License
 
 `pyprojectsort` is licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `pyprojectsort-0.2.2/pyproject.toml` & `pyprojectsort-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,21 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
+    "natsort==8.4.0",
     "tomli-w==1.0.0",
     "tomli==2.0.1",
 ]
 description = "Formatter for pyproject.toml files"
 dynamic = [
     "version",
 ]
```

### Comparing `pyprojectsort-0.2.2/PKG-INFO` & `pyprojectsort-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 Metadata-Version: 2.1
 Name: pyprojectsort
-Version: 0.2.2
+Version: 0.3.0
 Summary: Formatter for pyproject.toml files
 Author: Kieran Ryan
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: natsort==8.4.0
 Requires-Dist: tomli-w==1.0.0
 Requires-Dist: tomli==2.0.1
 Project-URL: Documentation, https://kieran-ryan.github.io/pyprojectsort/
 Project-URL: Source, https://github.com/kieran-ryan/pyprojectsort
 Project-URL: Tracker, https://github.com/kieran-ryan/pyprojectsort/issues
 
 # pyprojectsort
 
-[![image](https://badge.fury.io/py/pyprojectsort.svg)](https://pypi.org/project/pyprojectsort/)
-![image](https://img.shields.io/badge/license-MIT-blue)
-[![image](https://img.shields.io/pypi/pyversions/pyprojectsort.svg)](https://pypi.python.org/pypi/pyprojectsort)
+[![PyPI Version](https://badge.fury.io/py/pyprojectsort.svg)](https://pypi.org/project/pyprojectsort/)
+![LICENSE](https://img.shields.io/badge/license-MIT-blue)
+[![Python versions](https://img.shields.io/pypi/pyversions/pyprojectsort.svg)](https://pypi.org/pypi/pyprojectsort)
 ![Supported platforms](https://img.shields.io/badge/platforms-macOS%20%7C%20Windows%20%7C%20Linux-green)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![Pipeline status](https://github.com/kieran-ryan/python-package-template/actions/workflows/main.yml/badge.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/kieran-ryan/pyprojectsort/main.svg)](https://results.pre-commit.ci/latest/github/kieran-ryan/pyprojectsort/main)
 
 Formatter for pyproject.toml files.
 
-This package enforces consistent formatting of pyproject.toml files, reducing merge request conflicts and saving time otherwise spent to format manually. It also contributes to a cleaner git history and more readable code; enhancing overall project organisation and maintainability. Experience a streamlined workflow, reduced errors, and improved code readability with `pyprojectsort`.
+This package enforces consistent formatting of pyproject.toml files, reducing merge request conflicts and saving time otherwise spent on manual formatting. It also contributes to a cleaner git history and more readable code; enhancing overall project organisation and maintainability. Experience a streamlined workflow, reduced errors, and improved code readability with `pyprojectsort`.
 
 ## Features
 
-- Alphabetically sorts pyproject.toml by:
+- Alphanumerically sorts pyproject.toml by:
   - section
   - section key
   - list value
 - Reformats pyproject.toml to a standardised style
   - line per list value
   - double quotations
   - trailing commas
@@ -54,15 +60,15 @@
 
 ### Using pyprojectsort with [pre-commit](https://pre-commit.com)
 
 To use as an automated git hook, add this to your `.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/kieran-ryan/pyprojectsort
-  rev: v0.2.1
+  rev: v0.2.2
   hooks:
     - id: pyprojectsort
 ```
 
 ## Examples
 
 With the following `pyproject.toml`:
@@ -72,14 +78,19 @@
 ignore = ["G004",
 "T201",
     "ANN"
 ]
 
 [project]
 name = 'pyprojectsort'
+authors = [
+    { name = "Kieran Ryan" },
+    "Author Name <author@email.com>",
+    {name="Author name"}
+]
 
 [tool.radon]
 show_mi = true
 exclude = "tests/*,venv/*"
 total_average = true
 show_complexity = true
 
@@ -100,14 +111,19 @@
 [build-system]
 build-backend = "flit.buildapi"
 requires = [
     "flit",
 ]
 
 [project]
+authors = [
+    "Author Name <author@email.com>",
+    { name = "Author Name" },
+    { name = "Kieran Ryan" },
+]
 name = "pyprojectsort"
 
 [tool.radon]
 exclude = "tests/*,venv/*"
 show_complexity = true
 show_mi = true
 total_average = true
@@ -130,13 +146,31 @@
 
 The **--check** option can be used to determine whether your file would be reformatted.
 
 ```console
 pyprojectsort --check
 ```
 
-If the file needs reformatting, the program exits with code 1. This is useful for [pipeline integration](https://github.com/kieran-ryan/pyprojectsort/blob/d9cf5e1e646e1e5260f7cf0168ecd0a05ce8ed11/.github/workflows/main.yml#L30) as it prevents writing back changes so a clean repository is maintained for subsequent jobs.
+If the file needs reformatting, the program exits with an error code. This is useful for [pipeline integration](https://github.com/kieran-ryan/pyprojectsort/blob/d9cf5e1e646e1e5260f7cf0168ecd0a05ce8ed11/.github/workflows/main.yml#L30) as it prevents writing back changes so that a clean repository is maintained for subsequent jobs.
+
+The **--diff** option provides similar functionality but also displays any changes that would be made.
+
+```console
+pyprojectsort --diff
+```
+
+The diff of an alphabetically reordered array will appear as follows:
+
+```diff
+@@ -6,8 +6,8 @@
+[project]
+authors = [
++ { name = "Author Name" },
+  { name = "Kieran Ryan" },
+- { name = "Author Name" },
+]
+```
 
 ## License
 
 `pyprojectsort` is licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

