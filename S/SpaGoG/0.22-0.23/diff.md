# Comparing `tmp/SpaGoG-0.22.tar.gz` & `tmp/SpaGoG-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpaGoG-0.22.tar", last modified: Tue Jul 18 09:40:05 2023, max compression
+gzip compressed data, was "dist/SpaGoG-0.23.tar", last modified: Tue Jul 18 11:18:22 2023, max compression
```

## Comparing `SpaGoG-0.22.tar` & `SpaGoG-0.23.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1360 2023-07-18 09:39:59.000000 SpaGoG-0.22/setup.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1058 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/SOURCES.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/dependency_links.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        7 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/top_level.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       40 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/requires.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      266 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/PKG-INFO
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       79 2023-07-18 09:40:05.000000 SpaGoG-0.22/setup.cfg
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      266 2023-07-18 09:40:05.000000 SpaGoG-0.22/PKG-INFO
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     3196 2023-07-04 01:44:28.000000 SpaGoG-0.22/README.md
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/models/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    17250 2023-07-18 09:22:46.000000 SpaGoG-0.22/spagog/models/graphNodeClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/models/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6708 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/models/graphClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    14128 2023-07-18 09:22:45.000000 SpaGoG-0.22/spagog/models/abstractNN.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     3979 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/models/nodeClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      423 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/models/abstractModel.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/datasets/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7421 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/tabDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1986 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/graphDataset.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11819 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/tabDataset.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7321 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/graphDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7661 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/graphsDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    13210 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/graphsDataset.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/utils/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6338 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/knn.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     2887 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/gfp.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/__init__.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/utils/metrics/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/metrics/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1799 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/metrics/metrics.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/utils/data/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6347 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/data/tab2graph.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/data/__init__.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/default_params/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      260 2023-07-18 09:32:18.000000 SpaGoG-0.22/spagog/default_params/gc.json
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      618 2023-07-18 09:32:18.000000 SpaGoG-0.22/spagog/default_params/gnc.json
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:43.000000 SpaGoG-0.22/spagog/default_params/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      706 2023-05-12 23:49:43.000000 SpaGoG-0.22/spagog/default_params/load_params.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      649 2023-07-18 09:32:18.000000 SpaGoG-0.22/spagog/default_params/gc+nc.json
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     5202 2023-07-04 11:37:43.000000 SpaGoG-0.22/spagog/main.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    12191 2023-07-18 09:35:02.000000 SpaGoG-0.22/spagog/experiments.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/data/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     3426 2023-06-22 20:14:46.000000 SpaGoG-0.22/spagog/data/load_data.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:40.000000 SpaGoG-0.22/spagog/data/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1360 2023-07-18 11:18:18.000000 SpaGoG-0.23/setup.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/SpaGoG.egg-info/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1058 2023-07-18 11:18:22.000000 SpaGoG-0.23/SpaGoG.egg-info/SOURCES.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-07-18 11:18:22.000000 SpaGoG-0.23/SpaGoG.egg-info/dependency_links.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        7 2023-07-18 11:18:22.000000 SpaGoG-0.23/SpaGoG.egg-info/top_level.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       40 2023-07-18 11:18:22.000000 SpaGoG-0.23/SpaGoG.egg-info/requires.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      266 2023-07-18 11:18:22.000000 SpaGoG-0.23/SpaGoG.egg-info/PKG-INFO
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       79 2023-07-18 11:18:22.000000 SpaGoG-0.23/setup.cfg
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      266 2023-07-18 11:18:22.000000 SpaGoG-0.23/PKG-INFO
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     3196 2023-07-04 01:44:28.000000 SpaGoG-0.23/README.md
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/spagog/
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/spagog/models/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    17250 2023-07-18 09:22:46.000000 SpaGoG-0.23/spagog/models/graphNodeClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/models/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6708 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/models/graphClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    14128 2023-07-18 09:22:45.000000 SpaGoG-0.23/spagog/models/abstractNN.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     3979 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/models/nodeClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      423 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/models/abstractModel.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/spagog/datasets/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7421 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/datasets/tabDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1986 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/datasets/graphDataset.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/datasets/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    12195 2023-07-18 11:15:12.000000 SpaGoG-0.23/spagog/datasets/tabDataset.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7321 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/datasets/graphDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7661 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/datasets/graphsDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    13210 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/datasets/graphsDataset.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/spagog/utils/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6338 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/utils/knn.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     2887 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/utils/gfp.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/utils/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/spagog/utils/metrics/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/utils/metrics/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1799 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/utils/metrics/metrics.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/spagog/utils/data/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6347 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/utils/data/tab2graph.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/utils/data/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/spagog/default_params/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      260 2023-07-18 09:32:18.000000 SpaGoG-0.23/spagog/default_params/gc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      618 2023-07-18 09:32:18.000000 SpaGoG-0.23/spagog/default_params/gnc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:43.000000 SpaGoG-0.23/spagog/default_params/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      706 2023-05-12 23:49:43.000000 SpaGoG-0.23/spagog/default_params/load_params.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      649 2023-07-18 09:32:18.000000 SpaGoG-0.23/spagog/default_params/gc+nc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     5202 2023-07-04 11:37:43.000000 SpaGoG-0.23/spagog/main.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.23/spagog/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    12191 2023-07-18 09:35:02.000000 SpaGoG-0.23/spagog/experiments.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 11:18:22.000000 SpaGoG-0.23/spagog/data/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     3426 2023-06-22 20:14:46.000000 SpaGoG-0.23/spagog/data/load_data.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:40.000000 SpaGoG-0.23/spagog/data/__init__.py
```

### Comparing `SpaGoG-0.22/setup.py` & `SpaGoG-0.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from distutils.core import setup
 
 setup(
     name='SpaGoG',  # How you named your package folder (MyLib)
     packages=setuptools.find_packages(),  # Chose the same as "name"
-    version='0.22',  # Start with a small number and increase it with every change you make
+    version='0.23',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Sparse data classification using Graph of Graphs',  # Give a short description about your library
     author='Shachar Hananya',  # Type in your name
     author_email='shacharhananya@gmail.com',  # Type in your E-Mail
     # url='https://github.com/HananyaS/SpaGoG',  # Provide either the link to your github or to your website
     # download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.2.tar.gz',  # I explain this later on
     keywords=['GoG', 'Missing values', 'Graphs'],  # Keywords that define your package best
```

### Comparing `SpaGoG-0.22/SpaGoG.egg-info/SOURCES.txt` & `SpaGoG-0.23/SpaGoG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/README.md` & `SpaGoG-0.23/README.md`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/models/graphNodeClassification.py` & `SpaGoG-0.23/spagog/models/graphNodeClassification.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/models/graphClassification.py` & `SpaGoG-0.23/spagog/models/graphClassification.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/models/abstractNN.py` & `SpaGoG-0.23/spagog/models/abstractNN.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/models/nodeClassification.py` & `SpaGoG-0.23/spagog/models/nodeClassification.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/datasets/tabDataPair.py` & `SpaGoG-0.23/spagog/datasets/tabDataPair.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/datasets/graphDataset.py` & `SpaGoG-0.23/spagog/datasets/graphDataset.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/datasets/tabDataset.py` & `SpaGoG-0.23/spagog/datasets/tabDataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,70 +13,74 @@
 from sklearn.model_selection import train_test_split
 
 
 class TabDataset:
     _input_types = Union[torch.Tensor, np.ndarray]
 
     def __init__(
-            self,
-            name: str,
-            train: TabDataPair,
-            test: TabDataPair = None,
-            val: TabDataPair = None,
-            normalize: bool = False,
-            feature_selection: int = None,
+        self,
+        name: str,
+        train: TabDataPair,
+        test: TabDataPair = None,
+        val: TabDataPair = None,
+        normalize: bool = False,
+        feature_selection: int = None,
     ):
         self.name = name
         self.normalized = False
 
         self.train = train
         self.test_exists = test is not None
         self.val_exists = val is not None
 
         if self.test_exists:
             assert (
-                    test.get_num_features() == train.get_num_features()
+                test.get_num_features() == train.get_num_features()
             ), "Test doesn't have the same number of features as in train"
             self.test = test
             self.test.denormalize(inplace=True)
 
         if self.val_exists:
             assert (
-                    val.get_num_features() == train.get_num_features()
+                val.get_num_features() == train.get_num_features()
             ), "Validation doesn't have the same number of features as in train"
             self.val = val
             self.val.denormalize(inplace=True)
 
         unique_vals = self.remove_feats()
 
-        is_one_hot = lambda i: len(unique_vals[i]) == 2 and 0 in unique_vals[i] and 1 in unique_vals[i]
+        is_one_hot = (
+            lambda i: len(unique_vals[i]) == 2
+            and 0 in unique_vals[i]
+            and 1 in unique_vals[i]
+        )
         one_hot_feats = list(filter(is_one_hot, range(len(unique_vals))))
 
         self.one_hot_feats = one_hot_feats
 
         if normalize:
             self.zscore()
 
         if (
-                feature_selection is not None
-                and 1 < int(feature_selection) < self.train.get_num_features()
+            feature_selection is not None
+            and 1 < int(feature_selection) < self.train.get_num_features()
         ):
             print(f"Selecting best {int(feature_selection)} features!")
             X_train_np = self.train.X.numpy()
             row, col = np.where(1 - np.isnan(X_train_np))
             data = X_train_np[row, col]
 
             X_train_np = csr_matrix((data, (row, col)), shape=X_train_np.shape)
 
             Y_train_np = self.train.Y.detach().cpu().numpy()
 
             mi_scores = mutual_info_classif(X_train_np, Y_train_np)
             idx2remain = np.argpartition(mi_scores, kth=-int(feature_selection))[
-                         -int(feature_selection):
-                         ]
+                -int(feature_selection) :
+            ]
 
             self.train.X = self.train.X[:, idx2remain]
             self.val.X = self.val.X[:, idx2remain]
             self.test.X = self.test.X[:, idx2remain]
 
             new_one_hot_feats = []
 
@@ -84,26 +88,26 @@
                 if n in self.one_hot_feats:
                     new_one_hot_feats.append(i)
 
             self.one_hot_feats = new_one_hot_feats
 
     @classmethod
     def from_attributes(
-            cls,
-            name: str,
-            train_X: _input_types,
-            train_Y: _input_types = None,
-            test_X: _input_types = None,
-            test_Y: _input_types = None,
-            val_X: _input_types = None,
-            val_Y: _input_types = None,
-            shuffle: bool = False,
-            add_existence_cols: bool = False,
-            normalize: bool = True,
-            **kwargs,
+        cls,
+        name: str,
+        train_X: _input_types,
+        train_Y: _input_types = None,
+        test_X: _input_types = None,
+        test_Y: _input_types = None,
+        val_X: _input_types = None,
+        val_Y: _input_types = None,
+        shuffle: bool = False,
+        add_existence_cols: bool = False,
+        normalize: bool = True,
+        **kwargs,
     ):
         assert test_X is not None or test_Y is None
         assert val_X is not None or val_Y is None
 
         train = TabDataPair(
             X=train_X,
             Y=train_Y,
@@ -179,29 +183,40 @@
 
     def remove_feats(self):
         is_nan = lambda x: x == x
         find_unique_vals = lambda col: list(filter(is_nan, np.unique(col)))
 
         unique_vals = list(map(find_unique_vals, self.train.X.T))
 
-        feats2remain = list(filter(lambda i: len(unique_vals[i]) > 1, range(len(unique_vals))))
+        feats2remain = list(
+            filter(lambda i: len(unique_vals[i]) > 1, range(len(unique_vals)))
+        )
 
         self.train.X = self.train.X[:, feats2remain]
         self.test.X = self.test.X[:, feats2remain]
         self.val.X = self.val.X[:, feats2remain]
         unique_vals = [unique_vals[i] for i in feats2remain]
 
         if self.train.normalized:
-            self.train.norm_params = self.train.norm_params[0][feats2remain], self.train.norm_params[1][feats2remain]
+            self.train.norm_params = (
+                self.train.norm_params[0][feats2remain],
+                self.train.norm_params[1][feats2remain],
+            )
 
         if self.test.normalized:
-            self.test.norm_params = self.test.norm_params[0][feats2remain], self.test.norm_params[1][feats2remain]
+            self.test.norm_params = (
+                self.test.norm_params[0][feats2remain],
+                self.test.norm_params[1][feats2remain],
+            )
 
         if self.val.normalized:
-            self.val.norm_params = self.val.norm_params[0][feats2remain], self.val.norm_params[1][feats2remain]
+            self.val.norm_params = (
+                self.val.norm_params[0][feats2remain],
+                self.val.norm_params[1][feats2remain],
+            )
 
         return unique_vals
 
     def __str__(self):
         sets = ["train"]
 
         if self.test_exists:
@@ -215,15 +230,17 @@
     def zscore(self):
         if self.normalized:
             return self
 
         if self.train.normalized:
             self.train.denormalize(inplace=True)
 
-        _, mu, sigma = self.train.zscore(inplace=True, return_params=True, one_hot_features=self.one_hot_feats)
+        _, mu, sigma = self.train.zscore(
+            inplace=True, return_params=True, one_hot_features=self.one_hot_feats
+        )
 
         mu[self.one_hot_feats] = 0
         sigma[self.one_hot_feats] = 1
 
         if self.test_exists:
             if self.test.normalized:
                 self.test.denormalize(inplace=True)
@@ -304,42 +321,51 @@
             self.test.drop_existence_cols(inplace=True)
 
         if self.val_exists:
             self.val.drop_existence_cols(inplace=True)
 
     @classmethod
     def load(
-            cls,
-            train_X: pd.DataFrame = None,
-            train_Y: pd.DataFrame = None,
-            val_X: pd.DataFrame = None,
-            val_Y: pd.DataFrame = None,
-            test_X: pd.DataFrame = None,
-            test_Y: pd.DataFrame = None,
-            name: str = "",
-            **kwargs,
+        cls,
+        train_X: pd.DataFrame = None,
+        train_Y: pd.DataFrame = None,
+        val_X: pd.DataFrame = None,
+        val_Y: pd.DataFrame = None,
+        test_X: pd.DataFrame = None,
+        test_Y: pd.DataFrame = None,
+        split_if_no_val: bool = True,
+        name: str = "",
+        **kwargs,
     ):
         if train_X is not None and train_Y is not None and test_X is not None:
-            if val_X is None or val_Y is None:
-                train_X, val_X, train_Y, val_Y = train_test_split(train_X, train_Y, test_size=0.2, random_state=42)
+            if (val_X is None or val_Y is None) and split_if_no_val:
+                train_X, val_X, train_Y, val_Y = train_test_split(
+                    train_X, train_Y, test_size=0.2, random_state=42
+                )
 
             train_X = train_X.reset_index(drop=True)
             train_Y = train_Y.reset_index(drop=True)
-            val_X = val_X.reset_index(drop=True)
-            val_Y = val_Y.reset_index(drop=True)
-
             train_X = train_X.values
             train_Y = train_Y.values
-            val_X = val_X.values
-            val_Y = val_Y.values
             test_X = test_X.values
 
             if test_Y is not None:
                 test_Y = test_Y.values
 
+            if val_X is not None and val_Y is not None:
+                val_X = val_X.reset_index(drop=True)
+                val_Y = val_Y.reset_index(drop=True)
+
+                val_X = val_X.values
+                val_Y = val_Y.values
+
+            else:
+                val_X = None
+                val_Y = None
+
             return cls.from_attributes(
                 train_X=train_X,
                 train_Y=train_Y,
                 val_X=val_X,
                 val_Y=val_Y,
                 test_X=test_X,
                 test_Y=test_Y,
@@ -364,14 +390,16 @@
         else:
             val_mask = None
 
         if self.test_exists:
             test_data_X = self.get_test_data(as_loader=False).X
             all_data_X = torch.cat((all_data_X, test_data_X))
             if self.test.Y is not None:  # added if
-                all_data_Y = torch.cat((all_data_Y, self.get_test_data(as_loader=False).Y))
+                all_data_Y = torch.cat(
+                    (all_data_Y, self.get_test_data(as_loader=False).Y)
+                )
             test_mask = list(range(next_idx, next_idx + test_data_X.shape[0]))
 
         else:
             test_mask = None
 
         return all_data_X, all_data_Y, train_mask, val_mask, test_mask
```

### Comparing `SpaGoG-0.22/spagog/datasets/graphDataPair.py` & `SpaGoG-0.23/spagog/datasets/graphDataPair.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/datasets/graphsDataPair.py` & `SpaGoG-0.23/spagog/datasets/graphsDataPair.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/datasets/graphsDataset.py` & `SpaGoG-0.23/spagog/datasets/graphsDataset.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/utils/knn.py` & `SpaGoG-0.23/spagog/utils/knn.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/utils/gfp.py` & `SpaGoG-0.23/spagog/utils/gfp.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/utils/metrics/metrics.py` & `SpaGoG-0.23/spagog/utils/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/utils/data/tab2graph.py` & `SpaGoG-0.23/spagog/utils/data/tab2graph.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/default_params/gnc.json` & `SpaGoG-0.23/spagog/default_params/gnc.json`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/default_params/load_params.py` & `SpaGoG-0.23/spagog/default_params/load_params.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/default_params/gc+nc.json` & `SpaGoG-0.23/spagog/default_params/gc+nc.json`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/main.py` & `SpaGoG-0.23/spagog/main.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/experiments.py` & `SpaGoG-0.23/spagog/experiments.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.22/spagog/data/load_data.py` & `SpaGoG-0.23/spagog/data/load_data.py`

 * *Files identical despite different names*

