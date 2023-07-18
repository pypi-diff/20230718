# Comparing `tmp/PyTorch-Beacon-0.0.1.tar.gz` & `tmp/PyTorch-Beacon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTorch-Beacon-0.0.1.tar", last modified: Mon Jul 17 15:51:54 2023, max compression
+gzip compressed data, was "PyTorch-Beacon-0.0.2.tar", last modified: Tue Jul 18 16:19:21 2023, max compression
```

## Comparing `PyTorch-Beacon-0.0.1.tar` & `PyTorch-Beacon-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lukelele   (501) staff       (20)        0 2023-07-17 15:51:54.464166 PyTorch-Beacon-0.0.1/
--rw-r--r--   0 lukelele   (501) staff       (20)     1050 2023-07-17 15:38:51.000000 PyTorch-Beacon-0.0.1/LICENCE
--rw-r--r--   0 lukelele   (501) staff       (20)      313 2023-07-17 15:51:54.463403 PyTorch-Beacon-0.0.1/PKG-INFO
-drwxr-xr-x   0 lukelele   (501) staff       (20)        0 2023-07-17 15:51:54.457330 PyTorch-Beacon-0.0.1/PyTorch_Beacon.egg-info/
--rw-r--r--   0 lukelele   (501) staff       (20)      313 2023-07-17 15:51:54.000000 PyTorch-Beacon-0.0.1/PyTorch_Beacon.egg-info/PKG-INFO
--rw-r--r--   0 lukelele   (501) staff       (20)      278 2023-07-17 15:51:54.000000 PyTorch-Beacon-0.0.1/PyTorch_Beacon.egg-info/SOURCES.txt
--rw-r--r--   0 lukelele   (501) staff       (20)        1 2023-07-17 15:51:54.000000 PyTorch-Beacon-0.0.1/PyTorch_Beacon.egg-info/dependency_links.txt
--rw-r--r--   0 lukelele   (501) staff       (20)        7 2023-07-17 15:51:54.000000 PyTorch-Beacon-0.0.1/PyTorch_Beacon.egg-info/top_level.txt
--rw-r--r--   0 lukelele   (501) staff       (20)        0 2023-07-17 15:38:50.000000 PyTorch-Beacon-0.0.1/README.md
-drwxr-xr-x   0 lukelele   (501) staff       (20)        0 2023-07-17 15:51:54.462506 PyTorch-Beacon-0.0.1/beacon/
--rw-r--r--   0 lukelele   (501) staff       (20)       97 2023-07-17 12:54:32.000000 PyTorch-Beacon-0.0.1/beacon/__init__.py
--rw-r--r--   0 lukelele   (501) staff       (20)     1246 2023-07-17 14:47:08.000000 PyTorch-Beacon-0.0.1/beacon/dataloading.py
--rw-r--r--   0 lukelele   (501) staff       (20)      483 2023-07-17 13:34:24.000000 PyTorch-Beacon-0.0.1/beacon/metrics.py
--rw-r--r--   0 lukelele   (501) staff       (20)     1800 2023-07-17 15:02:30.000000 PyTorch-Beacon-0.0.1/beacon/training.py
--rw-r--r--   0 lukelele   (501) staff       (20)       16 2023-07-16 20:18:27.000000 PyTorch-Beacon-0.0.1/beacon/utils.py
--rw-r--r--   0 lukelele   (501) staff       (20)      422 2023-07-17 15:47:43.000000 PyTorch-Beacon-0.0.1/pyproject.toml
--rw-r--r--   0 lukelele   (501) staff       (20)       38 2023-07-17 15:51:54.464456 PyTorch-Beacon-0.0.1/setup.cfg
+drwxr-xr-x   0 lukelele   (501) staff       (20)        0 2023-07-18 16:19:21.653266 PyTorch-Beacon-0.0.2/
+-rw-r--r--   0 lukelele   (501) staff       (20)     1050 2023-07-17 15:38:51.000000 PyTorch-Beacon-0.0.2/LICENCE
+-rw-r--r--   0 lukelele   (501) staff       (20)      522 2023-07-18 16:19:21.653056 PyTorch-Beacon-0.0.2/PKG-INFO
+drwxr-xr-x   0 lukelele   (501) staff       (20)        0 2023-07-18 16:19:21.651017 PyTorch-Beacon-0.0.2/PyTorch_Beacon.egg-info/
+-rw-r--r--   0 lukelele   (501) staff       (20)      522 2023-07-18 16:19:21.000000 PyTorch-Beacon-0.0.2/PyTorch_Beacon.egg-info/PKG-INFO
+-rw-r--r--   0 lukelele   (501) staff       (20)      278 2023-07-18 16:19:21.000000 PyTorch-Beacon-0.0.2/PyTorch_Beacon.egg-info/SOURCES.txt
+-rw-r--r--   0 lukelele   (501) staff       (20)        1 2023-07-18 16:19:21.000000 PyTorch-Beacon-0.0.2/PyTorch_Beacon.egg-info/dependency_links.txt
+-rw-r--r--   0 lukelele   (501) staff       (20)        7 2023-07-18 16:19:21.000000 PyTorch-Beacon-0.0.2/PyTorch_Beacon.egg-info/top_level.txt
+-rw-r--r--   0 lukelele   (501) staff       (20)      208 2023-07-17 18:11:59.000000 PyTorch-Beacon-0.0.2/README.md
+drwxr-xr-x   0 lukelele   (501) staff       (20)        0 2023-07-18 16:19:21.652738 PyTorch-Beacon-0.0.2/beacon/
+-rw-r--r--   0 lukelele   (501) staff       (20)       97 2023-07-17 12:54:32.000000 PyTorch-Beacon-0.0.2/beacon/__init__.py
+-rw-r--r--   0 lukelele   (501) staff       (20)     1246 2023-07-17 15:56:19.000000 PyTorch-Beacon-0.0.2/beacon/dataloading.py
+-rw-r--r--   0 lukelele   (501) staff       (20)      483 2023-07-17 13:34:24.000000 PyTorch-Beacon-0.0.2/beacon/metrics.py
+-rw-r--r--   0 lukelele   (501) staff       (20)     1797 2023-07-18 16:17:38.000000 PyTorch-Beacon-0.0.2/beacon/training.py
+-rw-r--r--   0 lukelele   (501) staff       (20)      534 2023-07-17 18:27:53.000000 PyTorch-Beacon-0.0.2/beacon/utils.py
+-rw-r--r--   0 lukelele   (501) staff       (20)      470 2023-07-17 18:30:54.000000 PyTorch-Beacon-0.0.2/pyproject.toml
+-rw-r--r--   0 lukelele   (501) staff       (20)       38 2023-07-18 16:19:21.653343 PyTorch-Beacon-0.0.2/setup.cfg
```

### Comparing `PyTorch-Beacon-0.0.1/LICENCE` & `PyTorch-Beacon-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `PyTorch-Beacon-0.0.1/beacon/dataloading.py` & `PyTorch-Beacon-0.0.2/beacon/dataloading.py`

 * *Files identical despite different names*

### Comparing `PyTorch-Beacon-0.0.1/beacon/training.py` & `PyTorch-Beacon-0.0.2/beacon/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
     loss_func = loss_type()
     optimiser = optimiser(model.parameters(), lr=lr)
 
     losses = np.zeros(epochs)
     accuracies = np.zeros(epochs)
 
-    for epoch in tqdm(range(epochs)):
-        model.train()
+    model.train()
 
+    for epoch in tqdm(range(epochs)):
         batch_loss = 0
         batch_accuracy = 0
         
         for (x, y) in dataloader:
             x, y = x.to(device), y.to(device)
 
             y_pred = model(x)
@@ -52,13 +52,13 @@
 
     with torch.inference_mode():
         loss = 0
         for (x, y) in dataloader:
             x, y = x.to(device), y.to(device)
             y_pred = model(x)
             loss += loss_func(y_pred, y)
-            accuracy = accuracy_func(y_pred, y)
+            accuracy += accuracy_func(y_pred, y)
 
         loss /= len(dataloader)
         accuracy /= len(dataloader)
 
     return loss.item(), accuracy.item()
```

