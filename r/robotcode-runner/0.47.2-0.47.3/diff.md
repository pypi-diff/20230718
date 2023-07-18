# Comparing `tmp/robotcode_runner-0.47.2.tar.gz` & `tmp/robotcode_runner-0.47.3.tar.gz`

## Comparing `robotcode_runner-0.47.2.tar` & `robotcode_runner-0.47.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    23850 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.47.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    23700 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.47.3/PKG-INFO
```

### Comparing `robotcode_runner-0.47.2/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.47.3/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.2/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.47.3/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.2/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.47.3/src/robotcode/runner/cli/robot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.2/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.47.3/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.2/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.47.3/src/robotcode/runner/cli/discover/discover.py`

 * *Files 4% similar despite different names*

```diff
@@ -425,15 +425,15 @@
     except DataError as err:
         LOGGER.error(err)
         app.exit(DATA_ERROR)
 
     raise UnknownError("Unexpected error happened.")
 
 
-@discover.command(  # type: ignore[attr-defined]
+@discover.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
@@ -485,15 +485,15 @@
 
             app.echo_via_pager(print(collector.all.children[0]))
 
         else:
             app.print_data(ResultItem([collector.all], diagnostics), remove_defaults=True)
 
 
-@discover.command(  # type: ignore[attr-defined]
+@discover.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
@@ -532,15 +532,15 @@
             if collector.tests:
                 app.echo_via_pager(print(collector.tests))
 
         else:
             app.print_data(ResultItem(collector.tests, diagnostics), remove_defaults=True)
 
 
-@discover.command(  # type: ignore[attr-defined]
+@discover.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
@@ -584,15 +584,15 @@
 
 
 @dataclass
 class TagsResult:
     tags: Dict[str, List[TestItem]]
 
 
-@discover.command(  # type: ignore[attr-defined]
+@discover.command(
     context_settings={
         "allow_extra_args": True,
         "ignore_unknown_options": True,
     },
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
@@ -666,15 +666,15 @@
     machine: str
     processor: str
     platform: str
     system: str
     system_version: str
 
 
-@discover.command(  # type: ignore[attr-defined]
+@discover.command(
     add_help_option=True,
 )
 @pass_application
 def info(
     app: Application,
 ) -> None:
     """\
```

### Comparing `robotcode_runner-0.47.2/.gitignore` & `robotcode_runner-0.47.3/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.2/LICENSE.txt` & `robotcode_runner-0.47.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.2/README.md` & `robotcode_runner-0.47.3/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.47.2/pyproject.toml` & `robotcode_runner-0.47.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.47.2",
-  "robotcode-modifiers==0.47.2",
-  "robotcode==0.47.2",
+  "robotcode-robot==0.47.3",
+  "robotcode-modifiers==0.47.3",
+  "robotcode==0.47.3",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.47.2/PKG-INFO` & `robotcode_runner-0.47.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.47.2
+Version: 0.47.3
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.47.2
-Requires-Dist: robotcode-robot==0.47.2
-Requires-Dist: robotcode==0.47.2
+Requires-Dist: robotcode-modifiers==0.47.3
+Requires-Dist: robotcode-robot==0.47.3
+Requires-Dist: robotcode==0.47.3
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

