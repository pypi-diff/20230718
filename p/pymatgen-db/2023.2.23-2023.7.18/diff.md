# Comparing `tmp/pymatgen-db-2023.2.23.tar.gz` & `tmp/pymatgen-db-2023.7.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-db-2023.2.23.tar", last modified: Thu Feb 23 20:06:20 2023, max compression
+gzip compressed data, was "pymatgen-db-2023.7.18.tar", last modified: Tue Jul 18 14:47:08 2023, max compression
```

## Comparing `pymatgen-db-2023.2.23.tar` & `pymatgen-db-2023.7.18.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-23 20:06:20.849121 pymatgen-db-2023.2.23/
--rw-r--r--   0 shyue      (501) staff       (20)     2194 2023-02-23 20:06:00.000000 pymatgen-db-2023.2.23/CHANGES.rst
--rw-r--r--   0 shyue      (501) staff       (20)     1081 2022-05-02 17:49:04.000000 pymatgen-db-2023.2.23/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)      131 2022-07-25 20:45:52.000000 pymatgen-db-2023.2.23/MANIFEST.in
--rw-r--r--   0 shyue      (501) staff       (20)     7528 2023-02-23 20:06:20.849220 pymatgen-db-2023.2.23/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     6430 2022-05-02 17:49:04.000000 pymatgen-db-2023.2.23/README.rst
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-23 20:06:20.844094 pymatgen-db-2023.2.23/pymatgen/
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-23 20:06:20.846656 pymatgen-db-2023.2.23/pymatgen/db/
--rw-r--r--   0 shyue      (501) staff       (20)      878 2023-02-23 20:06:12.000000 pymatgen-db-2023.2.23/pymatgen/db/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-23 20:06:20.847461 pymatgen-db-2023.2.23/pymatgen/db/__pycache__/
--rw-r--r--   0 shyue      (501) staff       (20)     1143 2023-02-23 20:06:12.000000 pymatgen-db-2023.2.23/pymatgen/db/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 shyue      (501) staff       (20)     6447 2022-05-02 17:50:26.000000 pymatgen-db-2023.2.23/pymatgen/db/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 shyue      (501) staff       (20)    23382 2023-02-23 20:06:14.000000 pymatgen-db-2023.2.23/pymatgen/db/__pycache__/creator.cpython-39.pyc
--rw-r--r--   0 shyue      (501) staff       (20)     3731 2023-02-23 20:06:17.000000 pymatgen-db-2023.2.23/pymatgen/db/__pycache__/matproj.cpython-39.pyc
--rw-r--r--   0 shyue      (501) staff       (20)    24727 2023-02-23 20:06:12.000000 pymatgen-db-2023.2.23/pymatgen/db/__pycache__/query_engine.cpython-39.pyc
--rw-r--r--   0 shyue      (501) staff       (20)     3015 2023-02-23 20:06:17.000000 pymatgen-db-2023.2.23/pymatgen/db/__pycache__/util.cpython-39.pyc
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-23 20:06:20.847728 pymatgen-db-2023.2.23/pymatgen/db/alchemy/
--rw-r--r--   0 shyue      (501) staff       (20)      167 2022-05-02 17:49:04.000000 pymatgen-db-2023.2.23/pymatgen/db/alchemy/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-23 20:06:20.847979 pymatgen-db-2023.2.23/pymatgen/db/alchemy/__pycache__/
--rw-r--r--   0 shyue      (501) staff       (20)      337 2022-05-02 17:50:27.000000 pymatgen-db-2023.2.23/pymatgen/db/alchemy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 shyue      (501) staff       (20)     2642 2022-05-02 17:50:27.000000 pymatgen-db-2023.2.23/pymatgen/db/alchemy/__pycache__/transmuters.cpython-39.pyc
--rw-r--r--   0 shyue      (501) staff       (20)     2413 2022-05-02 17:49:04.000000 pymatgen-db-2023.2.23/pymatgen/db/alchemy/transmuters.py
--rw-r--r--   0 shyue      (501) staff       (20)      677 2022-05-02 17:49:04.000000 pymatgen-db-2023.2.23/pymatgen/db/aliases.json
--rw-r--r--   0 shyue      (501) staff       (20)     6430 2022-05-02 17:49:04.000000 pymatgen-db-2023.2.23/pymatgen/db/config.py
--rw-r--r--   0 shyue      (501) staff       (20)    31119 2023-02-23 20:00:42.000000 pymatgen-db-2023.2.23/pymatgen/db/creator.py
--rw-r--r--   0 shyue      (501) staff       (20)     3783 2023-02-23 19:55:21.000000 pymatgen-db-2023.2.23/pymatgen/db/matproj.py
--rw-r--r--   0 shyue      (501) staff       (20)    27387 2023-02-23 19:55:26.000000 pymatgen-db-2023.2.23/pymatgen/db/query_engine.py
--rw-r--r--   0 shyue      (501) staff       (20)     2580 2023-02-23 19:21:24.000000 pymatgen-db-2023.2.23/pymatgen/db/util.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-23 20:06:20.848612 pymatgen-db-2023.2.23/pymatgen_db.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     7528 2023-02-23 20:06:20.000000 pymatgen-db-2023.2.23/pymatgen_db.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      894 2023-02-23 20:06:20.000000 pymatgen-db-2023.2.23/pymatgen_db.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-02-23 20:06:20.000000 pymatgen-db-2023.2.23/pymatgen_db.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       64 2023-02-23 20:06:20.000000 pymatgen-db-2023.2.23/pymatgen_db.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        9 2023-02-23 20:06:20.000000 pymatgen-db-2023.2.23/pymatgen_db.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)      322 2022-05-02 17:49:04.000000 pymatgen-db-2023.2.23/pyproject.toml
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-02-23 20:06:20.848754 pymatgen-db-2023.2.23/scripts/
--rwxr-xr-x   0 shyue      (501) staff       (20)    15358 2022-05-02 17:49:04.000000 pymatgen-db-2023.2.23/scripts/mgdb
--rw-r--r--   0 shyue      (501) staff       (20)      358 2023-02-23 20:06:20.849508 pymatgen-db-2023.2.23/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     1847 2023-02-23 20:06:12.000000 pymatgen-db-2023.2.23/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-07-18 14:47:08.100125 pymatgen-db-2023.7.18/
+-rw-r--r--   0 shyue      (501) staff       (20)     2194 2023-02-23 20:06:00.000000 pymatgen-db-2023.7.18/CHANGES.rst
+-rw-r--r--   0 shyue      (501) staff       (20)     1081 2022-05-02 17:49:04.000000 pymatgen-db-2023.7.18/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)      131 2022-07-25 20:45:52.000000 pymatgen-db-2023.7.18/MANIFEST.in
+-rw-r--r--   0 shyue      (501) staff       (20)     7528 2023-07-18 14:47:08.100200 pymatgen-db-2023.7.18/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     6430 2022-05-02 17:49:04.000000 pymatgen-db-2023.7.18/README.rst
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-07-18 14:47:08.094053 pymatgen-db-2023.7.18/pymatgen/
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-07-18 14:47:08.096872 pymatgen-db-2023.7.18/pymatgen/db/
+-rw-r--r--   0 shyue      (501) staff       (20)      875 2023-07-18 14:45:05.000000 pymatgen-db-2023.7.18/pymatgen/db/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-07-18 14:47:08.098403 pymatgen-db-2023.7.18/pymatgen/db/__pycache__/
+-rw-r--r--   0 shyue      (501) staff       (20)     1136 2023-07-18 14:45:01.000000 pymatgen-db-2023.7.18/pymatgen/db/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 shyue      (501) staff       (20)     6447 2022-05-02 17:50:26.000000 pymatgen-db-2023.7.18/pymatgen/db/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 shyue      (501) staff       (20)    23382 2023-02-23 20:06:14.000000 pymatgen-db-2023.7.18/pymatgen/db/__pycache__/creator.cpython-39.pyc
+-rw-r--r--   0 shyue      (501) staff       (20)     3731 2023-02-23 20:06:17.000000 pymatgen-db-2023.7.18/pymatgen/db/__pycache__/matproj.cpython-39.pyc
+-rw-r--r--   0 shyue      (501) staff       (20)    24727 2023-02-23 20:06:12.000000 pymatgen-db-2023.7.18/pymatgen/db/__pycache__/query_engine.cpython-39.pyc
+-rw-r--r--   0 shyue      (501) staff       (20)     3015 2023-02-23 20:06:17.000000 pymatgen-db-2023.7.18/pymatgen/db/__pycache__/util.cpython-39.pyc
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-07-18 14:47:08.098702 pymatgen-db-2023.7.18/pymatgen/db/alchemy/
+-rw-r--r--   0 shyue      (501) staff       (20)      167 2022-05-02 17:49:04.000000 pymatgen-db-2023.7.18/pymatgen/db/alchemy/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-07-18 14:47:08.099053 pymatgen-db-2023.7.18/pymatgen/db/alchemy/__pycache__/
+-rw-r--r--   0 shyue      (501) staff       (20)      337 2022-05-02 17:50:27.000000 pymatgen-db-2023.7.18/pymatgen/db/alchemy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 shyue      (501) staff       (20)     2642 2022-05-02 17:50:27.000000 pymatgen-db-2023.7.18/pymatgen/db/alchemy/__pycache__/transmuters.cpython-39.pyc
+-rw-r--r--   0 shyue      (501) staff       (20)     2447 2023-07-18 14:45:31.000000 pymatgen-db-2023.7.18/pymatgen/db/alchemy/transmuters.py
+-rw-r--r--   0 shyue      (501) staff       (20)      677 2022-05-02 17:49:04.000000 pymatgen-db-2023.7.18/pymatgen/db/aliases.json
+-rw-r--r--   0 shyue      (501) staff       (20)     6280 2023-07-18 14:45:31.000000 pymatgen-db-2023.7.18/pymatgen/db/config.py
+-rw-r--r--   0 shyue      (501) staff       (20)    30919 2023-07-18 14:45:31.000000 pymatgen-db-2023.7.18/pymatgen/db/creator.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3774 2023-07-18 14:45:31.000000 pymatgen-db-2023.7.18/pymatgen/db/matproj.py
+-rw-r--r--   0 shyue      (501) staff       (20)    27320 2023-07-18 14:46:14.000000 pymatgen-db-2023.7.18/pymatgen/db/query_engine.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2566 2023-07-18 14:45:31.000000 pymatgen-db-2023.7.18/pymatgen/db/util.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-07-18 14:47:08.099747 pymatgen-db-2023.7.18/pymatgen_db.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)     7528 2023-07-18 14:47:08.000000 pymatgen-db-2023.7.18/pymatgen_db.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      894 2023-07-18 14:47:08.000000 pymatgen-db-2023.7.18/pymatgen_db.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-07-18 14:47:08.000000 pymatgen-db-2023.7.18/pymatgen_db.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       64 2023-07-18 14:47:08.000000 pymatgen-db-2023.7.18/pymatgen_db.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        9 2023-07-18 14:47:08.000000 pymatgen-db-2023.7.18/pymatgen_db.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     3044 2023-07-18 14:40:15.000000 pymatgen-db-2023.7.18/pyproject.toml
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-07-18 14:47:08.099872 pymatgen-db-2023.7.18/scripts/
+-rwxr-xr-x   0 shyue      (501) staff       (20)    14449 2023-07-18 14:41:14.000000 pymatgen-db-2023.7.18/scripts/mgdb
+-rw-r--r--   0 shyue      (501) staff       (20)      358 2023-07-18 14:47:08.100497 pymatgen-db-2023.7.18/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     1880 2023-07-18 14:45:01.000000 pymatgen-db-2023.7.18/setup.py
```

### Comparing `pymatgen-db-2023.2.23/CHANGES.rst` & `pymatgen-db-2023.7.18/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/LICENSE` & `pymatgen-db-2023.7.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/PKG-INFO` & `pymatgen-db-2023.7.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-db
-Version: 2023.2.23
+Version: 2023.7.18
 Summary: Pymatgen-db is a database add-on for the Python Materials Genomics (pymatgen) materials analysis library.
 Home-page: https://github.com/materialsproject/pymatgen-db
 Author: Shyue Ping Ong
 Author-email: shyuep@gmail.com
 Maintainer: Shyue Ping Ong
 Maintainer-email: shyuep@gmail.com
 License: MIT
```

### Comparing `pymatgen-db-2023.2.23/README.rst` & `pymatgen-db-2023.7.18/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/__init__.py` & `pymatgen-db-2023.7.18/pymatgen/db/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 Pymatgen-db is a database add-on for the Python Materials Genomics (pymatgen)
 materials analysis library. It enables the creation of Materials
 Project-style MongoDB databases for management of materials data and
 provides a clean and intuitive web ui for exploring that data. A query engine
 is also provided to enable the easy translation of MongoDB docs to useful
 pymatgen objects for analysis purposes.
 """
+from __future__ import annotations
 
 import os
 
 __author__ = "Shyue Ping Ong, Dan Gunter"
 __date__ = "Jul 22 2017"
-__version__ = "2023.2.23"
+__version__ = "2023.7.18"
 
 
-from .query_engine import QueryEngine
-
 SETTINGS_FILE = os.path.join(os.path.expanduser("~"), ".pmgrc.yaml")
 
 
 def _load_mgdb_settings():
     try:
         from ruamel.yaml import YAML
 
@@ -27,8 +26,8 @@
         with open(SETTINGS_FILE) as f:
             d = yaml.load(f)
     except OSError:
         return {}
     return d
 
 
-SETTINGS = _load_mgdb_settings()
+SETTINGS = _load_mgdb_settings()
```

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/__pycache__/__init__.cpython-39.pyc` & `pymatgen-db-2023.7.18/pymatgen/db/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Feb 23 20:06:12 2023 UTC, .py size: 878 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-00000000: 610d 0d0a 0000 0000 34c7 f763 6e03 0000  a.......4..cn...
+00000000: 610d 0d0a 0000 0000 6da5 b664 6a03 0000  a.......m..dj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
-00000030: 5a00 6401 6402 6c01 5a01 6403 5a02 6404  Z.d.d.l.Z.d.Z.d.
-00000040: 5a03 6405 5a04 6406 6407 6c05 6d06 5a06  Z.d.Z.d.d.l.m.Z.
-00000050: 0100 6501 6a07 a008 6501 6a07 a009 6408  ..e.j...e.j...d.
-00000060: a101 6409 a102 5a0a 640a 640b 8400 5a0b  ..d...Z.d.d...Z.
-00000070: 650b 8300 5a0c 6402 5300 290c 6195 0100  e...Z.d.S.).a...
+00000020: 0005 0000 0040 0000 0173 4c00 0000 6400  .....@...sL...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 5a03 6404 5a04 6405 5a05 6406  d.l.Z.d.Z.d.Z.d.
+00000050: 5a06 6503 6a07 a008 6503 6a07 a009 6407  Z.e.j...e.j...d.
+00000060: a101 6408 a102 5a0a 6409 640a 8400 5a0b  ..d...Z.d.d...Z.
+00000070: 650b 8300 5a0c 6403 5300 290b 6195 0100  e...Z.d.S.).a...
 00000080: 000a 5079 6d61 7467 656e 2d64 6220 6973  ..Pymatgen-db is
 00000090: 2061 2064 6174 6162 6173 6520 6164 642d   a database add-
 000000a0: 6f6e 2066 6f72 2074 6865 2050 7974 686f  on for the Pytho
 000000b0: 6e20 4d61 7465 7269 616c 7320 4765 6e6f  n Materials Geno
 000000c0: 6d69 6373 2028 7079 6d61 7467 656e 290a  mics (pymatgen).
 000000d0: 6d61 7465 7269 616c 7320 616e 616c 7973  materials analys
 000000e0: 6973 206c 6962 7261 7279 2e20 4974 2065  is library. It e
@@ -27,46 +27,45 @@
 000001a0: 696e 650a 6973 2061 6c73 6f20 7072 6f76  ine.is also prov
 000001b0: 6964 6564 2074 6f20 656e 6162 6c65 2074  ided to enable t
 000001c0: 6865 2065 6173 7920 7472 616e 736c 6174  he easy translat
 000001d0: 696f 6e20 6f66 204d 6f6e 676f 4442 2064  ion of MongoDB d
 000001e0: 6f63 7320 746f 2075 7365 6675 6c0a 7079  ocs to useful.py
 000001f0: 6d61 7467 656e 206f 626a 6563 7473 2066  matgen objects f
 00000200: 6f72 2061 6e61 6c79 7369 7320 7075 7270  or analysis purp
-00000210: 6f73 6573 2e0a e900 0000 004e 7a1a 5368  oses.......Nz.Sh
-00000220: 7975 6520 5069 6e67 204f 6e67 2c20 4461  yue Ping Ong, Da
-00000230: 6e20 4775 6e74 6572 7a0b 4a75 6c20 3232  n Gunterz.Jul 22
-00000240: 2032 3031 377a 0932 3032 332e 322e 3233   2017z.2023.2.23
-00000250: e901 0000 0029 01da 0b51 7565 7279 456e  .....)...QueryEn
-00000260: 6769 6e65 fa01 7e7a 0b2e 706d 6772 632e  gine..~z..pmgrc.
-00000270: 7961 6d6c 6300 0000 0000 0000 0000 0000  yamlc...........
-00000280: 0004 0000 0008 0000 0043 0000 0073 6400  .........C...sd.
-00000290: 0000 7a48 6401 6402 6c00 6d01 7d00 0100  ..zHd.d.l.m.}...
-000002a0: 7c00 8300 7d01 7402 7403 8301 8f1a 7d02  |...}.t.t.....}.
-000002b0: 7c01 a004 7c02 a101 7d03 5700 6400 0400  |...|...}.W.d...
-000002c0: 0400 8303 0100 6e10 3100 733c 3000 0100  ......n.1.s<0...
-000002d0: 0100 0100 5900 0100 5700 6e16 0400 7405  ....Y...W.n...t.
-000002e0: 795e 0100 0100 0100 6900 0600 5900 5300  y^......i...Y.S.
-000002f0: 3000 7c03 5300 2903 4e72 0100 0000 2901  0.|.S.).Nr....).
-00000300: da04 5941 4d4c 2906 5a0b 7275 616d 656c  ..YAML).Z.ruamel
-00000310: 2e79 616d 6c72 0500 0000 da04 6f70 656e  .yamlr......open
-00000320: da0d 5345 5454 494e 4753 5f46 494c 45da  ..SETTINGS_FILE.
-00000330: 046c 6f61 64da 074f 5345 7272 6f72 2904  .load..OSError).
-00000340: 7205 0000 00da 0479 616d 6cda 0166 da01  r......yaml..f..
-00000350: 64a9 0072 0d00 0000 fa42 2f55 7365 7273  d..r.....B/Users
-00000360: 2f73 6879 7565 2f72 6570 6f73 2f70 796d  /shyue/repos/pym
-00000370: 6174 6765 6e2d 6462 2f64 6f63 735f 7273  atgen-db/docs_rs
-00000380: 742f 2e2e 2f70 796d 6174 6765 6e2f 6462  t/../pymatgen/db
-00000390: 2f5f 5f69 6e69 745f 5f2e 7079 da13 5f6c  /__init__.py.._l
-000003a0: 6f61 645f 6d67 6462 5f73 6574 7469 6e67  oad_mgdb_setting
-000003b0: 7316 0000 0073 1000 0000 0001 0201 0c02  s....s..........
-000003c0: 0601 0a01 2c01 0c01 0a01 720f 0000 0029  ....,.....r....)
-000003d0: 0dda 075f 5f64 6f63 5f5f da02 6f73 da0a  ...__doc__..os..
-000003e0: 5f5f 6175 7468 6f72 5f5f da08 5f5f 6461  __author__..__da
-000003f0: 7465 5f5f da0b 5f5f 7665 7273 696f 6e5f  te__..__version_
-00000400: 5f5a 0c71 7565 7279 5f65 6e67 696e 6572  _Z.query_enginer
-00000410: 0300 0000 da04 7061 7468 da04 6a6f 696e  ......path..join
-00000420: da0a 6578 7061 6e64 7573 6572 7207 0000  ..expanduserr...
-00000430: 0072 0f00 0000 5a08 5345 5454 494e 4753  .r....Z.SETTINGS
-00000440: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000450: 0e00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000460: 0000 7310 0000 0004 0908 0204 0104 0104  ..s.............
-00000470: 030c 0216 0308 0c                        .......
+00000210: 6f73 6573 2e0a e900 0000 0029 01da 0b61  oses.......)...a
+00000220: 6e6e 6f74 6174 696f 6e73 4e7a 1a53 6879  nnotationsNz.Shy
+00000230: 7565 2050 696e 6720 4f6e 672c 2044 616e  ue Ping Ong, Dan
+00000240: 2047 756e 7465 727a 0b4a 756c 2032 3220   Gunterz.Jul 22 
+00000250: 3230 3137 7a09 3230 3233 2e37 2e31 38fa  2017z.2023.7.18.
+00000260: 017e 7a0b 2e70 6d67 7263 2e79 616d 6c63  .~z..pmgrc.yamlc
+00000270: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00000280: 0800 0000 4300 0001 7364 0000 007a 4864  ....C...sd...zHd
+00000290: 0164 026c 006d 017d 0001 007c 0083 007d  .d.l.m.}...|...}
+000002a0: 0174 0274 0383 018f 1a7d 027c 01a0 047c  .t.t.....}.|...|
+000002b0: 02a1 017d 0357 0064 0004 0004 0083 0301  ...}.W.d........
+000002c0: 006e 1031 0073 3c30 0001 0001 0001 0059  .n.1.s<0.......Y
+000002d0: 0001 0057 006e 1604 0074 0579 5e01 0001  ...W.n...t.y^...
+000002e0: 0001 0069 0006 0059 0053 0030 007c 0353  ...i...Y.S.0.|.S
+000002f0: 0029 034e 7201 0000 0029 01da 0459 414d  .).Nr....)...YAM
+00000300: 4c29 065a 0b72 7561 6d65 6c2e 7961 6d6c  L).Z.ruamel.yaml
+00000310: 7204 0000 00da 046f 7065 6eda 0d53 4554  r......open..SET
+00000320: 5449 4e47 535f 4649 4c45 da04 6c6f 6164  TINGS_FILE..load
+00000330: da07 4f53 4572 726f 7229 0472 0400 0000  ..OSError).r....
+00000340: da04 7961 6d6c da01 66da 0164 a900 720c  ..yaml..f..d..r.
+00000350: 0000 00fa 422f 5573 6572 732f 7368 7975  ....B/Users/shyu
+00000360: 652f 7265 706f 732f 7079 6d61 7467 656e  e/repos/pymatgen
+00000370: 2d64 622f 646f 6373 5f72 7374 2f2e 2e2f  -db/docs_rst/../
+00000380: 7079 6d61 7467 656e 2f64 622f 5f5f 696e  pymatgen/db/__in
+00000390: 6974 5f5f 2e70 79da 135f 6c6f 6164 5f6d  it__.py.._load_m
+000003a0: 6764 625f 7365 7474 696e 6773 1500 0000  gdb_settings....
+000003b0: 7310 0000 0000 0102 010c 0206 010a 012c  s..............,
+000003c0: 010c 010a 0172 0e00 0000 290d da07 5f5f  .....r....)...__
+000003d0: 646f 635f 5fda 0a5f 5f66 7574 7572 655f  doc__..__future_
+000003e0: 5f72 0200 0000 da02 6f73 da0a 5f5f 6175  _r......os..__au
+000003f0: 7468 6f72 5f5f da08 5f5f 6461 7465 5f5f  thor__..__date__
+00000400: da0b 5f5f 7665 7273 696f 6e5f 5fda 0470  ..__version__..p
+00000410: 6174 68da 046a 6f69 6eda 0a65 7870 616e  ath..join..expan
+00000420: 6475 7365 7272 0600 0000 720e 0000 005a  duserr....r....Z
+00000430: 0853 4554 5449 4e47 5372 0c00 0000 720c  .SETTINGSr....r.
+00000440: 0000 0072 0c00 0000 720d 0000 00da 083c  ...r....r......<
+00000450: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
+00000460: 0408 0c02 0802 0401 0401 0403 1603 080c  ................
```

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/__pycache__/config.cpython-39.pyc` & `pymatgen-db-2023.7.18/pymatgen/db/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/__pycache__/creator.cpython-39.pyc` & `pymatgen-db-2023.7.18/pymatgen/db/__pycache__/creator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/__pycache__/matproj.cpython-39.pyc` & `pymatgen-db-2023.7.18/pymatgen/db/__pycache__/matproj.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/__pycache__/query_engine.cpython-39.pyc` & `pymatgen-db-2023.7.18/pymatgen/db/__pycache__/query_engine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/__pycache__/util.cpython-39.pyc` & `pymatgen-db-2023.7.18/pymatgen/db/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/alchemy/__pycache__/transmuters.cpython-39.pyc` & `pymatgen-db-2023.7.18/pymatgen/db/alchemy/__pycache__/transmuters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/alchemy/transmuters.py` & `pymatgen-db-2023.7.18/pymatgen/db/alchemy/transmuters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """
 This module implements a version of pymatgen's Transmuter to generate
 TransformedStructures from DB data sources. They enable the
 high-throughput generation of new structures and input files.
 """
-
+from __future__ import annotations
 
 __author__ = "Shyue Ping Ong"
 __copyright__ = "Copyright 2012, The Materials Project"
 __version__ = "0.1"
 __maintainer__ = "Shyue Ping Ong"
 __email__ = "shyue@mit.edu"
 __date__ = "Mar 4, 2012"
```

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/aliases.json` & `pymatgen-db-2023.7.18/pymatgen/db/aliases.json`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/config.py` & `pymatgen-db-2023.7.18/pymatgen/db/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 Main class is DBConfig, which encapsulates a database configuration
 passed in as a file or object. For example::
     cfg1 = DBConfig()  # use defaults
     cfg2 = DBConfig("/path/to/myfile.json")  # read from file
     f = open("/other/file.json")
     cfg3 = DBConfig(f)  # read from file object
     # access dict of parsed conf. settings
-    settings = cfg1.settings
+    settings = cfg1.settings.
 """
+from __future__ import annotations
 
 import os
 
 from ruamel import yaml
 
 __author__ = "Dan Gunter <dkgunter@lbl.gov>"
 __date__ = "4/25/14"
@@ -24,22 +25,18 @@
 COLL_KEY = "collection"
 USER_KEY = "user"
 PASS_KEY = "password"
 ALIASES_KEY = "aliases"
 
 
 class ConfigurationFileError(Exception):
-    """
-    Error for Config File
-    """
+    """Error for Config File."""
 
     def __init__(self, filename, err):
-        """
-        Init for ConfigurationFileError.
-        """
+        """Init for ConfigurationFileError."""
         msg = f"reading '{filename}': {err}"
         Exception.__init__(self, msg)
 
 
 class DBConfig:
     """Database configuration."""
 
@@ -65,26 +62,25 @@
         Settings are created from config_dict, if given,
         or parsed config_file, if given, otherwise
         the DEFAULT_FILE is tried and if that is not present
         the DEFAULT_SETTINGS are used without modification.
         :param config_file: Read configuration from this file.
         :type config_file: file or str path
         :param config_dict: Set configuration from this dictionary.
-        :raises: ConfigurationFileError if cannot read/parse config_file
+        :raises: ConfigurationFileError if cannot read/parse config_file.
         """
         self._cfg = dict(self.DEFAULT_SETTINGS)
         settings = {}
         if config_dict:
             settings = config_dict.copy()
             auth_aliases(settings)
         else:
             # Try to use DEFAULT_FILE if no config_file
-            if config_file is None:
-                if os.path.exists(self.DEFAULT_FILE):
-                    config_file = self.DEFAULT_FILE
+            if config_file is None and os.path.exists(self.DEFAULT_FILE):
+                config_file = self.DEFAULT_FILE
             # If there was a config_file, parse it
             if config_file is not None:
                 try:
                     settings = get_settings(config_file)
                 except Exception as err:
                     path = _as_file(config_file).name
                     raise ConfigurationFileError(path, err)
@@ -96,80 +92,64 @@
 
     def copy(self):
         """Return a copy of self (internal settings are copied)."""
         return DBConfig(config_dict=self._cfg.copy())
 
     @property
     def settings(self):
-        """
-        Return settings
-        """
+        """Return settings."""
         return self._cfg
 
     @property
     def host(self):
-        """
-        Return host
-        """
+        """Return host."""
         return self._cfg.get(HOST_KEY, None)
 
     @property
     def port(self):
-        """
-        Return port.
-        """
+        """Return port."""
         return self._cfg.get(PORT_KEY, self.DEFAULT_PORT)
 
     @property
     def dbname(self):
         """Name of the database."""
         return self._cfg.get(DB_KEY, None)
 
     @dbname.setter
     def dbname(self, value):
-        """
-        Set dbname.
-        """
+        """Set dbname."""
         self._cfg[DB_KEY] = value
 
     @property
     def collection(self):
-        """
-        Return collection.
-        """
+        """Return collection."""
         return self._cfg.get(COLL_KEY, None)
 
     @collection.setter
     def collection(self, value):
-        """
-        Set collection.
-        """
+        """Set collection."""
         self._cfg[COLL_KEY] = value
 
     @property
     def user(self):
-        """
-        Return user.
-        """
+        """Return user."""
         return self._cfg.get(USER_KEY, None)
 
     @property
     def password(self):
-        """
-        Return password.
-        """
+        """Return password."""
         return self._cfg.get(PASS_KEY, None)
 
 
 def get_settings(infile):
     """Read settings from input file.
     :param infile: Input file for JSON settings.
     :type infile: file or str path
     :return: Settings parsed from file
-    :rtype: dict
+    :rtype: dict.
     """
     yml = yaml.YAML()
     settings = yml.load(_as_file(infile))
     if not hasattr(settings, "keys"):
         raise ValueError(f"Settings not found in {infile}")
 
     # Processing of namespaced parameters in .pmgrc.yaml.
@@ -197,15 +177,15 @@
     admin or readonly password will be in keys "user" and "password".
     :param settings: Connection settings
     :type settings: dict
     :param admin: Check for admin password
     :param readonly: Check for readonly password
     :param readonly_first: Check for readonly password before admin
     :return: Whether user/password were found
-    :rtype: bool
+    :rtype: bool.
     """
     U, P = USER_KEY, PASS_KEY
     # If user/password, un-prefixed, exists, do nothing.
     if U in settings and P in settings:
         return True
 
     # Set prefixes
```

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/creator.py` & `pymatgen-db-2023.7.18/pymatgen/db/creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module defines a Drone to assimilate vasp data and insert it into a
 Mongo database.
 """
-
+from __future__ import annotations
 
 import datetime
 import glob
 import json
 import logging
 import os
 import re
@@ -17,27 +17,27 @@
 from fnmatch import fnmatch
 
 import gridfs
 import numpy as np
 from monty.io import zopen
 from monty.json import MontyEncoder
 from pymongo import MongoClient
+
 from pymatgen.analysis.bond_valence import BVAnalyzer
 from pymatgen.analysis.local_env import VoronoiNN
 from pymatgen.analysis.structure_analyzer import oxide_type
 from pymatgen.apps.borg.hive import AbstractDrone
 from pymatgen.core.composition import Composition
 from pymatgen.core.structure import Structure
 from pymatgen.entries.computed_entries import ComputedEntry
 from pymatgen.ext.matproj import MPRester
 from pymatgen.io.cif import CifWriter
 from pymatgen.io.vasp import Incar, Kpoints, Oszicar, Outcar, Poscar, Potcar, Vasprun
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
-
 __author__ = "Shyue Ping Ong"
 __copyright__ = "Copyright 2012, The Materials Project"
 __version__ = "2.0.0"
 __maintainer__ = "Shyue Ping Ong"
 __email__ = "shyue@mit.edu"
 __date__ = "Mar 18, 2012"
 
@@ -184,42 +184,37 @@
             If in simulate_mode, the entire doc is returned for debugging
             purposes. Else, only the task_id of the inserted doc is returned.
         """
         try:
             d = self.get_task_doc(path)
             if self.mapi_key is not None and d["state"] == "successful":
                 self.calculate_stability(d)
-            tid = self._insert_doc(d)
-            return tid
+            return self._insert_doc(d)
         except Exception:
             import traceback
 
             logger.error(traceback.format_exc())
             return False
 
     def calculate_stability(self, d):
-        """
-        Calculate the stability (e_above_hull and decomposes_to) for a entry dict.
-        """
+        """Calculate the stability (e_above_hull and decomposes_to) for a entry dict."""
         m = MPRester(self.mapi_key)
         functional = d["pseudo_potential"]["functional"]
         syms = [f"{functional} {l}" for l in d["pseudo_potential"]["labels"]]
         entry = ComputedEntry(
             Composition(d["unit_cell_formula"]),
             d["output"]["final_energy"],
             parameters={"hubbards": d["hubbards"], "potcar_symbols": syms},
         )
         data = m.get_stability([entry])[0]
         for k in ("e_above_hull", "decomposes_to"):
             d["analysis"][k] = data[k]
 
     def get_task_doc(self, path):
-        """
-        Get the entire task doc for a path, including any post-processing.
-        """
+        """Get the entire task doc for a path, including any post-processing."""
         logger.info(f"Getting task doc for base dir :{path}")
         files = os.listdir(path)
         vasprun_files = OrderedDict()
         if "STOPCAR" in files:
             # Stopped runs. Try to parse as much as possible.
             logger.info(path + " contains stopped run")
         for r in self.runs:
@@ -237,15 +232,15 @@
                     vasprun_files["standard"] = f
 
         if len(vasprun_files) > 0:
             d = self.generate_doc(path, vasprun_files)
             if not d:
                 d = self.process_killed_run(path)
             self.post_process(path, d)
-        elif (not (path.endswith("relax1") or path.endswith("relax2"))) and contains_vasp_input(path):
+        elif (not (path.endswith(("relax1", "relax2")))) and contains_vasp_input(path):
             # If not Materials Project style, process as a killed run.
             logger.warning(path + " contains killed run")
             d = self.process_killed_run(path)
             self.post_process(path, d)
         else:
             raise ValueError("No VASP files found!")
 
@@ -325,15 +320,15 @@
             with zopen(filenames[0], "rt") as f:
                 transformations = json.load(f)
                 try:
                     m = re.match(r"(\d+)-ICSD", transformations["history"][0]["source"])
                     if m:
                         d["icsd_id"] = int(m.group(1))
                 except Exception:
-                    logger.warning("Cannot parse ICSD from transformations " "file.")
+                    logger.warning("Cannot parse ICSD from transformations file.")
                     pass
         else:
             logger.warning("Transformations file does not exist.")
 
         other_parameters = transformations.get("other_parameters")
         new_tags = None
         if other_parameters:
@@ -393,17 +388,15 @@
 
         if new_tags:
             d["tags"] = new_tags
 
         logger.info("Post-processed " + fullpath)
 
     def process_killed_run(self, dir_name):  # pylint: disable=R0201
-        """
-        Process a killed vasp run.
-        """
+        """Process a killed vasp run."""
         fullpath = os.path.abspath(dir_name)
         logger.info("Processing Killed run " + fullpath)
         d = {"dir_name": fullpath, "state": "killed", "oszicar": {}}
 
         for f in os.listdir(dir_name):
             filename = os.path.join(dir_name, f)
             if fnmatch(f, "INCAR*"):
@@ -465,26 +458,23 @@
                 except Exception:
                     logger.error(f"Unable to parse POTCAR for killed run in {dir_name}.")
             elif fnmatch(f, "OSZICAR"):
                 try:
                     d["oszicar"]["root"] = Oszicar(os.path.join(dir_name, f)).as_dict()
                 except Exception:
                     logger.error(f"Unable to parse OSZICAR for killed run in {dir_name}.")
-            elif re.match(r"relax\d", f):
-                if os.path.exists(os.path.join(dir_name, f, "OSZICAR")):
-                    try:
-                        d["oszicar"][f] = Oszicar(os.path.join(dir_name, f, "OSZICAR")).as_dict()
-                    except Exception:
-                        logger.error(f"Unable to parse OSZICAR for killed run in {dir_name}.")
+            elif re.match(r"relax\d", f) and os.path.exists(os.path.join(dir_name, f, "OSZICAR")):
+                try:
+                    d["oszicar"][f] = Oszicar(os.path.join(dir_name, f, "OSZICAR")).as_dict()
+                except Exception:
+                    logger.error(f"Unable to parse OSZICAR for killed run in {dir_name}.")
         return d
 
     def process_vasprun(self, dir_name, taskname, filename):
-        """
-        Process a vasprun.xml file.
-        """
+        """Process a vasprun.xml file."""
         vasprun_file = os.path.join(dir_name, filename)
         parse_projected_eigen = self.parse_projected_eigen and (
             self.parse_projected_eigen != "final" or taskname == self.runs[-1]
         )
         r = Vasprun(vasprun_file, parse_projected_eigen=parse_projected_eigen)
         d = r.as_dict()
         d["dir_name"] = os.path.abspath(dir_name)
@@ -610,57 +600,48 @@
             not any(parent.endswith(os.sep + r) for r in self.runs)
             and len(glob.glob(os.path.join(parent, "vasprun.xml*"))) > 0
         ):
             return [parent]
         return []
 
     def convert(self, d):  # pylint: disable=R0201
-        """
-        Just return the dict.
-        """
+        """Just return the dict."""
         return d
 
     def __str__(self):
         return "VaspToDbDictDrone"
 
     @classmethod
     def from_dict(cls, d):
-        """
-        From dict
-        """
+        """From dict."""
         return cls(**d["init_args"])
 
     def as_dict(self):
-        """
-        Dict representation.
-        """
+        """Dict representation."""
         init_args = {
             "host": self.host,
             "port": self.port,
             "database": self.database,
             "user": self.user,
             "password": self.password,
             "collection": self.collection,
             "parse_dos": self.parse_dos,
             "simulate_mode": self.simulate,
             "additional_fields": self.additional_fields,
             "update_duplicates": self.update_duplicates,
         }
-        output = {
+        return {
             "name": self.__class__.__name__,
             "init_args": init_args,
             "version": __version__,
         }
-        return output
 
 
 def get_basic_analysis_and_error_checks(d, max_force_threshold=0.5, volume_change_threshold=0.2):
-    """
-    Generate basic analysis and error checks data for a run.
-    """
+    """Generate basic analysis and error checks data for a run."""
     initial_vol = d["input"]["crystal"]["lattice"]["volume"]
     final_vol = d["output"]["crystal"]["lattice"]["volume"]
     delta_vol = final_vol - initial_vol
     percent_delta_vol = delta_vol / initial_vol
     coord_num = get_coordination_numbers(d)
     calc = d["calculations"][-1]
     gap = calc["output"]["bandgap"]
@@ -677,15 +658,15 @@
     bv_struct = Structure.from_dict(d["output"]["crystal"])
     try:
         bva = BVAnalyzer()
         bv_struct = bva.get_oxi_state_decorated_structure(bv_struct)
     except ValueError as e:
         logger.error(f"Valence cannot be determined due to {e}.")
     except Exception as ex:
-        logger.error(f"BVAnalyzer error {str(ex)}.")
+        logger.error(f"BVAnalyzer error {ex!s}.")
 
     max_force = None
     if d["state"] == "successful" and d["calculations"][0]["input"]["parameters"].get("NSW", 0) > 0:
         # handle the max force and max force error
         max_force = max(np.linalg.norm(a) for a in d["calculations"][-1]["output"]["ionic_steps"][-1]["forces"])
 
         if max_force > max_force_threshold:
```

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/matproj.py` & `pymatgen-db-2023.7.18/pymatgen/db/matproj.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 See https://medium.com/@shyuep/a-local-materials-project-database-1ea909430c95
 """
 from __future__ import annotations
 
 import itertools
 
 import pymongo
+
 from pymatgen.entries.computed_entries import ComputedStructureEntry
 from pymatgen.ext.matproj import MPRester
 
 
 class MPDB:
-    """
-    This module allows you to create a local MP database based on ComputedStructureEntries.
-    """
+    """This module allows you to create a local MP database based on ComputedStructureEntries."""
 
     def __init__(self, *args, **kwargs):
         """
         @param args: Pass through to MongoClient. E.g., you can create a connection using uri strings, etc.
         @param kwargs: Pass through to MongoClient. E.g., you can create a connection using uri strings, etc.
         """
         client = pymongo.MongoClient(*args, **kwargs)
```

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/query_engine.py` & `pymatgen-db-2023.7.18/pymatgen/db/query_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module provides a QueryEngine that simplifies queries for Mongo databases
 generated using hive.
 """
-
+from __future__ import annotations
 
 __author__ = "Shyue Ping Ong, Michael Kocher, Dan Gunter"
 __copyright__ = "Copyright 2011, The Materials Project"
 __version__ = "2.0"
 __maintainer__ = "Shyue Ping Ong"
 __email__ = "shyuep@gmail.com"
 __status__ = "Production"
@@ -18,14 +18,15 @@
 import os
 import zlib
 from collections import OrderedDict
 from collections.abc import Iterable
 
 import gridfs
 import pymongo
+
 from pymatgen.core import Composition, Structure
 from pymatgen.electronic_structure.core import Orbital, Spin
 from pymatgen.electronic_structure.dos import CompleteDos, Dos
 from pymatgen.entries.computed_entries import ComputedEntry, ComputedStructureEntry
 
 _log = logging.getLogger("mg." + __name__)
 
@@ -113,15 +114,15 @@
                     to organize the doc format in a way that is different from the
                     query format.
                 defaults (dict): Criteria that should be applied
                     by default to all queries. For example, a collection may
                     contain data from both successful and unsuccessful runs but
                     for most querying purposes, you may want just successful runs
                     only. Note that defaults do not affect explicitly specified
-                    criteria, i.e., if you suppy a query for {"state": "killed"},
+                    criteria, i.e., if you supply a query for {"state": "killed"},
                     this will override the default for {"state": "successful"}.
             default_properties (list): Property names (strings) to use by
                 default, if no `properties` are given to query().
             query_post (list): Functions to post-process the `criteria` passed
                 to `query()`, after aliases are resolved.
                 Function takes two args, the criteria dict and list of
                 result properties. Both may be modified in-place.
@@ -148,17 +149,15 @@
         self.set_aliases_and_defaults(aliases_config=aliases_config, default_properties=default_properties)
         # Post-processing functions
         self.query_post = query_post or []
         self.result_post = result_post or []
 
     @property
     def collection_name(self):
-        """
-        Returns collection name.
-        """
+        """Returns collection name."""
         return self._collection_name
 
     @collection_name.setter
     def collection_name(self, value):
         """Switch to another collection.
         Note that you may have to set the aliases and default properties if the
         schema of the new collection differs from the current collection.
@@ -192,19 +191,19 @@
         # set default properties
         if default_properties is None:
             self._default_props, self._default_prop_dict = None, None
         else:
             self._default_props, self._default_prop_dict = self._parse_properties(default_properties)
 
     def __enter__(self):
-        """Allows for use with the 'with' context manager"""
+        """Allows for use with the 'with' context manager."""
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        """Allows for use with the 'with' context manager"""
+        """Allows for use with the 'with' context manager."""
         self.close()
 
     def close(self):
         """Disconnects the connection."""
         self.connection.disconnect()
 
     def get_entries_in_system(
@@ -372,15 +371,15 @@
             elif key in ["$or", "$and"]:
                 parsed_crit[key] = [self._parse_criteria(m) for m in crit]
             else:
                 parsed_crit[self.aliases.get(key, key)] = crit
         return parsed_crit
 
     def ensure_index(self, key, unique=False):
-        """Wrapper for pymongo.Collection.ensure_index"""
+        """Wrapper for pymongo.Collection.ensure_index."""
         return self.collection.ensure_index(key, unique=unique)
 
     def query(self, properties=None, criteria=None, distinct_key=None, **kwargs):
         r"""
         Convenience method for database access.  All properties and criteria
         can be specified using simplified names defined in Aliases.  You can
         use the supported_properties property to get the list of supported
@@ -427,15 +426,15 @@
             return QueryListResults(prop_dict, cur, postprocess=self.result_post)
 
         return QueryResults(prop_dict, cur, postprocess=self.result_post)
 
     def _parse_properties(self, properties):
         """Make list of properties into 2 things:
         (1) dictionary of { 'aliased-field': 1, ... } for a mongodb query eg. {''}
-        (2) dictionary, keyed by aliased field, for display
+        (2) dictionary, keyed by aliased field, for display.
         """
         props = {}
         # TODO: clean up prop_dict?
         prop_dict = OrderedDict()
         # We use a dict instead of list to provide for a richer syntax
         for p in properties:
             if p in self.aliases:
@@ -525,17 +524,15 @@
     def __getitem__(self, item):
         """Support pymongo.Database syntax db['collection'] to access collections.
         Simply delegate this to the pymongo.Database instance, so behavior is the same.
         """
         return self.db[item]
 
     def get_dos_from_id(self, task_id):
-        """
-        Overrides the get_dos_from_id for the MIT gridfs format.
-        """
+        """Overrides the get_dos_from_id for the MIT gridfs format."""
         args = {"task_id": task_id}
         fields = ["calculations"]
         structure = self.get_structure_from_id(task_id)
         dosid = None
         for r in self.query(fields, args):
             dosid = r["calculations"][-1]["dos_fs_id"]
         if dosid is not None:
@@ -583,15 +580,15 @@
         self._prop_dict = prop_dict
         self._pproc = postprocess or []  # make empty values iterable
 
     def _wrapper(self, func):
         """
         This function wraps all callable objects returned by self.__getattr__.
         If the result is a cursor, wrap it into a QueryResults object
-        so that you can invoke postprocess functions in self._pproc
+        so that you can invoke postprocess functions in self._pproc.
         """
 
         def wrapped(*args, **kwargs):
             ret_val = func(*args, **kwargs)
             if isinstance(ret_val, pymongo.cursor.Cursor):
                 ret_val = self.from_cursor(ret_val)
             return ret_val
@@ -610,23 +607,19 @@
             # wrap callable objects to convert returned cursors into QueryResults
             if callable(ret_val):
                 return self._wrapper(ret_val)
             return ret_val
         raise AttributeError
 
     def clone(self):
-        """
-        Provide a clone of the QueryResults.
-        """
+        """Provide a clone of the QueryResults."""
         return QueryResults(self._prop_dict, self._results.clone())
 
     def from_cursor(self, cursor):
-        """
-        Create a QueryResults object from a cursor object
-        """
+        """Create a QueryResults object from a cursor object."""
         return QueryResults(self._prop_dict, cursor, self._pproc)
 
     def __len__(self):
         """Return length as a `count()` on the MongoDB cursor."""
         return len(list(self._results.clone()))
 
     def __getitem__(self, i):
@@ -669,27 +662,21 @@
             yield self._mapped_result(r)
 
 
 class QueryListResults(QueryResults):
     """Set of QueryResults on a list instead of a MongoDB cursor."""
 
     def clone(self):
-        """
-        Return a clone of the QueryListResults.
-        """
+        """Return a clone of the QueryListResults."""
         return QueryResults(self._prop_dict, self._results[:])
 
     def __len__(self):
         """Return length of iterable, as a list if possible; otherwise,
         fall back to the superclass' implementation.
         """
         if hasattr(self._results, "__len__"):
             return len(self._results)
         return QueryResults.__len__(self)
 
 
 class QueryError(Exception):
-    """
-    Exception class for errors occuring during queries.
-    """
-
-    pass
+    """Exception class for errors occurring during queries."""
```

### Comparing `pymatgen-db-2023.2.23/pymatgen/db/util.py` & `pymatgen-db-2023.7.18/pymatgen/db/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-"""
-Utility functions used across scripts.
-"""
+"""Utility functions used across scripts."""
+from __future__ import annotations
 
 import datetime
 import json
 import logging
 
 import bson
 from pymongo.mongo_client import MongoClient
@@ -15,41 +14,33 @@
 DEFAULT_CONFIG_FILE = DBConfig.DEFAULT_FILE
 DEFAULT_SETTINGS = DBConfig.DEFAULT_SETTINGS
 
 _log = logging.getLogger("mg.util")
 
 
 class MongoJSONEncoder(json.JSONEncoder):
-    """
-    JSON encoder to support ObjectIDs and datetime used in Mongo.
-    """
+    """JSON encoder to support ObjectIDs and datetime used in Mongo."""
 
     def default(self, o):
-        """
-        Override default to support ObjectID and datetime.
-        """
+        """Override default to support ObjectID and datetime."""
         if isinstance(o, bson.objectid.ObjectId):
             return str(o)
         if isinstance(o, datetime.datetime):
             return o.isoformat()
         return json.JSONEncoder.default(self, o)
 
 
 def get_settings(config_file):
-    """
-    Get settings from file.
-    """
+    """Get settings from file."""
     cfg = DBConfig(config_file)
     return cfg.settings
 
 
 def get_database(config_file=None, settings=None, admin=False, **kwargs):
-    """
-    Get a database object from a config file.
-    """
+    """Get a database object from a config file."""
     d = get_settings(config_file) if settings is None else settings
 
     try:
         user = d["admin_user"] if admin else d["readonly_user"]
         passwd = d["admin_password"] if admin else d["readonly_password"]
         conn = MongoClient(
             host=d["host"], port=d["port"], username=user, password=passwd, authSource=d["database"], **kwargs
@@ -74,15 +65,15 @@
     return db[settings["collection"]]
 
 
 def collection_keys(coll, sep="."):
     """Get a list of all (including nested) keys in a collection.
     Examines the first document in the collection.
     :param sep: Separator for nested keys
-    :return: List of str
+    :return: List of str.
     """
 
     def _keys(x, pre=""):
         for k in x:
             yield pre + k
             if isinstance(x[k], dict):
                 yield from _keys(x[k], pre + k + sep)
```

### Comparing `pymatgen-db-2023.2.23/pymatgen_db.egg-info/PKG-INFO` & `pymatgen-db-2023.7.18/pymatgen_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-db
-Version: 2023.2.23
+Version: 2023.7.18
 Summary: Pymatgen-db is a database add-on for the Python Materials Genomics (pymatgen) materials analysis library.
 Home-page: https://github.com/materialsproject/pymatgen-db
 Author: Shyue Ping Ong
 Author-email: shyuep@gmail.com
 Maintainer: Shyue Ping Ong
 Maintainer-email: shyuep@gmail.com
 License: MIT
```

### Comparing `pymatgen-db-2023.2.23/pymatgen_db.egg-info/SOURCES.txt` & `pymatgen-db-2023.7.18/pymatgen_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatgen-db-2023.2.23/scripts/mgdb` & `pymatgen-db-2023.7.18/scripts/mgdb`

 * *Files 8% similar despite different names*

```diff
@@ -1,227 +1,234 @@
 #!/usr/bin/env python
 
-"""
-A helper script for many matgendb functions.
-"""
+"""A helper script for many matgendb functions."""
+from __future__ import annotations
 
 __author__ = "Shyue Ping Ong"
 __copyright__ = "Copyright 2012, The Materials Project"
 __version__ = "1.2"
 __maintainer__ = "Shyue Ping Ong"
 __email__ = "shyue@mit.edu"
 __date__ = "Dec 1, 2012"
 
+import argparse
 import datetime
+import json
 import logging
 import multiprocessing
-import json
 import sys
-import argparse
-import six
 
-from pymongo import MongoClient, ASCENDING
+from pymongo import ASCENDING, MongoClient
 
 from pymatgen.apps.borg.queen import BorgQueen
-
-from matgendb import SETTINGS
-from matgendb.query_engine import QueryEngine
-from matgendb.creator import VaspToDbTaskDrone
-from matgendb.dbconfig import DBConfig
-from matgendb.util import get_settings, DEFAULT_SETTINGS, MongoJSONEncoder
+from pymatgen.db import SETTINGS
+from pymatgen.db.config import DBConfig
+from pymatgen.db.creator import VaspToDbTaskDrone
+from pymatgen.db.query_engine import QueryEngine
+from pymatgen.db.util import DEFAULT_SETTINGS, MongoJSONEncoder, get_settings
 
 _log = logging.getLogger("mg")  # parent
 
 
 def init_db(args):
     settings = DBConfig.ALL_SETTINGS
     defaults = dict(DEFAULT_SETTINGS)
     doc = {}
     print("Please supply the following configuration values")
     print("(press Enter if you want to accept the defaults)\n")
     for k in settings:
-        v = defaults.get(k, '')
-        val = six.moves.input("Enter {} (default: {}) : ".format(k, v))
+        v = defaults.get(k, "")
+        val = input(f"Enter {k} (default: {v}) : ")
         doc[k] = val if val else v
     doc["port"] = int(doc["port"])  # enforce the port as an int
-    for k in ["admin_user", "admin_password", "readonly_user",
-              "readonly_password"]:
-        v = defaults.get(k, '')
-        val = six.moves.input("Enter {} (default: {}) : ".format(k, v))
+    for k in ["admin_user", "admin_password", "readonly_user", "readonly_password"]:
+        v = defaults.get(k, "")
+        val = input(f"Enter {k} (default: {v}) : ")
         doc[k] = val if val else v
     with open(args.config_file, "w") as f:
         json.dump(doc, f, indent=4, sort_keys=True)
-    print("\nConfiguration written to {}!".format(args.config_file))
+    print(f"\nConfiguration written to {args.config_file}!")
 
 
 def update_db(args):
     FORMAT = "%(relativeCreated)d msecs : %(message)s"
 
     if args.logfile:
-        logging.basicConfig(level=logging.INFO, format=FORMAT,
-                            filename=args.logfile[0])
+        logging.basicConfig(level=logging.INFO, format=FORMAT, filename=args.logfile[0])
     else:
         logging.basicConfig(level=logging.INFO, format=FORMAT)
 
     d = get_settings(args.config_file)
 
-    _log.info("Db insertion started at {}.".format(datetime.datetime.now()))
+    _log.info(f"Db insertion started at {datetime.datetime.now()}.")
     additional_fields = {"author": args.author, "tags": args.tag}
     drone = VaspToDbTaskDrone(
-        host=d["host"], port=d["port"],  database=d["database"],
-        user=d["admin_user"], password=d["admin_password"],
+        host=d["host"],
+        port=d["port"],
+        database=d["database"],
+        user=d["admin_user"],
+        password=d["admin_password"],
         parse_dos=args.parse_dos,
-        collection=d["collection"], update_duplicates=args.force_update_dupes,
-        additional_fields=additional_fields, mapi_key=d.get("mapi_key", None))
+        collection=d["collection"],
+        update_duplicates=args.force_update_dupes,
+        additional_fields=additional_fields,
+        mapi_key=d.get("mapi_key", None),
+    )
     ncpus = multiprocessing.cpu_count() if not args.ncpus else args.ncpus
-    _log.info("Using {} cpus...".format(ncpus))
+    _log.info(f"Using {ncpus} cpus...")
     queen = BorgQueen(drone, number_of_drones=ncpus)
     queen.parallel_assimilate(args.directory)
     tids = list(map(int, filter(lambda x: x, queen.get_data())))
-    _log.info("Db upate completed at {}.".format(datetime.datetime.now()))
-    _log.info("{} new task ids inserted.".format(len(tids)))
+    _log.info(f"Db update completed at {datetime.datetime.now()}.")
+    _log.info(f"{len(tids)} new task ids inserted.")
 
 
 def optimize_indexes(args):
     d = get_settings(args.config_file)
     c = MongoClient(d["host"], d["port"])
     db = c[d["database"]]
     db.authenticate(d["admin_user"], d["admin_password"])
     coll = db[d["collection"]]
     coll.drop_indexes()
-    coll.ensure_index('task_id', unique=True)
-    for key in ['unit_cell_formula', 'reduced_cell_formula', 'chemsys',
-                'nsites', 'pretty_formula', 'analysis.e_above_hull',
-                "icsd_ids"]:
-        print("Building {} index".format(key))
+    coll.ensure_index("task_id", unique=True)
+    for key in [
+        "unit_cell_formula",
+        "reduced_cell_formula",
+        "chemsys",
+        "nsites",
+        "pretty_formula",
+        "analysis.e_above_hull",
+        "icsd_ids",
+    ]:
+        print(f"Building {key} index")
         coll.ensure_index(key)
     print("Building nelements and elements compound index")
-    compound_index = [('nelements', ASCENDING), ('elements', ASCENDING)]
+    compound_index = [("nelements", ASCENDING), ("elements", ASCENDING)]
     coll.ensure_index(compound_index)
     coll.ensure_index(compound_index)
 
 
 def query_db(args):
     from tabulate import tabulate
+
     d = get_settings(args.config_file)
-    qe = QueryEngine(host=d["host"], port=d["port"], database=d["database"],
-                     user=d["readonly_user"], password=d["readonly_password"],
-                     collection=d["collection"],
-                     aliases_config=d.get("aliases_config", None))
+    qe = QueryEngine(
+        host=d["host"],
+        port=d["port"],
+        database=d["database"],
+        user=d["readonly_user"],
+        password=d["readonly_password"],
+        collection=d["collection"],
+        aliases_config=d.get("aliases_config", None),
+    )
     criteria = None
     if args.criteria:
         try:
             criteria = json.loads(args.criteria)
         except ValueError:
-            print("Criteria {} is not a valid JSON string!".format(
-                args.criteria))
+            print(f"Criteria {args.criteria} is not a valid JSON string!")
             sys.exit(-1)
 
     # TODO: document this 'feature' --dang 4/4/2013
-    is_a_file = lambda s: len(s) == 1 and s[0].startswith(':')
+    def is_a_file(s):
+        return len(s) == 1 and s[0].startswith(":")
+
     if is_a_file(args.properties):
-        with open(args.properties[0][1:], 'rb') as f:
+        with open(args.properties[0][1:], "rb") as f:
             props = [s.strip() for s in f]
     else:
         props = args.properties
 
     if args.dump_json:
         for r in qe.query(properties=props, criteria=criteria):
             print(json.dumps(r, cls=MongoJSONEncoder))
     else:
         t = []
         for r in qe.query(properties=props, criteria=criteria):
             t.append([r[p] for p in props])
         print(tabulate(t, headers=props))
 
 
-class StatsCommands(object):
-    """Encapsulate statistics commands.
-    """
+class StatsCommands:
+    """Encapsulate statistics commands."""
+
     #: Constants for names of format options
     FORMAT_YAML, FORMAT_CLEAN = "yaml", "simple"
 
     def __init__(self, query_engine, output_format=None, latest_prop=None, **extra_kw):
         """Constructor.
 
         :param query_engine: Connection to Mongo
         :type query_engine: matgendb.query_engine.QueryEngine
         """
         self._qe = query_engine
         self._db, self._coll = query_engine.db, query_engine.collection
-        self.indent = ' ' * 4
+        self.indent = " " * 4
         # Keywords
         self._latest = latest_prop
         if output_format == self.FORMAT_YAML:
             self._format = self.yaml_format
             self._show_header = True
         elif output_format == self.FORMAT_CLEAN:
             self._format = self.clean_format
             self._show_header = False
 
     def header(self):
         if not self._show_header:
             return ""
-        s = self._format((("Database", self._db.name),
-                          ("Collection", self._coll.name),
-                          ("Values", "")))
-        return s
+        return self._format((("Database", self._db.name), ("Collection", self._coll.name), ("Values", "")))
 
     def stat(self, name):
-        func = 'stat_{}'.format(name)
+        func = f"stat_{name}"
         return getattr(self, func)()
 
     def stat_latest(self):
-        cur = self._coll.find({}, [self._latest])\
-                        .sort(self._latest, -1)\
-                        .limit(1)
+        cur = self._coll.find({}, [self._latest]).sort(self._latest, -1).limit(1)
         try:
-            value = "{}".format(cur[0][self._latest])
+            value = f"{cur[0][self._latest]}"
         except IndexError:
-            _log.error("Cannot get latest value: no records with field '{}'"
-                       .format(self._latest))
+            _log.error(f"Cannot get latest value: no records with field '{self._latest}'")
             return ""
         return self._format([("Latest", value)], depth=1)
 
     def stat_count(self):
-        value = "{:d}".format(self._coll.count())
+        value = f"{self._coll.count():d}"
         return self._format([("Count", value)], depth=1)
 
     def yaml_format(self, data, depth=0):
         rows, ind = [], self.indent * depth
         for k, v in data:
-            rows.append("{i}{k}: {v}".format(i=ind, k=k, v=v))
-        return '\n'.join(rows) + "\n"
+            rows.append(f"{ind}{k}: {v}")
+        return "\n".join(rows) + "\n"
 
     def clean_format(self, data, depth=0):
-        rows = ["{} {}".format(d[0].lower(), d[1]) for d in data]
-        return '\n'.join(rows) + "\n"
+        rows = [f"{d[0].lower()} {d[1]}" for d in data]
+        return "\n".join(rows) + "\n"
 
 
 def db_stats(args):
-    """Database and/or collection statistics.
-    """
+    """Database and/or collection statistics."""
     # Init db.
     cfg = get_settings(args.config_file)
     normalize_userpass(cfg)
     qe = QueryEngine(**cfg)
 
     # Copy stat args and keywords.
     stats, kw = {}, {}
     for k, v in vars(args).iteritems():
         if k.startswith("st_"):
             stats[k[3:]] = v
         else:
             kw[k] = v
 
     # Process 'show all'.
-    if stats['showall']:
+    if stats["showall"]:
         for k in stats.iterkeys():
             stats[k] = True
-    del stats['showall']
+    del stats["showall"]
 
     # Output destination.
     w = sys.stdout
 
     # Run commands.
     cmd = StatsCommands(qe, **kw)
     w.write(cmd.header())
@@ -230,150 +237,204 @@
             w.write(cmd.stat(k))
 
 
 def normalize_userpass(cfg):
     """In DB conn. config, normalize user/password from readonly and admin prefixes.
     In the end, there will be only keys 'user' and 'password'.
     """
-    for pfx in 'readonly', 'admin':  # in reverse order of priority, to overwrite
-        if (pfx + '_user') in cfg and (pfx + '_password') in cfg:
-            cfg[QueryEngine.USER_KEY] = cfg[pfx + '_user']
-            cfg[QueryEngine.PASSWORD_KEY] = cfg[pfx + '_password']
-            del cfg[pfx + '_user']
-            del cfg[pfx + '_password']
+    for pfx in "readonly", "admin":  # in reverse order of priority, to overwrite
+        if (pfx + "_user") in cfg and (pfx + "_password") in cfg:
+            cfg[QueryEngine.USER_KEY] = cfg[pfx + "_user"]
+            cfg[QueryEngine.PASSWORD_KEY] = cfg[pfx + "_password"]
+            del cfg[pfx + "_user"]
+            del cfg[pfx + "_password"]
 
 
 def init_logging(args):
-    """Initialize verbosity
-    """
+    """Initialize verbosity."""
     _log.propagate = False
     hndlr = logging.StreamHandler()
     hndlr.setFormatter(logging.Formatter("[%(levelname)-6s] %(asctime)s %(name)s :: %(message)s"))
     _log.addHandler(hndlr)
-    if 'quiet' in args and args.quiet:
+    if "quiet" in args and args.quiet:
         lvl = logging.CRITICAL
     else:
-        vb = args.vb if 'vb' in args else 0
+        vb = args.vb if "vb" in args else 0
         # Level:  default      -v            -vv
         lvl = (logging.WARN, logging.INFO, logging.DEBUG)[min(vb, 2)]
     _log.setLevel(lvl)
 
 
 if __name__ == "__main__":
     db_file = SETTINGS.get("PMGDB_DB_FILE")
-    parser = argparse.ArgumentParser(description="""
+    parser = argparse.ArgumentParser(
+        description="""
     mgdb is a complete command line db management script for pymatgen-db. It
     provides the facility to insert vasp runs, perform queries, and run a web
     server for exploring databases that you create. Type mgdb -h to see the
     various options.
 
     Author: Shyue Ping Ong
     Version: 3.0
-    Last updated: Mar 23 2013""")
+    Last updated: Mar 23 2013"""
+    )
 
     # Parents for all subparsers.
     parent_vb = argparse.ArgumentParser(add_help=False)
-    parent_vb.add_argument('--quiet', '-q', dest='quiet', action="store_true",
-                           default=False,
-                           help="Minimal verbosity.")
-    parent_vb.add_argument('--verbose', '-v', dest='vb', action="count",
-                           default=0,
-                           help="Print more verbose messages to standard error. "
-                                "Repeatable. (default=ERROR)")
+    parent_vb.add_argument("--quiet", "-q", dest="quiet", action="store_true", default=False, help="Minimal verbosity.")
+    parent_vb.add_argument(
+        "--verbose",
+        "-v",
+        dest="vb",
+        action="count",
+        default=0,
+        help="Print more verbose messages to standard error. Repeatable. (default=ERROR)",
+    )
     parent_cfg = argparse.ArgumentParser(add_help=False)
-    parent_cfg.add_argument("-c", "--config", dest="config_file", type=str,
-                            default=db_file,
-                            help="Config file to use. Generate one using mgdb "
-                            "init --config filename.json if necessary. "
-                            "Otherwise, the code searches for a db.json. If"
-                            "none is found, an no-authentication "
-                            "localhost:27017/vasp database and tasks "
-                            "collection is assumed.")
+    parent_cfg.add_argument(
+        "-c",
+        "--config",
+        dest="config_file",
+        type=str,
+        default=db_file,
+        help="Config file to use. Generate one using mgdb "
+        "init --config filename.json if necessary. "
+        "Otherwise, the code searches for a db.json. If"
+        "none is found, an no-authentication "
+        "localhost:27017/vasp database and tasks "
+        "collection is assumed.",
+    )
 
     # change db_file to the default "db.json" if it does not exist
     db_file = db_file or "db.json"
 
     # Init for all subparsers.
     subparsers = parser.add_subparsers()
 
     # The 'init' subcommand.
-    pinit = subparsers.add_parser("init", help="Initialization tools.",
-                                  parents=[parent_vb])
-    pinit.add_argument("-c", "--config", dest="config_file", type=str,
-                       nargs='?', default=db_file,
-                       help="Creates an db config file for the database. "
-                            "Default filename is db.json.")
+    pinit = subparsers.add_parser("init", help="Initialization tools.", parents=[parent_vb])
+    pinit.add_argument(
+        "-c",
+        "--config",
+        dest="config_file",
+        type=str,
+        nargs="?",
+        default=db_file,
+        help="Creates an db config file for the database. Default filename is db.json.",
+    )
     pinit.set_defaults(func=init_db)
 
     popt = subparsers.add_parser("optimize", help="Optimization tools.")
 
-    popt.add_argument("-c", "--config", dest="config_file", type=str,
-                      nargs='?', default=db_file,
-                      help="Creates an db config file for the database. "
-                           "Default filename is db.json.")
+    popt.add_argument(
+        "-c",
+        "--config",
+        dest="config_file",
+        type=str,
+        nargs="?",
+        default=db_file,
+        help="Creates an db config file for the database. Default filename is db.json.",
+    )
     popt.set_defaults(func=optimize_indexes)
 
     # The 'insert' subcommand.
-    pinsert = subparsers.add_parser("insert", help="Insert vasp runs.",
-                                    parents=[parent_vb, parent_cfg])
-    pinsert.add_argument("directory", metavar="directory", type=str,
-                         default=".", help="Root directory for runs.")
-    pinsert.add_argument("-l", "--logfile", dest="logfile", type=str,
-                         help="File to log db insertion. Defaults to stdout.")
-    pinsert.add_argument("-t", "--tag", dest="tag", type=str, nargs="+",
-                         default=[],
-                         help="Tag your runs for easier search."
-                              " Accepts multiple space-separated tags. E.g.,"
-                              " '--tag metal energy'")
-    pinsert.add_argument("-f", "--force", dest="force_update_dupes",
-                         action="store_true",
-                         help="Force update duplicates. This forces the "
-                              "analyzer to reanalyze already inserted data.")
-    pinsert.add_argument("-d", "--parse_dos", dest="parse_dos",
-                         action="store_true",
-                         help="Whether to parse the dos.")
-    pinsert.add_argument("-a", "--author", dest="author", type=str, nargs=1,
-                         default=None,
-                         help="Enter a *unique* author field so that you can "
-                              "trace back what you ran.")
-    pinsert.add_argument("-n", "--ncpus", dest="ncpus", type=int,
-                         default=None,
-                         help="Number of CPUs to use in inserting. If "
-                              "not specified, multiprocessing will use "
-                              "the number of cpus detected.")
+    pinsert = subparsers.add_parser("insert", help="Insert vasp runs.", parents=[parent_vb, parent_cfg])
+    pinsert.add_argument("directory", metavar="directory", type=str, default=".", help="Root directory for runs.")
+    pinsert.add_argument(
+        "-l", "--logfile", dest="logfile", type=str, help="File to log db insertion. Defaults to stdout."
+    )
+    pinsert.add_argument(
+        "-t",
+        "--tag",
+        dest="tag",
+        type=str,
+        nargs="+",
+        default=[],
+        help="Tag your runs for easier search. Accepts multiple space-separated tags. E.g., '--tag metal energy'",
+    )
+    pinsert.add_argument(
+        "-f",
+        "--force",
+        dest="force_update_dupes",
+        action="store_true",
+        help="Force update duplicates. This forces the analyzer to reanalyze already inserted data.",
+    )
+    pinsert.add_argument("-d", "--parse_dos", dest="parse_dos", action="store_true", help="Whether to parse the dos.")
+    pinsert.add_argument(
+        "-a",
+        "--author",
+        dest="author",
+        type=str,
+        nargs=1,
+        default=None,
+        help="Enter a *unique* author field so that you can trace back what you ran.",
+    )
+    pinsert.add_argument(
+        "-n",
+        "--ncpus",
+        dest="ncpus",
+        type=int,
+        default=None,
+        help="Number of CPUs to use in inserting. If "
+        "not specified, multiprocessing will use "
+        "the number of cpus detected.",
+    )
     pinsert.set_defaults(func=update_db)
 
     # The 'query' subcommand.
-    pquery = subparsers.add_parser("query",
-                                   help="Query tools. Requires the "
-                                        "use of pretty_table.",
-                                   parents=[parent_vb, parent_cfg])
-    pquery.add_argument("--crit", dest="criteria", type=str, default=None,
-                        help="Query criteria in typical json format. E.g., "
-                             "{\"task_id\": 1}.")
-    pquery.add_argument("--props", dest="properties", type=str, default=[],
-                        nargs='+', required=True,
-                        help="Desired properties. Repeatable. E.g., pretty_formula, "
-                             "task_id, energy...")
-    pquery.add_argument("--dump", dest="dump_json", action='store_true', default=False,
-                        help="Simply dump results to JSON instead of a tabular view")
+    pquery = subparsers.add_parser(
+        "query", help="Query tools. Requires the use of pretty_table.", parents=[parent_vb, parent_cfg]
+    )
+    pquery.add_argument(
+        "--crit",
+        dest="criteria",
+        type=str,
+        default=None,
+        help="Query criteria in typical json format. E.g., " '{"task_id": 1}.',
+    )
+    pquery.add_argument(
+        "--props",
+        dest="properties",
+        type=str,
+        default=[],
+        nargs="+",
+        required=True,
+        help="Desired properties. Repeatable. E.g., pretty_formula, task_id, energy...",
+    )
+    pquery.add_argument(
+        "--dump",
+        dest="dump_json",
+        action="store_true",
+        default=False,
+        help="Simply dump results to JSON instead of a tabular view",
+    )
     pquery.set_defaults(func=query_db)
 
     # The 'stats' subcommand.
-    pstats = subparsers.add_parser("stats", help="Database and/or collection statistics.",
-                                   parents=[parent_vb, parent_cfg])
+    pstats = subparsers.add_parser(
+        "stats", help="Database and/or collection statistics.", parents=[parent_vb, parent_cfg]
+    )
     pstats.add_argument("--count", help="Show count of records", dest="st_count", action="store_true")
     pstats.add_argument("--latest", help="Show time of latest record", dest="st_latest", action="store_true")
-    #pstats.add_argument("--size", help="Show min/max/avg/total record sizes", dest="", action="store_true")
+    # pstats.add_argument("--size", help="Show min/max/avg/total record sizes", dest="", action="store_true")
     pstats.add_argument("--all", help="Show all stats", dest="st_showall", action="store_true")
-    pstats.add_argument("--latest-prop", help="Property to use for latest record (default='updated_at')",
-                        default="updated_at", dest="latest_prop")
-    pstats.add_argument("-f", "--format", help="Output format", choices=[StatsCommands.FORMAT_YAML,
-                                                                         StatsCommands.FORMAT_CLEAN],
-                        default="yaml", dest="output_format")
+    pstats.add_argument(
+        "--latest-prop",
+        help="Property to use for latest record (default='updated_at')",
+        default="updated_at",
+        dest="latest_prop",
+    )
+    pstats.add_argument(
+        "-f",
+        "--format",
+        help="Output format",
+        choices=[StatsCommands.FORMAT_YAML, StatsCommands.FORMAT_CLEAN],
+        default="yaml",
+        dest="output_format",
+    )
     pstats.set_defaults(func=db_stats)
 
     # Parse args
     args = parser.parse_args()
 
     init_logging(args)
```

### Comparing `pymatgen-db-2023.2.23/setup.py` & `pymatgen-db-2023.7.18/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # Copyright (c) Pymatgen Development Team.
 # Distributed under the terms of the MIT License.
+"""Setup file for pymatgen-db."""
+from __future__ import annotations
 
 import os
 
-from setuptools import setup, find_namespace_packages
+from setuptools import find_namespace_packages, setup
 
 with open("README.rst") as f:
     long_desc = f.read()
 
 setup(
     name="pymatgen-db",
     packages=find_namespace_packages(include=["pymatgen.*"]),
-    version="2023.2.23",
+    version="2023.7.18",
     setup_requires=["numpy"],
     install_requires=["pymatgen>=2022.0.3", "monty>=0.9.6", "pymongo>=2.8"],
-    extras_require={
-        'tests': 'mongomock'
-    },
+    extras_require={"tests": "mongomock"},
     package_data={"pymatgen": ["db/*.json"]},
     include_package_data=True,
     author="Shyue Ping Ong",
     author_email="shyuep@gmail.com",
     maintainer="Shyue Ping Ong",
     maintainer_email="shyuep@gmail.com",
     url="https://github.com/materialsproject/pymatgen-db",
     license="MIT",
     description="Pymatgen-db is a database add-on for the Python Materials "
-                "Genomics (pymatgen) materials analysis library.",
+    "Genomics (pymatgen) materials analysis library.",
     long_description=long_desc,
-    keywords=["vasp", "gaussian", "materials", "project", "electronic",
-              "structure", "mongo"],
+    keywords=["vasp", "gaussian", "materials", "project", "electronic", "structure", "mongo"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Database"
+        "Topic :: Database",
     ],
-    scripts=[os.path.join("scripts", f) for f in os.listdir("scripts")
-             if not os.path.isdir(os.path.join("scripts", f))]
-)
+    scripts=[
+        os.path.join("scripts", f) for f in os.listdir("scripts") if not os.path.isdir(os.path.join("scripts", f))
+    ],
+)
```

