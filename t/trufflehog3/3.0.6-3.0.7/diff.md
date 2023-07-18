# Comparing `tmp/trufflehog3-3.0.6.tar.gz` & `tmp/trufflehog3-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trufflehog3-3.0.6.tar", last modified: Thu Jan 19 20:40:07 2023, max compression
+gzip compressed data, was "trufflehog3-3.0.7.tar", last modified: Tue Jul 18 16:18:04 2023, max compression
```

## Comparing `trufflehog3-3.0.6.tar` & `trufflehog3-3.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-01-19 20:40:07.667145 trufflehog3-3.0.6/
--rw-r--r--   0 ekzo       (501) staff       (20)    18046 2021-08-06 20:47:08.000000 trufflehog3-3.0.6/LICENSE
--rw-r--r--   0 ekzo       (501) staff       (20)       29 2021-08-06 20:47:15.000000 trufflehog3-3.0.6/MANIFEST.in
--rw-r--r--   0 ekzo       (501) staff       (20)     3889 2023-01-19 20:40:07.667200 trufflehog3-3.0.6/PKG-INFO
--rw-r--r--   0 ekzo       (501) staff       (20)     3586 2021-11-05 21:19:44.000000 trufflehog3-3.0.6/README.md
--rw-r--r--   0 ekzo       (501) staff       (20)      229 2023-01-19 20:40:07.667408 trufflehog3-3.0.6/setup.cfg
--rw-r--r--   0 ekzo       (501) staff       (20)      791 2021-08-09 06:55:14.000000 trufflehog3-3.0.6/setup.py
-drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-01-19 20:40:07.666050 trufflehog3-3.0.6/trufflehog3/
--rw-r--r--   0 ekzo       (501) staff       (20)     1559 2023-01-19 20:37:28.000000 trufflehog3-3.0.6/trufflehog3/__init__.py
--rw-r--r--   0 ekzo       (501) staff       (20)      210 2021-08-06 20:47:15.000000 trufflehog3-3.0.6/trufflehog3/__main__.py
--rwxr-xr-x   0 ekzo       (501) staff       (20)     8559 2021-12-08 21:56:24.000000 trufflehog3-3.0.6/trufflehog3/cli.py
--rw-r--r--   0 ekzo       (501) staff       (20)     8414 2021-08-12 11:54:21.000000 trufflehog3-3.0.6/trufflehog3/core.py
--rw-r--r--   0 ekzo       (501) staff       (20)     4151 2021-08-06 20:47:15.000000 trufflehog3-3.0.6/trufflehog3/helper.py
--rw-r--r--   0 ekzo       (501) staff       (20)    15165 2021-08-07 14:45:16.000000 trufflehog3-3.0.6/trufflehog3/models.py
--rw-r--r--   0 ekzo       (501) staff       (20)     3765 2021-08-06 20:47:15.000000 trufflehog3-3.0.6/trufflehog3/render.py
--rw-r--r--   0 ekzo       (501) staff       (20)     6187 2021-08-06 20:47:15.000000 trufflehog3-3.0.6/trufflehog3/search.py
--rw-r--r--   0 ekzo       (501) staff       (20)     7413 2021-11-04 17:17:22.000000 trufflehog3-3.0.6/trufflehog3/source.py
-drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-01-19 20:40:07.667051 trufflehog3-3.0.6/trufflehog3/static/
--rw-r--r--   0 ekzo       (501) staff       (20)    18591 2021-08-06 20:47:15.000000 trufflehog3-3.0.6/trufflehog3/static/report.html.j2
--rw-r--r--   0 ekzo       (501) staff       (20)      960 2021-08-06 20:47:15.000000 trufflehog3-3.0.6/trufflehog3/static/report.text.j2
--rw-r--r--   0 ekzo       (501) staff       (20)     4195 2021-08-09 06:55:14.000000 trufflehog3-3.0.6/trufflehog3/static/rules.yml
-drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-01-19 20:40:07.666703 trufflehog3-3.0.6/trufflehog3.egg-info/
--rw-r--r--   0 ekzo       (501) staff       (20)     3889 2023-01-19 20:40:07.000000 trufflehog3-3.0.6/trufflehog3.egg-info/PKG-INFO
--rw-r--r--   0 ekzo       (501) staff       (20)      554 2023-01-19 20:40:07.000000 trufflehog3-3.0.6/trufflehog3.egg-info/SOURCES.txt
--rw-r--r--   0 ekzo       (501) staff       (20)        1 2023-01-19 20:40:07.000000 trufflehog3-3.0.6/trufflehog3.egg-info/dependency_links.txt
--rw-r--r--   0 ekzo       (501) staff       (20)       52 2023-01-19 20:40:07.000000 trufflehog3-3.0.6/trufflehog3.egg-info/entry_points.txt
--rw-r--r--   0 ekzo       (501) staff       (20)       60 2023-01-19 20:40:07.000000 trufflehog3-3.0.6/trufflehog3.egg-info/requires.txt
--rw-r--r--   0 ekzo       (501) staff       (20)       12 2023-01-19 20:40:07.000000 trufflehog3-3.0.6/trufflehog3.egg-info/top_level.txt
+drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-07-18 16:18:04.971227 trufflehog3-3.0.7/
+-rw-r--r--   0 ekzo       (501) staff       (20)    18046 2021-08-06 20:47:08.000000 trufflehog3-3.0.7/LICENSE
+-rw-r--r--   0 ekzo       (501) staff       (20)       29 2021-08-06 20:47:15.000000 trufflehog3-3.0.7/MANIFEST.in
+-rw-r--r--   0 ekzo       (501) staff       (20)     3889 2023-07-18 16:18:04.971277 trufflehog3-3.0.7/PKG-INFO
+-rw-r--r--   0 ekzo       (501) staff       (20)     3586 2021-11-05 21:19:44.000000 trufflehog3-3.0.7/README.md
+-rw-r--r--   0 ekzo       (501) staff       (20)      229 2023-07-18 16:18:04.971477 trufflehog3-3.0.7/setup.cfg
+-rw-r--r--   0 ekzo       (501) staff       (20)      791 2021-08-09 06:55:14.000000 trufflehog3-3.0.7/setup.py
+drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-07-18 16:18:04.970062 trufflehog3-3.0.7/trufflehog3/
+-rw-r--r--   0 ekzo       (501) staff       (20)     1559 2023-07-18 16:15:40.000000 trufflehog3-3.0.7/trufflehog3/__init__.py
+-rw-r--r--   0 ekzo       (501) staff       (20)      210 2021-08-06 20:47:15.000000 trufflehog3-3.0.7/trufflehog3/__main__.py
+-rwxr-xr-x   0 ekzo       (501) staff       (20)     8559 2021-12-08 21:56:24.000000 trufflehog3-3.0.7/trufflehog3/cli.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     8414 2021-08-12 11:54:21.000000 trufflehog3-3.0.7/trufflehog3/core.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     4151 2021-08-06 20:47:15.000000 trufflehog3-3.0.7/trufflehog3/helper.py
+-rw-r--r--   0 ekzo       (501) staff       (20)    15165 2021-08-07 14:45:16.000000 trufflehog3-3.0.7/trufflehog3/models.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     3765 2021-08-06 20:47:15.000000 trufflehog3-3.0.7/trufflehog3/render.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     6187 2021-08-06 20:47:15.000000 trufflehog3-3.0.7/trufflehog3/search.py
+-rw-r--r--   0 ekzo       (501) staff       (20)     7413 2021-11-04 17:17:22.000000 trufflehog3-3.0.7/trufflehog3/source.py
+drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-07-18 16:18:04.971111 trufflehog3-3.0.7/trufflehog3/static/
+-rw-r--r--   0 ekzo       (501) staff       (20)    18591 2021-08-06 20:47:15.000000 trufflehog3-3.0.7/trufflehog3/static/report.html.j2
+-rw-r--r--   0 ekzo       (501) staff       (20)      960 2021-08-06 20:47:15.000000 trufflehog3-3.0.7/trufflehog3/static/report.text.j2
+-rw-r--r--   0 ekzo       (501) staff       (20)     4195 2021-08-09 06:55:14.000000 trufflehog3-3.0.7/trufflehog3/static/rules.yml
+drwxr-xr-x   0 ekzo       (501) staff       (20)        0 2023-07-18 16:18:04.970764 trufflehog3-3.0.7/trufflehog3.egg-info/
+-rw-r--r--   0 ekzo       (501) staff       (20)     3889 2023-07-18 16:18:04.000000 trufflehog3-3.0.7/trufflehog3.egg-info/PKG-INFO
+-rw-r--r--   0 ekzo       (501) staff       (20)      554 2023-07-18 16:18:04.000000 trufflehog3-3.0.7/trufflehog3.egg-info/SOURCES.txt
+-rw-r--r--   0 ekzo       (501) staff       (20)        1 2023-07-18 16:18:04.000000 trufflehog3-3.0.7/trufflehog3.egg-info/dependency_links.txt
+-rw-r--r--   0 ekzo       (501) staff       (20)       52 2023-07-18 16:18:04.000000 trufflehog3-3.0.7/trufflehog3.egg-info/entry_points.txt
+-rw-r--r--   0 ekzo       (501) staff       (20)       60 2023-07-18 16:18:04.000000 trufflehog3-3.0.7/trufflehog3.egg-info/requires.txt
+-rw-r--r--   0 ekzo       (501) staff       (20)       12 2023-07-18 16:18:04.000000 trufflehog3-3.0.7/trufflehog3.egg-info/top_level.txt
```

### Comparing `trufflehog3-3.0.6/LICENSE` & `trufflehog3-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/PKG-INFO` & `trufflehog3-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trufflehog3
-Version: 3.0.6
+Version: 3.0.7
 Summary: Find secrets in your codebase
 Home-page: https://github.com/feeltheajf/trufflehog3
 Author: Ilya Radostev
 Author-email: feeltheajf@gmail.com
 License: GNU
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trufflehog3 Version: 3.0.6 Summary: Find secrets in
+Metadata-Version: 2.1 Name: trufflehog3 Version: 3.0.7 Summary: Find secrets in
 your codebase Home-page: https://github.com/feeltheajf/trufflehog3 Author: Ilya
 Radostev Author-email: feeltheajf@gmail.com License: GNU Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE [![Package
 Version](https://img.shields.io/pypi/v/trufflehog3.svg)](https://pypi.org/
 project/trufflehog3) ![Python Version](https://img.shields.io/badge/python-3.7-
 informational.svg) [![Downloads](https://pepy.tech/badge/trufflehog3)](https://
 pepy.tech/project/trufflehog3) [![Tests](https://github.com/feeltheajf/
```

### Comparing `trufflehog3-3.0.6/README.md` & `trufflehog3-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/setup.py` & `trufflehog3-3.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/__init__.py` & `trufflehog3-3.0.7/trufflehog3/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 
 from pathlib import Path
 
 from trufflehog3 import helper
 
 __NAME__ = "trufflehog3"
-__VERSION__ = "3.0.6"
+__VERSION__ = "3.0.7"
 
 HERE = Path(__file__).parent
 STATIC_DIR = HERE / "static"
 HTML_TEMPLATE_FILE = "report.html.j2"
 TEXT_TEMPLATE_FILE = "report.text.j2"
 DEFAULT_RULES_FILE = STATIC_DIR / "rules.yml"
```

### Comparing `trufflehog3-3.0.6/trufflehog3/cli.py` & `trufflehog3-3.0.7/trufflehog3/cli.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/core.py` & `trufflehog3-3.0.7/trufflehog3/core.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/helper.py` & `trufflehog3-3.0.7/trufflehog3/helper.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/models.py` & `trufflehog3-3.0.7/trufflehog3/models.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/render.py` & `trufflehog3-3.0.7/trufflehog3/render.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/search.py` & `trufflehog3-3.0.7/trufflehog3/search.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/source.py` & `trufflehog3-3.0.7/trufflehog3/source.py`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/static/report.html.j2` & `trufflehog3-3.0.7/trufflehog3/static/report.html.j2`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/static/report.text.j2` & `trufflehog3-3.0.7/trufflehog3/static/report.text.j2`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3/static/rules.yml` & `trufflehog3-3.0.7/trufflehog3/static/rules.yml`

 * *Files identical despite different names*

### Comparing `trufflehog3-3.0.6/trufflehog3.egg-info/PKG-INFO` & `trufflehog3-3.0.7/trufflehog3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trufflehog3
-Version: 3.0.6
+Version: 3.0.7
 Summary: Find secrets in your codebase
 Home-page: https://github.com/feeltheajf/trufflehog3
 Author: Ilya Radostev
 Author-email: feeltheajf@gmail.com
 License: GNU
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trufflehog3 Version: 3.0.6 Summary: Find secrets in
+Metadata-Version: 2.1 Name: trufflehog3 Version: 3.0.7 Summary: Find secrets in
 your codebase Home-page: https://github.com/feeltheajf/trufflehog3 Author: Ilya
 Radostev Author-email: feeltheajf@gmail.com License: GNU Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE [![Package
 Version](https://img.shields.io/pypi/v/trufflehog3.svg)](https://pypi.org/
 project/trufflehog3) ![Python Version](https://img.shields.io/badge/python-3.7-
 informational.svg) [![Downloads](https://pepy.tech/badge/trufflehog3)](https://
 pepy.tech/project/trufflehog3) [![Tests](https://github.com/feeltheajf/
```

### Comparing `trufflehog3-3.0.6/trufflehog3.egg-info/SOURCES.txt` & `trufflehog3-3.0.7/trufflehog3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

