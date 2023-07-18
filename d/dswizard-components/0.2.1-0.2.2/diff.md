# Comparing `tmp/dswizard-components-0.2.1.tar.gz` & `tmp/dswizard-components-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dswizard-components-0.2.1.tar", last modified: Tue Mar  1 13:12:55 2022, max compression
+gzip compressed data, was "dswizard-components-0.2.2.tar", last modified: Wed Jun 29 08:23:44 2022, max compression
```

## Comparing `dswizard-components-0.2.1.tar` & `dswizard-components-0.2.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:12:55.359944 dswizard-components-0.2.1/
--rw-rw-r--   0 marc      (1000) marc      (1000)      116 2022-02-18 14:55:46.000000 dswizard-components-0.2.1/MANIFEST.in
--rw-rw-r--   0 marc      (1000) marc      (1000)      982 2022-03-01 13:12:55.359944 dswizard-components-0.2.1/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)      451 2021-04-17 12:01:34.000000 dswizard-components-0.2.1/README.md
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:12:55.351944 dswizard-components-0.2.1/dswizard/
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:12:55.351944 dswizard-components-0.2.1/dswizard/components/
--rw-rw-r--   0 marc      (1000) marc      (1000)      137 2022-01-04 14:54:30.000000 dswizard-components-0.2.1/dswizard/components/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    18814 2022-03-01 08:51:46.000000 dswizard-components-0.2.1/dswizard/components/base.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:12:55.351944 dswizard-components-0.2.1/dswizard/components/classification/
--rw-rw-r--   0 marc      (1000) marc      (1000)     1556 2022-01-04 15:27:16.000000 dswizard-components-0.2.1/dswizard/components/classification/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2151 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/classification/ada_boosting.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2463 2021-11-12 13:01:57.000000 dswizard-components-0.2.1/dswizard/components/classification/bernoulli_nb.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5099 2021-11-19 17:14:02.000000 dswizard-components-0.2.1/dswizard/components/classification/decision_tree.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:12:55.355944 dswizard-components-0.2.1/dswizard/components/classification/excluded/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2021-04-17 12:01:34.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5887 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/extra_trees.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1997 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/gaussian_nb.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4016 2021-11-19 17:14:46.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/gaussian_process.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2920 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/k_neighbors.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     6105 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/logistic_regression.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     8366 2022-03-01 08:45:45.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/mlp_classifier.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4115 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/passive_aggressive.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2172 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/qda.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4670 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/classification/excluded/svm.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5407 2021-11-19 17:14:02.000000 dswizard-components-0.2.1/dswizard/components/classification/gradient_boosting.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4391 2022-01-03 07:59:18.000000 dswizard-components-0.2.1/dswizard/components/classification/libsvm_svc.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3168 2021-11-12 13:03:17.000000 dswizard-components-0.2.1/dswizard/components/classification/linear_discriminant_analysis.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2413 2021-11-12 13:02:50.000000 dswizard-components-0.2.1/dswizard/components/classification/multinomial_nb.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5031 2021-11-19 17:14:02.000000 dswizard-components-0.2.1/dswizard/components/classification/random_forest.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5600 2022-01-03 18:47:13.000000 dswizard-components-0.2.1/dswizard/components/classification/sgd.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:12:55.355944 dswizard-components-0.2.1/dswizard/components/data_preprocessing/
--rw-rw-r--   0 marc      (1000) marc      (1000)      996 2022-01-04 15:27:16.000000 dswizard-components-0.2.1/dswizard/components/data_preprocessing/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4455 2022-03-01 10:47:00.000000 dswizard-components-0.2.1/dswizard/components/data_preprocessing/imputation.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2864 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/data_preprocessing/knn_imputer.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1003 2021-08-01 09:02:57.000000 dswizard-components-0.2.1/dswizard/components/data_preprocessing/max_abs_scaler.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      995 2021-08-01 09:02:57.000000 dswizard-components-0.2.1/dswizard/components/data_preprocessing/minmax.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1272 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/data_preprocessing/normalize.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2180 2021-08-01 09:02:57.000000 dswizard-components-0.2.1/dswizard/components/data_preprocessing/quantile_transformer.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1799 2022-03-01 08:56:00.000000 dswizard-components-0.2.1/dswizard/components/data_preprocessing/robust_scaler.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1177 2021-11-13 14:55:20.000000 dswizard-components-0.2.1/dswizard/components/data_preprocessing/standard_scaler.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:12:55.355944 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/
--rw-rw-r--   0 marc      (1000) marc      (1000)     1025 2022-01-04 15:27:16.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2227 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/bernoulli_rbm.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1603 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/binarizer.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3023 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/factor_analysis.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2878 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/fast_ica.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3928 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/feature_agglomeration.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2917 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/generic_univariate_select.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2075 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/kbinsdiscretizer.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4820 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/kpca.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1965 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/missing_indicator.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1907 2022-03-01 08:15:46.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/one_hot_encoding.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2221 2022-03-01 08:20:08.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/ordinal_encoder.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2651 2022-03-01 08:20:08.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/pca.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2099 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/polynomial.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4743 2022-03-01 08:20:08.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/random_trees_embedding.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3039 2021-06-30 08:10:47.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/select_k_best.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3927 2021-11-12 13:09:16.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/select_percentile.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2370 2022-03-01 08:20:08.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/truncated_svd.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1632 2022-01-09 20:29:09.000000 dswizard-components-0.2.1/dswizard/components/feature_preprocessing/variance_threshold.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    12093 2022-03-01 08:45:09.000000 dswizard-components-0.2.1/dswizard/components/meta_features.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4055 2022-03-01 08:25:03.000000 dswizard-components-0.2.1/dswizard/components/pipeline.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     7083 2022-03-01 08:37:36.000000 dswizard-components-0.2.1/dswizard/components/sklearn.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3553 2022-03-01 09:02:16.000000 dswizard-components-0.2.1/dswizard/components/util.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:12:55.355944 dswizard-components-0.2.1/dswizard/pynisher2/
--rw-rw-r--   0 marc      (1000) marc      (1000)       53 2022-01-04 09:23:52.000000 dswizard-components-0.2.1/dswizard/pynisher2/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    12330 2022-03-01 09:45:21.000000 dswizard-components-0.2.1/dswizard/pynisher2/limit_function_call.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:12:55.359944 dswizard-components-0.2.1/dswizard_components.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1000)      982 2022-03-01 13:12:55.000000 dswizard-components-0.2.1/dswizard_components.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)     3266 2022-03-01 13:12:55.000000 dswizard-components-0.2.1/dswizard_components.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)        1 2022-03-01 13:12:55.000000 dswizard-components-0.2.1/dswizard_components.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)      115 2022-03-01 13:12:55.000000 dswizard-components-0.2.1/dswizard_components.egg-info/requires.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)        9 2022-03-01 13:12:55.000000 dswizard-components-0.2.1/dswizard_components.egg-info/top_level.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)      114 2022-01-04 15:28:55.000000 dswizard-components-0.2.1/requirements.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)       38 2022-03-01 13:12:55.359944 dswizard-components-0.2.1/setup.cfg
--rw-rw-r--   0 marc      (1000) marc      (1000)     1335 2022-03-01 13:07:41.000000 dswizard-components-0.2.1/setup.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-06-29 08:23:44.320314 dswizard-components-0.2.2/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      116 2022-02-18 14:55:46.000000 dswizard-components-0.2.2/MANIFEST.in
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1082 2022-06-29 08:23:44.316314 dswizard-components-0.2.2/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)      451 2021-04-17 12:01:34.000000 dswizard-components-0.2.2/README.md
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-06-29 08:23:44.304314 dswizard-components-0.2.2/dswizard/
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-06-29 08:23:44.304314 dswizard-components-0.2.2/dswizard/components/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      137 2022-01-04 14:54:30.000000 dswizard-components-0.2.2/dswizard/components/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    18814 2022-03-01 08:51:46.000000 dswizard-components-0.2.2/dswizard/components/base.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-06-29 08:23:44.308314 dswizard-components-0.2.2/dswizard/components/classification/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1556 2022-01-04 15:27:16.000000 dswizard-components-0.2.2/dswizard/components/classification/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2151 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/classification/ada_boosting.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2463 2021-11-12 13:01:57.000000 dswizard-components-0.2.2/dswizard/components/classification/bernoulli_nb.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5099 2021-11-19 17:14:02.000000 dswizard-components-0.2.2/dswizard/components/classification/decision_tree.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-06-29 08:23:44.312314 dswizard-components-0.2.2/dswizard/components/classification/excluded/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2021-04-17 12:01:34.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5887 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/extra_trees.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1997 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/gaussian_nb.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4016 2021-11-19 17:14:46.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/gaussian_process.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2920 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/k_neighbors.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6105 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/logistic_regression.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     8366 2022-03-01 08:45:45.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/mlp_classifier.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4115 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/passive_aggressive.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2172 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/qda.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4670 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/classification/excluded/svm.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5407 2021-11-19 17:14:02.000000 dswizard-components-0.2.2/dswizard/components/classification/gradient_boosting.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4391 2022-01-03 07:59:18.000000 dswizard-components-0.2.2/dswizard/components/classification/libsvm_svc.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3168 2021-11-12 13:03:17.000000 dswizard-components-0.2.2/dswizard/components/classification/linear_discriminant_analysis.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2413 2021-11-12 13:02:50.000000 dswizard-components-0.2.2/dswizard/components/classification/multinomial_nb.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5031 2021-11-19 17:14:02.000000 dswizard-components-0.2.2/dswizard/components/classification/random_forest.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5600 2022-01-03 18:47:13.000000 dswizard-components-0.2.2/dswizard/components/classification/sgd.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-06-29 08:23:44.312314 dswizard-components-0.2.2/dswizard/components/data_preprocessing/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      996 2022-01-04 15:27:16.000000 dswizard-components-0.2.2/dswizard/components/data_preprocessing/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4455 2022-03-01 10:47:00.000000 dswizard-components-0.2.2/dswizard/components/data_preprocessing/imputation.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2864 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/data_preprocessing/knn_imputer.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1003 2021-08-01 09:02:57.000000 dswizard-components-0.2.2/dswizard/components/data_preprocessing/max_abs_scaler.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      995 2021-08-01 09:02:57.000000 dswizard-components-0.2.2/dswizard/components/data_preprocessing/minmax.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1272 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/data_preprocessing/normalize.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2180 2021-08-01 09:02:57.000000 dswizard-components-0.2.2/dswizard/components/data_preprocessing/quantile_transformer.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1799 2022-03-01 08:56:00.000000 dswizard-components-0.2.2/dswizard/components/data_preprocessing/robust_scaler.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1177 2021-11-13 14:55:20.000000 dswizard-components-0.2.2/dswizard/components/data_preprocessing/standard_scaler.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-06-29 08:23:44.316314 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1025 2022-01-04 15:27:16.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2227 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/bernoulli_rbm.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1603 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/binarizer.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3023 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/factor_analysis.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2878 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/fast_ica.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3928 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/feature_agglomeration.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2917 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/generic_univariate_select.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2075 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/kbinsdiscretizer.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4820 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/kpca.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1965 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/missing_indicator.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1907 2022-03-01 08:15:46.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/one_hot_encoding.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2221 2022-03-01 08:20:08.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/ordinal_encoder.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2651 2022-03-01 08:20:08.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/pca.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2099 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/polynomial.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4743 2022-03-01 08:20:08.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/random_trees_embedding.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3039 2021-06-30 08:10:47.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/select_k_best.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3927 2021-11-12 13:09:16.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/select_percentile.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2370 2022-03-01 08:20:08.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/truncated_svd.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1632 2022-01-09 20:29:09.000000 dswizard-components-0.2.2/dswizard/components/feature_preprocessing/variance_threshold.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    12093 2022-03-01 08:45:09.000000 dswizard-components-0.2.2/dswizard/components/meta_features.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4055 2022-03-01 08:25:03.000000 dswizard-components-0.2.2/dswizard/components/pipeline.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7083 2022-03-01 08:37:36.000000 dswizard-components-0.2.2/dswizard/components/sklearn.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3553 2022-03-01 09:02:16.000000 dswizard-components-0.2.2/dswizard/components/util.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-06-29 08:23:44.316314 dswizard-components-0.2.2/dswizard/pynisher2/
+-rw-rw-r--   0 marc      (1000) marc      (1000)       53 2022-01-04 09:23:52.000000 dswizard-components-0.2.2/dswizard/pynisher2/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    12330 2022-03-01 09:45:21.000000 dswizard-components-0.2.2/dswizard/pynisher2/limit_function_call.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-06-29 08:23:44.316314 dswizard-components-0.2.2/dswizard_components.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1082 2022-06-29 08:23:44.000000 dswizard-components-0.2.2/dswizard_components.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3266 2022-06-29 08:23:44.000000 dswizard-components-0.2.2/dswizard_components.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)        1 2022-06-29 08:23:44.000000 dswizard-components-0.2.2/dswizard_components.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)      115 2022-06-29 08:23:44.000000 dswizard-components-0.2.2/dswizard_components.egg-info/requires.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)        9 2022-06-29 08:23:44.000000 dswizard-components-0.2.2/dswizard_components.egg-info/top_level.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)      114 2022-04-08 06:29:22.000000 dswizard-components-0.2.2/requirements.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)       38 2022-06-29 08:23:44.320314 dswizard-components-0.2.2/setup.cfg
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1441 2022-06-29 08:19:54.000000 dswizard-components-0.2.2/setup.py
```

### Comparing `dswizard-components-0.2.1/PKG-INFO` & `dswizard-components-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: dswizard-components
-Version: 0.2.1
+Version: 0.2.2
 Summary: Contains all base algorithms used by dswizard
 Home-page: https://github.com/Ennosigaeon/dswizard-components
 Author: Marc Zoeller
 Author-email: m.zoeller@usu.de
 License: MIT
 Keywords: automl,machine learning,pipeline synthesis
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # dswizard-components
 
 [_dswizard_](https://github.com/Ennosigaeon/dswizzard) is an efficient solver for machine learning (ML) pipeline
 synthesis inspired by human behaviour. It automatically derives a pipeline structure, selects algorithms and performs
 hyperparameter optimization. This repository contains all _basic_ algorithms that can be optimized by _dswizard_. For
```

### Comparing `dswizard-components-0.2.1/dswizard/components/base.py` & `dswizard-components-0.2.2/dswizard/components/base.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/__init__.py` & `dswizard-components-0.2.2/dswizard/components/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/ada_boosting.py` & `dswizard-components-0.2.2/dswizard/components/classification/ada_boosting.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/bernoulli_nb.py` & `dswizard-components-0.2.2/dswizard/components/classification/bernoulli_nb.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/decision_tree.py` & `dswizard-components-0.2.2/dswizard/components/classification/decision_tree.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/excluded/extra_trees.py` & `dswizard-components-0.2.2/dswizard/components/classification/excluded/extra_trees.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/excluded/gaussian_nb.py` & `dswizard-components-0.2.2/dswizard/components/classification/excluded/gaussian_nb.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/excluded/gaussian_process.py` & `dswizard-components-0.2.2/dswizard/components/classification/excluded/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/excluded/k_neighbors.py` & `dswizard-components-0.2.2/dswizard/components/classification/excluded/k_neighbors.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/excluded/logistic_regression.py` & `dswizard-components-0.2.2/dswizard/components/classification/excluded/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/excluded/mlp_classifier.py` & `dswizard-components-0.2.2/dswizard/components/classification/excluded/mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/excluded/passive_aggressive.py` & `dswizard-components-0.2.2/dswizard/components/classification/excluded/passive_aggressive.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/excluded/qda.py` & `dswizard-components-0.2.2/dswizard/components/classification/excluded/qda.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/excluded/svm.py` & `dswizard-components-0.2.2/dswizard/components/classification/excluded/svm.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/gradient_boosting.py` & `dswizard-components-0.2.2/dswizard/components/classification/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/libsvm_svc.py` & `dswizard-components-0.2.2/dswizard/components/classification/libsvm_svc.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/linear_discriminant_analysis.py` & `dswizard-components-0.2.2/dswizard/components/classification/linear_discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/multinomial_nb.py` & `dswizard-components-0.2.2/dswizard/components/classification/multinomial_nb.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/random_forest.py` & `dswizard-components-0.2.2/dswizard/components/classification/random_forest.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/classification/sgd.py` & `dswizard-components-0.2.2/dswizard/components/classification/sgd.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/data_preprocessing/__init__.py` & `dswizard-components-0.2.2/dswizard/components/data_preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/data_preprocessing/imputation.py` & `dswizard-components-0.2.2/dswizard/components/data_preprocessing/imputation.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/data_preprocessing/knn_imputer.py` & `dswizard-components-0.2.2/dswizard/components/data_preprocessing/knn_imputer.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/data_preprocessing/max_abs_scaler.py` & `dswizard-components-0.2.2/dswizard/components/data_preprocessing/max_abs_scaler.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/data_preprocessing/minmax.py` & `dswizard-components-0.2.2/dswizard/components/data_preprocessing/minmax.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/data_preprocessing/normalize.py` & `dswizard-components-0.2.2/dswizard/components/data_preprocessing/normalize.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/data_preprocessing/quantile_transformer.py` & `dswizard-components-0.2.2/dswizard/components/data_preprocessing/quantile_transformer.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/data_preprocessing/robust_scaler.py` & `dswizard-components-0.2.2/dswizard/components/data_preprocessing/robust_scaler.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/data_preprocessing/standard_scaler.py` & `dswizard-components-0.2.2/dswizard/components/data_preprocessing/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/__init__.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/bernoulli_rbm.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/bernoulli_rbm.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/binarizer.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/binarizer.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/factor_analysis.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/factor_analysis.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/fast_ica.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/fast_ica.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/feature_agglomeration.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/feature_agglomeration.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/generic_univariate_select.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/generic_univariate_select.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/kbinsdiscretizer.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/kbinsdiscretizer.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/kpca.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/kpca.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/missing_indicator.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/missing_indicator.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/one_hot_encoding.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/ordinal_encoder.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/pca.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/pca.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/polynomial.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/polynomial.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/random_trees_embedding.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/random_trees_embedding.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/select_k_best.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/select_k_best.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/select_percentile.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/select_percentile.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/truncated_svd.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/truncated_svd.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/feature_preprocessing/variance_threshold.py` & `dswizard-components-0.2.2/dswizard/components/feature_preprocessing/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/meta_features.py` & `dswizard-components-0.2.2/dswizard/components/meta_features.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/pipeline.py` & `dswizard-components-0.2.2/dswizard/components/pipeline.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/sklearn.py` & `dswizard-components-0.2.2/dswizard/components/sklearn.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/components/util.py` & `dswizard-components-0.2.2/dswizard/components/util.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard/pynisher2/limit_function_call.py` & `dswizard-components-0.2.2/dswizard/pynisher2/limit_function_call.py`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/dswizard_components.egg-info/PKG-INFO` & `dswizard-components-0.2.2/dswizard_components.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: dswizard-components
-Version: 0.2.1
+Version: 0.2.2
 Summary: Contains all base algorithms used by dswizard
 Home-page: https://github.com/Ennosigaeon/dswizard-components
 Author: Marc Zoeller
 Author-email: m.zoeller@usu.de
 License: MIT
 Keywords: automl,machine learning,pipeline synthesis
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # dswizard-components
 
 [_dswizard_](https://github.com/Ennosigaeon/dswizzard) is an efficient solver for machine learning (ML) pipeline
 synthesis inspired by human behaviour. It automatically derives a pipeline structure, selects algorithms and performs
 hyperparameter optimization. This repository contains all _basic_ algorithms that can be optimized by _dswizard_. For
```

### Comparing `dswizard-components-0.2.1/dswizard_components.egg-info/SOURCES.txt` & `dswizard-components-0.2.2/dswizard_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dswizard-components-0.2.1/setup.py` & `dswizard-components-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,26 +18,28 @@
 
 # The text of the README file
 README = (pathlib.Path(__file__).parent / 'README.md').read_text()
 
 if __name__ == '__main__':
     setup(
         name='dswizard-components',
-        version='0.2.1',
+        version='0.2.2',
         description='Contains all base algorithms used by dswizard',
         long_description=README,
         long_description_content_type='text/markdown',
         author='Marc Zoeller',
         author_email='m.zoeller@usu.de',
         url='https://github.com/Ennosigaeon/dswizard-components',
         license='MIT',
         classifiers=[
             'License :: OSI Approved :: MIT License',
             'Programming Language :: Python :: 3',
-            'Programming Language :: Python :: 3.5'
+            'Programming Language :: Python :: 3.7',
+            'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9'
         ],
         packages=find_namespace_packages(include=['dswizard.*']),
-        python_requires='>=3.5',
+        python_requires='>=3.7',
         include_package_data=True,
         install_requires=requirements,
         keywords=['automl', 'machine learning', 'pipeline synthesis']
     )
```

