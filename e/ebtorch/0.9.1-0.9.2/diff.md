# Comparing `tmp/ebtorch-0.9.1.tar.gz` & `tmp/ebtorch-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebtorch-0.9.1.tar", last modified: Sat Jul 15 10:45:58 2023, max compression
+gzip compressed data, was "ebtorch-0.9.2.tar", last modified: Tue Jul 18 18:06:03 2023, max compression
```

## Comparing `ebtorch-0.9.1.tar` & `ebtorch-0.9.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.324609 ebtorch-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-15 10:45:44.000000 ebtorch-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-15 10:45:58.320608 ebtorch-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-15 10:45:44.000000 ebtorch-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.312608 ebtorch-0.9.1/ebtorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.316608 ebtorch-0.9.1/ebtorch/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/logging/avgmeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/logging/logcsv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.320608 ebtorch-0.9.1/ebtorch/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/conv2drp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/convolutional_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/coordconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/debuglayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/fieldtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.320608 ebtorch-0.9.1/ebtorch/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/functional/inner_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/kwta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/laplacenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/nnsemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/reshapelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/serf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/serlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/sinlu.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/smelu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.320608 ebtorch-0.9.1/ebtorch/nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/adverutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/autoclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/onlyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/reprutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.320608 ebtorch-0.9.1/ebtorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/adahessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/lookaround.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.316608 ebtorch-0.9.1/ebtorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 10:45:58.324609 ebtorch-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-15 10:45:44.000000 ebtorch-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:06:03.140245 ebtorch-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-18 18:05:49.000000 ebtorch-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 18:06:03.140245 ebtorch-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-18 18:05:49.000000 ebtorch-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:06:03.124245 ebtorch-0.9.2/ebtorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:06:03.128245 ebtorch-0.9.2/ebtorch/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/logging/avgmeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/logging/logcsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:06:03.136245 ebtorch-0.9.2/ebtorch/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/conv2drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/convolutional_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/coordconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/debuglayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/fieldtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:06:03.136245 ebtorch-0.9.2/ebtorch/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/functional/inner_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/kwta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/laplacenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/nnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/reshapelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/serf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/serlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/sinlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/smelu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:06:03.136245 ebtorch-0.9.2/ebtorch/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/utils/adverutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/utils/autoclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/utils/onlyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/nn/utils/reprutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:06:03.140245 ebtorch-0.9.2/ebtorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/optim/adahessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/optim/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/optim/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/optim/lookaround.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/optim/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-18 18:05:49.000000 ebtorch-0.9.2/ebtorch/optim/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:06:03.124245 ebtorch-0.9.2/ebtorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 18:06:03.000000 ebtorch-0.9.2/ebtorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-18 18:06:03.000000 ebtorch-0.9.2/ebtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:06:03.000000 ebtorch-0.9.2/ebtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:06:02.000000 ebtorch-0.9.2/ebtorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 18:06:03.000000 ebtorch-0.9.2/ebtorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:06:03.140245 ebtorch-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-18 18:05:49.000000 ebtorch-0.9.2/setup.py
```

### Comparing `ebtorch-0.9.1/LICENSE` & `ebtorch-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/PKG-INFO` & `ebtorch-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.1
+Version: 0.9.2
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.1 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.2 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.9.1/ebtorch/__init__.py` & `ebtorch-0.9.2/ebtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/logging/__init__.py` & `ebtorch-0.9.2/ebtorch/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/logging/avgmeter.py` & `ebtorch-0.9.2/ebtorch/logging/avgmeter.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/logging/logcsv.py` & `ebtorch-0.9.2/ebtorch/logging/logcsv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/__init__.py` & `ebtorch-0.9.2/ebtorch/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/architectures.py` & `ebtorch-0.9.2/ebtorch/nn/architectures.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/conv2drp.py` & `ebtorch-0.9.2/ebtorch/nn/conv2drp.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/convolutional_flatten.py` & `ebtorch-0.9.2/ebtorch/nn/convolutional_flatten.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/coordconv.py` & `ebtorch-0.9.2/ebtorch/nn/coordconv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/debuglayers.py` & `ebtorch-0.9.2/ebtorch/nn/debuglayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/fieldtransform.py` & `ebtorch-0.9.2/ebtorch/nn/fieldtransform.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/functional/__init__.py` & `ebtorch-0.9.2/ebtorch/nn/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/functional/inner_functional.py` & `ebtorch-0.9.2/ebtorch/nn/functional/inner_functional.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/kwta.py` & `ebtorch-0.9.2/ebtorch/nn/kwta.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/laplacenet.py` & `ebtorch-0.9.2/ebtorch/nn/laplacenet.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/mish.py` & `ebtorch-0.9.2/ebtorch/nn/mish.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/nnsemble.py` & `ebtorch-0.9.2/ebtorch/nn/nnsemble.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/reshapelayers.py` & `ebtorch-0.9.2/ebtorch/nn/reshapelayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/serf.py` & `ebtorch-0.9.2/ebtorch/nn/serf.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/serlu.py` & `ebtorch-0.9.2/ebtorch/nn/serlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/sinlu.py` & `ebtorch-0.9.2/ebtorch/nn/sinlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/smelu.py` & `ebtorch-0.9.2/ebtorch/nn/smelu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/utils/__init__.py` & `ebtorch-0.9.2/ebtorch/nn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/utils/adverutils.py` & `ebtorch-0.9.2/ebtorch/nn/utils/adverutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/utils/autoclip.py` & `ebtorch-0.9.2/ebtorch/nn/utils/autoclip.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/utils/onlyutils.py` & `ebtorch-0.9.2/ebtorch/nn/utils/onlyutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/utils/patches.py` & `ebtorch-0.9.2/ebtorch/nn/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/nn/utils/reprutils.py` & `ebtorch-0.9.2/ebtorch/nn/utils/reprutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/optim/__init__.py` & `ebtorch-0.9.2/ebtorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/optim/adahessian.py` & `ebtorch-0.9.2/ebtorch/optim/adahessian.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/optim/adan.py` & `ebtorch-0.9.2/ebtorch/optim/adan.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/optim/custom.py` & `ebtorch-0.9.2/ebtorch/optim/custom.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/optim/lion.py` & `ebtorch-0.9.2/ebtorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/optim/lookahead.py` & `ebtorch-0.9.2/ebtorch/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/optim/lookaround.py` & `ebtorch-0.9.2/ebtorch/optim/lookaround.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,19 +61,19 @@
             else:
                 d_p: Tensor = buf
         param.add_(d_p, alpha=-lr)
 
 
 def _parcheck(lr, required, momentum, weight_decay, nesterov, dampening):
     if lr is not required and lr < 0.0:
-        raise ValueError("Invalid learning rate: {}".format(lr))
+        raise ValueError(f"Invalid learning rate: {lr}")
     if momentum < 0.0:
-        raise ValueError("Invalid momentum value: {}".format(momentum))
+        raise ValueError(f"Invalid momentum value: {momentum}")
     if weight_decay < 0.0:
-        raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
+        raise ValueError(f"Invalid weight_decay value: {weight_decay}")
     if nesterov and (momentum <= 0 or dampening != 0):
         raise ValueError("Nesterov momentum requires a momentum and zero dampening")
 
 
 class Lookaround(Optimizer):
     def __init__(
         self,
@@ -82,15 +82,15 @@
         momentum=0,
         dampening=0,
         head_num=3,
         frequence=1,
         weight_decay=0,
         nesterov=False,
         *,
-        maximize=False
+        maximize=False,
     ):
         _parcheck(lr, required, momentum, weight_decay, nesterov, dampening)
         defaults = dict(
             lr=lr,
             momentum=momentum,
             dampening=dampening,
             weight_decay=weight_decay,
```

### Comparing `ebtorch-0.9.1/ebtorch/optim/radam.py` & `ebtorch-0.9.2/ebtorch/optim/radam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch/optim/sam.py` & `ebtorch-0.9.2/ebtorch/optim/sam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/ebtorch.egg-info/PKG-INFO` & `ebtorch-0.9.2/ebtorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.1
+Version: 0.9.2
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.1 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.2 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.9.1/ebtorch.egg-info/SOURCES.txt` & `ebtorch-0.9.2/ebtorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.1/setup.py` & `ebtorch-0.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 check_dependencies(DEPENDENCY_PACKAGE_NAMES)
 
 PACKAGENAME: str = "ebtorch"
 
 
 setup(
     name=PACKAGENAME,
-    version="0.9.1",
+    version="0.9.2",
     author="Emanuele Ballarin",
     author_email="emanuele@ballarin.cc",
     url="https://github.com/emaballarin/ebtorch",
     description="Collection of PyTorch additions, extensions, utilities, uses and abuses",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords=["Deep Learning", "Machine Learning"],
```

