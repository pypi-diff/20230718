# Comparing `tmp/flict-1.0.9.tar.gz` & `tmp/flict-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flict-1.0.9.tar", last modified: Mon Dec  5 08:30:34 2022, max compression
+gzip compressed data, was "flict-1.1.0.tar", last modified: Tue Jul 18 06:26:57 2023, max compression
```

## Comparing `flict-1.0.9.tar` & `flict-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.854724 flict-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-05 08:30:10.000000 flict-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-05 08:30:10.000000 flict-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2022-12-05 08:30:34.854724 flict-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2022-12-05 08:30:10.000000 flict-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.850724 flict-1.0.9/flict/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-05 08:30:10.000000 flict-1.0.9/flict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2022-12-05 08:30:10.000000 flict-1.0.9/flict/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.850724 flict-1.0.9/flict/flictlib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2022-12-05 08:30:34.000000 flict-1.0.9/flict/flictlib/flict_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.854724 flict-1.0.9/flict/flictlib/format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/dot_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/json_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/markdown_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/text_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/lic_comp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/license_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.854724 flict-1.0.9/flict/flictlib/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/project/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2022-12-05 08:30:10.000000 flict-1.0.9/flict/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.854724 flict-1.0.9/flict/var/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-05 08:30:10.000000 flict-1.0.9/flict/var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2022-12-05 08:30:10.000000 flict-1.0.9/flict/var/alias.json
--rw-r--r--   0 runner    (1001) docker     (123)   457966 2022-12-05 08:30:10.000000 flict-1.0.9/flict/var/scancode-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.850724 flict-1.0.9/flict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2022-12-05 08:30:10.000000 flict-1.0.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-05 08:30:10.000000 flict-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-05 08:30:34.854724 flict-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2022-12-05 08:30:10.000000 flict-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 06:26:33.000000 flict-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 06:26:33.000000 flict-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-18 06:26:57.326307 flict-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-18 06:26:33.000000 flict-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 06:26:33.000000 flict-1.1.0/flict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-07-18 06:26:33.000000 flict-1.1.0/flict/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/flictlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-18 06:26:57.000000 flict-1.1.0/flict/flictlib/flict_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/flictlib/format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/dot_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/markdown_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/format/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/lic_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/license_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/flictlib/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/project/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-18 06:26:33.000000 flict-1.1.0/flict/flictlib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-18 06:26:33.000000 flict-1.1.0/flict/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict/var/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-18 06:26:33.000000 flict-1.1.0/flict/var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-18 06:26:33.000000 flict-1.1.0/flict/var/alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)   457966 2023-07-18 06:26:33.000000 flict-1.1.0/flict/var/scancode-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:26:57.326307 flict-1.1.0/flict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 06:26:57.000000 flict-1.1.0/flict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-18 06:26:33.000000 flict-1.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 06:26:33.000000 flict-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 06:26:57.330307 flict-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-18 06:26:33.000000 flict-1.1.0/setup.py
```

### Comparing `flict-1.0.9/LICENSE` & `flict-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/PKG-INFO` & `flict-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: flict
-Version: 1.0.9
+Version: 1.1.0
 Summary: FOSS License Compatibility Tool
 Home-page: https://github.com/vinland-technology/flict
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <!--
 SPDX-FileCopyrightText: 2022 Henrik Sandklef <hesa@sandklef.com>
 
@@ -48,29 +47,29 @@
 ***FOSS License Compatibility Tool*** (***flict***) is a Free and Open
 Source Software tool to verify license compatibility for a package and
 its dependencies. You can use the tool to automate license
 compatibility verification in your compliance work flow.
 
 flict can:
 
-* verify licenses compatibilty for license expression and a packages and its dependencies
+* verify licenses compatibility for license expression and a packages and its dependencies
 
 * suggest candidate outbound licenses
 
 * simplify license expressions
 
-* display, in misc format, compatibilies between licenses
+* display, in misc format, compatibilities between licenses
 
 * ~~check outbound licenses against a policy (policy as supplied by the user)~~ (automatic now)
 
 flict supports:
 
 * 87 licenses (```flict -of text list```)
 
-* common non SPDX ways to write licenses (e.g GPLv2 -> GPL-2.0-only), see "License alias defininitions" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
+* common non SPDX ways to write licenses (e.g GPLv2 -> GPL-2.0-only), see "License alias definitions" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
 
 * adding your own licenses (and compatibilities), see "Extending the license db" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
 
 * specifying licenses that are not allowed, see "Denied licenses" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
 
 * specifying license preference in case of a choice (e.g. "MIT OR FTL"), see "Preferred licenses" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
```

### Comparing `flict-1.0.9/README.md` & `flict-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 ***FOSS License Compatibility Tool*** (***flict***) is a Free and Open
 Source Software tool to verify license compatibility for a package and
 its dependencies. You can use the tool to automate license
 compatibility verification in your compliance work flow.
 
 flict can:
 
-* verify licenses compatibilty for license expression and a packages and its dependencies
+* verify licenses compatibility for license expression and a packages and its dependencies
 
 * suggest candidate outbound licenses
 
 * simplify license expressions
 
-* display, in misc format, compatibilies between licenses
+* display, in misc format, compatibilities between licenses
 
 * ~~check outbound licenses against a policy (policy as supplied by the user)~~ (automatic now)
 
 flict supports:
 
 * 87 licenses (```flict -of text list```)
 
-* common non SPDX ways to write licenses (e.g GPLv2 -> GPL-2.0-only), see "License alias defininitions" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
+* common non SPDX ways to write licenses (e.g GPLv2 -> GPL-2.0-only), see "License alias definitions" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
 
 * adding your own licenses (and compatibilities), see "Extending the license db" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
 
 * specifying licenses that are not allowed, see "Denied licenses" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
 
 * specifying license preference in case of a choice (e.g. "MIT OR FTL"), see "Preferred licenses" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
```

### Comparing `flict-1.0.9/flict/__main__.py` & `flict-1.1.0/flict/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,15 @@
                            dest='list_translation',
                            action='store_true',
                            help='List translation information')
 
     merge_parser = subparsers.add_parser('merge', help="Merge additional licenses with OSADL's matrix. Will output to store in a file, for use with --license-matrix-file")
     merge_parser.set_defaults(which="merge", func=_merge_licenses)
     merge_parser.add_argument('--license-file', '-lf', type=str, dest='license_file', help='License file (JSON) to merge', default=None)
+    merge_parser.add_argument('--default-no', '-dn', action='store_true', dest='default_no', help='If no compatibility can be found in the additional matrix, "No" compatibility is assumed. Works only for JSON input matrix', default=False)
 
     # display-compatibility
     parser_d = subparsers.add_parser(
         'display-compatibility', help='display license compatibility graphically')
     parser_d.set_defaults(which="display-compatibility",
                           func=display_compatibility)
     parser_d.add_argument('license_expression', type=str, nargs='+',
```

### Comparing `flict-1.0.9/flict/flictlib/alias.py` & `flict-1.1.0/flict/flictlib/alias.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/arbiter.py` & `flict-1.1.0/flict/flictlib/arbiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,16 +205,16 @@
         """
         return self.license_compatibility.inbound_outbound_compatibility(outbound, inbound)
 
     def check_compatibilities(self, licenses, check_all=False):
         """Check compatbilitiy between supplied licenses"""
         return self.license_compatibility.check_compatibilities(licenses, check_all)
 
-    def extend_license_db(self, file_name):
-        return self.license_compatibility.extend_license_db(file_name)
+    def extend_license_db(self, file_name, oformat="JSON", default_no=False):
+        return self.license_compatibility.extend_license_db(file_name, oformat, default_no)
 
     def simplify_license(self, expr):
         return self.license_compatibility.simplify_license(expr)
 
     def parse_license(self, expr):
         return self.license_compatibility.parse_license(expr)
```

### Comparing `flict-1.0.9/flict/flictlib/flict_config.py` & `flict-1.1.0/flict/flictlib/flict_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 ###################################################################
 
 import json
 import os
 
-from osadl_matrix import OSADL_MATRIX
+from osadl_matrix import OSADL_MATRIX_JSON
 
 
 def read_user_config():
     for path in [
         os.environ.get('FLICT_USERCONFIG'),
-        os.path.join(os.environ.get('HOME'), '.flict.cfg'),
+        os.path.join(os.environ.get('HOME', '/does/not/exist'), '.flict.cfg'),
     ]:
         try:
             with open(path) as i:
                 return json.load(i)
         except Exception:  # noqa: S110 - it's okay ignore all errors here
             pass
     return {}
 
 
 _userconfig = read_user_config()
 
-flict_version = "1.0.9"
+flict_version = "1.1.0"
 
 SCRIPT_DIR = os.path.realpath(os.path.join(os.path.dirname(os.path.realpath(__file__)), "../"))
 
 VAR_DIR = os.path.join(SCRIPT_DIR, "var")
 
 BUILTIN_ALIAS_FILE = os.path.join(VAR_DIR, "alias.json")
 DEFAULT_FLICT_ALIAS_FILE = os.path.join(VAR_DIR, BUILTIN_ALIAS_FILE)
 
-DEFAULT_MATRIX_FILE = _userconfig.get('matrix-file', OSADL_MATRIX)
+DEFAULT_MATRIX_FILE = _userconfig.get('matrix-file', OSADL_MATRIX_JSON)
 DEFAULT_OUTPUT_FORMAT = _userconfig.get('output-format', "JSON")
```

### Comparing `flict-1.0.9/flict/flictlib/format/common.py` & `flict-1.1.0/flict/flictlib/format/common.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/format/dot_format.py` & `flict-1.1.0/flict/flictlib/format/dot_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/format/factory.py` & `flict-1.1.0/flict/flictlib/format/factory.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/format/format.py` & `flict-1.1.0/flict/flictlib/format/format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/format/json_format.py` & `flict-1.1.0/flict/flictlib/format/json_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/format/markdown_format.py` & `flict-1.1.0/flict/flictlib/format/markdown_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/format/text_format.py` & `flict-1.1.0/flict/flictlib/format/text_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/lic_comp.py` & `flict-1.1.0/flict/flictlib/lic_comp.py`

 * *Files 14% similar despite different names*

```diff
@@ -73,59 +73,83 @@
                         "outbound": {
                             "type": "license",
                             "name": "X11"
                         },
                         "outbound_aliased": "X11",
                         "allowed": true,
                         "compatibility": "Yes"  <--- compatiblity status for outbound X11 and inbound MIT
+                        "problems": [] <----- list of causes such as "Check dependency, Unknown"
                     }
                 ],
                 "outbound": {
                     "type": "license",
                     "name": "X11"
                 },
                 "compatibility": "Yes",   <--- compatiblity status for outbound X11 and inbound 'MIT OR LGPL-2.1-only'.
                 "allowed": true,
                 "check": "inbounds_outbound"
+                "problems": [] <----- list of causes such as "Check dependency, Unknown"
             }
 
         """
         parsed_outbound = self.license.get_license([outbound])
 
         logging.debug(f"inbounds_outbound_check({outbound}, {expr})")
         parsed = self.license.get_license(expr)
         logging.debug(f"inbounds_outbound_check: parsed:{parsed}")
 
         return self._inbounds_outbound_check(parsed_outbound, parsed)
 
+    def __internal_expr_to_str(self, expr):
+        if self.license.is_license(expr):
+            return expr['name']
+        elif self.license.is_operator(expr):
+            raise FlictError(ReturnCodes.RET_INTERNAL_ERROR,
+                             f'Internal error. Cannot transform {expr} to a license expression')
+
     def _inbounds_outbound_check_operator(self, outbound, expr):
         compat_summary = None
         allowed_summary = None
+        problem_summary = []
         op = self.license.operator(expr)
         operands = self.license.operands(expr)
         for operand in operands:
+            problems = []
             logging.debug(f"Check operand: {operand}")
 
             # get compatibility_tag between the operand and the outbound
             # and calculate and store the summarized compatibility
             compat = self._inbounds_outbound_check(outbound, operand)
-            compat_summary = self._update_compat(op, compat_summary, compat[COMPATIBILITY_TAG] == CompatibilityStatus.LICENSE_COMPATIBILITY_COMPATIBLE.value)
+            compat_tag = compat[COMPATIBILITY_TAG]
+            if compat_tag == "Yes" or compat_tag == "No":
+                compat_summary = self._update_compat(op, compat_summary, compat_tag == CompatibilityStatus.LICENSE_COMPATIBILITY_COMPATIBLE.value)
+            elif compat_tag == "Unknown":
+                problems.append(f'Unknown license compatibility between outbound \'{outbound["name"]}\' and {self.__internal_expr_to_str(operand)}')
+                compat_summary = self._update_compat(op, compat_summary, compat_tag == CompatibilityStatus.LICENSE_COMPATIBILITY_COMPATIBLE.value)
+            elif compat_tag.startswith("Check"):
+                problems.append(f'Manually check license compatibility between {outbound}')
+                compat_summary = self._update_compat(op, compat_summary, compat_tag == CompatibilityStatus.LICENSE_COMPATIBILITY_COMPATIBLE.value)
+            elif compat_tag == "Undefined":
+                raise FlictError(ReturnCodes.RET_INVALID_EXPRESSSION,
+                                 'Undefined license')
 
             # are licenses allowed or denied for this expression
             allowed = compat['allowed']
             allowed_summary = self._update_allowed(op, allowed_summary, allowed)
             operand['allowed'] = allowed
             operand[COMPATIBILITY_TAG] = compat[COMPATIBILITY_TAG]
+            operand["problems"] = problems
+            problem_summary.append(problems)
 
         # store outbound to make for easier reading of result
         expr['outbound'] = outbound
         expr[COMPATIBILITY_TAG] = compat_summary
-
         expr["allowed"] = allowed_summary
         expr['check'] = 'inbounds_outbound'
+        expr["problems"] = problem_summary
 
         return expr
 
     def _inbounds_outbound_check_license(self, outbound, expr):
         license_expr = self.license.license_name(expr)
 
         outbound_aliased = self.license.replace_aliases(self.license.license_name(outbound))
@@ -134,14 +158,15 @@
         compat = self.compatibility.check_compat(outbound_aliased, license_aliased)
 
         expr['license_aliased'] = license_aliased
         expr['check'] = 'inbounds_outbound'
         expr['outbound'] = outbound
         expr['outbound_aliased'] = outbound_aliased
         expr['allowed'] = self.license.license_allowed(license_expr)
+        expr['problems'] = []
 
         expr[COMPATIBILITY_TAG] = compat[COMPATIBILITY_TAG]
         return expr
 
     def _inbounds_outbound_check(self, outbound, expr):
         logging.debug(f"_inbounds_outbound_check({outbound}, {expr})")
         if self.license.is_license(expr):
@@ -149,15 +174,14 @@
         elif self.license.is_operator(expr):
             return self._inbounds_outbound_check_operator(outbound, expr)
         else:
             raise FlictError(ReturnCodes.RET_INTERNAL_ERROR,
                              f"Could not parse one of the expression: {outbound}, {expr}")
 
     def _update_compat(self, op, current, new):
-
         if current is None:
             updated = new
         elif op == LICENSE_COMPATIBILITY_AND:
             updated = current == CompatibilityStatus.LICENSE_COMPATIBILITY_COMPATIBLE.value and new
         elif op == LICENSE_COMPATIBILITY_OR:
             updated = current == CompatibilityStatus.LICENSE_COMPATIBILITY_COMPATIBLE.value or new
 
@@ -184,16 +208,16 @@
 
     def replace_aliases(self, expr):
         return self.alias.replace_aliases(expr)
 
     def check_compatibilities(self, licenses, check_all=False):
         return self.compatibility.check_compatibilities(licenses, check_all)
 
-    def extend_license_db(self, file_name):
-        return self.compatibility.extend_license_db(file_name)
+    def extend_license_db(self, file_name, oformat="JSON", default_no=False):
+        return self.compatibility.extend_license_db(file_name, oformat, default_no)
 
     def simplify_license(self, expr):
         return self.license.simplify_license(expr)
 
     def get_license(self, expr):
         return self.license.get_license(expr)
```

### Comparing `flict-1.0.9/flict/flictlib/license.py` & `flict-1.1.0/flict/flictlib/license.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/license_parser.py` & `flict-1.1.0/flict/flictlib/license_parser.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/logger.py` & `flict-1.1.0/flict/flictlib/logger.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/project/reader.py` & `flict-1.1.0/flict/flictlib/project/reader.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/flictlib/return_codes.py` & `flict-1.1.0/flict/flictlib/return_codes.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     # 9
 
     RET_INVALID_PROJECT = (10, "Invalid project")
     RET_INVALID_EXPRESSSION = (11, "Invalid expression")
     RET_FILE_NOT_FOUND = (12, "File not found")
     RET_INVALID_ALIAS_FILE = (13, "Invalid alias file")
     RET_INVALID_LICENSE_PREFERENCE = (13, "Invalid license preferences")
+    RET_INVALID_MATRIX = (14, "Invalid matrix or matrix extension")
 
     @classmethod
     def get_help(cls, indent="  "):
         """
         Return help string for all defined enum values
         """
         ret = []
```

### Comparing `flict-1.0.9/flict/flictlib/utils.py` & `flict-1.1.0/flict/flictlib/utils.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/impl.py` & `flict-1.1.0/flict/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ###################################################################
 #
 # flict - FOSS License Compatibility Tool
 #
 # SPDX-FileCopyrightText: 2021 Jens Erdmann
-# SPDX-FileCopyrightText: 2022 Henrik Sandklef
+# SPDX-FileCopyrightText: 2023 Henrik Sandklef
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 ###################################################################
 
 
 from flict.flictlib.return_codes import FlictError, ReturnCodes
@@ -23,15 +23,15 @@
 
     def __init__(self, args) -> None:
         self._args = args
         self.arbiter = self._get_arbiter()
         self._formatter = FormatterFactory.formatter(args.output_format)
 
     def merge_license_db(self):
-        return self.arbiter.extend_license_db(self._args.license_file)
+        return self.arbiter.extend_license_db(self._args.license_file, oformat=self._args.output_format, default_no=self._args.default_no)
 
     def display_compatibility(self):
         inter_compats = self.arbiter.check_compatibilities(self._args.license_expression)
         return self._formatter.format_compats(inter_compats)
 
     def simplify(self):
         simplified = self.arbiter.simplify_license(" ".join(self._args.license_expression))
@@ -42,24 +42,26 @@
             licenses = self.arbiter.supported_licenses()
         else:
             licenses = self.arbiter.licenses(" ".join(self._args.license_expression))
         outbounds = []
         try:
             for outbound in licenses:
                 compats = self.arbiter.inbounds_outbound_check(outbound, self._args.license_expression)
-                compatible = (compats['compatibility'] == "Yes")
-                if compatible:
+                compat_status = compats['compatibility']
+                if compat_status == "Yes":
                     outbounds.append(outbound)
+                elif compat_status == "No":
+                    pass
 
             outbounds.sort()
             return self._formatter.format_outbound_license(outbounds)
 
-        except BaseException:
+        except Exception as e:
             raise FlictError(ReturnCodes.RET_INVALID_EXPRESSSION,
-                             f'Invalid license expression: {self._args.license_expression}')
+                             f'Invalid license expression: {self._args.license_expression}. Original cause: {e}')
 
     def list_licenses(self):
         licenses = list(self.arbiter.supported_licenses())
         licenses.sort(key=str.lower)
         return self._formatter.format_support_licenses(licenses)
 
     def _handle_lico_project(self, reader, project_file, formatter):
```

### Comparing `flict-1.0.9/flict/var/alias.json` & `flict-1.1.0/flict/var/alias.json`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict/var/scancode-licenses.json` & `flict-1.1.0/flict/var/scancode-licenses.json`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict.egg-info/PKG-INFO` & `flict-1.1.0/flict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: flict
-Version: 1.0.9
+Version: 1.1.0
 Summary: FOSS License Compatibility Tool
 Home-page: https://github.com/vinland-technology/flict
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <!--
 SPDX-FileCopyrightText: 2022 Henrik Sandklef <hesa@sandklef.com>
 
@@ -48,29 +47,29 @@
 ***FOSS License Compatibility Tool*** (***flict***) is a Free and Open
 Source Software tool to verify license compatibility for a package and
 its dependencies. You can use the tool to automate license
 compatibility verification in your compliance work flow.
 
 flict can:
 
-* verify licenses compatibilty for license expression and a packages and its dependencies
+* verify licenses compatibility for license expression and a packages and its dependencies
 
 * suggest candidate outbound licenses
 
 * simplify license expressions
 
-* display, in misc format, compatibilies between licenses
+* display, in misc format, compatibilities between licenses
 
 * ~~check outbound licenses against a policy (policy as supplied by the user)~~ (automatic now)
 
 flict supports:
 
 * 87 licenses (```flict -of text list```)
 
-* common non SPDX ways to write licenses (e.g GPLv2 -> GPL-2.0-only), see "License alias defininitions" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
+* common non SPDX ways to write licenses (e.g GPLv2 -> GPL-2.0-only), see "License alias definitions" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
 
 * adding your own licenses (and compatibilities), see "Extending the license db" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
 
 * specifying licenses that are not allowed, see "Denied licenses" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
 
 * specifying license preference in case of a choice (e.g. "MIT OR FTL"), see "Preferred licenses" in [SETTINGS](https://github.com/vinland-technology/flict/blob/main/SETTINGS.md)
```

### Comparing `flict-1.0.9/flict.egg-info/SOURCES.txt` & `flict-1.1.0/flict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flict-1.0.9/flict.egg-info/requires.txt` & `flict-1.1.0/flict.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-license-expression~=30.0
-osadl-matrix==2022.12.2.81206
-wheel~=0.38
+license-expression~=30.1
+osadl-matrix==2023.6.23.30625
+wheel~=0.40
 
 [dev]
 bump2version~=1.0
 dataclasses~=0.6
-dlint~=0.13
-flake8-2020~=1.7
+dlint~=0.14
+flake8-2020~=1.8
 flake8-bandit~=4.1
-flake8-broken-line~=0.6
-flake8-bugbear~=22.10
-flake8-builtins~=2.0
+flake8-broken-line~=1.0
+flake8-bugbear~=23.7
+flake8-builtins~=2.1
 flake8-coding~=1.3
 flake8-commas~=2.1
-flake8-comprehensions~=3.10
+flake8-comprehensions~=3.14
 flake8-debugger~=4.1
-flake8-docstrings~=1.6
-flake8-eradicate~=1.4
+flake8-docstrings~=1.7
+flake8-eradicate~=1.5
 flake8-executable~=2.1
 flake8-fixme~=1.1
-flake8-functions==0.0.7
-flake8-isort==5.0.3
+flake8-functions==0.0.8
+flake8-isort==6.0.0
 flake8-logging-format==0.9.0
 flake8-mutable~=1.2
 flake8-pep3101~=2.0
 flake8-print~=5.0
 flake8-quotes~=3.3
 flake8-requirements~=1.7
 flake8-string-format~=0.3
-flake8-variables-names==0.0.5
-flake8~=5.0
+flake8-variables-names==0.0.6
+flake8~=6.0
 pytest-bandit~=0.6
-pytest-cov~=4.0
-pytest-forked~=1.4
+pytest-cov~=4.1
+pytest-forked~=1.6
 pytest-icdiff~=0.6
 pytest-random-order~=1.1
-pytest-socket~=0.5
+pytest-socket~=0.6
 pytest-sugar~=0.9
 pytest-tldr~=0.2
-pytest~=7.2
+pytest~=7.4
 reuse~=1.1
 twine~=4.0
```

### Comparing `flict-1.0.9/requirements-dev.txt` & `flict-1.1.0/requirements-dev.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 bump2version ~= 1.0
 dataclasses ~= 0.6
-dlint ~= 0.13
-flake8 ~= 5.0
-flake8-2020 ~= 1.7
+dlint ~= 0.14
+flake8 ~= 6.0
+flake8-2020 ~= 1.8
 flake8-bandit ~= 4.1
-flake8-broken-line ~= 0.6
-flake8-bugbear ~= 22.10
-flake8-builtins ~= 2.0
+flake8-broken-line ~= 1.0
+flake8-bugbear ~= 23.7
+flake8-builtins ~= 2.1
 flake8-coding ~= 1.3
 flake8-commas ~= 2.1
-flake8-comprehensions ~= 3.10
+flake8-comprehensions ~= 3.14
 flake8-debugger ~= 4.1
-flake8-docstrings ~= 1.6
-flake8-eradicate ~= 1.4
+flake8-docstrings ~= 1.7
+flake8-eradicate ~= 1.5
 flake8-executable ~= 2.1
 flake8-fixme ~= 1.1
-flake8-functions == 0.0.7
-flake8-isort == 5.0.3
+flake8-functions == 0.0.8
+flake8-isort == 6.0.0
 flake8-logging-format == 0.9.0
 flake8-mutable ~= 1.2
 flake8-pep3101 ~= 2.0
 flake8-print ~= 5.0
 flake8-quotes ~= 3.3
 flake8-requirements ~= 1.7
 flake8-string-format ~= 0.3
-flake8-variables-names == 0.0.5
-pytest ~= 7.2
+flake8-variables-names == 0.0.6
+pytest ~= 7.4
 pytest-bandit ~= 0.6
-pytest-cov ~= 4.0
-pytest-forked ~= 1.4
+pytest-cov ~= 4.1
+pytest-forked ~= 1.6
 pytest-icdiff ~= 0.6
 pytest-random-order ~= 1.1
-pytest-socket ~= 0.5
+pytest-socket ~= 0.6
 pytest-sugar ~= 0.9
 pytest-tldr ~= 0.2
 twine ~= 4.0
 reuse ~= 1.1
```

### Comparing `flict-1.0.9/setup.py` & `flict-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,17 +44,16 @@
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Legal Industry",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Quality Assurance",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
 )
```

