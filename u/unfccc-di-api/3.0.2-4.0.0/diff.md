# Comparing `tmp/unfccc_di_api-3.0.2.tar.gz` & `tmp/unfccc_di_api-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfccc_di_api-3.0.2.tar", last modified: Tue Dec 13 09:49:24 2022, max compression
+gzip compressed data, was "unfccc_di_api-4.0.0.tar", last modified: Tue Jul 18 13:31:29 2023, max compression
```

## Comparing `unfccc_di_api-3.0.2.tar` & `unfccc_di_api-4.0.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 09:49:24.852429 unfccc_di_api-3.0.2/
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 09:49:24.848430 unfccc_di_api-3.0.2/.github/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      324 2021-01-22 09:02:49.000000 unfccc_di_api-3.0.2/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 09:49:24.848430 unfccc_di_api-3.0.2/.github/workflows/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      757 2022-12-13 09:44:51.000000 unfccc_di_api-3.0.2/.github/workflows/ci.yml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1204 2021-01-22 09:32:02.000000 unfccc_di_api-3.0.2/.gitignore
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1287 2022-12-13 09:04:12.000000 unfccc_di_api-3.0.2/.pre-commit-config.yaml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      122 2021-01-06 18:41:35.000000 unfccc_di_api-3.0.2/.readthedocs.yml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      267 2021-12-03 11:12:26.000000 unfccc_di_api-3.0.2/AUTHORS.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1965 2022-12-13 09:41:19.000000 unfccc_di_api-3.0.2/CHANGELOG.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     3573 2022-12-13 09:31:40.000000 unfccc_di_api-3.0.2/CONTRIBUTING.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      618 2021-02-09 13:51:45.000000 unfccc_di_api-3.0.2/LICENSE
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2601 2021-12-03 10:27:21.000000 unfccc_di_api-3.0.2/Makefile
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     4587 2022-12-13 09:49:24.852429 unfccc_di_api-3.0.2/PKG-INFO
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1573 2022-12-13 09:49:03.000000 unfccc_di_api-3.0.2/README.rst
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 09:49:24.852429 unfccc_di_api-3.0.2/docs/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      626 2021-01-22 09:15:19.000000 unfccc_di_api-3.0.2/docs/Makefile
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      175 2021-01-22 12:06:40.000000 unfccc_di_api-3.0.2/docs/api.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       30 2021-01-22 09:15:19.000000 unfccc_di_api-3.0.2/docs/changelog.rst
--rwxrwxr-x   0 pflueger  (1000) pflueger  (1000)     5093 2021-02-09 13:51:04.000000 unfccc_di_api-3.0.2/docs/conf.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       33 2021-01-22 09:02:49.000000 unfccc_di_api-3.0.2/docs/contributing.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      326 2021-01-22 09:34:24.000000 unfccc_di_api-3.0.2/docs/credits.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      311 2021-01-22 09:35:15.000000 unfccc_di_api-3.0.2/docs/index.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1170 2021-01-22 09:22:52.000000 unfccc_di_api-3.0.2/docs/installation.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      775 2021-01-22 09:02:49.000000 unfccc_di_api-3.0.2/docs/make.bat
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       27 2021-01-22 09:02:49.000000 unfccc_di_api-3.0.2/docs/readme.rst
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       24 2021-01-22 13:56:15.000000 unfccc_di_api-3.0.2/docs/requirements.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     2648 2021-12-03 10:25:47.000000 unfccc_di_api-3.0.2/docs/usage.ipynb
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      191 2021-04-23 14:54:13.000000 unfccc_di_api-3.0.2/pyproject.toml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        2 2022-01-18 17:02:10.000000 unfccc_di_api-3.0.2/requirements.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        7 2021-04-23 13:59:01.000000 unfccc_di_api-3.0.2/requirements_dev.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1434 2022-12-13 09:49:24.852429 unfccc_di_api-3.0.2/setup.cfg
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       61 2021-04-23 15:10:15.000000 unfccc_di_api-3.0.2/setup.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1091 2022-12-13 09:43:00.000000 unfccc_di_api-3.0.2/tbump.toml
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      345 2022-12-13 09:30:53.000000 unfccc_di_api-3.0.2/tox.ini
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 09:49:24.852429 unfccc_di_api-3.0.2/unfccc_di_api/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      949 2022-12-13 09:43:00.000000 unfccc_di_api-3.0.2/unfccc_di_api/__init__.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 09:49:24.852429 unfccc_di_api-3.0.2/unfccc_di_api/tests/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      282 2021-01-22 12:11:02.000000 unfccc_di_api-3.0.2/unfccc_di_api/tests/__init__.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1979 2021-12-03 10:26:47.000000 unfccc_di_api-3.0.2/unfccc_di_api/tests/test_unfccc_di_api.py
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)    22579 2022-03-15 09:04:47.000000 unfccc_di_api-3.0.2/unfccc_di_api/unfccc_di_api.py
-drwxrwxr-x   0 pflueger  (1000) pflueger  (1000)        0 2022-12-13 09:49:24.852429 unfccc_di_api-3.0.2/unfccc_di_api.egg-info/
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     4587 2022-12-13 09:49:24.000000 unfccc_di_api-3.0.2/unfccc_di_api.egg-info/PKG-INFO
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      807 2022-12-13 09:49:24.000000 unfccc_di_api-3.0.2/unfccc_di_api.egg-info/SOURCES.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)        1 2022-12-13 09:49:24.000000 unfccc_di_api-3.0.2/unfccc_di_api.egg-info/dependency_links.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)      178 2022-12-13 09:49:24.000000 unfccc_di_api-3.0.2/unfccc_di_api.egg-info/requires.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)       14 2022-12-13 09:49:24.000000 unfccc_di_api-3.0.2/unfccc_di_api.egg-info/top_level.txt
--rw-rw-r--   0 pflueger  (1000) pflueger  (1000)     1167 2021-12-03 11:13:25.000000 unfccc_di_api-3.0.2/update_citation_info.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-07-18 13:31:29.679901 unfccc_di_api-4.0.0/
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-07-18 13:31:29.679901 unfccc_di_api-4.0.0/.github/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      324 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-07-18 13:31:29.679901 unfccc_di_api-4.0.0/.github/workflows/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      757 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1204 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/.gitignore
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1285 2023-07-18 08:44:51.000000 unfccc_di_api-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      202 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/.readthedocs.yml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      279 2023-07-18 13:14:19.000000 unfccc_di_api-4.0.0/AUTHORS.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2327 2023-07-18 13:14:53.000000 unfccc_di_api-4.0.0/CHANGELOG.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     3573 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      658 2023-07-18 13:14:19.000000 unfccc_di_api-4.0.0/LICENSE
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2800 2023-07-18 13:26:28.000000 unfccc_di_api-4.0.0/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5705 2023-07-18 13:31:29.679901 unfccc_di_api-4.0.0/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2329 2023-07-18 13:19:27.000000 unfccc_di_api-4.0.0/README.rst
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-07-18 13:31:29.679901 unfccc_di_api-4.0.0/docs/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      626 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/Makefile
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      175 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/api.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       30 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/changelog.rst
+-rwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)     5093 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/conf.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       33 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/contributing.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      326 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/credits.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      311 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/index.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1170 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/installation.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      775 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/make.bat
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       27 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/readme.rst
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       36 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/docs/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2396 2023-07-18 13:14:19.000000 unfccc_di_api-4.0.0/docs/usage.ipynb
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      191 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/pyproject.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        2 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/requirements.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        7 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/requirements_dev.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1456 2023-07-18 13:31:29.679901 unfccc_di_api-4.0.0/setup.cfg
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       61 2023-06-01 08:57:06.000000 unfccc_di_api-4.0.0/setup.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1105 2023-07-18 13:17:05.000000 unfccc_di_api-4.0.0/tbump.toml
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      345 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/tox.ini
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-07-18 13:31:29.679901 unfccc_di_api-4.0.0/unfccc_di_api/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1019 2023-07-18 13:17:05.000000 unfccc_di_api-4.0.0/unfccc_di_api/__init__.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-07-18 13:31:29.679901 unfccc_di_api-4.0.0/unfccc_di_api/tests/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      282 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/unfccc_di_api/tests/__init__.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     2581 2023-07-18 13:14:19.000000 unfccc_di_api-4.0.0/unfccc_di_api/tests/test_unfccc_di_api.py
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)    25850 2023-07-18 13:14:19.000000 unfccc_di_api-4.0.0/unfccc_di_api/unfccc_di_api.py
+drwxr-xr-x   0 mikapfl   (1000) mikapfl   (1000)        0 2023-07-18 13:31:29.679901 unfccc_di_api-4.0.0/unfccc_di_api.egg-info/
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     5705 2023-07-18 13:31:29.000000 unfccc_di_api-4.0.0/unfccc_di_api.egg-info/PKG-INFO
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      807 2023-07-18 13:31:29.000000 unfccc_di_api-4.0.0/unfccc_di_api.egg-info/SOURCES.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)        1 2023-07-18 13:31:29.000000 unfccc_di_api-4.0.0/unfccc_di_api.egg-info/dependency_links.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)      195 2023-07-18 13:31:29.000000 unfccc_di_api-4.0.0/unfccc_di_api.egg-info/requires.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)       14 2023-07-18 13:31:29.000000 unfccc_di_api-4.0.0/unfccc_di_api.egg-info/top_level.txt
+-rw-r--r--   0 mikapfl   (1000) mikapfl   (1000)     1167 2023-06-01 08:56:36.000000 unfccc_di_api-4.0.0/update_citation_info.py
```

### Comparing `unfccc_di_api-3.0.2/.github/workflows/ci.yml` & `unfccc_di_api-4.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `unfccc_di_api-3.0.2/.gitignore` & `unfccc_di_api-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `unfccc_di_api-3.0.2/.pre-commit-config.yaml` & `unfccc_di_api-4.0.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -11,38 +11,38 @@
       - id: check-ast
       - id: fix-byte-order-marker
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: detect-private-key
       - id: mixed-line-ending
   - repo: https://github.com/psf/black
-    rev: '22.10.0'
+    rev: '23.7.0'
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/flake8
     rev: '6.0.0'
     hooks:
       - id: flake8
   - repo: https://github.com/PyCQA/doc8
-    rev: 'v1.0.0'
+    rev: 'v1.1.1'
     hooks:
       - id: doc8
   - repo: https://github.com/PyCQA/isort
-    rev: '5.10.1'
+    rev: '5.12.0'
     hooks:
       - id: isort
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: '1.5.3'
+    rev: '1.7.0'
     hooks:
       - id: nbqa-black
         args: [ --nbqa-mutate, --line-length=75 ]
       - id: nbqa-check-ast
   - repo: https://github.com/asottile/blacken-docs
-    rev: 'v1.12.1'
+    rev: '1.15.0'
     hooks:
       - id: blacken-docs
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v0.991'
+    rev: 'v1.4.1'
     hooks:
       - id: mypy
         additional_dependencies:
           - types-requests
```

### Comparing `unfccc_di_api-3.0.2/CHANGELOG.rst` & `unfccc_di_api-4.0.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
 Changelog
 =========
 
+4.0.0 (2023-07-18)
+------------------
+
+* Breaking: the UNFCCC restricted API access, likely you have to change your code to
+  use the new ZenodoReader instead.
+* Add ZenodoReader which doesn't rely on API access.
+* Use data released until 2023-07-18 when using the ZenodoReader.
+* Build the documentation on ReadTheDocs using newer Python and Sphinx versions.
+
+
 3.0.2 (2022-12-13)
 ------------------
 
 * Support python 3.11.
 * Drop support for python 3.6.
 
 3.0.1 (2022-03-15)
```

### Comparing `unfccc_di_api-3.0.2/CONTRIBUTING.rst` & `unfccc_di_api-4.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `unfccc_di_api-3.0.2/LICENSE` & `unfccc_di_api-4.0.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Apache Software License 2.0
 
 Copyright 2020-2021 Potsdam-Institut für Klimafolgenforschung e.V.
+Copyright 2023 Climate Resource Pty Ltd
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `unfccc_di_api-3.0.2/Makefile` & `unfccc_di_api-4.0.0/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -54,33 +54,35 @@
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs html
 
 servedocs: docs ## compile the docs watching for changes
 	watchmedo shell-command -p '*.rst' -c '$(MAKE) -C docs html' -R -D .
 
 release: dist ## package and upload a release
-	venv/bin/twine upload dist/*
+	venv/bin/twine upload --repository unfccc dist/*
 
 dist: clean venv ## builds source and wheel package
 	venv/bin/python -m build
 	ls -l dist
 
 install: clean ## install the package to the active Python's site-packages
 	python setup.py install
 
 virtual-environment: venv ## setup a virtual environment for development
 
 venv: setup.py pyproject.toml setup.cfg
 	[ -d venv ] || python3 -m venv venv
+	venv/bin/python -m pip install --upgrade --upgrade-strategy eager pip wheel
 	venv/bin/python -m pip install -e .[dev]
 	touch venv
 
 update-venv:  ## update the development virtual environment
 	[ -d venv ] || python3 -m venv venv
-	venv/bin/python -m pip install --upgrade -e .[dev]
+	venv/bin/python -m pip install --upgrade --upgrade-strategy eager pip wheel
+	venv/bin/python -m pip install --upgrade --upgrade-strategy eager -e .[dev]
 	touch venv
 
 install-pre-commit: venv ## install the pre-commit hooks
 	venv/bin/pre-commit install
 
 update-citation: ## Update the citation information from zenodo
 	venv/bin/python update_citation_info.py
```

### Comparing `unfccc_di_api-3.0.2/PKG-INFO` & `unfccc_di_api-4.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfccc_di_api
-Version: 3.0.2
+Version: 4.0.0
 Summary: Python wrapper around the Flexible Query API of the UNFCCC.
 Home-page: https://github.com/pik-primap/unfccc_di_api
 Author: Mika Pflüger
 Author-email: mika.pflueger@pik-potsdam.de
 License: Apache Software License 2.0
 Project-URL: Documentation, https://unfccc-di-api.readthedocs.io
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,29 +44,45 @@
 Python wrapper around the `Flexible Query API <https://di.unfccc.int/flex_annex1>`_ of
 the UNFCCC.
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://unfccc-di-api.readthedocs.io.
 
+Warning
+-------
+
+Due to a recent change in the UNFCCC's API, the UNFCCCApiReader class is
+**not functional** any more in standard environments. To continue to access the data,
+you have two options:
+
+1. Use the new ZenodoReader. It provides access using the `query` function like the
+   UNFCCCApiReader, but only supports querying for a full dataset with all data. It
+   relies on our `data package <https://doi.org/10.5281/zenodo.4198782>`_, which we
+   update regularly; however, the data is naturally not as recent as querying from
+   the API directly.
+2. Run your functions in an environment which is not blocked by the UNFCCC DI API.
+   According to our tests, Azure virtual machines work, as well as github hosted
+   runners, with the exception of Mac OS runners.
+
 
 Features
 --------
 
 * High-level API to query all information for a given party.
 * Low-level API to selectively query information with the same resolution as in the
   UNFCCC web query tool.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Daniel Huppmann & Johannes Gütschow. (2022-12-13).
-pik-primap/unfccc_di_api: unfccc_di_api version 3.0.2.
-Zenodo. https://doi.org/10.5281/zenodo.7431899
+Mika Pflüger, Daniel Huppmann & Johannes Gütschow. (2023-07-18).
+pik-primap/unfccc_di_api: Version 4.0.0.
+Zenodo. https://doi.org/10.5281/zenodo.8160056
 
 Data package
 ------------
 If you just want all the data in CSV and parquet format (suitable for reading with
 pandas), look at our `data package <https://doi.org/10.5281/zenodo.4198782>`_.
 
 CI status and other links
@@ -76,14 +92,24 @@
    :target: https://results.pre-commit.ci/latest/github/pik-primap/unfccc_di_api/main
    :alt: pre-commit.ci status
 
 =========
 Changelog
 =========
 
+4.0.0 (2023-07-18)
+------------------
+
+* Breaking: the UNFCCC restricted API access, likely you have to change your code to
+  use the new ZenodoReader instead.
+* Add ZenodoReader which doesn't rely on API access.
+* Use data released until 2023-07-18 when using the ZenodoReader.
+* Build the documentation on ReadTheDocs using newer Python and Sphinx versions.
+
+
 3.0.2 (2022-12-13)
 ------------------
 
 * Support python 3.11.
 * Drop support for python 3.6.
 
 3.0.1 (2022-03-15)
```

### Comparing `unfccc_di_api-3.0.2/README.rst` & `unfccc_di_api-4.0.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -18,29 +18,45 @@
 Python wrapper around the `Flexible Query API <https://di.unfccc.int/flex_annex1>`_ of
 the UNFCCC.
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://unfccc-di-api.readthedocs.io.
 
+Warning
+-------
+
+Due to a recent change in the UNFCCC's API, the UNFCCCApiReader class is
+**not functional** any more in standard environments. To continue to access the data,
+you have two options:
+
+1. Use the new ZenodoReader. It provides access using the `query` function like the
+   UNFCCCApiReader, but only supports querying for a full dataset with all data. It
+   relies on our `data package <https://doi.org/10.5281/zenodo.4198782>`_, which we
+   update regularly; however, the data is naturally not as recent as querying from
+   the API directly.
+2. Run your functions in an environment which is not blocked by the UNFCCC DI API.
+   According to our tests, Azure virtual machines work, as well as github hosted
+   runners, with the exception of Mac OS runners.
+
 
 Features
 --------
 
 * High-level API to query all information for a given party.
 * Low-level API to selectively query information with the same resolution as in the
   UNFCCC web query tool.
 
 Citation
 --------
 If you use this library and want to cite it, please cite it as:
 
-Mika Pflüger, Daniel Huppmann & Johannes Gütschow. (2022-12-13).
-pik-primap/unfccc_di_api: unfccc_di_api version 3.0.2.
-Zenodo. https://doi.org/10.5281/zenodo.7431899
+Mika Pflüger, Daniel Huppmann & Johannes Gütschow. (2023-07-18).
+pik-primap/unfccc_di_api: Version 4.0.0.
+Zenodo. https://doi.org/10.5281/zenodo.8160056
 
 Data package
 ------------
 If you just want all the data in CSV and parquet format (suitable for reading with
 pandas), look at our `data package <https://doi.org/10.5281/zenodo.4198782>`_.
 
 CI status and other links
```

### Comparing `unfccc_di_api-3.0.2/docs/Makefile` & `unfccc_di_api-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `unfccc_di_api-3.0.2/docs/conf.py` & `unfccc_di_api-4.0.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 release = unfccc_di_api.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `unfccc_di_api-3.0.2/docs/installation.rst` & `unfccc_di_api-4.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `unfccc_di_api-3.0.2/docs/make.bat` & `unfccc_di_api-4.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `unfccc_di_api-3.0.2/docs/usage.ipynb` & `unfccc_di_api-4.0.0/docs/usage.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8357955798059964%*

 * *Differences: {"'cells'": "{0: {'metadata': {delete: ['collapsed']}, 'source': {insert: [(2, 'To download the "*

 * *            "data from Zenodo, import the package and instantiate the reader,\\n'), (3, 'which "*

 * *            "will download the most recent dataset:')], delete: [3, 2]}}, 1: {'source': {insert: "*

 * *            "[(2, 'reader = unfccc_di_api.ZenodoReader()')], delete: [2]}, 'metadata': {'jupyter': "*

 * *            "OrderedDict([('outputs_hidden', False)]), 'tags': [], delete: ['collapsed']}}, 2: "*

 * *            "{'metad […]*

```diff
@@ -1,147 +1,134 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": true,
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "# Usage\n",
                 "\n",
-                "To use the UNFCCC API, import the package and instantiate the reader,\n",
-                "which will download the most recent metadata from the UNFCCC:"
+                "To download the data from Zenodo, import the package and instantiate the reader,\n",
+                "which will download the most recent dataset:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                },
                 "pycharm": {
                     "name": "#%%\n"
-                }
+                },
+                "tags": []
             },
             "outputs": [],
             "source": [
                 "import unfccc_di_api\n",
                 "\n",
-                "reader = unfccc_di_api.UNFCCCApiReader()"
+                "reader = unfccc_di_api.ZenodoReader()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "Check for which parties data is available:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                },
                 "pycharm": {
                     "name": "#%%\n"
-                }
+                },
+                "tags": []
             },
             "outputs": [],
             "source": [
                 "reader.parties"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
                 "Access all data for a specific party:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "collapsed": false,
+                "jupyter": {
+                    "outputs_hidden": false
+                },
                 "pycharm": {
                     "name": "#%%\n"
-                }
+                },
+                "tags": []
             },
             "outputs": [],
             "source": [
                 "reader.query(party_code=\"AFG\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
                 "pycharm": {
                     "name": "#%% md\n"
                 }
             },
             "source": [
-                "Queries can be more specific, e.g. selecting only data about one gas:"
+                "You can also request data directly form the UNFCCC DI API if you have a way to\n",
+                "get access. Check the API docs section (next section), or the docstrings of\n",
+                "`UNFCCCApiReader` for details."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
-            },
+            "metadata": {},
             "outputs": [],
-            "source": [
-                "reader.query(party_code=\"DEU\", gases=[\"N\u2082O\"])"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
-            },
-            "source": [
-                "Queries can be made much more specific, if you want to. Check the API\n",
-                "docs section (next section), or the docstrings for details."
-            ]
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
-                "version": 2
+                "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython2",
-            "version": "2.7.6"
+            "pygments_lexer": "ipython3",
+            "version": "3.10.6"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 0
+    "nbformat_minor": 4
 }
```

### Comparing `unfccc_di_api-3.0.2/setup.cfg` & `unfccc_di_api-4.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unfccc_di_api
-version = 3.0.2
+version = 4.0.0
 author = Mika Pflüger
 author_email = mika.pflueger@pik-potsdam.de
 description = Python wrapper around the Flexible Query API of the UNFCCC.
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pik-primap/unfccc_di_api
 project_urls = 
@@ -18,38 +18,40 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 license = Apache Software License 2.0
-license_file = LICENSE
+license_files = LICENSE
 
 [options]
 packages = 
 	unfccc_di_api
 	unfccc_di_api.tests
 python_requires = >=3.7
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	pandas
 	treelib
 	requests
+	pooch
+	pyarrow
 
 [options.extras_require]
 test = pytest
 dev = 
 	pip
 	wheel
 	build
 	watchdog
 	flake8
 	coverage
-	Sphinx
+	Sphinx >= 6
 	twine
 	pytest
 	pytest-runner
 	pre-commit
 	sphinx_rtd_theme
 	ipykernel
 	nbsphinx
```

### Comparing `unfccc_di_api-3.0.2/tbump.toml` & `unfccc_di_api-4.0.0/tbump.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/pik-primap/unfccc_di_api/"
 
 [version]
-current = "3.0.2"
+current = "4.0.0"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
@@ -28,15 +28,15 @@
 
 [[file]]
 src = "unfccc_di_api/__init__.py"
 search = '__version__ = "{current_version}"'
 
 [[file]]
 src = "README.rst"
-search = 'pik-primap/unfccc_di_api: Version {current_version}.'
+search = 'pik-primap/unfccc_di_api: unfccc_di_api version {current_version}.'
 
 # You can specify a list of commands to
 # run after the files have been patched
 # and before the git commit is made
 
 [[before_commit]]
 name = "lint"
```

### Comparing `unfccc_di_api-3.0.2/unfccc_di_api/__init__.py` & `unfccc_di_api-4.0.0/unfccc_di_api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,12 +6,22 @@
 if you want to filter for specific variables and only query a subset of the data,
 you have to use the individual API objects for Annex I and non-Annex I parties,
 which are available at :py:attr:`UNFCCCApiReader.annex_one_reader` and
 :py:attr:`UNFCCCApiReader.non_annex_one_reader`, respectively."""
 
 __author__ = """Mika Pflüger"""
 __email__ = "mika.pflueger@pik-potsdam.de"
-__version__ = "3.0.2"
+__version__ = "4.0.0"
 
-from .unfccc_di_api import NoDataError, UNFCCCApiReader, UNFCCCSingleCategoryApiReader
+from .unfccc_di_api import (
+    NoDataError,
+    UNFCCCApiReader,
+    UNFCCCSingleCategoryApiReader,
+    ZenodoReader,
+)
 
-__all__ = ["UNFCCCApiReader", "UNFCCCSingleCategoryApiReader", "NoDataError"]
+__all__ = [
+    "UNFCCCApiReader",
+    "UNFCCCSingleCategoryApiReader",
+    "ZenodoReader",
+    "NoDataError",
+]
```

### Comparing `unfccc_di_api-3.0.2/unfccc_di_api/tests/test_unfccc_di_api.py` & `unfccc_di_api-4.0.0/unfccc_di_api/tests/test_unfccc_di_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,67 @@
 """Tests for the `unfccc_di_api` package."""
 
 import pytest
 
 import unfccc_di_api
-from unfccc_di_api import UNFCCCApiReader
+from unfccc_di_api import UNFCCCApiReader, ZenodoReader
 
 
 @pytest.fixture(scope="module")
 def api_reader() -> UNFCCCApiReader:
     return UNFCCCApiReader()
 
 
-def test_non_annex_one(api_reader: UNFCCCApiReader):
+@pytest.fixture(scope="module")
+def zenodo_reader() -> ZenodoReader:
+    return ZenodoReader()
+
+
+@pytest.fixture(scope="module", params=["unfccc", "zenodo"])
+def reader(request):
+    if request.param == "unfccc":
+        return UNFCCCApiReader()
+    if request.param == "zenodo":
+        return ZenodoReader()
+
+
+def test_not_implemented(zenodo_reader):
+    with pytest.raises(NotImplementedError):
+        zenodo_reader.query(party_code="DEU", gases=["N2O"])
+    with pytest.raises(NotImplementedError):
+        zenodo_reader.query(party_code="DEU", normalize_gas_names=False)
+
+
+def test_non_annex_one(api_reader):
     ans = api_reader.non_annex_one_reader.query(party_codes=["MMR"])
 
     match = "Unknown party *"
     with pytest.raises(ValueError, match=match):
         api_reader.non_annex_one_reader.query(party_codes=["ASDF"])
 
     assert len(ans) > 1
 
 
 def test_annex_one(api_reader: UNFCCCApiReader):
     ans = api_reader.annex_one_reader.query(party_codes=["DEU"], gases=["N₂O"])
     assert len(ans) > 1
 
 
-def test_unified(api_reader: UNFCCCApiReader):
-    ans = api_reader.query(party_code="AFG")
-    assert len(ans) > 1
-    ans = api_reader.query(party_code="DEU", gases=["N₂O"])
+def test_unified(reader):
+    ans = reader.query(party_code="AFG")
     assert len(ans) > 1
 
     match = "Unknown party *"
     with pytest.raises(ValueError, match=match):
-        api_reader.query(party_code="ASDF")
+        reader.query(party_code="ASDF")
+
+
+def test_unified_gases(api_reader: UNFCCCApiReader):
+    ans = api_reader.query(party_code="DEU", gases=["N₂O"])
+    assert len(ans) > 1
 
 
 @pytest.mark.parametrize("normalize", [True, False])
 def test_unified_as_ascii(api_reader: UNFCCCApiReader, normalize: bool):
     # assert that using standardized string ('N2O' instead of "N₂O") works
     ans = api_reader.query(
         party_code="DEU", gases=["N2O"], normalize_gas_names=normalize
```

### Comparing `unfccc_di_api-3.0.2/unfccc_di_api/unfccc_di_api.py` & `unfccc_di_api-4.0.0/unfccc_di_api/unfccc_di_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import itertools
 import logging
 import typing
+import zipfile
 
 import pandas as pd
+import pooch
 import requests
 import treelib
 
 # mapping from gas as simple string to subscript-format used by UNFCCC DI API
 GAS_MAPPING = {
     "CH4": "CH₄",
     "CO2": "CO₂",
@@ -68,14 +70,90 @@
             (gases, "gases"),
         ):
             if optional_param is not None:
                 query += f" {key}={optional_param!r}"
         KeyError.__init__(self, f"Query returned no data for: {query}")
 
 
+class ZenodoReader:
+    """Provides simplified unified access to the data provided by the Flexible Query
+    API of the UNFCCC data access, via the dataset stored at zenodo.
+
+    Essentially gives you the same API as the UNFCCCApiReader, but without complications
+    due to the protection measures of the DI API. The advantage of using the
+    ZenodoReader is that it works reliably without special measures, the disadvantage
+    is that the data might be a bit older.
+
+    Attributes
+    ----------
+    parties : list[str]
+        All parties as a 3-letter iso code.
+    """
+
+    def __init__(
+        self,
+        *,
+        url: str = "doi:10.5281/zenodo.8159736/parquet-only.zip",
+        known_hash: str = "md5:95d98404f642ed2b684594abba8934ba",
+    ):
+        self._zipfile_path = pooch.retrieve(url=url, known_hash=known_hash)
+        self._zipfile = zipfile.ZipFile(self._zipfile_path)
+        self.parties = [
+            x.split("/")[-1][:3]
+            for x in self._zipfile.namelist()
+            if x.endswith(".parquet")
+        ]
+
+    def _get_party_data(self, *, party: str) -> pd.DataFrame:
+        fnames = [x for x in self._zipfile.namelist() if x.endswith(f"{party}.parquet")]
+        try:
+            fname = fnames[0]
+        except IndexError:
+            raise ValueError(f"Unknown party: {party}.")
+        with self._zipfile.open(fname) as fd:
+            return pd.read_parquet(fd)
+
+    def query(
+        self,
+        *,
+        party_code: str,
+        gases: typing.Optional[typing.Sequence[str]] = None,
+        normalize_gas_names: bool = True,
+    ) -> pd.DataFrame:
+        """Query the dataset for party data.
+
+        Parameters
+        ----------
+        party_code : str
+            ISO code of a party for which to query. For possible values, see
+            :py:attr:`~ZenodoReader.parties`.
+        gases : list of str, optional
+            Limit the query to these gases. Accepts subscripts ("N₂O")
+            as well as ASCII-strings ("N2O"). Default: query for all gases.
+            Note that anything else than the default is not yet implemented and raises
+            an error. Just request the whole dataset and filter using pandas' normal
+            functionality.
+        normalize_gas_names : bool, optional
+            If :obj:`True`, return gases as ASCII strings ("N2O").
+            Else, return native UNFCCC notation ("N₂O"). Default: true.
+            Note that anything else than the default is not implemented and raises an
+            error. If you require unnormalized gas names, open an issue in the issue
+            tracker at github so we can understand your use case.
+
+        Returns
+        -------
+        pandas.DataFrame
+        """
+        if not normalize_gas_names:
+            raise NotImplementedError("Non-normalized gases not yet implemented")
+        if gases is not None:
+            raise NotImplementedError("Specific gas lists not yet implemented")
+        return self._get_party_data(party=party_code)
+
+
 class UNFCCCApiReader:
     """Provides simplified unified access to the Flexible Query API of the UNFCCC data
     access for all parties.
 
     Essentially encapsulates https://di.unfccc.int/flex_non_annex1 and
     https://di.unfccc.int/flex_annex1 .
 
@@ -214,15 +292,21 @@
         party_category : str
            Either ``nonAnnexOne`` or ``annexOne``.
         base_url : str
            Location of the UNFCCC api.
         """
         self.base_url = base_url
 
-        parties_raw = self._get(f"parties/{party_category}")
+        try:
+            parties_raw = self._get(f"parties/{party_category}")
+        except requests.JSONDecodeError:
+            raise RuntimeError(
+                "Access to the UNFCCC API denied - see"
+                " https://github.com/pik-primap/unfccc_di_api#warning for solutions"
+            )
         parties_entries = []
         for entry in parties_raw:
             if entry["categoryCode"] == party_category and entry["name"] != "Groups":
                 parties_entries.append(entry["parties"])
         if not parties_entries:
             raise ValueError(
                 f"Could not find parties for the party_category {party_category!r}."
@@ -294,15 +378,14 @@
     def _flexible_query(
         self,
         *,
         variable_ids: typing.Sequence[int],
         party_ids: typing.Sequence[int],
         year_ids: typing.Sequence[int],
     ) -> typing.List[dict]:
-
         if len(variable_ids) > 3000:
             logging.warning(
                 "Your query parameters lead to a lot of variables selected at once. "
                 "If the query fails, try restricting your query more."
             )
 
         return self._post(
```

### Comparing `unfccc_di_api-3.0.2/unfccc_di_api.egg-info/SOURCES.txt` & `unfccc_di_api-4.0.0/unfccc_di_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unfccc_di_api-3.0.2/update_citation_info.py` & `unfccc_di_api-4.0.0/update_citation_info.py`

 * *Files identical despite different names*

