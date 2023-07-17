# Comparing `tmp/pdbp-1.4.2.tar.gz` & `tmp/pdbp-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbp-1.4.2.tar", last modified: Thu Jun 29 21:48:04 2023, max compression
+gzip compressed data, was "pdbp-1.4.3.tar", last modified: Mon Jul 17 22:27:07 2023, max compression
```

## Comparing `pdbp-1.4.2.tar` & `pdbp-1.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:48:04.510915 pdbp-1.4.2/
--rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.4.2/.gitignore
--rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.4.2/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.4.2/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.4.2/LICENSE
--rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.4.2/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     6821 2023-06-29 21:48:04.510974 pdbp-1.4.2/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4805 2023-06-22 15:48:47.000000 pdbp-1.4.2/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.4.2/SECURITY.md
--rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-06-29 21:48:04.511145 pdbp-1.4.2/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5379 2023-06-29 21:47:09.000000 pdbp-1.4.2/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:48:04.510263 pdbp-1.4.2/src/
--rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.4.2/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:48:04.510811 pdbp-1.4.2/src/pdbp.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     6821 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      293 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      109 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-06-29 21:48:04.000000 pdbp-1.4.2/src/pdbp.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)    57865 2023-06-29 21:47:09.000000 pdbp-1.4.2/src/pdbp.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:27:07.104875 pdbp-1.4.3/
+-rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.4.3/.gitignore
+-rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.4.3/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.4.3/CONTRIBUTING.md
+-rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.4.3/LICENSE
+-rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.4.3/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     6964 2023-07-17 22:27:07.104927 pdbp-1.4.3/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     4948 2023-07-17 22:26:34.000000 pdbp-1.4.3/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.4.3/SECURITY.md
+-rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-07-17 22:27:07.105103 pdbp-1.4.3/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5954 2023-07-17 22:26:34.000000 pdbp-1.4.3/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:27:07.104149 pdbp-1.4.3/src/
+-rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.4.3/src/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:27:07.104755 pdbp-1.4.3/src/pdbp.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     6964 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      109 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)    57871 2023-07-17 22:26:34.000000 pdbp-1.4.3/src/pdbp.py
```

### Comparing `pdbp-1.4.2/.gitignore` & `pdbp-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.2/CODE_OF_CONDUCT.md` & `pdbp-1.4.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.2/CONTRIBUTING.md` & `pdbp-1.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.2/LICENSE` & `pdbp-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.2/PKG-INFO` & `pdbp-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.4.2
+Version: 1.4.3
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -44,15 +44,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
+<img width="680" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
@@ -93,17 +93,16 @@
 
 ```bash
 python -m pdbp <script.py>
 ```
 
 --------
 
-Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
-
-Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
+Basic **``Pdb+``** console commands:
+``n``, ``c``, ``s``, ``u``, ``d`` => ``next``, ``continue``, ``step``, ``up``, ``down``
 
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
 --------
 
 **``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
 
@@ -161,14 +160,20 @@
 
 > **Non-Sticky Mode:**
 
 <img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
 
 --------
 
+### Tab completion:
+
+<img width="584" alt="Pdb+ Tab Completion" src="https://user-images.githubusercontent.com/6788579/254074593-31fcd816-7a3f-445d-82e9-fc2c8d4d873c.png">
+
+--------
+
 ### Multi-layer highlighting in the same stack:
 
 <img width="536" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207925754-4d4ffce5-be6c-44b6-b614-ae0e800a93d8.png">
 
 
 ### More examples:
```

### Comparing `pdbp-1.4.2/README.md` & `pdbp-1.4.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
+<img width="680" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
@@ -45,17 +45,16 @@
 
 ```bash
 python -m pdbp <script.py>
 ```
 
 --------
 
-Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
-
-Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
+Basic **``Pdb+``** console commands:
+``n``, ``c``, ``s``, ``u``, ``d`` => ``next``, ``continue``, ``step``, ``up``, ``down``
 
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
 --------
 
 **``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
 
@@ -113,14 +112,20 @@
 
 > **Non-Sticky Mode:**
 
 <img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
 
 --------
 
+### Tab completion:
+
+<img width="584" alt="Pdb+ Tab Completion" src="https://user-images.githubusercontent.com/6788579/254074593-31fcd816-7a3f-445d-82e9-fc2c8d4d873c.png">
+
+--------
+
 ### Multi-layer highlighting in the same stack:
 
 <img width="536" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207925754-4d4ffce5-be6c-44b6-b614-ae0e800a93d8.png">
 
 
 ### More examples:
```

### Comparing `pdbp-1.4.2/setup.py` & `pdbp-1.4.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,35 +39,43 @@
             sys.exit()
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
         os.system("rm -f dist/*.egg; rm -f dist/*.tar.gz; rm -f dist/*.whl")
         os.system("rm -rf build/bdist.*; rm -rf build/lib")
         print("\n*** Installing build: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'build>=0.10.0'")
+        os.system("python -m pip install --upgrade 'build'")
         print("\n*** Installing pkginfo: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'pkginfo>=1.9.6'")
+        os.system("python -m pip install --upgrade 'pkginfo'")
         print("\n*** Installing readme-renderer: *** (For PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'readme-renderer>=40.0'")
+        os.system("python -m pip install --upgrade 'readme-renderer'")
+        print("\n*** Installing jaraco.classes: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'jaraco.classes'")
+        print("\n*** Installing more-itertools: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'more-itertools'")
+        print("\n*** Installing zipp: *** (Required for PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'zipp'")
+        print("\n*** Installing importlib-metadata: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'importlib-metadata'")
+        print("\n*** Installing keyring, requests-toolbelt: *** (For PyPI)\n")
+        os.system("python -m pip install --upgrade keyring requests-toolbelt")
         print("\n*** Installing twine: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'twine>=4.0.2'")
-        print("\n*** Installing tqdm: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade tqdm")
+        os.system("python -m pip install --upgrade 'twine'")
         print("\n*** Rebuilding distribution packages: ***\n")
         os.system("python -m build")  # Create new tar/wheel
         print("\n*** Publishing The Release to PyPI: ***\n")
         os.system("python -m twine upload dist/*")  # Requires ~/.pypirc Keys
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="pdbp",
-    version="1.4.2",
+    version="1.4.3",
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="pdb debugger tab color completion",
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
```

### Comparing `pdbp-1.4.2/src/pdbp.egg-info/PKG-INFO` & `pdbp-1.4.3/src/pdbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.4.2
+Version: 1.4.3
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -44,15 +44,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
+<img width="680" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
@@ -93,17 +93,16 @@
 
 ```bash
 python -m pdbp <script.py>
 ```
 
 --------
 
-Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
-
-Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
+Basic **``Pdb+``** console commands:
+``n``, ``c``, ``s``, ``u``, ``d`` => ``next``, ``continue``, ``step``, ``up``, ``down``
 
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
 --------
 
 **``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
 
@@ -161,14 +160,20 @@
 
 > **Non-Sticky Mode:**
 
 <img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
 
 --------
 
+### Tab completion:
+
+<img width="584" alt="Pdb+ Tab Completion" src="https://user-images.githubusercontent.com/6788579/254074593-31fcd816-7a3f-445d-82e9-fc2c8d4d873c.png">
+
+--------
+
 ### Multi-layer highlighting in the same stack:
 
 <img width="536" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207925754-4d4ffce5-be6c-44b6-b614-ae0e800a93d8.png">
 
 
 ### More examples:
```

### Comparing `pdbp-1.4.2/src/pdbp.py` & `pdbp-1.4.3/src/pdbp.py`

 * *Files 0% similar despite different names*

```diff
@@ -706,15 +706,15 @@
                 height_counter -= 1
                 if height_counter <= 0:
                     break
         if self.config.truncate_long_lines:
             maxlength = max(width - 9, 16)
             lines = [set_line_width(line, maxlength) for line in lines]
         else:
-            maxlength = max(map(len, lines))
+            maxlength = max(map(get_width, lines))
         if self.config.highlight:
             # Fill line with spaces. This is important when a bg color is
             # is used for highlighting the current line (via setbgcolor).
             tll = self.config.truncate_long_lines
             lines = [set_line_width(line, maxlength, tll) for line in lines]
             src = self.format_source("\n".join(lines))
             lines = src.splitlines()
```

