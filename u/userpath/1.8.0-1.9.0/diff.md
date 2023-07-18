# Comparing `tmp/userpath-1.8.0.tar.gz` & `tmp/userpath-1.9.0.tar.gz`

## Comparing `userpath-1.8.0.tar` & `userpath-1.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 userpath-1.8.0/.codecov.yml
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 userpath-1.8.0/.coveragerc
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 userpath-1.8.0/.gitattributes
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 userpath-1.8.0/.gitignore
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 userpath-1.8.0/HISTORY.rst
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 userpath-1.8.0/LICENSE.txt
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 userpath-1.8.0/README.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 userpath-1.8.0/pyproject.toml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 userpath-1.8.0/requirements-dev.txt
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 userpath-1.8.0/tox.ini
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 userpath-1.8.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 userpath-1.8.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 userpath-1.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/conftest.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/test_bash.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/test_fish.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/test_sh.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/test_windows.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/test_xonsh.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/test_zsh.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/utils.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/coverage/.gitignore
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/docker/debian
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/docker/docker-compose.yaml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 userpath-1.8.0/tests/docker/requirements.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 userpath-1.8.0/userpath/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 userpath-1.8.0/userpath/__main__.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 userpath-1.8.0/userpath/cli.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 userpath-1.8.0/userpath/core.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 userpath-1.8.0/userpath/interface.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 userpath-1.8.0/userpath/shells.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 userpath-1.8.0/userpath/utils.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 userpath-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 userpath-1.9.0/.codecov.yml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 userpath-1.9.0/.coveragerc
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 userpath-1.9.0/.gitattributes
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 userpath-1.9.0/HISTORY.rst
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 userpath-1.9.0/requirements-dev.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 userpath-1.9.0/tox.ini
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 userpath-1.9.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 userpath-1.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 userpath-1.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/test_bash.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/test_fish.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/test_sh.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/test_windows.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/test_xonsh.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/test_zsh.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/utils.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/coverage/.gitignore
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/docker/debian
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/docker/docker-compose.yaml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 userpath-1.9.0/tests/docker/requirements.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 userpath-1.9.0/userpath/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 userpath-1.9.0/userpath/__main__.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 userpath-1.9.0/userpath/cli.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 userpath-1.9.0/userpath/core.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 userpath-1.9.0/userpath/interface.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 userpath-1.9.0/userpath/shells.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 userpath-1.9.0/userpath/utils.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 userpath-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 userpath-1.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 userpath-1.9.0/README.md
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 userpath-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 userpath-1.9.0/PKG-INFO
```

### Comparing `userpath-1.8.0/HISTORY.rst` & `userpath-1.9.0/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 History
 -------
 
 master
 ^^^^^^
 
+1.9.0
+^^^^^
+
+- Ignore the current directory for path detection on Windows
+- On non-Windows systems only modify login shells
+
 1.8.0
 ^^^^^
 
 - Broadcast WM_SETTINGCHANGE on Windows
+- zsh: respect ZDOTDIR env var
 - Drop Python 2.7 & 3.6
 
 1.7.0
 ^^^^^
 
 - Fix path normalization to be aware of case-insensitive platforms and symlinks.
```

### Comparing `userpath-1.8.0/LICENSE.txt` & `userpath-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/README.md` & `userpath-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/pyproject.toml` & `userpath-1.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "click",
 ]
 dynamic = ["version"]
```

### Comparing `userpath-1.8.0/tox.ini` & `userpath-1.9.0/tox.ini`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/.github/workflows/build.yml` & `userpath-1.9.0/.github/workflows/build.yml`

 * *Files 16% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 
 jobs:
   build:
     name: Build wheels and source distribution
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Install build dependencies
       run: python -m pip install --upgrade build
 
     - name: Build
       run: python -m build
 
-    - uses: actions/upload-artifact@v2
+    - uses: actions/upload-artifact@v3
       with:
         name: artifacts
         path: dist/*
         if-no-files-found: error
 
   publish:
     name: Publish release
     needs:
     - build
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/download-artifact@v2
+    - uses: actions/download-artifact@v3
       with:
         name: artifacts
         path: dist
 
     - name: Push build artifacts to PyPI
-      uses: pypa/gh-action-pypi-publish@v1.4.2
+      uses: pypa/gh-action-pypi-publish@v1.8.8
       with:
-        skip_existing: true
+        skip-existing: true
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `userpath-1.8.0/.github/workflows/test.yml` & `userpath-1.9.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,24 @@
   run:
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest]
-        python-version: ['3.7']
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     env:
       PYTHON_VERSION: ${{ matrix.python-version }}
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install test dependencies
       run: pip install --upgrade tox
 
     - name: Run tests
```

### Comparing `userpath-1.8.0/tests/conftest.py` & `userpath-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/tests/test_bash.py` & `userpath-1.9.0/tests/test_bash.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/tests/test_fish.py` & `userpath-1.9.0/tests/test_fish.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/tests/test_sh.py` & `userpath-1.9.0/tests/test_sh.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/tests/test_windows.py` & `userpath-1.9.0/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/tests/test_xonsh.py` & `userpath-1.9.0/tests/test_xonsh.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/tests/test_zsh.py` & `userpath-1.9.0/tests/test_zsh.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/userpath/cli.py` & `userpath-1.9.0/userpath/cli.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/userpath/core.py` & `userpath-1.9.0/userpath/core.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/userpath/interface.py` & `userpath-1.9.0/userpath/interface.py`

 * *Files identical despite different names*

### Comparing `userpath-1.8.0/userpath/shells.py` & `userpath-1.9.0/userpath/shells.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,35 +26,31 @@
 
 class Bash(Shell):
     def config(self, location, front=True):
         head, tail = (location, '$PATH') if front else ('$PATH', location)
         new_path = '{}{}{}'.format(head, pathsep, tail)
         contents = 'export PATH="{}"'.format(new_path)
 
-        configs = {path.join(self.home, '.bashrc'): contents}
-
         # https://github.com/ofek/userpath/issues/3#issuecomment-492491977
         profile_path = path.join(self.home, '.profile')
         bash_profile_path = path.join(self.home, '.bash_profile')
 
         if path.exists(profile_path) and not path.exists(bash_profile_path):
             login_config = profile_path
         else:
             # NOTE: If it is decided in future that we want to make a distinction between
             # login and non-login shells, be aware that macOS will still need this since
             # Terminal.app runs a login shell by default for each new terminal window.
             login_config = bash_profile_path
 
-        configs[login_config] = contents
-
-        return configs
+        return {login_config: contents}
 
     @classmethod
     def show_path_commands(cls):
-        return [['bash', '-i', '-c', 'echo $PATH'], ['bash', '-i', '-l', '-c', 'echo $PATH']]
+        return [['bash', '-i', '-l', '-c', 'echo $PATH']]
 
 
 class Fish(Shell):
     def config(self, location, front=True):
         location = ' '.join(location.split(pathsep))
         head, tail = (location, '$PATH') if front else ('$PATH', location)
 
@@ -91,19 +87,20 @@
 class Zsh(Shell):
     def config(self, location, front=True):
         head, tail = (location, '$PATH') if front else ('$PATH', location)
         new_path = '{}{}{}'.format(head, pathsep, tail)
         contents = 'export PATH="{}"'.format(new_path)
 
         zdotdir = environ.get('ZDOTDIR', self.home)
-        return {path.join(zdotdir, '.zshrc'): contents, path.join(zdotdir, '.zprofile'): contents}
+
+        return {path.join(zdotdir, '.zprofile'): contents}
 
     @classmethod
     def show_path_commands(cls):
-        return [['zsh', '-i', '-c', 'echo $PATH'], ['zsh', '-i', '-l', '-c', 'echo $PATH']]
+        return [['zsh', '-i', '-l', '-c', 'echo $PATH']]
 
 
 SHELLS = {
     'bash': Bash,
     'fish': Fish,
     'sh': Sh,
     'xonsh': Xonsh,
```

### Comparing `userpath-1.8.0/userpath/utils.py` & `userpath-1.9.0/userpath/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     if isinstance(location, (list, tuple)):
         return os.pathsep.join(normpath(l) for l in location)
 
     return os.path.normcase(os.path.realpath(os.path.expanduser(location.strip(';:'))))
 
 
 def location_in_path(location, path):
-    return normpath(location) in (normpath(p) for p in path.split(os.pathsep))
+    return normpath(location) in (normpath(p) for p in path.split(os.pathsep) if p != '')
 
 
 def in_current_path(location):
     return location_in_path(location, os.environ.get('PATH', ''))
 
 
 def ensure_parent_dir_exists(path):
```

### Comparing `userpath-1.8.0/PKG-INFO` & `userpath-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: userpath
-Version: 1.8.0
+Version: 1.9.0
 Summary: Cross-platform tool for adding locations to the user PATH
 Project-URL: Funding, https://github.com/sponsors/ofek
 Project-URL: History, https://github.com/ofek/userpath/blob/master/HISTORY.rst
 Project-URL: Issues, https://github.com/ofek/userpath/issues
 Project-URL: Source, https://github.com/ofek/userpath
 Author-email: Ofek Lev <oss@ofek.dev>
+License-Expression: MIT
+License-File: LICENSE.txt
 Keywords: path,user path
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: click
 Description-Content-Type: text/markdown
 
 # userpath
```

