# Comparing `tmp/tokenlists-0.1.3.tar.gz` & `tmp/tokenlists-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenlists-0.1.3.tar", last modified: Tue Jun 13 01:51:18 2023, max compression
+gzip compressed data, was "tokenlists-0.1.4.tar", last modified: Tue Jul 18 20:03:17 2023, max compression
```

## Comparing `tokenlists-0.1.3.tar` & `tokenlists-0.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-13 01:50:57.000000 tokenlists-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-13 01:51:18.393734 tokenlists-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-13 01:50:57.000000 tokenlists-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-13 01:50:57.000000 tokenlists-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 01:51:18.393734 tokenlists-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-13 01:50:57.000000 tokenlists-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.389734 tokenlists-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tests/functional/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tests/functional/test_uniswap_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tests/integration/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/tokenlists/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/tokenlists.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:17.296564 tokenlists-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:17.296564 tokenlists-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:17.296564 tokenlists-0.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:17.296564 tokenlists-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-18 20:02:59.000000 tokenlists-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-07-18 20:02:59.000000 tokenlists-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-18 20:03:17.296564 tokenlists-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-18 20:02:59.000000 tokenlists-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-18 20:02:59.000000 tokenlists-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-18 20:03:17.296564 tokenlists-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-18 20:02:59.000000 tokenlists-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:17.292564 tokenlists-0.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:17.296564 tokenlists-0.1.4/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tests/functional/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tests/functional/test_uniswap_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:17.296564 tokenlists-0.1.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tests/integration/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:17.296564 tokenlists-0.1.4/tokenlists/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tokenlists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tokenlists/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tokenlists/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tokenlists/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tokenlists/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-18 20:02:59.000000 tokenlists-0.1.4/tokenlists/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-18 20:03:17.000000 tokenlists-0.1.4/tokenlists/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:03:17.296564 tokenlists-0.1.4/tokenlists.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-18 20:03:17.000000 tokenlists-0.1.4/tokenlists.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-18 20:03:17.000000 tokenlists-0.1.4/tokenlists.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:03:17.000000 tokenlists-0.1.4/tokenlists.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 20:03:17.000000 tokenlists-0.1.4/tokenlists.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:03:17.000000 tokenlists-0.1.4/tokenlists.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-18 20:03:17.000000 tokenlists-0.1.4/tokenlists.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 20:03:17.000000 tokenlists-0.1.4/tokenlists.egg-info/top_level.txt
```

### Comparing `tokenlists-0.1.3/.github/ISSUE_TEMPLATE/bug.md` & `tokenlists-0.1.4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/.github/ISSUE_TEMPLATE/feature.md` & `tokenlists-0.1.4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/.github/ISSUE_TEMPLATE/work-item.md` & `tokenlists-0.1.4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/.github/PULL_REQUEST_TEMPLATE.md` & `tokenlists-0.1.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/.github/release-drafter.yml` & `tokenlists-0.1.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/.github/workflows/commitlint.yaml` & `tokenlists-0.1.4/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/.github/workflows/publish.yml` & `tokenlists-0.1.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/.github/workflows/test.yaml` & `tokenlists-0.1.4/.github/workflows/test.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.7, 3.8, 3.9, "3.10", "3.11"]
+                python-version: [3.8, 3.9, "3.10", "3.11"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
```

### Comparing `tokenlists-0.1.3/.github/workflows/title.yaml` & `tokenlists-0.1.4/.github/workflows/title.yaml`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/.gitignore` & `tokenlists-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/.pre-commit-config.yaml` & `tokenlists-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/LICENSE` & `tokenlists-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/PKG-INFO` & `tokenlists-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: tokenlists
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python implementation of Uniswaps' tokenlists
 Home-page: https://github.com/ApeWorX/py-tokenlists
 Author: Ben Hauser
 Author-email: ben@hauser.id
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.2,<4
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `tokenlists-0.1.3/README.md` & `tokenlists-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/pyproject.toml` & `tokenlists-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/setup.py` & `tokenlists-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     author="Ben Hauser",
     author_email="ben@hauser.id",
     description="Python implementation of Uniswaps' tokenlists",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ApeWorX/py-tokenlists",
     include_package_data=True,
-    python_requires=">=3.7.2,<4",
+    python_requires=">=3.8,<4",
     install_requires=[
         "importlib-metadata ; python_version<'3.8'",
         "click>=8.1.3,<9",
         "pydantic>=1.9.2,<2",
         "pyyaml>=6.0,<7",
         "semantic-version>=2.10.0,<3",
         "requests>=2.28.1,<3",
@@ -85,14 +85,13 @@
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `tokenlists-0.1.3/tests/functional/test_schema_fuzzing.py` & `tokenlists-0.1.4/tests/functional/test_schema_fuzzing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import pytest
-import requests
+import requests  # type: ignore[import]
 from hypothesis import HealthCheck, given, settings
 from hypothesis_jsonschema import from_schema
 from pydantic import ValidationError
 
 from tokenlists import TokenList
 
 TOKENLISTS_SCHEMA = "https://uniswap.org/tokenlist.schema.json"
 
 
-def clean_iso_timestamps(tl: dict) -> dict:
-    """
-    Timestamps can be in any format, and our processing handles it okay
-    However, for testing purposes, we want the output format to line up,
-    and unfortunately there is some ambiguity in ISO timestamp formats.
-    """
+def clean_data(tl: dict) -> dict:
+    # NOTE: Timestamps can be in any format, and our processing handles it okay
+    #       However, for testing purposes, we want the output format to line up,
+    #       and unfortunately there is some ambiguity in ISO timestamp formats.
     tl["timestamp"] = tl["timestamp"].replace("Z", "+00:00")
+
+    # NOTE: We do not implement `tokenMap` schema version yet
+    if "tokenMap" in tl:
+        del tl["tokenMap"]
+
     return tl
 
 
 @pytest.mark.fuzzing
 @given(token_list=from_schema(requests.get(TOKENLISTS_SCHEMA).json()))
 @settings(suppress_health_check=(HealthCheck.too_slow,))
 def test_schema(token_list):
     try:
-        assert TokenList.parse_obj(token_list).dict() == clean_iso_timestamps(token_list)
+        assert TokenList.parse_obj(token_list).dict() == clean_data(token_list)
 
     except (ValidationError, ValueError):
         pass  # Expect these kinds of errors
```

### Comparing `tokenlists-0.1.3/tests/integration/test_cli.py` & `tokenlists-0.1.4/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/tokenlists/_cli.py` & `tokenlists-0.1.4/tokenlists/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# TODO: Seems like Click 8.1.5 introduced this
+# mypy: disable-error-code=attr-defined
 import re
 
 import click
 
 from .manager import TokenListManager
 from .typing import TokenSymbol
```

### Comparing `tokenlists-0.1.3/tokenlists/manager.py` & `tokenlists-0.1.4/tokenlists/manager.py`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/tokenlists/typing.py` & `tokenlists-0.1.4/tokenlists/typing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from itertools import chain
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 from pydantic import AnyUrl
 from pydantic import BaseModel as _BaseModel
 from pydantic import validator
 from semantic_version import Version  # type: ignore
 
 ChainId = int
@@ -24,23 +24,81 @@
 
         return super().dict(*args, **kwargs)
 
     class Config:
         froze = True
 
 
+class BridgeInfo(BaseModel):
+    tokenAddress: TokenAddress
+    originBridgeAddress: Optional[TokenAddress] = None
+    destBridgeAddress: Optional[TokenAddress] = None
+
+
 class TokenInfo(BaseModel):
     chainId: ChainId
     address: TokenAddress
     name: TokenName
     decimals: TokenDecimals
     symbol: TokenSymbol
-    logoURI: Optional[AnyUrl] = None
+    logoURI: Optional[str] = None
     tags: Optional[List[TagId]] = None
-    extensions: Optional[dict] = None
+    extensions: Optional[Dict[str, Any]] = None
+
+    @validator("logoURI")
+    def validate_uri(cls, v: Optional[str]) -> Optional[str]:
+        if v is None:
+            return v
+
+        if "://" not in v or not AnyUrl(v, scheme=v.split("://")[0]):
+            raise ValueError(f"'{v}' is not a valid URI")
+
+        return v
+
+    @validator("extensions", pre=True)
+    def parse_extensions(cls, v: Optional[Dict[str, Any]]) -> Optional[Dict[str, Any]]:
+        # 1. Check extension depth first
+        def extension_depth(obj: Optional[Dict[str, Any]]) -> int:
+            if not isinstance(obj, dict) or len(obj) == 0:
+                return 0
+
+            return 1 + max(extension_depth(v) for v in obj.values())
+
+        if (depth := extension_depth(v)) > 3:
+            raise ValueError(f"Extension depth is greater than 3: {depth}")
+
+        # 2. Parse valid extensions
+        if v and "bridgeInfo" in v:
+            raw_bridge_info = v.pop("bridgeInfo")
+            v["bridgeInfo"] = {int(k): BridgeInfo.parse_obj(v) for k, v in raw_bridge_info.items()}
+
+        return v
+
+    @validator("extensions")
+    def extensions_must_contain_allowed_types(
+        cls, d: Optional[Dict[str, Any]]
+    ) -> Optional[Dict[str, Any]]:
+        if not d:
+            return d
+
+        # NOTE: `extensions` is mapping from `str` to either:
+        #       - a parsed `dict` type (e.g. `BaseModel`)
+        #       - a "simple" type (e.g. dict, string, integer or boolean value)
+        for key, val in d.items():
+            if val is not None and not isinstance(val, (BaseModel, str, int, bool, dict)):
+                raise ValueError(f"Incorrect extension field value: {val}")
+
+        return d
+
+    @property
+    def bridge_info(self) -> Optional[BridgeInfo]:
+        if self.extensions and "bridgeInfo" in self.extensions:
+            return self.extensions["bridgeInfo"]  # type: ignore
+
+        return None
 
     @validator("address")
     def address_must_hex(cls, v: str):
         if not v.startswith("0x") or set(v) > set("x0123456789abcdefABCDEF") or len(v) % 2 != 0:
             raise ValueError("Address is not hex")
 
         address_bytes = bytes.fromhex(v[2:])  # NOTE: Skip `0x`
@@ -53,26 +111,14 @@
     @validator("decimals")
     def decimals_must_be_uint8(cls, v: TokenDecimals):
         if not (0 <= v < 256):
             raise ValueError(f"Invalid token decimals: {v}")
 
         return v
 
-    @validator("extensions")
-    def extensions_must_contain_simple_types(cls, d: Optional[dict]) -> Optional[dict]:
-        if not d:
-            return d
-
-        # `extensions` is `Dict[str, Union[str, int, bool, None]]`, but pydantic mutates entries
-        for val in d.values():
-            if not isinstance(val, (str, int, bool)) and val is not None:
-                raise ValueError(f"Incorrect extension field value: {val}")
-
-        return d
-
 
 class Tag(BaseModel):
     name: str
     description: str
 
 
 class TokenListVersion(BaseModel, Version):
@@ -105,15 +151,15 @@
 class TokenList(BaseModel):
     name: str
     timestamp: datetime
     version: TokenListVersion
     tokens: List[TokenInfo]
     keywords: Optional[List[str]] = None
     tags: Optional[Dict[TagId, Tag]] = None
-    logoURI: Optional[AnyUrl] = None
+    logoURI: Optional[str] = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Pull all the tags from all the tokens, reference or not
         all_tags = chain.from_iterable(
             list(token.tags) if token.tags else [] for token in self.tokens
@@ -130,12 +176,22 @@
                 f"Missing reference tags in tokenlist: {token_ref_tags - tokenlist_tags}"
             )
 
     class Config:
         # NOTE: Not frozen as we may need to dynamically modify this
         froze = False
 
+    @validator("logoURI")
+    def validate_uri(cls, v: Optional[str]) -> Optional[str]:
+        if v is None:
+            return v
+
+        if "://" not in v or not AnyUrl(v, scheme=v.split("://")[0]):
+            raise ValueError(f"'{v}' is not a valid URI")
+
+        return v
+
     def dict(self, *args, **kwargs) -> dict:
         data = super().dict(*args, **kwargs)
         # NOTE: This was the easiest way to make sure this property returns isoformat
         data["timestamp"] = self.timestamp.isoformat()
         return data
```

### Comparing `tokenlists-0.1.3/tokenlists.egg-info/PKG-INFO` & `tokenlists-0.1.4/tokenlists.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: tokenlists
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python implementation of Uniswaps' tokenlists
 Home-page: https://github.com/ApeWorX/py-tokenlists
 Author: Ben Hauser
 Author-email: ben@hauser.id
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.2,<4
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `tokenlists-0.1.3/tokenlists.egg-info/SOURCES.txt` & `tokenlists-0.1.4/tokenlists.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.3/tokenlists.egg-info/requires.txt` & `tokenlists-0.1.4/tokenlists.egg-info/requires.txt`

 * *Files identical despite different names*

