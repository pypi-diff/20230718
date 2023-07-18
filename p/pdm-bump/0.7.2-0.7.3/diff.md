# Comparing `tmp/pdm_bump-0.7.2.tar.gz` & `tmp/pdm_bump-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_bump-0.7.2.tar", last modified: Mon Jul 17 18:36:28 2023, max compression
+gzip compressed data, was "pdm_bump-0.7.3.tar", last modified: Tue Jul 18 19:38:01 2023, max compression
```

## Comparing `pdm_bump-0.7.2.tar` & `pdm_bump-0.7.3.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1092 2023-07-17 18:35:12.758294 pdm_bump-0.7.2/LICENSE
--rw-r--r--   0        0        0     2397 2023-07-17 18:35:12.758294 pdm_bump-0.7.2/README.md
--rw-r--r--   0        0        0     6003 2023-07-17 18:36:28.603353 pdm_bump-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      869 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/__init__.py
--rw-r--r--   0        0        0      542 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/__init__.py
--rw-r--r--   0        0        0     8508 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/base.py
--rw-r--r--   0        0        0     1954 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/explicit.py
--rw-r--r--   0        0        0     9966 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/increment.py
--rw-r--r--   0        0        0     8897 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/preview.py
--rw-r--r--   0        0        0     1558 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/actions/vcs.py
--rw-r--r--   0        0        0     1378 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/cli.py
--rw-r--r--   0        0        0      259 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/__init__.py
--rw-r--r--   0        0        0     9461 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/config.py
--rw-r--r--   0        0        0     2293 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/loader.py
--rw-r--r--   0        0        0     7404 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/logging.py
--rw-r--r--   0        0        0     7593 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/core/version.py
--rw-r--r--   0        0        0     6596 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/dynamic.py
--rw-r--r--   0        0        0     6668 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/plugin.py
--rw-r--r--   0        0        0        0 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/py.typed
--rw-r--r--   0        0        0     2402 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/source.py
--rw-r--r--   0        0        0      792 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/vcs/__init__.py
--rw-r--r--   0        0        0     9907 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/vcs/core.py
--rw-r--r--   0        0        0     1103 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/vcs/git.py
--rw-r--r--   0        0        0     7356 2023-07-17 18:35:12.762294 pdm_bump-0.7.2/src/pdm_bump/vcs/gitcli.py
--rw-r--r--   0        0        0     4906 2023-07-17 18:35:12.766294 pdm_bump-0.7.2/src/pdm_bump/vcs/mixins.py
--rw-r--r--   0        0        0    25464 2023-07-17 18:35:12.766294 pdm_bump-0.7.2/tests/action_test.py
--rw-r--r--   0        0        0     3743 2023-07-17 18:35:12.766294 pdm_bump-0.7.2/tests/plugin_test.py
--rw-r--r--   0        0        0    24207 2023-07-17 18:35:12.766294 pdm_bump-0.7.2/tests/version_test.py
--rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 pdm_bump-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-18 19:37:07.256097 pdm_bump-0.7.3/LICENSE
+-rw-r--r--   0        0        0     2397 2023-07-18 19:37:07.256097 pdm_bump-0.7.3/README.md
+-rw-r--r--   0        0        0     6003 2023-07-18 19:38:01.051993 pdm_bump-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      869 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/__init__.py
+-rw-r--r--   0        0        0      531 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/__init__.py
+-rw-r--r--   0        0        0     8508 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/base.py
+-rw-r--r--   0        0        0     1954 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/explicit.py
+-rw-r--r--   0        0        0     9966 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/increment.py
+-rw-r--r--   0        0        0     8897 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/preview.py
+-rw-r--r--   0        0        0     1558 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/actions/vcs.py
+-rw-r--r--   0        0        0     1378 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/cli.py
+-rw-r--r--   0        0        0      259 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/core/__init__.py
+-rw-r--r--   0        0        0     9461 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/core/config.py
+-rw-r--r--   0        0        0     7404 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/core/logging.py
+-rw-r--r--   0        0        0     7593 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/core/version.py
+-rw-r--r--   0        0        0     6596 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/dynamic.py
+-rw-r--r--   0        0        0     6668 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/py.typed
+-rw-r--r--   0        0        0     2402 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/source.py
+-rw-r--r--   0        0        0      699 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/__init__.py
+-rw-r--r--   0        0        0     9907 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/core.py
+-rw-r--r--   0        0        0     1103 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/git.py
+-rw-r--r--   0        0        0     7356 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/gitcli.py
+-rw-r--r--   0        0        0     4906 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/src/pdm_bump/vcs/mixins.py
+-rw-r--r--   0        0        0    25464 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/tests/action_test.py
+-rw-r--r--   0        0        0     3743 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/tests/plugin_test.py
+-rw-r--r--   0        0        0    24207 2023-07-18 19:37:07.260097 pdm_bump-0.7.3/tests/version_test.py
+-rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 pdm_bump-0.7.3/PKG-INFO
```

### Comparing `pdm_bump-0.7.2/LICENSE` & `pdm_bump-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/README.md` & `pdm_bump-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/pyproject.toml` & `pdm_bump-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-bump"
-version = "0.7.2"
+version = "0.7.3"
 readme = "README.md"
 description = "A plugin for PDM providing the ability to modify the version according to PEP440"
 authors = [
     { name = "Carsten Igel", email = "cig@bite-that-bit.de" },
 ]
 dependencies = [
     "pdm>=2.00",
```

### Comparing `pdm_bump-0.7.2/src/pdm_bump/__init__.py` & `pdm_bump-0.7.3/src/pdm_bump/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/actions/base.py` & `pdm_bump-0.7.3/src/pdm_bump/actions/base.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/actions/explicit.py` & `pdm_bump-0.7.3/src/pdm_bump/actions/explicit.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/actions/increment.py` & `pdm_bump-0.7.3/src/pdm_bump/actions/increment.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/actions/preview.py` & `pdm_bump-0.7.3/src/pdm_bump/actions/preview.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/actions/vcs.py` & `pdm_bump-0.7.3/src/pdm_bump/actions/vcs.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/cli.py` & `pdm_bump-0.7.3/src/pdm_bump/cli.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/core/config.py` & `pdm_bump-0.7.3/src/pdm_bump/core/config.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/core/logging.py` & `pdm_bump-0.7.3/src/pdm_bump/core/logging.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/core/version.py` & `pdm_bump-0.7.3/src/pdm_bump/core/version.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/dynamic.py` & `pdm_bump-0.7.3/src/pdm_bump/dynamic.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/plugin.py` & `pdm_bump-0.7.3/src/pdm_bump/plugin.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/source.py` & `pdm_bump-0.7.3/src/pdm_bump/source.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/vcs/__init__.py` & `pdm_bump-0.7.3/src/pdm_bump/vcs/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,30 +9,26 @@
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
 """"""
 
 
-from ..core.loader import loader as _loader
+# Justification: load module for decoupling
+from . import gitcli  # noqa: F401
 from .core import (
     DefaultVcsProvider,
     VcsProvider,
     VcsProviderAggregator,
     VcsProviderFactory,
     VcsProviderRegistry,
     vcs_provider,
     vcs_providers,
 )
 
-# Justification: Add items to registry
-_loader.load_modules_of_package(
-    __file__, __name__, "__init__", "core", "mixins"
-)
-
 __all__ = (
     "vcs_provider",
     "vcs_providers",
     "VcsProvider",
     "VcsProviderAggregator",
     "VcsProviderFactory",
     "VcsProviderRegistry",
```

### Comparing `pdm_bump-0.7.2/src/pdm_bump/vcs/core.py` & `pdm_bump-0.7.3/src/pdm_bump/vcs/core.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/vcs/git.py` & `pdm_bump-0.7.3/src/pdm_bump/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/vcs/gitcli.py` & `pdm_bump-0.7.3/src/pdm_bump/vcs/gitcli.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/src/pdm_bump/vcs/mixins.py` & `pdm_bump-0.7.3/src/pdm_bump/vcs/mixins.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/tests/action_test.py` & `pdm_bump-0.7.3/tests/action_test.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/tests/plugin_test.py` & `pdm_bump-0.7.3/tests/plugin_test.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/tests/version_test.py` & `pdm_bump-0.7.3/tests/version_test.py`

 * *Files identical despite different names*

### Comparing `pdm_bump-0.7.2/PKG-INFO` & `pdm_bump-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-bump
-Version: 0.7.2
+Version: 0.7.3
 Summary: A plugin for PDM providing the ability to modify the version according to PEP440
 Home-page: https://github.com/carstencodes/pdm-bump
 Author-Email: Carsten Igel <cig@bite-that-bit.de>
 License: MIT
 Project-URL: Homepage, https://github.com/carstencodes/pdm-bump
 Requires-Python: >=3.9
 Requires-Dist: pdm>=2.00
```

