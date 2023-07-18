# Comparing `tmp/phenotype_cover-0.8.tar.gz` & `tmp/phenotype_cover-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenotype_cover-0.8.tar", last modified: Wed Apr 19 15:22:52 2023, max compression
+gzip compressed data, was "phenotype_cover-0.9.tar", last modified: Tue Jul 18 13:50:31 2023, max compression
```

## Comparing `phenotype_cover-0.8.tar` & `phenotype_cover-0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.250129 phenotype_cover-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-19 15:22:40.000000 phenotype_cover-0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 15:22:40.000000 phenotype_cover-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 15:22:52.250129 phenotype_cover-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-19 15:22:40.000000 phenotype_cover-0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.246129 phenotype_cover-0.8/phenotype_cover.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:22:52.250129 phenotype_cover-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-19 15:22:40.000000 phenotype_cover-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.246129 phenotype_cover-0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.250129 phenotype_cover-0.8/src/phenotype_cover/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16346 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_gci_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_phenotype_cover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.250129 phenotype_cover-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-19 15:22:40.000000 phenotype_cover-0.8/tests/test_pairmat_construction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-19 15:22:40.000000 phenotype_cover-0.8/tests/test_phenotype_cover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:50:31.231986 phenotype_cover-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-18 13:50:22.000000 phenotype_cover-0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 13:50:22.000000 phenotype_cover-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 13:50:31.231986 phenotype_cover-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-18 13:50:22.000000 phenotype_cover-0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:50:31.227985 phenotype_cover-0.9/phenotype_cover.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 13:50:31.000000 phenotype_cover-0.9/phenotype_cover.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-18 13:50:31.000000 phenotype_cover-0.9/phenotype_cover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:50:31.000000 phenotype_cover-0.9/phenotype_cover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 13:50:31.000000 phenotype_cover-0.9/phenotype_cover.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 13:50:31.000000 phenotype_cover-0.9/phenotype_cover.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:50:31.231986 phenotype_cover-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-18 13:50:22.000000 phenotype_cover-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:50:31.227985 phenotype_cover-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:50:31.231986 phenotype_cover-0.9/src/phenotype_cover/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 13:50:22.000000 phenotype_cover-0.9/src/phenotype_cover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-18 13:50:22.000000 phenotype_cover-0.9/src/phenotype_cover/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16346 2023-07-18 13:50:22.000000 phenotype_cover-0.9/src/phenotype_cover/_gci_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-18 13:50:22.000000 phenotype_cover-0.9/src/phenotype_cover/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-18 13:50:22.000000 phenotype_cover-0.9/src/phenotype_cover/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-07-18 13:50:22.000000 phenotype_cover-0.9/src/phenotype_cover/_phenotype_cover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:50:31.231986 phenotype_cover-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-18 13:50:22.000000 phenotype_cover-0.9/tests/test_pairmat_construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-18 13:50:22.000000 phenotype_cover-0.9/tests/test_phenotype_cover.py
```

### Comparing `phenotype_cover-0.8/LICENSE.txt` & `phenotype_cover-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phenotype_cover-0.8/PKG-INFO` & `phenotype_cover-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenotype_cover
-Version: 0.8
+Version: 0.9
 Summary: phenotype_cover is a package for biomarker discovery using multiset multicover.
 Home-page: https://github.com/euxhenh/phenotype-cover
 Author: Euxhen Hasanaj
 Author-email: ehasanaj@cs.cmu.edu
 License: MIT
 Keywords: biomarker,marker,phenotype,scRNA-seq,set,cover,multiset,multicover
 Platform: ALL
```

### Comparing `phenotype_cover-0.8/README.rst` & `phenotype_cover-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `phenotype_cover-0.8/phenotype_cover.egg-info/PKG-INFO` & `phenotype_cover-0.9/phenotype_cover.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenotype-cover
-Version: 0.8
+Version: 0.9
 Summary: phenotype_cover is a package for biomarker discovery using multiset multicover.
 Home-page: https://github.com/euxhenh/phenotype-cover
 Author: Euxhen Hasanaj
 Author-email: ehasanaj@cs.cmu.edu
 License: MIT
 Keywords: biomarker,marker,phenotype,scRNA-seq,set,cover,multiset,multicover
 Platform: ALL
```

### Comparing `phenotype_cover-0.8/setup.py` & `phenotype_cover-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 options = {
     'name': 'phenotype_cover',
     'description': 'phenotype_cover is a package for biomarker discovery using multiset multicover.',
     'long_description': 'Implements the greedy and cross-entropy-method phenotype cover algorithms.',
     'license': 'MIT',
-    'version': '0.8',
+    'version': '0.9',
     'author': 'Euxhen Hasanaj',
     'author_email': 'ehasanaj@cs.cmu.edu',
     'url': 'https://github.com/euxhenh/phenotype-cover',
     'provides': ['phenotype_cover'],
     'package_dir': {'phenotype_cover': 'src/phenotype_cover'},
     'packages': find_packages(where='src'),
     'cmdclass': cmdclass,
```

### Comparing `phenotype_cover-0.8/src/phenotype_cover/_base.py` & `phenotype_cover-0.9/src/phenotype_cover/_base.py`

 * *Files identical despite different names*

### Comparing `phenotype_cover-0.8/src/phenotype_cover/_gci_wrapper.py` & `phenotype_cover-0.9/src/phenotype_cover/_gci_wrapper.py`

 * *Files identical despite different names*

### Comparing `phenotype_cover-0.8/src/phenotype_cover/_operations.py` & `phenotype_cover-0.9/src/phenotype_cover/_operations.py`

 * *Files identical despite different names*

### Comparing `phenotype_cover-0.8/src/phenotype_cover/_phenotype_cover.py` & `phenotype_cover-0.9/src/phenotype_cover/_phenotype_cover.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,16 +176,16 @@
 
         solution = self._gci_wrapper.predict(coverage, max_iters)
         self.solution = solution
         self.feature_importances_ = np.zeros(self.n_features_)
         self.feature_importances_[solution] = np.arange(
             len(solution) + 1, 1, -1)
         if self.n_pairs_with_incomplete_cover_ > 0 and self.verbose:
-            logger.warn("Could not cover "
-                        f"{self.n_pairs_with_incomplete_cover_} elements.")
+            logger.warning("Could not cover "
+                           f"{self.n_pairs_with_incomplete_cover_} elements.")
 
         self.n_outputs_ = len(solution)
         logger.info(f"Selected {self.n_outputs_} multisets.")
 
         return self.solution
 
     def plot_progress(self):
```

### Comparing `phenotype_cover-0.8/tests/test_pairmat_construction.py` & `phenotype_cover-0.9/tests/test_pairmat_construction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 import numpy as np
 from scipy.sparse import csr_matrix
 from numpy.testing import assert_allclose
-from src.phenotype_cover import pairwise_differences, group_by
+from phenotype_cover._operations import pairwise_differences, group_by
 
 
 class TestSelectors(unittest.TestCase):
     def test1(self):
         a = np.array([
             [1, 2, 6, 1],
             [3, 6, 7, 1],
```

### Comparing `phenotype_cover-0.8/tests/test_phenotype_cover.py` & `phenotype_cover-0.9/tests/test_phenotype_cover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 from numpy.testing import assert_allclose
 from sklearn.feature_selection import SelectFromModel
 
-from src.phenotype_cover import GreedyPC
-from src.phenotype_cover._gci_wrapper import GCIPython, GCIWrapper
+from phenotype_cover import GreedyPC
+from phenotype_cover._gci_wrapper import GCIPython, GCIWrapper
 
 
 def wrap(gci, x):
     gci.fit(x)
 
     assert gci.n_elements == 4
     assert gci.n_multisets_ == 5
```

