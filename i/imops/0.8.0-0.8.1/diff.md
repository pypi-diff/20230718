# Comparing `tmp/imops-0.8.0.tar.gz` & `tmp/imops-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imops-0.8.0.tar", last modified: Fri Jun  2 16:00:47 2023, max compression
+gzip compressed data, was "imops-0.8.1.tar", last modified: Tue Jul 18 15:11:31 2023, max compression
```

## Comparing `imops-0.8.0.tar` & `imops-0.8.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:00:47.351621 imops-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-02 16:00:44.000000 imops-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-02 16:00:44.000000 imops-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-02 16:00:47.351621 imops-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-06-02 16:00:44.000000 imops-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-02 16:00:44.000000 imops-0.8.0/_pyproject_build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:00:47.343621 imops-0.8.0/imops/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-02 16:00:44.000000 imops-0.8.0/imops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 16:00:44.000000 imops-0.8.0/imops/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-02 16:00:44.000000 imops-0.8.0/imops/_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-02 16:00:44.000000 imops-0.8.0/imops/_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-02 16:00:44.000000 imops-0.8.0/imops/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-02 16:00:44.000000 imops-0.8.0/imops/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-02 16:00:44.000000 imops-0.8.0/imops/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-06-02 16:00:44.000000 imops-0.8.0/imops/interp1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-02 16:00:44.000000 imops-0.8.0/imops/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-02 16:00:44.000000 imops-0.8.0/imops/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-02 16:00:44.000000 imops-0.8.0/imops/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-06-02 16:00:44.000000 imops-0.8.0/imops/radon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:00:47.351621 imops-0.8.0/imops/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_backprojection.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_fast_backprojection.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_fast_measure.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_fast_morphology.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_fast_numeric.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_fast_radon.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_fast_zoom.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_measure.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_morphology.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_numba_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_numeric.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_radon.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-06-02 16:00:44.000000 imops-0.8.0/imops/src/_zoom.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-02 16:00:44.000000 imops-0.8.0/imops/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-02 16:00:44.000000 imops-0.8.0/imops/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-02 16:00:44.000000 imops-0.8.0/imops/zoom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:00:47.343621 imops-0.8.0/imops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-02 16:00:47.000000 imops-0.8.0/imops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-02 16:00:47.000000 imops-0.8.0/imops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:00:47.000000 imops-0.8.0/imops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-02 16:00:47.000000 imops-0.8.0/imops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 16:00:47.000000 imops-0.8.0/imops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-02 16:00:44.000000 imops-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-02 16:00:44.000000 imops-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:00:47.351621 imops-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-02 16:00:44.000000 imops-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:11:31.587496 imops-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 15:11:29.000000 imops-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 15:11:29.000000 imops-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-18 15:11:31.587496 imops-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-18 15:11:29.000000 imops-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-18 15:11:29.000000 imops-0.8.1/_pyproject_build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:11:31.583496 imops-0.8.1/imops/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 15:11:29.000000 imops-0.8.1/imops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 15:11:29.000000 imops-0.8.1/imops/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-18 15:11:29.000000 imops-0.8.1/imops/_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-18 15:11:29.000000 imops-0.8.1/imops/_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-18 15:11:29.000000 imops-0.8.1/imops/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-18 15:11:29.000000 imops-0.8.1/imops/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-18 15:11:29.000000 imops-0.8.1/imops/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-07-18 15:11:29.000000 imops-0.8.1/imops/interp1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-18 15:11:29.000000 imops-0.8.1/imops/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-18 15:11:29.000000 imops-0.8.1/imops/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-18 15:11:29.000000 imops-0.8.1/imops/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-07-18 15:11:29.000000 imops-0.8.1/imops/radon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:11:31.587496 imops-0.8.1/imops/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_backprojection.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_fast_backprojection.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_fast_measure.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_fast_morphology.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_fast_numeric.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_fast_radon.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_fast_zoom.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_measure.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_morphology.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_numba_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_numeric.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_radon.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-07-18 15:11:29.000000 imops-0.8.1/imops/src/_zoom.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 15:11:29.000000 imops-0.8.1/imops/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-18 15:11:29.000000 imops-0.8.1/imops/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-18 15:11:29.000000 imops-0.8.1/imops/zoom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:11:31.587496 imops-0.8.1/imops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-18 15:11:31.000000 imops-0.8.1/imops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-18 15:11:31.000000 imops-0.8.1/imops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:11:31.000000 imops-0.8.1/imops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-18 15:11:31.000000 imops-0.8.1/imops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:11:31.000000 imops-0.8.1/imops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-18 15:11:29.000000 imops-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-18 15:11:29.000000 imops-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:11:31.587496 imops-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-18 15:11:29.000000 imops-0.8.1/setup.py
```

### Comparing `imops-0.8.0/LICENSE` & `imops-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/PKG-INFO` & `imops-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: imops
-Version: 0.8.0
+Version: 0.8.1
 Summary: Efficient parallelizable algorithms for multidimensional arrays to speed up your data pipelines
 Home-page: https://github.com/neuro-ml/imops
 Author: maxme1, vovaf709, talgat
 Author-email: maxs987@gmail.com, vovaf709@yandex.ru, saparov2130@gmail.com
 License: MIT
-Download-URL: https://github.com/neuro-ml/imops/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/neuro-ml/imops/archive/v0.8.1.tar.gz
 Keywords: image processing,fast,ndarray,data pipelines
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `imops-0.8.0/README.md` & `imops-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/_pyproject_build.py` & `imops-0.8.1/_pyproject_build.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/_configs.py` & `imops-0.8.1/imops/_configs.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/_numeric.py` & `imops-0.8.1/imops/_numeric.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/backend.py` & `imops-0.8.1/imops/backend.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/box.py` & `imops-0.8.1/imops/box.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/crop.py` & `imops-0.8.1/imops/crop.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/interp1d.py` & `imops-0.8.1/imops/interp1d.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/measure.py` & `imops-0.8.1/imops/measure.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/morphology.py` & `imops-0.8.1/imops/morphology.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/pad.py` & `imops-0.8.1/imops/pad.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/radon.py` & `imops-0.8.1/imops/radon.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_backprojection.pyx` & `imops-0.8.1/imops/src/_backprojection.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_fast_backprojection.pyx` & `imops-0.8.1/imops/src/_fast_backprojection.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_fast_measure.pyx` & `imops-0.8.1/imops/src/_fast_measure.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_fast_morphology.pyx` & `imops-0.8.1/imops/src/_fast_morphology.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_fast_numeric.pyx` & `imops-0.8.1/imops/src/_fast_numeric.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_fast_radon.pyx` & `imops-0.8.1/imops/src/_fast_radon.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_fast_zoom.pyx` & `imops-0.8.1/imops/src/_fast_zoom.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_measure.pyx` & `imops-0.8.1/imops/src/_measure.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_morphology.pyx` & `imops-0.8.1/imops/src/_morphology.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_numba_zoom.py` & `imops-0.8.1/imops/src/_numba_zoom.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_numeric.pyx` & `imops-0.8.1/imops/src/_numeric.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_radon.pyx` & `imops-0.8.1/imops/src/_radon.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/src/_zoom.pyx` & `imops-0.8.1/imops/src/_zoom.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/testing.py` & `imops-0.8.1/imops/testing.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/utils.py` & `imops-0.8.1/imops/utils.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops/zoom.py` & `imops-0.8.1/imops/zoom.py`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/imops.egg-info/PKG-INFO` & `imops-0.8.1/imops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: imops
-Version: 0.8.0
+Version: 0.8.1
 Summary: Efficient parallelizable algorithms for multidimensional arrays to speed up your data pipelines
 Home-page: https://github.com/neuro-ml/imops
 Author: maxme1, vovaf709, talgat
 Author-email: maxs987@gmail.com, vovaf709@yandex.ru, saparov2130@gmail.com
 License: MIT
-Download-URL: https://github.com/neuro-ml/imops/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/neuro-ml/imops/archive/v0.8.1.tar.gz
 Keywords: image processing,fast,ndarray,data pipelines
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `imops-0.8.0/imops.egg-info/SOURCES.txt` & `imops-0.8.1/imops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imops-0.8.0/pyproject.toml` & `imops-0.8.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ['setuptools', 'numpy', 'Cython']
+requires = ['setuptools', 'numpy', 'Cython<3.0.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'imops'
 dynamic = ['version']
 description = 'Efficient parallelizable algorithms for multidimensional arrays to speed up your data pipelines'
 readme = 'README.md'
@@ -21,23 +21,14 @@
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
-dependencies = [
-    "numpy>=1.7,<2.0.0; python_version < '3.8'",
-    "numpy>=1.22,<2.0.0; python_version >= '3.8'",
-    'scipy>=1.0,<2.0.0',
-    "dataclasses; python_version < '3.7'",
-    'Cython',
-    'connected-components-3d',
-    'fastremap',
-]
 
 [options]
 include_package_data = true
 
 [project.optional-dependencies]
 numba = ['numba']
 
@@ -74,7 +65,8 @@
 include = ['imops']
 
 [tool.setuptools.package-data]
 imops = ['py.typed']
 
 [tool.setuptools.dynamic]
 version = {attr = 'imops.__version__.__version__'}
+dependencies = { file = ['requirements.txt'] }
```

### Comparing `imops-0.8.0/setup.py` & `imops-0.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,12 +77,12 @@
     ],
     classifiers=classifiers,
     install_requires=requirements,
     extras_require={'numba': ['numba'], 'all': ['numba']},
     setup_requires=[
         # Setuptools 18.0 properly handles Cython extensions.
         'setuptools>=18.0',
-        'Cython',
+        'Cython<3.0.0',
     ],
     ext_modules=ext_modules,
     python_requires='>=3.6',
 )
```

