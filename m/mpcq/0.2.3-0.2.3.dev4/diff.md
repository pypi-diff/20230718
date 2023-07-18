# Comparing `tmp/mpcq-0.2.3.tar.gz` & `tmp/mpcq-0.2.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcq-0.2.3.tar", last modified: Tue Jul 18 11:23:00 2023, max compression
+gzip compressed data, was "mpcq-0.2.3.dev4.tar", last modified: Tue Jul 18 11:13:46 2023, max compression
```

## Comparing `mpcq-0.2.3.tar` & `mpcq-0.2.3.dev4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:23:00.427240 mpcq-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:23:00.415240 mpcq-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:23:00.419240 mpcq-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-18 11:22:23.000000 mpcq-0.2.3/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-18 11:22:23.000000 mpcq-0.2.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:22:23.000000 mpcq-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-18 11:22:23.000000 mpcq-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 11:22:23.000000 mpcq-0.2.3/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-18 11:23:00.427240 mpcq-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-18 11:22:23.000000 mpcq-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:23:00.423240 mpcq-0.2.3/mpcq/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/submission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:23:00.427240 mpcq-0.2.3/mpcq/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/tests/test_submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 11:22:23.000000 mpcq-0.2.3/mpcq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:23:00.423240 mpcq-0.2.3/mpcq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-18 11:23:00.000000 mpcq-0.2.3/mpcq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 11:23:00.000000 mpcq-0.2.3/mpcq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:23:00.000000 mpcq-0.2.3/mpcq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-18 11:23:00.000000 mpcq-0.2.3/mpcq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 11:23:00.000000 mpcq-0.2.3/mpcq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-18 11:22:23.000000 mpcq-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-18 11:22:23.000000 mpcq-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-18 11:23:00.427240 mpcq-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:22:23.000000 mpcq-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:13:46.842106 mpcq-0.2.3.dev4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:13:46.838106 mpcq-0.2.3.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:13:46.838106 mpcq-0.2.3.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-18 11:13:46.842106 mpcq-0.2.3.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:13:46.838106 mpcq-0.2.3.dev4/mpcq/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/submission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:13:46.842106 mpcq-0.2.3.dev4/mpcq/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/tests/test_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/mpcq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:13:46.842106 mpcq-0.2.3.dev4/mpcq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-18 11:13:46.000000 mpcq-0.2.3.dev4/mpcq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 11:13:46.000000 mpcq-0.2.3.dev4/mpcq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:13:46.000000 mpcq-0.2.3.dev4/mpcq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-18 11:13:46.000000 mpcq-0.2.3.dev4/mpcq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 11:13:46.000000 mpcq-0.2.3.dev4/mpcq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-18 11:13:46.842106 mpcq-0.2.3.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:13:01.000000 mpcq-0.2.3.dev4/setup.py
```

### Comparing `mpcq-0.2.3/.github/workflows/lint.yaml` & `mpcq-0.2.3.dev4/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/.github/workflows/publish.yaml` & `mpcq-0.2.3.dev4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/.pre-commit-config.yaml` & `mpcq-0.2.3.dev4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/PKG-INFO` & `mpcq-0.2.3.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcq
-Version: 0.2.3
+Version: 0.2.3.dev4
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpcq
 #### A Python package by the Asteroid Institute, a program of the B612 Foundation
```

### Comparing `mpcq-0.2.3/README.md` & `mpcq-0.2.3.dev4/README.md`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/mpcq/client.py` & `mpcq-0.2.3.dev4/mpcq/client.py`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/mpcq/observation.py` & `mpcq-0.2.3.dev4/mpcq/observation.py`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/mpcq/submission.py` & `mpcq-0.2.3.dev4/mpcq/submission.py`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/mpcq/tests/test_integration.py` & `mpcq-0.2.3.dev4/mpcq/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/mpcq/tests/test_utils.py` & `mpcq-0.2.3.dev4/mpcq/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/mpcq/utils.py` & `mpcq-0.2.3.dev4/mpcq/utils.py`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/mpcq.egg-info/PKG-INFO` & `mpcq-0.2.3.dev4/mpcq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcq
-Version: 0.2.3
+Version: 0.2.3.dev4
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpcq
 #### A Python package by the Asteroid Institute, a program of the B612 Foundation
```

### Comparing `mpcq-0.2.3/mpcq.egg-info/SOURCES.txt` & `mpcq-0.2.3.dev4/mpcq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/requirements.txt` & `mpcq-0.2.3.dev4/requirements.txt`

 * *Files identical despite different names*

### Comparing `mpcq-0.2.3/setup.cfg` & `mpcq-0.2.3.dev4/setup.cfg`

 * *Files identical despite different names*

