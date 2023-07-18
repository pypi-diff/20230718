# Comparing `tmp/autogluon.timeseries-0.8.3b20230717.tar.gz` & `tmp/autogluon.timeseries-0.8.3b20230718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.8.3b20230717.tar", last modified: Mon Jul 17 09:04:22 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.8.3b20230718.tar", last modified: Tue Jul 18 09:04:22 2023, max compression
```

## Comparing `autogluon.timeseries-0.8.3b20230717.tar` & `autogluon.timeseries-0.8.3b20230718.tar`

### file list

```diff
@@ -1,73 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.747637 autogluon.timeseries-0.8.3b20230717/
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:04:22.747637 autogluon.timeseries-0.8.3b20230717/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.739637 autogluon.timeseries-0.8.3b20230717/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.739637 autogluon.timeseries-0.8.3b20230717/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.739637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.739637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    16645 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49484 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48122 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.743637 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-17 09:03:42.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 09:04:22.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:04:22.739637 autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-17 09:04:22.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-17 09:04:22.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:04:22.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 09:04:22.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 09:04:22.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 09:04:22.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:04:22.000000 autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.317388 autogluon.timeseries-0.8.3b20230718/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.317388 autogluon.timeseries-0.8.3b20230718/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16645 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49176 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48122 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.321388 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-18 09:03:47.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 09:04:22.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:22.317388 autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-18 09:04:22.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-18 09:04:22.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:04:22.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 09:04:22.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-18 09:04:22.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 09:04:22.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:04:22.000000 autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.8.3b20230717/PKG-INFO` & `autogluon.timeseries-0.8.3b20230718/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.8.3b20230717
+Version: 0.8.3b20230718
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.8.3b20230717/setup.py` & `autogluon.timeseries-0.8.3b20230718/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import logging
+import os
+import shutil
+from datetime import timedelta
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterator, List, Optional, Type
 
 import gluonts
 import gluonts.core.settings
 import numpy as np
 import pandas as pd
+import torch
+from gluonts.core.component import from_hyperparameters
 from gluonts.dataset.common import Dataset as GluonTSDataset
 from gluonts.dataset.field_names import FieldName
-from gluonts.model.estimator import Estimator as GluonTSEstimator
 from gluonts.model.forecast import Forecast, QuantileForecast, SampleForecast
-from gluonts.model.predictor import Predictor as GluonTSPredictor
+from gluonts.torch.model.estimator import PyTorchLightningEstimator as GluonTSPyTorchLightningEstimator
 from gluonts.torch.model.forecast import DistributionForecast
+from gluonts.torch.model.predictor import PyTorchPredictor as GluonTSPyTorchPredictor
 from pandas.tseries.frequencies import to_offset
 
+from autogluon.common.loaders import load_pkl
 from autogluon.common.utils.log_utils import set_logger_verbosity
-from autogluon.core.hpo.constants import RAY_BACKEND
 from autogluon.core.utils import warning_filter
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TimeSeriesDataFrame
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
 from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_ts_dataframe
-from autogluon.timeseries.utils.warning_filters import disable_root_logger
+from autogluon.timeseries.utils.warning_filters import disable_root_logger, torch_warning_filter
 
 logger = logging.getLogger(__name__)
 gts_logger = logging.getLogger(gluonts.__name__)
+pl_loggers = [logging.getLogger(name) for name in logging.root.manager.loggerDict if "pytorch_lightning" in name]
 
 
 GLUONTS_SUPPORTED_OFFSETS = ["Y", "Q", "M", "W", "D", "B", "H", "T", "min", "S"]
 
 
 class SimpleGluonTSDataset(GluonTSDataset):
     """A simple GluonTS dataset that wraps a TimeSeriesDataFrame and implements the
@@ -123,18 +129,18 @@
         objective function the model intends to optimize, will use mean_wQuantileLoss by default.
     hyperparameters:
         various hyperparameters that will be used by model (can be search spaces instead of
         fixed values). See *Other Parameters* in each inheriting model's documentation for
         possible values.
     """
 
+    gluonts_estimator_class: Type[GluonTSPyTorchLightningEstimator]
     gluonts_model_path = "gluon_ts"
-    gluonts_estimator_class: Type[GluonTSEstimator] = None
     # datatype of floating point and integers passed internally to GluonTS
-    float_dtype: Type = np.float64
+    float_dtype: Type = np.float32
     int_dtype: Type = np.int64
     # default number of samples for prediction
     default_num_samples: int = 1000
     supports_known_covariates: bool = False
     supports_past_covariates: bool = False
 
     def __init__(
@@ -152,23 +158,25 @@
             freq=freq,
             prediction_length=prediction_length,
             name=name,
             eval_metric=eval_metric,
             hyperparameters=hyperparameters,
             **kwargs,
         )
-        self.gts_predictor: Optional[GluonTSPredictor] = None
+        self.gts_predictor: Optional[GluonTSPyTorchPredictor] = None
         self.callbacks = []
         self.num_feat_static_cat = 0
         self.num_feat_static_real = 0
         self.num_feat_dynamic_real = 0
         self.num_past_feat_dynamic_real = 0
         self.feat_static_cat_cardinality: List[int] = []
 
     def save(self, path: str = None, verbose: bool = True) -> str:
+        # we flush callbacks instance variable if it has been set. it can keep weak references which breaks training
+        self.callbacks = []
         # The GluonTS predictor is serialized using custom logic
         predictor = self.gts_predictor
         self.gts_predictor = None
         path = Path(super().save(path=path, verbose=verbose))
 
         with disable_root_logger():
             if predictor:
@@ -176,24 +184,20 @@
                 predictor.serialize(path / self.gluonts_model_path)
 
         self.gts_predictor = predictor
 
         return str(path)
 
     @classmethod
-    def load(
-        cls, path: str, reset_paths: bool = True, load_oof: bool = False, verbose: bool = True
-    ) -> "AbstractGluonTSModel":
-        model = super().load(
-            path=path,
-            reset_paths=reset_paths,
-            load_oof=load_oof,
-            verbose=verbose,
-        )
-        model.gts_predictor = GluonTSPredictor.deserialize(Path(path) / cls.gluonts_model_path)
+    def load(cls, path: str, reset_paths: bool = True, verbose: bool = True) -> "AbstractGluonTSModel":
+        with torch_warning_filter():
+            model = load_pkl.load(path=os.path.join(path, cls.model_file_name), verbose=verbose)
+            if reset_paths:
+                model.set_contexts(path)
+            model.gts_predictor = GluonTSPyTorchPredictor.deserialize(Path(path) / cls.gluonts_model_path)
         return model
 
     def _deferred_init_params_aux(self, **kwargs) -> None:
         """Update GluonTS specific parameters with information available
         only at training time.
         """
         if "dataset" in kwargs:
@@ -239,22 +243,49 @@
                 quantiles=self.quantile_levels,
                 callbacks=self.callbacks,
             )
         )
         return args
 
     def _get_estimator_init_args(self) -> Dict[str, Any]:
-        """Get GluonTS specific constructor arguments for estimator objects, an alias to
-        `self._get_model_params` for better readability."""
-        return self._get_model_params()
+        """Get GluonTS specific constructor arguments for estimator objects, an alias to `self._get_model_params`
+        for better readability."""
+        init_kwargs = self._get_model_params()
+        # Map MXNet kwarg names to PyTorch Lightning kwarg names
+        init_kwargs.setdefault("lr", init_kwargs.get("learning_rate", 1e-3))
+        init_kwargs.setdefault("max_epochs", init_kwargs.get("epochs"))
+        return init_kwargs
 
-    def _get_estimator(self) -> GluonTSEstimator:
+    def _get_estimator(self) -> GluonTSPyTorchLightningEstimator:
         """Return the GluonTS Estimator object for the model"""
-        with warning_filter():
-            return self.gluonts_estimator_class.from_hyperparameters(**self._get_estimator_init_args())
+        # As GluonTSPyTorchLightningEstimator objects do not implement `from_hyperparameters` convenience
+        # constructors, we re-implement the logic here.
+        # we translate the "epochs" parameter to "max_epochs" for consistency in the AbstractGluonTSModel interface
+
+        init_args = self._get_estimator_init_args()
+
+        trainer_kwargs = {}
+        epochs = init_args.get("max_epochs")
+        callbacks = init_args.get("callbacks", [])
+
+        # TODO: Provide trainer_kwargs outside the function (e.g., to specify # of GPUs)?
+        if epochs is not None:
+            trainer_kwargs.update({"max_epochs": epochs})
+        trainer_kwargs.update({"callbacks": callbacks, "enable_progress_bar": False})
+        trainer_kwargs["default_root_dir"] = self.path
+
+        if torch.cuda.is_available():
+            trainer_kwargs["accelerator"] = "gpu"
+            trainer_kwargs["devices"] = 1
+
+        return from_hyperparameters(
+            self.gluonts_estimator_class,
+            trainer_kwargs=trainer_kwargs,
+            **init_args,
+        )
 
     def _to_gluonts_dataset(
         self, time_series_df: Optional[TimeSeriesDataFrame], known_covariates: Optional[TimeSeriesDataFrame] = None
     ) -> Optional[GluonTSDataset]:
         if time_series_df is not None:
             if self.num_feat_static_cat > 0:
                 feat_static_cat = time_series_df.static_features[self.metadata.static_features_cat]
@@ -304,41 +335,49 @@
         self,
         train_data: TimeSeriesDataFrame,
         val_data: Optional[TimeSeriesDataFrame] = None,
         time_limit: int = None,
         **kwargs,
     ) -> None:
         verbosity = kwargs.get("verbosity", 2)
+        for pl_logger in pl_loggers:
+            pl_logger.setLevel(logging.ERROR if verbosity <= 3 else logging.INFO)
         set_logger_verbosity(verbosity, logger=logger)
         gts_logger.setLevel(logging.ERROR if verbosity <= 3 else logging.INFO)
 
         if verbosity > 3:
             logger.warning(
                 "GluonTS logging is turned on during training. Note that losses reported by GluonTS "
                 "may not correspond to those specified via `eval_metric`."
             )
 
         self._check_fit_params()
-
         # update auxiliary parameters
         self._deferred_init_params_aux(
             dataset=train_data, callbacks=self._get_callbacks(time_limit=time_limit), **kwargs
         )
 
         estimator = self._get_estimator()
         with warning_filter(), disable_root_logger(), gluonts.core.settings.let(gluonts.env.env, use_tqdm=False):
             self.gts_predictor = estimator.train(
                 self._to_gluonts_dataset(train_data),
                 validation_data=self._to_gluonts_dataset(val_data),
                 cache_data=True,
             )
 
+        lightning_logs_dir = Path(self.path) / "lightning_logs"
+        if lightning_logs_dir.exists() and lightning_logs_dir.is_dir():
+            logger.debug(f"Removing lightning_logs directory {lightning_logs_dir}")
+            shutil.rmtree(lightning_logs_dir)
+
     def _get_callbacks(self, time_limit: int, *args, **kwargs) -> List[Callable]:
         """Retrieve a list of callback objects for the GluonTS trainer"""
-        return []
+        from pytorch_lightning.callbacks import Timer
+
+        return [Timer(timedelta(seconds=time_limit))] if time_limit is not None else []
 
     def predict(
         self,
         data: TimeSeriesDataFrame,
         known_covariates: Optional[TimeSeriesDataFrame] = None,
         quantile_levels: List[float] = None,
         **kwargs,
@@ -392,15 +431,27 @@
         )
         return QuantileForecast(**forecast_init_args)
 
     @staticmethod
     def _distribution_to_quantile_forecast(
         forecast: DistributionForecast, quantile_levels: List[float]
     ) -> QuantileForecast:
-        raise NotImplementedError
+        # Compute all quantiles in parallel instead of a for-loop
+        quantiles = torch.tensor(quantile_levels, device=forecast.distribution.mean.device).reshape(-1, 1)
+        quantile_predictions = forecast.distribution.icdf(quantiles).cpu().detach().numpy()
+        forecast_arrays = np.vstack([forecast.mean, quantile_predictions])
+        forecast_keys = ["mean"] + [str(q) for q in quantile_levels]
+
+        forecast_init_args = dict(
+            forecast_arrays=forecast_arrays,
+            start_date=forecast.start_date,
+            forecast_keys=forecast_keys,
+            item_id=str(forecast.item_id),
+        )
+        return QuantileForecast(**forecast_init_args)
 
     def _gluonts_forecasts_to_data_frame(
         self,
         forecasts: List[Forecast],
         quantile_levels: List[float],
         forecast_index: pd.MultiIndex,
     ) -> TimeSeriesDataFrame:
@@ -427,10 +478,7 @@
             for quantile in quantile_levels:
                 item_forecast_dict[str(quantile)] = forecast.quantile(str(quantile))
             result_dfs.append(pd.DataFrame(item_forecast_dict))
 
         result = pd.concat(result_dfs)
         result.index = forecast_index
         return TimeSeriesDataFrame(result)
-
-    def _get_hpo_backend(self):
-        return RAY_BACKEND
```

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/models/presets.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,34 +48,14 @@
     AutoARIMA=AutoARIMAModel,
     DynamicOptimizedTheta=DynamicOptimizedThetaModel,
     Theta=ThetaModel,
     ARIMA=ARIMAModel,
     ETS=ETSModel,
     ThetaStatsmodels=ThetaStatsmodelsModel,
 )
-if agts.MXNET_INSTALLED:
-    from .gluonts.mx import (
-        DeepARMXNetModel,
-        MQCNNMXNetModel,
-        MQRNNMXNetModel,
-        SimpleFeedForwardMXNetModel,
-        TemporalFusionTransformerMXNetModel,
-        TransformerMXNetModel,
-    )
-
-    MODEL_TYPES.update(
-        dict(
-            DeepARMXNet=DeepARMXNetModel,
-            SimpleFeedForwardMXNet=SimpleFeedForwardMXNetModel,
-            MQCNNMXNet=MQCNNMXNetModel,
-            MQRNNMXNet=MQRNNMXNetModel,
-            TransformerMXNet=TransformerMXNetModel,
-            TemporalFusionTransformerMXNet=TemporalFusionTransformerMXNetModel,
-        )
-    )
 
 DEFAULT_MODEL_NAMES = {v: k for k, v in MODEL_TYPES.items()}
 DEFAULT_MODEL_PRIORITY = dict(
     Naive=100,
     SeasonalNaive=100,
     Theta=90,
     AutoETS=80,
@@ -87,20 +67,14 @@
     DirectTabular=40,
     AutoARIMA=30,
     # Models below are not included in any presets
     ARIMA=30,
     ThetaStatsmodels=90,
     SimpleFeedForward=30,
     DynamicOptimizedTheta=30,
-    DeepARMXNet=50,
-    SimpleFeedForwardMXNet=30,
-    TemporalFusionTransformerMXNet=50,
-    TransformerMXNet=30,
-    MQCNNMXNet=10,
-    MQRNNMXNet=10,
 )
 DEFAULT_CUSTOM_MODEL_PRIORITY = 0
 
 VALID_AG_ARGS_KEYS = {
     "name",
     "name_prefix",
     "name_suffix",
@@ -214,18 +188,21 @@
 
     for model in model_priority_list:
         if isinstance(model, str):
             if model not in MODEL_TYPES:
                 raise ValueError(f"Model {model} is not supported yet.")
             if model in excluded_models:
                 logger.info(
-                    f"\tFound '{model}' model in hyperparameters, but '{model}' "
+                    f"\tFound '{model}' model in `hyperparameters`, but '{model}' "
                     "is present in `excluded_model_types` and will be removed."
                 )
                 continue
+            if "mxnet" in model.lower():
+                logger.info(f"\tMXNet model '{model}' given in `hyperparameters` is deprecated and won't be trained. ")
+                continue
             model_type = MODEL_TYPES[model]
         elif isinstance(model, type):
             if not issubclass(model, AbstractTimeSeriesModel):
                 raise ValueError(f"Custom model type {model} must inherit from `AbstractTimeSeriesModel`.")
             model_type = model
         else:
             raise ValueError(
```

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import os
 import pprint
 import time
 import warnings
 from typing import Any, Dict, List, Optional, Type, Union
 
 import pandas as pd
+import pytorch_lightning as pl
 
 from autogluon.common.utils.log_utils import set_logger_verbosity
 from autogluon.common.utils.utils import check_saved_predictor_version, setup_outputdir
 from autogluon.core.utils.decorators import apply_presets
 from autogluon.core.utils.loaders import load_pkl, load_str
 from autogluon.core.utils.savers import save_pkl, save_str
 from autogluon.timeseries import __version__ as current_ag_version
 from autogluon.timeseries.configs import TIMESERIES_PRESETS_CONFIGS
-from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
+from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TimeSeriesDataFrame
 from autogluon.timeseries.learner import AbstractLearner, TimeSeriesLearner
 from autogluon.timeseries.trainer import AbstractTimeSeriesTrainer
-from autogluon.timeseries.utils.random import set_random_seed
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_FREQUENCIES = {"D", "W", "M", "Q", "A", "Y", "H", "T", "min", "S"}
 
 
 class TimeSeriesPredictor:
@@ -419,36 +419,33 @@
 
             In the above example, multiple versions of the DeepAR model with different values of the parameters
             "hidden_size" and "dropout_rate" will be trained.
         hyperparameter_tune_kwargs : str or dict, optional
             Hyperparameter tuning strategy and kwargs (for example, how many HPO trials to run). If ``None``, then
             hyperparameter tuning will not be performed.
 
-            Ray Tune backend is used to tune deep-learning forecasting models from GluonTS implemented in MXNet. All
-            other models use a custom HPO backed based on random search.
+            Currently, only HPO based on random search is supported for time series models.
 
-            Can be set to a string to choose one of available presets:
+            Setting this parameter to string ``"random"`` performs 10 trials of random search per model.
 
-            - ``"random"``: 10 trials of random search
-            - ``"auto"``: 10 trials of bayesian optimization GluonTS MXNet models, 10 trials of random search for other models
-
-            Alternatively, a dict can be passed for more fine-grained control. The dict must include the following keys
+            We can change the number of random search trials per model by passing a dictionary as `hyperparameter_tune_kwargs`.
+            The dict must include the following keys
 
             - ``"num_trials"``: int, number of configurations to train for each tuned model
-            - ``"searcher"``: one of ``"random"`` (random search), ``"bayes"`` (bayesian optimization for GluonTS MXNet models, random search for other models) and ``"auto"`` (same as ``"bayes"``).
-            - ``"scheduler"``: the only supported option is ``"local"`` (all models trained on the same machine)
+            - ``"searcher"``: currently, the only supported option is ``"random"`` (random search)
+            - ``"scheduler"``: currently, the only supported option is ``"local"`` (all models trained on the same machine)
 
             Example::
 
                 predictor.fit(
                     ...
                     hyperparameter_tune_kwargs={
-                        "scheduler": "local",
-                        "searcher": "auto",
                         "num_trials": 5,
+                        "searcher": "random",
+                        "scheduler": "local",
                     },
                 )
         excluded_model_types: List[str], optional
             Banned subset of model types to avoid training during ``fit()``, even if present in ``hyperparameters``.
             For example, the following code will train all models included in the ``high_quality`` presets except ``DeepAR``::
 
                 predictor.fit(
@@ -522,15 +519,15 @@
                 logger.warning("Multi-window backtesting is disabled (setting num_val_windows = 0)")
                 num_val_windows = 0
         num_val_windows = self._validate_num_val_windows(train_data, tuning_data, num_val_windows)
 
         logger.info("=====================================================")
 
         if random_seed is not None:
-            set_random_seed(random_seed)
+            pl.seed_everything(random_seed)
 
         time_left = None if time_limit is None else time_limit - (time.time() - time_start)
         self._learner.fit(
             train_data=train_data,
             val_data=tuning_data,
             hyperparameters=hyperparameters,
             hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
@@ -620,15 +617,15 @@
         item_id timestamp
         A       2020-01-08    30.2
                 2020-01-09    27.0
         B       2020-03-04    17.1
                 2020-03-05     8.3
         """
         if random_seed is not None:
-            set_random_seed(random_seed)
+            pl.seed_everything(random_seed)
         # Don't use data.item_ids in case data is not a TimeSeriesDataFrame
         original_item_id_order = data.reset_index()[ITEMID].unique()
         data = self._check_and_prepare_data_frame(data)
         predictions = self._learner.predict(data, known_covariates=known_covariates, model=model, use_cache=use_cache)
         return predictions.reindex(original_item_id_order, level=ITEMID)
 
     def evaluate(self, data: Union[TimeSeriesDataFrame, pd.DataFrame], **kwargs):
```

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.8.3b20230718/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.8.3b20230717
+Version: 0.8.3b20230718
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.8.3b20230717/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.8.3b20230718/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,14 @@
 src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
 src/autogluon/timeseries/models/autogluon_tabular/utils.py
 src/autogluon/timeseries/models/ensemble/__init__.py
 src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
 src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
 src/autogluon/timeseries/models/gluonts/__init__.py
 src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-src/autogluon/timeseries/models/gluonts/mx/__init__.py
-src/autogluon/timeseries/models/gluonts/mx/callback.py
-src/autogluon/timeseries/models/gluonts/mx/models.py
 src/autogluon/timeseries/models/gluonts/torch/__init__.py
 src/autogluon/timeseries/models/gluonts/torch/models.py
 src/autogluon/timeseries/models/local/__init__.py
 src/autogluon/timeseries/models/local/abstract_local_model.py
 src/autogluon/timeseries/models/local/naive.py
 src/autogluon/timeseries/models/local/statsforecast.py
 src/autogluon/timeseries/models/local/statsmodels.py
@@ -44,10 +41,9 @@
 src/autogluon/timeseries/models/multi_window/multi_window_model.py
 src/autogluon/timeseries/trainer/__init__.py
 src/autogluon/timeseries/trainer/abstract_trainer.py
 src/autogluon/timeseries/trainer/auto_trainer.py
 src/autogluon/timeseries/utils/__init__.py
 src/autogluon/timeseries/utils/features.py
 src/autogluon/timeseries/utils/forecast.py
-src/autogluon/timeseries/utils/random.py
 src/autogluon/timeseries/utils/seasonality.py
 src/autogluon/timeseries/utils/warning_filters.py
```

