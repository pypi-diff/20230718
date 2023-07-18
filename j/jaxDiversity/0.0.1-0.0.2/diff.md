# Comparing `tmp/jaxDiversity-0.0.1.tar.gz` & `tmp/jaxDiversity-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxDiversity-0.0.1.tar", last modified: Tue Jul 18 02:43:29 2023, max compression
+gzip compressed data, was "jaxDiversity-0.0.2.tar", last modified: Tue Jul 18 18:44:53 2023, max compression
```

## Comparing `jaxDiversity-0.0.1.tar` & `jaxDiversity-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 aradhak5 (319685) kvm        (108)        0 2023-07-18 02:43:29.085648 jaxDiversity-0.0.1/
--rw-rw-r--   0 aradhak5 (319685) kvm        (108)    11337 2023-04-27 10:12:58.000000 jaxDiversity-0.0.1/LICENSE
--rw-rw-r--   0 aradhak5 (319685) kvm        (108)      111 2023-04-27 10:12:58.000000 jaxDiversity-0.0.1/MANIFEST.in
--rw-r--r--   0 aradhak5 (319685) kvm        (108)     1007 2023-07-18 02:43:29.085648 jaxDiversity-0.0.1/PKG-INFO
--rw-r--r--   0 aradhak5 (319685) kvm        (108)      309 2023-07-18 01:01:07.000000 jaxDiversity-0.0.1/README.md
-drwxr-xr-x   0 aradhak5 (319685) kvm        (108)        0 2023-07-18 02:43:29.085648 jaxDiversity-0.0.1/jaxDiversity/
--rw-r--r--   0 aradhak5 (319685) kvm        (108)       22 2023-07-18 02:25:55.000000 jaxDiversity-0.0.1/jaxDiversity/__init__.py
--rw-r--r--   0 aradhak5 (319685) kvm        (108)     8793 2023-07-18 02:25:55.000000 jaxDiversity-0.0.1/jaxDiversity/_modidx.py
--rw-r--r--   0 aradhak5 (319685) kvm        (108)      503 2023-07-18 02:25:55.000000 jaxDiversity-0.0.1/jaxDiversity/baseline.py
--rw-r--r--   0 aradhak5 (319685) kvm        (108)      146 2023-07-18 02:25:55.000000 jaxDiversity-0.0.1/jaxDiversity/core.py
--rw-r--r--   0 aradhak5 (319685) kvm        (108)     4923 2023-07-18 02:25:55.000000 jaxDiversity-0.0.1/jaxDiversity/dataloading.py
--rw-r--r--   0 aradhak5 (319685) kvm        (108)     1218 2023-07-18 02:25:55.000000 jaxDiversity-0.0.1/jaxDiversity/hnn.py
--rw-r--r--   0 aradhak5 (319685) kvm        (108)     7401 2023-07-18 02:25:55.000000 jaxDiversity-0.0.1/jaxDiversity/loops.py
--rw-r--r--   0 aradhak5 (319685) kvm        (108)     4932 2023-07-18 02:25:55.000000 jaxDiversity-0.0.1/jaxDiversity/mlp.py
--rw-r--r--   0 aradhak5 (319685) kvm        (108)     1163 2023-07-18 02:25:55.000000 jaxDiversity-0.0.1/jaxDiversity/utilclasses.py
-drwxr-xr-x   0 aradhak5 (319685) kvm        (108)        0 2023-07-18 02:43:29.085648 jaxDiversity-0.0.1/jaxDiversity.egg-info/
--rw-r--r--   0 aradhak5 (319685) kvm        (108)     1007 2023-07-18 02:43:29.000000 jaxDiversity-0.0.1/jaxDiversity.egg-info/PKG-INFO
--rw-r--r--   0 aradhak5 (319685) kvm        (108)      517 2023-07-18 02:43:29.000000 jaxDiversity-0.0.1/jaxDiversity.egg-info/SOURCES.txt
--rw-r--r--   0 aradhak5 (319685) kvm        (108)        1 2023-07-18 02:43:29.000000 jaxDiversity-0.0.1/jaxDiversity.egg-info/dependency_links.txt
--rw-r--r--   0 aradhak5 (319685) kvm        (108)       46 2023-07-18 02:43:29.000000 jaxDiversity-0.0.1/jaxDiversity.egg-info/entry_points.txt
--rw-r--r--   0 aradhak5 (319685) kvm        (108)        1 2023-07-18 01:34:16.000000 jaxDiversity-0.0.1/jaxDiversity.egg-info/not-zip-safe
--rw-r--r--   0 aradhak5 (319685) kvm        (108)       78 2023-07-18 02:43:29.000000 jaxDiversity-0.0.1/jaxDiversity.egg-info/requires.txt
--rw-r--r--   0 aradhak5 (319685) kvm        (108)       13 2023-07-18 02:43:29.000000 jaxDiversity-0.0.1/jaxDiversity.egg-info/top_level.txt
--rw-r--r--   0 aradhak5 (319685) kvm        (108)     1118 2023-07-18 02:25:32.000000 jaxDiversity-0.0.1/settings.ini
--rw-r--r--   0 aradhak5 (319685) kvm        (108)       38 2023-07-18 02:43:29.085648 jaxDiversity-0.0.1/setup.cfg
--rw-rw-r--   0 aradhak5 (319685) kvm        (108)     2596 2023-04-27 10:12:58.000000 jaxDiversity-0.0.1/setup.py
+drwxr-xr-x   0 aradhak5 (319685) kvm        (108)        0 2023-07-18 18:44:53.620439 jaxDiversity-0.0.2/
+-rw-rw-r--   0 aradhak5 (319685) kvm        (108)    11337 2023-04-27 10:12:58.000000 jaxDiversity-0.0.2/LICENSE
+-rw-rw-r--   0 aradhak5 (319685) kvm        (108)      111 2023-04-27 10:12:58.000000 jaxDiversity-0.0.2/MANIFEST.in
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     6342 2023-07-18 18:44:53.620439 jaxDiversity-0.0.2/PKG-INFO
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     5611 2023-07-18 15:41:36.000000 jaxDiversity-0.0.2/README.md
+drwxr-xr-x   0 aradhak5 (319685) kvm        (108)        0 2023-07-18 18:44:53.616439 jaxDiversity-0.0.2/jaxDiversity/
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)       22 2023-07-18 18:44:17.000000 jaxDiversity-0.0.2/jaxDiversity/__init__.py
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     8690 2023-07-18 18:44:17.000000 jaxDiversity-0.0.2/jaxDiversity/_modidx.py
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)      501 2023-07-18 18:44:17.000000 jaxDiversity-0.0.2/jaxDiversity/baseline.py
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     4792 2023-07-18 18:44:17.000000 jaxDiversity-0.0.2/jaxDiversity/dataloading.py
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     1212 2023-07-18 18:44:17.000000 jaxDiversity-0.0.2/jaxDiversity/hnn.py
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     7097 2023-07-18 18:44:17.000000 jaxDiversity-0.0.2/jaxDiversity/loops.py
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     4877 2023-07-18 18:44:17.000000 jaxDiversity-0.0.2/jaxDiversity/mlp.py
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     1164 2023-07-18 18:44:17.000000 jaxDiversity-0.0.2/jaxDiversity/utilclasses.py
+drwxr-xr-x   0 aradhak5 (319685) kvm        (108)        0 2023-07-18 18:44:53.620439 jaxDiversity-0.0.2/jaxDiversity.egg-info/
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     6342 2023-07-18 18:44:53.000000 jaxDiversity-0.0.2/jaxDiversity.egg-info/PKG-INFO
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)      496 2023-07-18 18:44:53.000000 jaxDiversity-0.0.2/jaxDiversity.egg-info/SOURCES.txt
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)        1 2023-07-18 18:44:53.000000 jaxDiversity-0.0.2/jaxDiversity.egg-info/dependency_links.txt
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)      103 2023-07-18 18:44:53.000000 jaxDiversity-0.0.2/jaxDiversity.egg-info/entry_points.txt
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)        1 2023-07-18 01:34:16.000000 jaxDiversity-0.0.2/jaxDiversity.egg-info/not-zip-safe
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)       84 2023-07-18 18:44:53.000000 jaxDiversity-0.0.2/jaxDiversity.egg-info/requires.txt
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)       13 2023-07-18 18:44:53.000000 jaxDiversity-0.0.2/jaxDiversity.egg-info/top_level.txt
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)     1069 2023-07-18 18:44:17.000000 jaxDiversity-0.0.2/settings.ini
+-rw-r--r--   0 aradhak5 (319685) kvm        (108)       38 2023-07-18 18:44:53.620439 jaxDiversity-0.0.2/setup.cfg
+-rw-rw-r--   0 aradhak5 (319685) kvm        (108)     2596 2023-04-27 10:12:58.000000 jaxDiversity-0.0.2/setup.py
```

### Comparing `jaxDiversity-0.0.1/LICENSE` & `jaxDiversity-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxDiversity-0.0.1/jaxDiversity/_modidx.py` & `jaxDiversity-0.0.2/jaxDiversity/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/jaxDiversity',
                 'doc_host': 'https://NonlinearArtificialIntelligenceLabs.github.io',
                 'git_url': 'https://github.com/NonlinearArtificialIntelligenceLab/jaxDiversity',
                 'lib_path': 'jaxDiversity'},
   'syms': { 'jaxDiversity.baseline': {'jaxDiversity.baseline.compute_loss': ('baseline.html#compute_loss', 'jaxDiversity/baseline.py')},
-            'jaxDiversity.core': {'jaxDiversity.core.foo': ('core.html#foo', 'jaxDiversity/core.py')},
             'jaxDiversity.dataloading': { 'jaxDiversity.dataloading.DummyDataset': ( 'dataloading.html#dummydataset',
                                                                                      'jaxDiversity/dataloading.py'),
                                           'jaxDiversity.dataloading.DummyDataset.__getitem__': ( 'dataloading.html#dummydataset.__getitem__',
                                                                                                  'jaxDiversity/dataloading.py'),
                                           'jaxDiversity.dataloading.DummyDataset.__init__': ( 'dataloading.html#dummydataset.__init__',
                                                                                               'jaxDiversity/dataloading.py'),
                                           'jaxDiversity.dataloading.DummyDataset.__len__': ( 'dataloading.html#dummydataset.__len__',
```

### Comparing `jaxDiversity-0.0.1/jaxDiversity/dataloading.py` & `jaxDiversity-0.0.2/jaxDiversity/dataloading.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,155 +13,131 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 # %% ../nbs/01_dataloading.ipynb 7
 # create a dummy dataset for testing
 class DummyDataset(Dataset):
-    """Dummy dataset for testing"""
-
-    def __init__(
-        self,
-        n_samples=100,  # number of samples
-        n_features=5,  # number of features
-        n_targets=1,  # number of targets
-        seed=42,  # random seed
-    ):
+    """ Dummy dataset for testing"""
+    def __init__(self, n_samples=100, # number of samples
+                 n_features=5, # number of features
+                 n_targets=1, # number of targets
+                 seed=42 # random seed
+                 ):
         self.n_samples = n_samples
         self.n_features = n_features
         self.n_targets = n_targets
         self.seed = seed
         self.x = jnp.array(np.random.rand(n_samples, n_features))
         self.y = jnp.array(np.random.rand(n_samples, n_targets))
-
+    
     def __len__(self):
         return self.n_samples
-
+    
     def __getitem__(self, idx):
         return self.x[idx], self.y[idx]
 
 # %% ../nbs/01_dataloading.ipynb 8
 def numpy_collate(batch):
-    if isinstance(batch[0], np.ndarray):
-        return np.stack(batch)
-    elif isinstance(batch[0], (tuple, list)):
-        transposed = zip(*batch)
-        return [numpy_collate(samples) for samples in transposed]
-    else:
-        return np.array(batch)
-
+  if isinstance(batch[0], np.ndarray):
+    return np.stack(batch)
+  elif isinstance(batch[0], (tuple,list)):
+    transposed = zip(*batch)
+    return [numpy_collate(samples) for samples in transposed]
+  else:
+    return np.array(batch)
 
 class NumpyLoader(DataLoader):
-    """A dataloader that uses numpy_collate
-    to allow numpy arrays instead of torch tensors"""
-
-    def __init__(
-        self,
-        dataset,
-        batch_size=1,
-        shuffle=False,
-        sampler=None,
-        batch_sampler=None,
-        num_workers=0,
-        pin_memory=False,
-        drop_last=False,
-        timeout=0,
-        worker_init_fn=None,
-    ):
-        super(self.__class__, self).__init__(
-            dataset,
-            batch_size=batch_size,
-            shuffle=shuffle,
-            sampler=sampler,
-            batch_sampler=batch_sampler,
-            num_workers=num_workers,
-            collate_fn=numpy_collate,
-            pin_memory=pin_memory,
-            drop_last=drop_last,
-            timeout=timeout,
-            worker_init_fn=worker_init_fn,
-        )
+  """ A dataloader that uses numpy_collate 
+  to allow numpy arrays instead of torch tensors"""
+  def __init__(self, dataset, batch_size=1,
+                shuffle=False, sampler=None,
+                batch_sampler=None, num_workers=0,
+                pin_memory=False, drop_last=False,
+                timeout=0, worker_init_fn=None):
+    super(self.__class__, self).__init__(dataset,
+        batch_size=batch_size,
+        shuffle=shuffle,
+        sampler=sampler,
+        batch_sampler=batch_sampler,
+        num_workers=num_workers,
+        collate_fn=numpy_collate,
+        pin_memory=pin_memory,
+        drop_last=drop_last,
+        timeout=timeout,
+        worker_init_fn=worker_init_fn)
 
 # %% ../nbs/01_dataloading.ipynb 13
 class RealPendulumDataset(Dataset):
-    def __init__(
-        self,
-        root_path: str,  # path to data
-        train_split: float,  # fraction of data to use for training
-        train: bool = True,  # whether to use train or test data
-    ):
+    
+    def __init__(self, root_path: str, # path to data
+                 train_split: float, # fraction of data to use for training
+                 train: bool =True # whether to use train or test data
+                 ):
         self.root_path = root_path
-        self.headers = ["time", "theta", "theta_dot", "theta_ddot"]
-        data = np.loadtxt(root_path + "extracted_angles.csv", delimiter=",")
+        self.headers = ['time', 'theta', 'theta_dot', 'theta_ddot']
+        data = np.loadtxt(root_path+ "extracted_angles.csv", delimiter=',')
 
         if train:
-            data = data[: int(train_split * len(data))]
+            data = data[:int(train_split*len(data))]
         else:
-            data = data[int(train_split * len(data)) :]
+            data = data[int(train_split*len(data)):]
 
         # separate x(theta, theta_dot) and y(theta_dot, theta_ddot)
-        self.x = data[:, 1:3]
-        self.y = data[:, 2:]
-
+        self.x = data[:,1:3]
+        self.y = data[:,2:]
+    
     def __len__(self):
         return len(self.y)
-
-    def __getitem__(self, idx):
+    
+    def __getitem__(self,idx):
         return jnp.array(self.x[idx]), jnp.array(self.y[idx])
+       
 
 # %% ../nbs/01_dataloading.ipynb 19
 class HHDataset(Dataset):
-    def __init__(
-        self, root_path, train  # path to data  # whether to use train or test data
-    ):
+    def __init__(self, root_path, # path to data
+                 train # whether to use train or test data
+                 ):
         if train:
-            self.path = root_path + "train/train.csv"
+            self.path =  root_path + "train/train.csv"
         else:
-            self.path = root_path + "valid/valid.csv"
-
-        data = np.loadtxt(self.path, delimiter=",", skiprows=1)
+            self.path =  root_path + "valid/valid.csv"
+        
+        data = np.loadtxt(self.path, delimiter=',', skiprows=1)
         # make a dictionary with keys "x" and "y" with x being q1, q2, p1, p2 and y being dq1, dq2, dp1, dp2
 
         data = {"x": data[:, :4], "y": data[:, 5:]}
         self.x = data["x"][::400]
         self.y = data["y"][::400]
-
+    
     def __len__(self):
         return len(self.y)
-
-    def __getitem__(self, idx):
+    
+    def __getitem__(self,idx):
         return jnp.array(self.x[idx]), jnp.array(self.y[idx])
 
 # %% ../nbs/01_dataloading.ipynb 26
 class SwingingSticksDataset(Dataset):
-    def __init__(
-        self,
-        root_path,  # path to data
-        train_split,  # fraction of data to use for training
-        train=True,  # whether to use train or test data
-    ):
+    def __init__(self, root_path, # path to data
+                 train_split, # fraction of data to use for training
+                 train=True # whether to use train or test data
+                 ):
         self.root_path = root_path
-        self.headers = [
-            "time",
-            "theta_a",
-            "theta_A",
-            "theta_a_dot",
-            "theta_A_dot",
-            "theta_a_ddot",
-            "theta_A_ddot",
-        ]
-        data = np.loadtxt(root_path + "SSData.txt", delimiter="\t")
+        self.headers = ['time', 'theta_a','theta_A', 'theta_a_dot', 'theta_A_dot', 'theta_a_ddot', 'theta_A_ddot']
+        data = np.loadtxt(root_path + "SSData.txt", delimiter='\t')
+
 
         if train:
-            data = data[: int(train_split * len(data))]
+            data = data[:int(train_split*len(data))]
         else:
-            data = data[int(train_split * len(data)) :]
+            data = data[int(train_split*len(data)):]
 
         # separate x and y
-        self.x = data[:, 1:5]
-        self.y = data[:, 3:]
-
+        self.x = data[:,1:5]
+        self.y = data[:,3:]
+    
     def __len__(self):
         return len(self.y)
-
-    def __getitem__(self, idx):
+    
+    def __getitem__(self,idx):
         return jnp.array(self.x[idx]), jnp.array(self.y[idx])
```

### Comparing `jaxDiversity-0.0.1/jaxDiversity/hnn.py` & `jaxDiversity-0.0.2/jaxDiversity/hnn.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 __all__ = ['hamiltonian_factory', 'compute_loss']
 
 # %% ../nbs/05_HNN.ipynb 4
 import jax
 import jax.numpy as jnp
 import equinox as eqx
 
+
 # %% ../nbs/05_HNN.ipynb 5
 from .mlp import MultiActMLP, deterministic_init, init_linear_weight
 
 # %% ../nbs/05_HNN.ipynb 6
 def hamiltonian_factory(model, afuncs):
     """Returns a function that computes the Hamiltonian of a given model."""
-
-    def hamiltonian(q, p):
+    def hamiltonian(q,p):
         """Hamiltonian taking in q and p as 1D arrays."""
         q = q.reshape((1, -1))
         p = p.reshape((1, -1))
         x = jnp.concatenate([q, p], axis=None)
         return model(x, afuncs)[0].reshape(())
-
     return hamiltonian
 
 # %% ../nbs/05_HNN.ipynb 7
 @eqx.filter_value_and_grad()
 def compute_loss(model, x, y, afuncs):
     """Computes hamilton's equations to get dqdp and then computes the loss"""
     hamiltonian = hamiltonian_factory(model, afuncs)
     q, p = jnp.split(x, 2, axis=1)
-    dHdq = jax.vmap(jax.grad(hamiltonian, argnums=0))(q, p)
+    dHdq= jax.vmap(jax.grad(hamiltonian, argnums=0))(q, p)
     dHdp = jax.vmap(jax.grad(hamiltonian, argnums=1))(q, p)
-    dqdp = jnp.concatenate([dHdp, -dHdq], axis=1)  # pred_y
-    loss = jnp.mean((dqdp - y) ** 2)
+    dqdp = jnp.concatenate([dHdp, -dHdq], axis=1) # pred_y
+    loss = jnp.mean((dqdp - y)**2)
 
     return loss
```

### Comparing `jaxDiversity-0.0.1/jaxDiversity/loops.py` & `jaxDiversity-0.0.2/jaxDiversity/loops.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,139 +13,102 @@
 import logging
 from tqdm.notebook import trange
 import pickle
 from functools import partial
 import json
 from dataclasses import asdict
 
+
 # %% ../nbs/06_Loops.ipynb 5
 from .dataloading import NumpyLoader, DummyDataset
-from jaxDiversity.utilclasses import (
-    InnerConfig,
-    OuterConfig,
-    InnerResults,
-    OuterResults,
-)
-from jaxDiversity.mlp import (
-    mlp_afunc,
-    MultiActMLP,
-    init_linear_weight,
-    xavier_normal_init,
-    save,
-)
+from .utilclasses import InnerConfig, OuterConfig, InnerResults, OuterResults
+from .mlp import mlp_afunc, MultiActMLP, init_linear_weight, xavier_normal_init, save
 from .baseline import compute_loss as compute_loss_baseline
 from .hnn import compute_loss as compute_loss_hnn
 
+
 # %% ../nbs/06_Loops.ipynb 7
 @eqx.filter_jit
 def make_step(model, x, y, afuncs, optim, opt_state, compute_loss):
     loss, grads = compute_loss(model, x, y, afuncs)
     updates, opt_state = optim.update(grads, opt_state)
     model = eqx.apply_updates(model, updates)
     return loss, grads, model, opt_state
 
 # %% ../nbs/06_Loops.ipynb 8
-def inner_opt(
-    model,
-    train_data,
-    test_data,
-    afuncs,
-    opt,
-    loss_fn,
-    config,
-    training=False,
-    verbose=False,
-):
+def inner_opt(model, train_data, test_data, afuncs, opt, loss_fn, config, training=False, verbose=False):
     """
     inner optimization loop
     """
     train_loss = []
     test_loss = []
     grad_norm = []
 
     opt_state = opt.init(model)
     for epoch in range(config.epochs):
         if training:
-            for x, y in train_data:
-                loss, grads, model, opt_state = make_step(
-                    model, x, y, afuncs, opt, opt_state, loss_fn
-                )
+            for x,y in train_data:
+                loss, grads, model, opt_state = make_step(model, x, y, afuncs, opt, opt_state, loss_fn)
                 train_loss.append(loss)
                 grad_norm_tree = jax.tree_map(lambda x: jnp.linalg.norm(x), grads)
                 grad_norm_scalar = jax.tree_util.tree_reduce(jnp.add, grad_norm_tree)
                 grad_norm.append(grad_norm_scalar)
-
-        for x, y in test_data:
+        
+        for x,y in test_data:
             x = jax.lax.stop_gradient(x)
             y = jax.lax.stop_gradient(y)
             loss, _ = loss_fn(model, x, y, afuncs)
             test_loss.append(loss)
         if verbose:
-            logging.info(
-                f"Epoch {epoch :03d} | Train Loss: {train_loss[-1] :.4e} | Test Loss: {test_loss[-1]:.4e} | Grad Norm: {grad_norm[-1]:.4e}"
-            )
-
-    return (
-        model,
-        opt_state,
-        InnerResults(jnp.array(train_loss), jnp.array(test_loss), jnp.array(grad_norm)),
-    )
+            logging.info(f"Epoch {epoch :03d} | Train Loss: {train_loss[-1] :.4e} | Test Loss: {test_loss[-1]:.4e} | Grad Norm: {grad_norm[-1]:.4e}")
+
+    return model, opt_state, InnerResults(jnp.array(train_loss), jnp.array(test_loss), jnp.array(grad_norm))
 
 # %% ../nbs/06_Loops.ipynb 11
 @eqx.filter_value_and_grad()
 def outer_loss(outer_models, inner_model, x, y, loss_fn, base_act):
-    inner_afuncs = [
-        partial(mlp_afunc, model=outer_model, base_act=base_act)
-        for outer_model in outer_models
-    ]
+    inner_afuncs = [ partial(mlp_afunc, model = outer_model, base_act = base_act) for outer_model in outer_models]
     loss, _ = loss_fn(inner_model, x, y, inner_afuncs)
     return loss
 
+
 # %% ../nbs/06_Loops.ipynb 12
 @eqx.filter_jit
-def outer_step(
-    outer_models, inner_model, x, y, meta_opt, meta_opt_state, loss_fn, base_act
-):
+def outer_step(outer_models, inner_model, x, y, meta_opt, meta_opt_state, loss_fn, base_act):
     loss, grads = outer_loss(outer_models, inner_model, x, y, loss_fn, base_act)
     updates, opt_state = meta_opt.update(grads, meta_opt_state)
     model = eqx.apply_updates(outer_models, updates)
     return loss, grads, model, opt_state
 
 # %% ../nbs/06_Loops.ipynb 13
-def outer_opt(
-    train_dataloader,
-    test_dataloader,
-    loss_fn,
-    inner_config,
-    outer_config,
-    opt,
-    meta_opt,
-    save_path=None,
-):
+def outer_opt(train_dataloader, test_dataloader, loss_fn, inner_config, outer_config, opt, meta_opt, save_path=None):
     """
     outer optimization loop
     """
     outer_model_key = jax.random.PRNGKey(outer_config.seed)
     inner_model_key = jax.random.PRNGKey(inner_config.seed)
 
     outer_models = []
     for _ in range(inner_config.n_fns):
-        model = eqx.nn.MLP(
-            in_size=outer_config.input_dim,
-            out_size=outer_config.output_dim,
-            width_size=outer_config.hidden_layer_sizes[0],
-            depth=1,
-            key=outer_model_key,
-            use_bias=True,
-        )
+        model = eqx.nn.MLP(in_size=outer_config.input_dim,
+                        out_size=outer_config.output_dim,
+                        width_size=outer_config.hidden_layer_sizes[0],
+                        depth=1,
+                        key=outer_model_key,
+                        use_bias=True)
         outer_models.append(model)
 
     meta_opt_states = meta_opt.init(eqx.filter(outer_models, eqx.is_array))
 
-    results = {"train_loss": [], "test_loss": [], "inner_afuncs": [], "grad_norms": []}
+    results = {
+        "train_loss": [],
+        "test_loss": [],
+        "inner_afuncs": [],
+        "grad_norms": []
+    }
 
     inner_afuncs = []
 
     if inner_config.base_act == "sin":
         base_act = jnp.sin
     elif inner_config.base_act == "relu":
         base_act = jnp.relu
@@ -155,91 +118,64 @@
     if save_path is not None:
         # save config files
         with open(f"{save_path}/inner_config.json", "w") as f:
             json.dump(asdict(inner_config), f)
         with open(f"{save_path}/outer_config.json", "w") as f:
             json.dump(asdict(outer_config), f)
 
+
     for step in trange(outer_config.steps):
-        inner_afuncs = [
-            partial(mlp_afunc, model=outer_model, base_act=base_act)
-            for outer_model in outer_models
-        ]
-
-        inner_model = MultiActMLP(
-            inner_config.input_dim,
-            inner_config.output_dim,
-            inner_config.hidden_layer_sizes,
-            inner_model_key,
-            bias=True,
-        )
-
-        inner_model = init_linear_weight(
-            inner_model, xavier_normal_init, inner_model_key
-        )
-
-        inner_model, _, inner_results = inner_opt(
-            inner_model,
-            train_dataloader,
-            test_dataloader,
-            inner_afuncs,
-            opt,
-            loss_fn,
-            inner_config,
-            training=True,
-            verbose=False,
-        )
-
-        x, y = next(iter(train_dataloader))
-
-        loss, grads, outer_models, meta_opt_states = outer_step(
-            outer_models,
-            inner_model,
-            x,
-            y,
-            meta_opt,
-            meta_opt_states,
-            loss_fn,
-            base_act,
-        )
+
+        inner_afuncs = [ partial(mlp_afunc, model = outer_model, base_act = base_act) for outer_model in outer_models]
+
+        inner_model = MultiActMLP(inner_config.input_dim,
+                                    inner_config.output_dim,
+                                    inner_config.hidden_layer_sizes,
+                                    inner_model_key, bias=True)
+        
+        inner_model = init_linear_weight(inner_model, xavier_normal_init, inner_model_key)
+
+        inner_model, _, inner_results = inner_opt(inner_model,
+                                    train_dataloader, test_dataloader,
+                                    inner_afuncs, opt, loss_fn,
+                                    inner_config, training=True,
+                                    verbose=False)
+
+        x,y = next(iter(train_dataloader))
+
+        
+        loss, grads, outer_models, meta_opt_states = outer_step(outer_models, inner_model, x, y, meta_opt, meta_opt_states, loss_fn, base_act)
         grad_norm_tree = jax.tree_map(lambda x: jnp.linalg.norm(x), grads)
         grad_norm_scalar = jax.tree_util.tree_reduce(jnp.add, grad_norm_tree)
         results["grad_norms"].append(grad_norm_scalar)
         results["train_loss"].append(loss)
         mean_inner_test_loss = np.mean(inner_results.test_loss[-50:])
         results["test_loss"].append(mean_inner_test_loss)
 
         if step % outer_config.print_every == 0:
-            logging.info(
-                f"Step {step :03d} | Train Loss: {results['train_loss'][-1] :.4e} | Test Loss: {mean_inner_test_loss :.4e} | Grad Norm: {results['grad_norms'][-1] :.4e}"
-            )
+            logging.info(f"Step {step :03d} | Train Loss: {results['train_loss'][-1] :.4e} | Test Loss: {mean_inner_test_loss :.4e} | Grad Norm: {results['grad_norms'][-1] :.4e}")
 
         # sample activation functions
         x_sample = jnp.linspace(-10, 10, 100)
         y_list = [x_sample]
         for afunc in inner_afuncs:
             y_list.append(afunc(x_sample))
         results["inner_afuncs"].append(y_list)
 
-        if (
-            step % 100 == 0 or step == outer_config.steps - 1
-        ) and save_path is not None:
+
+        if (step % 100 == 0 or step == outer_config.steps-1) and save_path is not None:
             # pickle and save results
             with open(f"{save_path}/step_{step}.pkl", "wb") as f:
                 pickle.dump(results, f)
-
+            
             # save models
             for i, model in enumerate(outer_models):
-                save(
-                    f"{save_path}/step_{step}_activation_model_{i}.eqx",
-                    asdict(outer_config),
-                    model,
-                )
-
-    results_obj = OuterResults(
-        inner_test_loss=np.array(results["test_loss"]),
-        train_loss=np.array(results["train_loss"]),
-        inner_afuncs=np.array(results["inner_afuncs"]),
-        grad_norm=np.array(results["grad_norms"]),
-    )
-
+                save(f"{save_path}/step_{step}_activation_model_{i}.eqx", asdict(outer_config), model)
+    
+    results_obj = OuterResults(inner_test_loss= np.array(results["test_loss"]),
+                               train_loss= np.array(results["train_loss"]),
+                               inner_afuncs= np.array(results["inner_afuncs"]),
+                                 grad_norm= np.array(results["grad_norms"]))
+    
     return outer_models, results_obj
+
+
```

### Comparing `jaxDiversity-0.0.1/jaxDiversity/mlp.py` & `jaxDiversity-0.0.2/jaxDiversity/mlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,132 +8,114 @@
 import jax
 import jax.numpy as jnp
 import equinox as eqx
 import json
 
 # %% ../nbs/03_MLP.ipynb 5
 def trunc_init(weight: jax.Array, key: jax.random.PRNGKey) -> jax.Array:
-    """truncated normal initialization"""
+    """ truncated normal initialization """
     out, in_ = weight.shape
     stddev = jnp.sqrt(1 / in_)
     return stddev * jax.random.truncated_normal(key, lower=-2, upper=2)
 
-
 def deterministic_init(weight: jax.Array, key: jax.random.PRNGKey) -> jax.Array:
-    """constant initialization
+    """ constant initialization  
     parameters only for consistency with other initializations"""
     return jnp.ones(weight.shape) * 1e-3
 
-
 def xavier_normal_init(weight: jax.Array, key: jax.random.PRNGKey) -> jax.Array:
-    """xavier normal initialization"""
+    """ xavier normal initialization """
     out, in_ = weight.shape
     stddev = jnp.sqrt(2 / in_)
     return stddev * jax.random.normal(key, shape=weight.shape)
 
-
 def xavier_uniform_init(weight: jax.Array, key: jax.random.PRNGKey) -> jax.Array:
-    """xavier uniform initialization"""
+    """ xavier uniform initialization """
     out, in_ = weight.shape
     bound = jnp.sqrt(6 / in_)
     return bound * jax.random.uniform(key, shape=weight.shape, minval=-1, maxval=1)
 
+
 # %% ../nbs/03_MLP.ipynb 6
 def init_linear_weight(model, init_fn, key):
-    """initialize linear weights of a model with a given init_fn"""
-
+    """ initialize linear weights of a model with a given init_fn"""
     def is_linear(x):
         return isinstance(x, eqx.nn.Linear)
-
     def get_weights(m):
-        return [
-            x.weight
-            for x in jax.tree_util.tree_leaves(m, is_leaf=is_linear)
-            if is_linear(x)
-        ]
-
+        return [x.weight for x in jax.tree_util.tree_leaves(m, is_leaf=is_linear) if is_linear(x)]
     weights = get_weights(model)
-    new_weights = [
-        init_fn(weight, subkey)
-        for weight, subkey in zip(weights, jax.random.split(key, len(weights)))
-    ]
+    new_weights = [init_fn(weight, subkey)
+                    for weight, subkey in zip(weights, jax.random.split(key, len(weights)))]
     new_model = eqx.tree_at(get_weights, model, new_weights)
     return new_model
 
 # %% ../nbs/03_MLP.ipynb 7
 class MultiActMLP(eqx.Module):
     input_dim: int
     output_dim: int
     hidden_layer_sizes: list
     layers: list
-    bias: bool  # whether to include bias in the linear layers
+    bias: bool # whether to include bias in the linear layers
 
-    def __init__(self, input_dim, output_dim, hidden_layer_sizes, key, bias=True):
+    def __init__(self, input_dim, output_dim, hidden_layer_sizes, key, bias = True):
         super().__init__()
         self.bias = bias
         self.input_dim = input_dim
         self.output_dim = output_dim
         self.hidden_layer_sizes = [input_dim] + hidden_layer_sizes + [output_dim]
         self.layers = []
         keys = jax.random.split(key, len(self.hidden_layer_sizes))
-        for i in range(len(self.hidden_layer_sizes) - 1):
-            layer = eqx.nn.Linear(
-                self.hidden_layer_sizes[i],
-                self.hidden_layer_sizes[i + 1],
-                key=keys[i],
-                use_bias=bias,
-            )
+        for i in range(len(self.hidden_layer_sizes)-1):
+            layer = eqx.nn.Linear(self.hidden_layer_sizes[i],
+                                  self.hidden_layer_sizes[i+1], key=keys[i], use_bias=bias)
             self.layers.append(layer)
-
+    
     def __call__(self, x, afuncs):
         """
         x: input data
         afuncs: activation functions
         splits the layers into sections and applies the activation function
         """
         activity = []
         for layer in self.layers[:-1]:
-            split_idx = int(layer.weight.shape[0] / len(afuncs))
+            split_idx = int(layer.weight.shape[0]/len(afuncs))
             x = layer(x)
             activity.append(x)
             for i, afunc in enumerate(afuncs):
                 # applies activation functions to each split of layer
-                x = x.at[i * split_idx : (i + 1) * split_idx].set(
-                    afunc(x[i * split_idx : (i + 1) * split_idx])
-                )
-
+                x = x.at[i*split_idx:(i+1)*split_idx].set(afunc(x[i*split_idx:(i+1)*split_idx]))
+                
         # return self.apply_linear(x, self.layers[-1]), activity
         return self.layers[-1](x), activity
 
 # %% ../nbs/03_MLP.ipynb 9
 def save(filename, hyperparams, model):
-    """save model and hyperparameters to file"""
+    """ save model and hyperparameters to file """
     with open(filename, "wb") as f:
         hyperparam_str = json.dumps(hyperparams)
         f.write((hyperparam_str + "\n").encode())
         eqx.tree_serialise_leaves(f, model)
 
+
 # %% ../nbs/03_MLP.ipynb 11
 def make_mlp(config_dict):
-    """initialize MLP using hyperparameters from config_dict"""
+    """ initialize MLP using hyperparameters from config_dict """
     key = jax.random.PRNGKey(config_dict["seed"])
     model_key, init_key = jax.random.split(key)
-    model = eqx.nn.MLP(
-        in_size=config_dict["input_dim"],
-        out_size=config_dict["output_dim"],
-        width_size=config_dict["hidden_layer_sizes"][0],
-        depth=1,
-        key=model_key,
-        use_bias=True,
-    )
+    model = eqx.nn.MLP(in_size=config_dict["input_dim"],
+                        out_size=config_dict["output_dim"],
+                        width_size=config_dict["hidden_layer_sizes"][0],
+                        depth=1,
+                        key=model_key,
+                        use_bias=True)
     return model
 
 # %% ../nbs/03_MLP.ipynb 12
 def load(filename, make=make_mlp):
-    """load model and hyperparameters from file"""
+    """ load model and hyperparameters from file """
     with open(filename, "rb") as f:
         hyperparams = json.loads(f.readline().decode())
         model = make(hyperparams)
         return eqx.tree_deserialise_leaves(f, model)
 
 # %% ../nbs/03_MLP.ipynb 14
 def mlp_afunc(x, model, base_act):
```

### Comparing `jaxDiversity-0.0.1/jaxDiversity/utilclasses.py` & `jaxDiversity-0.0.2/jaxDiversity/utilclasses.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     batch_size: int
     epochs: int
     lr: float
     mu: float
     n_fns: int
     l2_reg: float
     seed: int
-    base_act: str = "sin"
+    base_act: str = 'sin'
+
 
 # %% ../nbs/02_UtilClasses.ipynb 5
 @dataclass
 class OuterConfig:
     input_dim: int
     output_dim: int
     hidden_layer_sizes: list
@@ -37,23 +38,23 @@
 
 # %% ../nbs/02_UtilClasses.ipynb 6
 @dataclass
 class InnerResults:
     """
     dataclass to store inner loop results
     """
-
     train_loss: list
     test_loss: list
     grad_norm: list
 
+
 # %% ../nbs/02_UtilClasses.ipynb 7
 @dataclass
 class OuterResults:
     """
     dataclass to store outer loop results
     """
-
     inner_test_loss: list
     train_loss: list
     inner_afuncs: list
     grad_norm: list
+
```

### Comparing `jaxDiversity-0.0.1/settings.ini` & `jaxDiversity-0.0.2/settings.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 [DEFAULT]
-# All sections below are required unless otherwise specified.
-# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
-
-### Python library ###
 repo = jaxDiversity
-lib_name = %(repo)s
-version = 0.0.1
-min_python = 3.10
+lib_name = jaxDiversity
+version = 0.0.2
+min_python = 3.9
 license = apache2
-black_formatting = True
-
-### nbdev ###
+black_formatting = False
 doc_path = _docs
 lib_path = jaxDiversity
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
-
-### Docs ###
 branch = main
 custom_sidebar = False
 doc_host = https://NonlinearArtificialIntelligenceLabs.github.io
-doc_baseurl = /%(repo)s
-git_url = https://github.com/NonlinearArtificialIntelligenceLab/%(repo)s
-title = %(lib_name)s
-
-### PyPI ###
+doc_baseurl = /jaxDiversity
+git_url = https://github.com/NonlinearArtificialIntelligenceLab/jaxDiversity
+title = jaxDiversity
 audience = Developers
-author = NonlinearArtificialIntelligenceLab
+author = Anil Radhakrishnan
 author_email = aradhak5@ncsu.edu
-copyright = 2023 onwards, %(author)s
+copyright = 2023 onwards, Anil Radhakrishnan
 description = jax implementation for metalearning neuronal diversity
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
-user = Anil Radhakrishnan
+user = NonlinearArtificialIntelligenceLab
+requirements = nbdev jax jaxlib optax equinox fastcore matplotlib pandas torch seaborn tqdm
+console_scripts = nbdev_export=nbdev.cli:nbdev_export
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
 
-### Optional ###
-requirements = fastcore pandas numpy matplotlib seaborn jax jaxlib equinox optax tqdm
-# dev_requirements = 
-# console_scripts =
```

### Comparing `jaxDiversity-0.0.1/setup.py` & `jaxDiversity-0.0.2/setup.py`

 * *Files identical despite different names*

