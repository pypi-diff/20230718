# Comparing `tmp/docwalker-1.0.1.tar.gz` & `tmp/docwalker-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docwalker-1.0.1.tar", max compression
+gzip compressed data, was "docwalker-1.0.2.tar", max compression
```

## Comparing `docwalker-1.0.1.tar` & `docwalker-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-14 01:02:51.187406 docwalker-1.0.1/docwalker/__init__.py
--rw-r--r--   0        0        0      328 2023-07-15 21:06:52.667191 docwalker-1.0.1/docwalker/__main__.py
--rw-r--r--   0        0        0     2549 2023-07-15 21:08:59.854343 docwalker-1.0.1/docwalker/app.py
--rw-r--r--   0        0        0     2029 2023-07-16 05:47:04.424839 docwalker-1.0.1/docwalker/cli.py
--rw-r--r--   0        0        0     2236 2023-07-15 04:42:56.411048 docwalker-1.0.1/docwalker/parser.py
--rw-r--r--   0        0        0      200 2023-07-15 20:29:50.785817 docwalker-1.0.1/docwalker/styles/main.css
--rw-r--r--   0        0        0     1091 2023-07-14 00:40:47.748612 docwalker-1.0.1/LICENSE
--rw-r--r--   0        0        0     1226 2023-07-16 05:20:39.834783 docwalker-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1673 2023-07-16 05:45:17.255285 docwalker-1.0.1/README.md
--rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 docwalker-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 04:09:12.113322 docwalker-1.0.2/docwalker/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-18 04:07:58.699860 docwalker-1.0.2/docwalker/__main__.py
+-rw-r--r--   0        0        0     2412 2023-07-18 04:11:48.078942 docwalker-1.0.2/docwalker/app.py
+-rw-r--r--   0        0        0     2108 2023-07-18 04:08:03.643508 docwalker-1.0.2/docwalker/cli.py
+-rw-r--r--   0        0        0     2460 2023-07-17 22:57:00.465598 docwalker-1.0.2/docwalker/parser.py
+-rw-r--r--   0        0        0      200 2023-07-15 20:29:50.785817 docwalker-1.0.2/docwalker/styles/main.css
+-rw-r--r--   0        0        0     1091 2023-07-14 00:40:47.748612 docwalker-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1225 2023-07-18 04:15:12.219545 docwalker-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1738 2023-07-18 04:20:45.431547 docwalker-1.0.2/README.md
+-rw-r--r--   0        0        0     2519 1970-01-01 00:00:00.000000 docwalker-1.0.2/PKG-INFO
```

### Comparing `docwalker-1.0.1/docwalker/app.py` & `docwalker-1.0.2/docwalker/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,32 +27,23 @@
 
 Press the **`O`** key to open the directory tree and select a document to view
 its documentation.
 """
 
 
 class ViewerApp(App):
-    """@
-    ## Class: ViewerApp
-    @"""
-
     CSS_PATH = "styles/main.css"
 
     BINDINGS = [
         Binding(key="o", action="open_file", description="Open File"),
         Binding(key="t", action="toggle_dark", description="Toggle Light/Dark Mode"),
         Binding(key="q", action="quit", description="Quit"),
     ]
 
     def __init__(self, src_dir: str, config: dict, **kwargs):
-        """@
-        ### def __init__
-
-        Initialization function.
-        @"""
         self._show_directory = False
         self._src_dir = src_dir
         self._config = config
         self._parser = Parser(self._config)
         super().__init__(**kwargs)
 
     async def action_open_file(self):
```

### Comparing `docwalker-1.0.1/docwalker/cli.py` & `docwalker-1.0.2/docwalker/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,20 +28,26 @@
 [parser.listing]
 syntax_start = {_default_listing_syntax_start}
 syntax_end = {_default_listing_syntax_end}
 
 """
 
 PARSER = ArgumentParser(prog="docwalker", description=_description)
-PARSER.add_argument("src_dir", type=str, help="The source directory to examine.")
+PARSER.add_argument(
+    "-d",
+    "--dir",
+    type=str,
+    default=".",
+    help="The source directory to examine. [default: the current directory '.']",
+)
 PARSER.add_argument(
     "-f",
     "--file",
     type=str,
-    help="The config file to reference for custom parsing [default: '<src_dir>/.dwconf']",
+    help="The config file to reference for custom parsing [default: '<dir>/.dwconf']",
 )
 
 
 def generate_config(path: str = ".dwconf") -> dict:
     output = {}
     if not os.path.exists(path):
         with open(path, "w+") as file:
```

### Comparing `docwalker-1.0.1/docwalker/parser.py` & `docwalker-1.0.2/docwalker/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 class Parser:
     def __init__(self, config: dict) -> None:
         self._config = config
-
         self._lines = []
-
         self._block = False
-        self._block_len = 0
-
         self._listing = False
+        self._continuous = False
 
     def parse(self, path: str) -> str:
         self._lines = []
         with open(path, "r") as file:
             for line in file.readlines():
                 self.parse_line(line)
         return "".join(self._lines)
 
     def parse_line(self, line: str):
         _line = line.lstrip()
         # NORMAL LOGIC
         if _line.startswith(self._config["inline_syntax"]):
-            self._lines.append(_line.lstrip(self._config["inline_syntax"]) + "\n")
+            self._lines.append(
+                _line.lstrip(self._config["inline_syntax"])
+                + ("\n" if self._continuous else "")
+            )
+            self._continuous = True
+            return
+        else:
+            self._continuous = False
         # END NORMAL LOGIC
 
         # BLOCK LOGIC
-        elif _line.startswith(self._config["block_syntax_start"]):
+        if _line.startswith(self._config["block_syntax_start"]):
             self._block = True
             temp = _line.lstrip(self._config["block_syntax_start"])
             if len(temp) > 0:
                 self._lines.append(temp)
         elif _line.strip().endswith(self._config["block_syntax_end"]) and self._block:
             self._block = False
             temp = _line.strip().rstrip(self._config["block_syntax_end"])
             if len(temp) > 0:
                 self._lines.append(temp)
+            self._lines.append("\n")
         elif self._block:
             if len(_line) == 0:
                 self._lines.append("\n")
             else:
                 self._lines.append(_line)
         # END BLOCK LOGIC
```

### Comparing `docwalker-1.0.1/LICENSE` & `docwalker-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docwalker-1.0.1/pyproject.toml` & `docwalker-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "docwalker"
-version = "1.0.1"
+version = "1.0.2"
 description = "Quickly view documentation in source code in a language-agnostic way."
 authors = ["Conner Marzen <connermarzen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["tui", "documentation", "viewer"]
 classifiers = [
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
   #   5 - Production/Stable
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `docwalker-1.0.1/README.md` & `docwalker-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![docwalker_windows_screenshot](./doc/windows_screenshot.png)
+
 # docwalker
 
 [![PyPI version](https://badge.fury.io/py/docwalker.svg)](https://badge.fury.io/py/docwalker)
 
 Quickly view documentation in source code in a language-agnostic way.
 
 Docwalker processes custom characters in both inline and block comments to
```

### Comparing `docwalker-1.0.1/PKG-INFO` & `docwalker-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: docwalker
-Version: 1.0.1
+Version: 1.0.2
 Summary: Quickly view documentation in source code in a language-agnostic way.
 License: MIT
 Keywords: tui,documentation,viewer
 Author: Conner Marzen
 Author-email: connermarzen@gmail.com
 Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: textual (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
 
+![docwalker_windows_screenshot](./doc/windows_screenshot.png)
+
 # docwalker
 
 [![PyPI version](https://badge.fury.io/py/docwalker.svg)](https://badge.fury.io/py/docwalker)
 
 Quickly view documentation in source code in a language-agnostic way.
 
 Docwalker processes custom characters in both inline and block comments to
```

