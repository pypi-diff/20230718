# Comparing `tmp/pytest_textual_snapshot-0.2.0.tar.gz` & `tmp/pytest_textual_snapshot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_textual_snapshot-0.2.0.tar", max compression
+gzip compressed data, was "pytest_textual_snapshot-0.3.0.tar", max compression
```

## Comparing `pytest_textual_snapshot-0.2.0.tar` & `pytest_textual_snapshot-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2023-06-27 13:20:54.234165 pytest_textual_snapshot-0.2.0/LICENSE
--rw-r--r--   0        0        0     1562 2023-06-27 13:20:54.234390 pytest_textual_snapshot-0.2.0/README.md
--rw-r--r--   0        0        0     1503 2023-07-12 14:34:46.975557 pytest_textual_snapshot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7553 2023-06-27 13:20:54.234651 pytest_textual_snapshot-0.2.0/pytest_textual_snapshot.py
--rw-r--r--   0        0        0    11112 2023-06-27 13:20:54.234850 pytest_textual_snapshot-0.2.0/resources/snapshot_report_template.jinja2
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 pytest_textual_snapshot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-27 13:20:54.234165 pytest_textual_snapshot-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1562 2023-06-27 13:20:54.234390 pytest_textual_snapshot-0.3.0/README.md
+-rw-r--r--   0        0        0     1503 2023-07-18 11:27:56.120331 pytest_textual_snapshot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7627 2023-07-18 11:27:56.121125 pytest_textual_snapshot-0.3.0/pytest_textual_snapshot.py
+-rw-r--r--   0        0        0    11112 2023-06-27 13:20:54.234850 pytest_textual_snapshot-0.3.0/resources/snapshot_report_template.jinja2
+-rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 pytest_textual_snapshot-0.3.0/PKG-INFO
```

### Comparing `pytest_textual_snapshot-0.2.0/LICENSE` & `pytest_textual_snapshot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_textual_snapshot-0.2.0/README.md` & `pytest_textual_snapshot-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_textual_snapshot-0.2.0/pyproject.toml` & `pytest_textual_snapshot-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-textual-snapshot"
-version = "0.2.0"
+version = "0.3.0"
 description = "Snapshot testing for Textual apps"
 authors = ["Darren Burns <darren@textualize.io>"]
 maintainers = ["Darren Burns <darren@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/darrenburns/pytest-textual-snapshot"
 classifiers = [
```

### Comparing `pytest_textual_snapshot-0.2.0/pytest_textual_snapshot.py` & `pytest_textual_snapshot-0.3.0/pytest_textual_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,31 @@
 
 import os
 from dataclasses import dataclass
 from datetime import datetime
 from operator import attrgetter
 from os import PathLike
 from pathlib import Path, PurePath
-from typing import Awaitable, Union, List, Optional, Callable, Iterable
+from typing import Awaitable, Union, List, Optional, Callable, Iterable, TYPE_CHECKING
 
 import pytest
 from _pytest.config import ExitCode
 from _pytest.fixtures import FixtureRequest
 from _pytest.main import Session
 from _pytest.terminal import TerminalReporter
 from jinja2 import Template
 from rich.console import Console
 from syrupy import SnapshotAssertion
 
-from textual._doc import take_svg_screenshot
-from textual._import_app import import_app
-from textual.app import App
-from textual.pilot import Pilot
+if TYPE_CHECKING:
+    from textual.pilot import Pilot
 
 TEXTUAL_SNAPSHOT_SVG_KEY = pytest.StashKey[str]()
 TEXTUAL_ACTUAL_SVG_KEY = pytest.StashKey[str]()
 TEXTUAL_SNAPSHOT_PASS = pytest.StashKey[bool]()
-TEXTUAL_APP_KEY = pytest.StashKey[App]()
 
 
 def pytest_addoption(parser):
     parser.addoption(
         '--snapshot-report', action='store', default="snapshot_report.html", help='Snapshot test output HTML path.'
     )
 
@@ -64,41 +61,44 @@
             run_before: An arbitrary callable that runs arbitrary code before taking the
                 screenshot. Use this to simulate complex user interactions with the app
                 that cannot be simulated by key presses.
 
         Returns:
             Whether the screenshot matches the snapshot.
         """
+        from textual._import_app import import_app
         node = request.node
         path = Path(app_path)
         if path.is_absolute():
             # If the user supplies an absolute path, just use it directly.
             app = import_app(str(path.resolve()))
         else:
             # If a relative path is supplied by the user, it's relative to the location of the pytest node,
             # NOT the location that `pytest` was invoked from.
             node_path = node.path.parent
             resolved = (node_path / app_path).resolve()
             app = import_app(str(resolved))
 
+        from textual._doc import take_svg_screenshot
         actual_screenshot = take_svg_screenshot(
             app=app,
             press=press,
             terminal_size=terminal_size,
             run_before=run_before,
         )
         result = snapshot == actual_screenshot
 
         if result is False:
             # The split and join below is a mad hack, sorry...
             node.stash[TEXTUAL_SNAPSHOT_SVG_KEY] = "\n".join(
                 str(snapshot).splitlines()[1:-1]
             )
             node.stash[TEXTUAL_ACTUAL_SVG_KEY] = actual_screenshot
-            node.stash[TEXTUAL_APP_KEY] = app
+            from textual.app import App
+            node.stash[pytest.StashKey[App]()] = app
         else:
             node.stash[TEXTUAL_SNAPSHOT_PASS] = True
 
         return result
 
     return compare
 
@@ -129,15 +129,16 @@
     num_snapshots_passing = 0
 
     for item in session.items:
         # Grab the data our fixture attached to the pytest node
         num_snapshots_passing += int(item.stash.get(TEXTUAL_SNAPSHOT_PASS, False))
         snapshot_svg = item.stash.get(TEXTUAL_SNAPSHOT_SVG_KEY, None)
         actual_svg = item.stash.get(TEXTUAL_ACTUAL_SVG_KEY, None)
-        app = item.stash.get(TEXTUAL_APP_KEY, None)
+        from textual.app import App
+        app = item.stash.get(pytest.StashKey[App](), None)
 
         if app:
             path, line_index, name = item.reportinfo()
             diffs.append(
                 SvgSnapshotDiff(
                     snapshot=str(snapshot_svg),
                     actual=str(actual_svg),
```

### Comparing `pytest_textual_snapshot-0.2.0/resources/snapshot_report_template.jinja2` & `pytest_textual_snapshot-0.3.0/resources/snapshot_report_template.jinja2`

 * *Files identical despite different names*

### Comparing `pytest_textual_snapshot-0.2.0/PKG-INFO` & `pytest_textual_snapshot-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-textual-snapshot
-Version: 0.2.0
+Version: 0.3.0
 Summary: Snapshot testing for Textual apps
 Home-page: https://github.com/darrenburns/pytest-textual-snapshot
 License: MIT
 Author: Darren Burns
 Author-email: darren@textualize.io
 Maintainer: Darren Burns
 Maintainer-email: darren@textualize.io
```

