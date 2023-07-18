# Comparing `tmp/neuralforecast-1.6.0.tar.gz` & `tmp/neuralforecast-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralforecast-1.6.0.tar", last modified: Tue Jul 11 17:46:23 2023, max compression
+gzip compressed data, was "neuralforecast-1.6.1.tar", last modified: Tue Jul 18 21:18:45 2023, max compression
```

## Comparing `neuralforecast-1.6.0.tar` & `neuralforecast-1.6.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.629325 neuralforecast-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-11 17:46:13.000000 neuralforecast-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 17:46:13.000000 neuralforecast-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-11 17:46:23.629325 neuralforecast-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-11 17:46:13.000000 neuralforecast-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.617325 neuralforecast-1.6.0/neuralforecast/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   127213 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)    33122 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.621325 neuralforecast-1.6.0/neuralforecast/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_base_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_base_multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    26007 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_base_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    29923 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_base_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/common/_scalers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27205 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.621325 neuralforecast-1.6.0/neuralforecast/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/losses/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    83647 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/losses/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.629325 neuralforecast-1.6.0/neuralforecast/models/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26097 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/autoformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/dilated_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25474 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/fedformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/gru.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/hint.py
--rw-r--r--   0 runner    (1001) docker     (123)    16629 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/nbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/nbeatsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)    35871 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/patchtst.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/stemgnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/tcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23078 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/tft.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/models/vanillatransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/tsdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/neuralforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:23.617325 neuralforecast-1.6.0/neuralforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 17:46:23.000000 neuralforecast-1.6.0/neuralforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:46:23.629325 neuralforecast-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-11 17:46:14.000000 neuralforecast-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:18:45.879973 neuralforecast-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-07-18 21:18:45.879973 neuralforecast-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:18:45.871973 neuralforecast-1.6.1/neuralforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130237 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:18:45.875973 neuralforecast-1.6.1/neuralforecast/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/common/_base_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24025 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/common/_base_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26007 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/common/_base_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30121 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/common/_base_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/common/_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/common/_scalers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27146 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:18:45.875973 neuralforecast-1.6.1/neuralforecast/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15633 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/losses/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83647 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/losses/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:18:45.879973 neuralforecast-1.6.1/neuralforecast/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26097 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/autoformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/deepar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/dilated_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25474 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/fedformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/gru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16629 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/nbeats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/nbeatsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35871 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/patchtst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/stemgnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/tcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23157 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/tft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/models/vanillatransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/tsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/neuralforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:18:45.871973 neuralforecast-1.6.1/neuralforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15207 2023-07-18 21:18:45.000000 neuralforecast-1.6.1/neuralforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-18 21:18:45.000000 neuralforecast-1.6.1/neuralforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:18:45.000000 neuralforecast-1.6.1/neuralforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 21:18:45.000000 neuralforecast-1.6.1/neuralforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:18:45.000000 neuralforecast-1.6.1/neuralforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 21:18:45.000000 neuralforecast-1.6.1/neuralforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 21:18:45.000000 neuralforecast-1.6.1/neuralforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:18:45.879973 neuralforecast-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-18 21:18:34.000000 neuralforecast-1.6.1/setup.py
```

### Comparing `neuralforecast-1.6.0/LICENSE` & `neuralforecast-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/PKG-INFO` & `neuralforecast-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralforecast
-Version: 1.6.0
+Version: 1.6.1
 Summary: Time series forecasting suite using deep learning models
 Home-page: https://github.com/Nixtla/neuralforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting deep-learning
 Classifier: Development Status :: 3 - Alpha
@@ -90,16 +90,16 @@
 # Split data and declare panel dataset
 Y_df = AirPassengersDF
 Y_train_df = Y_df[Y_df.ds<='1959-12-31'] # 132 train
 Y_test_df = Y_df[Y_df.ds>'1959-12-31'] # 12 test
 
 # Fit and predict with NBEATS and NHITS models
 horizon = len(Y_test_df)
-models = [NBEATS(input_size=2 * horizon, h=horizon, max_epochs=50),
-          NHITS(input_size=2 * horizon, h=horizon, max_epochs=50)]
+models = [NBEATS(input_size=2 * horizon, h=horizon, max_steps=50),
+          NHITS(input_size=2 * horizon, h=horizon, max_steps=50)]
 nf = NeuralForecast(models=models, freq='M')
 nf.fit(df=Y_train_df)
 Y_hat_df = nf.predict().reset_index()
 
 # Plot predictions
 fig, ax = plt.subplots(1, 1, figsize = (20, 7))
 Y_hat_df = Y_test_df.merge(Y_hat_df, how='left', on=['unique_id', 'ds'])
```

### Comparing `neuralforecast-1.6.0/README.md` & `neuralforecast-1.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 # Split data and declare panel dataset
 Y_df = AirPassengersDF
 Y_train_df = Y_df[Y_df.ds<='1959-12-31'] # 132 train
 Y_test_df = Y_df[Y_df.ds>'1959-12-31'] # 12 test
 
 # Fit and predict with NBEATS and NHITS models
 horizon = len(Y_test_df)
-models = [NBEATS(input_size=2 * horizon, h=horizon, max_epochs=50),
-          NHITS(input_size=2 * horizon, h=horizon, max_epochs=50)]
+models = [NBEATS(input_size=2 * horizon, h=horizon, max_steps=50),
+          NHITS(input_size=2 * horizon, h=horizon, max_steps=50)]
 nf = NeuralForecast(models=models, freq='M')
 nf.fit(df=Y_train_df)
 Y_hat_df = nf.predict().reset_index()
 
 # Plot predictions
 fig, ax = plt.subplots(1, 1, figsize = (20, 7))
 Y_hat_df = Y_test_df.merge(Y_hat_df, how='left', on=['unique_id', 'ds'])
```

### Comparing `neuralforecast-1.6.0/neuralforecast/_modidx.py` & `neuralforecast-1.6.1/neuralforecast/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,17 @@
                 'doc_baseurl': '/neuralforecast/',
                 'doc_host': 'https://Nixtla.github.io',
                 'git_url': 'https://github.com/Nixtla/neuralforecast/',
                 'lib_path': 'neuralforecast'},
   'syms': { 'neuralforecast.auto': { 'neuralforecast.auto.AutoAutoformer': ('models.html#autoautoformer', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoAutoformer.__init__': ( 'models.html#autoautoformer.__init__',
                                                                                       'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoDeepAR': ('models.html#autodeepar', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoDeepAR.__init__': ( 'models.html#autodeepar.__init__',
+                                                                                  'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDilatedRNN': ('models.html#autodilatedrnn', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDilatedRNN.__init__': ( 'models.html#autodilatedrnn.__init__',
                                                                                       'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoFEDformer': ('models.html#autofedformer', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoFEDformer.__init__': ( 'models.html#autofedformer.__init__',
                                                                                      'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoGRU': ('models.html#autogru', 'neuralforecast/auto.py'),
@@ -378,14 +381,34 @@
                                                                                                           'neuralforecast/models/autoformer.py'),
                                                   'neuralforecast.models.autoformer.SeriesDecomp': ( 'models.autoformer.html#seriesdecomp',
                                                                                                      'neuralforecast/models/autoformer.py'),
                                                   'neuralforecast.models.autoformer.SeriesDecomp.__init__': ( 'models.autoformer.html#seriesdecomp.__init__',
                                                                                                               'neuralforecast/models/autoformer.py'),
                                                   'neuralforecast.models.autoformer.SeriesDecomp.forward': ( 'models.autoformer.html#seriesdecomp.forward',
                                                                                                              'neuralforecast/models/autoformer.py')},
+            'neuralforecast.models.deepar': { 'neuralforecast.models.deepar.Decoder': ( 'models.deepar.html#decoder',
+                                                                                        'neuralforecast/models/deepar.py'),
+                                              'neuralforecast.models.deepar.Decoder.__init__': ( 'models.deepar.html#decoder.__init__',
+                                                                                                 'neuralforecast/models/deepar.py'),
+                                              'neuralforecast.models.deepar.Decoder.forward': ( 'models.deepar.html#decoder.forward',
+                                                                                                'neuralforecast/models/deepar.py'),
+                                              'neuralforecast.models.deepar.DeepAR': ( 'models.deepar.html#deepar',
+                                                                                       'neuralforecast/models/deepar.py'),
+                                              'neuralforecast.models.deepar.DeepAR.__init__': ( 'models.deepar.html#deepar.__init__',
+                                                                                                'neuralforecast/models/deepar.py'),
+                                              'neuralforecast.models.deepar.DeepAR.forward': ( 'models.deepar.html#deepar.forward',
+                                                                                               'neuralforecast/models/deepar.py'),
+                                              'neuralforecast.models.deepar.DeepAR.predict_step': ( 'models.deepar.html#deepar.predict_step',
+                                                                                                    'neuralforecast/models/deepar.py'),
+                                              'neuralforecast.models.deepar.DeepAR.train_forward': ( 'models.deepar.html#deepar.train_forward',
+                                                                                                     'neuralforecast/models/deepar.py'),
+                                              'neuralforecast.models.deepar.DeepAR.training_step': ( 'models.deepar.html#deepar.training_step',
+                                                                                                     'neuralforecast/models/deepar.py'),
+                                              'neuralforecast.models.deepar.DeepAR.validation_step': ( 'models.deepar.html#deepar.validation_step',
+                                                                                                       'neuralforecast/models/deepar.py')},
             'neuralforecast.models.dilated_rnn': { 'neuralforecast.models.dilated_rnn.AttentiveLSTMLayer': ( 'models.dilated_rnn.html#attentivelstmlayer',
                                                                                                              'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.AttentiveLSTMLayer.__init__': ( 'models.dilated_rnn.html#attentivelstmlayer.__init__',
                                                                                                                       'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.AttentiveLSTMLayer.forward': ( 'models.dilated_rnn.html#attentivelstmlayer.forward',
                                                                                                                      'neuralforecast/models/dilated_rnn.py'),
                                                    'neuralforecast.models.dilated_rnn.DRNN': ( 'models.dilated_rnn.html#drnn',
```

### Comparing `neuralforecast-1.6.0/neuralforecast/auto.py` & `neuralforecast-1.6.1/neuralforecast/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/models.ipynb.
 
 # %% auto 0
-__all__ = ['AutoRNN', 'AutoLSTM', 'AutoGRU', 'AutoTCN', 'AutoDilatedRNN', 'AutoMLP', 'AutoNBEATS', 'AutoNBEATSx', 'AutoNHITS',
-           'AutoTFT', 'AutoVanillaTransformer', 'AutoInformer', 'AutoAutoformer', 'AutoFEDformer', 'AutoPatchTST',
-           'AutoStemGNN', 'AutoHINT']
+__all__ = ['AutoRNN', 'AutoLSTM', 'AutoGRU', 'AutoTCN', 'AutoDeepAR', 'AutoDilatedRNN', 'AutoMLP', 'AutoNBEATS', 'AutoNBEATSx',
+           'AutoNHITS', 'AutoTFT', 'AutoVanillaTransformer', 'AutoInformer', 'AutoAutoformer', 'AutoFEDformer',
+           'AutoPatchTST', 'AutoStemGNN', 'AutoHINT']
 
-# %% ../nbs/models.ipynb 2
+# %% ../nbs/models.ipynb 3
 from os import cpu_count
 import torch
 
 from ray import tune
 from ray.tune.search.basic_variant import BasicVariantGenerator
 
 from .common._base_auto import BaseAuto
 
 from .models.rnn import RNN
 from .models.gru import GRU
 from .models.tcn import TCN
 from .models.lstm import LSTM
+from .models.deepar import DeepAR
 from .models.dilated_rnn import DilatedRNN
 
 from .models.mlp import MLP
 from .models.nbeats import NBEATS
 from .models.nbeatsx import NBEATSx
 from .models.nhits import NHITS
 
@@ -31,17 +32,17 @@
 from .models.autoformer import Autoformer
 from .models.fedformer import FEDformer
 from .models.patchtst import PatchTST
 
 from .models.stemgnn import StemGNN
 from .models.hint import HINT
 
-from .losses.pytorch import MAE
+from .losses.pytorch import MAE, MQLoss, DistributionLoss
 
-# %% ../nbs/models.ipynb 8
+# %% ../nbs/models.ipynb 9
 class AutoRNN(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
         "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "encoder_n_layers": tune.randint(1, 4),
@@ -96,15 +97,15 @@
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
         )
 
-# %% ../nbs/models.ipynb 12
+# %% ../nbs/models.ipynb 13
 class AutoLSTM(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
         "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "encoder_n_layers": tune.randint(1, 4),
@@ -154,15 +155,15 @@
             num_samples=num_samples,
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
         )
 
-# %% ../nbs/models.ipynb 16
+# %% ../nbs/models.ipynb 17
 class AutoGRU(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
         "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "encoder_n_layers": tune.randint(1, 4),
@@ -214,15 +215,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 19
+# %% ../nbs/models.ipynb 20
 class AutoTCN(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
         "inference_input_size_multiplier": [-1],
         "h": None,
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
         "context_size": tune.choice([5, 10, 50]),
@@ -273,15 +274,75 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 22
+# %% ../nbs/models.ipynb 23
+class AutoDeepAR(BaseAuto):
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "lstm_hidden_size": tune.choice([32, 64, 128, 256]),
+        "lstm_n_layers": tune.randint(1, 4),
+        "lstm_dropout": tune.uniform(0.0, 0.5),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice(["robust", "minmax1"]),
+        "max_steps": tune.choice([500, 1000, 2000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        loss=DistributionLoss(
+            distribution="StudentT", level=[80, 90], return_params=False
+        ),
+        valid_loss=MQLoss(level=[80, 90]),
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+    ):
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.default_config.copy()
+            config["input_size"] = tune.choice(
+                [h * x for x in self.default_config["input_size_multiplier"]]
+            )
+
+            # Rolling windows with step_size=1 or step_size=h
+            # See `BaseWindows` and `BaseRNN`'s create_windows
+            config["step_size"] = tune.choice([1, h])
+            del config["input_size_multiplier"]
+
+        super(AutoDeepAR, self).__init__(
+            cls_model=DeepAR,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+        )
+
+# %% ../nbs/models.ipynb 26
 class AutoDilatedRNN(BaseAuto):
     default_config = {
         "input_size_multiplier": [-1, 4, 16, 64],
         "inference_input_size_multiplier": [-1],
         "h": None,
         "cell_type": tune.choice(["LSTM", "GRU"]),
         "encoder_hidden_size": tune.choice([50, 100, 200, 300]),
@@ -334,15 +395,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 26
+# %% ../nbs/models.ipynb 30
 class AutoMLP(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([256, 512, 1024]),
         "num_layers": tune.randint(2, 6),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -391,15 +452,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 29
+# %% ../nbs/models.ipynb 33
 class AutoNBEATS(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
         "max_steps": tune.choice([500, 1000]),
@@ -446,15 +507,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 32
+# %% ../nbs/models.ipynb 36
 class AutoNBEATSx(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
         "max_steps": tune.choice([500, 1000]),
@@ -501,15 +562,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 35
+# %% ../nbs/models.ipynb 39
 class AutoNHITS(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "n_pool_kernel_size": tune.choice(
             [[2, 2, 1], 3 * [1], 3 * [2], 3 * [4], [8, 4, 1], [16, 8, 1]]
         ),
@@ -573,15 +634,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 39
+# %% ../nbs/models.ipynb 43
 class AutoTFT(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -630,15 +691,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 42
+# %% ../nbs/models.ipynb 46
 class AutoVanillaTransformer(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -687,15 +748,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 45
+# %% ../nbs/models.ipynb 49
 class AutoInformer(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -744,15 +805,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 48
+# %% ../nbs/models.ipynb 52
 class AutoAutoformer(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -801,15 +862,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 51
+# %% ../nbs/models.ipynb 55
 class AutoFEDformer(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
@@ -857,15 +918,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 54
+# %% ../nbs/models.ipynb 58
 class AutoPatchTST(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3],
         "h": None,
         "hidden_size": tune.choice([16, 128, 256]),
         "n_head": tune.choice([4, 16]),
         "patch_len": tune.choice([16, 24]),
@@ -916,15 +977,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 59
+# %% ../nbs/models.ipynb 63
 class AutoStemGNN(BaseAuto):
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4],
         "h": None,
         "n_series": None,
         "n_stacks": tune.choice([2, 3]),
         "multi_layer": tune.choice([3, 5, 7]),
@@ -977,15 +1038,15 @@
             refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
         )
 
-# %% ../nbs/models.ipynb 63
+# %% ../nbs/models.ipynb 67
 class AutoHINT(BaseAuto):
     def __init__(
         self,
         cls_model,
         h,
         loss,
         valid_loss,
```

### Comparing `neuralforecast-1.6.0/neuralforecast/common/_base_auto.py` & `neuralforecast-1.6.1/neuralforecast/common/_base_auto.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/common/_base_multivariate.py` & `neuralforecast-1.6.1/neuralforecast/common/_base_multivariate.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/common/_base_recurrent.py` & `neuralforecast-1.6.1/neuralforecast/common/_base_recurrent.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/common/_base_windows.py` & `neuralforecast-1.6.1/neuralforecast/common/_base_windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,19 +199,21 @@
             # -> [B * Ws, L+H, C] 0, 2, 3, 1
             windows_per_serie = windows.shape[2]
             windows = windows.permute(0, 2, 3, 1).contiguous()
             windows = windows.reshape(-1, window_size, len(temporal_cols))
 
             # Sample and Available conditions
             available_idx = temporal_cols.get_loc("available_mask")
-            sample_condition = windows[:, -self.h :, available_idx]
-            sample_condition = torch.sum(sample_condition, axis=1)
-            available_condition = windows[:, : -self.h, available_idx]
+            available_condition = windows[:, : self.input_size, available_idx]
             available_condition = torch.sum(available_condition, axis=1)
-            final_condition = (sample_condition > 0) & (available_condition > 0)
+            final_condition = available_condition > 0
+            if self.h > 0:
+                sample_condition = windows[:, self.input_size :, available_idx]
+                sample_condition = torch.sum(sample_condition, axis=1)
+                final_condition = (sample_condition > 0) & (available_condition > 0)
             windows = windows[final_condition]
 
             # Parse Static data to match windows
             # [B, S_in] -> [B, Ws, S_in] -> [B*Ws, S_in]
             static = batch.get("static", None)
             static_cols = batch.get("static_cols", None)
             if static is not None:
@@ -315,15 +317,16 @@
         temporal = windows["temporal"]  # B, L+H, C
         temporal_cols = windows["temporal_cols"].copy()  # B, L+H, C
 
         # To avoid leakage uses only the lags
         temporal_data_cols = temporal_cols.drop("available_mask").tolist()
         temporal_data = temporal[:, :, temporal_cols.get_indexer(temporal_data_cols)]
         temporal_mask = temporal[:, :, temporal_cols.get_loc("available_mask")].clone()
-        temporal_mask[:, -self.h :] = 0.0
+        if self.h > 0:
+            temporal_mask[:, -self.h :] = 0.0
 
         # Normalize. self.scaler stores the shift and scale for inverse transform
         temporal_mask = temporal_mask.unsqueeze(
             -1
         )  # Add channel dimension for scaler.transform.
         temporal_data = self.scaler.transform(x=temporal_data, mask=temporal_mask)
 
@@ -366,39 +369,42 @@
 
         return y_hat, y_loc, y_scale
 
     def _parse_windows(self, batch, windows):
         # Filter insample lags from outsample horizon
         y_idx = batch["temporal_cols"].get_loc("y")
         mask_idx = batch["temporal_cols"].get_loc("available_mask")
-        insample_y = windows["temporal"][:, : -self.h, y_idx]
-        insample_mask = windows["temporal"][:, : -self.h, mask_idx]
-        outsample_y = windows["temporal"][:, -self.h :, y_idx]
-        outsample_mask = windows["temporal"][:, -self.h :, mask_idx]
 
-        # Filter historic exogenous variables
+        insample_y = windows["temporal"][:, : self.input_size, y_idx]
+        insample_mask = windows["temporal"][:, : self.input_size, mask_idx]
+
+        # Declare additional information
+        outsample_y = None
+        outsample_mask = None
+        hist_exog = None
+        futr_exog = None
+        stat_exog = None
+
+        if self.h > 0:
+            outsample_y = windows["temporal"][:, self.input_size :, y_idx]
+            outsample_mask = windows["temporal"][:, self.input_size :, mask_idx]
+
         if len(self.hist_exog_list):
             hist_exog_idx = windows["temporal_cols"].get_indexer(self.hist_exog_list)
-            hist_exog = windows["temporal"][:, : -self.h, hist_exog_idx]
-        else:
-            hist_exog = None
+            hist_exog = windows["temporal"][:, : self.input_size, hist_exog_idx]
 
-        # Filter future exogenous variables
         if len(self.futr_exog_list):
             futr_exog_idx = windows["temporal_cols"].get_indexer(self.futr_exog_list)
             futr_exog = windows["temporal"][:, :, futr_exog_idx]
-        else:
-            futr_exog = None
-        # Filter static variables
+
         if len(self.stat_exog_list):
             static_idx = windows["static_cols"].get_indexer(self.stat_exog_list)
             stat_exog = windows["static"][:, static_idx]
-        else:
-            stat_exog = None
 
+        # TODO: think a better way of removing insample_y features
         if self.exclude_insample_y:
             insample_y = insample_y * 0
 
         return (
             insample_y,
             insample_mask,
             outsample_y,
```

### Comparing `neuralforecast-1.6.0/neuralforecast/common/_modules.py` & `neuralforecast-1.6.1/neuralforecast/common/_modules.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/common/_scalers.py` & `neuralforecast-1.6.1/neuralforecast/common/_scalers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/common.scalers.ipynb.
 
 # %% auto 0
-__all__ = ['masked_median', 'masked_mean', 'minmax_scaler', 'minmax1_scaler', 'std_scaler', 'robust_scaler', 'invariant_scaler',
-           'identity_scaler', 'TemporalNorm']
+__all__ = ['masked_median', 'masked_mean', 'minmax_statistics', 'minmax_scaler', 'inv_minmax_scaler', 'minmax1_statistics',
+           'minmax1_scaler', 'inv_minmax1_scaler', 'std_statistics', 'std_scaler', 'inv_std_scaler',
+           'robust_statistics', 'robust_scaler', 'inv_robust_scaler', 'invariant_statistics', 'invariant_scaler',
+           'inv_invariant_scaler', 'identity_statistics', 'identity_scaler', 'inv_identity_scaler', 'TemporalNorm']
 
 # %% ../../nbs/common.scalers.ipynb 4
 import torch
 import torch.nn as nn
 
 # %% ../../nbs/common.scalers.ipynb 7
 def masked_median(x, mask, dim=-1, keepdim=True):
@@ -51,15 +53,15 @@
     """
     x_nan = x.float().masked_fill(mask < 1, float("nan"))
     x_mean = x_nan.nanmean(dim=dim, keepdim=keepdim)
     x_mean = torch.nan_to_num(x_mean, nan=0.0)
     return x_mean
 
 # %% ../../nbs/common.scalers.ipynb 11
-def minmax_scaler(x, mask, eps=1e-6, dim=-1):
+def minmax_statistics(x, mask, eps=1e-6, dim=-1):
     """MinMax Scaler
 
     Standardizes temporal features by ensuring its range dweels between
     [0,1] range. This transformation is often used as an alternative
     to the standard scaler. The scaled features are obtained as:
 
     $$\mathbf{z} = (\mathbf{x}_{[B,T,C]}-\mathrm{min}({\mathbf{x}})_{[B,1,C]})/
@@ -88,24 +90,26 @@
     x_max = x_max.type(x.dtype)
     x_min = x_min.type(x.dtype)
 
     # x_range and prevent division by zero
     x_range = x_max - x_min
     x_range[x_range == 0] = 1.0
     x_range = x_range + eps
+    return x_min, x_range
+
+
+def minmax_scaler(x, x_min, x_range):
+    return (x - x_min) / x_range
 
-    z = (x - x_min) / x_range
-    return z, x_min, x_range
 
-# %% ../../nbs/common.scalers.ipynb 12
 def inv_minmax_scaler(z, x_min, x_range):
     return z * x_range + x_min
 
-# %% ../../nbs/common.scalers.ipynb 14
-def minmax1_scaler(x, mask, eps=1e-6, dim=-1):
+# %% ../../nbs/common.scalers.ipynb 13
+def minmax1_statistics(x, mask, eps=1e-6, dim=-1):
     """MinMax1 Scaler
 
     Standardizes temporal features by ensuring its range dweels between
     [-1,1] range. This transformation is often used as an alternative
     to the standard scaler or classic Min Max Scaler.
     The scaled features are obtained as:
 
@@ -135,26 +139,29 @@
     x_max = x_max.type(x.dtype)
     x_min = x_min.type(x.dtype)
 
     # x_range and prevent division by zero
     x_range = x_max - x_min
     x_range[x_range == 0] = 1.0
     x_range = x_range + eps
+    return x_min, x_range
+
 
+def minmax1_scaler(x, x_min, x_range):
     x = (x - x_min) / x_range
     z = x * (2) - 1
-    return z, x_min, x_range
+    return z
+
 
-# %% ../../nbs/common.scalers.ipynb 15
 def inv_minmax1_scaler(z, x_min, x_range):
     z = (z + 1) / 2
     return z * x_range + x_min
 
-# %% ../../nbs/common.scalers.ipynb 17
-def std_scaler(x, mask, dim=-1, eps=1e-6):
+# %% ../../nbs/common.scalers.ipynb 15
+def std_statistics(x, mask, dim=-1, eps=1e-6):
     """Standard Scaler
 
     Standardizes features by removing the mean and scaling
     to unit variance along the `dim` dimension.
 
     For example, for `base_windows` models, the scaled features are obtained as (with dim=1):
 
@@ -173,24 +180,26 @@
     """
     x_means = masked_mean(x=x, mask=mask, dim=dim)
     x_stds = torch.sqrt(masked_mean(x=(x - x_means) ** 2, mask=mask, dim=dim))
 
     # Protect against division by zero
     x_stds[x_stds == 0] = 1.0
     x_stds = x_stds + eps
+    return x_means, x_stds
+
+
+def std_scaler(x, x_means, x_stds):
+    return (x - x_means) / x_stds
 
-    z = (x - x_means) / x_stds
-    return z, x_means, x_stds
 
-# %% ../../nbs/common.scalers.ipynb 18
 def inv_std_scaler(z, x_mean, x_std):
     return (z * x_std) + x_mean
 
-# %% ../../nbs/common.scalers.ipynb 20
-def robust_scaler(x, mask, dim=-1, eps=1e-6):
+# %% ../../nbs/common.scalers.ipynb 17
+def robust_statistics(x, mask, dim=-1, eps=1e-6):
     """Robust Median Scaler
 
     Standardizes features by removing the median and scaling
     with the mean absolute deviation (mad) a robust estimator of variance.
     This scaler is particularly useful with noisy data where outliers can
     heavily influence the sample mean / variance in a negative way.
     In these scenarios the median and amd give better results.
@@ -221,24 +230,26 @@
     x_stds = torch.sqrt(masked_mean(x=(x - x_means) ** 2, mask=mask, dim=dim))
     x_mad_aux = x_stds * 0.6744897501960817
     x_mad = x_mad * (x_mad > 0) + x_mad_aux * (x_mad == 0)
 
     # Protect against division by zero
     x_mad[x_mad == 0] = 1.0
     x_mad = x_mad + eps
+    return x_median, x_mad
+
+
+def robust_scaler(x, x_median, x_mad):
+    return (x - x_median) / x_mad
 
-    z = (x - x_median) / x_mad
-    return z, x_median, x_mad
 
-# %% ../../nbs/common.scalers.ipynb 21
 def inv_robust_scaler(z, x_median, x_mad):
     return z * x_mad + x_median
 
-# %% ../../nbs/common.scalers.ipynb 23
-def invariant_scaler(x, mask, dim=-1, eps=1e-6):
+# %% ../../nbs/common.scalers.ipynb 19
+def invariant_statistics(x, mask, dim=-1, eps=1e-6):
     """Invariant Median Scaler
 
     Standardizes features by removing the median and scaling
     with the mean absolute deviation (mad) a robust estimator of variance.
     Aditionally it complements the transformation with the arcsinh transformation.
 
     For example, for `base_windows` models, the scaled features are obtained as (with dim=1):
@@ -267,24 +278,26 @@
     x_stds = torch.sqrt(masked_mean(x=(x - x_means) ** 2, mask=mask, dim=dim))
     x_mad_aux = x_stds * 0.6744897501960817
     x_mad = x_mad * (x_mad > 0) + x_mad_aux * (x_mad == 0)
 
     # Protect against division by zero
     x_mad[x_mad == 0] = 1.0
     x_mad = x_mad + eps
+    return x_median, x_mad
+
+
+def invariant_scaler(x, x_median, x_mad):
+    return torch.arcsinh((x - x_median) / x_mad)
 
-    z = torch.arcsinh((x - x_median) / x_mad)
-    return z, x_median, x_mad
 
-# %% ../../nbs/common.scalers.ipynb 24
 def inv_invariant_scaler(z, x_median, x_mad):
     return torch.sinh(z) * x_mad + x_median
 
-# %% ../../nbs/common.scalers.ipynb 26
-def identity_scaler(x, mask, dim=-1, eps=1e-6):
+# %% ../../nbs/common.scalers.ipynb 21
+def identity_statistics(x, mask, dim=-1, eps=1e-6):
     """Identity Scaler
 
     A placeholder identity scaler, that is argument insensitive.
 
     **Parameters:**<br>
     `x`: torch.Tensor input tensor.<br>
     `mask`: torch Tensor bool, same dimension as `x`, indicates where `x` is valid and False
@@ -299,21 +312,25 @@
     # Collapse dim dimension
     shape = list(x.shape)
     shape[dim] = 1
 
     x_shift = torch.zeros(shape)
     x_scale = torch.ones(shape)
 
-    return x, x_shift, x_scale
+    return x_shift, x_scale
+
+
+def identity_scaler(x, x_shift, x_scale):
+    return x
+
 
-# %% ../../nbs/common.scalers.ipynb 27
 def inv_identity_scaler(z, x_shift, x_scale):
     return z
 
-# %% ../../nbs/common.scalers.ipynb 30
+# %% ../../nbs/common.scalers.ipynb 24
 class TemporalNorm(nn.Module):
     """Temporal Normalization
 
     Standardization of the features is a common requirement for many
     machine learning estimators, and it is commonly achieved by removing
     the level and scaling its variance. The `TemporalNorm` module applies
     temporal normalization over the batch of inputs as defined by the type of scaler.
@@ -326,14 +343,23 @@
     `dim` (int, optional): Dimension over to compute scale and shift. Defaults to -1.<br>
     `eps` (float, optional): Small value to avoid division by zero. Defaults to 1e-6.<br>
 
     """
 
     def __init__(self, scaler_type="robust", dim=-1, eps=1e-6):
         super().__init__()
+        compute_statistics = {
+            None: identity_statistics,
+            "identity": identity_statistics,
+            "standard": std_statistics,
+            "robust": robust_statistics,
+            "minmax": minmax_statistics,
+            "minmax1": minmax1_statistics,
+            "invariant": invariant_statistics,
+        }
         scalers = {
             None: identity_scaler,
             "identity": identity_scaler,
             "standard": std_scaler,
             "robust": robust_scaler,
             "minmax": minmax_scaler,
             "minmax1": minmax1_scaler,
@@ -346,14 +372,15 @@
             "robust": inv_robust_scaler,
             "minmax": inv_minmax_scaler,
             "minmax1": inv_minmax1_scaler,
             "invariant": inv_invariant_scaler,
         }
         assert scaler_type in scalers.keys(), f"{scaler_type} not defined"
 
+        self.compute_statistics = compute_statistics[scaler_type]
         self.scaler = scalers[scaler_type]
         self.inverse_scaler = inverse_scalers[scaler_type]
         self.scaler_type = scaler_type
         self.dim = dim
         self.eps = eps
 
     # @torch.no_grad()
@@ -365,17 +392,20 @@
         `mask`: torch Tensor bool, shape  [batch, time] where `x` is valid and False
                 where `x` should be masked. Mask should not be all False in any column of
                 dimension dim to avoid NaNs from zero division.<br>
 
         **Returns:**<br>
         `z`: torch.Tensor same shape as `x`, except scaled.
         """
-        z, x_shift, x_scale = self.scaler(x=x, mask=mask, dim=self.dim, eps=self.eps)
+        x_shift, x_scale = self.compute_statistics(
+            x=x, mask=mask, dim=self.dim, eps=self.eps
+        )
         self.x_shift = x_shift
         self.x_scale = x_scale
+        z = self.scaler(x, x_shift, x_scale)
         return z
 
     # @torch.no_grad()
     def inverse_transform(self, z, x_shift=None, x_scale=None):
         """Scale back the data to the original representation.
 
         **Parameters:**<br>
```

### Comparing `neuralforecast-1.6.0/neuralforecast/core.py` & `neuralforecast-1.6.1/neuralforecast/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from .tsdataset import TimeSeriesDataset
 from neuralforecast.models import (
     GRU,
     LSTM,
     RNN,
     TCN,
+    DeepAR,
     DilatedRNN,
     MLP,
     NHITS,
     NBEATS,
     NBEATSx,
     TFT,
     VanillaTransformer,
@@ -114,14 +115,15 @@
 
 # %% ../nbs/core.ipynb 11
 MODEL_FILENAME_DICT = {
     "gru": GRU,
     "lstm": LSTM,
     "rnn": RNN,
     "tcn": TCN,
+    "deepar": DeepAR,
     "dilatedrnn": DilatedRNN,
     "mlp": MLP,
     "nbeats": NBEATS,
     "nbeatsx": NBEATSx,
     "nhits": NHITS,
     "tft": TFT,
     "vanillatransformer": VanillaTransformer,
@@ -129,14 +131,15 @@
     "autoformer": Autoformer,
     "patchtst": PatchTST,
     "stemgnn": StemGNN,
     "autogru": GRU,
     "autolstm": LSTM,
     "autornn": RNN,
     "autotcn": TCN,
+    "autodeepar": DeepAR,
     "autodilatedrnn": DilatedRNN,
     "automlp": MLP,
     "autonbeats": NBEATS,
     "autonbeatsx": NBEATSx,
     "autonhits": NHITS,
     "autotft": TFT,
     "autovanillatransformer": VanillaTransformer,
@@ -171,15 +174,16 @@
             Returns instantiated `NeuralForecast` class.
         """
         assert all(
             model.h == models[0].h for model in models
         ), "All models should have the same horizon"
 
         self.h = models[0].h
-        self.models = models
+        self.models_init = models
+        self.models = [deepcopy(model) for model in self.models_init]
         self.freq = pd.tseries.frequencies.to_offset(freq)
 
         # Flags and attributes
         self._fitted = False
 
     def _prepare_fit(self, df, static_df, sort_df):
         # TODO: uids, last_dates and ds should be properties of the dataset class. See github issue.
@@ -190,15 +194,15 @@
 
     def fit(
         self,
         df: Optional[pd.DataFrame] = None,
         static_df: Optional[pd.DataFrame] = None,
         val_size: Optional[int] = 0,
         sort_df: bool = True,
-        use_init_models: bool = True,
+        use_init_models: bool = False,
         verbose: bool = False,
     ):
         """Fit the core.NeuralForecast.
 
         Fit `models` to a large set of time series from DataFrame `df`.
         and store fitted models for later inspection.
 
@@ -209,15 +213,15 @@
             If None, a previously stored dataset is required.
         static_df : pandas.DataFrame, optional (default=None)
             DataFrame with columns [`unique_id`] and static exogenous.
         val_size : int, optional (default=0)
             Size of validation set.
         sort_df : bool, optional (default=False)
             Sort `df` before fitting.
-        use_init_models : bool, optional (default=True)
+        use_init_models : bool, optional (default=False)
             Use initial model passed when NeuralForecast object was instantiated.
         verbose : bool (default=False)
             Print processing steps.
 
         Returns
         -------
         self : NeuralForecast
@@ -244,19 +248,21 @@
 
         if val_size is not None:
             if self.dataset.min_size < val_size:
                 warnings.warn(
                     "Validation set size is larger than the shorter time-series."
                 )
 
-        # Recover initial model if use_init_models or is the first time fitting
-        if (use_init_models) or (not self._fitted):
-            self.models_fitted = [deepcopy(model) for model in self.models]
+        # Recover initial model if use_init_models
+        if use_init_models:
+            self.models = [deepcopy(model) for model in self.models_init]
+            if self._fitted:
+                print("WARNING: Deleting previously fitted models.")
 
-        for model in self.models_fitted:
+        for model in self.models:
             model.fit(self.dataset, val_size=val_size)
 
         self._fitted = True
 
     def predict(
         self,
         df: Optional[pd.DataFrame] = None,
@@ -308,15 +314,15 @@
             uids = self.uids
             last_dates = self.last_dates
             if verbose:
                 print("Using stored dataset.")
 
         cols = []
         count_names = {"model": 0}
-        for model in self.models_fitted:
+        for model in self.models:
             model_name = repr(model)
             count_names[model_name] = count_names.get(model_name, -1) + 1
             if count_names[model_name] > 0:
                 model_name += str(count_names[model_name])
             cols += [model_name + n for n in model.loss.output_names]
 
         # Placeholder dataframe for predictions with unique_id and ds
@@ -332,15 +338,15 @@
         else:
             dataset = TimeSeriesDataset.update_dataset(
                 dataset=dataset, future_df=fcsts_df.reset_index()
             )
 
         col_idx = 0
         fcsts = np.full((self.h * len(uids), len(cols)), fill_value=np.nan)
-        for model in self.models_fitted:
+        for model in self.models:
             old_test_size = model.get_test_size()
             model.set_test_size(self.h)  # To predict h steps ahead
             model_fcsts = model.predict(dataset=dataset, **data_kwargs)
             # Append predictions in memory placeholder
             output_length = len(model.loss.output_names)
             fcsts[:, col_idx : col_idx + output_length] = model_fcsts
             col_idx += output_length
@@ -357,15 +363,15 @@
         df: Optional[pd.DataFrame] = None,
         static_df: Optional[pd.DataFrame] = None,
         n_windows: int = 1,
         step_size: int = 1,
         val_size: Optional[int] = 0,
         test_size: Optional[int] = None,
         sort_df: bool = True,
-        use_init_models: bool = True,
+        use_init_models: bool = False,
         verbose: bool = False,
         **data_kwargs,
     ):
         """Temporal Cross-Validation with core.NeuralForecast.
 
         `core.NeuralForecast`'s cross-validation efficiently fits a list of NeuralForecast
         models through multiple windows, in either chained or rolled manner.
@@ -383,15 +389,15 @@
             Step size between each window.
         val_size : int, optional (default=None)
             Length of validation size. If passed, set `n_windows=None`.
         test_size : int, optional (default=None)
             Length of test size. If passed, set `n_windows=None`.
         sort_df : bool (default=True)
             Sort `df` before fitting.
-        use_init_models : bool, option (default=True)
+        use_init_models : bool, option (default=False)
             Use initial model passed when object was instantiated.
         verbose : bool (default=False)
             Print processing steps.
         data_kwargs : kwargs
             Extra arguments to be passed to the dataset within each model.
 
         Returns
@@ -409,28 +415,30 @@
                 df=df, static_df=static_df, sort_df=sort_df
             )
             self.sort_df = sort_df
         else:
             if verbose:
                 print("Using stored dataset.")
 
-        # Recover initial model if use_init_models and not fitted. If already fitted, will use models_fitted
-        if (use_init_models) or (not self._fitted):
-            self.models_fitted = [deepcopy(model) for model in self.models]
+        # Recover initial model if use_init_models.
+        if use_init_models:
+            self.models = [deepcopy(model) for model in self.models_init]
+            if self._fitted:
+                print("WARNING: Deleting previously fitted models.")
 
         cols = []
         count_names = {"model": 0}
-        for model in self.models_fitted:
+        for model in self.models:
             model_name = repr(model)
             count_names[model_name] = count_names.get(model_name, -1) + 1
             if count_names[model_name] > 0:
                 model_name += str(count_names[model_name])
             cols += [model_name + n for n in model.loss.output_names]
 
-        h = self.models_fitted[0].h
+        h = self.models[0].h
         if test_size is None:
             test_size = h + step_size * (n_windows - 1)
         elif n_windows is None:
             if (test_size - h) % step_size:
                 raise Exception("`test_size - h` should be module `step_size`")
             n_windows = int((test_size - h) / step_size) + 1
         elif (n_windows is None) and (test_size is None):
@@ -455,15 +463,15 @@
         fcsts_df.index = idx
 
         col_idx = 0
         fcsts = np.full(
             (self.dataset.n_groups * h * n_windows, len(cols)), np.nan, dtype=np.float32
         )
 
-        for model in self.models_fitted:
+        for model in self.models:
             model.fit(dataset=self.dataset, val_size=val_size, test_size=test_size)
             model_fcsts = model.predict(
                 self.dataset, step_size=step_size, **data_kwargs
             )
 
             # Append predictions in memory placeholder
             output_length = len(model.loss.output_names)
@@ -510,23 +518,23 @@
                 print(
                     f"WARNING: Predict insample might not provide accurate predictions for \
                       recurrent model {repr(model)} class yet due to scaling."
                 )
 
         cols = []
         count_names = {"model": 0}
-        for model in self.models_fitted:
+        for model in self.models:
             model_name = repr(model)
             count_names[model_name] = count_names.get(model_name, -1) + 1
             if count_names[model_name] > 0:
                 model_name += str(count_names[model_name])
             cols += [model_name + n for n in model.loss.output_names]
 
         # Remove test set from dataset and last dates
-        test_size = self.models_fitted[0].get_test_size()
+        test_size = self.models[0].get_test_size()
         if test_size > 0:
             trimmed_dataset = TimeSeriesDataset.trim_dataset(
                 dataset=self.dataset, right_trim=test_size, left_trim=0
             )
             last_dates_train = self.last_dates.shift(-test_size, freq=self.freq)
         else:
             trimmed_dataset = self.dataset
@@ -545,15 +553,15 @@
             step_size=step_size,
         )
         fcsts_df = fcsts_df.set_index("unique_id")
 
         col_idx = 0
         fcsts = np.full((len(fcsts_df), len(cols)), np.nan, dtype=np.float32)
 
-        for model in self.models_fitted:
+        for model in self.models:
             # Test size is the number of periods to forecast (full size of trimmed dataset)
             model.set_test_size(test_size=trimmed_dataset.max_size)
 
             # Predict
             model_fcsts = model.predict(trimmed_dataset, step_size=step_size)
             # Append predictions in memory placeholder
             output_length = len(model.loss.output_names)
@@ -600,15 +608,15 @@
         """
         # Standarize path without '/'
         if path[-1] == "/":
             path = path[:-1]
 
         # Model index list
         if model_index is None:
-            model_index = list(range(len(self.models_fitted)))
+            model_index = list(range(len(self.models)))
 
         # Create directory if not exists
         os.makedirs(path, exist_ok=True)
 
         # Check if directory is empty to protect overwriting files
         dir = os.listdir(path)
 
@@ -616,15 +624,15 @@
         if (len(dir) > 0) and (not overwrite):
             raise Exception(
                 "Directory is not empty. Set `overwrite=True` to overwrite files."
             )
 
         # Save models
         count_names = {"model": 0}
-        for i, model in enumerate(self.models_fitted):
+        for i, model in enumerate(self.models):
             # Skip model if not in list
             if i not in model_index:
                 continue
 
             model_name = repr(model).lower().replace("_", "")
             count_names[model_name] = count_names.get(model_name, -1) + 1
             model.save(f"{path}/{model_name}_{count_names[model_name]}.ckpt")
@@ -718,15 +726,11 @@
         if dataset is not None:
             neuralforecast.dataset = dataset
             neuralforecast.uids = config_dict["uids"]
             neuralforecast.last_dates = config_dict["last_dates"]
             neuralforecast.ds = config_dict["ds"]
             neuralforecast.sort_df = config_dict["sort_df"]
 
-        # Fitted flag and models_fitted
+        # Fitted flag
         neuralforecast._fitted = config_dict["_fitted"]
-        if config_dict["_fitted"]:
-            neuralforecast.models_fitted = [
-                deepcopy(model) for model in neuralforecast.models
-            ]
 
         return neuralforecast
```

### Comparing `neuralforecast-1.6.0/neuralforecast/losses/numpy.py` & `neuralforecast-1.6.1/neuralforecast/losses/numpy.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/losses/pytorch.py` & `neuralforecast-1.6.1/neuralforecast/losses/pytorch.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/__init__.py` & `neuralforecast-1.6.1/neuralforecast/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-__all__ = ['RNN', 'GRU', 'LSTM', 'TCN', 'DilatedRNN',
+__all__ = ['RNN', 'GRU', 'LSTM', 'TCN', 'DeepAR', 'DilatedRNN',
            'MLP', 'NHITS', 'NBEATS', 'NBEATSx',
            'TFT', 'VanillaTransformer', 'Informer', 'Autoformer', 'PatchTST', 'FEDformer',
            'StemGNN', 'HINT']
 
 from .rnn import RNN
 from .gru import GRU
 from .lstm import LSTM
 from .tcn import TCN
+from .deepar import DeepAR
 from .dilated_rnn import DilatedRNN
 from .mlp import MLP
 from .nhits import NHITS
 from .nbeats import NBEATS
 from .nbeatsx import NBEATSx
 from .tft import TFT
 from .stemgnn import StemGNN
```

### Comparing `neuralforecast-1.6.0/neuralforecast/models/autoformer.py` & `neuralforecast-1.6.1/neuralforecast/models/autoformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/dilated_rnn.py` & `neuralforecast-1.6.1/neuralforecast/models/dilated_rnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/fedformer.py` & `neuralforecast-1.6.1/neuralforecast/models/fedformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/gru.py` & `neuralforecast-1.6.1/neuralforecast/models/gru.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/hint.py` & `neuralforecast-1.6.1/neuralforecast/models/hint.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/informer.py` & `neuralforecast-1.6.1/neuralforecast/models/informer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/lstm.py` & `neuralforecast-1.6.1/neuralforecast/models/lstm.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/mlp.py` & `neuralforecast-1.6.1/neuralforecast/models/mlp.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/nbeats.py` & `neuralforecast-1.6.1/neuralforecast/models/nbeats.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/nbeatsx.py` & `neuralforecast-1.6.1/neuralforecast/models/nbeatsx.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/nhits.py` & `neuralforecast-1.6.1/neuralforecast/models/nhits.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/patchtst.py` & `neuralforecast-1.6.1/neuralforecast/models/patchtst.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/rnn.py` & `neuralforecast-1.6.1/neuralforecast/models/rnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/stemgnn.py` & `neuralforecast-1.6.1/neuralforecast/models/stemgnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/tcn.py` & `neuralforecast-1.6.1/neuralforecast/models/tcn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/models/tft.py` & `neuralforecast-1.6.1/neuralforecast/models/tft.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,14 +392,15 @@
     `h`: int, Forecast horizon. <br>
     `input_size`: int, autorregresive inputs size, y=[1,2,3,4] input_size=2 -> y_[t-2:t]=[1,2].<br>
     `stat_exog_list`: str list, static continuous columns.<br>
     `hist_exog_list`: str list, historic continuous columns.<br>
     `futr_exog_list`: str list, future continuous columns.<br>
     `hidden_size`: int, units of embeddings and encoders.<br>
     `dropout`: float (0, 1), dropout of inputs VSNs.<br>
+    `n_head`: int=4, number of attention heads in temporal fusion decoder.<br>
     `attn_dropout`: float (0, 1), dropout of fusion decoder's attention layer.<br>
     `shared_weights`: bool, If True, all blocks within each stack will share parameters. <br>
     `activation`: str, activation from ['ReLU', 'Softplus', 'Tanh', 'SELU', 'LeakyReLU', 'PReLU', 'Sigmoid'].<br>
     `loss`: PyTorch module, instantiated train loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `valid_loss`: PyTorch module=`loss`, instantiated valid loss class from [losses collection](https://nixtla.github.io/neuralforecast/losses.pytorch.html).<br>
     `max_steps`: int=1000, maximum number of training steps.<br>
     `learning_rate`: float=1e-3, Learning rate between (0, 1).<br>
```

### Comparing `neuralforecast-1.6.0/neuralforecast/models/vanillatransformer.py` & `neuralforecast-1.6.1/neuralforecast/models/vanillatransformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/tsdataset.py` & `neuralforecast-1.6.1/neuralforecast/tsdataset.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast/utils.py` & `neuralforecast-1.6.1/neuralforecast/utils.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.6.0/neuralforecast.egg-info/PKG-INFO` & `neuralforecast-1.6.1/neuralforecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralforecast
-Version: 1.6.0
+Version: 1.6.1
 Summary: Time series forecasting suite using deep learning models
 Home-page: https://github.com/Nixtla/neuralforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting deep-learning
 Classifier: Development Status :: 3 - Alpha
@@ -90,16 +90,16 @@
 # Split data and declare panel dataset
 Y_df = AirPassengersDF
 Y_train_df = Y_df[Y_df.ds<='1959-12-31'] # 132 train
 Y_test_df = Y_df[Y_df.ds>'1959-12-31'] # 12 test
 
 # Fit and predict with NBEATS and NHITS models
 horizon = len(Y_test_df)
-models = [NBEATS(input_size=2 * horizon, h=horizon, max_epochs=50),
-          NHITS(input_size=2 * horizon, h=horizon, max_epochs=50)]
+models = [NBEATS(input_size=2 * horizon, h=horizon, max_steps=50),
+          NHITS(input_size=2 * horizon, h=horizon, max_steps=50)]
 nf = NeuralForecast(models=models, freq='M')
 nf.fit(df=Y_train_df)
 Y_hat_df = nf.predict().reset_index()
 
 # Plot predictions
 fig, ax = plt.subplots(1, 1, figsize = (20, 7))
 Y_hat_df = Y_test_df.merge(Y_hat_df, how='left', on=['unique_id', 'ds'])
```

### Comparing `neuralforecast-1.6.0/neuralforecast.egg-info/SOURCES.txt` & `neuralforecast-1.6.1/neuralforecast.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 neuralforecast/common/_modules.py
 neuralforecast/common/_scalers.py
 neuralforecast/losses/__init__.py
 neuralforecast/losses/numpy.py
 neuralforecast/losses/pytorch.py
 neuralforecast/models/__init__.py
 neuralforecast/models/autoformer.py
+neuralforecast/models/deepar.py
 neuralforecast/models/dilated_rnn.py
 neuralforecast/models/fedformer.py
 neuralforecast/models/gru.py
 neuralforecast/models/hint.py
 neuralforecast/models/informer.py
 neuralforecast/models/lstm.py
 neuralforecast/models/mlp.py
```

### Comparing `neuralforecast-1.6.0/settings.ini` & `neuralforecast-1.6.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Nixtla
 description = Time series forecasting suite using deep learning models
 keywords = time-series forecasting deep-learning 
 author = Nixtla
 author_email = business@nixtla.io
 copyright = Nixtla Inc.
 branch = main
-version = 1.6.0
+version = 1.6.1
 min_python = 3.8
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
 requirements = numpy>=1.21.6 pandas>=1.3.5 torch>=2.0.0 pytorch-lightning>=2.0.0 ray[tune]>=2.2.0
```

### Comparing `neuralforecast-1.6.0/setup.py` & `neuralforecast-1.6.1/setup.py`

 * *Files identical despite different names*

