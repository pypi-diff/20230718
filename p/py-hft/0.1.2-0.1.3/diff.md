# Comparing `tmp/py_hft-0.1.2.tar.gz` & `tmp/py_hft-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_hft-0.1.2.tar", last modified: Tue Apr 11 11:47:49 2023, max compression
+gzip compressed data, was "py_hft-0.1.3.tar", last modified: Tue Jul 18 04:55:09 2023, max compression
```

## Comparing `py_hft-0.1.2.tar` & `py_hft-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.586935 py_hft-0.1.2/
--rw-r--r--   0 root         (0) root         (0)      264 2023-04-11 11:47:49.585935 py_hft-0.1.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.584935 py_hft-0.1.2/py_hft/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.585935 py_hft-0.1.2/py_hft/hft_struct/
--rw-r--r--   0 root         (0) root         (0)     3096 2022-10-02 00:43:47.000000 py_hft-0.1.2/py_hft/hft_struct/Reader.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/hft_struct/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1412 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/hft_struct/exchange_info.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-04-11 11:46:12.000000 py_hft-0.1.2/py_hft/hft_struct/market_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     2156 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/hft_struct/order.py
--rw-r--r--   0 root         (0) root         (0)     1065 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/hft_struct/struct_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.585935 py_hft-0.1.2/py_hft/util/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3085 2022-09-20 15:24:18.000000 py_hft-0.1.2/py_hft/util/factor.py
--rw-r--r--   0 root         (0) root         (0)     7802 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/util/mploter.py
--rw-r--r--   0 root         (0) root         (0)     6173 2022-09-12 16:13:27.000000 py_hft-0.1.2/py_hft/util/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.585935 py_hft-0.1.2/py_hft/vendor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8195 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/ali_oss_tools.py
--rw-r--r--   0 root         (0) root         (0)     9113 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/jq_tools.py
--rw-r--r--   0 root         (0) root         (0)     1649 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/rq_tools.py
--rw-r--r--   0 root         (0) root         (0)     8012 2022-09-19 02:41:54.000000 py_hft-0.1.2/py_hft/vendor/tushare_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:47:49.584935 py_hft-0.1.2/py_hft.egg-info/
--rw-r--r--   0 root         (0) root         (0)      264 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      595 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-11 11:47:49.000000 py_hft-0.1.2/py_hft.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 11:47:49.586935 py_hft-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3365 2023-04-11 11:47:41.000000 py_hft-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.606588 py_hft-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-18 04:55:09.605588 py_hft-0.1.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.603588 py_hft-0.1.3/py_hft/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.604588 py_hft-0.1.3/py_hft/hft_struct/
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-07-18 04:51:31.000000 py_hft-0.1.3/py_hft/hft_struct/Reader.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/hft_struct/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/hft_struct/exchange_info.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-07-18 04:54:35.000000 py_hft-0.1.3/py_hft/hft_struct/market_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/hft_struct/order.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/hft_struct/struct_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.605588 py_hft-0.1.3/py_hft/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2022-09-20 15:24:18.000000 py_hft-0.1.3/py_hft/util/factor.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/util/mploter.py
+-rw-r--r--   0 root         (0) root         (0)     6173 2022-09-12 16:13:27.000000 py_hft-0.1.3/py_hft/util/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.605588 py_hft-0.1.3/py_hft/vendor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8195 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/ali_oss_tools.py
+-rw-r--r--   0 root         (0) root         (0)     9113 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/jq_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/rq_tools.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2022-09-19 02:41:54.000000 py_hft-0.1.3/py_hft/vendor/tushare_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:55:09.603588 py_hft-0.1.3/py_hft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      595 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-18 04:55:09.000000 py_hft-0.1.3/py_hft.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 04:55:09.606588 py_hft-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-07-18 04:55:05.000000 py_hft-0.1.3/setup.py
```

### Comparing `py_hft-0.1.2/py_hft/hft_struct/Reader.py` & `py_hft-0.1.3/py_hft/hft_struct/Reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,19 +39,20 @@
     del df['ts_'], df['sec']
     RedPrint('load cost', time.time()-start,  color='green')
     return df.set_index('dt')
 
   @staticmethod
   def load_shot(file_path, topic, cols=['bp0_', 'ap0_', 'bs0_', 'as0_', 'lp_', 'tvr_', 'ls_', 'vol_', 'oi_']):
     shot = MarketSnapshot()
-    m = 'a16,i8,i8,' + 'f8,' * 10 + 'i4,' * 10 + 'f8,f8,' + 'i4,' * 3 + 'i4'
-    df = pd.DataFrame(np.frombuffer(open('%s'%(file_path), 'rb').read(), dtype=m))
+    m = 'a8,a16,i8,i8,' + 'f8,' * 10 + 'i4,' * 10 + 'f8,f8,' + 'i4,' * 3 + 'i4'
+    df = pd.DataFrame(np.frombuffer(open('%s'%(file_path), 'rb').read()[40:], dtype=m))
     #del df['f24'], df['f29']
     del df['f28']
-    df.columns = shot.__dict__.keys()
+    df.columns = ['vptr'] + [shot.__dict__.keys()]
+    del df['vptr']
     tme = df['ts_'] + df['uts_'] / 1e6
     del df['uts_']
     df['tk_'] = df['tk_'].apply(lambda x: str(x)[2:].split('\\x0')[0].split("'")[0])
     df['topic'] = topic
     dtt = pd.to_datetime(tme, unit='s', utc=True).dt.tz_convert('Asia/Shanghai')
     #df['date'] = dtt.dt.date#.apply(lambda x: int(x.strftime('%Y%M%d')))
     #df['time'] = dtt.dt.time
```

### Comparing `py_hft-0.1.2/py_hft/hft_struct/exchange_info.py` & `py_hft-0.1.3/py_hft/hft_struct/exchange_info.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/hft_struct/market_snapshot.py` & `py_hft-0.1.3/py_hft/hft_struct/market_snapshot.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/hft_struct/order.py` & `py_hft-0.1.3/py_hft/hft_struct/order.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/hft_struct/struct_util.py` & `py_hft-0.1.3/py_hft/hft_struct/struct_util.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/util/factor.py` & `py_hft-0.1.3/py_hft/util/factor.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/util/mploter.py` & `py_hft-0.1.3/py_hft/util/mploter.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/util/util.py` & `py_hft-0.1.3/py_hft/util/util.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/vendor/ali_oss_tools.py` & `py_hft-0.1.3/py_hft/vendor/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/vendor/jq_tools.py` & `py_hft-0.1.3/py_hft/vendor/jq_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/vendor/rq_tools.py` & `py_hft-0.1.3/py_hft/vendor/rq_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft/vendor/tushare_tools.py` & `py_hft-0.1.3/py_hft/vendor/tushare_tools.py`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/py_hft.egg-info/SOURCES.txt` & `py_hft-0.1.3/py_hft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_hft-0.1.2/setup.py` & `py_hft-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'py_hft'
 DESCRIPTION = 'util for hft'
 URL = 'https://zhuanlan.zhihu.com/p/26159930'
 EMAIL = 'arockie123@gmail.com'
 AUTHOR = 'arockie'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['tushare', 'matplotlib', 'tqdm', 'psutil', 'pandas', 'tabulate', 'ipython', 'catboost', 'statsmodels', 'scipy', 'termcolor', 'jupyter', 'tushare']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

