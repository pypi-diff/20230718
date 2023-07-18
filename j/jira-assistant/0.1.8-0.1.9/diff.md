# Comparing `tmp/jira-assistant-0.1.8.tar.gz` & `tmp/jira-assistant-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira-assistant-0.1.8.tar", last modified: Fri Apr 14 15:33:14 2023, max compression
+gzip compressed data, was "jira-assistant-0.1.9.tar", last modified: Thu Apr 20 08:59:21 2023, max compression
```

## Comparing `jira-assistant-0.1.8.tar` & `jira-assistant-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.622610 jira-assistant-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.622610 jira-assistant-0.1.8/src/jira_assistant/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/src/jira_assistant/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/assets/excel_definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/assets/sprint_schedule.json
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15774 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/story.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/src/jira_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:59:21.653933 jira-assistant-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-04-20 08:59:21.653933 jira-assistant-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 08:59:21.653933 jira-assistant-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:59:21.645933 jira-assistant-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:59:21.649933 jira-assistant-0.1.9/src/jira_assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:59:21.649933 jira-assistant-0.1.9/src/jira_assistant/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/assets/excel_definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/assets/sprint_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24102 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15971 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/src/jira_assistant/story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:59:21.649933 jira-assistant-0.1.9/src/jira_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-04-20 08:59:21.000000 jira-assistant-0.1.9/src/jira_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-20 08:59:21.000000 jira-assistant-0.1.9/src/jira_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:59:21.000000 jira-assistant-0.1.9/src/jira_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 08:59:21.000000 jira-assistant-0.1.9/src/jira_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-20 08:59:21.000000 jira-assistant-0.1.9/src/jira_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 08:59:21.000000 jira-assistant-0.1.9/src/jira_assistant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:59:21.649933 jira-assistant-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/tests/test_console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/tests/test_excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/tests/test_excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/tests/test_jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/tests/test_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/tests/test_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/tests/test_sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-20 08:58:58.000000 jira-assistant-0.1.9/tests/test_story.py
```

### Comparing `jira-assistant-0.1.8/LICENSE` & `jira-assistant-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/PKG-INFO` & `jira-assistant-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-assistant
-Version: 0.1.8
+Version: 0.1.9
 Summary: Useful Jira tools
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,29 +28,31 @@
 Project-URL: Documentation, https://jira-assistant.readthedocs.io/en/stable
 Project-URL: Source, https://github.com/SharryXu/jira-assistant
 Project-URL: Tracker, https://github.com/SharryXu/jira-assistant/issues
 Keywords: jira,excel,sorting,project management,tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 Jira Assistant - userful jira tools
 =============================================
 
@@ -68,24 +70,24 @@
     :target: https://img.shields.io/github/repo-size/sharryxu/jira-assistant
     :alt: Package Size
 
 .. |GitHubIssues| image:: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :target: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :alt: GitHub issues
 
-.. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml/badge.svg
-    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml
+.. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-linux-test.yml/badge.svg
+    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-linux-test.yml
     :alt: python 3.11 (Linux)
 
-.. |Mac OS| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml/badge.svg
-    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml
+.. |Mac OS| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-macos-test.yml/badge.svg
+    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-macos-test.yml
     :alt: python 3.11 (Mac OS)
 
-.. |Windows| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-windows-test.yml/badge.svg
-    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-windows-test.yml
+.. |Windows| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-windows-test.yml/badge.svg
+    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-windows-test.yml
     :alt: python 3.11 (Windows)
 
 .. |Pylint| image:: https://github.com/sharryxu/jira-assistant/actions/workflows/pylint.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/pylint.yml
     :alt: Pylint 
 
 .. |CodeQL| image:: https://github.com/sharryxu/jira-assistant/workflows/CodeQL/badge.svg
```

### Comparing `jira-assistant-0.1.8/README.rst` & `jira-assistant-0.1.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     :target: https://img.shields.io/github/repo-size/sharryxu/jira-assistant
     :alt: Package Size
 
 .. |GitHubIssues| image:: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :target: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :alt: GitHub issues
 
-.. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml/badge.svg
-    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml
+.. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-linux-test.yml/badge.svg
+    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-linux-test.yml
     :alt: python 3.11 (Linux)
 
-.. |Mac OS| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml/badge.svg
-    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml
+.. |Mac OS| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-macos-test.yml/badge.svg
+    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-macos-test.yml
     :alt: python 3.11 (Mac OS)
 
-.. |Windows| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-windows-test.yml/badge.svg
-    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-windows-test.yml
+.. |Windows| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-windows-test.yml/badge.svg
+    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-windows-test.yml
     :alt: python 3.11 (Windows)
 
 .. |Pylint| image:: https://github.com/sharryxu/jira-assistant/actions/workflows/pylint.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/pylint.yml
     :alt: Pylint 
 
 .. |CodeQL| image:: https://github.com/sharryxu/jira-assistant/workflows/CodeQL/badge.svg
```

### Comparing `jira-assistant-0.1.8/pyproject.toml` & `jira-assistant-0.1.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jira-assistant"
 authors = [{ name = "Sharry Xu", email = "sharry.xu@outlook.com" }]
 description = "Useful Jira tools"
 readme = "README.rst"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Development Status :: 6 - Mature",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
@@ -32,17 +34,19 @@
 dependencies = [
     "openpyxl >= 3.0.10",
     "python-dateutil >= 2.8.2",
     "python-dotenv >= 0.21.1",
     "requests >= 2.28.2",
     "jira >= 3.5.0",
     'tomli; python_version < "3.11"',
+    'importlib_resources; python_version < "3.8"',
+    'importlib_metadata; python_version < "3.8"',
     'requests-mock >= 1.10.0'
 ]
-version = "0.1.8"
+version = "0.1.9"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "pylint"]
 
 [project.urls]
 Documentation = "https://jira-assistant.readthedocs.io/en/stable"
 Source = "https://github.com/SharryXu/jira-assistant"
```

### Comparing `jira-assistant-0.1.8/src/jira_assistant/__init__.py` & `jira-assistant-0.1.9/src/jira_assistant/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # -*- coding: utf-8 -*-
 """
 This module is used to list all exported classes/methods.
 """
-from importlib import metadata
-from importlib.metadata import version
+try:
+    from importlib import metadata
+except ImportError:
+    import importlib_metadata as metadata
 
 from .console_script import generate_template, process_excel_file, update_jira_info
 from .excel_definition import ExcelDefinition, ExcelDefinitionColumn
 from .excel_operation import (
     output_to_csv_file,
     output_to_excel_file,
     read_excel_file,
     run_steps_and_sort_excel_file,
 )
 from .milestone import Milestone
 from .priority import Priority
 from .sprint_schedule import SprintScheduleStore
 from .story import Story, StoryFactory
 
-__version__ = version("jira_assistant")
+__version__ = metadata.version("jira_assistant")
 
 __all__ = [
     "ExcelDefinition",
     "ExcelDefinitionColumn",
     "read_excel_file",
     "output_to_csv_file",
     "output_to_excel_file",
@@ -32,9 +34,7 @@
     "SprintScheduleStore",
     "Story",
     "StoryFactory",
     "process_excel_file",
     "generate_template",
     "update_jira_info",
 ]
-
-del metadata
```

### Comparing `jira-assistant-0.1.8/src/jira_assistant/assets/excel_definition.json` & `jira-assistant-0.1.9/src/jira_assistant/assets/excel_definition.json`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/src/jira_assistant/assets/sprint_schedule.json` & `jira-assistant-0.1.9/src/jira_assistant/assets/sprint_schedule.json`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/src/jira_assistant/console_script.py` & `jira-assistant-0.1.9/src/jira_assistant/console_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 This module is used to provide the console program.
 """
 import os
 import pathlib
 import sys
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
 from datetime import datetime
-from importlib.resources import files
 from pathlib import Path
 from shutil import copyfile
 from typing import Optional
 from urllib.parse import ParseResult, urlparse
 
 from dotenv import set_key
 
@@ -21,14 +20,15 @@
 __all__ = ["process_excel_file", "generate_template", "update_jira_info"]
 
 
 def get_args_for_process_excel_file() -> Namespace:
     parser = ArgumentParser(
         description="Jira tool: Used to pre-process and sort stories",
         formatter_class=ArgumentDefaultsHelpFormatter,
+        allow_abbrev=False,
     )
 
     parser.add_argument(
         "input_file", metavar="input_file", type=pathlib.Path, help="Source Excel file."
     )
     parser.add_argument(
         "-o",
@@ -189,15 +189,15 @@
 
 def generate_template():
     try:
         args = get_args_for_generate_template()
 
         template_type: str = str(args.template_type).lower()
 
-        result: Path | None = None
+        result: Optional[Path] = None
         if template_type == "excel":
             result = _generate_excel_template(
                 _generate_timestamp_filename("excel-template", ".xlsx")
             )
         elif template_type == "excel-definition":
             result = copyfile(
                 SRC_ASSETS / "excel_definition.json",
@@ -229,16 +229,16 @@
         Path.cwd()
         / f'{prefix}-{datetime.now().strftime("%y-%m-%d-%H-%M-%S")}{extension}'
     ).resolve()
 
 
 def _generate_excel_template(output_file: "Path") -> Optional[Path]:
     try:
-        excel_definition = ExcelDefinition().load(
-            files("jira_assistant.assets").joinpath("excel_definition.json").read_text()
+        excel_definition = ExcelDefinition().load_file(
+            SRC_ASSETS / "excel_definition.json"
         )
         output_to_excel_file(output_file, [], excel_definition)
         return output_file
     except Exception as e:
         print(e)
         return None
```

### Comparing `jira-assistant-0.1.8/src/jira_assistant/excel_definition.py` & `jira-assistant-0.1.9/src/jira_assistant/excel_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # -*- coding: utf-8 -*-
 """
 This module is used to store excel column definition information.
 """
-import json
+from __future__ import annotations
+
 import pathlib
 import re
 from copy import deepcopy
 from datetime import datetime
+from json import loads
+from json.decoder import JSONDecodeError
 from pathlib import Path
-from types import NoneType
-from typing import Any, Optional, TypedDict, Union
+from typing import Any, List, Optional, Set, TypedDict, Union
 
 from .milestone import Milestone
 from .priority import Priority
 
 __all__ = ["ExcelDefinition"]
 
 RaiseRankingLevelScopeIndexValidationRule = re.compile(
@@ -66,15 +68,15 @@
         enabled=pre_process_step_enabled,
         config=pre_process_step_config,
     )
 
 
 class SortStrategy(TypedDict):
     name: str
-    priority: int | NoneType
+    priority: Optional[int]
     enabled: bool
     config: dict
 
 
 def parse_json_item_to_sort_strategy(json_item: Any) -> SortStrategy:
     strategy_name = ""
     strategy_priority = 0
@@ -128,23 +130,23 @@
         config=strategy_config,
     )
 
 
 class ExcelDefinitionColumn(TypedDict):
     index: int
     name: str
-    type: type | NoneType
+    type: Optional[type]
     require_sort: bool
     sort_order: bool
     scope_require_sort: bool
     scope_sort_order: bool
     inline_weights: int
     raise_ranking: int
     scope_raise_ranking: int
-    jira_field_mapping: dict[str, str] | NoneType
+    jira_field_mapping: Optional[dict[str, str]]
 
 
 def parse_json_item_to_excel_definition_column(json_item: Any) -> ExcelDefinitionColumn:
     column_index = 0
     column_name = ""
     column_type = None
     column_require_sort = False
@@ -223,49 +225,65 @@
             JSON string content
         """
 
         if content is None:
             raise ValueError("There is no content in the excel definition file.")
 
         try:
-            raw_data = json.loads(content)
+            raw_data = loads(content)
+        except JSONDecodeError as e:
+            raise SyntaxError(
+                f"The structure of excel definition file is wrong. Hint: {e.msg} in line {e.lineno}:{e.colno}."
+            ) from e
 
-            if len(raw_data) > 0:
-                if raw_data[0].get("PreProcessSteps", None) is not None:
-                    for item in raw_data[0]["PreProcessSteps"]:
+        parse_errors = []
+
+        if len(raw_data) > 0:
+            if raw_data[0].get("PreProcessSteps", None) is not None:
+                for item in raw_data[0]["PreProcessSteps"]:
+                    try:
                         self.pre_process_steps.append(
                             parse_json_item_to_pre_process_step(item)
                         )
+                    except (TypeError, ValueError) as e:
+                        parse_errors.append(e.args[0])
 
-                if raw_data[0].get("SortStrategies", None) is not None:
-                    for item in raw_data[0]["SortStrategies"]:
+            if raw_data[0].get("SortStrategies", None) is not None:
+                for item in raw_data[0]["SortStrategies"]:
+                    try:
                         self.sort_strategies.append(
                             parse_json_item_to_sort_strategy(item)
                         )
+                    except (TypeError, ValueError) as e:
+                        parse_errors.append(e.args[0])
 
-            if len(raw_data) >= 1:
-                for item in raw_data[1]["Columns"]:
+        if len(raw_data) >= 1:
+            for item in raw_data[1]["Columns"]:
+                try:
                     self.columns.append(
                         parse_json_item_to_excel_definition_column(item)
                     )
-        except TypeError:
-            raise
-        except ValueError:
-            raise
-        except Exception as e:
-            raise ValueError(
-                "The JSON structure of the excel definition file is wrong. Please check the documentation: https://github.com/SharryXu/jira-assistant"
-            ) from e
+                except (TypeError, ValueError) as e:
+                    parse_errors.append(e.args[0])
+
+        if parse_errors:
+            # Avoid duplicate error messages.
+            parse_error_message = "\n".join(
+                [f"{index + 1}. {err}" for index, err in enumerate(set(parse_errors))]
+            )
+            raise SyntaxError(
+                f"The excel definition file has below issues need to be fixed:\n{parse_error_message}"
+            )
 
         return self
 
     @staticmethod
     def parse_raise_ranking_level_scope_index_expression(
         expression: Union[Any, None],
-    ) -> Optional[set[int]]:
+    ) -> Optional[Set[int]]:
         if expression is None or not isinstance(expression, str):
             return None
         if len(expression) == 0 or expression.isspace():
             return set()
         if (
             RaiseRankingLevelScopeIndexValidationRule.fullmatch(
                 "".join(expression.split(" "))
@@ -299,22 +317,22 @@
             try:
                 self.load(table_definition_file.read())
             finally:
                 table_definition_file.close()
 
         return self
 
-    def validate(self) -> "list":
+    def validate(self) -> "List":
         return (
             self._validate_pre_process_steps()
             + self._validate_sort_strategies()
             + self._validate_column_definitions()
         )
 
-    def _validate_pre_process_steps(self) -> "list[str]":
+    def _validate_pre_process_steps(self) -> "List[str]":
         invalid_definitions = []
 
         # Validate PreProcessSteps
         for pre_process_step in self.pre_process_steps:
             if pre_process_step["name"].isspace() or len(pre_process_step["name"]) == 0:
                 invalid_definitions.append("The PreProcessStep name is invalid.")
                 # If strategy name is invalid, no need to check more.
@@ -335,15 +353,15 @@
             ] and not isinstance(pre_process_step["config"]["JiraStatuses"], list):
                 invalid_definitions.append(
                     f"The format of the Jira Statuses is invalid. PreProcessStep: {pre_process_step['name']}. Supported format like: ['CLOSED', 'PENDING RELEASE']."
                 )
 
         return invalid_definitions
 
-    def _validate_sort_strategies(self) -> "list[str]":
+    def _validate_sort_strategies(self) -> "List[str]":
         invalid_definitions = []
 
         # Validate Strategies
         strategy_priorities: list[int] = []
         for strategy in self.sort_strategies:
             if strategy["name"].isspace() or len(strategy["name"]) == 0:
                 invalid_definitions.append("The strategy name is invalid.")
@@ -381,33 +399,33 @@
         if len(strategy_priorities) != len(set(strategy_priorities)):
             invalid_definitions.append(
                 "The priority of strategies cannot be duplicate."
             )
 
         return invalid_definitions
 
-    def _validate_column_definitions(self) -> "list[str]":
+    def _validate_column_definitions(self) -> "List[str]":
         invalid_definitions = []
 
         # Validate the Columns
         exist_story_id = False
         exist_indexes = []
         exist_inline_weights = []
         for column in self.get_columns():
             column_index: int = column["index"]
             column_name: str = column["name"]
-            column_type: type | None = column["type"]
+            column_type: Optional[type] = column["type"]
             column_require_sort: bool = column["require_sort"]
             column_sort_order: bool = column["sort_order"]
             column_scope_require_sort: bool = column["scope_require_sort"]
             column_scope_sort_order: bool = column["scope_sort_order"]
             column_inline_weights: int = column["inline_weights"]
             column_raise_ranking: int = column["raise_ranking"]
             column_scope_raise_ranking: int = column["scope_raise_ranking"]
-            column_jira_field_mapping: dict | None = column["jira_field_mapping"]
+            column_jira_field_mapping: Optional[dict] = column["jira_field_mapping"]
 
             # Check Name cannot be empty
             if len(column_name) == 0:
                 invalid_definitions.append(
                     f"Column name cannot be empty. Index: {column_index}"
                 )
                 continue
@@ -557,33 +575,33 @@
             return float
         return None
 
     def __iter__(self):
         for item in self.columns:
             yield item
 
-    def get_columns(self) -> "list[ExcelDefinitionColumn]":
+    def get_columns(self) -> "List[ExcelDefinitionColumn]":
         return deepcopy(self.columns)
 
-    def get_columns_name(self) -> "list[str | None]":
+    def get_columns_name(self) -> "List[Optional[str]]":
         return [item["name"] for item in self.columns]
 
     @property
     def max_column_index(self) -> int:
         return self.columns[len(self.columns) - 1]["index"]
 
-    def get_sort_strategies(self, enabled: bool = True) -> "list[SortStrategy]":
+    def get_sort_strategies(self, enabled: bool = True) -> "List[SortStrategy]":
         result: list[SortStrategy] = []
         for sort_strategy in self.sort_strategies:
             if sort_strategy["enabled"] == enabled:
                 result.append(deepcopy(sort_strategy))
         result.sort(key=_sort_priority_map, reverse=False)
         return result
 
-    def get_pre_process_steps(self, enabled: bool = True) -> "list[PreProcessStep]":
+    def get_pre_process_steps(self, enabled: bool = True) -> "List[PreProcessStep]":
         result: list[PreProcessStep] = []
         for pre_process_step in self.pre_process_steps:
             if pre_process_step["enabled"] == enabled:
                 result.append(deepcopy(pre_process_step))
         return result
 
     def total_count(self):
```

### Comparing `jira-assistant-0.1.8/src/jira_assistant/excel_operation.py` & `jira-assistant-0.1.9/src/jira_assistant/excel_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 This module offers a set of operations that user can modify their excel files.
 """
 import pathlib
 import warnings
-from importlib.resources import files
+
+try:
+    from importlib.resources import files
+except ImportError:
+    from importlib_resources import files
+
 from os import environ, remove
 from pathlib import Path
-from typing import Optional, Union
+from typing import List, Optional, Tuple, Union
 
 import openpyxl
 from dotenv import load_dotenv
 from openpyxl.workbook import Workbook
 from openpyxl.worksheet._read_only import ReadOnlyWorksheet
 from openpyxl.worksheet.worksheet import Worksheet
 from urllib3 import disable_warnings
@@ -43,15 +48,15 @@
 ASSETS = HERE / "assets"
 
 
 def read_excel_file(
     file: Union[str, Path],
     excel_definition: ExcelDefinition,
     sprint_schedule: SprintScheduleStore,
-) -> tuple[list[str], list[Story]]:
+) -> Tuple[List[str], List[Story]]:
     """
     Read and parse the excel file
 
     :parm file:
         The excel file that you want to read
 
     :parm excel_definition:
@@ -91,15 +96,15 @@
         # the range of the actual count.
         column_count = min(excel_definition.max_column_index, sheet.max_column)
 
         if sheet.max_row < 2:
             work_book.close()
             return ([], [])
 
-        columns: list[str] = []
+        columns: List[str] = []
 
         for column_index in range(1, column_count + 1):
             columns.append(str(sheet.cell(row=1, column=column_index).value))
 
         stories = []
 
         excel_definition_columns = excel_definition.get_columns()
@@ -135,15 +140,15 @@
     if first_cell_value is None or len(str(first_cell_value)) == 0:
         return True
     return False
 
 
 def output_to_csv_file(
     file: Union[str, Path],
-    stories: "list[Story]",
+    stories: "List[Story]",
     over_write: bool = True,
 ):
     if file is None or not pathlib.Path(file).is_absolute():
         raise ValueError("The file is invalid.")
 
     if pathlib.Path(file).exists():
         if over_write is True:
@@ -154,17 +159,17 @@
     with open(file, mode="x+", encoding="utf-8") as csv_file:
         for story in stories:
             csv_file.writelines([str(story)])
 
 
 def output_to_excel_file(
     file: Union[str, Path],
-    stories: "list[Story]",
+    stories: "List[Story]",
     excel_definition: ExcelDefinition,
-    columns_in_excel: Optional[list[str]] = None,
+    columns_in_excel: Optional[List[str]] = None,
     over_write: bool = True,
 ):
     """
     Generate excel file
 
     :parm file:
         Output excel file name including the path
@@ -217,40 +222,40 @@
 
     for column_index, column in enumerate(columns):
         cell = sheet.cell(row=1, column=column_index + 1)
         # There are three kinds of Cells. Only the Cell has the value attribute.
         if hasattr(cell, "value"):
             setattr(cell, "value", column)
 
-    if stories is not None:
+    if stories is not None and stories:
         for row_index, story in enumerate(stories):
             for column in excel_definition_columns:
                 if column["name"] is None:
                     continue
                 cell = sheet.cell(row=row_index + 2, column=column["index"])
                 if hasattr(cell, "value"):
                     setattr(cell, "value", story.format_value(column["name"]))
 
     work_book.save(str(file))
     work_book.close()
 
 
 def _query_jira_information(
-    stories: list[Story], excel_definition: ExcelDefinition
+    stories: List[Story], excel_definition: ExcelDefinition
 ) -> bool:
     load_dotenv(ASSETS / ".env")
 
-    jira_url: str | None = environ.get("JIRA_URL", default=None)
+    jira_url: Optional[str] = environ.get("JIRA_URL", default=None)
     if jira_url is None or jira_url.isspace() or len(jira_url) == 0:
         print(
             "The jira url is invalid. Please use the update-jira-info command to add/update url."
         )
         return False
 
-    jira_acccess_token: str | None = environ.get("JIRA_ACCESS_TOKEN", default=None)
+    jira_acccess_token: Optional[str] = environ.get("JIRA_ACCESS_TOKEN", default=None)
     if (
         jira_acccess_token is None
         or jira_acccess_token.isspace()
         or len(jira_acccess_token) == 0
     ):
         print(
             "The jira access token is invalid. Please use the update-jira-info command to add/update token."
@@ -338,25 +343,29 @@
 
     :parm over_write:
         Whether or not the exist output file will be over-write.
     """
     sprint_schedule = SprintScheduleStore()
     if sprint_schedule_file is None:
         sprint_schedule.load(
-            files("jira_assistant.assets").joinpath("sprint_schedule.json").read_text()
+            files("jira_assistant.assets")
+            .joinpath("sprint_schedule.json")
+            .read_text(encoding="utf-8")
         )
         print("Using default sprint schedule...")
     else:
         sprint_schedule.load_file(sprint_schedule_file)
         print("Using custom sprint schedule...")
 
     excel_definition = ExcelDefinition()
     if excel_definition_file is None:
         excel_definition.load(
-            files("jira_assistant.assets").joinpath("excel_definition.json").read_text()
+            files("jira_assistant.assets")
+            .joinpath("excel_definition.json")
+            .read_text(encoding="utf-8")
         )
         print("Using default excel definition...")
     else:
         excel_definition.load_file(excel_definition_file)
         print("Using custom excel definition...")
 
     validation_result = excel_definition.validate()
@@ -386,15 +395,15 @@
             need_call_jira_api: bool = False
             for excel_definition_column in excel_definition.get_columns():
                 if excel_definition_column["jira_field_mapping"] is not None:
                     need_call_jira_api = True
                     break
 
             if need_call_jira_api:
-                stories_need_call_jira: list[Story] = []
+                stories_need_call_jira: List[Story] = []
                 for story in stories:
                     if story.need_sort:
                         stories_need_call_jira.append(story)
                 if not _query_jira_information(
                     stories_need_call_jira, excel_definition
                 ):
                     print("Retrieve jira information failed.")
```

### Comparing `jira-assistant-0.1.8/src/jira_assistant/jira_client.py` & `jira-assistant-0.1.9/src/jira_assistant/jira_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 This module is used to store excel column definition information.
 """
 import warnings
-from typing import Any
+from typing import Any, Dict, List
 
 from jira import JIRA, JIRAError
 from urllib3 import disable_warnings
 
 # Currently, the openpyxl package will report an obsolete warning.
 warnings.simplefilter(action="ignore", category=UserWarning)
 # Disable the HTTPS certificate verification warning.
@@ -28,27 +28,29 @@
             if self.jira.myself() is not None:
                 return True
             return False
         except JIRAError:
             return False
 
     def get_stories_detail(
-        self, story_ids: list[str], jira_fields: list[dict[str, str]]
-    ) -> "dict[str, dict[str, str]]":
+        self, story_ids: List[str], jira_fields: List[Dict[str, str]]
+    ) -> "Dict[str, Dict[str, str]]":
         final_result = {}
         batch_size = 200
 
         try:
             if len(story_ids) > batch_size:
                 start_index = 0
                 end_index = batch_size
                 while end_index <= len(story_ids) and start_index < len(story_ids):
                     # print(f"Start: {start_index}, End: {end_index}")
-                    final_result = final_result | self._internal_get_stories_detail(
-                        story_ids[start_index:end_index], jira_fields
+                    final_result.update(
+                        self._internal_get_stories_detail(
+                            story_ids[start_index:end_index], jira_fields
+                        )
                     )
                     start_index = end_index
                     if start_index + batch_size < len(story_ids):
                         end_index = start_index + batch_size
                     else:
                         end_index = start_index + (len(story_ids) - end_index)
                 return final_result
@@ -58,20 +60,20 @@
             print(
                 f"Calling JIRA API failed. HttpStatusCode: {e.status_code}. Response: {e.response.json()}"
             )
 
             return {}
 
     def _internal_get_stories_detail(
-        self, story_ids: list[str], jira_fields: list[dict[str, str]]
-    ) -> "dict[str, dict[str, str]]":
+        self, story_ids: List[str], jira_fields: List[Dict[str, str]]
+    ) -> "Dict[str, Dict[str, str]]":
         id_query = ",".join([f"'{str(story_id)}'" for story_id in story_ids])
 
         try:
-            search_result: dict[str, Any] = self.jira.search_issues(
+            search_result: Dict[str, Any] = self.jira.search_issues(
                 jql_str=f"id in ({id_query})",
                 maxResults=len(story_ids),
                 fields=[field["jira_name"] for field in jira_fields],
                 json_result=True,
             )  # type: ignore
 
             final_result = {}
```

### Comparing `jira-assistant-0.1.8/src/jira_assistant/milestone.py` & `jira-assistant-0.1.9/src/jira_assistant/milestone.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/src/jira_assistant/priority.py` & `jira-assistant-0.1.9/src/jira_assistant/priority.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/src/jira_assistant/sprint_schedule.py` & `jira-assistant-0.1.9/src/jira_assistant/sprint_schedule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-import json
 import pathlib
+from json import loads
+from json.decoder import JSONDecodeError
 from pathlib import Path
-from typing import Union
+from typing import List, Union
 
 __all__ = ["SprintScheduleStore"]
 
 
 class SprintScheduleStore:
     def __init__(self) -> None:
-        self.store: list[tuple] = []
+        self.store: List[tuple] = []
 
     def load(self, content: str):
         """
         Load json string to generate the priority list
 
         :param content:
             JSON string content
         """
         if content is None:
             return
 
         try:
-            raw_data = json.loads(content)
+            raw_data = loads(content)
+        except JSONDecodeError as e:
+            raise SyntaxError(
+                f"The structure of sprint schedule file is wrong. Hint: {e.msg} in line {e.lineno}:{e.colno}."
+            ) from e
 
+        priority = 0
+        sprints = []
+        for item in raw_data:
+            for key, value in item.items():
+                if key.lower() in "priority":
+                    if value is None or not isinstance(value, int):
+                        # Just skip invalid items.
+                        continue
+                    priority = value
+                if key.lower() in "sprints":
+                    if value is None or not isinstance(value, list):
+                        continue
+                    for sprint in value:
+                        if len(sprint) > 0:
+                            sprints.append(sprint)
+
+            for sprint in sprints:
+                self.store.append((sprint, priority))
+            sprints.clear()
             priority = 0
-            sprints = []
-            for item in raw_data:
-                for key, value in item.items():
-                    if key.lower() in "priority":
-                        priority = value
-                    if key.lower() in "sprints":
-                        for sprint in value:
-                            if len(sprint) > 0:
-                                sprints.append(sprint)
-
-                for sprint in sprints:
-                    self.store.append((sprint, priority))
-                sprints.clear()
-                priority = 0
-        except Exception as e:
-            raise ValueError(
-                "The JSON structure of the sprint schedule file is wrong. Please check the documentation: https://github.com/SharryXu/jira-assistant"
-            ) from e
 
     def load_file(self, file: Union[str, Path]):
         """
         Load json file to generate the excel definition
 
         :param file:
             JSON file location
```

### Comparing `jira-assistant-0.1.8/src/jira_assistant/story.py` & `jira-assistant-0.1.9/src/jira_assistant/story.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from datetime import datetime
 from decimal import Decimal
 from functools import cmp_to_key
 from operator import attrgetter
-from typing import Any, Optional
+from typing import Any, Dict, List, Optional, Set, Tuple
 
 from dateutil import parser
 
 from .excel_definition import ExcelDefinition, ExcelDefinitionColumn
 from .milestone import Milestone
 from .priority import Priority, convert_to_priority
 from .sprint_schedule import SprintScheduleStore
@@ -150,43 +150,43 @@
         for column in self.factory.columns:
             if column["name"] is not None and hasattr(self, column["name"]):
                 result += f"{str(getattr(self, column['name']))}{separator}"
         return result
 
 
 class StoryFactory:
-    def __init__(self, columns: "list[ExcelDefinitionColumn]") -> None:
+    def __init__(self, columns: "List[ExcelDefinitionColumn]") -> None:
         if columns is None:
             raise ValueError("Columns must be provided!")
         self._columns = columns
         self._inline_weight_compare_rules = (
             self.__generate_inline_weights_compare_rules()
         )
 
-    def __generate_inline_weights_compare_rules(self) -> "list[tuple[str, int]]":
+    def __generate_inline_weights_compare_rules(self) -> "List[Tuple[str, int]]":
         rules = []
         for column in self._columns:
             if column["inline_weights"] > 0:
                 rules.append((column["name"], column["inline_weights"]))
         rules.sort(key=lambda r: r[1], reverse=True)
         return rules
 
     @property
     def columns(self):
         return self._columns
 
     @property
-    def inline_weights_compare_rules(self) -> "list[tuple[str, int]]":
+    def inline_weights_compare_rules(self) -> "List[Tuple[str, int]]":
         return self._inline_weight_compare_rules
 
     def create_story(self) -> Story:
         return Story(self)
 
 
-def sort_stories_by_inline_weights(stories: "list[Story]") -> "list[Story]":
+def sort_stories_by_inline_weights(stories: "List[Story]") -> "List[Story]":
     return sorted(
         stories, key=cmp_to_key(compare_story_based_on_inline_weights), reverse=True
     )
 
 
 def compare_story_based_on_inline_weights(
     story_a: Optional[Story], story_b: Optional[Story]
@@ -212,15 +212,15 @@
         story_a.factory != story_b.factory
         or story_a.factory is None
         or story_b.factory is None
     ):
         raise ValueError("The compare stories were built by different factory.")
 
     # story a and b have the same factory.
-    compare_rules: list[tuple[str, int]] = story_a.factory.inline_weights_compare_rules
+    compare_rules: List[Tuple[str, int]] = story_a.factory.inline_weights_compare_rules
 
     rules_count = len(compare_rules)
 
     if rules_count == 0:
         return 0
 
     skip_index_of_a = []
@@ -285,21 +285,21 @@
 
         count -= 1
         continue
     return 0
 
 
 def sort_stories_by_property_and_order(
-    stories: "list[Story]", excel_definition: ExcelDefinition, config: dict
+    stories: "List[Story]", excel_definition: ExcelDefinition, config: dict
 ):
-    sort_rules: list[tuple[str, bool]] = []
+    sort_rules: List[Tuple[str, bool]] = []
     excel_definition_columns = excel_definition.get_columns()
 
     if "ParentScopeIndexRange" in config:
-        column_definitions: dict[int, ExcelDefinitionColumn] = {
+        column_definitions: Dict[int, ExcelDefinitionColumn] = {
             c["index"]: c for c in excel_definition_columns
         }
 
         for column in excel_definition_columns:
             if column["scope_require_sort"] is True and column["name"] is not None:
                 sort_rules.append((column["name"], column["scope_sort_order"]))
 
@@ -314,26 +314,26 @@
             if column["require_sort"] is True and column["name"] is not None:
                 sort_rules.append((column["name"], column["sort_order"]))
 
         _internal_sort_stories_by_property_and_order(stories, sort_rules)
 
 
 def _internal_sort_stories_by_property_and_order(
-    stories: "list[Story]", sort_rules: "list[tuple[str, bool]]"
+    stories: "List[Story]", sort_rules: "List[Tuple[str, bool]]"
 ):
     for column_name, sort_order in reversed(sort_rules):
         stories.sort(key=attrgetter(column_name), reverse=sort_order)
 
 
 def _internal_sort_stories_by_property_and_order_considering_parent_range(
-    stories: "list[Story]",
-    story_columns: "dict[int, ExcelDefinitionColumn]",
-    sort_rules: "list[tuple[str, bool]]",
-    parent_level_index_range: "set[int]",
-) -> "list[Story]":
+    stories: "List[Story]",
+    story_columns: "Dict[int, ExcelDefinitionColumn]",
+    sort_rules: "List[Tuple[str, bool]]",
+    parent_level_index_range: "Set[int]",
+) -> "List[Story]":
     begin_index = 0
     end_index = 0
     while end_index <= len(stories) - 1:
         for i in range(begin_index, len(stories) - 1):
             all_parent_column_matched = True
             for column_index in parent_level_index_range:
                 if (
@@ -358,19 +358,19 @@
         begin_index = end_index + 1
         end_index = begin_index
 
     return stories
 
 
 def sort_stories_by_raise_ranking(
-    stories: "list[Story]", excel_definition: ExcelDefinition, config: dict
-) -> "list[Story]":
+    stories: "List[Story]", excel_definition: ExcelDefinition, config: Dict
+) -> "List[Story]":
     if stories is None:
         return []
-    sort_rules: list[tuple[str, int]] = []
+    sort_rules: List[Tuple[str, int]] = []
     excel_definition_columns = excel_definition.get_columns()
 
     result = []
 
     # New raise ranking mode.
     if "ParentScopeIndexRange" in config:
         for column in excel_definition_columns:
@@ -383,15 +383,15 @@
                 )
 
         if len(sort_rules) == 0:
             return stories
 
         sort_rules.sort(key=lambda x: x[1], reverse=True)  # sort by scope_raise_ranking
 
-        column_definitions: dict[int, ExcelDefinitionColumn] = {
+        column_definitions: Dict[int, ExcelDefinitionColumn] = {
             c["index"]: c for c in excel_definition_columns
         }
 
         result = _internal_raise_story_ranking_by_property_considering_parent_level(
             stories,
             column_definitions,
             sort_rules,
@@ -415,30 +415,30 @@
         for property_name, _ in sort_rules:
             result = _internal_raise_story_ranking_by_property(stories, property_name)
 
     return result
 
 
 def _internal_raise_story_ranking_by_property(
-    stories: "list[Story]", property_name: str
-) -> "list[Story]":
+    stories: "List[Story]", property_name: str
+) -> "List[Story]":
     if stories is None or len(stories) == 0:
         return stories
     # Use first story as example
     if not hasattr(stories[0], property_name):
         return stories
     return _raise_story_ranking_by_property(stories, property_name)
 
 
 def _internal_raise_story_ranking_by_property_considering_parent_level(
-    stories: "list[Story]",
-    story_columns: "dict[int, ExcelDefinitionColumn]",
-    sort_rules: "list[tuple[str, int]]",
-    parent_level_index_range: "set[int]",
-) -> "list[Story]":
+    stories: "List[Story]",
+    story_columns: "Dict[int, ExcelDefinitionColumn]",
+    sort_rules: "List[Tuple[str, int]]",
+    parent_level_index_range: "Set[int]",
+) -> "List[Story]":
     begin_index = 0
     end_index = 0
     while end_index <= len(stories) - 1:
         for i in range(begin_index, len(stories) - 1):
             all_parent_column_matched = True
             for column_index in parent_level_index_range:
                 if (
@@ -462,19 +462,19 @@
         end_index = begin_index
 
     return stories
 
 
 # Only bool indicator for now
 def _raise_story_ranking_by_property(
-    stories: "list[Story]", property_name: str
-) -> "list[Story]":
+    stories: "List[Story]", property_name: str
+) -> "List[Story]":
     if not isinstance(getattr(stories[0], property_name), bool):
         return stories
-    result: list[Story] = [stories[0]] * len(stories)
+    result: List[Story] = [stories[0]] * len(stories)
     j = 0
     for story in stories:
         if getattr(story, property_name) is True:
             result[j] = story
             j += 1
     for story in stories:
         if getattr(story, property_name) is False:
```

### Comparing `jira-assistant-0.1.8/src/jira_assistant.egg-info/PKG-INFO` & `jira-assistant-0.1.9/src/jira_assistant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-assistant
-Version: 0.1.8
+Version: 0.1.9
 Summary: Useful Jira tools
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,29 +28,31 @@
 Project-URL: Documentation, https://jira-assistant.readthedocs.io/en/stable
 Project-URL: Source, https://github.com/SharryXu/jira-assistant
 Project-URL: Tracker, https://github.com/SharryXu/jira-assistant/issues
 Keywords: jira,excel,sorting,project management,tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 Jira Assistant - userful jira tools
 =============================================
 
@@ -68,24 +70,24 @@
     :target: https://img.shields.io/github/repo-size/sharryxu/jira-assistant
     :alt: Package Size
 
 .. |GitHubIssues| image:: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :target: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :alt: GitHub issues
 
-.. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml/badge.svg
-    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml
+.. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-linux-test.yml/badge.svg
+    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-linux-test.yml
     :alt: python 3.11 (Linux)
 
-.. |Mac OS| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml/badge.svg
-    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-macos-test.yml
+.. |Mac OS| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-macos-test.yml/badge.svg
+    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-macos-test.yml
     :alt: python 3.11 (Mac OS)
 
-.. |Windows| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-windows-test.yml/badge.svg
-    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-windows-test.yml
+.. |Windows| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-windows-test.yml/badge.svg
+    :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-windows-test.yml
     :alt: python 3.11 (Windows)
 
 .. |Pylint| image:: https://github.com/sharryxu/jira-assistant/actions/workflows/pylint.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/pylint.yml
     :alt: Pylint 
 
 .. |CodeQL| image:: https://github.com/sharryxu/jira-assistant/workflows/CodeQL/badge.svg
```

### Comparing `jira-assistant-0.1.8/src/jira_assistant.egg-info/SOURCES.txt` & `jira-assistant-0.1.9/src/jira_assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/tests/test_console_script.py` & `jira-assistant-0.1.9/tests/test_console_script.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,29 @@
             check=True,
         )
 
         assert "xlsx has been saved" in result.stdout.decode("utf-8")
 
         remove(HERE / "files/happy_path_sorted.xlsx")
 
+    def test_process_excel_file_using_invalid_definition_file(self):
+        with pytest.raises(CalledProcessError):
+            result = run(
+                [
+                    "process-excel-file",
+                    HERE / "files/happy_path.xlsx",
+                    "--excel_definition_file",
+                    HERE / "files/excel_definition_invalid_structure.txt",
+                ],
+                capture_output=True,
+                check=True,
+            )
+
+            assert "xlsx has been saved" in result.stdout.decode("utf-8")
+
     def test_generate_template_excel_definition(self):
         result = run(
             ["generate-template", "excel-definition"], capture_output=True, check=True
         )
 
         assert "Generate success" in result.stdout.decode("utf-8")
         assert "excel-definition" in result.stdout.decode("utf-8")
```

### Comparing `jira-assistant-0.1.8/tests/test_excel_definition.py` & `jira-assistant-0.1.9/tests/test_excel_definition.py`

 * *Files 25% similar despite different names*

```diff
@@ -88,17 +88,26 @@
         validation_result = store.validate()
 
         assert len(validation_result) == 1
 
     def test_validate_invalid_name(self):
         excel_definition_filename = TEST_ASSETS / "excel_definition_invalid_name.json"
         store = ExcelDefinition()
-        with raises(TypeError):
+        with raises(SyntaxError) as err:
             store.load_file(excel_definition_filename)
 
+        assert (
+            "The excel definition file has below issues need to be fixed"
+            in err.value.args[0]
+        )
+        assert (
+            "The Name property type in the column definition should be string."
+            in err.value.args[0]
+        )
+
     def test_validate_invalid_raise_ranking(self):
         excel_definition_filename = (
             TEST_ASSETS / "excel_definition_invalid_raise_ranking.json"
         )
         store = ExcelDefinition()
         store.load_file(excel_definition_filename)
 
@@ -125,17 +134,26 @@
         validation_result = store.validate()
 
         assert len(validation_result) == 2
 
     def test_validate_invalid_index(self):
         excel_definition_filename = TEST_ASSETS / "excel_definition_invalid_index.json"
         store = ExcelDefinition()
-        with raises(TypeError):
+        with raises(SyntaxError) as err:
             store.load_file(excel_definition_filename)
 
+        assert (
+            "The excel definition file has below issues need to be fixed"
+            in err.value.args[0]
+        )
+        assert (
+            "The Index property type in the column definition is not integer."
+            in err.value.args[0]
+        )
+
     def test_validate_index_not_continuation(self):
         excel_definition_filename = (
             TEST_ASSETS / "excel_definition_index_not_continuation.json"
         )
         store = ExcelDefinition()
         store.load_file(excel_definition_filename)
 
@@ -160,7 +178,36 @@
         )
         store = ExcelDefinition()
         store.load_file(excel_definition_filename)
 
         validation_result = store.validate()
 
         assert len(validation_result) == 1
+
+    def test_validate_invalid_structure(self):
+        excel_definition_filename = (
+            TEST_ASSETS / "excel_definition_invalid_structure.txt"
+        )
+        store = ExcelDefinition()
+
+        with raises(Exception) as err:
+            store.load_file(excel_definition_filename)
+
+        assert (
+            "The structure of excel definition file is wrong. Hint: Expecting ',' delimiter in line 49:1"
+            in err.value.args[0]
+        )
+
+    def test_validate_invalid_pre_process_step_name(self):
+        excel_definition_filename = (
+            TEST_ASSETS / "excel_definition_invalid_pre_process_step_name.json"
+        )
+        store = ExcelDefinition()
+
+        with raises(SyntaxError) as err:
+            store.load_file(excel_definition_filename)
+
+        assert (
+            "The excel definition file has below issues need to be fixed"
+            in err.value.args[0]
+        )
+        assert "The pre-process step must have a name." in err.value.args[0]
```

### Comparing `jira-assistant-0.1.8/tests/test_excel_operation.py` & `jira-assistant-0.1.9/tests/test_excel_operation.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/tests/test_jira_client.py` & `jira-assistant-0.1.9/tests/test_jira_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 
 from mock_server import (
     mock_jira_requests,
     mock_jira_requests_with_failed_status_code,
     mock_jira_stories,
 )
```

### Comparing `jira-assistant-0.1.8/tests/test_milestone.py` & `jira-assistant-0.1.9/tests/test_milestone.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/tests/test_priority.py` & `jira-assistant-0.1.9/tests/test_priority.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/tests/test_sprint_schedule.py` & `jira-assistant-0.1.9/tests/test_sprint_schedule.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.8/tests/test_story.py` & `jira-assistant-0.1.9/tests/test_story.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from decimal import Decimal
+from typing import List
 
 from pytest import raises
 
 from jira_assistant.excel_definition import ExcelDefinitionColumn
 from jira_assistant.priority import Priority
 from jira_assistant.story import (
     Story,
@@ -10,15 +11,15 @@
     compare_story_based_on_inline_weights,
     convert_to_bool,
     convert_to_datetime,
     convert_to_decimal,
 )
 
 
-def mock_data() -> list[Story]:
+def mock_data() -> List[Story]:
     story_factory = StoryFactory(
         [
             ExcelDefinitionColumn(
                 index=1,
                 name="name",
                 type=str,
                 require_sort=False,
```

