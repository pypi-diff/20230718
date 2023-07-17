# Comparing `tmp/hpsspy-0.6.1.tar.gz` & `tmp/hpsspy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpsspy-0.6.1.tar", last modified: Fri May 20 21:04:58 2022, max compression
+gzip compressed data, was "hpsspy-0.7.0.tar", last modified: Mon Jul 17 22:53:20 2023, max compression
```

## Comparing `hpsspy-0.6.1.tar` & `hpsspy-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 benjamin.weaver   (502) staff       (20)        0 2022-05-20 21:04:58.422763 hpsspy-0.6.1/
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     1529 2022-05-20 19:25:59.000000 hpsspy-0.6.1/LICENSE.rst
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)       57 2022-05-20 19:25:59.000000 hpsspy-0.6.1/MANIFEST.in
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     2555 2022-05-20 21:04:58.423004 hpsspy-0.6.1/PKG-INFO
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     1801 2022-05-20 20:59:32.000000 hpsspy-0.6.1/README.rst
-drwxr-xr-x   0 benjamin.weaver   (502) staff       (20)        0 2022-05-20 21:04:58.413123 hpsspy-0.6.1/doc/
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     6762 2022-05-04 21:57:07.000000 hpsspy-0.6.1/doc/Makefile
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)      261 2022-05-04 21:57:07.000000 hpsspy-0.6.1/doc/api.rst
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     2302 2022-05-20 21:04:42.000000 hpsspy-0.6.1/doc/changes.rst
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     9327 2022-05-20 19:25:59.000000 hpsspy-0.6.1/doc/conf.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)    10076 2022-05-20 19:25:59.000000 hpsspy-0.6.1/doc/configuration.rst
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     1288 2022-05-20 19:25:59.000000 hpsspy-0.6.1/doc/index.rst
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     4032 2022-05-04 21:57:07.000000 hpsspy-0.6.1/doc/using.rst
-drwxr-xr-x   0 benjamin.weaver   (502) staff       (20)        0 2022-05-20 21:04:58.414027 hpsspy-0.6.1/hpsspy/
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)      362 2022-05-20 21:04:42.000000 hpsspy-0.6.1/hpsspy/__init__.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     1711 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/conftest.py
-drwxr-xr-x   0 benjamin.weaver   (502) staff       (20)        0 2022-05-20 21:04:58.416535 hpsspy-0.6.1/hpsspy/data/
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)      813 2022-05-04 21:57:07.000000 hpsspy-0.6.1/hpsspy/data/desi.json
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)    20552 2022-05-04 21:57:07.000000 hpsspy-0.6.1/hpsspy/data/sdss.json
-drwxr-xr-x   0 benjamin.weaver   (502) staff       (20)        0 2022-05-20 21:04:58.417715 hpsspy-0.6.1/hpsspy/os/
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)      195 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/os/__init__.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     7679 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/os/_os.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     1155 2022-05-06 21:29:35.000000 hpsspy-0.6.1/hpsspy/os/path.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)    27173 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/scan.py
-drwxr-xr-x   0 benjamin.weaver   (502) staff       (20)        0 2022-05-20 21:04:58.419959 hpsspy-0.6.1/hpsspy/test/
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)      172 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/test/__init__.py
-drwxr-xr-x   0 benjamin.weaver   (502) staff       (20)        0 2022-05-20 21:04:58.422355 hpsspy-0.6.1/hpsspy/test/t/
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)       32 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/test/t/hpss_cache.csv
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)       24 2022-05-04 21:57:07.000000 hpsspy-0.6.1/hpsspy/test/t/invalid_file
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)      219 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/test/t/missing_cache.json
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     1358 2022-05-04 21:57:07.000000 hpsspy-0.6.1/hpsspy/test/t/test_scan.json
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     1217 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/test/test_data.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)    12117 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/test/test_os.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)    16162 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/test/test_scan.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)      446 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/test/test_top_level.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     8546 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/test/test_util.py
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)    10244 2022-05-20 19:25:59.000000 hpsspy-0.6.1/hpsspy/util.py
-drwxr-xr-x   0 benjamin.weaver   (502) staff       (20)        0 2022-05-20 21:04:58.415862 hpsspy-0.6.1/hpsspy.egg-info/
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     2555 2022-05-20 21:04:57.000000 hpsspy-0.6.1/hpsspy.egg-info/PKG-INFO
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)      817 2022-05-20 21:04:58.000000 hpsspy-0.6.1/hpsspy.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)        1 2022-05-20 21:04:57.000000 hpsspy-0.6.1/hpsspy.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)       55 2022-05-20 21:04:57.000000 hpsspy-0.6.1/hpsspy.egg-info/entry_points.txt
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)       55 2022-05-20 21:04:57.000000 hpsspy-0.6.1/hpsspy.egg-info/requires.txt
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)        7 2022-05-20 21:04:58.000000 hpsspy-0.6.1/hpsspy.egg-info/top_level.txt
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)        1 2022-05-20 21:04:57.000000 hpsspy-0.6.1/hpsspy.egg-info/zip-safe
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)      102 2022-05-20 19:25:59.000000 hpsspy-0.6.1/pyproject.toml
--rw-r--r--   0 benjamin.weaver   (502) staff       (20)     1606 2022-05-20 21:04:58.424061 hpsspy-0.6.1/setup.cfg
--rwxr-xr-x   0 benjamin.weaver   (502) staff       (20)     1196 2022-05-20 19:25:59.000000 hpsspy-0.6.1/setup.py
+drwxr-xr-x   0 weaver     (501) staff       (20)        0 2023-07-17 22:53:20.457075 hpsspy-0.7.0/
+-rw-r--r--   0 weaver     (501) staff       (20)     1529 2023-07-17 22:06:20.000000 hpsspy-0.7.0/LICENSE.rst
+-rw-r--r--   0 weaver     (501) staff       (20)       57 2022-05-21 01:23:05.000000 hpsspy-0.7.0/MANIFEST.in
+-rw-r--r--   0 weaver     (501) staff       (20)     2520 2023-07-17 22:53:20.457406 hpsspy-0.7.0/PKG-INFO
+-rw-r--r--   0 weaver     (501) staff       (20)     1766 2023-07-17 22:06:20.000000 hpsspy-0.7.0/README.rst
+drwxr-xr-x   0 weaver     (501) staff       (20)        0 2023-07-17 22:53:20.444796 hpsspy-0.7.0/doc/
+-rw-r--r--   0 weaver     (501) staff       (20)     6762 2015-02-03 20:49:03.000000 hpsspy-0.7.0/doc/Makefile
+-rw-r--r--   0 weaver     (501) staff       (20)      261 2017-01-18 00:27:11.000000 hpsspy-0.7.0/doc/api.rst
+-rw-r--r--   0 weaver     (501) staff       (20)     2719 2023-07-17 22:09:30.000000 hpsspy-0.7.0/doc/changes.rst
+-rw-r--r--   0 weaver     (501) staff       (20)     9662 2023-07-17 22:06:20.000000 hpsspy-0.7.0/doc/conf.py
+-rw-r--r--   0 weaver     (501) staff       (20)    10076 2022-05-21 01:23:05.000000 hpsspy-0.7.0/doc/configuration.rst
+-rw-r--r--   0 weaver     (501) staff       (20)     1253 2023-07-17 22:06:20.000000 hpsspy-0.7.0/doc/index.rst
+-rw-r--r--   0 weaver     (501) staff       (20)       55 2023-07-17 22:06:20.000000 hpsspy-0.7.0/doc/rtd-requirements.txt
+-rw-r--r--   0 weaver     (501) staff       (20)     4153 2023-07-17 22:06:20.000000 hpsspy-0.7.0/doc/using.rst
+drwxr-xr-x   0 weaver     (501) staff       (20)        0 2023-07-17 22:53:20.446624 hpsspy-0.7.0/hpsspy/
+-rw-r--r--   0 weaver     (501) staff       (20)      362 2023-07-17 22:06:20.000000 hpsspy-0.7.0/hpsspy/__init__.py
+-rw-r--r--   0 weaver     (501) staff       (20)     1711 2022-05-21 01:23:05.000000 hpsspy-0.7.0/hpsspy/conftest.py
+drwxr-xr-x   0 weaver     (501) staff       (20)        0 2023-07-17 22:53:20.449277 hpsspy-0.7.0/hpsspy/data/
+-rw-r--r--   0 weaver     (501) staff       (20)      813 2019-05-19 04:11:03.000000 hpsspy-0.7.0/hpsspy/data/desi.json
+-rw-r--r--   0 weaver     (501) staff       (20)    20552 2019-05-19 04:11:03.000000 hpsspy-0.7.0/hpsspy/data/sdss.json
+drwxr-xr-x   0 weaver     (501) staff       (20)        0 2023-07-17 22:53:20.450376 hpsspy-0.7.0/hpsspy/os/
+-rw-r--r--   0 weaver     (501) staff       (20)      195 2022-05-21 01:23:05.000000 hpsspy-0.7.0/hpsspy/os/__init__.py
+-rw-r--r--   0 weaver     (501) staff       (20)     7679 2022-05-21 01:23:05.000000 hpsspy-0.7.0/hpsspy/os/_os.py
+-rw-r--r--   0 weaver     (501) staff       (20)     1155 2019-05-16 02:40:23.000000 hpsspy-0.7.0/hpsspy/os/path.py
+-rw-r--r--   0 weaver     (501) staff       (20)    28811 2023-07-17 22:06:20.000000 hpsspy-0.7.0/hpsspy/scan.py
+drwxr-xr-x   0 weaver     (501) staff       (20)        0 2023-07-17 22:53:20.452836 hpsspy-0.7.0/hpsspy/test/
+-rw-r--r--   0 weaver     (501) staff       (20)      172 2022-05-21 01:23:05.000000 hpsspy-0.7.0/hpsspy/test/__init__.py
+drwxr-xr-x   0 weaver     (501) staff       (20)        0 2023-07-17 22:53:20.456602 hpsspy-0.7.0/hpsspy/test/t/
+-rw-r--r--   0 weaver     (501) staff       (20)       32 2022-05-21 01:23:05.000000 hpsspy-0.7.0/hpsspy/test/t/hpss_cache.csv
+-rw-r--r--   0 weaver     (501) staff       (20)       24 2019-01-29 23:01:40.000000 hpsspy-0.7.0/hpsspy/test/t/invalid_file
+-rw-r--r--   0 weaver     (501) staff       (20)     1047 2023-07-17 22:06:20.000000 hpsspy-0.7.0/hpsspy/test/t/missing_cache.json
+-rw-r--r--   0 weaver     (501) staff       (20)     1689 2023-07-17 22:06:20.000000 hpsspy-0.7.0/hpsspy/test/t/test_scan.json
+-rw-r--r--   0 weaver     (501) staff       (20)      505 2023-07-17 22:06:20.000000 hpsspy-0.7.0/hpsspy/test/t/test_scan_disk_cache.csv
+-rw-r--r--   0 weaver     (501) staff       (20)      110 2023-07-17 22:06:20.000000 hpsspy-0.7.0/hpsspy/test/t/test_scan_disk_cache_missing.csv
+-rw-r--r--   0 weaver     (501) staff       (20)       94 2023-07-17 22:06:20.000000 hpsspy-0.7.0/hpsspy/test/t/test_scan_disk_cache_multiple.csv
+-rw-r--r--   0 weaver     (501) staff       (20)     1217 2022-05-21 01:23:05.000000 hpsspy-0.7.0/hpsspy/test/test_data.py
+-rw-r--r--   0 weaver     (501) staff       (20)    12326 2023-07-17 22:06:20.000000 hpsspy-0.7.0/hpsspy/test/test_os.py
+-rw-r--r--   0 weaver     (501) staff       (20)    39614 2023-07-17 22:06:20.000000 hpsspy-0.7.0/hpsspy/test/test_scan.py
+-rw-r--r--   0 weaver     (501) staff       (20)      446 2022-05-21 01:23:05.000000 hpsspy-0.7.0/hpsspy/test/test_top_level.py
+-rw-r--r--   0 weaver     (501) staff       (20)     8546 2022-05-21 01:23:05.000000 hpsspy-0.7.0/hpsspy/test/test_util.py
+-rw-r--r--   0 weaver     (501) staff       (20)    10244 2022-05-21 01:23:05.000000 hpsspy-0.7.0/hpsspy/util.py
+drwxr-xr-x   0 weaver     (501) staff       (20)        0 2023-07-17 22:53:20.448719 hpsspy-0.7.0/hpsspy.egg-info/
+-rw-r--r--   0 weaver     (501) staff       (20)     2520 2023-07-17 22:53:20.000000 hpsspy-0.7.0/hpsspy.egg-info/PKG-INFO
+-rw-r--r--   0 weaver     (501) staff       (20)      976 2023-07-17 22:53:20.000000 hpsspy-0.7.0/hpsspy.egg-info/SOURCES.txt
+-rw-r--r--   0 weaver     (501) staff       (20)        1 2023-07-17 22:53:20.000000 hpsspy-0.7.0/hpsspy.egg-info/dependency_links.txt
+-rw-r--r--   0 weaver     (501) staff       (20)       55 2023-07-17 22:53:20.000000 hpsspy-0.7.0/hpsspy.egg-info/entry_points.txt
+-rw-r--r--   0 weaver     (501) staff       (20)       55 2023-07-17 22:53:20.000000 hpsspy-0.7.0/hpsspy.egg-info/requires.txt
+-rw-r--r--   0 weaver     (501) staff       (20)        7 2023-07-17 22:53:20.000000 hpsspy-0.7.0/hpsspy.egg-info/top_level.txt
+-rw-r--r--   0 weaver     (501) staff       (20)        1 2023-07-17 22:53:03.000000 hpsspy-0.7.0/hpsspy.egg-info/zip-safe
+-rw-r--r--   0 weaver     (501) staff       (20)      102 2023-07-17 22:50:11.000000 hpsspy-0.7.0/pyproject.toml
+-rw-r--r--   0 weaver     (501) staff       (20)     1564 2023-07-17 22:53:20.460447 hpsspy-0.7.0/setup.cfg
+-rwxr-xr-x   0 weaver     (501) staff       (20)     1196 2022-05-21 01:23:05.000000 hpsspy-0.7.0/setup.py
```

### Comparing `hpsspy-0.6.1/LICENSE.rst` & `hpsspy-0.7.0/LICENSE.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2014-2022, Benjamin Alan Weaver <benjamin.weaver@noirlab.edu>
+Copyright (c) 2014-2023, Benjamin Alan Weaver <benjamin.weaver@noirlab.edu>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `hpsspy-0.6.1/PKG-INFO` & `hpsspy-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpsspy
-Version: 0.6.1
+Version: 0.7.0
 Summary: Package for interacting with HPSS.
 Home-page: http://github.com/weaverba137/hpsspy
 Author: Benjamin Alan Weaver
 Author-email: benjamin.weaver@noirlab.edu
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -60,17 +60,17 @@
 .. _HPSS: https://www.nersc.gov/systems/hpss-data-archive/
 .. _NERSC: https://www.nersc.gov
 .. _GitHub: https://github.com/weaverba137/hpsspy
 
 Requirements
 ------------
 
-HPSSPy assumes that the HPSS utilities `hsi and htar`_ are installed.  You may
-need a NERSC account to download and install these utilities.
+HPSSPy assumes that the HPSS utilities `hsi and htar`_ are installed.  As of
+2023, these utilities are only available within the NERSC_ environment.
 
-.. _`hsi and htar`: https://www.nersc.gov/users/data-and-file-systems/hpss/storing-and-retrieving-data/software-downloads/
+.. _`hsi and htar`: https://docs.nersc.gov/filesystems/archive/#common-commands
 
 License
 -------
 
 HPSSPy is free software licensed under a 3-clause BSD-style license. For details see
 the ``LICENSE.rst`` file.
```

### Comparing `hpsspy-0.6.1/README.rst` & `hpsspy-0.7.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 .. _HPSS: https://www.nersc.gov/systems/hpss-data-archive/
 .. _NERSC: https://www.nersc.gov
 .. _GitHub: https://github.com/weaverba137/hpsspy
 
 Requirements
 ------------
 
-HPSSPy assumes that the HPSS utilities `hsi and htar`_ are installed.  You may
-need a NERSC account to download and install these utilities.
+HPSSPy assumes that the HPSS utilities `hsi and htar`_ are installed.  As of
+2023, these utilities are only available within the NERSC_ environment.
 
-.. _`hsi and htar`: https://www.nersc.gov/users/data-and-file-systems/hpss/storing-and-retrieving-data/software-downloads/
+.. _`hsi and htar`: https://docs.nersc.gov/filesystems/archive/#common-commands
 
 License
 -------
 
 HPSSPy is free software licensed under a 3-clause BSD-style license. For details see
 the ``LICENSE.rst`` file.
```

### Comparing `hpsspy-0.6.1/doc/Makefile` & `hpsspy-0.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/doc/changes.rst` & `hpsspy-0.7.0/doc/changes.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =============
 Release Notes
 =============
 
+0.7.0 (2023-07-17)
+------------------
+
+* :command:`missing_from_hpss` will proceed through all stages, even if
+  serious errors are detected, to facilitate batch processing. The older
+  behavior can be enabled with ``--exit-on-error`` (PR `#15`_).
+* Fix error handling for a variety of corner cases (PR `#15`_).
+* Increase test coverage to 100% (PR `#15`_).
+
+.. _`#15`: https://github.com/weaverba137/hpsspy/pull/15
+
 0.6.1 (2022-05-20)
 ------------------
 
 * Bumped version due to malformed PyPI upload.
 
 0.6.0 (2022-05-20)
 ------------------
```

### Comparing `hpsspy-0.6.1/doc/conf.py` & `hpsspy-0.7.0/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,24 @@
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 keep_warnings = False
 
 # Include functions that begin with an underscore, e.g. _private().
 napoleon_include_private_with_doc = True
 
+# This value contains a list of modules to be mocked up. This is useful when
+# some external dependencies are not met at build time and break the
+# building process.
+autodoc_mock_imports = []
+for missing in ('pytz', ):
+    try:
+        foo = import_module(missing)
+    except ImportError:
+        autodoc_mock_imports.append(missing)
+
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #html_theme = 'default'
 #html_theme = 'haiku'
 try:
```

### Comparing `hpsspy-0.6.1/doc/configuration.rst` & `hpsspy-0.7.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/doc/index.rst` & `hpsspy-0.7.0/doc/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 .. _HPSS: https://www.nersc.gov/systems/hpss-data-archive/
 .. _NERSC: https://www.nersc.gov
 .. _GitHub: https://github.com/weaverba137/hpsspy
 
 Requirements
 ++++++++++++
 
-HPSSPy assumes that the HPSS utilities `hsi and htar`_ are installed.  You may
-need a NERSC account to download and install these utilities.
+HPSSPy assumes that the HPSS utilities `hsi and htar`_ are installed.  As of
+2023, these utilities are only available within the NERSC_ environment.
 
-.. _`hsi and htar`: https://www.nersc.gov/users/data-and-file-systems/hpss/storing-and-retrieving-data/software-downloads/
+.. _`hsi and htar`: https://docs.nersc.gov/filesystems/archive/#common-commands
 
 HPSSPy expects these utilities to exist in the directory ``${HPSS_DIR}/bin``, so
 be sure the environment variable :envvar:`HPSS_DIR` is defined.
 
 Contents
 ++++++++
```

### Comparing `hpsspy-0.6.1/doc/using.rst` & `hpsspy-0.7.0/doc/using.rst`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,25 @@
     from sys import exit
     from hpsspy.scan import main
     exit(main())
 
 Options
 +++++++
 
-There are a lot of command-line options.  ``missing_from_hpss --help`` will
+There are several of command-line options.  ``missing_from_hpss --help`` will
 display all of them. Just the short versions of the commands are
 shown here.
 
 -c DIR      Cache files (described below) are written to
             ``$HOME/cache`` by default.  This option
             allows the user to choose any directory.
 -D          Delete and recreate the disk cache file
             (described below).
+-E          Exit if an error is detected while processing files
+            on disk or on HPSS.
 -H          Delete and recreate the HPSS cache file
             (described below).
 -l N        Limit archive files to this size in GB.
             The default is 1024 GB (1 TB).
 -p          Issue the HPSS commands necessary to actually
             back up the files found that need to be backed up.
 -r N        Issue a progress report on how many files
@@ -56,23 +58,23 @@
 :command:`missing_from_hpss` uses a few cache files primarily to reduce
 memory footprint.  These files will be stored in ``$HOME/cache``
 by default.  The files are:
 
 Disk Cache
     A CSV file of the form ``disk_cache_<section>.csv``, where ``<section>`` is
     the section (as defined above) specified on the command-line.  The
-    columns are file name and file size in bytes.
+    columns are file name, file size in bytes and modification time.
 
 HPSS Cache
-    A plain-text file of the form ``hpss_cache_<section>.txt``,
-    where ``<section>`` is the section (as defined above) specified on
-    the command-line.  This is simply a list of files found on HPSS.
+    A CSV file of the form ``hpss_cache_<section>.csv``, where ``<section>`` is
+    the section (as defined above) specified on the command-line.  The
+    columns are file name, file size in bytes and modification time.
 
 Missing File Cache
-    A JSON file of the form ``$HOME/cache/missing_files_<section>.json``,
+    A JSON file of the form ``missing_files_<section>.json``,
     where ``<section>`` is the section (as defined above) specified on the
     command-line. It contains a map of HPSS archive files to the files that
     belong in that archive.  In addition the size of the resulting files
     (modulo small overheads from the archive file creation process) will
     be saved to this file.
 
 These files are *not* cleaned up by default because they are very useful
```

### Comparing `hpsspy-0.6.1/hpsspy/conftest.py` & `hpsspy-0.7.0/hpsspy/conftest.py`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/hpsspy/data/desi.json` & `hpsspy-0.7.0/hpsspy/data/desi.json`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/hpsspy/data/sdss.json` & `hpsspy-0.7.0/hpsspy/data/sdss.json`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/hpsspy/os/_os.py` & `hpsspy-0.7.0/hpsspy/os/_os.py`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/hpsspy/os/path.py` & `hpsspy-0.7.0/hpsspy/os/path.py`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/hpsspy/scan.py` & `hpsspy-0.7.0/hpsspy/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,16 @@
     pattern_used = dict()
     section_warning = set()
     with open(disk_files_cache, newline='') as t:
         reader = csv.DictReader(t)
         for row in reader:
             f = row['Name']
             nfiles += 1
+            if (nfiles % report) == 0:
+                logger.info("%9d files scanned.", nfiles)
             if f in hpss_map["__exclude__"]:
                 logger.info("%s is excluded.", f)
                 continue
             section = f.split('/')[0]
             if section == f:
                 #
                 # Top-level section containing no subdirectories.
@@ -217,14 +219,16 @@
             #
             mapped = 0
             for r in s:
                 if r[0].pattern not in pattern_used:
                     pattern_used[r[0].pattern] = 0
                 m = r[0].match(f)
                 if m is not None:
+                    logger.debug("pattern_used[r'%s'] += 1", r[0].pattern)
+                    logger.debug("r[1] = r'%s'", r[1])
                     pattern_used[r[0].pattern] += 1
                     mapped += 1
                     if r[1] == "EXCLUDE":
                         logger.debug("%s is excluded from backups.", f)
                     elif r[1] == "AUTOMATED":
                         logger.debug("%s is backed up by some other " +
                                      "automated process.", f)
@@ -256,16 +260,14 @@
                                                'exists': exists}
             if mapped == 0:
                 logger.error("%s is not mapped to any file on HPSS!", f)
                 nmissing += 1
             if mapped > 1:
                 logger.error("%s is mapped to multiple files on HPSS!", f)
                 nmultiple += 1
-            if (nfiles % report) == 0:
-                logger.info("%9d files scanned.", nfiles)
     for p in pattern_used:
         if pattern_used[p] == 0:
             logger.info("Pattern '%s' was never used, " +
                         "maybe files have been removed from disk?", p)
     #
     # Eliminate backups that exist and have no newer files on disk.
     #
@@ -326,14 +328,15 @@
         if h.endswith('.tar'):
             disk_chdir = os.path.dirname(h)
             full_chdir = os.path.join(disk_root, disk_chdir)
             if h.endswith('_files.tar'):
                 Lfile = os.path.join(get_tmpdir(),
                                      os.path.basename(h.replace('.tar',
                                                                 '.txt')))
+                logger.debug(Lfile)
                 htar_dir = None
                 Lfile_lines = ('\n'.join([os.path.basename(f)
                                           for f in missing[h]['files']]) +
                                '\n')
                 if test:
                     logger.debug(Lfile_lines)
                 else:
@@ -356,15 +359,21 @@
                                 and htar_re.match(d) is not None]
                 else:
                     logger.error(("Could not find directories corresponding " +
                                   "to %s!"), h)
                     continue
             logger.debug("os.chdir('%s')", full_chdir)
             os.chdir(full_chdir)
-            h_dir = os.path.join(hpss_root, disk_chdir)
+            #
+            # Avoid adding a trailing slash.
+            #
+            if disk_chdir:
+                h_dir = os.path.join(hpss_root, disk_chdir)
+            else:
+                h_dir = hpss_root
             if h_dir not in created_directories:
                 logger.debug("makedirs('%s', mode='%s')", h_dir, dirmode)
                 if not test:
                     makedirs(h_dir, mode=dirmode)
                 created_directories.add(h_dir)
             if Lfile is None:
                 logger.info("htar('-cvf', '%s', '-H', " +
@@ -487,32 +496,41 @@
         logger.debug("Using existing file cache: %s", disk_files_cache)
         return True
     else:
         logger.info("No disk cache file, starting scan.")
         with open(disk_files_cache, 'w', newline='') as t:
             writer = csv.writer(t)
             writer.writerow(['Name', 'Size', 'Mtime'])
-            try:
-                for disk_root in disk_roots:
-                    logger.debug("Starting os.walk at %s.", disk_root)
+            for disk_root in disk_roots:
+                logger.debug("Starting os.walk at %s.", disk_root)
+                try:
                     for root, dirs, files in os.walk(disk_root):
                         logger.debug("Scanning disk directory %s.", root)
                         for f in files:
                             fullname = os.path.join(root, f)
                             if not os.path.islink(fullname):
                                 cachename = fullname.replace(disk_root+'/', '')
-                                s = os.stat(fullname)
-                                writer.writerow([cachename,
-                                                 s.st_size,
-                                                 int(s.st_mtime)])
-            except OSError as e:
-                logger.error('Exception encountered while creating ' +
-                             'disk cache file!')
-                logger.error(e.strerror)
-                return False
+                                try:
+                                    s = os.stat(fullname)
+                                except PermissionError as perr:
+                                    logger.error("%s: %s",
+                                                 perr.strerror, perr.filename)
+                                    continue
+                                try:
+                                    writer.writerow([cachename,
+                                                     s.st_size,
+                                                     int(s.st_mtime)])
+                                except UnicodeEncodeError as e:
+                                    logger.error("Could not write %s to cache file due to unusual characters!",
+                                                 fullname.encode(errors='surrogatepass'))
+                                    logger.error("Message was: %s.", str(e))
+                except OSError as oerr:
+                    logger.error('Exception encountered while traversing %s!', disk_root)
+                    logger.error(oerr.strerror)
+                    return False
     return True
 
 
 def scan_hpss(hpss_root, hpss_files_cache, overwrite=False):
     """Scan a directory on HPSS and return the files found there.
 
     Parameters
@@ -573,17 +591,33 @@
         return (release_root,)
     if not pd:
         return (release_root,)
     broot = os.path.basename(config['root'])
     if ((len(pd) == 1) and (pd[0] == broot)):
         return (release_root,)
     if pd[0].startswith('/'):
-        return tuple([os.path.join(d, os.path.basename(release_root))
-                      for d in pd])
-    return tuple([release_root.replace(broot, d) for d in pd])
+        roots = [os.path.join(d, os.path.basename(release_root))
+                 for d in pd]
+    else:
+        roots = [release_root.replace(broot, d) for d in pd]
+    #
+    # Is any root a pure symlink to another root?
+    #
+    remove = list()
+    for r in roots:
+        if os.path.islink(r):
+            rr = os.readlink(r)
+            if rr.startswith('.'):
+                rr = os.path.normpath(os.path.join(config['root'], rr))
+            if rr in roots:
+                remove.append(r)
+    rs = set(roots)
+    for r in remove:
+        rs.remove(r)
+    return tuple(rs)
 
 
 def _options():
     """Parse command-line options.
 
     Returns
     -------
@@ -596,14 +630,17 @@
                         metavar='DIR',
                         default=os.path.join(os.environ['HOME'], 'cache'),
                         help=('Write cache files to DIR (Default: ' +
                               '%(default)s).'))
     parser.add_argument('-D', '--overwrite-disk', action='store_true',
                         dest='overwrite_disk',
                         help='Ignore any existing disk cache files.')
+    parser.add_argument('-E', '--exit-on-error', action='store_true',
+                        dest='errexit',
+                        help='Exit if an error is detected in the file analysis stages.')
     parser.add_argument('-H', '--overwrite-hpss', action='store_true',
                         dest='overwrite_hpss',
                         help='Ignore any existing HPSS cache files.')
     parser.add_argument('-l', '--size-limit', action='store', type=float,
                         dest='limit', metavar='N', default=1024.0,
                         help=("Do not allow archive files larger than " +
                               "N GB (Default: %(default)s GB)."))
@@ -683,26 +720,26 @@
     disk_files_cache = os.path.join(options.cache,
                                     ('disk_files_' +
                                      '{0}.csv').format(options.release))
     logger.debug("disk_files_cache = '%s'", disk_files_cache)
     disk_roots = physical_disks(release_root, config)
     status = scan_disk(disk_roots, disk_files_cache,
                        overwrite=options.overwrite_disk)
-    if not status:
+    if options.errexit and not status:
         return 1
     #
     # See if the files are on HPSS.
     #
     missing_files_cache = os.path.join(options.cache,
                                        ('missing_files_' +
                                         '{0}.json').format(options.release))
     logger.debug("missing_files_cache = '%s'", missing_files_cache)
     status = find_missing(hpss_map, hpss_files, disk_files_cache,
                           missing_files_cache, options.report, options.limit)
-    if not status:
+    if options.errexit and not status:
         return 1
     #
     # Post process to generate HPSS commands
     #
     if options.process or options.test:
         process_missing(missing_files_cache, release_root, hpss_release_root,
                         test=options.test)
```

### Comparing `hpsspy-0.6.1/hpsspy/test/t/test_scan.json` & `hpsspy-0.7.0/hpsspy/test/t/test_scan.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9330018939393939%*

 * *Differences: {"'data'": "{'d1': {'d1/spectro/data/.*$': 'AUTOMATED'}, 'd2': "*

 * *           "{'d2/spectro/redux/([0-9a-zA-Z_-]+)/preproc/.*$': 'EXCLUDE', delete: "*

 * *           "['d2/spectro/redux/preproc/.*$']}, '__top__': OrderedDict([('[^/]+$', "*

 * *           "'data_files.tar')]), 'd4': OrderedDict(), 'd5': "*

 * *           "OrderedDict([('d5/spectro/redux/preproc/.*$', 'EXCLUDE'), "*

 * *           "('d5/spectro/redux/([0-9a-zA-Z_-]+)/[^/]+$', "*

 * *           "'d2/spectro/redux/\\\\1/\\\\1_files.tar')])}"}*

```diff
@@ -6,30 +6,39 @@
         ],
         "root": "/temporary"
     },
     "data": {
         "__exclude__": [
             "README.html"
         ],
+        "__top__": {
+            "[^/]+$": "data_files.tar"
+        },
         "d1": {
             "d1/([^/]+\\.txt)$": "d1/\\1",
             "d1/batch/.*$": "d1/batch.tar",
+            "d1/spectro/data/.*$": "AUTOMATED",
             "d1/templates/[^/]+$": "d1/templates/templates_files.tar"
         },
         "d2": {
             "d2/(batch|fiberassign)/.*$": "d2/d2_\\1.tar",
             "d2/[^/]+$": "d2/d2_files.tar",
             "d2/spectro/redux/([0-9a-zA-Z_-]+)/(calib2d|plan|run)/.*$": "d2/spectro/redux/\\1/\\1_\\2.tar",
             "d2/spectro/redux/([0-9a-zA-Z_-]+)/[^/]+$": "d2/spectro/redux/\\1/\\1_files.tar",
             "d2/spectro/redux/([0-9a-zA-Z_-]+)/exposures/([0-9]{8})/.*$": "d2/spectro/redux/\\1/exposures/\\1_exposures_\\2.tar",
+            "d2/spectro/redux/([0-9a-zA-Z_-]+)/preproc/.*$": "EXCLUDE",
             "d2/spectro/redux/([0-9a-zA-Z_-]+)/spectra-([0-9]+)/([0-9]+)/.*$": "d2/spectro/redux/\\1/spectra-\\2/\\1_spectra-\\2_\\3.tar",
-            "d2/spectro/redux/preproc/.*$": "EXCLUDE",
             "d2/spectro/sim/([0-9a-zA-Z_-]+)/([0-9]{8})/.*$": "d2/spectro/sim/\\1/sim_\\1_\\2.tar",
             "d2/targets/([0-9]+)/.*$": "d2/targets/d2_targets_\\1.tar",
             "d2/targets/[^/]+$": "d2/targets/d2_targets_files.tar"
+        },
+        "d4": {},
+        "d5": {
+            "d5/spectro/redux/([0-9a-zA-Z_-]+)/[^/]+$": "d2/spectro/redux/\\1/\\1_files.tar",
+            "d5/spectro/redux/preproc/.*$": "EXCLUDE"
         }
     },
     "redux": {
         "__exclude__": []
     },
     "www": {
         "__exclude__": []
```

### Comparing `hpsspy-0.6.1/hpsspy/test/test_data.py` & `hpsspy-0.7.0/hpsspy/test/test_data.py`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/hpsspy/test/test_os.py` & `hpsspy-0.7.0/hpsspy/test/test_os.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,22 @@
             self.raises = raises
             self.args = list()
             self.kwargs = list()
 
         def __call__(self, *args, **kwargs):
             self.args.append(tuple(args))
             self.kwargs.append(kwargs)
-            if self.raises:
-                raise self.raises
             r = self.return_values[self.counter]
+            if isinstance(self.raises, list):
+                if self.raises[self.counter] is not None:
+                    raise self.raises[self.counter]
+            elif self.raises is not None:
+                raise self.raises
+            else:
+                pass
             self.counter += 1
             return r
 
     return SaveArgs
 
 
 def test_chmod(monkeypatch, mock_call):
```

### Comparing `hpsspy-0.6.1/hpsspy/test/test_util.py` & `hpsspy-0.7.0/hpsspy/test/test_util.py`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/hpsspy/util.py` & `hpsspy-0.7.0/hpsspy/util.py`

 * *Files identical despite different names*

### Comparing `hpsspy-0.6.1/hpsspy.egg-info/PKG-INFO` & `hpsspy-0.7.0/hpsspy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpsspy
-Version: 0.6.1
+Version: 0.7.0
 Summary: Package for interacting with HPSS.
 Home-page: http://github.com/weaverba137/hpsspy
 Author: Benjamin Alan Weaver
 Author-email: benjamin.weaver@noirlab.edu
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -60,17 +60,17 @@
 .. _HPSS: https://www.nersc.gov/systems/hpss-data-archive/
 .. _NERSC: https://www.nersc.gov
 .. _GitHub: https://github.com/weaverba137/hpsspy
 
 Requirements
 ------------
 
-HPSSPy assumes that the HPSS utilities `hsi and htar`_ are installed.  You may
-need a NERSC account to download and install these utilities.
+HPSSPy assumes that the HPSS utilities `hsi and htar`_ are installed.  As of
+2023, these utilities are only available within the NERSC_ environment.
 
-.. _`hsi and htar`: https://www.nersc.gov/users/data-and-file-systems/hpss/storing-and-retrieving-data/software-downloads/
+.. _`hsi and htar`: https://docs.nersc.gov/filesystems/archive/#common-commands
 
 License
 -------
 
 HPSSPy is free software licensed under a 3-clause BSD-style license. For details see
 the ``LICENSE.rst`` file.
```

### Comparing `hpsspy-0.6.1/hpsspy.egg-info/SOURCES.txt` & `hpsspy-0.7.0/hpsspy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.py
 doc/Makefile
 doc/api.rst
 doc/changes.rst
 doc/conf.py
 doc/configuration.rst
 doc/index.rst
+doc/rtd-requirements.txt
 doc/using.rst
 hpsspy/__init__.py
 hpsspy/conftest.py
 hpsspy/scan.py
 hpsspy/util.py
 hpsspy.egg-info/PKG-INFO
 hpsspy.egg-info/SOURCES.txt
@@ -32,8 +33,11 @@
 hpsspy/test/test_os.py
 hpsspy/test/test_scan.py
 hpsspy/test/test_top_level.py
 hpsspy/test/test_util.py
 hpsspy/test/t/hpss_cache.csv
 hpsspy/test/t/invalid_file
 hpsspy/test/t/missing_cache.json
-hpsspy/test/t/test_scan.json
+hpsspy/test/t/test_scan.json
+hpsspy/test/t/test_scan_disk_cache.csv
+hpsspy/test/t/test_scan_disk_cache_missing.csv
+hpsspy/test/t/test_scan_disk_cache_multiple.csv
```

### Comparing `hpsspy-0.6.1/setup.cfg` & `hpsspy-0.7.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -47,18 +47,16 @@
 exclude = .github/*
 
 [coverage:run]
 relative_files = True
 source = 
 	hpsspy
 omit = 
-	hpsspy/_version.py
 	hpsspy/conftest.py
 	hpsspy/test/*
-	*/hpsspy/_version.py
 	*/hpsspy/conftest.py
 	*/hpsspy/test/*
 
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
 	except ImportError
```

### Comparing `hpsspy-0.6.1/setup.py` & `hpsspy-0.7.0/setup.py`

 * *Files identical despite different names*

