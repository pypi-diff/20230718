# Comparing `tmp/kshell-utilities-1.5.0.0.tar.gz` & `tmp/kshell-utilities-1.5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kshell-utilities-1.5.0.0.tar", last modified: Tue Jul 18 09:08:00 2023, max compression
+gzip compressed data, was "kshell-utilities-1.5.0.1.tar", last modified: Tue Jul 18 09:19:45 2023, max compression
```

## Comparing `kshell-utilities-1.5.0.0.tar` & `kshell-utilities-1.5.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:08:00.517451 kshell-utilities-1.5.0.0/
--rw-r--r--   0 jon        (501) staff       (20)     1077 2021-09-29 15:16:13.000000 kshell-utilities-1.5.0.0/LICENSE
--rw-r--r--   0 jon        (501) staff       (20)      588 2023-07-18 09:08:00.517127 kshell-utilities-1.5.0.0/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      904 2023-03-30 08:04:36.000000 kshell-utilities-1.5.0.0/README.md
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:08:00.512060 kshell-utilities-1.5.0.0/kshell_utilities/
--rw-r--r--   0 jon        (501) staff       (20)      708 2023-07-14 08:53:01.000000 kshell-utilities-1.5.0.0/kshell_utilities/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)    33280 2022-09-18 11:42:03.000000 kshell-utilities-1.5.0.0/kshell_utilities/collect_logs.py
--rw-r--r--   0 jon        (501) staff       (20)    10820 2023-07-14 09:10:01.000000 kshell-utilities-1.5.0.0/kshell_utilities/compare.py
--rw-r--r--   0 jon        (501) staff       (20)    13139 2023-07-14 09:08:52.000000 kshell-utilities-1.5.0.0/kshell_utilities/count_dim.py
--rw-r--r--   0 jon        (501) staff       (20)     6302 2023-07-14 08:53:22.000000 kshell-utilities-1.5.0.0/kshell_utilities/data_structures.py
--rw-r--r--   0 jon        (501) staff       (20)     1751 2022-05-26 10:28:32.000000 kshell-utilities-1.5.0.0/kshell_utilities/deprecated.py
--rw-r--r--   0 jon        (501) staff       (20)    51983 2023-07-14 08:55:38.000000 kshell-utilities-1.5.0.0/kshell_utilities/general_utilities.py
--rw-r--r--   0 jon        (501) staff       (20)      125 2021-10-13 13:01:44.000000 kshell-utilities-1.5.0.0/kshell_utilities/kshell_exceptions.py
--rw-r--r--   0 jon        (501) staff       (20)   106779 2023-07-17 03:34:31.000000 kshell-utilities-1.5.0.0/kshell_utilities/kshell_utilities.py
--rw-r--r--   0 jon        (501) staff       (20)    42408 2021-04-14 10:39:16.000000 kshell-utilities-1.5.0.0/kshell_utilities/kshell_utilities_tmp.py
--rw-r--r--   0 jon        (501) staff       (20)    34975 2023-07-14 09:03:44.000000 kshell-utilities-1.5.0.0/kshell_utilities/loaders.py
--rw-r--r--   0 jon        (501) staff       (20)      563 2023-03-30 07:57:17.000000 kshell-utilities-1.5.0.0/kshell_utilities/other_tools.py
--rw-r--r--   0 jon        (501) staff       (20)     4853 2023-07-14 08:54:55.000000 kshell-utilities-1.5.0.0/kshell_utilities/parameters.py
--rw-r--r--   0 jon        (501) staff       (20)     8086 2023-07-14 09:11:24.000000 kshell-utilities-1.5.0.0/kshell_utilities/partition_compare.py
--rw-r--r--   0 jon        (501) staff       (20)    87644 2023-07-14 08:53:46.000000 kshell-utilities-1.5.0.0/kshell_utilities/partition_editor.py
--rw-r--r--   0 jon        (501) staff       (20)     9036 2023-07-14 09:02:39.000000 kshell-utilities-1.5.0.0/kshell_utilities/partition_tools.py
--rw-r--r--   0 jon        (501) staff       (20)    10587 2023-07-14 09:10:36.000000 kshell-utilities-1.5.0.0/kshell_utilities/script_editing.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:08:00.513899 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)      588 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      916 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)       41 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)       23 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/top_level.txt
--rw-r--r--   0 jon        (501) staff       (20)      103 2021-09-29 18:32:05.000000 kshell-utilities-1.5.0.0/pyproject.toml
--rw-r--r--   0 jon        (501) staff       (20)       38 2023-07-18 09:08:00.517560 kshell-utilities-1.5.0.0/setup.cfg
--rw-r--r--   0 jon        (501) staff       (20)      988 2023-07-14 08:39:09.000000 kshell-utilities-1.5.0.0/setup.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:08:00.516327 kshell-utilities-1.5.0.0/tests/
--rw-r--r--   0 jon        (501) staff       (20)        0 2021-05-04 13:07:04.000000 kshell-utilities-1.5.0.0/tests/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)    18919 2023-03-22 04:07:31.000000 kshell-utilities-1.5.0.0/tests/test_all.py
--rw-r--r--   0 jon        (501) staff       (20)     6091 2023-03-31 05:09:49.000000 kshell-utilities-1.5.0.0/tests/test_partition_editor.py
--rw-r--r--   0 jon        (501) staff       (20)     1327 2023-03-22 04:07:31.000000 kshell-utilities-1.5.0.0/tests/test_spin_parity_list.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:19:45.776361 kshell-utilities-1.5.0.1/
+-rw-r--r--   0 jon        (501) staff       (20)     1077 2021-09-29 15:16:13.000000 kshell-utilities-1.5.0.1/LICENSE
+-rw-r--r--   0 jon        (501) staff       (20)      588 2023-07-18 09:19:45.776118 kshell-utilities-1.5.0.1/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      904 2023-03-30 08:04:36.000000 kshell-utilities-1.5.0.1/README.md
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:19:45.771330 kshell-utilities-1.5.0.1/kshell_utilities/
+-rw-r--r--   0 jon        (501) staff       (20)      708 2023-07-18 09:18:49.000000 kshell-utilities-1.5.0.1/kshell_utilities/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)    33280 2022-09-18 11:42:03.000000 kshell-utilities-1.5.0.1/kshell_utilities/collect_logs.py
+-rw-r--r--   0 jon        (501) staff       (20)    10820 2023-07-14 09:10:01.000000 kshell-utilities-1.5.0.1/kshell_utilities/compare.py
+-rw-r--r--   0 jon        (501) staff       (20)    13139 2023-07-14 09:08:52.000000 kshell-utilities-1.5.0.1/kshell_utilities/count_dim.py
+-rw-r--r--   0 jon        (501) staff       (20)     6302 2023-07-14 08:53:22.000000 kshell-utilities-1.5.0.1/kshell_utilities/data_structures.py
+-rw-r--r--   0 jon        (501) staff       (20)     1751 2022-05-26 10:28:32.000000 kshell-utilities-1.5.0.1/kshell_utilities/deprecated.py
+-rw-r--r--   0 jon        (501) staff       (20)    51983 2023-07-14 08:55:38.000000 kshell-utilities-1.5.0.1/kshell_utilities/general_utilities.py
+-rw-r--r--   0 jon        (501) staff       (20)      125 2021-10-13 13:01:44.000000 kshell-utilities-1.5.0.1/kshell_utilities/kshell_exceptions.py
+-rw-r--r--   0 jon        (501) staff       (20)   106815 2023-07-18 09:14:23.000000 kshell-utilities-1.5.0.1/kshell_utilities/kshell_utilities.py
+-rw-r--r--   0 jon        (501) staff       (20)    42408 2021-04-14 10:39:16.000000 kshell-utilities-1.5.0.1/kshell_utilities/kshell_utilities_tmp.py
+-rw-r--r--   0 jon        (501) staff       (20)    34975 2023-07-14 09:03:44.000000 kshell-utilities-1.5.0.1/kshell_utilities/loaders.py
+-rw-r--r--   0 jon        (501) staff       (20)      563 2023-03-30 07:57:17.000000 kshell-utilities-1.5.0.1/kshell_utilities/other_tools.py
+-rw-r--r--   0 jon        (501) staff       (20)     4853 2023-07-14 08:54:55.000000 kshell-utilities-1.5.0.1/kshell_utilities/parameters.py
+-rw-r--r--   0 jon        (501) staff       (20)     8086 2023-07-14 09:11:24.000000 kshell-utilities-1.5.0.1/kshell_utilities/partition_compare.py
+-rw-r--r--   0 jon        (501) staff       (20)    87644 2023-07-14 08:53:46.000000 kshell-utilities-1.5.0.1/kshell_utilities/partition_editor.py
+-rw-r--r--   0 jon        (501) staff       (20)     9036 2023-07-14 09:02:39.000000 kshell-utilities-1.5.0.1/kshell_utilities/partition_tools.py
+-rw-r--r--   0 jon        (501) staff       (20)    10587 2023-07-14 09:10:36.000000 kshell-utilities-1.5.0.1/kshell_utilities/script_editing.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:19:45.773655 kshell-utilities-1.5.0.1/kshell_utilities.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)      588 2023-07-18 09:19:45.000000 kshell-utilities-1.5.0.1/kshell_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      916 2023-07-18 09:19:45.000000 kshell-utilities-1.5.0.1/kshell_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2023-07-18 09:19:45.000000 kshell-utilities-1.5.0.1/kshell_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)       41 2023-07-18 09:19:45.000000 kshell-utilities-1.5.0.1/kshell_utilities.egg-info/requires.txt
+-rw-r--r--   0 jon        (501) staff       (20)       23 2023-07-18 09:19:45.000000 kshell-utilities-1.5.0.1/kshell_utilities.egg-info/top_level.txt
+-rw-r--r--   0 jon        (501) staff       (20)      103 2021-09-29 18:32:05.000000 kshell-utilities-1.5.0.1/pyproject.toml
+-rw-r--r--   0 jon        (501) staff       (20)       38 2023-07-18 09:19:45.776448 kshell-utilities-1.5.0.1/setup.cfg
+-rw-r--r--   0 jon        (501) staff       (20)      988 2023-07-18 09:19:15.000000 kshell-utilities-1.5.0.1/setup.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:19:45.775460 kshell-utilities-1.5.0.1/tests/
+-rw-r--r--   0 jon        (501) staff       (20)        0 2021-05-04 13:07:04.000000 kshell-utilities-1.5.0.1/tests/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)    18919 2023-03-22 04:07:31.000000 kshell-utilities-1.5.0.1/tests/test_all.py
+-rw-r--r--   0 jon        (501) staff       (20)     6091 2023-03-31 05:09:49.000000 kshell-utilities-1.5.0.1/tests/test_partition_editor.py
+-rw-r--r--   0 jon        (501) staff       (20)     1327 2023-03-22 04:07:31.000000 kshell-utilities-1.5.0.1/tests/test_spin_parity_list.py
```

### Comparing `kshell-utilities-1.5.0.0/LICENSE` & `kshell-utilities-1.5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/PKG-INFO` & `kshell-utilities-1.5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kshell-utilities
-Version: 1.5.0.0
+Version: 1.5.0.1
 Summary: Handy utilities for handling nuclear shell model calculations from KSHELL
 Home-page: https://github.com/GaffaSnobb/kshell-utilities
 Author: ['Jon Kristian Dahl', 'Johannes Heines']
 Author-email: jonkd@uio.no
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
```

### Comparing `kshell-utilities-1.5.0.0/README.md` & `kshell-utilities-1.5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/__init__.py` & `kshell-utilities-1.5.0.1/kshell_utilities/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Jon Kristian Dahl, Johannes Heines"
-__version__ = "1.5.0.0"
+__version__ = "1.5.0.1"
 __credits__ = "Noritaka Shimizu, Jørgen Eriksson Midtbø"
 
 """
 Version legend:
 a.b.c.d
 
 a: major release
```

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/collect_logs.py` & `kshell-utilities-1.5.0.1/kshell_utilities/collect_logs.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/compare.py` & `kshell-utilities-1.5.0.1/kshell_utilities/compare.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/count_dim.py` & `kshell-utilities-1.5.0.1/kshell_utilities/count_dim.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/data_structures.py` & `kshell-utilities-1.5.0.1/kshell_utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/deprecated.py` & `kshell-utilities-1.5.0.1/kshell_utilities/deprecated.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/general_utilities.py` & `kshell-utilities-1.5.0.1/kshell_utilities/general_utilities.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/kshell_utilities.py` & `kshell-utilities-1.5.0.1/kshell_utilities/kshell_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import os, sys, multiprocessing, hashlib, ast, time, re
 from fractions import Fraction
 from typing import Union, Callable, Tuple, Iterable
 from itertools import chain
 import numpy as np
 import numba
 import matplotlib.pyplot as plt
@@ -2802,8 +2803,8 @@
             print(f"{np.mean(B_decay) = }")
             print(f"{np.min(B_decay) = }")
             print(f"{np.max(B_decay) = }")
             print(f"{sum(B_decay) = }")
             print(f"{sum(B_decay == 0) = }")
             print(f"{sum(B_decay != 0) = }")
             print(f"{len(B_decay) = }")
-            print()
+            print()
```

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/kshell_utilities_tmp.py` & `kshell-utilities-1.5.0.1/kshell_utilities/kshell_utilities_tmp.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/loaders.py` & `kshell-utilities-1.5.0.1/kshell_utilities/loaders.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/other_tools.py` & `kshell-utilities-1.5.0.1/kshell_utilities/other_tools.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/parameters.py` & `kshell-utilities-1.5.0.1/kshell_utilities/parameters.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/partition_compare.py` & `kshell-utilities-1.5.0.1/kshell_utilities/partition_compare.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/partition_editor.py` & `kshell-utilities-1.5.0.1/kshell_utilities/partition_editor.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/partition_tools.py` & `kshell-utilities-1.5.0.1/kshell_utilities/partition_tools.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities/script_editing.py` & `kshell-utilities-1.5.0.1/kshell_utilities/script_editing.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities.egg-info/PKG-INFO` & `kshell-utilities-1.5.0.1/kshell_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kshell-utilities
-Version: 1.5.0.0
+Version: 1.5.0.1
 Summary: Handy utilities for handling nuclear shell model calculations from KSHELL
 Home-page: https://github.com/GaffaSnobb/kshell-utilities
 Author: ['Jon Kristian Dahl', 'Johannes Heines']
 Author-email: jonkd@uio.no
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
```

### Comparing `kshell-utilities-1.5.0.0/kshell_utilities.egg-info/SOURCES.txt` & `kshell-utilities-1.5.0.1/kshell_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/setup.py` & `kshell-utilities-1.5.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     import pypandoc
 #     long_description = pypandoc.convert('README.md', 'rst')
 # except (IOError, ImportError, OSError):
 #     long_description = ""
 
 setup(
     name = 'kshell-utilities',
-    version = '1.5.0.0',    
+    version = '1.5.0.1',    
     description = 'Handy utilities for handling nuclear shell model calculations from KSHELL',
     # long_description = long_description,
     url = 'https://github.com/GaffaSnobb/kshell-utilities',
     author = ['Jon Kristian Dahl', 'Johannes Heines'],
     author_email = 'jonkd@uio.no',
     packages = ['kshell_utilities', 'tests'],
     install_requires = ['numpy', 'matplotlib', 'seaborn', 'scipy', 'numba', 'vum'],
```

### Comparing `kshell-utilities-1.5.0.0/tests/test_all.py` & `kshell-utilities-1.5.0.1/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/tests/test_partition_editor.py` & `kshell-utilities-1.5.0.1/tests/test_partition_editor.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.5.0.0/tests/test_spin_parity_list.py` & `kshell-utilities-1.5.0.1/tests/test_spin_parity_list.py`

 * *Files identical despite different names*

