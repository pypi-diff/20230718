# Comparing `tmp/MEGNetSparse-0.0.4.tar.gz` & `tmp/MEGNetSparse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGNetSparse-0.0.4.tar", last modified: Wed Jul  5 23:02:50 2023, max compression
+gzip compressed data, was "MEGNetSparse-0.0.5.tar", last modified: Tue Jul 18 21:31:54 2023, max compression
```

## Comparing `MEGNetSparse-0.0.4.tar` & `MEGNetSparse-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:51.332479 MEGNetSparse-0.0.4/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.4/.gitignore
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     1091 2023-07-05 16:12:03.000000 MEGNetSparse-0.0.4/LICENSE
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:50.894993 MEGNetSparse-0.0.4/MEGNetSparse/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      120 2023-07-03 18:52:42.000000 MEGNetSparse-0.0.4/MEGNetSparse/__init__.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5423 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.4/MEGNetSparse/dense2sparse.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3586 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.4/MEGNetSparse/eos.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5105 2023-06-03 16:16:46.000000 MEGNetSparse-0.0.4/MEGNetSparse/layers.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3015 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.4/MEGNetSparse/model.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     6891 2023-06-03 16:26:00.000000 MEGNetSparse-0.0.4/MEGNetSparse/struct2graph.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     7445 2023-07-05 23:01:46.000000 MEGNetSparse-0.0.4/MEGNetSparse/trainer.py
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      885 2023-06-18 16:37:50.000000 MEGNetSparse-0.0.4/MEGNetSparse/utils.py
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:51.035601 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/PKG-INFO
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      612 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/SOURCES.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        1 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/dependency_links.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       27 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/requires.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       13 2023-07-05 23:02:50.000000 MEGNetSparse-0.0.4/MEGNetSparse.egg-info/top_level.txt
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-05 23:02:51.332479 MEGNetSparse-0.0.4/PKG-INFO
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2536 2023-07-05 16:00:57.000000 MEGNetSparse-0.0.4/README.md
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:51.223103 MEGNetSparse-0.0.4/examples/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       19 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.4/examples/.gitignore
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      812 2023-06-05 21:35:25.000000 MEGNetSparse-0.0.4/examples/MoS2.cif
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      814 2022-09-29 08:35:52.000000 MEGNetSparse-0.0.4/examples/WSe2.cif
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    13944 2022-04-12 22:15:21.000000 MEGNetSparse-0.0.4/examples/descriptors.csv
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    15149 2023-07-03 19:04:43.000000 MEGNetSparse-0.0.4/examples/example.ipynb
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       82 2023-06-05 21:35:26.000000 MEGNetSparse-0.0.4/examples/initial_structures.csv
-drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-05 23:02:51.301227 MEGNetSparse-0.0.4/examples/pilot/
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)   148416 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.4/examples/pilot/data.pickle.gz
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    10925 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.4/examples/pilot/targets.csv.gz
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      437 2023-07-05 23:02:37.000000 MEGNetSparse-0.0.4/pyproject.toml
--rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-05 23:02:51.332479 MEGNetSparse-0.0.4/setup.cfg
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 21:31:54.423576 MEGNetSparse-0.0.5/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.5/.gitignore
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     1091 2023-07-05 16:12:03.000000 MEGNetSparse-0.0.5/LICENSE
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 21:31:53.917183 MEGNetSparse-0.0.5/MEGNetSparse/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      120 2023-07-03 18:52:42.000000 MEGNetSparse-0.0.5/MEGNetSparse/__init__.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5423 2023-07-05 18:52:27.000000 MEGNetSparse-0.0.5/MEGNetSparse/dense2sparse.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3586 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.5/MEGNetSparse/eos.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     5105 2023-06-03 16:16:46.000000 MEGNetSparse-0.0.5/MEGNetSparse/layers.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     1878 2023-07-13 07:21:34.000000 MEGNetSparse-0.0.5/MEGNetSparse/losses.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     3015 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.5/MEGNetSparse/model.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     6891 2023-06-03 16:26:00.000000 MEGNetSparse-0.0.5/MEGNetSparse/struct2graph.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     8040 2023-07-18 20:38:26.000000 MEGNetSparse-0.0.5/MEGNetSparse/trainer.py
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      885 2023-06-18 16:37:50.000000 MEGNetSparse-0.0.5/MEGNetSparse/utils.py
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 21:31:54.057807 MEGNetSparse-0.0.5/MEGNetSparse.egg-info/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-18 21:31:53.000000 MEGNetSparse-0.0.5/MEGNetSparse.egg-info/PKG-INFO
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      635 2023-07-18 21:31:53.000000 MEGNetSparse-0.0.5/MEGNetSparse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        1 2023-07-18 21:31:53.000000 MEGNetSparse-0.0.5/MEGNetSparse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       27 2023-07-18 21:31:53.000000 MEGNetSparse-0.0.5/MEGNetSparse.egg-info/requires.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       13 2023-07-18 21:31:53.000000 MEGNetSparse-0.0.5/MEGNetSparse.egg-info/top_level.txt
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2698 2023-07-18 21:31:54.407941 MEGNetSparse-0.0.5/PKG-INFO
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)     2536 2023-07-05 16:00:57.000000 MEGNetSparse-0.0.5/README.md
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 21:31:54.282949 MEGNetSparse-0.0.5/examples/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       19 2023-06-21 13:21:55.000000 MEGNetSparse-0.0.5/examples/.gitignore
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      812 2023-06-05 21:35:25.000000 MEGNetSparse-0.0.5/examples/MoS2.cif
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      814 2022-09-29 08:35:52.000000 MEGNetSparse-0.0.5/examples/WSe2.cif
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    13944 2022-04-12 22:15:21.000000 MEGNetSparse-0.0.5/examples/descriptors.csv
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    15149 2023-07-03 19:04:43.000000 MEGNetSparse-0.0.5/examples/example.ipynb
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       82 2023-06-05 21:35:26.000000 MEGNetSparse-0.0.5/examples/initial_structures.csv
+drwxrwxrwx   0 qwerty    (1000) qwerty    (1000)        0 2023-07-18 21:31:54.376695 MEGNetSparse-0.0.5/examples/pilot/
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)   148416 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.5/examples/pilot/data.pickle.gz
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)    10925 2023-06-05 22:44:44.000000 MEGNetSparse-0.0.5/examples/pilot/targets.csv.gz
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)      437 2023-07-18 21:30:40.000000 MEGNetSparse-0.0.5/pyproject.toml
+-rwxrwxrwx   0 qwerty    (1000) qwerty    (1000)       38 2023-07-18 21:31:54.423576 MEGNetSparse-0.0.5/setup.cfg
```

### Comparing `MEGNetSparse-0.0.4/LICENSE` & `MEGNetSparse-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/MEGNetSparse/dense2sparse.py` & `MEGNetSparse-0.0.5/MEGNetSparse/dense2sparse.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/MEGNetSparse/eos.py` & `MEGNetSparse-0.0.5/MEGNetSparse/eos.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/MEGNetSparse/layers.py` & `MEGNetSparse-0.0.5/MEGNetSparse/layers.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/MEGNetSparse/model.py` & `MEGNetSparse-0.0.5/MEGNetSparse/model.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/MEGNetSparse/struct2graph.py` & `MEGNetSparse-0.0.5/MEGNetSparse/struct2graph.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/MEGNetSparse/trainer.py` & `MEGNetSparse-0.0.5/MEGNetSparse/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import numpy as np
 import torch
 from joblib import Parallel, delayed
 from tqdm import tqdm
 from torch_geometric.loader import DataLoader
 import torch.nn.functional as F
+from torch.utils.data import WeightedRandomSampler
 
 from .model import MEGNet
 from .utils import Scaler
 from .struct2graph import FlattenGaussianDistanceConverter, GaussianDistanceConverter, AtomFeaturesExtractor, \
     SimpleCrystalConverter
+from .losses import MSELoss, MAELoss
 
 
 def set_attr(structure, attr, name):
     setattr(structure, name, attr)
     return structure
 
 
@@ -72,31 +74,40 @@
     def prepare_data(
             self,
             train_data,
             train_targets,
             test_data,
             test_targets,
             target_name,
+            train_weights=None,
+            test_weights=None,
     ):
         print('adding targets to data')
         train_data = [set_attr(s, y, 'y') for s, y in zip(train_data, train_targets)]
         test_data = [set_attr(s, y, 'y') for s, y in zip(test_data, test_targets)]
 
+        if test_weights is not None:
+            test_data = [set_attr(s, w, 'weight') for s, w in zip(test_data, test_weights)]
+
         print("converting data")
         self.train_structures = Parallel(n_jobs=-1)(
             delayed(self.converter.convert)(s) for s in tqdm(train_data))
         self.test_structures = Parallel(n_jobs=-1)(
             delayed(self.converter.convert)(s) for s in tqdm(test_data))
         self.scaler.fit(self.train_structures)
 
+        if train_weights is not None:
+            self.sampler = WeightedRandomSampler(torch.tensor(train_weights).float(), len(train_weights))
+
         self.trainloader = DataLoader(
             self.train_structures,
             batch_size=self.config["model"]["train_batch_size"],
             shuffle=True,
             num_workers=0,
+            sampler=self.sampler if train_weights is not None else None
         )
 
         self.testloader = DataLoader(
             self.test_structures,
             batch_size=self.config["model"]["test_batch_size"],
             shuffle=False,
             num_workers=0
@@ -125,17 +136,18 @@
             loss.backward()
 
             self.optimizer.step()
             self.optimizer.zero_grad()
 
             mses.append(loss.to("cpu").data.numpy())
             maes.append(
-                F.l1_loss(
+                MAELoss(
                     self.scaler.inverse_transform(preds),
                     batch.y,
+                    weights=batch.weight,
                     reduction='sum'
                 ).to('cpu').data.numpy()
             )
 
         train_mae = sum(maes) / len(self.train_structures)
         self.scheduler.step(train_mae)
         train_mse = np.mean(mses)
@@ -151,17 +163,18 @@
                 batch = batch.to(self.device)
 
                 preds = self.model(
                     batch.x, batch.edge_index, batch.edge_attr, batch.state, batch.batch, batch.bond_batch
                 ).squeeze()
 
                 total.append(
-                    F.l1_loss(
+                    MAELoss(
                         self.scaler.inverse_transform(preds),
                         batch.y,
+                        weights=batch.weight,
                         reduction='sum'
                     ).to('cpu').data.numpy()
                 )
                 results.append(self.scaler.inverse_transform(preds))
 
             cur_test_loss = sum(total) / len(self.test_structures)
```

### Comparing `MEGNetSparse-0.0.4/MEGNetSparse/utils.py` & `MEGNetSparse-0.0.5/MEGNetSparse/utils.py`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/MEGNetSparse.egg-info/PKG-INFO` & `MEGNetSparse-0.0.5/MEGNetSparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGNetSparse
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Romanov Ignat <romanov.ignat.p@gmail.com>
 Project-URL: Homepage, https://github.com/RomanovIgnat/MEGNet_pytorch_test
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MEGNetSparse
```

### Comparing `MEGNetSparse-0.0.4/MEGNetSparse.egg-info/SOURCES.txt` & `MEGNetSparse-0.0.5/MEGNetSparse.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 README.md
 pyproject.toml
 MEGNetSparse/__init__.py
 MEGNetSparse/dense2sparse.py
 MEGNetSparse/eos.py
 MEGNetSparse/layers.py
+MEGNetSparse/losses.py
 MEGNetSparse/model.py
 MEGNetSparse/struct2graph.py
 MEGNetSparse/trainer.py
 MEGNetSparse/utils.py
 MEGNetSparse.egg-info/PKG-INFO
 MEGNetSparse.egg-info/SOURCES.txt
 MEGNetSparse.egg-info/dependency_links.txt
```

### Comparing `MEGNetSparse-0.0.4/PKG-INFO` & `MEGNetSparse-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGNetSparse
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Romanov Ignat <romanov.ignat.p@gmail.com>
 Project-URL: Homepage, https://github.com/RomanovIgnat/MEGNet_pytorch_test
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MEGNetSparse
```

### Comparing `MEGNetSparse-0.0.4/README.md` & `MEGNetSparse-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/examples/MoS2.cif` & `MEGNetSparse-0.0.5/examples/MoS2.cif`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/examples/WSe2.cif` & `MEGNetSparse-0.0.5/examples/WSe2.cif`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/examples/descriptors.csv` & `MEGNetSparse-0.0.5/examples/descriptors.csv`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/examples/example.ipynb` & `MEGNetSparse-0.0.5/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/examples/pilot/data.pickle.gz` & `MEGNetSparse-0.0.5/examples/pilot/data.pickle.gz`

 * *Files identical despite different names*

### Comparing `MEGNetSparse-0.0.4/examples/pilot/targets.csv.gz` & `MEGNetSparse-0.0.5/examples/pilot/targets.csv.gz`

 * *Files identical despite different names*

