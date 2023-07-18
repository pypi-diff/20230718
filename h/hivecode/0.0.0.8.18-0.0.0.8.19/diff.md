# Comparing `tmp/hivecode-0.0.0.8.18.tar.gz` & `tmp/hivecode-0.0.0.8.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivecode-0.0.0.8.18.tar", last modified: Mon May  8 01:39:15 2023, max compression
+gzip compressed data, was "hivecode-0.0.0.8.19.tar", last modified: Tue Jul 18 05:08:33 2023, max compression
```

## Comparing `hivecode-0.0.0.8.18.tar` & `hivecode-0.0.0.8.19.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.060758 hivecode-0.0.0.8.18/
--rw-rw-rw-   0        0        0     3946 2023-05-08 01:39:15.061267 hivecode-0.0.0.8.18/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.18/README.rst
--rw-rw-rw-   0        0        0     1387 2023-05-08 01:39:03.000000 hivecode-0.0.0.8.18/pyproject.toml
--rw-rw-rw-   0        0        0      185 2023-02-13 02:12:12.000000 hivecode-0.0.0.8.18/requirements.txt
--rw-rw-rw-   0        0        0     1304 2023-05-08 01:39:15.067310 hivecode-0.0.0.8.18/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.015698 hivecode-0.0.0.8.18/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.026787 hivecode-0.0.0.8.18/src/hiveadb/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hiveadb/__init__.py
--rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.18/src/hiveadb/eda.py
--rw-rw-rw-   0        0        0    11311 2023-04-12 03:58:56.000000 hivecode-0.0.0.8.18/src/hiveadb/function.py
--rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.18/src/hiveadb/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hiveadb/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.042371 hivecode-0.0.0.8.18/src/hivecode.egg-info/
--rw-rw-rw-   0        0        0     3946 2023-05-08 01:39:14.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      747 2023-05-08 01:39:15.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 01:39:14.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 01:34:18.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      275 2023-05-08 01:39:14.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-05-08 01:39:14.000000 hivecode-0.0.0.8.18/src/hivecode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.054748 hivecode-0.0.0.8.18/src/hivecore/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivecore/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.18/src/hivecore/constant.py
--rw-rw-rw-   0        0        0     9275 2023-04-24 04:05:22.000000 hivecode-0.0.0.8.18/src/hivecore/decorator.py
--rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.18/src/hivecore/eda.py
--rw-rw-rw-   0        0        0     4261 2023-05-08 01:08:47.000000 hivecode-0.0.0.8.18/src/hivecore/function.py
--rw-rw-rw-   0        0        0     1617 2023-04-12 05:20:34.000000 hivecode-0.0.0.8.18/src/hivecore/pattern.py
--rw-rw-rw-   0        0        0    29856 2023-04-12 03:24:52.000000 hivecode-0.0.0.8.18/src/hivecore/preprocess.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivecore/py.typed
--rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.18/src/hivecore/visual.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:39:15.059745 hivecode-0.0.0.8.18/src/hivesignal/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/analysis.py
--rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/eda.py
--rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/py.typed
--rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.18/src/hivesignal/transform.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.675951 hivecode-0.0.0.8.19/
+-rw-rw-rw-   0        0        0     3790 2023-07-18 05:08:33.676456 hivecode-0.0.0.8.19/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.19/README.rst
+-rw-rw-rw-   0        0        0     1402 2023-07-18 05:08:24.000000 hivecode-0.0.0.8.19/pyproject.toml
+-rw-rw-rw-   0        0        0      184 2023-07-17 06:05:11.000000 hivecode-0.0.0.8.19/requirements.txt
+-rw-rw-rw-   0        0        0     1181 2023-07-18 05:08:33.676957 hivecode-0.0.0.8.19/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.640816 hivecode-0.0.0.8.19/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.649861 hivecode-0.0.0.8.19/src/hiveadb/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hiveadb/__init__.py
+-rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.19/src/hiveadb/eda.py
+-rw-rw-rw-   0        0        0    11311 2023-04-12 03:58:56.000000 hivecode-0.0.0.8.19/src/hiveadb/function.py
+-rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.19/src/hiveadb/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hiveadb/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.661868 hivecode-0.0.0.8.19/src/hivecode.egg-info/
+-rw-rw-rw-   0        0        0     3790 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      274 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.669912 hivecode-0.0.0.8.19/src/hivecore/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivecore/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.19/src/hivecore/constant.py
+-rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.19/src/hivecore/decorator.py
+-rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.19/src/hivecore/eda.py
+-rw-rw-rw-   0        0        0     4261 2023-05-08 01:08:47.000000 hivecode-0.0.0.8.19/src/hivecore/function.py
+-rw-rw-rw-   0        0        0    32125 2023-07-16 07:35:55.000000 hivecode-0.0.0.8.19/src/hivecore/patterns.py
+-rw-rw-rw-   0        0        0    29856 2023-04-12 03:24:52.000000 hivecode-0.0.0.8.19/src/hivecore/preprocess.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivecore/py.typed
+-rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.19/src/hivecore/visual.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.674946 hivecode-0.0.0.8.19/src/hivesignal/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/analysis.py
+-rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/eda.py
+-rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/py.typed
+-rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.18/PKG-INFO` & `hivecode-0.0.0.8.19/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.18
+Version: 0.0.0.8.19
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: dev
 
 .. |PyPI version Hivecode| image:: https://img.shields.io/pypi/v/hivecode.svg
    :target: https://pypi.org/project/hivecode/
```

### Comparing `hivecode-0.0.0.8.18/README.rst` & `hivecode-0.0.0.8.19/README.rst`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/pyproject.toml` & `hivecode-0.0.0.8.19/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "hivecode"
 description = "Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell."
-version = "0.0.0.8.18"
+version = "0.0.0.8.19"
 requires-python = ">=3.8.0"
 readme = "README.rst"
 authors = [
     {name = "Juan Manuel Mejía Botero", email="juanmam941025@gmail.com"},
     {name = "Sebastian López Valencia", email="sebaslv12@hotmail.com"}
 ]
 
-dynamic = ["dependencies"]
+dynamic = ["dependencies", "classifiers"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 
 [project.optional-dependencies]
 dev = [
     "build",
```

### Comparing `hivecode-0.0.0.8.18/setup.cfg` & `hivecode-0.0.0.8.19/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -25,58 +25,50 @@
 00000180: 616e 204d 616e 7565 6c20 4d65 6ac3 ad61  an Manuel Mej..a
 00000190: 2042 6f74 6572 6f0d 0a70 6c61 7466 6f72   Botero..platfor
 000001a0: 6d73 203d 2075 6e69 782c 206c 696e 7578  ms = unix, linux
 000001b0: 2c20 6f73 782c 2063 7967 7769 6e2c 2077  , osx, cygwin, w
 000001c0: 696e 3332 0d0a 636c 6173 7369 6669 6572  in32..classifier
 000001d0: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
 000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001f0: 7974 686f 6e20 3a3a 2033 0d0a 0950 726f  ython :: 3...Pro
-00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000220: 203a 3a20 4f6e 6c79 0d0a 0950 726f 6772   :: Only...Progr
-00000230: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000240: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-00000250: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000260: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000270: 6e20 3a3a 2033 2e39 0d0a 0950 726f 6772  n :: 3.9...Progr
-00000280: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000290: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-000002a0: 300d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  0....[options]..
-000002b0: 7061 636b 6167 6573 203d 200d 0a09 6869  packages = ...hi
-000002c0: 7665 636f 7265 0d0a 0968 6976 6561 6462  vecore...hiveadb
-000002d0: 0d0a 0968 6976 6573 6967 6e61 6c0d 0a70  ...hivesignal..p
-000002e0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-000002f0: 203e 3d33 2e38 2e30 0d0a 696e 7374 616c   >=3.8.0..instal
-00000300: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-00000310: 7061 7261 6d69 6b6f 3d3d 322e 3131 2e30  paramiko==2.11.0
-00000320: 0d0a 0973 6370 3e3d 302e 3134 2e34 0d0a  ...scp>=0.14.4..
-00000330: 0973 6b6c 6561 726e 3e3d 302e 3234 2e31  .sklearn>=0.24.1
-00000340: 0d0a 0961 7a75 7265 2d63 6f73 6d6f 733e  ...azure-cosmos>
-00000350: 3d34 2e33 2e30 0d0a 096f 7065 6e70 7978  =4.3.0...openpyx
-00000360: 6c3e 3d33 2e30 2e31 300d 0a09 7471 646d  l>=3.0.10...tqdm
-00000370: 3e3d 342e 3634 2e31 0d0a 0973 6369 7079  >=4.64.1...scipy
-00000380: 3e3d 312e 362e 320d 0a09 6d61 7470 6c6f  >=1.6.2...matplo
-00000390: 746c 6962 3e3d 332e 342e 320d 0a09 6e75  tlib>=3.4.2...nu
-000003a0: 6d70 793e 3d31 2e32 302e 310d 0a09 7061  mpy>=1.20.1...pa
-000003b0: 6e64 6173 3e3d 312e 322e 340d 0a09 7365  ndas>=1.2.4...se
-000003c0: 6162 6f72 6e3e 3d30 2e31 312e 310d 0a09  aborn>=0.11.1...
-000003d0: 6b6f 616c 6173 0d0a 7061 636b 6167 655f  koalas..package_
-000003e0: 6469 7220 3d20 0d0a 093d 2073 7263 0d0a  dir = ...= src..
-000003f0: 7a69 705f 7361 6665 203d 206e 6f0d 0a0d  zip_safe = no...
-00000400: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
-00000410: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
-00000420: 6e67 203d 200d 0a09 7079 7465 7374 3e3d  ng = ...pytest>=
-00000430: 362e 300d 0a09 7079 7465 7374 2d63 6f76  6.0...pytest-cov
-00000440: 3e3d 322e 300d 0a09 6d79 7079 3e3d 302e  >=2.0...mypy>=0.
-00000450: 3931 300d 0a09 666c 616b 6538 3e3d 332e  910...flake8>=3.
-00000460: 390d 0a09 746f 783e 3d33 2e32 340d 0a0d  9...tox>=3.24...
-00000470: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000480: 655f 6461 7461 5d0d 0a68 6976 6563 6f72  e_data]..hivecor
-00000490: 6520 3d20 7079 2e74 7970 6564 0d0a 6869  e = py.typed..hi
-000004a0: 7665 6164 6220 3d20 7079 2e74 7970 6564  veadb = py.typed
-000004b0: 0d0a 6869 7665 7369 676e 616c 203d 2070  ..hivesignal = p
-000004c0: 792e 7479 7065 640d 0a0d 0a5b 666c 616b  y.typed....[flak
-000004d0: 6538 5d0d 0a6d 6178 2d6c 696e 652d 6c65  e8]..max-line-le
-000004e0: 6e67 7468 203d 2031 3630 0d0a 0d0a 5b65  ngth = 160....[e
-000004f0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000500: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000510: 203d 2030 0d0a 0d0a                       = 0....
+000001f0: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+00000200: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000210: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000220: 3a20 332e 3131 0d0a 0d0a 5b6f 7074 696f  : 3.11....[optio
+00000230: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
+00000240: 0d0a 0968 6976 6563 6f72 650d 0a09 6869  ...hivecore...hi
+00000250: 7665 6164 620d 0a09 6869 7665 7369 676e  veadb...hivesign
+00000260: 616c 0d0a 7079 7468 6f6e 5f72 6571 7569  al..python_requi
+00000270: 7265 7320 3d20 3e3d 332e 382e 300d 0a69  res = >=3.8.0..i
+00000280: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+00000290: 3d20 0d0a 0970 6172 616d 696b 6f3d 3d32  = ...paramiko==2
+000002a0: 2e31 312e 300d 0a09 7363 703e 3d30 2e31  .11.0...scp>=0.1
+000002b0: 342e 340d 0a09 736b 6c65 6172 6e3e 3d30  4.4...sklearn>=0
+000002c0: 2e32 342e 310d 0a09 617a 7572 652d 636f  .24.1...azure-co
+000002d0: 736d 6f73 3e3d 342e 332e 300d 0a09 6f70  smos>=4.3.0...op
+000002e0: 656e 7079 786c 3e3d 332e 302e 3130 0d0a  enpyxl>=3.0.10..
+000002f0: 0974 7164 6d3e 3d34 2e36 342e 310d 0a09  .tqdm>=4.64.1...
+00000300: 7363 6970 793e 3d31 2e36 2e32 0d0a 096d  scipy>=1.6.2...m
+00000310: 6174 706c 6f74 6c69 623e 3d33 2e34 2e32  atplotlib>=3.4.2
+00000320: 0d0a 096e 756d 7079 3e3d 312e 3230 2e31  ...numpy>=1.20.1
+00000330: 0d0a 0970 616e 6461 733e 3d31 2e32 2e34  ...pandas>=1.2.4
+00000340: 0d0a 0973 6561 626f 726e 3e3d 302e 3131  ...seaborn>=0.11
+00000350: 2e31 0d0a 096b 6f61 6c61 730d 0a70 6163  .1...koalas..pac
+00000360: 6b61 6765 5f64 6972 203d 200d 0a09 3d20  kage_dir = ...= 
+00000370: 7372 630d 0a7a 6970 5f73 6166 6520 3d20  src..zip_safe = 
+00000380: 6e6f 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  no....[options.e
+00000390: 7874 7261 735f 7265 7175 6972 655d 0d0a  xtras_require]..
+000003a0: 7465 7374 696e 6720 3d20 0d0a 0970 7974  testing = ...pyt
+000003b0: 6573 743e 3d36 2e30 0d0a 0970 7974 6573  est>=6.0...pytes
+000003c0: 742d 636f 763e 3d32 2e30 0d0a 096d 7970  t-cov>=2.0...myp
+000003d0: 793e 3d30 2e39 3130 0d0a 0966 6c61 6b65  y>=0.910...flake
+000003e0: 383e 3d33 2e39 0d0a 0974 6f78 3e3d 332e  8>=3.9...tox>=3.
+000003f0: 3234 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  24....[options.p
+00000400: 6163 6b61 6765 5f64 6174 615d 0d0a 6869  ackage_data]..hi
+00000410: 7665 636f 7265 203d 2070 792e 7479 7065  vecore = py.type
+00000420: 640d 0a68 6976 6561 6462 203d 2070 792e  d..hiveadb = py.
+00000430: 7479 7065 640d 0a68 6976 6573 6967 6e61  typed..hivesigna
+00000440: 6c20 3d20 7079 2e74 7970 6564 0d0a 0d0a  l = py.typed....
+00000450: 5b66 6c61 6b65 385d 0d0a 6d61 782d 6c69  [flake8]..max-li
+00000460: 6e65 2d6c 656e 6774 6820 3d20 3136 300d  ne-length = 160.
+00000470: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000480: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000490: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `hivecode-0.0.0.8.18/src/hiveadb/eda.py` & `hivecode-0.0.0.8.19/src/hiveadb/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hiveadb/function.py` & `hivecode-0.0.0.8.19/src/hiveadb/function.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hiveadb/io.py` & `hivecode-0.0.0.8.19/src/hiveadb/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hivecode.egg-info/PKG-INFO` & `hivecode-0.0.0.8.19/src/hivecode.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.18
+Version: 0.0.0.8.19
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: dev
 
 .. |PyPI version Hivecode| image:: https://img.shields.io/pypi/v/hivecode.svg
    :target: https://pypi.org/project/hivecode/
```

### Comparing `hivecode-0.0.0.8.18/src/hivecode.egg-info/SOURCES.txt` & `hivecode-0.0.0.8.19/src/hivecode.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 src/hivecode.egg-info/requires.txt
 src/hivecode.egg-info/top_level.txt
 src/hivecore/__init__.py
 src/hivecore/constant.py
 src/hivecore/decorator.py
 src/hivecore/eda.py
 src/hivecore/function.py
-src/hivecore/pattern.py
+src/hivecore/patterns.py
 src/hivecore/preprocess.py
 src/hivecore/py.typed
 src/hivecore/visual.py
 src/hivesignal/__init__.py
 src/hivesignal/analysis.py
 src/hivesignal/eda.py
 src/hivesignal/io.py
```

### Comparing `hivecode-0.0.0.8.18/src/hivecore/constant.py` & `hivecode-0.0.0.8.19/src/hivecore/constant.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hivecore/decorator.py` & `hivecode-0.0.0.8.19/src/hivecore/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,33 +6,14 @@
 from time import time, sleep, perf_counter
 from typing import List, Tuple, Union, Any, Callable
 
 """
 The hivecore.decorator module includes multiple decorators that can be used to enhance classes and functions.
 """
 
-def singleton( class_: type ) -> object:
-    """
-    A decorator used to turn a class into a Singleton. This makes it so that if a class has already been instanciated one, that instance will be returned instead of a second one.
-
-    :param class_: A class to apply the singleton to. Applied as a Decorator.
-    :type class_: Class
-    :return: Singleton instance of that Class.
-    :rtype: Object
-    """
-    instances = {}
-
-    @wraps(class_)
-    def getinstance(*args, **kwargs):
-        if class_ not in instances:
-            instances[class_] = class_(*args, **kwargs)
-        return instances[class_]
-
-    return getinstance
-
 
 def timer(in_milis: bool = True) -> Tuple[any, float]:
     """
     A decorator that can measure how long a function takes to run.
     
     :param in_milis: A flag to determine if the result should be returned as milis or in seconds. Default: False 
     :type in_milis: Optional[bool], optional
@@ -258,7 +239,28 @@
             key = kwargs.get(key_param)
             if not key or key in used_keys:
                 raise ValueError("Invalid key or key already used.")
             used_keys.add(key)
             return func(*args, **kwargs)
         return wrapper
     return decorator
+
+
+@deprecated("Singleton decorator has been moved to hivecore.patterns and will only be available there in future versions.")
+def singleton( class_: type ) -> object:
+    """
+    A decorator used to turn a class into a Singleton. This makes it so that if a class has already been instanciated one, that instance will be returned instead of a second one.
+
+    :param class_: A class to apply the singleton to. Applied as a Decorator.
+    :type class_: Class
+    :return: Singleton instance of that Class.
+    :rtype: Object
+    """
+    instances = {}
+
+    @wraps(class_)
+    def getinstance(*args, **kwargs):
+        if class_ not in instances:
+            instances[class_] = class_(*args, **kwargs)
+        return instances[class_]
+
+    return getinstance
```

### Comparing `hivecode-0.0.0.8.18/src/hivecore/eda.py` & `hivecode-0.0.0.8.19/src/hivecore/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hivecore/function.py` & `hivecode-0.0.0.8.19/src/hivecore/function.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hivecore/preprocess.py` & `hivecode-0.0.0.8.19/src/hivecore/preprocess.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hivecore/visual.py` & `hivecode-0.0.0.8.19/src/hivecore/visual.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hivesignal/analysis.py` & `hivecode-0.0.0.8.19/src/hivesignal/analysis.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hivesignal/io.py` & `hivecode-0.0.0.8.19/src/hivesignal/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.18/src/hivesignal/transform.py` & `hivecode-0.0.0.8.19/src/hivesignal/transform.py`

 * *Files identical despite different names*

