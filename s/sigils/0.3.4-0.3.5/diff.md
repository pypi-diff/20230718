# Comparing `tmp/sigils-0.3.4.tar.gz` & `tmp/sigils-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigils-0.3.4.tar", last modified: Sun Jul 16 06:24:33 2023, max compression
+gzip compressed data, was "sigils-0.3.5.tar", last modified: Tue Jul 18 00:07:50 2023, max compression
```

## Comparing `sigils-0.3.4.tar` & `sigils-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 06:24:33.526569 sigils-0.3.4/
--rw-rw-rw-   0        0        0     1879 2023-07-16 03:01:57.000000 sigils-0.3.4/.gitignore
--rw-rw-rw-   0        0        0     1096 2023-07-16 06:22:50.000000 sigils-0.3.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1084 2023-07-16 05:32:45.000000 sigils-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     4249 2023-07-16 06:24:33.524572 sigils-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3212 2023-07-16 06:04:34.000000 sigils-0.3.4/README.rst
--rw-rw-rw-   0        0        0     1198 2023-07-16 06:21:43.000000 sigils-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0        0 2023-07-16 02:42:31.000000 sigils-0.3.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 06:24:33.526569 sigils-0.3.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 06:24:33.443528 sigils-0.3.4/sigils/
--rw-rw-rw-   0        0        0     8015 2023-07-16 06:03:15.000000 sigils-0.3.4/sigils/__init__.py
--rw-rw-rw-   0        0        0     1698 2023-07-16 05:18:48.000000 sigils-0.3.4/sigils/__main__.py
--rw-rw-rw-   0        0        0     2631 2023-07-16 06:03:48.000000 sigils-0.3.4/sigils/tests.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:24:33.519568 sigils-0.3.4/sigils.egg-info/
--rw-rw-rw-   0        0        0     4249 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 06:24:33.000000 sigils-0.3.4/sigils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       75 2023-07-16 06:21:28.000000 sigils-0.3.4/test.json
+drwxrwxrwx   0        0        0        0 2023-07-18 00:07:50.215875 sigils-0.3.5/
+-rw-rw-rw-   0        0        0     1879 2023-07-18 00:04:03.000000 sigils-0.3.5/.gitignore
+-rw-rw-rw-   0        0        0     1247 2023-07-18 00:04:03.000000 sigils-0.3.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1084 2023-07-18 00:04:03.000000 sigils-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     4274 2023-07-18 00:07:50.212876 sigils-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3214 2023-07-18 00:04:03.000000 sigils-0.3.5/README.rst
+-rw-rw-rw-   0        0        0     1224 2023-07-18 00:04:03.000000 sigils-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0        0 2023-07-18 00:04:03.000000 sigils-0.3.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:07:50.216873 sigils-0.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 00:07:50.143826 sigils-0.3.5/sigils/
+-rw-rw-rw-   0        0        0     9538 2023-07-18 00:04:03.000000 sigils-0.3.5/sigils/__init__.py
+-rw-rw-rw-   0        0        0     2764 2023-07-18 00:04:03.000000 sigils-0.3.5/sigils/__main__.py
+-rw-rw-rw-   0        0        0     1018 2023-07-18 00:04:03.000000 sigils-0.3.5/sigils/benchmark.py
+-rw-rw-rw-   0        0        0     5441 2023-07-18 00:04:03.000000 sigils-0.3.5/sigils/tests.py
+-rw-rw-rw-   0        0        0    24389 2023-07-18 00:04:03.000000 sigils-0.3.5/sigils/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-18 00:07:50.207863 sigils-0.3.5/sigils.egg-info/
+-rw-rw-rw-   0        0        0     4274 2023-07-18 00:07:49.000000 sigils-0.3.5/sigils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-18 00:07:50.000000 sigils-0.3.5/sigils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 00:07:49.000000 sigils-0.3.5/sigils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-18 00:07:49.000000 sigils-0.3.5/sigils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 00:07:49.000000 sigils-0.3.5/sigils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       75 2023-07-18 00:04:03.000000 sigils-0.3.5/test.json
```

### Comparing `sigils-0.3.4/.gitignore` & `sigils-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sigils-0.3.4/CHANGELOG.md` & `sigils-0.3.5/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Release Notes
 =============
 
+0.3.5 (2023-07-16)
+-------------------
+
+Added (simplified) support for function tools once again.
+
+This should work: %[sigil-name.field.upper]
+
 0.3.4 (2023-07-16)
 -------------------
 
 Restore backwards compatibility with Python 3.9.
 
 0.3.1 (2023-07-15)
 -------------------
```

### Comparing `sigils-0.3.4/LICENSE` & `sigils-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sigils-0.3.4/PKG-INFO` & `sigils-0.3.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sigils
-Version: 0.3.4
-Summary: Interpolate with %[sigils].
+Version: 0.3.5
+Summary: Interpolate %[meta-text] with %[sigils].
 Author-email: Rafael Jesús Guillén Osorio <arthexis@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/arthexis/sigils
 Project-URL: Bug-Tracker, https://github.com/arthexis/sigils/issues
-Keywords: utils,sigils,string,text,context
+Keywords: utils,sigils,string,text,meta-text,context
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
 
 ================
 Sigils
 ================
 
 "An inscribed or painted symbol considered to have magical power."
 
-Sigils is a Python library for magic and string interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
+Sigils is a Python library for text and meta-text interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
 
 Any Python object can be provided as context, including nested dictionaries, lists, and functions. Sigils can be used directly from Python or from the command line. Sigils is thread-safe and has no dependencies outside of the Python standard library.
 
 Installation
 ============
 
 Install Sigils using pip:
```

### Comparing `sigils-0.3.4/README.rst` & `sigils-0.3.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ================
 Sigils
 ================
 
 "An inscribed or painted symbol considered to have magical power."
 
-Sigils is a Python library for magic and string interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
+Sigils is a Python library for text and meta-text interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
 
 Any Python object can be provided as context, including nested dictionaries, lists, and functions. Sigils can be used directly from Python or from the command line. Sigils is thread-safe and has no dependencies outside of the Python standard library.
 
 Installation
 ============
 
 Install Sigils using pip:
```

### Comparing `sigils-0.3.4/pyproject.toml` & `sigils-0.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sigils"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
     {name = "Rafael Jesús Guillén Osorio", email = "arthexis@gmail.com"},
 ]
-description = "Interpolate with %[sigils]."
+description = "Interpolate %[meta-text] with %[sigils]."
 readme = "README.rst"
 requires-python = ">=3.9"
-keywords = ["utils", "sigils", "string", "text", "context"]
+keywords = ["utils", "sigils", "string", "text", "meta-text", "context"]
 license = {text = "MIT"}
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Libraries',
     'Topic :: Text Processing :: Markup',
     'Topic :: Software Development :: Pre-processors',
```

### Comparing `sigils-0.3.4/sigils/__init__.py` & `sigils-0.3.5/sigils/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import threading
+from .tools import tools
 
 
 class Sigil:
     _cache = threading.local()
 
     class Context:
         _context = threading.local()
@@ -35,103 +36,137 @@
         """
         self.template = template
         self.pattern = getattr(self._cache, 'value', {}).get(template)
         if self.pattern is None:
             self.pattern = re.compile(r'%\[(.*?)\]')
             self._cache.value = {template: self.pattern}
 
-    def _resolve(self, context, depth=0, execute=True, max_depth=6):
+    def _run_func_with_sigil_args(self, func, func_args, value, context, execute, max_depth, debug):
+        num_args = func.__code__.co_argcount
+        if func_args:
+            if debug:
+                print(f"Tool: {func}, value: {value}, func_args: {func_args}")
+            resolved_args = [Sigil(f'%[{arg}]').interpolate(
+                context, execute, max_depth
+            ) for arg in func_args]
+            if debug:
+                print(f"Resolved args: {resolved_args}")
+            if num_args > 0:
+                if resolved_args and '%[' not in resolved_args[0]:
+                    return func(resolved_args[0], *resolved_args[1:num_args - 1])
+                else:
+                    return func(func_args[0], *func_args[1:num_args - 1])
+            else:
+                return func()
+        else:
+            if num_args == 1:
+                return func(str(value))
+            else:
+                return func()
+
+    def _resolve(self, context, depth=0, execute=True, max_depth=6, debug=False):
         resolved = {}
         for match in self.pattern.findall(self.template):
+            if debug:
+                print(f"Found match: {match}")
             keys = match.split('.')
+            if debug:
+                print(f"Split keys: {keys}")
             value = context
-            function_args = []
-            try:
-                for i, key in enumerate(keys):
-                    if ':' in key:
-                        key, *function_args = key.split(':')
-                    literal = False
-                    if key.startswith('%'):
-                        key = key[1:]
-                        literal = True
-                    if literal:
-                        temp = key
-                    elif isinstance(value, dict):
-                        temp = value.get(key)
-                    elif isinstance(value, list) and key.isdigit():
-                        temp = value[int(key)]
+            func_args = []
+            for i, key in enumerate(keys):
+                if ':' in key:
+                    key_parts = key.split(':')
+                    key = key_parts[0]
+                    func_args = key_parts[1:]
+                if debug:
+                    print(f"Processing key: {key}, func_args: {func_args}")
+                literal = False
+                if key.startswith('%'):
+                    key = key[1:]
+                    literal = True
+                if literal:
+                    temp = key
+                elif value and isinstance(value, dict) and key in value:
+                    if debug:
+                        print(f"Value is a dict with the key: {value}")
+                    temp = value.get(key, None)
+                    if callable(temp):
+                        temp = self._run_func_with_sigil_args(
+                            temp, func_args, value, context, execute, max_depth, debug)
+                elif value and isinstance(value, list) and key.isdigit():
+                    if debug:
+                        print(f"Value is a list: {value}")
+                    temp = value[int(key)]
+                elif key in tools:
+                    if debug:
+                        print(f"Found tool: {key}")
+                    tool_func = tools[key]
+                    if callable(tool_func):
+                        temp = self._run_func_with_sigil_args(
+                            tool_func, func_args, value, context, execute, max_depth, debug)
                     else:
-                        temp = None
-                    if temp is None and '-' in key and not literal:
-                        temp = value.get(key.replace('-', '_')) if isinstance(value, dict) else None
-                    if temp is None and hasattr(value, key) and not literal:
-                        temp = getattr(value, key)
-                    if temp is None and '-' in key and hasattr(value, key.replace('-', '_')) and not literal:
-                        temp = getattr(value, key.replace('-', '_'))
-                    if temp is not None:
-                        value = temp
-                        if callable(value) and execute:
-                            if function_args:
-                                resolved_function_args = [Sigil(f'%[{arg}]').interpolate(context) for arg in function_args]
-                                value = value(*resolved_function_args)
-                            else:
-                                value = value()
-                    else:
-                        value = None
-                        break
-            except (TypeError, AttributeError):
-                value = None
+                        if debug:
+                            print(f"Non-callable tool: {tool_func}")
+                        temp = tool_func
+                else:
+                    if debug:
+                        print(f"Value is an object: {value}")
+                    temp = None
+                if debug:
+                    print(f"Temp value: {temp}")
+                if temp and callable(temp):
+                    temp = temp()
+                if temp is None and '-' in key and not literal:
+                    temp = value.get(key.replace('-', '_')) if isinstance(value, dict) else None
+                if temp is None and hasattr(value, key) and not literal:
+                    temp = getattr(value, key)
+                if temp is None and '-' in key and hasattr(value, key.replace('-', '_')) and not literal:
+                    temp = getattr(value, key.replace('-', '_'))
+                if temp is not None:
+                    value = temp
+                else:
+                    if debug:
+                        print(f"Could not find value for key: {key}")
+                    value = None
+                    break
             if value is not None:
                 resolved[match] = value
             else:
                 global_context = getattr(Sigil.Context._context, 'value', {})
                 value = global_context.get(match.replace('-', '_'), None)
                 if value is not None:
                     resolved[match] = value
         if depth < max_depth:
             for key, value in list(resolved.items()):
                 if isinstance(value, str) and '%' in value:
+                    if debug:
+                        print(f"Found nested sigil: {value}")
                     s = Sigil(value)
-                    resolved_value = s._resolve(context, depth + 1, execute, max_depth)
+                    resolved_value = s._resolve(context, depth + 1, execute, max_depth, debug)
                     if resolved_value:
                         resolved[key] = {
-                            'value': s.interpolate(context, execute, max_depth),
+                            'value': s.interpolate(context, execute, max_depth, debug),
                             'sub_values': resolved_value
                         }
                     else:
                         resolved[key] = {'value': value}
         return resolved
 
-    def _get_value(self, key, value):
-        if isinstance(value, dict):
-            temp = value.get(key)
-            if temp is None and '-' in key:
-                temp = value.get(key.replace('-', '_'))
-        elif isinstance(value, list):
-            try:
-                temp = value[int(key)]
-            except (IndexError, ValueError):
-                temp = None
-        else:
-            temp = getattr(value, key, None)
-            if temp is None and '-' in key:
-                temp = getattr(value, key.replace('-', '_'), None)
-        return temp
-
-    def interpolate(self, context, execute=True, max_depth=6, handle_errors="propagate"):
+    def interpolate(self, context, execute=True, max_depth=6, handle_errors="propagate", debug=False):
         """
         Interpolate the template with the provided context.
 
         Args:
             context (dict or object): The context from which to take the values.
             execute (bool, optional): If True, execute any callable values found in the context. Defaults to True.
             max_depth (int, optional): The maximum depth for resolving nested sigils. Defaults to 6.
             handle_errors (str, optional): How to handle errors that occur during interpolation. 
                 Can be "propagate" (raise the error), "ignore" (return the original template), 
-                or "replace" (replace the template with the error message). Defaults to "propagate".
+                "replace" (replace the template with the error message). Defaults to "propagate".
 
         Returns:
             str: The interpolated string.
 
         Raises:
             Exception: If handle_errors is set to "propagate" and an error occurs during interpolation.
 
@@ -143,15 +178,15 @@
         print(s.interpolate(context))  # Outputs: "Hello, Alice!"
         ```
 
         """
         if context is None:
             context = Sigil.Context.current_context
         try:
-            resolved = self._resolve(context, 0, execute, max_depth)
+            resolved = self._resolve(context, 0, execute, max_depth, debug)
         except Exception as e:
             if handle_errors == "propagate":
                 raise e
             elif handle_errors == "ignore":
                 return self.template
             else:  # handle_errors == "replace"
                 return str(e)
@@ -202,14 +237,12 @@
         ```python
         s = Sigil("Hello, %[name]!")
         context = {"name": "Alice"}
         print(s % context)  # Outputs: "Hello, Alice!"
         ```
 
         """
-        print(f"Context: {context}")
-        result = self.interpolate(context)
-        print(f"Interpolated result: {result}") 
+        result = self.interpolate(context or {})
         return result
         
 
 __all__ = ['Sigil']
```

### Comparing `sigils-0.3.4/sigils.egg-info/PKG-INFO` & `sigils-0.3.5/sigils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sigils
-Version: 0.3.4
-Summary: Interpolate with %[sigils].
+Version: 0.3.5
+Summary: Interpolate %[meta-text] with %[sigils].
 Author-email: Rafael Jesús Guillén Osorio <arthexis@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/arthexis/sigils
 Project-URL: Bug-Tracker, https://github.com/arthexis/sigils/issues
-Keywords: utils,sigils,string,text,context
+Keywords: utils,sigils,string,text,meta-text,context
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
 
 ================
 Sigils
 ================
 
 "An inscribed or painted symbol considered to have magical power."
 
-Sigils is a Python library for magic and string interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
+Sigils is a Python library for text and meta-text interpolation. It provides advanced capabilities such as context-based interpolation, function execution, nested and recursive interpolation, case-insensitive matching, and global context support.
 
 Any Python object can be provided as context, including nested dictionaries, lists, and functions. Sigils can be used directly from Python or from the command line. Sigils is thread-safe and has no dependencies outside of the Python standard library.
 
 Installation
 ============
 
 Install Sigils using pip:
```

