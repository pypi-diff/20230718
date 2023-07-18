# Comparing `tmp/pytest_dryrun-0.1.0.tar.gz` & `tmp/pytest_dryrun-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dryrun-0.1.0.tar", max compression
+gzip compressed data, was "pytest_dryrun-1.0.0.tar", max compression
```

## Comparing `pytest_dryrun-0.1.0.tar` & `pytest_dryrun-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      771 2023-07-11 13:22:30.829411 pytest_dryrun-0.1.0/README.md
--rw-r--r--   0        0        0      598 2023-07-11 13:23:15.326397 pytest_dryrun-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      148 2023-07-11 12:34:22.310339 pytest_dryrun-0.1.0/pytest_dryrun/__init__.py
--rw-r--r--   0        0        0     1692 2023-07-11 13:12:29.880599 pytest_dryrun-0.1.0/pytest_dryrun/pytest_dryrun.py
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 pytest_dryrun-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 09:59:24.005497 pytest_dryrun-1.0.0/README.md
+-rw-r--r--   0        0        0     1204 2023-07-18 09:59:24.005497 pytest_dryrun-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      530 2023-07-18 09:59:24.005497 pytest_dryrun-1.0.0/pytest_dryrun/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 09:59:24.005497 pytest_dryrun-1.0.0/pytest_dryrun/py.typed
+-rw-r--r--   0        0        0     1692 2023-07-18 09:59:24.005497 pytest_dryrun-1.0.0/pytest_dryrun/pytest_dryrun.py
+-rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 pytest_dryrun-1.0.0/PKG-INFO
```

### Comparing `pytest_dryrun-0.1.0/README.md` & `pytest_dryrun-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # Pytest Dryrun Plugin
 
 A Pytest plugin to ignore tests during collection without reporting them in the
 test summary.
 
+## Installation
+
+With Pip
+
+```sh
+$ pip install pytest-dryrun
+Successfully installed pytest-dryrun-0.1.0
+```
+
 ## Usage
 
 When the `--dryrun` flag is passed to Pytest, only tests marked with `dryrun`
 will be collected and run.
 
 ```py
 @pytest.mark.dryrun
@@ -17,12 +26,23 @@
 
 def test_thing_two():
     """This test will not by run if the `--dryrun` flag is given to Pytest"""
     box = get_box()
     assert "thing two" in box
 ```
 
+Tests can also be marked with `dryrun` using the library's export:
+
+```py
+from pytest_dryrun import dryrun
+
+@dryrun
+def test_thing_one():
+    box = get_box()
+    assert "thing one" in box
+```
+
 If the `--no-dryrun` flag is given, only tests not marked with `dryrun` will be
 collected, meaning that in the example above, only `test_thing_two` will be
 run.
 
 The `--dryrun` and `--no-dryrun` arguments are mutually-exclusive.
```

### Comparing `pytest_dryrun-0.1.0/pytest_dryrun/pytest_dryrun.py` & `pytest_dryrun-1.0.0/pytest_dryrun/pytest_dryrun.py`

 * *Files identical despite different names*

