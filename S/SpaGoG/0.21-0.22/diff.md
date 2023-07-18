# Comparing `tmp/SpaGoG-0.21.tar.gz` & `tmp/SpaGoG-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpaGoG-0.21.tar", last modified: Mon Jun 26 09:56:42 2023, max compression
+gzip compressed data, was "dist/SpaGoG-0.22.tar", last modified: Tue Jul 18 09:40:05 2023, max compression
```

## Comparing `SpaGoG-0.21.tar` & `SpaGoG-0.22.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1359 2023-06-26 09:56:34.000000 SpaGoG-0.21/setup.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/SpaGoG.egg-info/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1055 2023-06-26 09:56:42.000000 SpaGoG-0.21/SpaGoG.egg-info/SOURCES.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-06-26 09:56:42.000000 SpaGoG-0.21/SpaGoG.egg-info/dependency_links.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        7 2023-06-26 09:56:42.000000 SpaGoG-0.21/SpaGoG.egg-info/top_level.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       40 2023-06-26 09:56:42.000000 SpaGoG-0.21/SpaGoG.egg-info/requires.txt
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      266 2023-06-26 09:56:42.000000 SpaGoG-0.21/SpaGoG.egg-info/PKG-INFO
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       79 2023-06-26 09:56:42.000000 SpaGoG-0.21/setup.cfg
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.21/README
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      266 2023-06-26 09:56:42.000000 SpaGoG-0.21/PKG-INFO
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/spagog/
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/spagog/models/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    17286 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/models/graphNodeClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/models/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6708 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/models/graphClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    14164 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/models/abstractNN.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     3979 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/models/nodeClassification.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      423 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/models/abstractModel.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/spagog/datasets/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7421 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/datasets/tabDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1986 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/datasets/graphDataset.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/datasets/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11819 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/datasets/tabDataset.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7321 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/datasets/graphDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     7661 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/datasets/graphsDataPair.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    13210 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/datasets/graphsDataset.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/spagog/utils/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6338 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/utils/knn.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     2887 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/utils/gfp.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/utils/__init__.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/spagog/utils/metrics/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/utils/metrics/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1799 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/utils/metrics/metrics.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/spagog/utils/data/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     6347 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/utils/data/tab2graph.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/utils/data/__init__.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/spagog/default_params/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      236 2023-05-12 23:49:43.000000 SpaGoG-0.21/spagog/default_params/gc.json
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      594 2023-05-12 23:49:43.000000 SpaGoG-0.21/spagog/default_params/gnc.json
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:43.000000 SpaGoG-0.21/spagog/default_params/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      706 2023-05-12 23:49:43.000000 SpaGoG-0.21/spagog/default_params/load_params.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      595 2023-05-12 23:49:43.000000 SpaGoG-0.21/spagog/default_params/gc+nc.json
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     5201 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/main.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.21/spagog/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11963 2023-06-26 08:07:41.000000 SpaGoG-0.21/spagog/experiments.py
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 09:56:42.000000 SpaGoG-0.21/spagog/data/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     3426 2023-06-22 20:14:46.000000 SpaGoG-0.21/spagog/data/load_data.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:40.000000 SpaGoG-0.21/spagog/data/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1360 2023-07-18 09:39:59.000000 SpaGoG-0.22/setup.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1058 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/SOURCES.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/dependency_links.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        7 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/top_level.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       40 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/requires.txt
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      266 2023-07-18 09:40:05.000000 SpaGoG-0.22/SpaGoG.egg-info/PKG-INFO
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       79 2023-07-18 09:40:05.000000 SpaGoG-0.22/setup.cfg
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      266 2023-07-18 09:40:05.000000 SpaGoG-0.22/PKG-INFO
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     3196 2023-07-04 01:44:28.000000 SpaGoG-0.22/README.md
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/models/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    17250 2023-07-18 09:22:46.000000 SpaGoG-0.22/spagog/models/graphNodeClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/models/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6708 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/models/graphClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    14128 2023-07-18 09:22:45.000000 SpaGoG-0.22/spagog/models/abstractNN.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     3979 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/models/nodeClassification.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      423 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/models/abstractModel.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/datasets/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7421 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/tabDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1986 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/graphDataset.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    11819 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/tabDataset.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7321 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/graphDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     7661 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/graphsDataPair.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    13210 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/datasets/graphsDataset.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/utils/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6338 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/knn.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     2887 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/gfp.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        1 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/utils/metrics/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/metrics/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1799 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/metrics/metrics.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/utils/data/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     6347 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/data/tab2graph.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/utils/data/__init__.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/default_params/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      260 2023-07-18 09:32:18.000000 SpaGoG-0.22/spagog/default_params/gc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      618 2023-07-18 09:32:18.000000 SpaGoG-0.22/spagog/default_params/gnc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:43.000000 SpaGoG-0.22/spagog/default_params/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      706 2023-05-12 23:49:43.000000 SpaGoG-0.22/spagog/default_params/load_params.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      649 2023-07-18 09:32:18.000000 SpaGoG-0.22/spagog/default_params/gc+nc.json
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     5202 2023-07-04 11:37:43.000000 SpaGoG-0.22/spagog/main.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.22/spagog/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    12191 2023-07-18 09:35:02.000000 SpaGoG-0.22/spagog/experiments.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-07-18 09:40:05.000000 SpaGoG-0.22/spagog/data/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     3426 2023-06-22 20:14:46.000000 SpaGoG-0.22/spagog/data/load_data.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-05-12 23:49:40.000000 SpaGoG-0.22/spagog/data/__init__.py
```

### Comparing `SpaGoG-0.21/setup.py` & `SpaGoG-0.22/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 from distutils.core import setup
 
 setup(
     name='SpaGoG',  # How you named your package folder (MyLib)
     packages=setuptools.find_packages(),  # Chose the same as "name"
-    version='0.21',  # Start with a small number and increase it with every change you make
+    version='0.22',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Sparse data classification using Graph of Graphs',  # Give a short description about your library
     author='Shachar Hananya',  # Type in your name
     author_email='shacharhananya@gmail.com',  # Type in your E-Mail
     # url='https://github.com/HananyaS/SpaGoG',  # Provide either the link to your github or to your website
     # download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.2.tar.gz',  # I explain this later on
     keywords=['GoG', 'Missing values', 'Graphs'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
         'pandas',
         'torch',
         'torch-geometric',
         'matplotlib',
     ],
     # classifiers=[
-    #     'License :: OSI Approved :: MIT License',  # Again, pick a license
+    #     'License :: OSI Approved :: MIT License',  # Again, pick a licensex
     #     'Programming Language :: Python :: 3.8',
     # ],
     # add the json files that appear in default_params folder
     package_data={'spagog': ['default_params/*.json']},
 )
```

### Comparing `SpaGoG-0.21/SpaGoG.egg-info/SOURCES.txt` & `SpaGoG-0.22/SpaGoG.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-README
+README.md
 setup.cfg
 setup.py
 SpaGoG.egg-info/PKG-INFO
 SpaGoG.egg-info/SOURCES.txt
 SpaGoG.egg-info/dependency_links.txt
 SpaGoG.egg-info/requires.txt
 SpaGoG.egg-info/top_level.txt
```

### Comparing `SpaGoG-0.21/spagog/models/graphNodeClassification.py` & `SpaGoG-0.22/spagog/models/graphNodeClassification.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,26 +148,26 @@
             train_mask: list,
             val_mask: list,
             test_mask: list,
             n_epochs: int = 100,
             batch_size: int = 32,
             optimizer: torch.optim = optim.Adam,
             alpha: float = 2,
-            early_stopping_patience: int = -1,
+            early_stopping: int = -1,
             verbose: bool = False,
             clf_from: str = 'nc',
             gc_lr: float = 0.001,
             gc_weight_decay: float = 0,
             nc_lr: float = 0.001,
             nc_weight_decay: float = 0,
     ):
 
         given_test_y = graphs_dataset.test.Y is not None
 
-        if early_stopping_patience > 0:
+        if early_stopping > 0:
             c = 0
             min_val_loss = np.inf
 
         (
             graphs_train_loader,
             graphs_val_loader,
             graphs_test_loader,
@@ -313,23 +313,23 @@
                     f"\tTrain total loss:\t{train_loss_total}\n",
                     f"\tTrain GC AUC:\t{train_gc_auc}\n",
                     f"\tVal GC AUC:\t{val_gc_auc}\n",
                     f"\tTrain final AUC:\t{train_final_auc}\n",
                     f"\tVal final AUC:\t{val_final_auc}\n",
                 )
 
-            if early_stopping_patience > 0:
+            if early_stopping > 0:
                 if val_loss_total < min_val_loss:
                     min_val_loss = val_loss_total
                     c = 0
 
                 else:
                     c += 1
 
-                if c == early_stopping_patience:
+                if c == early_stopping:
                     if verbose:
                         print(f"\nEarly stopping triggered at epoch {epoch}.\n")
                     break
 
         best_epoch, best_val_total_loss = np.argmin(val_total_losses) + 1, np.min(
             val_total_losses
         )
```

### Comparing `SpaGoG-0.21/spagog/models/graphClassification.py` & `SpaGoG-0.22/spagog/models/graphClassification.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/models/abstractNN.py` & `SpaGoG-0.22/spagog/models/abstractNN.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,25 +134,25 @@
         weight_decay: float = 0,
         optimizer: torch.optim = optim.Adam,
         verbose: bool = False,
         criterion: torch.nn.modules.loss = nn.CrossEntropyLoss(reduction="mean"),
         labels_from_loader: Callable = lambda loader: loader.dataset.gdp.Y,
         metric: str = "auc",
         save_model: bool = False,
-        early_stopping_patience: int = -1,
+        early_stopping: int = -1,
     ):
         assert metric in ["auc", "accuracy"]
 
         self.train()
         train_losses, val_losses = [], []
         train_aucs, val_aucs = [], []
 
         optimizer = optimizer(self.parameters(), lr=lr, weight_decay=weight_decay)
 
-        if early_stopping_patience > 0:
+        if early_stopping > 0:
             c = 0
             max_val_auc = np.inf
 
         t_per_epoch = []
         t_per_train_epoch = []
         t_per_val_epoch = []
         t_per_auc_epoch = []
@@ -243,23 +243,23 @@
                     f"Epoch {epoch}/{n_epochs}:\n"
                     f"\tTrain loss: {total_train_loss:.4f}\n"
                     f"\tVal loss: {total_val_loss:.4f}\n"
                     f"\tTrain AUC: {train_auc:.4f}\n"
                     f"\tVal AUC: {val_auc:.4f}"
                 )
 
-            if early_stopping_patience > 0:
+            if early_stopping > 0:
                 if val_auc > max_val_auc:
                     max_val_auc = val_auc
                     c = 0
 
                 else:
                     c += 1
 
-                if c == early_stopping_patience:
+                if c == early_stopping:
                     if verbose:
                         print(f"\nEarly stopping triggered at epoch {epoch}\n")
                     break
 
             t_per_epoch.append(time.time() - t_start)
 
         results_cache = self.evaluate(
```

### Comparing `SpaGoG-0.21/spagog/models/nodeClassification.py` & `SpaGoG-0.22/spagog/models/nodeClassification.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/datasets/tabDataPair.py` & `SpaGoG-0.22/spagog/datasets/tabDataPair.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/datasets/graphDataset.py` & `SpaGoG-0.22/spagog/datasets/graphDataset.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/datasets/tabDataset.py` & `SpaGoG-0.22/spagog/datasets/tabDataset.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/datasets/graphDataPair.py` & `SpaGoG-0.22/spagog/datasets/graphDataPair.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/datasets/graphsDataPair.py` & `SpaGoG-0.22/spagog/datasets/graphsDataPair.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/datasets/graphsDataset.py` & `SpaGoG-0.22/spagog/datasets/graphsDataset.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/utils/knn.py` & `SpaGoG-0.22/spagog/utils/knn.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/utils/gfp.py` & `SpaGoG-0.22/spagog/utils/gfp.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/utils/metrics/metrics.py` & `SpaGoG-0.22/spagog/utils/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/utils/data/tab2graph.py` & `SpaGoG-0.22/spagog/utils/data/tab2graph.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/default_params/gnc.json` & `SpaGoG-0.22/spagog/default_params/gnc.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'early_stopping'": '30'}*

```diff
@@ -1,11 +1,12 @@
 {
     "alpha": 0.5201743477,
     "clf_from": "gc",
     "distance": "heur_dist",
+    "early_stopping": 30,
     "embedding_layer": "one_before_last",
     "gc_activation": "elu",
     "gc_batch_size": 32,
     "gc_dropout": 0.1942761753,
     "gc_layer_1": 24,
     "gc_layer_2": 5,
     "gc_lr": 0.0001502896907,
```

### Comparing `SpaGoG-0.21/spagog/default_params/load_params.py` & `SpaGoG-0.22/spagog/default_params/load_params.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.21/spagog/main.py` & `SpaGoG-0.22/spagog/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             print(
                 f"\t\tTest:\t{res_cache['Test AUC']}"
             )
 
         print("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~")
 
     if verbosity > 0:
-        _et = time.time()
+        _et  = time.time()
         diff = _et - _st
 
         _sec = np.round(diff % 60, 2)
         _min = int(diff / 60)
 
         print(f"All program last {_min} minutes and {_sec} seconds.")
```

### Comparing `SpaGoG-0.21/spagog/experiments.py` & `SpaGoG-0.22/spagog/experiments.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 
 from pkg_resources import resource_filename
 
 PROJECT_DIR = "."
 
 
 def run_gc(
-        tab_dataset: TabDataset,
-        params: dict,
-        early_stopping: int = 30,
-        inter_sample_edges: torch.Tensor = None,
-        verbose: bool = True,
-        evaluate_metrics: bool = True,
-        probs: bool = False,
-        to_numpy: bool = True,
+    tab_dataset: TabDataset,
+    params: dict,
+    inter_sample_edges: torch.Tensor = None,
+    verbose: bool = True,
+    evaluate_metrics: bool = True,
+    probs: bool = False,
+    to_numpy: bool = True,
 ):
     graphs_dataset, *_ = GraphsDataset.from_tab(
         tab_data=tab_dataset,
         inter_sample_edges=inter_sample_edges,
         knn_kwargs={
             "distance": params.get("distance", "heur_dist"),
             "k": params.get("k", 3),
@@ -49,55 +48,58 @@
     model = GC(
         input_example=graphs_dataset,
         RECEIVED_PARAMS=RECEIVED_PARAMS,
         init_weights=params.get("init", "xavier_normal"),
         embedding_layer="first",
     )
 
+    early_stopping = params.get("early_stopping", 30)
+
     cache = model.fit(
         train_loader=train_loader,
         val_loader=val_loader,
         test_loader=test_loader,
         lr=params.get("lr", 0.01),
-        early_stopping_patience=early_stopping,
+        early_stopping=early_stopping,
         n_epochs=600,
         verbose=verbose,
         weight_decay=params.get("weight_decay", 0.001),
         dataset_name=tab_dataset.name,
     )
 
     y_test = model.predict(test_loader, probs=False, to_numpy=to_numpy)
 
     if evaluate_metrics and verbose == 1:
-        print(f"Test accuracy: {(test_loader.dataset.gdp.Y.flatten() == y_test).float().mean():.4f}")
+        print(
+            f"Test accuracy: {(test_loader.dataset.gdp.Y.flatten() == y_test).float().mean():.4f}"
+        )
 
     if probs:
         y_test = model.predict(test_loader, probs=True, to_numpy=to_numpy)
 
     return y_test, cache
 
 
 def run_gnc(
-        tab_dataset: TabDataset,
-        params: dict,
-        early_stopping: int = 30,
-        inter_sample_edges: torch.Tensor = None,
-        verbose: bool = True,
-        evaluate_metrics: bool = True,
-        probs: bool = False,
-        to_numpy: bool = True,
+    tab_dataset: TabDataset,
+    params: dict,
+    inter_sample_edges: torch.Tensor = None,
+    verbose: bool = True,
+    evaluate_metrics: bool = True,
+    probs: bool = False,
+    to_numpy: bool = True,
 ):
     graphs_dataset, inter_samples_edges, masks = GraphsDataset.from_tab(
         tab_data=tab_dataset,
         knn_kwargs={
             "distance": params.get("distance", "heur_dist"),
             "k": params.get("k", 30),
         },
         inter_sample_edges=inter_sample_edges,
-        calc_intra_edges=True
+        calc_intra_edges=True,
     )
 
     train_mask, val_mask, test_mask = masks
 
     nc_h_layers = [int(params["nc_layer_1"]), int(params["nc_layer_2"])]
     nc_dropouts = [float(params["nc_dropout_1"]), float(params["nc_dropout_2"])]
 
@@ -124,23 +126,28 @@
             "dropout": gc_params["dropout"],
         }
 
         gc_model = GC(
             input_example=graphs_dataset,
             RECEIVED_PARAMS=RECEIVED_PARAMS,
             init_weights=gc_params.get("init", "xavier_normal"),
-            embedding_layer=params["embedding_layer"]  # embedding_layer,
+            embedding_layer=params["embedding_layer"],  # embedding_layer,
         )
 
+        if "gc_early_stopping" in gc_params.keys():
+            gc_early_stopping = gc_params["gc_early_stopping"]
+        else:
+            gc_early_stopping = gc_params.get("early_stopping", 30)
+
         _ = gc_model.fit(
             train_loader=train_loader,
             val_loader=val_loader,
             test_loader=test_loader,
             lr=gc_params.get("lr", 0.01),
-            early_stopping_patience=30,
+            early_stopping=gc_early_stopping,
             n_epochs=600,
             verbose=verbose,
             weight_decay=gc_params.get("weight_decay", 0.001),
             dataset_name=tab_dataset.name,
         )
 
     else:
@@ -152,75 +159,88 @@
             "RECEIVED_PARAMS": {
                 "preweight": params["gc_preweight"],
                 "layer_1": params["gc_layer_1"],
                 "layer_2": params["gc_layer_2"],
                 "activation": params["gc_activation"],
                 "dropout": params["gc_dropout"],
             },
-            "embedding_layer": params["embedding_layer"]  # embedding_layer,
+            "embedding_layer": params["embedding_layer"],  # embedding_layer,
         },
         nc_kwargs={
             "h_layers": nc_h_layers,
             "dropouts": nc_dropouts,
             "activations": nc_activations,
         },
         gc_model=gc_model,
     )
 
+    early_stopping = params.get("early_stopping", 30)
+
     cache, all_graphs_loader = model.fit(
         graphs_dataset,
         inter_samples_edges,
         train_mask,
         val_mask,
         test_mask,
-        n_epochs=10000,
+        n_epochs=100,
         gc_lr=params["gc_lr"],
         nc_lr=params["nc_lr"],
         gc_weight_decay=params["gc_weight_decay"],
         nc_weight_decay=params["nc_weight_decay"],
         alpha=params["alpha"],
         batch_size=params.get("batch_size", 10),
-        early_stopping_patience=early_stopping,
+        early_stopping=early_stopping,
         verbose=verbose,
-        clf_from=params["clf_from"]  # clf_from
+        clf_from=params["clf_from"],  # clf_from
     )
 
-    y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"],
-                           probs=False,
-                           to_numpy=to_numpy)
+    y_test = model.predict(
+        all_graphs_loader,
+        inter_samples_edges.T,
+        test_mask,
+        clf_from=params["clf_from"],
+        probs=False,
+        to_numpy=to_numpy,
+    )
 
     if evaluate_metrics and verbose == 1:
-        print(f"Test accuracy: {(test_loader.dataset.gdp.Y.flatten() == y_test).float().mean():.4f}")
+        print(
+            f"Test accuracy: {(test_loader.dataset.gdp.Y.flatten() == y_test).float().mean():.4f}"
+        )
 
     if probs:
-        y_test = model.predict(all_graphs_loader, inter_samples_edges.T, test_mask, clf_from=params["clf_from"],
-                               probs=True,
-                               to_numpy=to_numpy)
+        y_test = model.predict(
+            all_graphs_loader,
+            inter_samples_edges.T,
+            test_mask,
+            clf_from=params["clf_from"],
+            probs=True,
+            to_numpy=to_numpy,
+        )
 
     return y_test, cache
 
 
 def run_gc_nc(
-        tab_dataset: TabDataset,
-        params: dict,
-        early_stopping: int = 30,
-        inter_sample_edges: torch.Tensor = None,
-        verbose: bool = True,
-        evaluate_metrics: bool = True,
-        probs: bool = False,
-        to_numpy: bool = True,
+    tab_dataset: TabDataset,
+    params: dict,
+    inter_sample_edges: torch.Tensor = None,
+    verbose: bool = True,
+    evaluate_metrics: bool = True,
+    probs: bool = False,
+    to_numpy: bool = True,
 ):
     graphs_dataset, inter_sample_edges, masks = GraphsDataset.from_tab(
         tab_data=tab_dataset,
         knn_kwargs={
             "distance": params.get("distance", "heur_dist"),
             "k": params.get("k", 30),
         },
         inter_sample_edges=inter_sample_edges,
-        calc_intra_edges=True
+        calc_intra_edges=True,
     )
 
     train_graphs_loader = graphs_dataset.train.to_loader(
         batch_size=params["batch_size"]
     )
 
     val_graphs_loader = graphs_dataset.val.to_loader(batch_size=params["batch_size"])
@@ -234,23 +254,25 @@
         "dropout": params["gc_dropout"],
     }
 
     gc_model = GC(
         input_example=graphs_dataset,
         RECEIVED_PARAMS=GC_RECEIVED_PARAMS,
         init_weights=params.get("init", "xavier_normal"),
-        embedding_layer=params["embedding_layer"]  # embedding_layer
+        embedding_layer=params["embedding_layer"],  # embedding_layer
     )
 
+    gc_early_stopping = params.get("gc_early_stopping", 30)
+
     _ = gc_model.fit(
         train_loader=train_graphs_loader,
         val_loader=val_graphs_loader,
         test_loader=test_graphs_loader,
         lr=params["gc_lr"],
-        early_stopping_patience=early_stopping,
+        early_stopping=gc_early_stopping,
         n_epochs=600,
         verbose=verbose,
         weight_decay=params.get("gc_weight_decay", 0),
         dataset_name=tab_dataset.name,
     )
 
     def extract_embeddings(graphs_loader):
@@ -323,21 +345,23 @@
     test_graph = [
         (
             (all_embeddings, inter_sample_edges.T, masks[2]),
             tab_dataset.test.Y,
         )
     ]
 
+    nc_early_stopping = params.get("nc_early_stopping", 30)
+
     cache = nc_model.fit(
         train_loader=train_graph,
         val_loader=val_graph,
         test_loader=test_graph,
         lr=params["nc_lr"],
         n_epochs=600,
-        early_stopping_patience=early_stopping,
+        early_stopping=nc_early_stopping,
         weight_decay=params.get("nc_weight_decay", 0),
         verbose=verbose,
         dataset_name=graphs_dataset.name.replace("graphs", "graph"),
         labels_from_loader=lambda x: x[0][1],
     )
 
     y_test = nc_model.predict(test_graph, probs=False, to_numpy=to_numpy)
@@ -353,27 +377,34 @@
 
 def get_default_params_file(model):
     abs_path = resource_filename(__name__, ".")
     return os.path.join(abs_path, f"default_params/{model}.json")
 
 
 def get_tab_data(
-        train_X: pd.DataFrame,
-        train_Y: pd.DataFrame,
-        test_X: pd.DataFrame,
-        test_Y: pd.DataFrame = None,
-        val_X: pd.DataFrame = None,
-        val_Y: pd.DataFrame = None,
-        name: str = "",
-        use_existence_cols: bool = True,
-        *args,
-        **kwargs
+    train_X: pd.DataFrame,
+    train_Y: pd.DataFrame,
+    test_X: pd.DataFrame,
+    test_Y: pd.DataFrame = None,
+    val_X: pd.DataFrame = None,
+    val_Y: pd.DataFrame = None,
+    name: str = "",
+    use_existence_cols: bool = True,
+    *args,
+    **kwargs,
 ):
-    tab_dataset = TabDataset.load(train_X=train_X, train_Y=train_Y, test_X=test_X, test_Y=test_Y, val_X=val_X,
-                                  val_Y=val_Y, name=name,
-                                  *args,
-                                  **kwargs)
+    tab_dataset = TabDataset.load(
+        train_X=train_X,
+        train_Y=train_Y,
+        test_X=test_X,
+        test_Y=test_Y,
+        val_X=val_X,
+        val_Y=val_Y,
+        name=name,
+        *args,
+        **kwargs,
+    )
 
     if use_existence_cols:
         tab_dataset.add_existence_cols()
 
     return tab_dataset
```

### Comparing `SpaGoG-0.21/spagog/data/load_data.py` & `SpaGoG-0.22/spagog/data/load_data.py`

 * *Files identical despite different names*

