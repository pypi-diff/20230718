# Comparing `tmp/tox-pyenv-redux-0.1.0.tar.gz` & `tmp/tox_pyenv_redux-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-pyenv-redux-0.1.0.tar", max compression
+gzip compressed data, was "tox_pyenv_redux-0.1.1.tar", max compression
```

## Comparing `tox-pyenv-redux-0.1.0.tar` & `tox_pyenv_redux-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1087 2022-01-13 12:18:26.969928 tox-pyenv-redux-0.1.0/LICENSE
--rw-r--r--   0        0        0      154 2022-04-03 12:17:54.796401 tox-pyenv-redux-0.1.0/README.md
--rw-r--r--   0        0        0     1479 2022-04-03 12:04:55.040315 tox-pyenv-redux-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-04-03 12:02:27.590039 tox-pyenv-redux-0.1.0/src/_tox_pyenv_redux/__init__.py
--rw-r--r--   0        0        0      453 2022-04-03 11:52:50.889053 tox-pyenv-redux-0.1.0/src/_tox_pyenv_redux/plugin.py
--rw-r--r--   0        0        0     1009 2022-04-03 12:22:47.965489 tox-pyenv-redux-0.1.0/setup.py
--rw-r--r--   0        0        0     1154 2022-04-03 12:22:47.965626 tox-pyenv-redux-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-07-18 10:10:12.399676 tox_pyenv_redux-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1383 2023-07-17 11:41:57.164472 tox_pyenv_redux-0.1.1/README.md
+-rw-r--r--   0        0        0     1078 2023-07-18 10:09:49.427308 tox_pyenv_redux-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-18 10:10:34.196026 tox_pyenv_redux-0.1.1/src/_tox_pyenv_redux/__init__.py
+-rw-r--r--   0        0        0      453 2022-04-03 11:52:50.889053 tox_pyenv_redux-0.1.1/src/_tox_pyenv_redux/plugin.py
+-rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 tox_pyenv_redux-0.1.1/PKG-INFO
```

### Comparing `tox-pyenv-redux-0.1.0/LICENSE` & `tox_pyenv_redux-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021 un.def <me@undef.im>
+Copyright (c) 2022, 2023 un.def <me@undef.im>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tox-pyenv-redux-0.1.0/PKG-INFO` & `tox_pyenv_redux-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,64 @@
 Metadata-Version: 2.1
 Name: tox-pyenv-redux
-Version: 0.1.0
-Summary: A tox plugin using pyenv to find Python executables
+Version: 0.1.1
+Summary: A tox Python discovery plugin for pyenv-installed interpreters
 Home-page: https://github.com/un-def/tox-pyenv-redux
 License: MIT
 Keywords: tox,pyenv
 Author: un.def
 Author-email: me@undef.im
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Dist: pyenv-inspect (>=0.2,<0.3)
-Requires-Dist: tox
+Requires-Dist: tox (<4)
 Project-URL: Repository, https://github.com/un-def/tox-pyenv-redux
 Description-Content-Type: text/markdown
 
 # tox-pyenv-redux
 
-A [tox][tox] plugin using [pyenv][pyenv] to find Python executables
+A [tox][tox] Python discovery plugin for [pyenv][pyenv]–installed interpreters
+
+**IMPORTANT**: this plugin is only compatible with legacy versions of tox (0.x—3.x). Starting with tox version 4, the Python discovery job is delegated to [virtualenv][virtualenv] ([docs][tox-docs-discovery-migration]).
+
+## Migration to tox 4
+
+1. Uninstall tox-pyenv-redux
+2. Install [virtualenv-pyenv][virtualenv-pyenv]
+3. Set the virtualenv discovery mechanism to `pyenv` using one of the following methods:
+    * the environment variable in a shell (e.g., in `.bashrc`, `.zshenv`, `.envrc`, `.env`):
+      ```shell
+      export VIRTUALENV_DISCOVERY=pyenv
+      ```
+    * the environment variable in [a tox config][tox-docs-config]:
+      ```ini
+      [testenv]
+      set_env =
+        VIRTUALENV_DISCOVERY = pyenv
+      ```
+    * the option in [a virtualenv config][virtualenv-docs-config]:
+      ```ini
+      [virtualenv]
+      discovery = pyenv
+      ```
 
 
 [tox]: https://tox.wiki/
 [pyenv]: https://github.com/pyenv/pyenv
+[virtualenv]: https://virtualenv.pypa.io/
+[virtualenv-pyenv]: https://github.com/un-def/virtualenv-pyenv
+[tox-docs-discovery-migration]: https://tox.wiki/en/latest/plugins.html#tox-get-python-executable
+[tox-docs-config]: https://tox.wiki/en/latest/config.html
+[virtualenv-docs-config]: https://virtualenv.pypa.io/en/latest/cli_interface.html#conf-file
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

