# Comparing `tmp/pdbplus-1.4.2.tar.gz` & `tmp/pdbplus-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbplus-1.4.2.tar", last modified: Thu Jun 29 21:50:09 2023, max compression
+gzip compressed data, was "pdbplus-1.4.3.tar", last modified: Mon Jul 17 22:28:50 2023, max compression
```

## Comparing `pdbplus-1.4.2.tar` & `pdbplus-1.4.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:50:09.367777 pdbplus-1.4.2/
--rw-r--r--   0 michael    (501) staff       (20)     7052 2023-06-29 21:50:09.367681 pdbplus-1.4.2/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     5099 2023-06-22 14:53:13.000000 pdbplus-1.4.2/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-29 21:50:09.367539 pdbplus-1.4.2/pdbplus.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     7052 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      172 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       12 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-29 21:50:09.000000 pdbplus-1.4.2/pdbplus.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-06-29 21:50:09.367808 pdbplus-1.4.2/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5032 2023-06-29 21:49:47.000000 pdbplus-1.4.2/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:28:50.990539 pdbplus-1.4.3/
+-rw-r--r--   0 michael    (501) staff       (20)     7195 2023-07-17 22:28:50.990428 pdbplus-1.4.3/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     5242 2023-07-17 22:14:22.000000 pdbplus-1.4.3/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:28:50.990275 pdbplus-1.4.3/pdbplus.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     7195 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      172 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       12 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-17 22:28:50.990575 pdbplus-1.4.3/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5607 2023-07-17 22:12:51.000000 pdbplus-1.4.3/setup.py
```

### Comparing `pdbplus-1.4.2/PKG-INFO` & `pdbplus-1.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.4.2
+Version: 1.4.3
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -47,15 +47,15 @@
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
+<img width="680" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
@@ -96,17 +96,16 @@
 
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
 
@@ -164,14 +163,20 @@
 
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

### Comparing `pdbplus-1.4.2/README.md` & `pdbplus-1.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
+<img width="680" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
@@ -50,17 +50,16 @@
 
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
 
@@ -118,14 +117,20 @@
 
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

### Comparing `pdbplus-1.4.2/pdbplus.egg-info/PKG-INFO` & `pdbplus-1.4.3/pdbplus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.4.2
+Version: 1.4.3
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -47,15 +47,15 @@
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="660" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
+<img width="680" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/247826485-d782911e-d817-4ea6-86dd-215991d7b8ea.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for [pdb](https://docs.python.org/3/library/pdb.html) and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
@@ -96,17 +96,16 @@
 
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
 
@@ -164,14 +163,20 @@
 
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

### Comparing `pdbplus-1.4.2/setup.py` & `pdbplus-1.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,35 +36,43 @@
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
-        os.system('python -m twine upload dist/*')  # Requires ~/.pypirc Keys
+        os.system("python -m twine upload dist/*")  # Requires ~/.pypirc Keys
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name='pdbplus',
-    version='1.4.2',
+    version='1.4.3',
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
         "Download": "https://pypi.org/project/pdbp/#files",
@@ -103,14 +111,14 @@
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
     python_requires=">=3.6",
     install_requires=[
-        'pdbp>=1.4.2',
+        'pdbp>=1.4.3',
     ],
     setup_requires=[],
     packages=[],
 )
 
 print("\n*** pdbplus Installation Complete! ***\n")
```

