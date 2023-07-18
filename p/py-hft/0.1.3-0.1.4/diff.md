# Comparing `tmp/py_hft-0.1.3.tar.gz` & `tmp/py_hft-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_hft-0.1.3.tar", last modified: Tue Jul 18 04:55:09 2023, max compression
+gzip compressed data, was "py_hft-0.1.4.tar", last modified: Tue Jul 18 06:26:32 2023, max compression
```

## Comparing `py_hft-0.1.3.tar` & `py_hft-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.606588 py_hft-0.1.3/
--rw-r--r--   0 root         (0) root         (0)      264 2023-07-18 04:55:09.605588 py_hft-0.1.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.603588 py_hft-0.1.3/py_hft/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.604588 py_hft-0.1.3/py_hft/hft_struct/
--rw-r--r--   0 root         (0) root         (0)     3136 2023-07-18 04:51:31.000000 py_hft-0.1.3/py_hft/hft_struct/Reader.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/hft_struct/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1412 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/hft_struct/exchange_info.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-07-18 04:54:35.000000 py_hft-0.1.3/py_hft/hft_struct/market_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     2156 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/hft_struct/order.py
--rw-r--r--   0 root         (0) root         (0)     1065 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/hft_struct/struct_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.605588 py_hft-0.1.3/py_hft/util/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3085 2022-09-20 15:24:18.000000 py_hft-0.1.3/py_hft/util/factor.py
--rw-r--r--   0 root         (0) root         (0)     7802 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/util/mploter.py
--rw-r--r--   0 root         (0) root         (0)     6173 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/util/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.605588 py_hft-0.1.3/py_hft/vendor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8195 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/ali_oss_tools.py
--rw-r--r--   0 root         (0) root         (0)     9113 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/jq_tools.py
--rw-r--r--   0 root         (0) root         (0)     1649 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/rq_tools.py
--rw-r--r--   0 root         (0) root         (0)     8012 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/tushare_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.603588 py_hft-0.1.3/py_hft.egg-info/
--rw-r--r--   0 root         (0) root         (0)      264 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      595 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 04:55:09.606588 py_hft-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3365 2023-07-18 04:55:05.000000 py_hft-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:26:32.704349 py_hft-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-18 06:26:32.704349 py_hft-0.1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:26:32.703349 py_hft-0.1.4/py_hft/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.4/py_hft/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:26:32.704349 py_hft-0.1.4/py_hft/hft_struct/
+-rw-r--r--   0 root         (0) root         (0)     5064 2023-07-18 05:39:59.000000 py_hft-0.1.4/py_hft/hft_struct/Reader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.4/py_hft/hft_struct/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-07-18 05:37:10.000000 py_hft-0.1.4/py_hft/hft_struct/book_ticker.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2022-09-12 16:13:27.000000 py_hft-0.1.4/py_hft/hft_struct/exchange_info.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-07-18 04:54:35.000000 py_hft-0.1.4/py_hft/hft_struct/market_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2022-09-12 16:13:27.000000 py_hft-0.1.4/py_hft/hft_struct/order.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-07-18 05:30:55.000000 py_hft-0.1.4/py_hft/hft_struct/struct_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:26:32.704349 py_hft-0.1.4/py_hft/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.4/py_hft/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2022-09-20 15:24:18.000000 py_hft-0.1.4/py_hft/util/factor.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2022-09-12 16:13:27.000000 py_hft-0.1.4/py_hft/util/mploter.py
+-rw-r--r--   0 root         (0) root         (0)     6173 2022-09-12 16:13:27.000000 py_hft-0.1.4/py_hft/util/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:26:32.704349 py_hft-0.1.4/py_hft/vendor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 02:41:54.000000 py_hft-0.1.4/py_hft/vendor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8195 2022-09-19 02:41:54.000000 py_hft-0.1.4/py_hft/vendor/ali_oss_tools.py
+-rw-r--r--   0 root         (0) root         (0)     9113 2022-09-19 02:41:54.000000 py_hft-0.1.4/py_hft/vendor/jq_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2022-09-19 02:41:54.000000 py_hft-0.1.4/py_hft/vendor/rq_tools.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2022-09-19 02:41:54.000000 py_hft-0.1.4/py_hft/vendor/tushare_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 06:26:32.703349 py_hft-0.1.4/py_hft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-18 06:26:32.000000 py_hft-0.1.4/py_hft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-18 06:26:32.000000 py_hft-0.1.4/py_hft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 06:26:32.000000 py_hft-0.1.4/py_hft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-18 06:26:32.000000 py_hft-0.1.4/py_hft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-18 06:26:32.000000 py_hft-0.1.4/py_hft.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 06:26:32.704349 py_hft-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3359 2023-07-18 06:26:26.000000 py_hft-0.1.4/setup.py
```

### Comparing `py_hft-0.1.3/py_hft/hft_struct/exchange_info.py` & `py_hft-0.1.4/py_hft/hft_struct/exchange_info.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft/hft_struct/market_snapshot.py` & `py_hft-0.1.4/py_hft/hft_struct/market_snapshot.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft/hft_struct/order.py` & `py_hft-0.1.4/py_hft/hft_struct/order.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft/hft_struct/struct_util.py` & `py_hft-0.1.4/py_hft/hft_struct/struct_util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .market_snapshot import *
+from .book_ticker import *
 from .order import *
 from .exchange_info import *
 from collections.abc import Iterable
 import sys
 
 def Show(s, f=None):
   if f: f.write(s.__str__()+'\n')
```

### Comparing `py_hft-0.1.3/py_hft/util/factor.py` & `py_hft-0.1.4/py_hft/util/factor.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft/util/mploter.py` & `py_hft-0.1.4/py_hft/util/mploter.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft/util/util.py` & `py_hft-0.1.4/py_hft/util/util.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft/vendor/ali_oss_tools.py` & `py_hft-0.1.4/py_hft/vendor/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft/vendor/jq_tools.py` & `py_hft-0.1.4/py_hft/vendor/jq_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft/vendor/rq_tools.py` & `py_hft-0.1.4/py_hft/vendor/rq_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft/vendor/tushare_tools.py` & `py_hft-0.1.4/py_hft/vendor/tushare_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.3/py_hft.egg-info/SOURCES.txt` & `py_hft-0.1.4/py_hft.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 py_hft.egg-info/PKG-INFO
 py_hft.egg-info/SOURCES.txt
 py_hft.egg-info/dependency_links.txt
 py_hft.egg-info/requires.txt
 py_hft.egg-info/top_level.txt
 py_hft/hft_struct/Reader.py
 py_hft/hft_struct/__init__.py
+py_hft/hft_struct/book_ticker.py
 py_hft/hft_struct/exchange_info.py
 py_hft/hft_struct/market_snapshot.py
 py_hft/hft_struct/order.py
 py_hft/hft_struct/struct_util.py
 py_hft/util/__init__.py
 py_hft/util/factor.py
 py_hft/util/mploter.py
```

### Comparing `py_hft-0.1.3/setup.py` & `py_hft-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import sys
 from shutil import rmtree
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'py_hft'
 DESCRIPTION = 'util for hft'
-URL = 'https://zhuanlan.zhihu.com/p/26159930'
+URL = 'https://zhuanlan.zhihu.com/p/26'
 EMAIL = 'arockie123@gmail.com'
 AUTHOR = 'arockie'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['tushare', 'matplotlib', 'tqdm', 'psutil', 'pandas', 'tabulate', 'ipython', 'catboost', 'statsmodels', 'scipy', 'termcolor', 'jupyter', 'tushare']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

