# Comparing `tmp/similarity_ts-1.0.1.tar.gz` & `tmp/similarity_ts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarity_ts-1.0.1.tar", last modified: Tue Jul 18 05:53:00 2023, max compression
+gzip compressed data, was "similarity_ts-1.0.2.tar", last modified: Tue Jul 18 06:26:24 2023, max compression
```

## Comparing `similarity_ts-1.0.1.tar` & `similarity_ts-1.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 05:53:00.091655 similarity_ts-1.0.1/
--rw-r--r--   0 afdez      (501) staff       (20)     1079 2023-07-16 10:03:12.000000 similarity_ts-1.0.1/LICENSE
--rw-r--r--   0 afdez      (501) staff       (20)    17043 2023-07-18 05:53:00.091361 similarity_ts-1.0.1/PKG-INFO
--rw-r--r--   0 afdez      (501) staff       (20)    16315 2023-07-18 05:51:21.000000 similarity_ts-1.0.1/README.md
--rw-r--r--   0 afdez      (501) staff       (20)      959 2023-07-18 05:52:54.000000 similarity_ts-1.0.1/pyproject.toml
--rw-r--r--   0 afdez      (501) staff       (20)       38 2023-07-18 05:53:00.091760 similarity_ts-1.0.1/setup.cfg
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 05:53:00.078363 similarity_ts-1.0.1/src/
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 05:53:00.080884 similarity_ts-1.0.1/src/similarity_ts/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.1/src/similarity_ts/__init__.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 05:53:00.083477 similarity_ts-1.0.1/src/similarity_ts/helpers/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.1/src/similarity_ts/helpers/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)     2161 2023-07-17 10:38:41.000000 similarity_ts-1.0.1/src/similarity_ts/helpers/csv_reader_helper.py
--rw-r--r--   0 afdez      (501) staff       (20)     1113 2023-07-16 14:24:04.000000 similarity_ts-1.0.1/src/similarity_ts/helpers/dynamic_import_helper.py
--rw-r--r--   0 afdez      (501) staff       (20)     1928 2023-07-17 11:05:25.000000 similarity_ts-1.0.1/src/similarity_ts/helpers/window_sampler.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 05:53:00.087524 similarity_ts-1.0.1/src/similarity_ts/metrics/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)      669 2023-07-17 10:39:19.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/cc.py
--rw-r--r--   0 afdez      (501) staff       (20)      637 2023-07-17 10:39:19.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/cp.py
--rw-r--r--   0 afdez      (501) staff       (20)     1164 2023-07-17 11:15:50.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/dtw.py
--rw-r--r--   0 afdez      (501) staff       (20)     1430 2023-07-17 11:15:50.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/hi.py
--rw-r--r--   0 afdez      (501) staff       (20)     1065 2023-07-17 11:15:50.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/js.py
--rw-r--r--   0 afdez      (501) staff       (20)     3999 2023-07-17 11:15:50.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/kl.py
--rw-r--r--   0 afdez      (501) staff       (20)      889 2023-07-17 11:15:50.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/ks.py
--rw-r--r--   0 afdez      (501) staff       (20)      350 2023-07-17 10:39:19.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/metric.py
--rw-r--r--   0 afdez      (501) staff       (20)      798 2023-07-17 10:39:19.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/metric_computer.py
--rw-r--r--   0 afdez      (501) staff       (20)      321 2023-07-14 17:03:35.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/metric_config.py
--rw-r--r--   0 afdez      (501) staff       (20)     1552 2023-07-17 07:05:11.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/metric_factory.py
--rw-r--r--   0 afdez      (501) staff       (20)     1011 2023-07-17 11:15:50.000000 similarity_ts-1.0.1/src/similarity_ts/metrics/mmd.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 05:53:00.090894 similarity_ts-1.0.1/src/similarity_ts/plots/
--rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.1/src/similarity_ts/plots/__init__.py
--rw-r--r--   0 afdez      (501) staff       (20)     4295 2023-07-14 17:42:31.000000 similarity_ts-1.0.1/src/similarity_ts/plots/delta.py
--rw-r--r--   0 afdez      (501) staff       (20)     1064 2023-07-14 17:09:09.000000 similarity_ts-1.0.1/src/similarity_ts/plots/dimensionalty_reduction.py
--rw-r--r--   0 afdez      (501) staff       (20)     1129 2023-07-14 17:18:51.000000 similarity_ts-1.0.1/src/similarity_ts/plots/dtw.py
--rw-r--r--   0 afdez      (501) staff       (20)     1464 2023-07-14 17:18:51.000000 similarity_ts-1.0.1/src/similarity_ts/plots/pca.py
--rw-r--r--   0 afdez      (501) staff       (20)     1162 2023-07-14 17:18:51.000000 similarity_ts-1.0.1/src/similarity_ts/plots/plot.py
--rw-r--r--   0 afdez      (501) staff       (20)      976 2023-07-14 17:56:55.000000 similarity_ts-1.0.1/src/similarity_ts/plots/plot_computer.py
--rw-r--r--   0 afdez      (501) staff       (20)      518 2023-07-14 17:10:27.000000 similarity_ts-1.0.1/src/similarity_ts/plots/plot_config.py
--rw-r--r--   0 afdez      (501) staff       (20)     1681 2023-07-17 07:05:11.000000 similarity_ts-1.0.1/src/similarity_ts/plots/plot_factory.py
--rw-r--r--   0 afdez      (501) staff       (20)     2277 2023-07-14 17:18:51.000000 similarity_ts-1.0.1/src/similarity_ts/plots/tsne.py
--rw-r--r--   0 afdez      (501) staff       (20)     2128 2023-07-14 17:09:09.000000 similarity_ts-1.0.1/src/similarity_ts/plots/two_dimensions.py
--rw-r--r--   0 afdez      (501) staff       (20)     1084 2023-07-14 12:53:28.000000 similarity_ts-1.0.1/src/similarity_ts/similarity_analysis_computer.py
--rw-r--r--   0 afdez      (501) staff       (20)     1755 2023-07-17 11:16:50.000000 similarity_ts-1.0.1/src/similarity_ts/similarity_ts.py
--rw-r--r--   0 afdez      (501) staff       (20)      672 2023-07-14 16:52:41.000000 similarity_ts-1.0.1/src/similarity_ts/similarity_ts_config.py
-drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 05:53:00.082138 similarity_ts-1.0.1/src/similarity_ts.egg-info/
--rw-r--r--   0 afdez      (501) staff       (20)    17043 2023-07-18 05:53:00.000000 similarity_ts-1.0.1/src/similarity_ts.egg-info/PKG-INFO
--rw-r--r--   0 afdez      (501) staff       (20)     1445 2023-07-18 05:53:00.000000 similarity_ts-1.0.1/src/similarity_ts.egg-info/SOURCES.txt
--rw-r--r--   0 afdez      (501) staff       (20)        1 2023-07-18 05:53:00.000000 similarity_ts-1.0.1/src/similarity_ts.egg-info/dependency_links.txt
--rw-r--r--   0 afdez      (501) staff       (20)       65 2023-07-18 05:53:00.000000 similarity_ts-1.0.1/src/similarity_ts.egg-info/requires.txt
--rw-r--r--   0 afdez      (501) staff       (20)       14 2023-07-18 05:53:00.000000 similarity_ts-1.0.1/src/similarity_ts.egg-info/top_level.txt
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.145019 similarity_ts-1.0.2/
+-rw-r--r--   0 afdez      (501) staff       (20)     1079 2023-07-16 10:03:12.000000 similarity_ts-1.0.2/LICENSE
+-rw-r--r--   0 afdez      (501) staff       (20)    17150 2023-07-18 06:26:24.144744 similarity_ts-1.0.2/PKG-INFO
+-rw-r--r--   0 afdez      (501) staff       (20)    16422 2023-07-18 06:26:01.000000 similarity_ts-1.0.2/README.md
+-rw-r--r--   0 afdez      (501) staff       (20)      959 2023-07-18 06:26:16.000000 similarity_ts-1.0.2/pyproject.toml
+-rw-r--r--   0 afdez      (501) staff       (20)       38 2023-07-18 06:26:24.145078 similarity_ts-1.0.2/setup.cfg
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.131829 similarity_ts-1.0.2/src/
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.134630 similarity_ts-1.0.2/src/similarity_ts/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.2/src/similarity_ts/__init__.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.137418 similarity_ts-1.0.2/src/similarity_ts/helpers/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.2/src/similarity_ts/helpers/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)     2161 2023-07-17 10:38:41.000000 similarity_ts-1.0.2/src/similarity_ts/helpers/csv_reader_helper.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1113 2023-07-16 14:24:04.000000 similarity_ts-1.0.2/src/similarity_ts/helpers/dynamic_import_helper.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1928 2023-07-17 11:05:25.000000 similarity_ts-1.0.2/src/similarity_ts/helpers/window_sampler.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.141303 similarity_ts-1.0.2/src/similarity_ts/metrics/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)      669 2023-07-17 10:39:19.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/cc.py
+-rw-r--r--   0 afdez      (501) staff       (20)      637 2023-07-17 10:39:19.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/cp.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1164 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/dtw.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1430 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/hi.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1065 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/js.py
+-rw-r--r--   0 afdez      (501) staff       (20)     3999 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/kl.py
+-rw-r--r--   0 afdez      (501) staff       (20)      889 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/ks.py
+-rw-r--r--   0 afdez      (501) staff       (20)      350 2023-07-17 10:39:19.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/metric.py
+-rw-r--r--   0 afdez      (501) staff       (20)      798 2023-07-17 10:39:19.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/metric_computer.py
+-rw-r--r--   0 afdez      (501) staff       (20)      321 2023-07-14 17:03:35.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/metric_config.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1552 2023-07-17 07:05:11.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/metric_factory.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1011 2023-07-17 11:15:50.000000 similarity_ts-1.0.2/src/similarity_ts/metrics/mmd.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.144364 similarity_ts-1.0.2/src/similarity_ts/plots/
+-rw-r--r--   0 afdez      (501) staff       (20)        0 2023-07-14 15:40:23.000000 similarity_ts-1.0.2/src/similarity_ts/plots/__init__.py
+-rw-r--r--   0 afdez      (501) staff       (20)     4295 2023-07-14 17:42:31.000000 similarity_ts-1.0.2/src/similarity_ts/plots/delta.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1064 2023-07-14 17:09:09.000000 similarity_ts-1.0.2/src/similarity_ts/plots/dimensionalty_reduction.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1129 2023-07-14 17:18:51.000000 similarity_ts-1.0.2/src/similarity_ts/plots/dtw.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1464 2023-07-14 17:18:51.000000 similarity_ts-1.0.2/src/similarity_ts/plots/pca.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1162 2023-07-14 17:18:51.000000 similarity_ts-1.0.2/src/similarity_ts/plots/plot.py
+-rw-r--r--   0 afdez      (501) staff       (20)      976 2023-07-14 17:56:55.000000 similarity_ts-1.0.2/src/similarity_ts/plots/plot_computer.py
+-rw-r--r--   0 afdez      (501) staff       (20)      518 2023-07-14 17:10:27.000000 similarity_ts-1.0.2/src/similarity_ts/plots/plot_config.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1681 2023-07-17 07:05:11.000000 similarity_ts-1.0.2/src/similarity_ts/plots/plot_factory.py
+-rw-r--r--   0 afdez      (501) staff       (20)     2277 2023-07-14 17:18:51.000000 similarity_ts-1.0.2/src/similarity_ts/plots/tsne.py
+-rw-r--r--   0 afdez      (501) staff       (20)     2128 2023-07-14 17:09:09.000000 similarity_ts-1.0.2/src/similarity_ts/plots/two_dimensions.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1084 2023-07-14 12:53:28.000000 similarity_ts-1.0.2/src/similarity_ts/similarity_analysis_computer.py
+-rw-r--r--   0 afdez      (501) staff       (20)     1755 2023-07-17 11:16:50.000000 similarity_ts-1.0.2/src/similarity_ts/similarity_ts.py
+-rw-r--r--   0 afdez      (501) staff       (20)      672 2023-07-14 16:52:41.000000 similarity_ts-1.0.2/src/similarity_ts/similarity_ts_config.py
+drwxr-xr-x   0 afdez      (501) staff       (20)        0 2023-07-18 06:26:24.136014 similarity_ts-1.0.2/src/similarity_ts.egg-info/
+-rw-r--r--   0 afdez      (501) staff       (20)    17150 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/PKG-INFO
+-rw-r--r--   0 afdez      (501) staff       (20)     1445 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/SOURCES.txt
+-rw-r--r--   0 afdez      (501) staff       (20)        1 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/dependency_links.txt
+-rw-r--r--   0 afdez      (501) staff       (20)       65 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/requires.txt
+-rw-r--r--   0 afdez      (501) staff       (20)       14 2023-07-18 06:26:24.000000 similarity_ts-1.0.2/src/similarity_ts.egg-info/top_level.txt
```

### Comparing `similarity_ts-1.0.1/LICENSE` & `similarity_ts-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/PKG-INFO` & `similarity_ts-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity_ts
-Version: 1.0.1
+Version: 1.0.2
 Summary: SimilarityTS is an open-source project designed to facilitate the evaluation and comparison of multivariate time series data
 Author-email: Alejandro Fernández-Montes <afdez@us.es>, Damián Fernández-Cerero <damiancerero@us.es>, Felipe Escalera González <fescalera@us.es>
 Project-URL: Homepage, https://github.com/alejandrofdez-us/similarity-ts
 Project-URL: Bug Tracker, https://github.com/alejandrofdez-us/similarity-ts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -129,14 +129,15 @@
 
 (*) The metric used for the selection of the most
 similar `ts1` time-series window per each `ts2s` time-series file is selectable.`dtw` is the default selected metric, however, any of
 the
 [metrics](#available-metrics) are also available for this purpose. See the [toolkit configuration section](#configuring-the-toolkit)
 
 ### Minimal usage examples:
+Usage examples can be found at: https://github.com/alejandrofdez-us/similarity-ts/tree/main/usage_examples
 
 1. Compute metrics between random time series (`ts1`: one time series of lenght 200 and 2 dimensions and `ts2`: five time series of length 100 and 2 dimensions):
     ```Python
     import numpy as np
     from similarity_ts.similarity_ts import SimilarityTs
     
     ts1 = np.random.rand(200, 2)
```

### Comparing `similarity_ts-1.0.1/README.md` & `similarity_ts-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -439,582 +439,589 @@
 00001b60: 6520 666f 7220 7468 6973 2070 7572 706f  e for this purpo
 00001b70: 7365 2e20 5365 6520 7468 6520 5b74 6f6f  se. See the [too
 00001b80: 6c6b 6974 2063 6f6e 6669 6775 7261 7469  lkit configurati
 00001b90: 6f6e 2073 6563 7469 6f6e 5d28 2363 6f6e  on section](#con
 00001ba0: 6669 6775 7269 6e67 2d74 6865 2d74 6f6f  figuring-the-too
 00001bb0: 6c6b 6974 290a 0a23 2323 204d 696e 696d  lkit)..### Minim
 00001bc0: 616c 2075 7361 6765 2065 7861 6d70 6c65  al usage example
-00001bd0: 733a 0a0a 312e 2043 6f6d 7075 7465 206d  s:..1. Compute m
-00001be0: 6574 7269 6373 2062 6574 7765 656e 2072  etrics between r
-00001bf0: 616e 646f 6d20 7469 6d65 2073 6572 6965  andom time serie
-00001c00: 7320 2860 7473 3160 3a20 6f6e 6520 7469  s (`ts1`: one ti
-00001c10: 6d65 2073 6572 6965 7320 6f66 206c 656e  me series of len
-00001c20: 6768 7420 3230 3020 616e 6420 3220 6469  ght 200 and 2 di
-00001c30: 6d65 6e73 696f 6e73 2061 6e64 2060 7473  mensions and `ts
-00001c40: 3260 3a20 6669 7665 2074 696d 6520 7365  2`: five time se
-00001c50: 7269 6573 206f 6620 6c65 6e67 7468 2031  ries of length 1
-00001c60: 3030 2061 6e64 2032 2064 696d 656e 7369  00 and 2 dimensi
-00001c70: 6f6e 7329 3a0a 2020 2020 6060 6050 7974  ons):.    ```Pyt
-00001c80: 686f 6e0a 2020 2020 696d 706f 7274 206e  hon.    import n
-00001c90: 756d 7079 2061 7320 6e70 0a20 2020 2066  umpy as np.    f
-00001ca0: 726f 6d20 7369 6d69 6c61 7269 7479 5f74  rom similarity_t
-00001cb0: 732e 7369 6d69 6c61 7269 7479 5f74 7320  s.similarity_ts 
-00001cc0: 696d 706f 7274 2053 696d 696c 6172 6974  import Similarit
-00001cd0: 7954 730a 2020 2020 0a20 2020 2074 7331  yTs.    .    ts1
-00001ce0: 203d 206e 702e 7261 6e64 6f6d 2e72 616e   = np.random.ran
-00001cf0: 6428 3230 302c 2032 290a 2020 2020 7473  d(200, 2).    ts
-00001d00: 3273 203d 206e 702e 7261 6e64 6f6d 2e72  2s = np.random.r
-00001d10: 616e 6428 352c 2031 3030 2c20 3229 0a20  and(5, 100, 2). 
-00001d20: 2020 2073 696d 696c 6172 6974 795f 7473     similarity_ts
-00001d30: 203d 2053 696d 696c 6172 6974 7954 7328   = SimilarityTs(
-00001d40: 7473 312c 2074 7332 7329 0a20 2020 2066  ts1, ts2s).    f
-00001d50: 6f72 2074 7332 5f6e 616d 652c 206d 6574  or ts2_name, met
-00001d60: 7269 635f 6e61 6d65 2c20 636f 6d70 7574  ric_name, comput
-00001d70: 6564 5f6d 6574 7269 6320 696e 2073 696d  ed_metric in sim
-00001d80: 696c 6172 6974 795f 7473 2e67 6574 5f6d  ilarity_ts.get_m
-00001d90: 6574 7269 635f 636f 6d70 7574 6572 2829  etric_computer()
-00001da0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-00001db0: 6627 7b74 7332 5f6e 616d 657d 2e20 7b6d  f'{ts2_name}. {m
-00001dc0: 6574 7269 635f 6e61 6d65 7d3a 207b 636f  etric_name}: {co
-00001dd0: 6d70 7574 6564 5f6d 6574 7269 637d 2729  mputed_metric}')
-00001de0: 0a20 2020 2060 6060 0a0a 312e 2043 6f6d  .    ```..1. Com
-00001df0: 7075 7465 206d 6574 7269 6373 2061 6e64  pute metrics and
-00001e00: 2066 6967 7572 6573 2062 6574 7765 656e   figures between
-00001e10: 2072 616e 646f 6d20 7469 6d65 2073 6572   random time ser
-00001e20: 6965 7320 616e 6420 7361 7665 2066 6967  ies and save fig
-00001e30: 7572 6573 3a0a 2020 2020 6060 6050 7974  ures:.    ```Pyt
-00001e40: 686f 6e0a 2020 2020 696d 706f 7274 206f  hon.    import o
-00001e50: 730a 2020 2020 696d 706f 7274 206e 756d  s.    import num
-00001e60: 7079 2061 7320 6e70 0a20 2020 2066 726f  py as np.    fro
-00001e70: 6d20 7369 6d69 6c61 7269 7479 5f74 732e  m similarity_ts.
-00001e80: 706c 6f74 732e 706c 6f74 5f66 6163 746f  plots.plot_facto
-00001e90: 7279 2069 6d70 6f72 7420 506c 6f74 4661  ry import PlotFa
-00001ea0: 6374 6f72 790a 2020 2020 6672 6f6d 2073  ctory.    from s
-00001eb0: 696d 696c 6172 6974 795f 7473 2e73 696d  imilarity_ts.sim
-00001ec0: 696c 6172 6974 795f 7473 2069 6d70 6f72  ilarity_ts impor
-00001ed0: 7420 5369 6d69 6c61 7269 7479 5473 0a20  t SimilarityTs. 
-00001ee0: 2020 200a 2020 2020 6465 6620 6d61 696e     .    def main
-00001ef0: 2829 3a0a 2020 2020 2020 2020 7473 3120  ():.        ts1 
-00001f00: 3d20 6e70 2e72 616e 646f 6d2e 7261 6e64  = np.random.rand
-00001f10: 2832 3030 2c20 3229 0a20 2020 2020 2020  (200, 2).       
-00001f20: 2074 7332 7320 3d20 6e70 2e72 616e 646f   ts2s = np.rando
-00001f30: 6d2e 7261 6e64 2835 2c20 3130 302c 2032  m.rand(5, 100, 2
-00001f40: 290a 2020 2020 2020 2020 7369 6d69 6c61  ).        simila
-00001f50: 7269 7479 5f74 7320 3d20 5369 6d69 6c61  rity_ts = Simila
-00001f60: 7269 7479 5473 2874 7331 2c20 7473 3273  rityTs(ts1, ts2s
-00001f70: 290a 2020 2020 2020 2020 666f 7220 7473  ).        for ts
-00001f80: 325f 6e61 6d65 2c20 6d65 7472 6963 5f6e  2_name, metric_n
-00001f90: 616d 652c 2063 6f6d 7075 7465 645f 6d65  ame, computed_me
-00001fa0: 7472 6963 2069 6e20 7369 6d69 6c61 7269  tric in similari
-00001fb0: 7479 5f74 732e 6765 745f 6d65 7472 6963  ty_ts.get_metric
-00001fc0: 5f63 6f6d 7075 7465 7228 293a 0a20 2020  _computer():.   
-00001fd0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00001fe0: 277b 7473 325f 6e61 6d65 7d2e 207b 6d65  '{ts2_name}. {me
-00001ff0: 7472 6963 5f6e 616d 657d 3a20 7b63 6f6d  tric_name}: {com
-00002000: 7075 7465 645f 6d65 7472 6963 7d27 290a  puted_metric}').
-00002010: 2020 2020 2020 2020 666f 7220 7473 325f          for ts2_
-00002020: 6e61 6d65 2c20 706c 6f74 5f6e 616d 652c  name, plot_name,
-00002030: 2067 656e 6572 6174 6564 5f70 6c6f 7473   generated_plots
-00002040: 2069 6e20 7369 6d69 6c61 7269 7479 5f74   in similarity_t
-00002050: 732e 6765 745f 706c 6f74 5f63 6f6d 7075  s.get_plot_compu
-00002060: 7465 7228 293a 0a20 2020 2020 2020 2020  ter():.         
-00002070: 2020 205f 5f73 6176 655f 6669 6775 7265     __save_figure
-00002080: 7328 7473 325f 6e61 6d65 2c20 706c 6f74  s(ts2_name, plot
-00002090: 5f6e 616d 652c 2067 656e 6572 6174 6564  _name, generated
-000020a0: 5f70 6c6f 7473 290a 2020 2020 0a20 2020  _plots).    .   
-000020b0: 200a 2020 2020 6465 6620 5f5f 7361 7665   .    def __save
-000020c0: 5f66 6967 7572 6573 2866 696c 656e 616d  _figures(filenam
-000020d0: 652c 2070 6c6f 745f 6e61 6d65 2c20 6765  e, plot_name, ge
-000020e0: 6e65 7261 7465 645f 706c 6f74 7329 3a0a  nerated_plots):.
-000020f0: 2020 2020 2020 2020 666f 7220 706c 6f74          for plot
-00002100: 2069 6e20 6765 6e65 7261 7465 645f 706c   in generated_pl
-00002110: 6f74 733a 0a20 2020 2020 2020 2020 2020  ots:.           
-00002120: 2064 6972 5f70 6174 6820 3d20 5f5f 6372   dir_path = __cr
-00002130: 6561 7465 5f64 6972 6563 746f 7279 2866  eate_directory(f
-00002140: 696c 656e 616d 652c 2066 2766 6967 7572  ilename, f'figur
-00002150: 6573 272c 2070 6c6f 745f 6e61 6d65 290a  es', plot_name).
-00002160: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
-00002170: 5b30 5d2e 7361 7665 6669 6728 6627 7b64  [0].savefig(f'{d
-00002180: 6972 5f70 6174 687d 7b70 6c6f 745b 305d  ir_path}{plot[0]
-00002190: 2e61 7865 735b 305d 2e67 6574 5f74 6974  .axes[0].get_tit
-000021a0: 6c65 2829 7d2e 7064 6627 2c20 666f 726d  le()}.pdf', form
-000021b0: 6174 3d27 7064 6627 2c20 6262 6f78 5f69  at='pdf', bbox_i
-000021c0: 6e63 6865 733d 2774 6967 6874 2729 0a20  nches='tight'). 
-000021d0: 2020 200a 2020 2020 0a20 2020 2064 6566     .    .    def
-000021e0: 205f 5f63 7265 6174 655f 6469 7265 6374   __create_direct
-000021f0: 6f72 7928 6669 6c65 6e61 6d65 2c20 7061  ory(filename, pa
-00002200: 7468 2c20 706c 6f74 5f6e 616d 6529 3a0a  th, plot_name):.
-00002210: 2020 2020 2020 2020 6966 2070 6c6f 745f          if plot_
-00002220: 6e61 6d65 2069 6e20 506c 6f74 4661 6374  name in PlotFact
-00002230: 6f72 792e 6765 745f 696e 7374 616e 6365  ory.get_instance
-00002240: 2829 2e66 6967 7572 6573 5f72 6571 7569  ().figures_requi
-00002250: 7265 735f 616c 6c5f 7361 6d70 6c65 733a  res_all_samples:
-00002260: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
-00002270: 5f70 6174 6820 3d20 6627 7b70 6174 687d  _path = f'{path}
-00002280: 2f7b 706c 6f74 5f6e 616d 657d 2f27 0a20  /{plot_name}/'. 
-00002290: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000022a0: 2020 2020 2020 2020 206f 7269 6769 6e61           origina
-000022b0: 6c5f 6669 6c65 6e61 6d65 203d 206f 732e  l_filename = os.
-000022c0: 7061 7468 2e73 706c 6974 6578 7428 6669  path.splitext(fi
-000022d0: 6c65 6e61 6d65 295b 305d 0a20 2020 2020  lename)[0].     
-000022e0: 2020 2020 2020 2064 6972 5f70 6174 6820         dir_path 
-000022f0: 3d20 6627 7b70 6174 687d 2f7b 6f72 6967  = f'{path}/{orig
-00002300: 696e 616c 5f66 696c 656e 616d 657d 2f7b  inal_filename}/{
-00002310: 706c 6f74 5f6e 616d 657d 2f27 0a20 2020  plot_name}/'.   
-00002320: 2020 2020 206f 732e 6d61 6b65 6469 7273       os.makedirs
-00002330: 2864 6972 5f70 6174 682c 2065 7869 7374  (dir_path, exist
-00002340: 5f6f 6b3d 5472 7565 290a 2020 2020 2020  _ok=True).      
-00002350: 2020 7265 7475 726e 2064 6972 5f70 6174    return dir_pat
-00002360: 680a 2020 2020 0a20 2020 2069 6620 5f5f  h.    .    if __
-00002370: 6e61 6d65 5f5f 203d 3d20 275f 5f6d 6169  name__ == '__mai
-00002380: 6e5f 5f27 3a0a 2020 2020 2020 2020 6d61  n__':.        ma
-00002390: 696e 2829 0a20 2020 2060 6060 0a0a 2323  in().    ```..##
-000023a0: 2043 6f6e 6669 6775 7269 6e67 2074 6865   Configuring the
-000023b0: 2054 6f6f 6c6b 6974 0a55 7365 7273 2063   Toolkit.Users c
-000023c0: 616e 2070 726f 7669 6465 206d 6574 7269  an provide metri
-000023d0: 6373 206f 7220 6669 6775 7265 7320 746f  cs or figures to
-000023e0: 2062 6520 636f 6d70 7574 6564 2f67 656e   be computed/gen
-000023f0: 6572 6174 6564 2061 6e64 2073 6f6d 6520  erated and some 
-00002400: 6f74 6865 7220 7061 7261 6d65 7465 7269  other parameteri
-00002410: 7361 7469 6f6e 2e20 5468 6520 666f 6c6c  sation. The foll
-00002420: 6f77 696e 6720 636f 6465 2073 6e69 7070  owing code snipp
-00002430: 6574 200a 6372 6561 7465 7320 6120 636f  et .creates a co
-00002440: 6e66 6967 7572 6174 696f 6e20 6f62 6a65  nfiguration obje
-00002450: 6374 2074 6861 7420 7368 6f75 6c64 2062  ct that should b
-00002460: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
-00002470: 6053 696d 696c 6172 6974 7954 7360 2063  `SimilarityTs` c
-00002480: 6f6e 7374 7275 6374 6f72 3a0a 6060 6050  onstructor:.```P
-00002490: 7974 686f 6e0a 6465 6620 5f5f 6372 6561  ython.def __crea
-000024a0: 7465 5f73 696d 696c 6172 6974 795f 7473  te_similarity_ts
-000024b0: 5f63 6f6e 6669 6728 293a 0a20 2020 2023  _config():.    #
-000024c0: 2054 6865 206c 6973 7420 6f66 206d 6574   The list of met
-000024d0: 7269 6373 206e 616d 6573 2074 6861 7420  rics names that 
-000024e0: 7769 6c6c 2062 6520 636f 6d70 7574 6564  will be computed
-000024f0: 0a20 2020 206d 6574 7269 635f 636f 6e66  .    metric_conf
-00002500: 6967 203d 204d 6574 7269 6343 6f6e 6669  ig = MetricConfi
-00002510: 6728 5b27 6a73 272c 2027 6d6d 6427 5d29  g(['js', 'mmd'])
-00002520: 200a 2020 2020 2320 5468 6520 6c69 7374   .    # The list
-00002530: 206f 6620 6669 6775 7265 206e 616d 6573   of figure names
-00002540: 2074 6861 7420 7769 6c6c 2062 6520 6765   that will be ge
-00002550: 6e65 7261 7465 6420 616e 6420 7468 6520  nerated and the 
-00002560: 7469 6d65 2073 7465 7020 696e 2073 6563  time step in sec
-00002570: 6f6e 6473 206f 6620 7468 6520 7469 6d65  onds of the time
-00002580: 2073 6572 6965 732e 0a20 2020 2070 6c6f   series..    plo
-00002590: 745f 636f 6e66 6967 203d 2050 6c6f 7443  t_config = PlotC
-000025a0: 6f6e 6669 6728 5b27 6465 6c74 6127 2c20  onfig(['delta', 
-000025b0: 2770 6361 275d 2c20 7469 6d65 7374 616d  'pca'], timestam
-000025c0: 705f 6672 6571 7565 6e63 795f 7365 636f  p_frequency_seco
-000025d0: 6e64 733d 3330 3029 0a0a 2020 2020 2320  nds=300)..    # 
-000025e0: 4e61 6d65 206f 6620 6561 6368 2074 696d  Name of each tim
-000025f0: 6520 7365 7269 6573 206f 6620 7468 6520  e series of the 
-00002600: 7473 3273 2073 6574 206f 6620 7469 6d65  ts2s set of time
-00002610: 2073 6572 6965 730a 2020 2020 7473 325f   series.    ts2_
-00002620: 6e61 6d65 7320 3d20 5b27 7473 325f 315f  names = ['ts2_1_
-00002630: 6e61 6d65 272c 2027 7473 325f 325f 6e61  name', 'ts2_2_na
-00002640: 6d65 272c 2027 7473 325f 335f 6e61 6d65  me', 'ts2_3_name
-00002650: 272c 2027 7473 325f 345f 6e61 6d65 272c  ', 'ts2_4_name',
-00002660: 2027 7473 325f 355f 6e61 6d65 275d 0a20   'ts2_5_name']. 
-00002670: 2020 2023 204e 616d 6520 6f66 2074 6865     # Name of the
-00002680: 2066 6561 7475 7265 730a 2020 2020 6865   features.    he
-00002690: 6164 6572 5f6e 616d 6573 203d 205b 2766  ader_names = ['f
-000026a0: 6561 7475 7265 315f 6e61 6d65 272c 2027  eature1_name', '
-000026b0: 6665 6174 7572 6532 5f6e 616d 6527 5d0a  feature2_name'].
-000026c0: 2020 2020 0a20 2020 2023 2043 7265 6174      .    # Creat
-000026d0: 696f 6e20 6f66 2074 6865 2063 6f6e 6669  ion of the confi
-000026e0: 6775 7261 7469 6f6e 0a20 2020 2020 2023  guration.      #
-000026f0: 2073 7472 6964 6520 666f 7220 6375 7474   stride for cutt
-00002700: 696e 6720 7468 6520 7473 3120 7768 656e  ing the ts1 when
-00002710: 206e 6565 6465 640a 2020 2020 2020 2320   needed.      # 
-00002720: 6d65 7472 6963 2075 7365 6420 666f 7220  metric used for 
-00002730: 7365 6c65 6374 696e 6720 7468 6520 6d6f  selecting the mo
-00002740: 7374 2073 696d 696c 6172 2077 696e 646f  st similar windo
-00002750: 770a 2020 2020 7369 6d69 6c61 7269 7479  w.    similarity
-00002760: 5f74 735f 636f 6e66 6967 203d 2053 696d  _ts_config = Sim
-00002770: 696c 6172 6974 7954 7343 6f6e 6669 6728  ilarityTsConfig(
-00002780: 6d65 7472 6963 5f63 6f6e 6669 672c 2070  metric_config, p
-00002790: 6c6f 745f 636f 6e66 6967 2c0a 2020 2020  lot_config,.    
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2020 2020 2020 2020 2020 7374 7269 6465            stride
-000027d0: 3d31 302c 2077 696e 646f 775f 7365 6c65  =10, window_sele
-000027e0: 6374 696f 6e5f 6d65 7472 6963 3d27 6b6c  ction_metric='kl
-000027f0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bd0: 733a 0a55 7361 6765 2065 7861 6d70 6c65  s:.Usage example
+00001be0: 7320 6361 6e20 6265 2066 6f75 6e64 2061  s can be found a
+00001bf0: 743a 2068 7474 7073 3a2f 2f67 6974 6875  t: https://githu
+00001c00: 622e 636f 6d2f 616c 656a 616e 6472 6f66  b.com/alejandrof
+00001c10: 6465 7a2d 7573 2f73 696d 696c 6172 6974  dez-us/similarit
+00001c20: 792d 7473 2f74 7265 652f 6d61 696e 2f75  y-ts/tree/main/u
+00001c30: 7361 6765 5f65 7861 6d70 6c65 730a 0a31  sage_examples..1
+00001c40: 2e20 436f 6d70 7574 6520 6d65 7472 6963  . Compute metric
+00001c50: 7320 6265 7477 6565 6e20 7261 6e64 6f6d  s between random
+00001c60: 2074 696d 6520 7365 7269 6573 2028 6074   time series (`t
+00001c70: 7331 603a 206f 6e65 2074 696d 6520 7365  s1`: one time se
+00001c80: 7269 6573 206f 6620 6c65 6e67 6874 2032  ries of lenght 2
+00001c90: 3030 2061 6e64 2032 2064 696d 656e 7369  00 and 2 dimensi
+00001ca0: 6f6e 7320 616e 6420 6074 7332 603a 2066  ons and `ts2`: f
+00001cb0: 6976 6520 7469 6d65 2073 6572 6965 7320  ive time series 
+00001cc0: 6f66 206c 656e 6774 6820 3130 3020 616e  of length 100 an
+00001cd0: 6420 3220 6469 6d65 6e73 696f 6e73 293a  d 2 dimensions):
+00001ce0: 0a20 2020 2060 6060 5079 7468 6f6e 0a20  .    ```Python. 
+00001cf0: 2020 2069 6d70 6f72 7420 6e75 6d70 7920     import numpy 
+00001d00: 6173 206e 700a 2020 2020 6672 6f6d 2073  as np.    from s
+00001d10: 696d 696c 6172 6974 795f 7473 2e73 696d  imilarity_ts.sim
+00001d20: 696c 6172 6974 795f 7473 2069 6d70 6f72  ilarity_ts impor
+00001d30: 7420 5369 6d69 6c61 7269 7479 5473 0a20  t SimilarityTs. 
+00001d40: 2020 200a 2020 2020 7473 3120 3d20 6e70     .    ts1 = np
+00001d50: 2e72 616e 646f 6d2e 7261 6e64 2832 3030  .random.rand(200
+00001d60: 2c20 3229 0a20 2020 2074 7332 7320 3d20  , 2).    ts2s = 
+00001d70: 6e70 2e72 616e 646f 6d2e 7261 6e64 2835  np.random.rand(5
+00001d80: 2c20 3130 302c 2032 290a 2020 2020 7369  , 100, 2).    si
+00001d90: 6d69 6c61 7269 7479 5f74 7320 3d20 5369  milarity_ts = Si
+00001da0: 6d69 6c61 7269 7479 5473 2874 7331 2c20  milarityTs(ts1, 
+00001db0: 7473 3273 290a 2020 2020 666f 7220 7473  ts2s).    for ts
+00001dc0: 325f 6e61 6d65 2c20 6d65 7472 6963 5f6e  2_name, metric_n
+00001dd0: 616d 652c 2063 6f6d 7075 7465 645f 6d65  ame, computed_me
+00001de0: 7472 6963 2069 6e20 7369 6d69 6c61 7269  tric in similari
+00001df0: 7479 5f74 732e 6765 745f 6d65 7472 6963  ty_ts.get_metric
+00001e00: 5f63 6f6d 7075 7465 7228 293a 0a20 2020  _computer():.   
+00001e10: 2020 2020 2070 7269 6e74 2866 277b 7473       print(f'{ts
+00001e20: 325f 6e61 6d65 7d2e 207b 6d65 7472 6963  2_name}. {metric
+00001e30: 5f6e 616d 657d 3a20 7b63 6f6d 7075 7465  _name}: {compute
+00001e40: 645f 6d65 7472 6963 7d27 290a 2020 2020  d_metric}').    
+00001e50: 6060 600a 0a31 2e20 436f 6d70 7574 6520  ```..1. Compute 
+00001e60: 6d65 7472 6963 7320 616e 6420 6669 6775  metrics and figu
+00001e70: 7265 7320 6265 7477 6565 6e20 7261 6e64  res between rand
+00001e80: 6f6d 2074 696d 6520 7365 7269 6573 2061  om time series a
+00001e90: 6e64 2073 6176 6520 6669 6775 7265 733a  nd save figures:
+00001ea0: 0a20 2020 2060 6060 5079 7468 6f6e 0a20  .    ```Python. 
+00001eb0: 2020 2069 6d70 6f72 7420 6f73 0a20 2020     import os.   
+00001ec0: 2069 6d70 6f72 7420 6e75 6d70 7920 6173   import numpy as
+00001ed0: 206e 700a 2020 2020 6672 6f6d 2073 696d   np.    from sim
+00001ee0: 696c 6172 6974 795f 7473 2e70 6c6f 7473  ilarity_ts.plots
+00001ef0: 2e70 6c6f 745f 6661 6374 6f72 7920 696d  .plot_factory im
+00001f00: 706f 7274 2050 6c6f 7446 6163 746f 7279  port PlotFactory
+00001f10: 0a20 2020 2066 726f 6d20 7369 6d69 6c61  .    from simila
+00001f20: 7269 7479 5f74 732e 7369 6d69 6c61 7269  rity_ts.similari
+00001f30: 7479 5f74 7320 696d 706f 7274 2053 696d  ty_ts import Sim
+00001f40: 696c 6172 6974 7954 730a 2020 2020 0a20  ilarityTs.    . 
+00001f50: 2020 2064 6566 206d 6169 6e28 293a 0a20     def main():. 
+00001f60: 2020 2020 2020 2074 7331 203d 206e 702e         ts1 = np.
+00001f70: 7261 6e64 6f6d 2e72 616e 6428 3230 302c  random.rand(200,
+00001f80: 2032 290a 2020 2020 2020 2020 7473 3273   2).        ts2s
+00001f90: 203d 206e 702e 7261 6e64 6f6d 2e72 616e   = np.random.ran
+00001fa0: 6428 352c 2031 3030 2c20 3229 0a20 2020  d(5, 100, 2).   
+00001fb0: 2020 2020 2073 696d 696c 6172 6974 795f       similarity_
+00001fc0: 7473 203d 2053 696d 696c 6172 6974 7954  ts = SimilarityT
+00001fd0: 7328 7473 312c 2074 7332 7329 0a20 2020  s(ts1, ts2s).   
+00001fe0: 2020 2020 2066 6f72 2074 7332 5f6e 616d       for ts2_nam
+00001ff0: 652c 206d 6574 7269 635f 6e61 6d65 2c20  e, metric_name, 
+00002000: 636f 6d70 7574 6564 5f6d 6574 7269 6320  computed_metric 
+00002010: 696e 2073 696d 696c 6172 6974 795f 7473  in similarity_ts
+00002020: 2e67 6574 5f6d 6574 7269 635f 636f 6d70  .get_metric_comp
+00002030: 7574 6572 2829 3a0a 2020 2020 2020 2020  uter():.        
+00002040: 2020 2020 7072 696e 7428 6627 7b74 7332      print(f'{ts2
+00002050: 5f6e 616d 657d 2e20 7b6d 6574 7269 635f  _name}. {metric_
+00002060: 6e61 6d65 7d3a 207b 636f 6d70 7574 6564  name}: {computed
+00002070: 5f6d 6574 7269 637d 2729 0a20 2020 2020  _metric}').     
+00002080: 2020 2066 6f72 2074 7332 5f6e 616d 652c     for ts2_name,
+00002090: 2070 6c6f 745f 6e61 6d65 2c20 6765 6e65   plot_name, gene
+000020a0: 7261 7465 645f 706c 6f74 7320 696e 2073  rated_plots in s
+000020b0: 696d 696c 6172 6974 795f 7473 2e67 6574  imilarity_ts.get
+000020c0: 5f70 6c6f 745f 636f 6d70 7574 6572 2829  _plot_computer()
+000020d0: 3a0a 2020 2020 2020 2020 2020 2020 5f5f  :.            __
+000020e0: 7361 7665 5f66 6967 7572 6573 2874 7332  save_figures(ts2
+000020f0: 5f6e 616d 652c 2070 6c6f 745f 6e61 6d65  _name, plot_name
+00002100: 2c20 6765 6e65 7261 7465 645f 706c 6f74  , generated_plot
+00002110: 7329 0a20 2020 200a 2020 2020 0a20 2020  s).    .    .   
+00002120: 2064 6566 205f 5f73 6176 655f 6669 6775   def __save_figu
+00002130: 7265 7328 6669 6c65 6e61 6d65 2c20 706c  res(filename, pl
+00002140: 6f74 5f6e 616d 652c 2067 656e 6572 6174  ot_name, generat
+00002150: 6564 5f70 6c6f 7473 293a 0a20 2020 2020  ed_plots):.     
+00002160: 2020 2066 6f72 2070 6c6f 7420 696e 2067     for plot in g
+00002170: 656e 6572 6174 6564 5f70 6c6f 7473 3a0a  enerated_plots:.
+00002180: 2020 2020 2020 2020 2020 2020 6469 725f              dir_
+00002190: 7061 7468 203d 205f 5f63 7265 6174 655f  path = __create_
+000021a0: 6469 7265 6374 6f72 7928 6669 6c65 6e61  directory(filena
+000021b0: 6d65 2c20 6627 6669 6775 7265 7327 2c20  me, f'figures', 
+000021c0: 706c 6f74 5f6e 616d 6529 0a20 2020 2020  plot_name).     
+000021d0: 2020 2020 2020 2070 6c6f 745b 305d 2e73         plot[0].s
+000021e0: 6176 6566 6967 2866 277b 6469 725f 7061  avefig(f'{dir_pa
+000021f0: 7468 7d7b 706c 6f74 5b30 5d2e 6178 6573  th}{plot[0].axes
+00002200: 5b30 5d2e 6765 745f 7469 746c 6528 297d  [0].get_title()}
+00002210: 2e70 6466 272c 2066 6f72 6d61 743d 2770  .pdf', format='p
+00002220: 6466 272c 2062 626f 785f 696e 6368 6573  df', bbox_inches
+00002230: 3d27 7469 6768 7427 290a 2020 2020 0a20  ='tight').    . 
+00002240: 2020 200a 2020 2020 6465 6620 5f5f 6372     .    def __cr
+00002250: 6561 7465 5f64 6972 6563 746f 7279 2866  eate_directory(f
+00002260: 696c 656e 616d 652c 2070 6174 682c 2070  ilename, path, p
+00002270: 6c6f 745f 6e61 6d65 293a 0a20 2020 2020  lot_name):.     
+00002280: 2020 2069 6620 706c 6f74 5f6e 616d 6520     if plot_name 
+00002290: 696e 2050 6c6f 7446 6163 746f 7279 2e67  in PlotFactory.g
+000022a0: 6574 5f69 6e73 7461 6e63 6528 292e 6669  et_instance().fi
+000022b0: 6775 7265 735f 7265 7175 6972 6573 5f61  gures_requires_a
+000022c0: 6c6c 5f73 616d 706c 6573 3a0a 2020 2020  ll_samples:.    
+000022d0: 2020 2020 2020 2020 6469 725f 7061 7468          dir_path
+000022e0: 203d 2066 277b 7061 7468 7d2f 7b70 6c6f   = f'{path}/{plo
+000022f0: 745f 6e61 6d65 7d2f 270a 2020 2020 2020  t_name}/'.      
+00002300: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00002310: 2020 2020 6f72 6967 696e 616c 5f66 696c      original_fil
+00002320: 656e 616d 6520 3d20 6f73 2e70 6174 682e  ename = os.path.
+00002330: 7370 6c69 7465 7874 2866 696c 656e 616d  splitext(filenam
+00002340: 6529 5b30 5d0a 2020 2020 2020 2020 2020  e)[0].          
+00002350: 2020 6469 725f 7061 7468 203d 2066 277b    dir_path = f'{
+00002360: 7061 7468 7d2f 7b6f 7269 6769 6e61 6c5f  path}/{original_
+00002370: 6669 6c65 6e61 6d65 7d2f 7b70 6c6f 745f  filename}/{plot_
+00002380: 6e61 6d65 7d2f 270a 2020 2020 2020 2020  name}/'.        
+00002390: 6f73 2e6d 616b 6564 6972 7328 6469 725f  os.makedirs(dir_
+000023a0: 7061 7468 2c20 6578 6973 745f 6f6b 3d54  path, exist_ok=T
+000023b0: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
+000023c0: 7572 6e20 6469 725f 7061 7468 0a20 2020  urn dir_path.   
+000023d0: 200a 2020 2020 6966 205f 5f6e 616d 655f   .    if __name_
+000023e0: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
+000023f0: 0a20 2020 2020 2020 206d 6169 6e28 290a  .        main().
+00002400: 2020 2020 6060 600a 0a23 2320 436f 6e66      ```..## Conf
+00002410: 6967 7572 696e 6720 7468 6520 546f 6f6c  iguring the Tool
+00002420: 6b69 740a 5573 6572 7320 6361 6e20 7072  kit.Users can pr
+00002430: 6f76 6964 6520 6d65 7472 6963 7320 6f72  ovide metrics or
+00002440: 2066 6967 7572 6573 2074 6f20 6265 2063   figures to be c
+00002450: 6f6d 7075 7465 642f 6765 6e65 7261 7465  omputed/generate
+00002460: 6420 616e 6420 736f 6d65 206f 7468 6572  d and some other
+00002470: 2070 6172 616d 6574 6572 6973 6174 696f   parameterisatio
+00002480: 6e2e 2054 6865 2066 6f6c 6c6f 7769 6e67  n. The following
+00002490: 2063 6f64 6520 736e 6970 7065 7420 0a63   code snippet .c
+000024a0: 7265 6174 6573 2061 2063 6f6e 6669 6775  reates a configu
+000024b0: 7261 7469 6f6e 206f 626a 6563 7420 7468  ration object th
+000024c0: 6174 2073 686f 756c 6420 6265 2070 6173  at should be pas
+000024d0: 7365 6420 746f 2074 6865 2060 5369 6d69  sed to the `Simi
+000024e0: 6c61 7269 7479 5473 6020 636f 6e73 7472  larityTs` constr
+000024f0: 7563 746f 723a 0a60 6060 5079 7468 6f6e  uctor:.```Python
+00002500: 0a64 6566 205f 5f63 7265 6174 655f 7369  .def __create_si
+00002510: 6d69 6c61 7269 7479 5f74 735f 636f 6e66  milarity_ts_conf
+00002520: 6967 2829 3a0a 2020 2020 2320 5468 6520  ig():.    # The 
+00002530: 6c69 7374 206f 6620 6d65 7472 6963 7320  list of metrics 
+00002540: 6e61 6d65 7320 7468 6174 2077 696c 6c20  names that will 
+00002550: 6265 2063 6f6d 7075 7465 640a 2020 2020  be computed.    
+00002560: 6d65 7472 6963 5f63 6f6e 6669 6720 3d20  metric_config = 
+00002570: 4d65 7472 6963 436f 6e66 6967 285b 276a  MetricConfig(['j
+00002580: 7327 2c20 276d 6d64 275d 2920 0a20 2020  s', 'mmd']) .   
+00002590: 2023 2054 6865 206c 6973 7420 6f66 2066   # The list of f
+000025a0: 6967 7572 6520 6e61 6d65 7320 7468 6174  igure names that
+000025b0: 2077 696c 6c20 6265 2067 656e 6572 6174   will be generat
+000025c0: 6564 2061 6e64 2074 6865 2074 696d 6520  ed and the time 
+000025d0: 7374 6570 2069 6e20 7365 636f 6e64 7320  step in seconds 
+000025e0: 6f66 2074 6865 2074 696d 6520 7365 7269  of the time seri
+000025f0: 6573 2e0a 2020 2020 706c 6f74 5f63 6f6e  es..    plot_con
+00002600: 6669 6720 3d20 506c 6f74 436f 6e66 6967  fig = PlotConfig
+00002610: 285b 2764 656c 7461 272c 2027 7063 6127  (['delta', 'pca'
+00002620: 5d2c 2074 696d 6573 7461 6d70 5f66 7265  ], timestamp_fre
+00002630: 7175 656e 6379 5f73 6563 6f6e 6473 3d33  quency_seconds=3
+00002640: 3030 290a 0a20 2020 2023 204e 616d 6520  00)..    # Name 
+00002650: 6f66 2065 6163 6820 7469 6d65 2073 6572  of each time ser
+00002660: 6965 7320 6f66 2074 6865 2074 7332 7320  ies of the ts2s 
+00002670: 7365 7420 6f66 2074 696d 6520 7365 7269  set of time seri
+00002680: 6573 0a20 2020 2074 7332 5f6e 616d 6573  es.    ts2_names
+00002690: 203d 205b 2774 7332 5f31 5f6e 616d 6527   = ['ts2_1_name'
+000026a0: 2c20 2774 7332 5f32 5f6e 616d 6527 2c20  , 'ts2_2_name', 
+000026b0: 2774 7332 5f33 5f6e 616d 6527 2c20 2774  'ts2_3_name', 't
+000026c0: 7332 5f34 5f6e 616d 6527 2c20 2774 7332  s2_4_name', 'ts2
+000026d0: 5f35 5f6e 616d 6527 5d0a 2020 2020 2320  _5_name'].    # 
+000026e0: 4e61 6d65 206f 6620 7468 6520 6665 6174  Name of the feat
+000026f0: 7572 6573 0a20 2020 2068 6561 6465 725f  ures.    header_
+00002700: 6e61 6d65 7320 3d20 5b27 6665 6174 7572  names = ['featur
+00002710: 6531 5f6e 616d 6527 2c20 2766 6561 7475  e1_name', 'featu
+00002720: 7265 325f 6e61 6d65 275d 0a20 2020 200a  re2_name'].    .
+00002730: 2020 2020 2320 4372 6561 7469 6f6e 206f      # Creation o
+00002740: 6620 7468 6520 636f 6e66 6967 7572 6174  f the configurat
+00002750: 696f 6e0a 2020 2020 2020 2320 7374 7269  ion.      # stri
+00002760: 6465 2066 6f72 2063 7574 7469 6e67 2074  de for cutting t
+00002770: 6865 2074 7331 2077 6865 6e20 6e65 6564  he ts1 when need
+00002780: 6564 0a20 2020 2020 2023 206d 6574 7269  ed.      # metri
+00002790: 6320 7573 6564 2066 6f72 2073 656c 6563  c used for selec
+000027a0: 7469 6e67 2074 6865 206d 6f73 7420 7369  ting the most si
+000027b0: 6d69 6c61 7220 7769 6e64 6f77 0a20 2020  milar window.   
+000027c0: 2073 696d 696c 6172 6974 795f 7473 5f63   similarity_ts_c
+000027d0: 6f6e 6669 6720 3d20 5369 6d69 6c61 7269  onfig = Similari
+000027e0: 7479 5473 436f 6e66 6967 286d 6574 7269  tyTsConfig(metri
+000027f0: 635f 636f 6e66 6967 2c20 706c 6f74 5f63  c_config, plot_c
+00002800: 6f6e 6669 672c 0a20 2020 2020 2020 2020  onfig,.         
 00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002820: 2074 7332 5f6e 616d 6573 3d74 7332 5f6e   ts2_names=ts2_n
-00002830: 616d 6573 2c20 6865 6164 6572 5f6e 616d  ames, header_nam
-00002840: 6573 3d68 6561 6465 725f 6e61 6d65 7329  es=header_names)
-00002850: 0a20 2020 2072 6574 7572 6e20 7369 6d69  .    return simi
-00002860: 6c61 7269 7479 5f74 735f 636f 6e66 6967  larity_ts_config
-00002870: 0a60 6060 0a0a 4966 206e 6f20 6d65 7472  .```..If no metr
-00002880: 6963 7320 6e6f 7220 6669 6775 7265 7320  ics nor figures 
-00002890: 6172 6520 7072 6f76 6964 6564 2c20 7468  are provided, th
-000028a0: 6520 746f 6f6c 2077 696c 6c20 636f 6d70  e tool will comp
-000028b0: 7574 6520 616c 6c20 7468 6520 6176 6169  ute all the avai
-000028c0: 6c61 626c 6520 6d65 7472 6963 7320 616e  lable metrics an
-000028d0: 6420 6669 6775 7265 732e 0a0a 5468 6520  d figures...The 
-000028e0: 666f 6c6c 6f77 696e 6720 6172 6775 6d65  following argume
-000028f0: 6e74 7320 6172 6520 616c 736f 2061 7661  nts are also ava
-00002900: 696c 6162 6c65 2066 6f72 2066 696e 652d  ilable for fine-
-00002910: 7475 6e69 6e67 3a0a 0a2d 2060 7469 6d65  tuning:..- `time
-00002920: 7374 616d 705f 6672 6571 7565 6e63 795f  stamp_frequency_
-00002930: 7365 636f 6e64 7360 3a20 7468 6520 6672  seconds`: the fr
-00002940: 6571 7565 6e63 7920 696e 2073 6563 6f6e  equency in secon
-00002950: 6473 2069 6e20 7768 6963 6820 7361 6d70  ds in which samp
-00002960: 6c65 7320 7765 7265 2074 616b 656e 2e20  les were taken. 
-00002970: 5468 6973 2069 7320 6e65 6564 6564 2074  This is needed t
-00002980: 6f20 6765 6e65 7261 7465 2074 6865 2064  o generate the d
-00002990: 656c 7461 2066 6967 7572 6573 2077 6974  elta figures wit
-000029a0: 6820 636f 7272 6563 7420 7469 6d65 206d  h correct time m
-000029b0: 6167 6e69 7475 6465 732e 2042 7920 6465  agnitudes. By de
-000029c0: 6661 756c 7420 6973 0a20 2060 3160 2073  fault is.  `1` s
-000029d0: 6563 6f6e 642e 0a2d 2060 7374 7269 6465  econd..- `stride
-000029e0: 603a 2077 6865 6e20 6074 7331 6020 7469  `: when `ts1` ti
-000029f0: 6d65 2d73 6572 6965 7320 6973 206c 6f6e  me-series is lon
-00002a00: 6765 7220 7468 616e 2060 7473 3273 6020  ger than `ts2s` 
-00002a10: 7469 6d65 2d73 6572 6965 7320 7468 6520  time-series the 
-00002a20: 7769 6e64 6f77 7320 6172 6520 636f 6d70  windows are comp
-00002a30: 7574 6564 2062 7920 7573 696e 6720 610a  uted by using a.
-00002a40: 2020 7374 7269 6465 206f 6620 6031 6020    stride of `1` 
-00002a50: 6279 2064 6566 6175 6c74 2e20 536f 6d65  by default. Some
-00002a60: 7469 6d65 7320 7573 696e 6720 6120 6c61  times using a la
-00002a70: 7267 6572 2076 616c 7565 2066 6f72 2074  rger value for t
-00002a80: 6865 2073 7472 6964 6520 7061 7261 6d65  he stride parame
-00002a90: 7465 7220 696d 7072 6f76 6573 2074 6865  ter improves the
-00002aa0: 2070 6572 666f 726d 616e 6365 2062 7920   performance by 
-00002ab0: 736b 6970 7069 6e67 0a20 2074 6865 2063  skipping.  the c
-00002ac0: 6f6d 7075 7461 7469 6f6e 206f 6620 7369  omputation of si
-00002ad0: 6d69 6c61 7269 7479 2062 6574 7765 656e  milarity between
-00002ae0: 2073 6f20 6d61 6e79 2077 696e 646f 7773   so many windows
-00002af0: 2e0a 2d20 6077 696e 646f 775f 7365 6c65  ..- `window_sele
-00002b00: 6374 696f 6e5f 6d65 7472 6963 603a 2074  ction_metric`: t
-00002b10: 6865 206d 6574 7269 6320 7573 6564 2066  he metric used f
-00002b20: 6f72 2074 6865 2073 656c 6563 7469 6f6e  or the selection
-00002b30: 206f 6620 7468 6520 6d6f 7374 2073 696d   of the most sim
-00002b40: 696c 6172 2060 7473 3160 2074 696d 652d  ilar `ts1` time-
-00002b50: 7365 7269 6573 2077 696e 646f 7720 7065  series window pe
-00002b60: 7220 6561 6368 2060 7473 3273 6020 7469  r each `ts2s` ti
-00002b70: 6d65 2d73 6572 6965 7320 6669 6c65 2069  me-series file i
-00002b80: 7320 7365 6c65 6374 6162 6c65 2e60 6474  s selectable.`dt
-00002b90: 7760 2069 7320 7468 6520 6465 6661 756c  w` is the defaul
-00002ba0: 7420 7365 6c65 6374 6564 206d 6574 7269  t selected metri
-00002bb0: 632c 2068 6f77 6576 6572 2c20 616e 7920  c, however, any 
-00002bc0: 6f66 2074 6865 205b 6d65 7472 6963 735d  of the [metrics]
-00002bd0: 2823 6176 6169 6c61 626c 652d 6d65 7472  (#available-metr
-00002be0: 6963 7329 2061 7265 2061 6c73 6f20 6176  ics) are also av
-00002bf0: 6169 6c61 626c 6520 666f 7220 7468 6973  ailable for this
-00002c00: 2070 7572 706f 7365 2e20 5365 6520 7468   purpose. See th
-00002c10: 6520 5b74 6f6f 6c6b 6974 2063 6f6e 6669  e [toolkit confi
-00002c20: 6775 7261 7469 6f6e 2073 6563 7469 6f6e  guration section
-00002c30: 5d28 2363 6f6e 6669 6775 7269 6e67 2d74  ](#configuring-t
-00002c40: 6865 2d74 6f6f 6c6b 6974 292e 0a2d 2060  he-toolkit)..- `
-00002c50: 7473 325f 6e61 6d65 7360 3a20 6e61 6d65  ts2_names`: name
-00002c60: 206f 6620 6561 6368 2074 696d 6520 7365   of each time se
-00002c70: 7269 6573 206f 6620 7468 6520 6074 7332  ries of the `ts2
-00002c80: 7360 2073 6574 206f 6620 7469 6d65 2073  s` set of time s
-00002c90: 6572 6965 732e 0a2d 2060 6865 6164 6572  eries..- `header
-00002ca0: 5f6e 616d 6573 603a 206e 616d 6520 6f66  _names`: name of
-00002cb0: 2074 6865 2066 6561 7475 7265 730a 0a0a   the features...
-00002cc0: 2323 2045 7874 656e 6469 6e67 2074 6865  ## Extending the
-00002cd0: 2074 6f6f 6c6b 6974 0a0a 4164 6469 7469   toolkit..Additi
-00002ce0: 6f6e 616c 6c79 2c20 7573 6572 7320 6d61  onally, users ma
-00002cf0: 7920 696d 706c 656d 656e 7420 7468 6569  y implement thei
-00002d00: 7220 6f77 6e20 6d65 7472 6963 206f 7220  r own metric or 
-00002d10: 6669 6775 7265 2063 6c61 7373 6573 2061  figure classes a
-00002d20: 6e64 2069 6e63 6c75 6465 2074 6865 6d20  nd include them 
-00002d30: 6279 2075 7369 6e67 2074 6865 2060 4d65  by using the `Me
-00002d40: 7472 6963 4661 6374 6f72 7960 206f 7220  tricFactory` or 
-00002d50: 6050 6c6f 7446 6163 746f 7279 6020 7265  `PlotFactory` re
-00002d60: 6769 7374 6572 206d 6574 686f 6473 2e20  gister methods. 
-00002d70: 546f 2065 6e73 7572 6520 636f 6d70 6174  To ensure compat
-00002d80: 6962 696c 6974 7920 7769 7468 206f 7572  ibility with our
-00002d90: 2074 6f6f 6c6b 6974 2c20 7468 6579 2068   toolkit, they h
-00002da0: 6176 6520 746f 2069 6e68 6572 6974 2066  ave to inherit f
-00002db0: 726f 6d20 7468 6520 6261 7365 2063 6c61  rom the base cla
-00002dc0: 7373 6573 2060 4d65 7472 6963 6020 616e  sses `Metric` an
-00002dd0: 6420 6050 6c6f 7460 2e0a 0a54 6865 2066  d `Plot`...The f
-00002de0: 6f6c 6c6f 7769 6e67 2063 6f64 6520 736e  ollowing code sn
-00002df0: 6970 7065 7420 6973 2061 6e20 6578 616d  ippet is an exam
-00002e00: 706c 6520 6f66 2068 6f77 2074 6f20 696e  ple of how to in
-00002e10: 7472 6f64 7563 6520 7468 6520 4575 636c  troduce the Eucl
-00002e20: 6964 6561 6e20 6469 7374 616e 6365 206d  idean distance m
-00002e30: 6574 7269 633a 0a0a 6060 6050 7974 686f  etric:..```Pytho
-00002e40: 6e0a 2365 752e 7079 0a69 6d70 6f72 7420  n.#eu.py.import 
-00002e50: 6e75 6d70 7920 6173 206e 700a 6672 6f6d  numpy as np.from
-00002e60: 2073 696d 696c 6172 6974 795f 7473 2e6d   similarity_ts.m
-00002e70: 6574 7269 6373 2e6d 6574 7269 6320 696d  etrics.metric im
-00002e80: 706f 7274 204d 6574 7269 630a 0a0a 636c  port Metric...cl
-00002e90: 6173 7320 4575 636c 6964 6561 6e44 6973  ass EuclideanDis
-00002ea0: 7461 6e63 6528 4d65 7472 6963 293a 0a0a  tance(Metric):..
-00002eb0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00002ec0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00002ed0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00002ee0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00002ef0: 6e61 6d65 203d 2027 6564 270a 0a20 2020  name = 'ed'..   
-00002f00: 2064 6566 2063 6f6d 7075 7465 2873 656c   def compute(sel
-00002f10: 662c 2074 7331 2c20 7473 322c 2073 696d  f, ts1, ts2, sim
-00002f20: 696c 6172 6974 795f 7473 293a 0a20 2020  ilarity_ts):.   
-00002f30: 2020 2020 206d 6574 7269 635f 7265 7375       metric_resu
-00002f40: 6c74 203d 207b 274d 756c 7469 7661 7269  lt = {'Multivari
-00002f50: 6174 6527 3a20 7365 6c66 2e5f 5f65 6428  ate': self.__ed(
-00002f60: 7473 312c 2074 7332 297d 0a20 2020 2020  ts1, ts2)}.     
-00002f70: 2020 2072 6574 7572 6e20 6d65 7472 6963     return metric
-00002f80: 5f72 6573 756c 740a 0a20 2020 2064 6566  _result..    def
-00002f90: 2063 6f6d 7075 7465 5f64 6973 7461 6e63   compute_distanc
-00002fa0: 6528 7365 6c66 2c20 7473 312c 2074 7332  e(self, ts1, ts2
-00002fb0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00002fc0: 6e20 7365 6c66 2e5f 5f65 6428 7473 312c  n self.__ed(ts1,
-00002fd0: 2074 7332 290a 0a20 2020 2064 6566 205f   ts2)..    def _
-00002fe0: 5f65 6428 7365 6c66 2c20 7473 312c 2074  _ed(self, ts1, t
-00002ff0: 7332 293a 0a20 2020 2020 2020 2072 6574  s2):.        ret
-00003000: 7572 6e20 6e70 2e6c 696e 616c 672e 6e6f  urn np.linalg.no
-00003010: 726d 2874 7331 202d 2074 7332 290a 0a60  rm(ts1 - ts2)..`
-00003020: 6060 0a0a 4166 7465 7277 6172 642c 2074  ``..Afterward, t
-00003030: 6869 7320 6d65 7472 6963 2063 616e 2062  his metric can b
-00003040: 6520 7265 6769 7374 6572 6564 2062 7920  e registered by 
-00003050: 7573 696e 6720 7468 6520 6072 6567 6973  using the `regis
-00003060: 7465 725f 6d65 7472 6963 286d 6574 7269  ter_metric(metri
-00003070: 635f 636c 6173 7329 6020 6d65 7468 6f64  c_class)` method
-00003080: 2066 726f 6d20 604d 6574 7269 6346 6163   from `MetricFac
-00003090: 746f 7279 6020 6173 2073 686f 776e 2069  tory` as shown i
-000030a0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-000030b0: 636f 6465 2073 6e69 7070 6574 3a0a 6060  code snippet:.``
-000030c0: 6050 7974 686f 6e0a 696d 706f 7274 206e  `Python.import n
-000030d0: 756d 7079 2061 7320 6e70 0a66 726f 6d20  umpy as np.from 
-000030e0: 7369 6d69 6c61 7269 7479 5f74 732e 7369  similarity_ts.si
-000030f0: 6d69 6c61 7269 7479 5f74 7320 696d 706f  milarity_ts impo
-00003100: 7274 2053 696d 696c 6172 6974 7954 730a  rt SimilarityTs.
-00003110: 6672 6f6d 2073 696d 696c 6172 6974 795f  from similarity_
-00003120: 7473 2e6d 6574 7269 6373 2e6d 6574 7269  ts.metrics.metri
-00003130: 635f 6661 6374 6f72 7920 696d 706f 7274  c_factory import
-00003140: 204d 6574 7269 6346 6163 746f 7279 0a66   MetricFactory.f
-00003150: 726f 6d20 6564 2069 6d70 6f72 7420 4575  rom ed import Eu
-00003160: 636c 6964 6561 6e44 6973 7461 6e63 650a  clideanDistance.
-00003170: 0a4d 6574 7269 6346 6163 746f 7279 2e67  .MetricFactory.g
-00003180: 6574 5f69 6e73 7461 6e63 6528 292e 7265  et_instance().re
-00003190: 6769 7374 6572 5f6d 6574 7269 6328 4575  gister_metric(Eu
-000031a0: 636c 6964 6561 6e44 6973 7461 6e63 6529  clideanDistance)
-000031b0: 0a74 7331 203d 206e 702e 7261 6e64 6f6d  .ts1 = np.random
-000031c0: 2e72 616e 6428 3230 302c 2032 290a 7473  .rand(200, 2).ts
-000031d0: 3273 203d 206e 702e 7261 6e64 6f6d 2e72  2s = np.random.r
-000031e0: 616e 6428 352c 2031 3030 2c20 3229 0a73  and(5, 100, 2).s
-000031f0: 696d 696c 6172 6974 795f 7473 203d 2053  imilarity_ts = S
-00003200: 696d 696c 6172 6974 7954 7328 7473 312c  imilarityTs(ts1,
-00003210: 2074 7332 7329 0a66 6f72 2074 7332 5f6e   ts2s).for ts2_n
-00003220: 616d 652c 206d 6574 7269 635f 6e61 6d65  ame, metric_name
-00003230: 2c20 636f 6d70 7574 6564 5f6d 6574 7269  , computed_metri
-00003240: 6320 696e 2073 696d 696c 6172 6974 795f  c in similarity_
-00003250: 7473 2e67 6574 5f6d 6574 7269 635f 636f  ts.get_metric_co
-00003260: 6d70 7574 6572 2829 3a0a 2020 2020 7072  mputer():.    pr
-00003270: 696e 7428 6627 7b74 7332 5f6e 616d 657d  int(f'{ts2_name}
-00003280: 2e20 7b6d 6574 7269 635f 6e61 6d65 7d3a  . {metric_name}:
-00003290: 207b 636f 6d70 7574 6564 5f6d 6574 7269   {computed_metri
-000032a0: 637d 2729 0a60 6060 0a0a 5369 6d69 6c61  c}').```..Simila
-000032b0: 726c 792c 206e 6577 2070 6c6f 7473 2063  rly, new plots c
-000032c0: 616e 2062 6520 696e 7472 6f64 7563 6564  an be introduced
-000032d0: 2e20 466f 7220 696e 7374 616e 6365 2061  . For instance a
-000032e0: 2060 5369 6d69 6c61 7269 7479 506c 6f74   `SimilarityPlot
-000032f0: 4279 436f 7272 656c 6174 696f 6e60 2063  ByCorrelation` c
-00003300: 6f75 6c64 2062 6520 6465 6669 6e65 6420  ould be defined 
-00003310: 6173 3a0a 6060 6050 7974 686f 6e0a 2363  as:.```Python.#c
-00003320: 635f 706c 6f74 2e70 790a 696d 706f 7274  c_plot.py.import
-00003330: 206e 756d 7079 2061 7320 6e70 0a69 6d70   numpy as np.imp
-00003340: 6f72 7420 6d61 7470 6c6f 746c 6962 2e70  ort matplotlib.p
-00003350: 7970 6c6f 7420 6173 2070 6c74 0a66 726f  yplot as plt.fro
-00003360: 6d20 7369 6d69 6c61 7269 7479 5f74 732e  m similarity_ts.
-00003370: 706c 6f74 732e 706c 6f74 2069 6d70 6f72  plots.plot impor
-00003380: 7420 506c 6f74 0a0a 0a63 6c61 7373 2053  t Plot...class S
-00003390: 696d 696c 6172 6974 7950 6c6f 7442 7943  imilarityPlotByC
-000033a0: 6f72 7265 6c61 7469 6f6e 2850 6c6f 7429  orrelation(Plot)
-000033b0: 3a0a 0a20 2020 2064 6566 205f 5f69 6e69  :..    def __ini
-000033c0: 745f 5f28 7365 6c66 2c20 6669 675f 7369  t__(self, fig_si
-000033d0: 7a65 3d28 382c 2036 2929 3a0a 2020 2020  ze=(8, 6)):.    
-000033e0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-000033f0: 6974 5f5f 2866 6967 5f73 697a 6529 0a20  it__(fig_size). 
-00003400: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
-00003410: 203d 2027 6363 2d70 6c6f 7427 0a0a 2020   = 'cc-plot'..  
-00003420: 2020 6465 6620 636f 6d70 7574 6528 7365    def compute(se
-00003430: 6c66 2c20 7369 6d69 6c61 7269 7479 5f74  lf, similarity_t
-00003440: 732c 2074 7332 5f66 696c 656e 616d 6529  s, ts2_filename)
-00003450: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
-00003460: 292e 636f 6d70 7574 6528 7369 6d69 6c61  ).compute(simila
-00003470: 7269 7479 5f74 732c 2074 7332 5f66 696c  rity_ts, ts2_fil
-00003480: 656e 616d 6529 0a20 2020 2020 2020 206e  ename).        n
-00003490: 5f66 6561 7475 7265 7320 3d20 7365 6c66  _features = self
-000034a0: 2e74 7331 2e73 6861 7065 5b31 5d0a 2020  .ts1.shape[1].  
-000034b0: 2020 2020 2020 7369 6d69 6c61 7269 7479        similarity
-000034c0: 203d 206e 702e 636f 7272 636f 6566 2873   = np.corrcoef(s
-000034d0: 656c 662e 7473 312e 542c 2073 656c 662e  elf.ts1.T, self.
-000034e0: 7473 322e 5429 0a20 2020 2020 2020 2066  ts2.T).        f
-000034f0: 6967 2c20 6178 203d 2070 6c74 2e73 7562  ig, ax = plt.sub
-00003500: 706c 6f74 7328 290a 2020 2020 2020 2020  plots().        
-00003510: 696d 203d 2061 782e 696d 7368 6f77 2873  im = ax.imshow(s
-00003520: 696d 696c 6172 6974 792c 2063 6d61 703d  imilarity, cmap=
-00003530: 2752 6459 6c42 7527 2c20 766d 696e 3d2d  'RdYlBu', vmin=-
-00003540: 312c 2076 6d61 783d 3129 0a20 2020 2020  1, vmax=1).     
-00003550: 2020 2061 782e 7365 745f 7874 6963 6b73     ax.set_xticks
-00003560: 286e 702e 6172 616e 6765 286e 5f66 6561  (np.arange(n_fea
-00003570: 7475 7265 732a 3229 290a 2020 2020 2020  tures*2)).      
-00003580: 2020 6178 2e73 6574 5f79 7469 636b 7328    ax.set_yticks(
-00003590: 6e70 2e61 7261 6e67 6528 6e5f 6665 6174  np.arange(n_feat
-000035a0: 7572 6573 2a32 2929 0a20 2020 2020 2020  ures*2)).       
-000035b0: 2078 7469 636b 6c61 6265 6c73 203d 205b   xticklabels = [
-000035c0: 6627 7473 315f 7b6e 6665 6174 7572 6573  f'ts1_{nfeatures
-000035d0: 5f69 6e64 6578 7d27 666f 7220 6e66 6561  _index}'for nfea
-000035e0: 7475 7265 735f 696e 6465 7820 696e 2072  tures_index in r
-000035f0: 616e 6765 2831 2c20 6e5f 6665 6174 7572  ange(1, n_featur
-00003600: 6573 2b31 295d 0a20 2020 2020 2020 2078  es+1)].        x
-00003610: 7469 636b 6c61 6265 6c73 203d 2078 7469  ticklabels = xti
-00003620: 636b 6c61 6265 6c73 202b 205b 6627 7473  cklabels + [f'ts
-00003630: 325f 7b6e 6665 6174 7572 6573 5f69 6e64  2_{nfeatures_ind
-00003640: 6578 7d27 666f 7220 6e66 6561 7475 7265  ex}'for nfeature
-00003650: 735f 696e 6465 7820 696e 2072 616e 6765  s_index in range
-00003660: 2831 2c20 6e5f 6665 6174 7572 6573 2b31  (1, n_features+1
-00003670: 295d 0a20 2020 2020 2020 2061 782e 7365  )].        ax.se
-00003680: 745f 7874 6963 6b6c 6162 656c 7328 7874  t_xticklabels(xt
-00003690: 6963 6b6c 6162 656c 7329 0a20 2020 2020  icklabels).     
-000036a0: 2020 2061 782e 7365 745f 7974 6963 6b6c     ax.set_ytickl
-000036b0: 6162 656c 7328 7874 6963 6b6c 6162 656c  abels(xticklabel
-000036c0: 7329 0a20 2020 2020 2020 2061 782e 7365  s).        ax.se
-000036d0: 745f 786c 6162 656c 2827 4665 6174 7572  t_xlabel('Featur
-000036e0: 6527 290a 2020 2020 2020 2020 6178 2e73  e').        ax.s
-000036f0: 6574 5f79 6c61 6265 6c28 2746 6561 7475  et_ylabel('Featu
-00003700: 7265 2729 0a20 2020 2020 2020 2066 6f72  re').        for
-00003710: 2069 2069 6e20 7261 6e67 6528 6e5f 6665   i in range(n_fe
-00003720: 6174 7572 6573 2a32 293a 0a20 2020 2020  atures*2):.     
-00003730: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-00003740: 7261 6e67 6528 6e5f 6665 6174 7572 6573  range(n_features
-00003750: 2a32 293a 0a20 2020 2020 2020 2020 2020  *2):.           
-00003760: 2020 2020 2061 782e 7465 7874 286a 2c20       ax.text(j, 
-00003770: 692c 2066 277b 7369 6d69 6c61 7269 7479  i, f'{similarity
-00003780: 5b69 2c20 6a5d 3a2e 3266 7d27 2c20 6861  [i, j]:.2f}', ha
-00003790: 3d27 6365 6e74 6572 272c 2076 613d 2763  ='center', va='c
-000037a0: 656e 7465 7227 2c20 636f 6c6f 723d 2762  enter', color='b
-000037b0: 6c61 636b 2729 0a0a 2020 2020 2020 2020  lack')..        
-000037c0: 6362 6172 203d 2061 782e 6669 6775 7265  cbar = ax.figure
-000037d0: 2e63 6f6c 6f72 6261 7228 696d 2c20 6178  .colorbar(im, ax
-000037e0: 3d61 7829 0a20 2020 2020 2020 2063 6261  =ax).        cba
-000037f0: 722e 6178 2e73 6574 5f79 6c61 6265 6c28  r.ax.set_ylabel(
-00003800: 2753 696d 696c 6172 6974 7927 2c20 726f  'Similarity', ro
-00003810: 7461 7469 6f6e 3d2d 3930 2c20 7661 3d27  tation=-90, va='
-00003820: 626f 7474 6f6d 2729 0a20 2020 2020 2020  bottom').       
-00003830: 2070 6c74 2e74 6974 6c65 2827 7369 6d69   plt.title('simi
-00003840: 6c61 7269 7479 2d63 6f72 7265 6c61 7469  larity-correlati
-00003850: 6f6e 2729 0a20 2020 2020 2020 2070 6c74  on').        plt
-00003860: 2e74 6967 6874 5f6c 6179 6f75 7428 290a  .tight_layout().
-00003870: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00003880: 2866 6967 2c20 6178 295d 0a60 6060 0a0a  (fig, ax)].```..
-00003890: 4166 7465 7277 6172 642c 2074 6869 7320  Afterward, this 
-000038a0: 706c 6f74 2063 616e 2062 6520 7265 6769  plot can be regi
-000038b0: 7374 6572 6564 2062 7920 7573 696e 6720  stered by using 
-000038c0: 7468 6520 6072 6567 6973 7465 725f 706c  the `register_pl
-000038d0: 6f74 2870 6c6f 745f 636c 6173 7329 6020  ot(plot_class)` 
-000038e0: 6d65 7468 6f64 2066 726f 6d20 6050 6c6f  method from `Plo
-000038f0: 7446 6163 746f 7279 6020 6173 2073 686f  tFactory` as sho
-00003900: 776e 2069 6e20 7468 6520 666f 6c6c 6f77  wn in the follow
-00003910: 696e 6720 636f 6465 2073 6e69 7070 6574  ing code snippet
-00003920: 2074 6861 7420 7265 6769 7374 6572 2074   that register t
-00003930: 6865 206e 6577 206d 6574 7269 6320 616e  he new metric an
-00003940: 6420 7468 6520 6e65 7720 706c 6f74 3a0a  d the new plot:.
-00003950: 6060 6050 7974 686f 6e0a 696d 706f 7274  ```Python.import
-00003960: 206f 730a 696d 706f 7274 206e 756d 7079   os.import numpy
-00003970: 2061 7320 6e70 0a66 726f 6d20 7369 6d69   as np.from simi
-00003980: 6c61 7269 7479 5f74 732e 706c 6f74 732e  larity_ts.plots.
-00003990: 706c 6f74 5f66 6163 746f 7279 2069 6d70  plot_factory imp
-000039a0: 6f72 7420 506c 6f74 4661 6374 6f72 790a  ort PlotFactory.
-000039b0: 6672 6f6d 2073 696d 696c 6172 6974 795f  from similarity_
-000039c0: 7473 2e73 696d 696c 6172 6974 795f 7473  ts.similarity_ts
-000039d0: 2069 6d70 6f72 7420 5369 6d69 6c61 7269   import Similari
-000039e0: 7479 5473 0a66 726f 6d20 7369 6d69 6c61  tyTs.from simila
-000039f0: 7269 7479 5f74 732e 6d65 7472 6963 732e  rity_ts.metrics.
-00003a00: 6d65 7472 6963 5f66 6163 746f 7279 2069  metric_factory i
-00003a10: 6d70 6f72 7420 4d65 7472 6963 4661 6374  mport MetricFact
-00003a20: 6f72 790a 6672 6f6d 2065 6420 696d 706f  ory.from ed impo
-00003a30: 7274 2045 7563 6c69 6465 616e 4469 7374  rt EuclideanDist
-00003a40: 616e 6365 0a66 726f 6d20 6363 5f70 6c6f  ance.from cc_plo
-00003a50: 7420 696d 706f 7274 2053 696d 696c 6172  t import Similar
-00003a60: 6974 7950 6c6f 7442 7943 6f72 7265 6c61  ityPlotByCorrela
-00003a70: 7469 6f6e 0a0a 6465 6620 6d61 696e 2829  tion..def main()
-00003a80: 3a0a 2020 2020 4d65 7472 6963 4661 6374  :.    MetricFact
-00003a90: 6f72 792e 6765 745f 696e 7374 616e 6365  ory.get_instance
-00003aa0: 2829 2e72 6567 6973 7465 725f 6d65 7472  ().register_metr
-00003ab0: 6963 2845 7563 6c69 6465 616e 4469 7374  ic(EuclideanDist
-00003ac0: 616e 6365 290a 2020 2020 506c 6f74 4661  ance).    PlotFa
-00003ad0: 6374 6f72 792e 6765 745f 696e 7374 616e  ctory.get_instan
-00003ae0: 6365 2829 2e72 6567 6973 7465 725f 706c  ce().register_pl
-00003af0: 6f74 2853 696d 696c 6172 6974 7950 6c6f  ot(SimilarityPlo
-00003b00: 7442 7943 6f72 7265 6c61 7469 6f6e 290a  tByCorrelation).
-00003b10: 2020 2020 7473 3120 3d20 6e70 2e72 616e      ts1 = np.ran
-00003b20: 646f 6d2e 7261 6e64 2832 3030 2c20 3229  dom.rand(200, 2)
-00003b30: 0a20 2020 2074 7332 7320 3d20 6e70 2e72  .    ts2s = np.r
-00003b40: 616e 646f 6d2e 7261 6e64 2835 2c20 3130  andom.rand(5, 10
-00003b50: 302c 2032 290a 2020 2020 7369 6d69 6c61  0, 2).    simila
-00003b60: 7269 7479 5f74 7320 3d20 5369 6d69 6c61  rity_ts = Simila
-00003b70: 7269 7479 5473 2874 7331 2c20 7473 3273  rityTs(ts1, ts2s
-00003b80: 290a 2020 2020 666f 7220 7473 325f 6e61  ).    for ts2_na
-00003b90: 6d65 2c20 6d65 7472 6963 5f6e 616d 652c  me, metric_name,
-00003ba0: 2063 6f6d 7075 7465 645f 6d65 7472 6963   computed_metric
-00003bb0: 2069 6e20 7369 6d69 6c61 7269 7479 5f74   in similarity_t
-00003bc0: 732e 6765 745f 6d65 7472 6963 5f63 6f6d  s.get_metric_com
-00003bd0: 7075 7465 7228 293a 0a20 2020 2020 2020  puter():.       
-00003be0: 2070 7269 6e74 2866 277b 7473 325f 6e61   print(f'{ts2_na
-00003bf0: 6d65 7d2e 207b 6d65 7472 6963 5f6e 616d  me}. {metric_nam
-00003c00: 657d 3a20 7b63 6f6d 7075 7465 645f 6d65  e}: {computed_me
-00003c10: 7472 6963 7d27 290a 2020 2020 666f 7220  tric}').    for 
-00003c20: 7473 325f 6e61 6d65 2c20 706c 6f74 5f6e  ts2_name, plot_n
-00003c30: 616d 652c 2067 656e 6572 6174 6564 5f70  ame, generated_p
-00003c40: 6c6f 7473 2069 6e20 7369 6d69 6c61 7269  lots in similari
-00003c50: 7479 5f74 732e 6765 745f 706c 6f74 5f63  ty_ts.get_plot_c
-00003c60: 6f6d 7075 7465 7228 293a 0a20 2020 2020  omputer():.     
-00003c70: 2020 205f 5f73 6176 655f 6669 6775 7265     __save_figure
-00003c80: 7328 7473 325f 6e61 6d65 2c20 706c 6f74  s(ts2_name, plot
-00003c90: 5f6e 616d 652c 2067 656e 6572 6174 6564  _name, generated
-00003ca0: 5f70 6c6f 7473 290a 0a0a 6465 6620 5f5f  _plots)...def __
-00003cb0: 7361 7665 5f66 6967 7572 6573 2866 696c  save_figures(fil
-00003cc0: 656e 616d 652c 2070 6c6f 745f 6e61 6d65  ename, plot_name
-00003cd0: 2c20 6765 6e65 7261 7465 645f 706c 6f74  , generated_plot
-00003ce0: 7329 3a0a 2020 2020 666f 7220 706c 6f74  s):.    for plot
-00003cf0: 2069 6e20 6765 6e65 7261 7465 645f 706c   in generated_pl
-00003d00: 6f74 733a 0a20 2020 2020 2020 2064 6972  ots:.        dir
-00003d10: 5f70 6174 6820 3d20 5f5f 6372 6561 7465  _path = __create
-00003d20: 5f64 6972 6563 746f 7279 2866 696c 656e  _directory(filen
-00003d30: 616d 652c 2066 2766 6967 7572 6573 272c  ame, f'figures',
-00003d40: 2070 6c6f 745f 6e61 6d65 290a 2020 2020   plot_name).    
-00003d50: 2020 2020 706c 6f74 5b30 5d2e 7361 7665      plot[0].save
-00003d60: 6669 6728 6627 7b64 6972 5f70 6174 687d  fig(f'{dir_path}
-00003d70: 7b70 6c6f 745b 305d 2e61 7865 735b 305d  {plot[0].axes[0]
-00003d80: 2e67 6574 5f74 6974 6c65 2829 7d2e 7064  .get_title()}.pd
-00003d90: 6627 2c20 666f 726d 6174 3d27 7064 6627  f', format='pdf'
-00003da0: 2c20 6262 6f78 5f69 6e63 6865 733d 2774  , bbox_inches='t
-00003db0: 6967 6874 2729 0a0a 0a64 6566 205f 5f63  ight')...def __c
-00003dc0: 7265 6174 655f 6469 7265 6374 6f72 7928  reate_directory(
-00003dd0: 6669 6c65 6e61 6d65 2c20 7061 7468 2c20  filename, path, 
-00003de0: 706c 6f74 5f6e 616d 6529 3a0a 2020 2020  plot_name):.    
-00003df0: 6966 2070 6c6f 745f 6e61 6d65 2069 6e20  if plot_name in 
-00003e00: 506c 6f74 4661 6374 6f72 792e 6765 745f  PlotFactory.get_
-00003e10: 696e 7374 616e 6365 2829 2e66 6967 7572  instance().figur
-00003e20: 6573 5f72 6571 7569 7265 735f 616c 6c5f  es_requires_all_
-00003e30: 7361 6d70 6c65 733a 0a20 2020 2020 2020  samples:.       
-00003e40: 2064 6972 5f70 6174 6820 3d20 6627 7b70   dir_path = f'{p
-00003e50: 6174 687d 2f7b 706c 6f74 5f6e 616d 657d  ath}/{plot_name}
-00003e60: 2f27 0a20 2020 2065 6c73 653a 0a20 2020  /'.    else:.   
-00003e70: 2020 2020 206f 7269 6769 6e61 6c5f 6669       original_fi
-00003e80: 6c65 6e61 6d65 203d 206f 732e 7061 7468  lename = os.path
-00003e90: 2e73 706c 6974 6578 7428 6669 6c65 6e61  .splitext(filena
-00003ea0: 6d65 295b 305d 0a20 2020 2020 2020 2064  me)[0].        d
-00003eb0: 6972 5f70 6174 6820 3d20 6627 7b70 6174  ir_path = f'{pat
-00003ec0: 687d 2f7b 6f72 6967 696e 616c 5f66 696c  h}/{original_fil
-00003ed0: 656e 616d 657d 2f7b 706c 6f74 5f6e 616d  ename}/{plot_nam
-00003ee0: 657d 2f27 0a20 2020 206f 732e 6d61 6b65  e}/'.    os.make
-00003ef0: 6469 7273 2864 6972 5f70 6174 682c 2065  dirs(dir_path, e
-00003f00: 7869 7374 5f6f 6b3d 5472 7565 290a 2020  xist_ok=True).  
-00003f10: 2020 7265 7475 726e 2064 6972 5f70 6174    return dir_pat
-00003f20: 680a 0a69 6620 5f5f 6e61 6d65 5f5f 203d  h..if __name__ =
-00003f30: 3d20 275f 5f6d 6169 6e5f 5f27 3a0a 2020  = '__main__':.  
-00003f40: 2020 6d61 696e 2829 0a60 6060 0a0a 2323    main().```..##
-00003f50: 204c 6963 656e 7365 0a0a 5369 6d69 6c61   License..Simila
-00003f60: 7269 7479 5453 2074 6f6f 6c6b 6974 2069  rityTS toolkit i
-00003f70: 7320 6672 6565 2061 6e64 206f 7065 6e2d  s free and open-
-00003f80: 736f 7572 6365 2073 6f66 7477 6172 6520  source software 
-00003f90: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
-00003fa0: 6865 205b 4d49 5420 6c69 6365 6e73 655d  he [MIT license]
-00003fb0: 284c 4943 454e 5345 292e 0a              (LICENSE)..
+00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002830: 2020 2020 2073 7472 6964 653d 3130 2c20       stride=10, 
+00002840: 7769 6e64 6f77 5f73 656c 6563 7469 6f6e  window_selection
+00002850: 5f6d 6574 7269 633d 276b 6c27 2c0a 2020  _metric='kl',.  
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2020 2020 2020 2020 2020 7473 325f              ts2_
+00002890: 6e61 6d65 733d 7473 325f 6e61 6d65 732c  names=ts2_names,
+000028a0: 2068 6561 6465 725f 6e61 6d65 733d 6865   header_names=he
+000028b0: 6164 6572 5f6e 616d 6573 290a 2020 2020  ader_names).    
+000028c0: 7265 7475 726e 2073 696d 696c 6172 6974  return similarit
+000028d0: 795f 7473 5f63 6f6e 6669 670a 6060 600a  y_ts_config.```.
+000028e0: 0a49 6620 6e6f 206d 6574 7269 6373 206e  .If no metrics n
+000028f0: 6f72 2066 6967 7572 6573 2061 7265 2070  or figures are p
+00002900: 726f 7669 6465 642c 2074 6865 2074 6f6f  rovided, the too
+00002910: 6c20 7769 6c6c 2063 6f6d 7075 7465 2061  l will compute a
+00002920: 6c6c 2074 6865 2061 7661 696c 6162 6c65  ll the available
+00002930: 206d 6574 7269 6373 2061 6e64 2066 6967   metrics and fig
+00002940: 7572 6573 2e0a 0a54 6865 2066 6f6c 6c6f  ures...The follo
+00002950: 7769 6e67 2061 7267 756d 656e 7473 2061  wing arguments a
+00002960: 7265 2061 6c73 6f20 6176 6169 6c61 626c  re also availabl
+00002970: 6520 666f 7220 6669 6e65 2d74 756e 696e  e for fine-tunin
+00002980: 673a 0a0a 2d20 6074 696d 6573 7461 6d70  g:..- `timestamp
+00002990: 5f66 7265 7175 656e 6379 5f73 6563 6f6e  _frequency_secon
+000029a0: 6473 603a 2074 6865 2066 7265 7175 656e  ds`: the frequen
+000029b0: 6379 2069 6e20 7365 636f 6e64 7320 696e  cy in seconds in
+000029c0: 2077 6869 6368 2073 616d 706c 6573 2077   which samples w
+000029d0: 6572 6520 7461 6b65 6e2e 2054 6869 7320  ere taken. This 
+000029e0: 6973 206e 6565 6465 6420 746f 2067 656e  is needed to gen
+000029f0: 6572 6174 6520 7468 6520 6465 6c74 6120  erate the delta 
+00002a00: 6669 6775 7265 7320 7769 7468 2063 6f72  figures with cor
+00002a10: 7265 6374 2074 696d 6520 6d61 676e 6974  rect time magnit
+00002a20: 7564 6573 2e20 4279 2064 6566 6175 6c74  udes. By default
+00002a30: 2069 730a 2020 6031 6020 7365 636f 6e64   is.  `1` second
+00002a40: 2e0a 2d20 6073 7472 6964 6560 3a20 7768  ..- `stride`: wh
+00002a50: 656e 2060 7473 3160 2074 696d 652d 7365  en `ts1` time-se
+00002a60: 7269 6573 2069 7320 6c6f 6e67 6572 2074  ries is longer t
+00002a70: 6861 6e20 6074 7332 7360 2074 696d 652d  han `ts2s` time-
+00002a80: 7365 7269 6573 2074 6865 2077 696e 646f  series the windo
+00002a90: 7773 2061 7265 2063 6f6d 7075 7465 6420  ws are computed 
+00002aa0: 6279 2075 7369 6e67 2061 0a20 2073 7472  by using a.  str
+00002ab0: 6964 6520 6f66 2060 3160 2062 7920 6465  ide of `1` by de
+00002ac0: 6661 756c 742e 2053 6f6d 6574 696d 6573  fault. Sometimes
+00002ad0: 2075 7369 6e67 2061 206c 6172 6765 7220   using a larger 
+00002ae0: 7661 6c75 6520 666f 7220 7468 6520 7374  value for the st
+00002af0: 7269 6465 2070 6172 616d 6574 6572 2069  ride parameter i
+00002b00: 6d70 726f 7665 7320 7468 6520 7065 7266  mproves the perf
+00002b10: 6f72 6d61 6e63 6520 6279 2073 6b69 7070  ormance by skipp
+00002b20: 696e 670a 2020 7468 6520 636f 6d70 7574  ing.  the comput
+00002b30: 6174 696f 6e20 6f66 2073 696d 696c 6172  ation of similar
+00002b40: 6974 7920 6265 7477 6565 6e20 736f 206d  ity between so m
+00002b50: 616e 7920 7769 6e64 6f77 732e 0a2d 2060  any windows..- `
+00002b60: 7769 6e64 6f77 5f73 656c 6563 7469 6f6e  window_selection
+00002b70: 5f6d 6574 7269 6360 3a20 7468 6520 6d65  _metric`: the me
+00002b80: 7472 6963 2075 7365 6420 666f 7220 7468  tric used for th
+00002b90: 6520 7365 6c65 6374 696f 6e20 6f66 2074  e selection of t
+00002ba0: 6865 206d 6f73 7420 7369 6d69 6c61 7220  he most similar 
+00002bb0: 6074 7331 6020 7469 6d65 2d73 6572 6965  `ts1` time-serie
+00002bc0: 7320 7769 6e64 6f77 2070 6572 2065 6163  s window per eac
+00002bd0: 6820 6074 7332 7360 2074 696d 652d 7365  h `ts2s` time-se
+00002be0: 7269 6573 2066 696c 6520 6973 2073 656c  ries file is sel
+00002bf0: 6563 7461 626c 652e 6064 7477 6020 6973  ectable.`dtw` is
+00002c00: 2074 6865 2064 6566 6175 6c74 2073 656c   the default sel
+00002c10: 6563 7465 6420 6d65 7472 6963 2c20 686f  ected metric, ho
+00002c20: 7765 7665 722c 2061 6e79 206f 6620 7468  wever, any of th
+00002c30: 6520 5b6d 6574 7269 6373 5d28 2361 7661  e [metrics](#ava
+00002c40: 696c 6162 6c65 2d6d 6574 7269 6373 2920  ilable-metrics) 
+00002c50: 6172 6520 616c 736f 2061 7661 696c 6162  are also availab
+00002c60: 6c65 2066 6f72 2074 6869 7320 7075 7270  le for this purp
+00002c70: 6f73 652e 2053 6565 2074 6865 205b 746f  ose. See the [to
+00002c80: 6f6c 6b69 7420 636f 6e66 6967 7572 6174  olkit configurat
+00002c90: 696f 6e20 7365 6374 696f 6e5d 2823 636f  ion section](#co
+00002ca0: 6e66 6967 7572 696e 672d 7468 652d 746f  nfiguring-the-to
+00002cb0: 6f6c 6b69 7429 2e0a 2d20 6074 7332 5f6e  olkit)..- `ts2_n
+00002cc0: 616d 6573 603a 206e 616d 6520 6f66 2065  ames`: name of e
+00002cd0: 6163 6820 7469 6d65 2073 6572 6965 7320  ach time series 
+00002ce0: 6f66 2074 6865 2060 7473 3273 6020 7365  of the `ts2s` se
+00002cf0: 7420 6f66 2074 696d 6520 7365 7269 6573  t of time series
+00002d00: 2e0a 2d20 6068 6561 6465 725f 6e61 6d65  ..- `header_name
+00002d10: 7360 3a20 6e61 6d65 206f 6620 7468 6520  s`: name of the 
+00002d20: 6665 6174 7572 6573 0a0a 0a23 2320 4578  features...## Ex
+00002d30: 7465 6e64 696e 6720 7468 6520 746f 6f6c  tending the tool
+00002d40: 6b69 740a 0a41 6464 6974 696f 6e61 6c6c  kit..Additionall
+00002d50: 792c 2075 7365 7273 206d 6179 2069 6d70  y, users may imp
+00002d60: 6c65 6d65 6e74 2074 6865 6972 206f 776e  lement their own
+00002d70: 206d 6574 7269 6320 6f72 2066 6967 7572   metric or figur
+00002d80: 6520 636c 6173 7365 7320 616e 6420 696e  e classes and in
+00002d90: 636c 7564 6520 7468 656d 2062 7920 7573  clude them by us
+00002da0: 696e 6720 7468 6520 604d 6574 7269 6346  ing the `MetricF
+00002db0: 6163 746f 7279 6020 6f72 2060 506c 6f74  actory` or `Plot
+00002dc0: 4661 6374 6f72 7960 2072 6567 6973 7465  Factory` registe
+00002dd0: 7220 6d65 7468 6f64 732e 2054 6f20 656e  r methods. To en
+00002de0: 7375 7265 2063 6f6d 7061 7469 6269 6c69  sure compatibili
+00002df0: 7479 2077 6974 6820 6f75 7220 746f 6f6c  ty with our tool
+00002e00: 6b69 742c 2074 6865 7920 6861 7665 2074  kit, they have t
+00002e10: 6f20 696e 6865 7269 7420 6672 6f6d 2074  o inherit from t
+00002e20: 6865 2062 6173 6520 636c 6173 7365 7320  he base classes 
+00002e30: 604d 6574 7269 6360 2061 6e64 2060 506c  `Metric` and `Pl
+00002e40: 6f74 602e 0a0a 5468 6520 666f 6c6c 6f77  ot`...The follow
+00002e50: 696e 6720 636f 6465 2073 6e69 7070 6574  ing code snippet
+00002e60: 2069 7320 616e 2065 7861 6d70 6c65 206f   is an example o
+00002e70: 6620 686f 7720 746f 2069 6e74 726f 6475  f how to introdu
+00002e80: 6365 2074 6865 2045 7563 6c69 6465 616e  ce the Euclidean
+00002e90: 2064 6973 7461 6e63 6520 6d65 7472 6963   distance metric
+00002ea0: 3a0a 0a60 6060 5079 7468 6f6e 0a23 6575  :..```Python.#eu
+00002eb0: 2e70 790a 696d 706f 7274 206e 756d 7079  .py.import numpy
+00002ec0: 2061 7320 6e70 0a66 726f 6d20 7369 6d69   as np.from simi
+00002ed0: 6c61 7269 7479 5f74 732e 6d65 7472 6963  larity_ts.metric
+00002ee0: 732e 6d65 7472 6963 2069 6d70 6f72 7420  s.metric import 
+00002ef0: 4d65 7472 6963 0a0a 0a63 6c61 7373 2045  Metric...class E
+00002f00: 7563 6c69 6465 616e 4469 7374 616e 6365  uclideanDistance
+00002f10: 284d 6574 7269 6329 3a0a 0a20 2020 2064  (Metric):..    d
+00002f20: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00002f30: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
+00002f40: 2829 2e5f 5f69 6e69 745f 5f28 290a 2020  ().__init__().  
+00002f50: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
+00002f60: 3d20 2765 6427 0a0a 2020 2020 6465 6620  = 'ed'..    def 
+00002f70: 636f 6d70 7574 6528 7365 6c66 2c20 7473  compute(self, ts
+00002f80: 312c 2074 7332 2c20 7369 6d69 6c61 7269  1, ts2, similari
+00002f90: 7479 5f74 7329 3a0a 2020 2020 2020 2020  ty_ts):.        
+00002fa0: 6d65 7472 6963 5f72 6573 756c 7420 3d20  metric_result = 
+00002fb0: 7b27 4d75 6c74 6976 6172 6961 7465 273a  {'Multivariate':
+00002fc0: 2073 656c 662e 5f5f 6564 2874 7331 2c20   self.__ed(ts1, 
+00002fd0: 7473 3229 7d0a 2020 2020 2020 2020 7265  ts2)}.        re
+00002fe0: 7475 726e 206d 6574 7269 635f 7265 7375  turn metric_resu
+00002ff0: 6c74 0a0a 2020 2020 6465 6620 636f 6d70  lt..    def comp
+00003000: 7574 655f 6469 7374 616e 6365 2873 656c  ute_distance(sel
+00003010: 662c 2074 7331 2c20 7473 3229 3a0a 2020  f, ts1, ts2):.  
+00003020: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00003030: 662e 5f5f 6564 2874 7331 2c20 7473 3229  f.__ed(ts1, ts2)
+00003040: 0a0a 2020 2020 6465 6620 5f5f 6564 2873  ..    def __ed(s
+00003050: 656c 662c 2074 7331 2c20 7473 3229 3a0a  elf, ts1, ts2):.
+00003060: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00003070: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 7473  p.linalg.norm(ts
+00003080: 3120 2d20 7473 3229 0a0a 6060 600a 0a41  1 - ts2)..```..A
+00003090: 6674 6572 7761 7264 2c20 7468 6973 206d  fterward, this m
+000030a0: 6574 7269 6320 6361 6e20 6265 2072 6567  etric can be reg
+000030b0: 6973 7465 7265 6420 6279 2075 7369 6e67  istered by using
+000030c0: 2074 6865 2060 7265 6769 7374 6572 5f6d   the `register_m
+000030d0: 6574 7269 6328 6d65 7472 6963 5f63 6c61  etric(metric_cla
+000030e0: 7373 2960 206d 6574 686f 6420 6672 6f6d  ss)` method from
+000030f0: 2060 4d65 7472 6963 4661 6374 6f72 7960   `MetricFactory`
+00003100: 2061 7320 7368 6f77 6e20 696e 2074 6865   as shown in the
+00003110: 2066 6f6c 6c6f 7769 6e67 2063 6f64 6520   following code 
+00003120: 736e 6970 7065 743a 0a60 6060 5079 7468  snippet:.```Pyth
+00003130: 6f6e 0a69 6d70 6f72 7420 6e75 6d70 7920  on.import numpy 
+00003140: 6173 206e 700a 6672 6f6d 2073 696d 696c  as np.from simil
+00003150: 6172 6974 795f 7473 2e73 696d 696c 6172  arity_ts.similar
+00003160: 6974 795f 7473 2069 6d70 6f72 7420 5369  ity_ts import Si
+00003170: 6d69 6c61 7269 7479 5473 0a66 726f 6d20  milarityTs.from 
+00003180: 7369 6d69 6c61 7269 7479 5f74 732e 6d65  similarity_ts.me
+00003190: 7472 6963 732e 6d65 7472 6963 5f66 6163  trics.metric_fac
+000031a0: 746f 7279 2069 6d70 6f72 7420 4d65 7472  tory import Metr
+000031b0: 6963 4661 6374 6f72 790a 6672 6f6d 2065  icFactory.from e
+000031c0: 6420 696d 706f 7274 2045 7563 6c69 6465  d import Euclide
+000031d0: 616e 4469 7374 616e 6365 0a0a 4d65 7472  anDistance..Metr
+000031e0: 6963 4661 6374 6f72 792e 6765 745f 696e  icFactory.get_in
+000031f0: 7374 616e 6365 2829 2e72 6567 6973 7465  stance().registe
+00003200: 725f 6d65 7472 6963 2845 7563 6c69 6465  r_metric(Euclide
+00003210: 616e 4469 7374 616e 6365 290a 7473 3120  anDistance).ts1 
+00003220: 3d20 6e70 2e72 616e 646f 6d2e 7261 6e64  = np.random.rand
+00003230: 2832 3030 2c20 3229 0a74 7332 7320 3d20  (200, 2).ts2s = 
+00003240: 6e70 2e72 616e 646f 6d2e 7261 6e64 2835  np.random.rand(5
+00003250: 2c20 3130 302c 2032 290a 7369 6d69 6c61  , 100, 2).simila
+00003260: 7269 7479 5f74 7320 3d20 5369 6d69 6c61  rity_ts = Simila
+00003270: 7269 7479 5473 2874 7331 2c20 7473 3273  rityTs(ts1, ts2s
+00003280: 290a 666f 7220 7473 325f 6e61 6d65 2c20  ).for ts2_name, 
+00003290: 6d65 7472 6963 5f6e 616d 652c 2063 6f6d  metric_name, com
+000032a0: 7075 7465 645f 6d65 7472 6963 2069 6e20  puted_metric in 
+000032b0: 7369 6d69 6c61 7269 7479 5f74 732e 6765  similarity_ts.ge
+000032c0: 745f 6d65 7472 6963 5f63 6f6d 7075 7465  t_metric_compute
+000032d0: 7228 293a 0a20 2020 2070 7269 6e74 2866  r():.    print(f
+000032e0: 277b 7473 325f 6e61 6d65 7d2e 207b 6d65  '{ts2_name}. {me
+000032f0: 7472 6963 5f6e 616d 657d 3a20 7b63 6f6d  tric_name}: {com
+00003300: 7075 7465 645f 6d65 7472 6963 7d27 290a  puted_metric}').
+00003310: 6060 600a 0a53 696d 696c 6172 6c79 2c20  ```..Similarly, 
+00003320: 6e65 7720 706c 6f74 7320 6361 6e20 6265  new plots can be
+00003330: 2069 6e74 726f 6475 6365 642e 2046 6f72   introduced. For
+00003340: 2069 6e73 7461 6e63 6520 6120 6053 696d   instance a `Sim
+00003350: 696c 6172 6974 7950 6c6f 7442 7943 6f72  ilarityPlotByCor
+00003360: 7265 6c61 7469 6f6e 6020 636f 756c 6420  relation` could 
+00003370: 6265 2064 6566 696e 6564 2061 733a 0a60  be defined as:.`
+00003380: 6060 5079 7468 6f6e 0a23 6363 5f70 6c6f  ``Python.#cc_plo
+00003390: 742e 7079 0a69 6d70 6f72 7420 6e75 6d70  t.py.import nump
+000033a0: 7920 6173 206e 700a 696d 706f 7274 206d  y as np.import m
+000033b0: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
+000033c0: 2061 7320 706c 740a 6672 6f6d 2073 696d   as plt.from sim
+000033d0: 696c 6172 6974 795f 7473 2e70 6c6f 7473  ilarity_ts.plots
+000033e0: 2e70 6c6f 7420 696d 706f 7274 2050 6c6f  .plot import Plo
+000033f0: 740a 0a0a 636c 6173 7320 5369 6d69 6c61  t...class Simila
+00003400: 7269 7479 506c 6f74 4279 436f 7272 656c  rityPlotByCorrel
+00003410: 6174 696f 6e28 506c 6f74 293a 0a0a 2020  ation(Plot):..  
+00003420: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00003430: 656c 662c 2066 6967 5f73 697a 653d 2838  elf, fig_size=(8
+00003440: 2c20 3629 293a 0a20 2020 2020 2020 2073  , 6)):.        s
+00003450: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+00003460: 6669 675f 7369 7a65 290a 2020 2020 2020  fig_size).      
+00003470: 2020 7365 6c66 2e6e 616d 6520 3d20 2763    self.name = 'c
+00003480: 632d 706c 6f74 270a 0a20 2020 2064 6566  c-plot'..    def
+00003490: 2063 6f6d 7075 7465 2873 656c 662c 2073   compute(self, s
+000034a0: 696d 696c 6172 6974 795f 7473 2c20 7473  imilarity_ts, ts
+000034b0: 325f 6669 6c65 6e61 6d65 293a 0a20 2020  2_filename):.   
+000034c0: 2020 2020 2073 7570 6572 2829 2e63 6f6d       super().com
+000034d0: 7075 7465 2873 696d 696c 6172 6974 795f  pute(similarity_
+000034e0: 7473 2c20 7473 325f 6669 6c65 6e61 6d65  ts, ts2_filename
+000034f0: 290a 2020 2020 2020 2020 6e5f 6665 6174  ).        n_feat
+00003500: 7572 6573 203d 2073 656c 662e 7473 312e  ures = self.ts1.
+00003510: 7368 6170 655b 315d 0a20 2020 2020 2020  shape[1].       
+00003520: 2073 696d 696c 6172 6974 7920 3d20 6e70   similarity = np
+00003530: 2e63 6f72 7263 6f65 6628 7365 6c66 2e74  .corrcoef(self.t
+00003540: 7331 2e54 2c20 7365 6c66 2e74 7332 2e54  s1.T, self.ts2.T
+00003550: 290a 2020 2020 2020 2020 6669 672c 2061  ).        fig, a
+00003560: 7820 3d20 706c 742e 7375 6270 6c6f 7473  x = plt.subplots
+00003570: 2829 0a20 2020 2020 2020 2069 6d20 3d20  ().        im = 
+00003580: 6178 2e69 6d73 686f 7728 7369 6d69 6c61  ax.imshow(simila
+00003590: 7269 7479 2c20 636d 6170 3d27 5264 596c  rity, cmap='RdYl
+000035a0: 4275 272c 2076 6d69 6e3d 2d31 2c20 766d  Bu', vmin=-1, vm
+000035b0: 6178 3d31 290a 2020 2020 2020 2020 6178  ax=1).        ax
+000035c0: 2e73 6574 5f78 7469 636b 7328 6e70 2e61  .set_xticks(np.a
+000035d0: 7261 6e67 6528 6e5f 6665 6174 7572 6573  range(n_features
+000035e0: 2a32 2929 0a20 2020 2020 2020 2061 782e  *2)).        ax.
+000035f0: 7365 745f 7974 6963 6b73 286e 702e 6172  set_yticks(np.ar
+00003600: 616e 6765 286e 5f66 6561 7475 7265 732a  ange(n_features*
+00003610: 3229 290a 2020 2020 2020 2020 7874 6963  2)).        xtic
+00003620: 6b6c 6162 656c 7320 3d20 5b66 2774 7331  klabels = [f'ts1
+00003630: 5f7b 6e66 6561 7475 7265 735f 696e 6465  _{nfeatures_inde
+00003640: 787d 2766 6f72 206e 6665 6174 7572 6573  x}'for nfeatures
+00003650: 5f69 6e64 6578 2069 6e20 7261 6e67 6528  _index in range(
+00003660: 312c 206e 5f66 6561 7475 7265 732b 3129  1, n_features+1)
+00003670: 5d0a 2020 2020 2020 2020 7874 6963 6b6c  ].        xtickl
+00003680: 6162 656c 7320 3d20 7874 6963 6b6c 6162  abels = xticklab
+00003690: 656c 7320 2b20 5b66 2774 7332 5f7b 6e66  els + [f'ts2_{nf
+000036a0: 6561 7475 7265 735f 696e 6465 787d 2766  eatures_index}'f
+000036b0: 6f72 206e 6665 6174 7572 6573 5f69 6e64  or nfeatures_ind
+000036c0: 6578 2069 6e20 7261 6e67 6528 312c 206e  ex in range(1, n
+000036d0: 5f66 6561 7475 7265 732b 3129 5d0a 2020  _features+1)].  
+000036e0: 2020 2020 2020 6178 2e73 6574 5f78 7469        ax.set_xti
+000036f0: 636b 6c61 6265 6c73 2878 7469 636b 6c61  cklabels(xtickla
+00003700: 6265 6c73 290a 2020 2020 2020 2020 6178  bels).        ax
+00003710: 2e73 6574 5f79 7469 636b 6c61 6265 6c73  .set_yticklabels
+00003720: 2878 7469 636b 6c61 6265 6c73 290a 2020  (xticklabels).  
+00003730: 2020 2020 2020 6178 2e73 6574 5f78 6c61        ax.set_xla
+00003740: 6265 6c28 2746 6561 7475 7265 2729 0a20  bel('Feature'). 
+00003750: 2020 2020 2020 2061 782e 7365 745f 796c         ax.set_yl
+00003760: 6162 656c 2827 4665 6174 7572 6527 290a  abel('Feature').
+00003770: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00003780: 2072 616e 6765 286e 5f66 6561 7475 7265   range(n_feature
+00003790: 732a 3229 3a0a 2020 2020 2020 2020 2020  s*2):.          
+000037a0: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
+000037b0: 286e 5f66 6561 7475 7265 732a 3229 3a0a  (n_features*2):.
+000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037d0: 6178 2e74 6578 7428 6a2c 2069 2c20 6627  ax.text(j, i, f'
+000037e0: 7b73 696d 696c 6172 6974 795b 692c 206a  {similarity[i, j
+000037f0: 5d3a 2e32 667d 272c 2068 613d 2763 656e  ]:.2f}', ha='cen
+00003800: 7465 7227 2c20 7661 3d27 6365 6e74 6572  ter', va='center
+00003810: 272c 2063 6f6c 6f72 3d27 626c 6163 6b27  ', color='black'
+00003820: 290a 0a20 2020 2020 2020 2063 6261 7220  )..        cbar 
+00003830: 3d20 6178 2e66 6967 7572 652e 636f 6c6f  = ax.figure.colo
+00003840: 7262 6172 2869 6d2c 2061 783d 6178 290a  rbar(im, ax=ax).
+00003850: 2020 2020 2020 2020 6362 6172 2e61 782e          cbar.ax.
+00003860: 7365 745f 796c 6162 656c 2827 5369 6d69  set_ylabel('Simi
+00003870: 6c61 7269 7479 272c 2072 6f74 6174 696f  larity', rotatio
+00003880: 6e3d 2d39 302c 2076 613d 2762 6f74 746f  n=-90, va='botto
+00003890: 6d27 290a 2020 2020 2020 2020 706c 742e  m').        plt.
+000038a0: 7469 746c 6528 2773 696d 696c 6172 6974  title('similarit
+000038b0: 792d 636f 7272 656c 6174 696f 6e27 290a  y-correlation').
+000038c0: 2020 2020 2020 2020 706c 742e 7469 6768          plt.tigh
+000038d0: 745f 6c61 796f 7574 2829 0a20 2020 2020  t_layout().     
+000038e0: 2020 2072 6574 7572 6e20 5b28 6669 672c     return [(fig,
+000038f0: 2061 7829 5d0a 6060 600a 0a41 6674 6572   ax)].```..After
+00003900: 7761 7264 2c20 7468 6973 2070 6c6f 7420  ward, this plot 
+00003910: 6361 6e20 6265 2072 6567 6973 7465 7265  can be registere
+00003920: 6420 6279 2075 7369 6e67 2074 6865 2060  d by using the `
+00003930: 7265 6769 7374 6572 5f70 6c6f 7428 706c  register_plot(pl
+00003940: 6f74 5f63 6c61 7373 2960 206d 6574 686f  ot_class)` metho
+00003950: 6420 6672 6f6d 2060 506c 6f74 4661 6374  d from `PlotFact
+00003960: 6f72 7960 2061 7320 7368 6f77 6e20 696e  ory` as shown in
+00003970: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00003980: 6f64 6520 736e 6970 7065 7420 7468 6174  ode snippet that
+00003990: 2072 6567 6973 7465 7220 7468 6520 6e65   register the ne
+000039a0: 7720 6d65 7472 6963 2061 6e64 2074 6865  w metric and the
+000039b0: 206e 6577 2070 6c6f 743a 0a60 6060 5079   new plot:.```Py
+000039c0: 7468 6f6e 0a69 6d70 6f72 7420 6f73 0a69  thon.import os.i
+000039d0: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
+000039e0: 700a 6672 6f6d 2073 696d 696c 6172 6974  p.from similarit
+000039f0: 795f 7473 2e70 6c6f 7473 2e70 6c6f 745f  y_ts.plots.plot_
+00003a00: 6661 6374 6f72 7920 696d 706f 7274 2050  factory import P
+00003a10: 6c6f 7446 6163 746f 7279 0a66 726f 6d20  lotFactory.from 
+00003a20: 7369 6d69 6c61 7269 7479 5f74 732e 7369  similarity_ts.si
+00003a30: 6d69 6c61 7269 7479 5f74 7320 696d 706f  milarity_ts impo
+00003a40: 7274 2053 696d 696c 6172 6974 7954 730a  rt SimilarityTs.
+00003a50: 6672 6f6d 2073 696d 696c 6172 6974 795f  from similarity_
+00003a60: 7473 2e6d 6574 7269 6373 2e6d 6574 7269  ts.metrics.metri
+00003a70: 635f 6661 6374 6f72 7920 696d 706f 7274  c_factory import
+00003a80: 204d 6574 7269 6346 6163 746f 7279 0a66   MetricFactory.f
+00003a90: 726f 6d20 6564 2069 6d70 6f72 7420 4575  rom ed import Eu
+00003aa0: 636c 6964 6561 6e44 6973 7461 6e63 650a  clideanDistance.
+00003ab0: 6672 6f6d 2063 635f 706c 6f74 2069 6d70  from cc_plot imp
+00003ac0: 6f72 7420 5369 6d69 6c61 7269 7479 506c  ort SimilarityPl
+00003ad0: 6f74 4279 436f 7272 656c 6174 696f 6e0a  otByCorrelation.
+00003ae0: 0a64 6566 206d 6169 6e28 293a 0a20 2020  .def main():.   
+00003af0: 204d 6574 7269 6346 6163 746f 7279 2e67   MetricFactory.g
+00003b00: 6574 5f69 6e73 7461 6e63 6528 292e 7265  et_instance().re
+00003b10: 6769 7374 6572 5f6d 6574 7269 6328 4575  gister_metric(Eu
+00003b20: 636c 6964 6561 6e44 6973 7461 6e63 6529  clideanDistance)
+00003b30: 0a20 2020 2050 6c6f 7446 6163 746f 7279  .    PlotFactory
+00003b40: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
+00003b50: 7265 6769 7374 6572 5f70 6c6f 7428 5369  register_plot(Si
+00003b60: 6d69 6c61 7269 7479 506c 6f74 4279 436f  milarityPlotByCo
+00003b70: 7272 656c 6174 696f 6e29 0a20 2020 2074  rrelation).    t
+00003b80: 7331 203d 206e 702e 7261 6e64 6f6d 2e72  s1 = np.random.r
+00003b90: 616e 6428 3230 302c 2032 290a 2020 2020  and(200, 2).    
+00003ba0: 7473 3273 203d 206e 702e 7261 6e64 6f6d  ts2s = np.random
+00003bb0: 2e72 616e 6428 352c 2031 3030 2c20 3229  .rand(5, 100, 2)
+00003bc0: 0a20 2020 2073 696d 696c 6172 6974 795f  .    similarity_
+00003bd0: 7473 203d 2053 696d 696c 6172 6974 7954  ts = SimilarityT
+00003be0: 7328 7473 312c 2074 7332 7329 0a20 2020  s(ts1, ts2s).   
+00003bf0: 2066 6f72 2074 7332 5f6e 616d 652c 206d   for ts2_name, m
+00003c00: 6574 7269 635f 6e61 6d65 2c20 636f 6d70  etric_name, comp
+00003c10: 7574 6564 5f6d 6574 7269 6320 696e 2073  uted_metric in s
+00003c20: 696d 696c 6172 6974 795f 7473 2e67 6574  imilarity_ts.get
+00003c30: 5f6d 6574 7269 635f 636f 6d70 7574 6572  _metric_computer
+00003c40: 2829 3a0a 2020 2020 2020 2020 7072 696e  ():.        prin
+00003c50: 7428 6627 7b74 7332 5f6e 616d 657d 2e20  t(f'{ts2_name}. 
+00003c60: 7b6d 6574 7269 635f 6e61 6d65 7d3a 207b  {metric_name}: {
+00003c70: 636f 6d70 7574 6564 5f6d 6574 7269 637d  computed_metric}
+00003c80: 2729 0a20 2020 2066 6f72 2074 7332 5f6e  ').    for ts2_n
+00003c90: 616d 652c 2070 6c6f 745f 6e61 6d65 2c20  ame, plot_name, 
+00003ca0: 6765 6e65 7261 7465 645f 706c 6f74 7320  generated_plots 
+00003cb0: 696e 2073 696d 696c 6172 6974 795f 7473  in similarity_ts
+00003cc0: 2e67 6574 5f70 6c6f 745f 636f 6d70 7574  .get_plot_comput
+00003cd0: 6572 2829 3a0a 2020 2020 2020 2020 5f5f  er():.        __
+00003ce0: 7361 7665 5f66 6967 7572 6573 2874 7332  save_figures(ts2
+00003cf0: 5f6e 616d 652c 2070 6c6f 745f 6e61 6d65  _name, plot_name
+00003d00: 2c20 6765 6e65 7261 7465 645f 706c 6f74  , generated_plot
+00003d10: 7329 0a0a 0a64 6566 205f 5f73 6176 655f  s)...def __save_
+00003d20: 6669 6775 7265 7328 6669 6c65 6e61 6d65  figures(filename
+00003d30: 2c20 706c 6f74 5f6e 616d 652c 2067 656e  , plot_name, gen
+00003d40: 6572 6174 6564 5f70 6c6f 7473 293a 0a20  erated_plots):. 
+00003d50: 2020 2066 6f72 2070 6c6f 7420 696e 2067     for plot in g
+00003d60: 656e 6572 6174 6564 5f70 6c6f 7473 3a0a  enerated_plots:.
+00003d70: 2020 2020 2020 2020 6469 725f 7061 7468          dir_path
+00003d80: 203d 205f 5f63 7265 6174 655f 6469 7265   = __create_dire
+00003d90: 6374 6f72 7928 6669 6c65 6e61 6d65 2c20  ctory(filename, 
+00003da0: 6627 6669 6775 7265 7327 2c20 706c 6f74  f'figures', plot
+00003db0: 5f6e 616d 6529 0a20 2020 2020 2020 2070  _name).        p
+00003dc0: 6c6f 745b 305d 2e73 6176 6566 6967 2866  lot[0].savefig(f
+00003dd0: 277b 6469 725f 7061 7468 7d7b 706c 6f74  '{dir_path}{plot
+00003de0: 5b30 5d2e 6178 6573 5b30 5d2e 6765 745f  [0].axes[0].get_
+00003df0: 7469 746c 6528 297d 2e70 6466 272c 2066  title()}.pdf', f
+00003e00: 6f72 6d61 743d 2770 6466 272c 2062 626f  ormat='pdf', bbo
+00003e10: 785f 696e 6368 6573 3d27 7469 6768 7427  x_inches='tight'
+00003e20: 290a 0a0a 6465 6620 5f5f 6372 6561 7465  )...def __create
+00003e30: 5f64 6972 6563 746f 7279 2866 696c 656e  _directory(filen
+00003e40: 616d 652c 2070 6174 682c 2070 6c6f 745f  ame, path, plot_
+00003e50: 6e61 6d65 293a 0a20 2020 2069 6620 706c  name):.    if pl
+00003e60: 6f74 5f6e 616d 6520 696e 2050 6c6f 7446  ot_name in PlotF
+00003e70: 6163 746f 7279 2e67 6574 5f69 6e73 7461  actory.get_insta
+00003e80: 6e63 6528 292e 6669 6775 7265 735f 7265  nce().figures_re
+00003e90: 7175 6972 6573 5f61 6c6c 5f73 616d 706c  quires_all_sampl
+00003ea0: 6573 3a0a 2020 2020 2020 2020 6469 725f  es:.        dir_
+00003eb0: 7061 7468 203d 2066 277b 7061 7468 7d2f  path = f'{path}/
+00003ec0: 7b70 6c6f 745f 6e61 6d65 7d2f 270a 2020  {plot_name}/'.  
+00003ed0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003ee0: 6f72 6967 696e 616c 5f66 696c 656e 616d  original_filenam
+00003ef0: 6520 3d20 6f73 2e70 6174 682e 7370 6c69  e = os.path.spli
+00003f00: 7465 7874 2866 696c 656e 616d 6529 5b30  text(filename)[0
+00003f10: 5d0a 2020 2020 2020 2020 6469 725f 7061  ].        dir_pa
+00003f20: 7468 203d 2066 277b 7061 7468 7d2f 7b6f  th = f'{path}/{o
+00003f30: 7269 6769 6e61 6c5f 6669 6c65 6e61 6d65  riginal_filename
+00003f40: 7d2f 7b70 6c6f 745f 6e61 6d65 7d2f 270a  }/{plot_name}/'.
+00003f50: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
+00003f60: 6469 725f 7061 7468 2c20 6578 6973 745f  dir_path, exist_
+00003f70: 6f6b 3d54 7275 6529 0a20 2020 2072 6574  ok=True).    ret
+00003f80: 7572 6e20 6469 725f 7061 7468 0a0a 6966  urn dir_path..if
+00003f90: 205f 5f6e 616d 655f 5f20 3d3d 2027 5f5f   __name__ == '__
+00003fa0: 6d61 696e 5f5f 273a 0a20 2020 206d 6169  main__':.    mai
+00003fb0: 6e28 290a 6060 600a 0a23 2320 4c69 6365  n().```..## Lice
+00003fc0: 6e73 650a 0a53 696d 696c 6172 6974 7954  nse..SimilarityT
+00003fd0: 5320 746f 6f6c 6b69 7420 6973 2066 7265  S toolkit is fre
+00003fe0: 6520 616e 6420 6f70 656e 2d73 6f75 7263  e and open-sourc
+00003ff0: 6520 736f 6674 7761 7265 206c 6963 656e  e software licen
+00004000: 7365 6420 756e 6465 7220 7468 6520 5b4d  sed under the [M
+00004010: 4954 206c 6963 656e 7365 5d28 4c49 4345  IT license](LICE
+00004020: 4e53 4529 2e0a                           NSE)..
```

### Comparing `similarity_ts-1.0.1/pyproject.toml` & `similarity_ts-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "similarity_ts"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name = "Alejandro Fernández-Montes", email = "afdez@us.es" },
     { name = "Damián Fernández-Cerero", email = "damiancerero@us.es" },
     { name = "Felipe Escalera González", email = "fescalera@us.es" },
 ]
 dependencies = ["dtaidistance", "matplotlib", "pandas", "scikit-learn", "tqdm", "natsort", "chardet"]
 description = "SimilarityTS is an open-source project designed to facilitate the evaluation and comparison of multivariate time series data"
```

### Comparing `similarity_ts-1.0.1/src/similarity_ts/helpers/csv_reader_helper.py` & `similarity_ts-1.0.2/src/similarity_ts/helpers/csv_reader_helper.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/helpers/dynamic_import_helper.py` & `similarity_ts-1.0.2/src/similarity_ts/helpers/dynamic_import_helper.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/helpers/window_sampler.py` & `similarity_ts-1.0.2/src/similarity_ts/helpers/window_sampler.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/cc.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/cc.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/cp.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/cp.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/dtw.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/dtw.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/hi.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/hi.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/js.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/js.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/kl.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/kl.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/ks.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/ks.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/metric_computer.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/metric_computer.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/metric_factory.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/metric_factory.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/metrics/mmd.py` & `similarity_ts-1.0.2/src/similarity_ts/metrics/mmd.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/delta.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/delta.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/dimensionalty_reduction.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/dimensionalty_reduction.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/dtw.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/dtw.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/pca.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/pca.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/plot.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/plot.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/plot_computer.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/plot_computer.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/plot_config.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/plot_config.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/plot_factory.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/plot_factory.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/tsne.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/tsne.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/plots/two_dimensions.py` & `similarity_ts-1.0.2/src/similarity_ts/plots/two_dimensions.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/similarity_analysis_computer.py` & `similarity_ts-1.0.2/src/similarity_ts/similarity_analysis_computer.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/similarity_ts.py` & `similarity_ts-1.0.2/src/similarity_ts/similarity_ts.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts/similarity_ts_config.py` & `similarity_ts-1.0.2/src/similarity_ts/similarity_ts_config.py`

 * *Files identical despite different names*

### Comparing `similarity_ts-1.0.1/src/similarity_ts.egg-info/PKG-INFO` & `similarity_ts-1.0.2/src/similarity_ts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity-ts
-Version: 1.0.1
+Version: 1.0.2
 Summary: SimilarityTS is an open-source project designed to facilitate the evaluation and comparison of multivariate time series data
 Author-email: Alejandro Fernández-Montes <afdez@us.es>, Damián Fernández-Cerero <damiancerero@us.es>, Felipe Escalera González <fescalera@us.es>
 Project-URL: Homepage, https://github.com/alejandrofdez-us/similarity-ts
 Project-URL: Bug Tracker, https://github.com/alejandrofdez-us/similarity-ts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -129,14 +129,15 @@
 
 (*) The metric used for the selection of the most
 similar `ts1` time-series window per each `ts2s` time-series file is selectable.`dtw` is the default selected metric, however, any of
 the
 [metrics](#available-metrics) are also available for this purpose. See the [toolkit configuration section](#configuring-the-toolkit)
 
 ### Minimal usage examples:
+Usage examples can be found at: https://github.com/alejandrofdez-us/similarity-ts/tree/main/usage_examples
 
 1. Compute metrics between random time series (`ts1`: one time series of lenght 200 and 2 dimensions and `ts2`: five time series of length 100 and 2 dimensions):
     ```Python
     import numpy as np
     from similarity_ts.similarity_ts import SimilarityTs
     
     ts1 = np.random.rand(200, 2)
```

### Comparing `similarity_ts-1.0.1/src/similarity_ts.egg-info/SOURCES.txt` & `similarity_ts-1.0.2/src/similarity_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

