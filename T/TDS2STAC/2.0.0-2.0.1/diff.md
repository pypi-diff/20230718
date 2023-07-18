# Comparing `tmp/TDS2STAC-2.0.0.tar.gz` & `tmp/TDS2STAC-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDS2STAC-2.0.0.tar", last modified: Thu Jul  6 11:09:45 2023, max compression
+gzip compressed data, was "TDS2STAC-2.0.1.tar", last modified: Tue Jul 18 18:36:27 2023, max compression
```

## Comparing `TDS2STAC-2.0.0.tar` & `TDS2STAC-2.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.340764 TDS2STAC-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     3603 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)    13807 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      389 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10810 2023-07-06 11:09:45.340764 TDS2STAC-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9403 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.338764 TDS2STAC-2.0.0/TDS2STAC.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10810 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      624 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      326 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 11:09:45.000000 TDS2STAC-2.0.0/TDS2STAC.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.338764 TDS2STAC-2.0.0/docs/
--rw-r--r--   0 root         (0) root         (0)      609 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/authors.rst
--rwxr-xr-x   0 root         (0) root         (0)     4870 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/history.rst
--rw-r--r--   0 root         (0) root         (0)      296 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1174 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      806 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/readme.rst
--rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/docs/usage.rst
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)     1896 2023-07-06 11:09:45.341764 TDS2STAC-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      296 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.341764 TDS2STAC-2.0.0/tds2stac/
--rw-r--r--   0 root         (0) root         (0)       99 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-07-06 11:09:45.341764 TDS2STAC-2.0.0/tds2stac/_version.py
--rw-r--r--   0 root         (0) root         (0)    54920 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/app.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/cli.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/constants.py
--rw-r--r--   0 root         (0) root         (0)     7868 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/core.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tds2stac/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:09:45.340764 TDS2STAC-2.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1808 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/tests/test_tds2stac.py
--rw-r--r--   0 root         (0) root         (0)    84134 2023-07-06 11:08:20.000000 TDS2STAC-2.0.0/versioneer.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-18 18:36:27.499801 TDS2STAC-2.0.1/
+-rw-r--r--   0 hadizadeh-m (15144)      901      168 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/AUTHORS.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     3603 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901    13807 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/LICENSE
+-rw-r--r--   0 hadizadeh-m (15144)      901      389 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/MANIFEST.in
+-rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-18 18:36:27.499904 TDS2STAC-2.0.1/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901     9403 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/README.rst
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-18 18:36:27.497104 TDS2STAC-2.0.1/TDS2STAC.egg-info/
+-rw-r--r--   0 hadizadeh-m (15144)      901    10810 2023-07-18 18:36:27.000000 TDS2STAC-2.0.1/TDS2STAC.egg-info/PKG-INFO
+-rw-r--r--   0 hadizadeh-m (15144)      901      624 2023-07-18 18:36:27.000000 TDS2STAC-2.0.1/TDS2STAC.egg-info/SOURCES.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        1 2023-07-18 18:36:27.000000 TDS2STAC-2.0.1/TDS2STAC.egg-info/dependency_links.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901      553 2023-07-18 18:36:27.000000 TDS2STAC-2.0.1/TDS2STAC.egg-info/requires.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901        9 2023-07-18 18:36:27.000000 TDS2STAC-2.0.1/TDS2STAC.egg-info/top_level.txt
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-18 18:36:27.498261 TDS2STAC-2.0.1/docs/
+-rw-r--r--   0 hadizadeh-m (15144)      901      609 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/Makefile
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/authors.rst
+-rwxr-xr-x   0 hadizadeh-m (15144)      901     4870 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/conf.py
+-rw-r--r--   0 hadizadeh-m (15144)      901       33 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/contributing.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       28 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/history.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      296 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/index.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901     1174 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/installation.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      806 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/make.bat
+-rw-r--r--   0 hadizadeh-m (15144)      901       27 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/readme.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901       71 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/docs/usage.rst
+-rw-r--r--   0 hadizadeh-m (15144)      901      181 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/pyproject.toml
+-rw-r--r--   0 hadizadeh-m (15144)      901      226 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/requirements_dev.txt
+-rw-r--r--   0 hadizadeh-m (15144)      901     1896 2023-07-18 18:36:27.501004 TDS2STAC-2.0.1/setup.cfg
+-rw-r--r--   0 hadizadeh-m (15144)      901      427 2023-07-18 18:33:02.000000 TDS2STAC-2.0.1/setup.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-18 18:36:27.501311 TDS2STAC-2.0.1/tds2stac/
+-rw-r--r--   0 hadizadeh-m (15144)      901       99 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/tds2stac/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901      497 2023-07-18 18:36:27.501347 TDS2STAC-2.0.1/tds2stac/_version.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    54920 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/tds2stac/app.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     2579 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/tds2stac/cli.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     3286 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/tds2stac/constants.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     7868 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/tds2stac/core.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     3696 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/tds2stac/utils.py
+drwxr-xr-x   0 hadizadeh-m (15144)      901        0 2023-07-18 18:36:27.499670 TDS2STAC-2.0.1/tests/
+-rw-r--r--   0 hadizadeh-m (15144)      901       38 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/tests/__init__.py
+-rw-r--r--   0 hadizadeh-m (15144)      901     1808 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/tests/test_tds2stac.py
+-rw-r--r--   0 hadizadeh-m (15144)      901    84134 2023-07-18 18:29:50.000000 TDS2STAC-2.0.1/versioneer.py
```

### Comparing `TDS2STAC-2.0.0/CONTRIBUTING.rst` & `TDS2STAC-2.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/LICENSE` & `TDS2STAC-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/PKG-INFO` & `TDS2STAC-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDS2STAC
-Version: 2.0.0
+Version: 2.0.1
 Summary: A STAC catalog creator from Thredds data server
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://tds2stac.readthedocs.io/
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
```

### Comparing `TDS2STAC-2.0.0/README.rst` & `TDS2STAC-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/TDS2STAC.egg-info/PKG-INFO` & `TDS2STAC-2.0.1/TDS2STAC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDS2STAC
-Version: 2.0.0
+Version: 2.0.1
 Summary: A STAC catalog creator from Thredds data server
 Home-page: https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
 Author: Mostafa Hadizadeh
 Author-email: mostafa.hadizadeh@kit.edu
 License: EUPL-1.2
 Project-URL: Documentation, https://tds2stac.readthedocs.io/
 Project-URL: Source, https://codebase.helmholtz.cloud/CAT4KIT/tds2stac
```

### Comparing `TDS2STAC-2.0.0/TDS2STAC.egg-info/SOURCES.txt` & `TDS2STAC-2.0.1/TDS2STAC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/docs/Makefile` & `TDS2STAC-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/docs/conf.py` & `TDS2STAC-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/docs/installation.rst` & `TDS2STAC-2.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/docs/make.bat` & `TDS2STAC-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/setup.cfg` & `TDS2STAC-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 	autodocsumm
 	sphinxcontrib-django
 
 [mypy]
 ignore_missing_imports = True
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = tds2stac/_version.py
 versionfile_build = tds2stac/_version.py
 tag_prefix = 
 parentdir_prefix = 
 
 [bdist_wheel]
```

### Comparing `TDS2STAC-2.0.0/tds2stac/app.py` & `TDS2STAC-2.0.1/tds2stac/app.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/tds2stac/cli.py` & `TDS2STAC-2.0.1/tds2stac/cli.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/tds2stac/constants.py` & `TDS2STAC-2.0.1/tds2stac/constants.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/tds2stac/core.py` & `TDS2STAC-2.0.1/tds2stac/core.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/tds2stac/utils.py` & `TDS2STAC-2.0.1/tds2stac/utils.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/tests/test_tds2stac.py` & `TDS2STAC-2.0.1/tests/test_tds2stac.py`

 * *Files identical despite different names*

### Comparing `TDS2STAC-2.0.0/versioneer.py` & `TDS2STAC-2.0.1/versioneer.py`

 * *Files identical despite different names*

