# Comparing `tmp/csbdeep-0.7.3.tar.gz` & `tmp/csbdeep-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csbdeep-0.7.3.tar", last modified: Fri Feb 10 22:57:27 2023, max compression
+gzip compressed data, was "csbdeep-0.7.4.tar", last modified: Tue Jul 18 13:11:30 2023, max compression
```

## Comparing `csbdeep-0.7.3.tar` & `csbdeep-0.7.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-02-10 22:57:27.861290 csbdeep-0.7.3/
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     2110 2023-02-10 22:57:27.861290 csbdeep-0.7.3/PKG-INFO
--rw-rw-r--   0 uwe       (1000) uwe       (1000)      996 2022-05-20 14:22:35.000000 csbdeep-0.7.3/README.md
-drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-02-10 22:57:27.857290 csbdeep-0.7.3/csbdeep/
--rw-rw-r--   0 uwe       (1000) uwe       (1000)       89 2020-07-06 10:33:48.000000 csbdeep-0.7.3/csbdeep/__init__.py
-drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-02-10 22:57:27.861290 csbdeep-0.7.3/csbdeep/data/
--rw-rw-r--   0 uwe       (1000) uwe       (1000)      134 2018-06-06 10:43:33.000000 csbdeep-0.7.3/csbdeep/data/__init__.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)    18999 2022-05-20 14:22:35.000000 csbdeep-0.7.3/csbdeep/data/generate.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     8066 2019-06-19 10:28:49.000000 csbdeep-0.7.3/csbdeep/data/prepare.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     4548 2019-02-01 17:34:57.000000 csbdeep-0.7.3/csbdeep/data/rawdata.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)    14380 2022-05-20 14:22:35.000000 csbdeep-0.7.3/csbdeep/data/transform.py
-drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-02-10 22:57:27.861290 csbdeep-0.7.3/csbdeep/internals/
--rw-rw-r--   0 uwe       (1000) uwe       (1000)        0 2020-07-06 10:34:05.000000 csbdeep-0.7.3/csbdeep/internals/__init__.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     7437 2023-02-10 20:19:06.000000 csbdeep-0.7.3/csbdeep/internals/blocks.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     2326 2020-07-08 13:00:19.000000 csbdeep-0.7.3/csbdeep/internals/losses.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     6774 2020-07-08 13:00:19.000000 csbdeep-0.7.3/csbdeep/internals/nets.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)    17110 2020-02-10 21:46:09.000000 csbdeep-0.7.3/csbdeep/internals/predict.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     1933 2018-06-06 10:43:33.000000 csbdeep-0.7.3/csbdeep/internals/probability.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     5319 2020-12-17 21:34:37.000000 csbdeep-0.7.3/csbdeep/internals/train.py
-drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-02-10 22:57:27.861290 csbdeep-0.7.3/csbdeep/io/
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     5261 2022-05-20 14:22:46.000000 csbdeep-0.7.3/csbdeep/io/__init__.py
-drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-02-10 22:57:27.861290 csbdeep-0.7.3/csbdeep/models/
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     2193 2020-07-08 13:00:19.000000 csbdeep-0.7.3/csbdeep/models/__init__.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)    10918 2022-05-20 14:22:35.000000 csbdeep-0.7.3/csbdeep/models/base_model.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     6457 2022-05-20 14:22:35.000000 csbdeep-0.7.3/csbdeep/models/care_isotropic.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     7443 2020-07-08 13:00:19.000000 csbdeep-0.7.3/csbdeep/models/care_projection.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)    20596 2022-05-20 21:47:58.000000 csbdeep-0.7.3/csbdeep/models/care_standard.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     2084 2022-05-20 14:22:35.000000 csbdeep-0.7.3/csbdeep/models/care_upsampling.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)    10407 2022-05-20 14:22:46.000000 csbdeep-0.7.3/csbdeep/models/config.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     4244 2022-05-20 14:22:35.000000 csbdeep-0.7.3/csbdeep/models/pretrained.py
-drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-02-10 22:57:27.861290 csbdeep-0.7.3/csbdeep/scripts/
--rw-rw-r--   0 uwe       (1000) uwe       (1000)        0 2018-06-06 10:43:33.000000 csbdeep-0.7.3/csbdeep/scripts/__init__.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     9527 2022-05-20 14:22:46.000000 csbdeep-0.7.3/csbdeep/scripts/care_predict.py
-drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-02-10 22:57:27.861290 csbdeep-0.7.3/csbdeep/utils/
--rw-rw-r--   0 uwe       (1000) uwe       (1000)      156 2020-07-06 10:43:55.000000 csbdeep-0.7.3/csbdeep/utils/__init__.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     4223 2019-06-19 10:28:49.000000 csbdeep-0.7.3/csbdeep/utils/plot_utils.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)      409 2018-11-28 15:10:24.000000 csbdeep-0.7.3/csbdeep/utils/six.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)    25334 2021-08-19 22:20:39.000000 csbdeep-0.7.3/csbdeep/utils/tf.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     8161 2021-05-27 09:10:45.000000 csbdeep-0.7.3/csbdeep/utils/utils.py
--rw-rw-r--   0 uwe       (1000) uwe       (1000)       21 2023-02-10 22:44:30.000000 csbdeep-0.7.3/csbdeep/version.py
-drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-02-10 22:57:27.857290 csbdeep-0.7.3/csbdeep.egg-info/
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     2110 2023-02-10 22:57:27.000000 csbdeep-0.7.3/csbdeep.egg-info/PKG-INFO
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     1024 2023-02-10 22:57:27.000000 csbdeep-0.7.3/csbdeep.egg-info/SOURCES.txt
--rw-rw-r--   0 uwe       (1000) uwe       (1000)        1 2023-02-10 22:57:27.000000 csbdeep-0.7.3/csbdeep.egg-info/dependency_links.txt
--rw-rw-r--   0 uwe       (1000) uwe       (1000)       68 2023-02-10 22:57:27.000000 csbdeep-0.7.3/csbdeep.egg-info/entry_points.txt
--rw-rw-r--   0 uwe       (1000) uwe       (1000)      137 2023-02-10 22:57:27.000000 csbdeep-0.7.3/csbdeep.egg-info/requires.txt
--rw-rw-r--   0 uwe       (1000) uwe       (1000)        8 2023-02-10 22:57:27.000000 csbdeep-0.7.3/csbdeep.egg-info/top_level.txt
--rw-rw-r--   0 uwe       (1000) uwe       (1000)      108 2023-02-10 22:57:27.861290 csbdeep-0.7.3/setup.cfg
--rw-rw-r--   0 uwe       (1000) uwe       (1000)     1933 2023-02-10 22:45:14.000000 csbdeep-0.7.3/setup.py
+drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-07-18 13:11:30.112371 csbdeep-0.7.4/
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     2161 2023-07-18 13:11:30.112371 csbdeep-0.7.4/PKG-INFO
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)      996 2022-05-20 14:22:35.000000 csbdeep-0.7.4/README.md
+drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-07-18 13:11:30.112371 csbdeep-0.7.4/csbdeep/
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)       89 2020-07-06 10:33:48.000000 csbdeep-0.7.4/csbdeep/__init__.py
+drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-07-18 13:11:30.112371 csbdeep-0.7.4/csbdeep/data/
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)      134 2018-06-06 10:43:33.000000 csbdeep-0.7.4/csbdeep/data/__init__.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)    18999 2022-05-20 14:22:35.000000 csbdeep-0.7.4/csbdeep/data/generate.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     8066 2019-06-19 10:28:49.000000 csbdeep-0.7.4/csbdeep/data/prepare.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     4548 2019-02-01 17:34:57.000000 csbdeep-0.7.4/csbdeep/data/rawdata.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)    14380 2022-05-20 14:22:35.000000 csbdeep-0.7.4/csbdeep/data/transform.py
+drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-07-18 13:11:30.112371 csbdeep-0.7.4/csbdeep/internals/
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)        0 2020-07-06 10:34:05.000000 csbdeep-0.7.4/csbdeep/internals/__init__.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     7437 2023-02-10 20:19:06.000000 csbdeep-0.7.4/csbdeep/internals/blocks.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     2326 2020-07-08 13:00:19.000000 csbdeep-0.7.4/csbdeep/internals/losses.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     6774 2020-07-08 13:00:19.000000 csbdeep-0.7.4/csbdeep/internals/nets.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)    17110 2020-02-10 21:46:09.000000 csbdeep-0.7.4/csbdeep/internals/predict.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     1933 2018-06-06 10:43:33.000000 csbdeep-0.7.4/csbdeep/internals/probability.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     5562 2023-07-18 12:44:17.000000 csbdeep-0.7.4/csbdeep/internals/train.py
+drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-07-18 13:11:30.112371 csbdeep-0.7.4/csbdeep/io/
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     5261 2022-05-20 14:22:46.000000 csbdeep-0.7.4/csbdeep/io/__init__.py
+drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-07-18 13:11:30.112371 csbdeep-0.7.4/csbdeep/models/
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     2193 2020-07-08 13:00:19.000000 csbdeep-0.7.4/csbdeep/models/__init__.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)    10918 2022-05-20 14:22:35.000000 csbdeep-0.7.4/csbdeep/models/base_model.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     6457 2022-05-20 14:22:35.000000 csbdeep-0.7.4/csbdeep/models/care_isotropic.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     7443 2020-07-08 13:00:19.000000 csbdeep-0.7.4/csbdeep/models/care_projection.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)    20654 2023-07-18 12:44:17.000000 csbdeep-0.7.4/csbdeep/models/care_standard.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     2084 2022-05-20 14:22:35.000000 csbdeep-0.7.4/csbdeep/models/care_upsampling.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)    10489 2023-07-18 12:44:17.000000 csbdeep-0.7.4/csbdeep/models/config.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     4244 2022-05-20 14:22:35.000000 csbdeep-0.7.4/csbdeep/models/pretrained.py
+drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-07-18 13:11:30.112371 csbdeep-0.7.4/csbdeep/scripts/
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)        0 2018-06-06 10:43:33.000000 csbdeep-0.7.4/csbdeep/scripts/__init__.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     9527 2022-05-20 14:22:46.000000 csbdeep-0.7.4/csbdeep/scripts/care_predict.py
+drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-07-18 13:11:30.112371 csbdeep-0.7.4/csbdeep/utils/
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)      156 2020-07-06 10:43:55.000000 csbdeep-0.7.4/csbdeep/utils/__init__.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     4223 2019-06-19 10:28:49.000000 csbdeep-0.7.4/csbdeep/utils/plot_utils.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)      409 2018-11-28 15:10:24.000000 csbdeep-0.7.4/csbdeep/utils/six.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)    25334 2021-08-19 22:20:39.000000 csbdeep-0.7.4/csbdeep/utils/tf.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     8161 2021-05-27 09:10:45.000000 csbdeep-0.7.4/csbdeep/utils/utils.py
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)       21 2023-07-18 12:45:06.000000 csbdeep-0.7.4/csbdeep/version.py
+drwxrwxr-x   0 uwe       (1000) uwe       (1000)        0 2023-07-18 13:11:30.112371 csbdeep-0.7.4/csbdeep.egg-info/
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     2161 2023-07-18 13:11:30.000000 csbdeep-0.7.4/csbdeep.egg-info/PKG-INFO
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     1024 2023-07-18 13:11:30.000000 csbdeep-0.7.4/csbdeep.egg-info/SOURCES.txt
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)        1 2023-07-18 13:11:30.000000 csbdeep-0.7.4/csbdeep.egg-info/dependency_links.txt
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)       68 2023-07-18 13:11:30.000000 csbdeep-0.7.4/csbdeep.egg-info/entry_points.txt
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)      144 2023-07-18 13:11:30.000000 csbdeep-0.7.4/csbdeep.egg-info/requires.txt
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)        8 2023-07-18 13:11:30.000000 csbdeep-0.7.4/csbdeep.egg-info/top_level.txt
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)      108 2023-07-18 13:11:30.112371 csbdeep-0.7.4/setup.cfg
+-rw-rw-r--   0 uwe       (1000) uwe       (1000)     1994 2023-07-18 12:44:17.000000 csbdeep-0.7.4/setup.py
```

### Comparing `csbdeep-0.7.3/PKG-INFO` & `csbdeep-0.7.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csbdeep
-Version: 0.7.3
+Version: 0.7.4
 Summary: CSBDeep - a toolbox for Content-aware Image Restoration (CARE)
 Home-page: http://csbdeep.bioimagecomputing.com/
 Author: Uwe Schmidt, Martin Weigert
 Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
 License: BSD 3-Clause License
 Project-URL: Documentation, http://csbdeep.bioimagecomputing.com/doc/
 Project-URL: Repository, https://github.com/csbdeep/csbdeep
@@ -26,12 +26,13 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tf1
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `csbdeep-0.7.3/README.md` & `csbdeep-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/data/generate.py` & `csbdeep-0.7.4/csbdeep/data/generate.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/data/prepare.py` & `csbdeep-0.7.4/csbdeep/data/prepare.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/data/rawdata.py` & `csbdeep-0.7.4/csbdeep/data/rawdata.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/data/transform.py` & `csbdeep-0.7.4/csbdeep/data/transform.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/internals/blocks.py` & `csbdeep-0.7.4/csbdeep/internals/blocks.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/internals/losses.py` & `csbdeep-0.7.4/csbdeep/internals/losses.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/internals/nets.py` & `csbdeep-0.7.4/csbdeep/internals/nets.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/internals/predict.py` & `csbdeep-0.7.4/csbdeep/internals/predict.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/internals/probability.py` & `csbdeep-0.7.4/csbdeep/internals/probability.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/internals/train.py` & `csbdeep-0.7.4/csbdeep/internals/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,21 @@
 
     def __getitem__(self, i):
         return self.batch(i)
 
 
 class DataWrapper(RollingSequence):
 
-    def __init__(self, X, Y, batch_size, length):
+    def __init__(self, X, Y, batch_size, length, augmenter=None):
         super(DataWrapper, self).__init__(data_size=len(X), batch_size=batch_size, length=length, shuffle=True)
         len(X) == len(Y) or _raise(ValueError("X and Y must have same length"))
         self.X, self.Y = X, Y
+        self.augmenter = augmenter
 
     def __getitem__(self, i):
         idx = self.batch(i)
-        return self.X[idx], self.Y[idx]
+        X, Y = self.X[idx], self.Y[idx]
+        if self.augmenter is not None:
+            X,Y = tuple(zip(*tuple(self.augmenter(x,y) for x,y in zip(X,Y))))
+            X,Y = np.stack(X), np.stack(Y)
+            
+        return X,Y
```

### Comparing `csbdeep-0.7.3/csbdeep/io/__init__.py` & `csbdeep-0.7.4/csbdeep/io/__init__.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/models/__init__.py` & `csbdeep-0.7.4/csbdeep/models/__init__.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/models/base_model.py` & `csbdeep-0.7.4/csbdeep/models/base_model.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/models/care_isotropic.py` & `csbdeep-0.7.4/csbdeep/models/care_isotropic.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/models/care_projection.py` & `csbdeep-0.7.4/csbdeep/models/care_projection.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/models/care_standard.py` & `csbdeep-0.7.4/csbdeep/models/care_standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             If ``None`` (default), uses ``Adam`` with the learning rate specified in ``config``.
         kwargs : dict
             Additional arguments for :func:`csbdeep.internals.train.prepare_model`.
 
         """
         if optimizer is None:
             Adam = keras_import('optimizers', 'Adam')
-            learning_rate = 'lr' if Version(keras.__version__) < Version('2.3.0') else 'learning_rate'
+            learning_rate = 'lr' if Version(getattr(keras, '__version__', '9.9.9')) < Version('2.3.0') else 'learning_rate'
             optimizer = Adam(**{learning_rate: self.config.train_learning_rate})
         self.callbacks = train.prepare_model(self.keras_model, optimizer, self.config.train_loss, **kwargs)
 
         if self.basedir is not None:
             self.callbacks += self._checkpoint_callbacks()
 
             if self.config.train_tensorboard:
@@ -131,15 +131,15 @@
                 rlrop_params['verbose'] = True
             # TF2: add as first callback to put 'lr' in the logs for TensorBoard
             self.callbacks.insert(0,ReduceLROnPlateau(**rlrop_params))
 
         self._model_prepared = True
 
 
-    def train(self, X,Y, validation_data, epochs=None, steps_per_epoch=None):
+    def train(self, X,Y, validation_data, epochs=None, steps_per_epoch=None, augmenter=None):
         """Train the neural network with the given data.
 
         Parameters
         ----------
         X : :class:`numpy.ndarray`
             Array of source images.
         Y : :class:`numpy.ndarray`
@@ -186,15 +186,15 @@
 
         if (self.config.train_tensorboard and self.basedir is not None and
             not IS_TF_1 and not any(isinstance(cb,CARETensorBoardImage) for cb in self.callbacks)):
             self.callbacks.append(CARETensorBoardImage(model=self.keras_model, data=validation_data,
                                                        log_dir=str(self.logdir/'logs'/'images'),
                                                        n_images=3, prob_out=self.config.probabilistic))
 
-        training_data = train.DataWrapper(X, Y, self.config.train_batch_size, length=epochs*steps_per_epoch)
+        training_data = train.DataWrapper(X, Y, self.config.train_batch_size, length=epochs*steps_per_epoch, augmenter=augmenter)
 
         fit = self.keras_model.fit_generator if IS_TF_1 else self.keras_model.fit
         history = fit(iter(training_data), validation_data=validation_data,
                       epochs=epochs, steps_per_epoch=steps_per_epoch,
                       callbacks=self.callbacks, verbose=1)
         self._training_finished()
```

### Comparing `csbdeep-0.7.3/csbdeep/models/care_upsampling.py` & `csbdeep-0.7.4/csbdeep/models/care_upsampling.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/models/config.py` & `csbdeep-0.7.4/csbdeep/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,16 @@
         self.train_epochs          = 100
         self.train_steps_per_epoch = 400
         self.train_learning_rate   = 0.0004
         self.train_batch_size      = 16
         self.train_tensorboard     = True
 
         # the parameter 'min_delta' was called 'epsilon' for keras<=2.1.5
-        min_delta_key = 'epsilon' if Version(keras.__version__)<=Version('2.1.5') else 'min_delta'
+        # keras.__version__ was removed in tensorflow 2.13.0
+        min_delta_key = 'epsilon' if Version(getattr(keras, '__version__', '9.9.9'))<=Version('2.1.5') else 'min_delta'
         self.train_reduce_lr       = {'factor': 0.5, 'patience': 10, min_delta_key: 0}
 
         # disallow setting 'n_dim' manually
         try:
             del kwargs['n_dim']
             # warnings.warn("ignoring parameter 'n_dim'")
         except:
```

### Comparing `csbdeep-0.7.3/csbdeep/models/pretrained.py` & `csbdeep-0.7.4/csbdeep/models/pretrained.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/scripts/care_predict.py` & `csbdeep-0.7.4/csbdeep/scripts/care_predict.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/utils/plot_utils.py` & `csbdeep-0.7.4/csbdeep/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/utils/tf.py` & `csbdeep-0.7.4/csbdeep/utils/tf.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep/utils/utils.py` & `csbdeep-0.7.4/csbdeep/utils/utils.py`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/csbdeep.egg-info/PKG-INFO` & `csbdeep-0.7.4/csbdeep.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csbdeep
-Version: 0.7.3
+Version: 0.7.4
 Summary: CSBDeep - a toolbox for Content-aware Image Restoration (CARE)
 Home-page: http://csbdeep.bioimagecomputing.com/
 Author: Uwe Schmidt, Martin Weigert
 Author-email: research@uweschmidt.org, martin.weigert@epfl.ch
 License: BSD 3-Clause License
 Project-URL: Documentation, http://csbdeep.bioimagecomputing.com/doc/
 Project-URL: Repository, https://github.com/csbdeep/csbdeep
@@ -26,12 +26,13 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tf1
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `csbdeep-0.7.3/csbdeep.egg-info/SOURCES.txt` & `csbdeep-0.7.4/csbdeep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csbdeep-0.7.3/setup.py` & `csbdeep-0.7.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,28 +35,29 @@
           'License :: OSI Approved :: BSD License',
 
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
       ],
 
       install_requires=[
           "numpy",
           "scipy",
           "matplotlib",
           "six",
           "tifffile",
           "tqdm",
           "packaging",
       ],
 
       extras_require={
-          "tf1":  ["keras>=2.1.2,<2.4","protobuf<3.21"],
+          "tf1":  ["keras>=2.1.2,<2.4","protobuf<3.21","h5py<3"],
           "test": ["pytest"],
           "docs": ["sphinx","sphinx-rtd-theme"],
       },
 
       entry_points={
           'console_scripts': [
               'care_predict = csbdeep.scripts.care_predict:main'
```

