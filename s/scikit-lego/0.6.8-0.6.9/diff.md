# Comparing `tmp/scikit-lego-0.6.8.tar.gz` & `tmp/scikit-lego-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-lego-0.6.8.tar", last modified: Sat Jul  3 12:38:32 2021, max compression
+gzip compressed data, was "dist/scikit-lego-0.6.9.tar", last modified: Thu Dec  9 11:38:50 2021, max compression
```

## Comparing `scikit-lego-0.6.8.tar` & `scikit-lego-0.6.9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10133 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/PKG-INFO
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/scikit_lego.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10133 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/scikit_lego.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4318 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/scikit_lego.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/scikit_lego.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      759 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/scikit_lego.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       13 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/scikit_lego.egg-info/top_level.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2073 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/sklego/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       22 2021-07-03 12:38:16.000000 scikit-lego-0.6.8/sklego/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/base.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5031 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/common.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/sklego/data/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    59235 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/data/abalone.zip
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    18826 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/data/arrests.zip
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2108 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/data/chickweight.zip
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3620 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/data/hearts.zip
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1340 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/data/heroes.zip
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2974 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/data/penguins.zip
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    17379 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/datasets.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/sklego/decomposition/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      165 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/decomposition/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3153 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/decomposition/pca_reconstruction.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3002 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/decomposition/umap_reconstruction.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2375 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/dummy.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    34236 2021-07-03 12:38:16.000000 scikit-lego-0.6.8/sklego/linear_model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/sklego/meta/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      930 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/meta/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3494 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/meta/_grouped_utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3105 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/meta/confusion_balancer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2326 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/meta/decay_estimator.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1271 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/meta/estimator_transformer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      346 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/meta/grouped_estimator.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    12689 2021-07-03 12:38:16.000000 scikit-lego-0.6.8/sklego/meta/grouped_predictor.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5524 2021-06-04 09:27:19.000000 scikit-lego-0.6.8/sklego/meta/grouped_transformer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2733 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/meta/outlier_classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1320 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/meta/outlier_remover.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3711 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/meta/regression_outlier_detector.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6775 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/meta/subjective_classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2781 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/meta/thresholder.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4930 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/meta/zero_inflated_regressor.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8028 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/metrics.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/sklego/mixture/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      340 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/mixture/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4227 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/mixture/bayesian_gmm_classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6496 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/mixture/bayesian_gmm_detector.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3552 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/mixture/gmm_classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5647 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/mixture/gmm_outlier_detector.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10001 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8569 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/naive_bayes.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3725 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/neighbors.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1592 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/notinstalled.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     8879 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/pandas_utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13472 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/pipeline.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/sklego/preprocessing/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      820 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/preprocessing/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7203 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/preprocessing/columncapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2164 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/preprocessing/dictmapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      905 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/preprocessing/identitytransformer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6440 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/preprocessing/intervalencoder.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1101 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/preprocessing/outlier_remover.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     9482 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/preprocessing/pandastransformers.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1666 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/preprocessing/patsytransformer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6186 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/preprocessing/projections.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      831 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/sklego/preprocessing/randomadder.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5460 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/preprocessing/repeatingbasis.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1388 2020-12-22 21:02:23.000000 scikit-lego-0.6.8/sklego/testing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1141 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/sklego/this.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/tests/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4892 2021-07-03 12:38:16.000000 scikit-lego-0.6.8/tests/conftest.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/tests/test_common/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_common/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      402 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_common/test_basics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3408 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_common/test_transformerselectormixin.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1401 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_datasets.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/tests/test_estimators/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_estimators/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1637 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_estimators/test_basics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      915 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_estimators/test_deadzone.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4391 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_demographic_parity.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3901 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_equal_opportunity.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1428 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_gmm_naive_bayes.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4099 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_imbalanced_linear_regression.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3156 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_lad_regression.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      739 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_lowess.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      964 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_mixture_classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4150 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_mixture_detector.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1028 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_neighbor_classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1072 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_pca_reconstruction.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1101 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_probweight_regression.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3818 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_quantile_regression.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1837 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_estimators/test_randomregressor.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1325 2021-07-03 12:38:16.000000 scikit-lego-0.6.8/tests/test_estimators/test_umap_reconstruction.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/tests/test_meta/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_meta/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      974 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_meta/test_confusion_balancer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1950 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_decay_estimator.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2072 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_estimatortransformer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    15125 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_grouped_predictor.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10438 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_grouped_transformer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2092 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_outlier_classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2904 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_outlier_remover.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2111 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_regression_outlier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6628 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_subjective_classifier.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2882 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_thresholder.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2672 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_meta/test_zero_inflated_regressor.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/tests/test_metrics/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_metrics/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      904 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_metrics/test_correlation_score.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2850 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_metrics/test_equal_opportunity.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1813 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_metrics/test_p_percent.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3941 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_metrics/test_subset_metric.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/tests/test_model_selection/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_model_selection/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2088 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_model_selection/test_klusterfold.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4875 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_model_selection/test_timegapsplit.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      784 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_notinstalled.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-07-03 12:38:32.000000 scikit-lego-0.6.8/tests/test_preprocessing/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_preprocessing/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3880 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_columncapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2098 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_columndropper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1700 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_columnselector.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1801 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_dictmapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      701 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_identitytransformer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3597 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_informationfilter.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3505 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_interval_encoder.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2845 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_orthogonal_transformer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3264 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_outlier_remover.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2805 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_pandastypeselector.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3806 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_patsy_transformer.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1371 2021-06-04 09:27:25.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_randomadder.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1692 2020-12-22 20:59:42.000000 scikit-lego-0.6.8/tests/test_preprocessing/test_repeatingbasisfunction.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10133 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/PKG-INFO
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/scikit_lego.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10133 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/scikit_lego.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4318 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/scikit_lego.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/scikit_lego.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      759 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/scikit_lego.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       13 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/scikit_lego.egg-info/top_level.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2073 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/sklego/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       22 2021-12-09 11:35:08.000000 scikit-lego-0.6.9/sklego/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/base.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5031 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/common.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/sklego/data/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    59235 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/data/abalone.zip
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    18826 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/data/arrests.zip
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2108 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/data/chickweight.zip
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3620 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/data/hearts.zip
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1340 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/data/heroes.zip
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2974 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/data/penguins.zip
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    17379 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/datasets.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/sklego/decomposition/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      165 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/decomposition/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3153 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/decomposition/pca_reconstruction.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3002 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/decomposition/umap_reconstruction.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2375 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/dummy.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    34236 2021-07-03 12:38:16.000000 scikit-lego-0.6.9/sklego/linear_model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/sklego/meta/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      930 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/meta/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3494 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/meta/_grouped_utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3105 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/meta/confusion_balancer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2326 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/meta/decay_estimator.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1271 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/meta/estimator_transformer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      346 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/meta/grouped_estimator.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    12689 2021-07-03 12:38:16.000000 scikit-lego-0.6.9/sklego/meta/grouped_predictor.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5524 2021-06-04 09:27:19.000000 scikit-lego-0.6.9/sklego/meta/grouped_transformer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2733 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/meta/outlier_classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1320 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/meta/outlier_remover.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3711 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/meta/regression_outlier_detector.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6775 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/meta/subjective_classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2990 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/sklego/meta/thresholder.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4930 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/meta/zero_inflated_regressor.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     8028 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/metrics.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/sklego/mixture/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      340 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/mixture/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4227 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/mixture/bayesian_gmm_classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6496 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/mixture/bayesian_gmm_detector.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3552 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/mixture/gmm_classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5647 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/mixture/gmm_outlier_detector.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10001 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     8569 2021-08-05 09:33:23.000000 scikit-lego-0.6.9/sklego/naive_bayes.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3725 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/neighbors.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1592 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/notinstalled.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     9426 2021-12-09 11:35:08.000000 scikit-lego-0.6.9/sklego/pandas_utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13472 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/pipeline.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/sklego/preprocessing/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      820 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/preprocessing/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     7203 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/preprocessing/columncapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2164 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/preprocessing/dictmapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      905 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/preprocessing/identitytransformer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6440 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/preprocessing/intervalencoder.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1101 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/preprocessing/outlier_remover.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     9482 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/preprocessing/pandastransformers.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1666 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/preprocessing/patsytransformer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6186 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/preprocessing/projections.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      831 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/sklego/preprocessing/randomadder.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5460 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/preprocessing/repeatingbasis.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1388 2020-12-22 21:02:23.000000 scikit-lego-0.6.9/sklego/testing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1141 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/sklego/this.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/tests/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4892 2021-07-03 12:38:16.000000 scikit-lego-0.6.9/tests/conftest.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/tests/test_common/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_common/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      402 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_common/test_basics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3408 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_common/test_transformerselectormixin.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1401 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_datasets.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/tests/test_estimators/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_estimators/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1637 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_estimators/test_basics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      915 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_estimators/test_deadzone.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4481 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_demographic_parity.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3991 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_equal_opportunity.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1518 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_gmm_naive_bayes.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4099 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_estimators/test_imbalanced_linear_regression.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3156 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_estimators/test_lad_regression.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      829 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_lowess.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1054 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_mixture_classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4241 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_mixture_detector.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1118 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_neighbor_classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1163 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_pca_reconstruction.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1191 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_probweight_regression.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3818 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_estimators/test_quantile_regression.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1928 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_randomregressor.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1416 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_estimators/test_umap_reconstruction.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/tests/test_meta/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_meta/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      974 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_meta/test_confusion_balancer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1950 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_meta/test_decay_estimator.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2072 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_meta/test_estimatortransformer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    15293 2021-12-09 11:35:08.000000 scikit-lego-0.6.9/tests/test_meta/test_grouped_predictor.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10438 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_meta/test_grouped_transformer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2092 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_meta/test_outlier_classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2904 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_meta/test_outlier_remover.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2111 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_meta/test_regression_outlier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6628 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_meta/test_subjective_classifier.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3393 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_meta/test_thresholder.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2672 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_meta/test_zero_inflated_regressor.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/tests/test_metrics/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_metrics/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      904 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_metrics/test_correlation_score.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2850 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_metrics/test_equal_opportunity.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1813 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_metrics/test_p_percent.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3941 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_metrics/test_subset_metric.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/tests/test_model_selection/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_model_selection/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2088 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_model_selection/test_klusterfold.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4875 2021-06-04 09:27:25.000000 scikit-lego-0.6.9/tests/test_model_selection/test_timegapsplit.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      784 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_notinstalled.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2021-12-09 11:38:50.000000 scikit-lego-0.6.9/tests/test_preprocessing/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_preprocessing/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3971 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_columncapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2098 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_columndropper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1700 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_columnselector.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1892 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_dictmapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      791 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_identitytransformer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3688 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_informationfilter.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3509 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_interval_encoder.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2935 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_orthogonal_transformer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3264 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_outlier_remover.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2805 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_pandastypeselector.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3806 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_patsy_transformer.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1462 2021-11-30 08:51:18.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_randomadder.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1692 2020-12-22 20:59:42.000000 scikit-lego-0.6.9/tests/test_preprocessing/test_repeatingbasisfunction.py
```

### Comparing `scikit-lego-0.6.8/PKG-INFO` & `scikit-lego-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-lego
-Version: 0.6.8
+Version: 0.6.9
 Summary: a collection of lego bricks for scikit-learn pipelines
 Home-page: https://scikit-lego.netlify.app/
 Author: Vincent D. Warmerdam & Matthijs Brouns
 License: UNKNOWN
 Description: [![Build status](https://github.com/koaning/scikit-lego/workflows/Unit%20Tests/badge.svg)](https://github.com/{github_id}/{repository}/workflows/{workflow_name}/badge.svg)
         [![Downloads](https://pepy.tech/badge/scikit-lego/month)](https://pepy.tech/project/scikit-lego)
         [![Version](https://img.shields.io/pypi/v/scikit-lego)](https://pypi.org/project/scikit-lego/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scikit-lego Version: 0.6.8 Summary: a collection of
+Metadata-Version: 2.1 Name: scikit-lego Version: 0.6.9 Summary: a collection of
 lego bricks for scikit-learn pipelines Home-page: https://scikit-
 lego.netlify.app/ Author: Vincent D. Warmerdam & Matthijs Brouns License:
 UNKNOWN Description: [![Build status](https://github.com/koaning/scikit-lego/
 workflows/Unit%20Tests/badge.svg)](https://github.com/{github_id}/{repository}/
 workflows/{workflow_name}/badge.svg) [![Downloads](https://pepy.tech/badge/
 scikit-lego/month)](https://pepy.tech/project/scikit-lego) [![Version](https://
 img.shields.io/pypi/v/scikit-lego)](https://pypi.org/project/scikit-lego/) [!
```

### Comparing `scikit-lego-0.6.8/scikit_lego.egg-info/PKG-INFO` & `scikit-lego-0.6.9/scikit_lego.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-lego
-Version: 0.6.8
+Version: 0.6.9
 Summary: a collection of lego bricks for scikit-learn pipelines
 Home-page: https://scikit-lego.netlify.app/
 Author: Vincent D. Warmerdam & Matthijs Brouns
 License: UNKNOWN
 Description: [![Build status](https://github.com/koaning/scikit-lego/workflows/Unit%20Tests/badge.svg)](https://github.com/{github_id}/{repository}/workflows/{workflow_name}/badge.svg)
         [![Downloads](https://pepy.tech/badge/scikit-lego/month)](https://pepy.tech/project/scikit-lego)
         [![Version](https://img.shields.io/pypi/v/scikit-lego)](https://pypi.org/project/scikit-lego/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scikit-lego Version: 0.6.8 Summary: a collection of
+Metadata-Version: 2.1 Name: scikit-lego Version: 0.6.9 Summary: a collection of
 lego bricks for scikit-learn pipelines Home-page: https://scikit-
 lego.netlify.app/ Author: Vincent D. Warmerdam & Matthijs Brouns License:
 UNKNOWN Description: [![Build status](https://github.com/koaning/scikit-lego/
 workflows/Unit%20Tests/badge.svg)](https://github.com/{github_id}/{repository}/
 workflows/{workflow_name}/badge.svg) [![Downloads](https://pepy.tech/badge/
 scikit-lego/month)](https://pepy.tech/project/scikit-lego) [![Version](https://
 img.shields.io/pypi/v/scikit-lego)](https://pypi.org/project/scikit-lego/) [!
```

### Comparing `scikit-lego-0.6.8/scikit_lego.egg-info/SOURCES.txt` & `scikit-lego-0.6.9/scikit_lego.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/scikit_lego.egg-info/requires.txt` & `scikit-lego-0.6.9/scikit_lego.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/setup.py` & `scikit-lego-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/base.py` & `scikit-lego-0.6.9/sklego/base.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/common.py` & `scikit-lego-0.6.9/sklego/common.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/data/abalone.zip` & `scikit-lego-0.6.9/sklego/data/abalone.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/data/arrests.zip` & `scikit-lego-0.6.9/sklego/data/arrests.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/data/chickweight.zip` & `scikit-lego-0.6.9/sklego/data/chickweight.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/data/hearts.zip` & `scikit-lego-0.6.9/sklego/data/hearts.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/data/heroes.zip` & `scikit-lego-0.6.9/sklego/data/heroes.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/data/penguins.zip` & `scikit-lego-0.6.9/sklego/data/penguins.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/datasets.py` & `scikit-lego-0.6.9/sklego/datasets.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/decomposition/pca_reconstruction.py` & `scikit-lego-0.6.9/sklego/decomposition/pca_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/decomposition/umap_reconstruction.py` & `scikit-lego-0.6.9/sklego/decomposition/umap_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/dummy.py` & `scikit-lego-0.6.9/sklego/dummy.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/linear_model.py` & `scikit-lego-0.6.9/sklego/linear_model.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/__init__.py` & `scikit-lego-0.6.9/sklego/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/_grouped_utils.py` & `scikit-lego-0.6.9/sklego/meta/_grouped_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/confusion_balancer.py` & `scikit-lego-0.6.9/sklego/meta/confusion_balancer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/decay_estimator.py` & `scikit-lego-0.6.9/sklego/meta/decay_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/estimator_transformer.py` & `scikit-lego-0.6.9/sklego/meta/estimator_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/grouped_predictor.py` & `scikit-lego-0.6.9/sklego/meta/grouped_predictor.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/grouped_transformer.py` & `scikit-lego-0.6.9/sklego/meta/grouped_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/outlier_classifier.py` & `scikit-lego-0.6.9/sklego/meta/outlier_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/outlier_remover.py` & `scikit-lego-0.6.9/sklego/meta/outlier_remover.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/regression_outlier_detector.py` & `scikit-lego-0.6.9/sklego/meta/regression_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/subjective_classifier.py` & `scikit-lego-0.6.9/sklego/meta/subjective_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/meta/thresholder.py` & `scikit-lego-0.6.9/sklego/meta/thresholder.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,39 +27,40 @@
     """
 
     def __init__(self, model, threshold: float, refit=False):
         self.model = model
         self.threshold = threshold
         self.refit = refit
 
-    def _handle_refit(self, X, y):
+    def _handle_refit(self, X, y, sample_weight=None):
         """Only refit when we need to, unless refit=True is present."""
         if self.refit:
-            self.estimator_.fit(X, y)
+            self.estimator_.fit(X, y, sample_weight=sample_weight)
         else:
             try:
                 _ = self.estimator_.predict(X[:1])
             except NotFittedError:
-                self.estimator_.fit(X, y)
+                self.estimator_.fit(X, y, sample_weight=sample_weight)
 
-    def fit(self, X, y):
+    def fit(self, X, y, sample_weight=None):
         """
         Fit the data.
 
         :param X: array-like, shape=(n_columns, n_samples,) training data.
         :param y: array-like, shape=(n_samples,) training data.
+        :param sample_weight: array-like, shape=(n_samples) Individual weights for each sample.
         :return: Returns an instance of self.
         """
         X, y = check_X_y(X, y, estimator=self, dtype=FLOAT_DTYPES)
         self.estimator_ = clone(self.model)
         if not isinstance(self.estimator_, ProbabilisticClassifier):
             raise ValueError(
                 "The Thresholder meta model only works on classifcation models with .predict_proba."
             )
-        self._handle_refit(X, y)
+        self._handle_refit(X, y, sample_weight)
         self.classes_ = self.estimator_.classes_
         if len(self.classes_) != 2:
             raise ValueError(
                 "The Thresholder meta model only works on models with two classes."
             )
         return self
```

### Comparing `scikit-lego-0.6.8/sklego/meta/zero_inflated_regressor.py` & `scikit-lego-0.6.9/sklego/meta/zero_inflated_regressor.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/metrics.py` & `scikit-lego-0.6.9/sklego/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/mixture/bayesian_gmm_classifier.py` & `scikit-lego-0.6.9/sklego/mixture/bayesian_gmm_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/mixture/bayesian_gmm_detector.py` & `scikit-lego-0.6.9/sklego/mixture/bayesian_gmm_detector.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/mixture/gmm_classifier.py` & `scikit-lego-0.6.9/sklego/mixture/gmm_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/mixture/gmm_outlier_detector.py` & `scikit-lego-0.6.9/sklego/mixture/gmm_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/model_selection.py` & `scikit-lego-0.6.9/sklego/model_selection.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/naive_bayes.py` & `scikit-lego-0.6.9/sklego/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/neighbors.py` & `scikit-lego-0.6.9/sklego/neighbors.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/notinstalled.py` & `scikit-lego-0.6.9/sklego/notinstalled.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/pandas_utils.py` & `scikit-lego-0.6.9/sklego/pandas_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import datetime as dt
 import inspect
+from functools import partial, wraps
 
 import numpy as np
 import pandas as pd
-import datetime as dt
+from scipy.ndimage.interpolation import shift
 
-from functools import wraps, partial
 from sklego.common import as_list
-from scipy.ndimage.interpolation import shift
 
 
 def _get_shape_delta(old_shape, new_shape):
     diffs = [
         ("+" if new > old else "") + str(new - old)
         for new, old in zip(new_shape, old_shape)
     ]
@@ -23,27 +23,29 @@
     *,
     time_taken=True,
     shape=True,
     shape_delta=False,
     names=False,
     dtypes=False,
     print_fn=print,
-    display_args=True
+    display_args=True,
+    log_error=True,
 ):
     """
     Decorates a function that transforms a pandas dataframe to add automated logging statements
 
     :param func: callable, function to log, defaults to None
     :param time_taken: bool, log the time it took to run a function, defaults to True
     :param shape: bool, log the shape of the output result, defaults to True
     :param shape_delta: bool, log the difference in shape of input and output, defaults to False
     :param names: bool, log the names of the columns of the result, defaults to False
     :param dtypes: bool, log the dtypes of the results, defaults to False
     :param print_fn: callable, print function (e.g. print or logger.info), defaults to print
     :param print_args: bool, whether or not to print the arguments given to the function.
+    :param log_error: bool, whether to add the Exception message to the log if the function fails, defaults to True.
     :returns: the result of the function
 
     :Example:
     >>> @log_step
     ... def remove_outliers(df, min_obs=5):
     ...     pass
 
@@ -58,47 +60,55 @@
             log_step,
             time_taken=time_taken,
             shape=shape,
             shape_delta=shape_delta,
             names=names,
             dtypes=dtypes,
             print_fn=print_fn,
-            display_args=display_args
+            display_args=display_args,
+            log_error=log_error,
         )
 
     names = False if dtypes else names
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         if shape_delta:
             old_shape = args[0].shape
         tic = dt.datetime.now()
 
-        result = func(*args, **kwargs)
-
-        optional_strings = [
-            f"time={dt.datetime.now() - tic}" if time_taken else None,
-            f"n_obs={result.shape[0]}, n_col={result.shape[1]}" if shape else None,
-            _get_shape_delta(old_shape, result.shape) if shape_delta else None,
-            f"names={result.columns.to_list()}" if names else None,
-            f"dtypes={result.dtypes.to_dict()}" if dtypes else None,
-        ]
-
-        combined = " ".join([s for s in optional_strings if s])
-
-        if display_args:
-
-            func_args = inspect.signature(func).bind(*args, **kwargs).arguments
-            func_args_str = "".join(
-                ", {} = {!r}".format(*item) for item in list(func_args.items())[1:]
-            )
-            print_fn(f"[{func.__name__}(df{func_args_str})] " + combined,)
-        else:
-            print_fn(f"[{func.__name__}]" + combined,)
-        return result
+        optional_strings = []
+        try:
+            result = func(*args, **kwargs)
+            optional_strings = [
+                f"time={dt.datetime.now() - tic}" if time_taken else None,
+                f"n_obs={result.shape[0]}, n_col={result.shape[1]}" if shape else None,
+                _get_shape_delta(old_shape, result.shape) if shape_delta else None,
+                f"names={result.columns.to_list()}" if names else None,
+                f"dtypes={result.dtypes.to_dict()}" if dtypes else None,
+            ]
+            return result
+        except Exception as exc:
+            optional_strings = [
+                f"time={dt.datetime.now() - tic}" if time_taken else None,
+                "FAILED" + (f" with error: {exc}" if log_error else "")
+            ]
+            raise
+        finally:
+            combined = " ".join([s for s in optional_strings if s])
+
+            if display_args:
+
+                func_args = inspect.signature(func).bind(*args, **kwargs).arguments
+                func_args_str = "".join(
+                    ", {} = {!r}".format(*item) for item in list(func_args.items())[1:]
+                )
+                print_fn(f"[{func.__name__}(df{func_args_str})] " + combined,)
+            else:
+                print_fn(f"[{func.__name__}]" + combined,)
 
     return wrapper
 
 
 def log_step_extra(
     *log_functions, print_fn=print, **log_func_kwargs,
 ):
```

### Comparing `scikit-lego-0.6.8/sklego/pipeline.py` & `scikit-lego-0.6.9/sklego/pipeline.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/__init__.py` & `scikit-lego-0.6.9/sklego/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/columncapper.py` & `scikit-lego-0.6.9/sklego/preprocessing/columncapper.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/dictmapper.py` & `scikit-lego-0.6.9/sklego/preprocessing/dictmapper.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/identitytransformer.py` & `scikit-lego-0.6.9/sklego/preprocessing/identitytransformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/intervalencoder.py` & `scikit-lego-0.6.9/sklego/preprocessing/intervalencoder.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/outlier_remover.py` & `scikit-lego-0.6.9/sklego/preprocessing/outlier_remover.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/pandastransformers.py` & `scikit-lego-0.6.9/sklego/preprocessing/pandastransformers.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/patsytransformer.py` & `scikit-lego-0.6.9/sklego/preprocessing/patsytransformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/projections.py` & `scikit-lego-0.6.9/sklego/preprocessing/projections.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/randomadder.py` & `scikit-lego-0.6.9/sklego/preprocessing/randomadder.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/preprocessing/repeatingbasis.py` & `scikit-lego-0.6.9/sklego/preprocessing/repeatingbasis.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/testing.py` & `scikit-lego-0.6.9/sklego/testing.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/sklego/this.py` & `scikit-lego-0.6.9/sklego/this.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/conftest.py` & `scikit-lego-0.6.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_common/test_transformerselectormixin.py` & `scikit-lego-0.6.9/tests/test_common/test_transformerselectormixin.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_datasets.py` & `scikit-lego-0.6.9/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_basics.py` & `scikit-lego-0.6.9/tests/test_estimators/test_basics.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_deadzone.py` & `scikit-lego-0.6.9/tests/test_estimators/test_deadzone.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_demographic_parity.py` & `scikit-lego-0.6.9/tests/test_estimators/test_demographic_parity.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, classifier_checks]),
         exclude=[
             "check_sample_weights_invariance",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 @pytest.mark.cvxpy
 def test_standard_checks(test_fn):
     trf = DemographicParityClassifier(
         covariance_threshold=None,
```

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_equal_opportunity.py` & `scikit-lego-0.6.9/tests/test_estimators/test_equal_opportunity.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, classifier_checks]),
         exclude=[
             "check_sample_weights_invariance",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 @pytest.mark.cvxpy
 def test_standard_checks(test_fn):
     trf = EqualOpportunityClassifier(
         covariance_threshold=None,
```

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_gmm_naive_bayes.py` & `scikit-lego-0.6.9/tests/test_estimators/test_gmm_naive_bayes.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks]),
         exclude=[
             "check_sample_weights_invariance",
             "check_non_transformer_estimators_n_iter",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     clf1 = GaussianMixtureNB()
     clf2 = GaussianMixtureNB(n_components=2)
     clf3 = BayesianGaussianMixtureNB()
```

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_imbalanced_linear_regression.py` & `scikit-lego-0.6.9/tests/test_estimators/test_imbalanced_linear_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_lad_regression.py` & `scikit-lego-0.6.9/tests/test_estimators/test_lad_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_lowess.py` & `scikit-lego-0.6.9/tests/test_estimators/test_lowess.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, regressor_checks]),
         exclude=[
             "check_sample_weights_invariance",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     lowess = LowessRegression()
     test_fn(LowessRegression.__name__, lowess)
```

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_mixture_classifier.py` & `scikit-lego-0.6.9/tests/test_estimators/test_mixture_classifier.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks]),
         exclude=[
             "check_sample_weights_invariance",
             "check_non_transformer_estimators_n_iter",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     clf = GMMClassifier()
     test_fn(GMMClassifier.__name__, clf)
     clf = BayesianGMMClassifier()
```

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_mixture_detector.py` & `scikit-lego-0.6.9/tests/test_estimators/test_mixture_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, outlier_checks]),
         exclude=[
             "check_sample_weights_invariance",
-            "check_outliers_train"
+            "check_outliers_train",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     clf_quantile = GMMOutlierDetector(threshold=0.999, method="quantile")
     test_fn(GMMOutlierDetector.__name__ + "_quantile", clf_quantile)
```

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_neighbor_classifier.py` & `scikit-lego-0.6.9/tests/test_estimators/test_neighbor_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, classifier_checks]),
         exclude=[
             "check_sample_weights_invariance",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     test_fn(BayesianKernelDensityClassifier.__name__, BayesianKernelDensityClassifier())
```

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_pca_reconstruction.py` & `scikit-lego-0.6.9/tests/test_estimators/test_pca_reconstruction.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, outlier_checks]),
         exclude=[
             "check_sample_weights_invariance",
             "check_outliers_fit_predict",
-            "check_outliers_train"
+            "check_outliers_train",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     outlier_mod = PCAOutlierDetection(n_components=2, threshold=0.05, random_state=42, variant='absolute')
     test_fn(PCAOutlierDetection.__name__, outlier_mod)
```

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_quantile_regression.py` & `scikit-lego-0.6.9/tests/test_estimators/test_quantile_regression.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_randomregressor.py` & `scikit-lego-0.6.9/tests/test_estimators/test_randomregressor.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, regressor_checks]),
         exclude=[
             "check_sample_weights_invariance",
             "check_methods_subset_invariance",
-            "check_regressors_train"
+            "check_regressors_train",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     # Tests that are skipped:
     # 'check_methods_subset_invariance': Since we add noise, the method is not invariant on a subset
     # 'check_regressors_train': score is not always greater than 0.5 due to randomness
```

### Comparing `scikit-lego-0.6.8/tests/test_estimators/test_umap_reconstruction.py` & `scikit-lego-0.6.9/tests/test_estimators/test_umap_reconstruction.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,17 @@
             "check_outliers_train",
             "check_fit2d_predict1d",
             "check_methods_subset_invariance",
             "check_fit2d_1sample",
             "check_fit2d_1feature",
             "check_dict_unchanged",
             "check_dont_overwrite_parameters",
-            "check_classifier_data_not_an_array"
+            "check_classifier_data_not_an_array",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     outlier_mod = UMAPOutlierDetection(n_components=2, threshold=0.1)
     test_fn(UMAPOutlierDetection.__name__, outlier_mod)
```

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_confusion_balancer.py` & `scikit-lego-0.6.9/tests/test_meta/test_confusion_balancer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_decay_estimator.py` & `scikit-lego-0.6.9/tests/test_meta/test_decay_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_estimatortransformer.py` & `scikit-lego-0.6.9/tests/test_meta/test_estimatortransformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_grouped_predictor.py` & `scikit-lego-0.6.9/tests/test_meta/test_grouped_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,16 @@
     expected_prediction = [
         np.array([means["Earth"], means["NL"], means["Amsterdam"]]) @ shrinkage_factors,
         np.array([means["Earth"], means["NL"], means["Rotterdam"]]) @ shrinkage_factors,
         np.array([means["Earth"], means["BE"], means["Antwerp"]]) @ shrinkage_factors,
         np.array([means["Earth"], means["BE"], means["Brussels"]]) @ shrinkage_factors,
     ]
 
-    assert expected_prediction == shrink_est.predict(X).tolist()
+    for exp, pred in zip(expected_prediction, shrink_est.predict(X).tolist()):
+        assert pytest.approx(exp) == pred
 
 
 def test_relative_shrinkage(shrinkage_data):
     df, means = shrinkage_data
 
     X, y = df.drop(columns="Target"), df["Target"]
 
@@ -188,15 +189,16 @@
     expected_prediction = [
         np.array([means["Earth"], means["NL"], means["Amsterdam"]]) @ shrinkage_factors,
         np.array([means["Earth"], means["NL"], means["Rotterdam"]]) @ shrinkage_factors,
         np.array([means["Earth"], means["BE"], means["Antwerp"]]) @ shrinkage_factors,
         np.array([means["Earth"], means["BE"], means["Brussels"]]) @ shrinkage_factors,
     ]
 
-    assert expected_prediction == shrink_est.predict(X).tolist()
+    for exp, pred in zip(expected_prediction, shrink_est.predict(X).tolist()):
+        assert pytest.approx(exp) == pred
 
 
 def test_min_n_obs_shrinkage(shrinkage_data):
     df, means = shrinkage_data
 
     X, y = df.drop(columns="Target"), df["Target"]
 
@@ -208,15 +210,16 @@
         min_n_obs=2,
     )
 
     shrink_est.fit(X, y)
 
     expected_prediction = [means["NL"], means["NL"], means["BE"], means["BE"]]
 
-    assert expected_prediction == shrink_est.predict(X).tolist()
+    for exp, pred in zip(expected_prediction, shrink_est.predict(X).tolist()):
+        assert pytest.approx(exp) == pred
 
 
 def test_min_n_obs_shrinkage_too_little_obs(shrinkage_data):
     df, means = shrinkage_data
 
     X, y = df.drop(columns="Target"), df["Target"]
```

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_grouped_transformer.py` & `scikit-lego-0.6.9/tests/test_meta/test_grouped_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_outlier_classifier.py` & `scikit-lego-0.6.9/tests/test_meta/test_outlier_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_outlier_remover.py` & `scikit-lego-0.6.9/tests/test_meta/test_outlier_remover.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_regression_outlier.py` & `scikit-lego-0.6.9/tests/test_meta/test_regression_outlier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_subjective_classifier.py` & `scikit-lego-0.6.9/tests/test_meta/test_subjective_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_thresholder.py` & `scikit-lego-0.6.9/tests/test_meta/test_thresholder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import numpy as np
+import copy
 from sklearn.linear_model import LogisticRegression, LinearRegression
 from sklearn.exceptions import NotFittedError
 
 from sklego.common import flatten
 from sklego.meta import Thresholder
 from tests.conftest import general_checks, classifier_checks, select_tests
 
@@ -81,7 +82,23 @@
     lr = LogisticRegression()
     mod = Thresholder(lr, threshold=0.5, refit=False)
     np.random.seed(42)
     X = np.random.normal(0, 1, (100, 3))
     y = np.random.normal(0, 1, (100,)) < 0
     mod.fit(X, y).predict(X)
     assert mod.fit(X, y).predict(X).shape == y.shape
+
+
+@pytest.mark.parametrize('refit', [True, False])
+def test_passes_sample_weight(refit):
+    class CustomLR(LogisticRegression):
+        def fit(self, X, y, sample_weight=None):
+            assert sample_weight is not None
+            super().fit(X, y)
+
+    mod = Thresholder(CustomLR(), threshold=0.5, refit=refit)
+    np.random.seed(42)
+    X = np.random.normal(0, 1, (100, 3))
+    y = np.random.normal(0, 1, (100,)) < 0
+    weight = np.random.random(100)
+
+    mod.fit(X, y, sample_weight=weight)
```

### Comparing `scikit-lego-0.6.8/tests/test_meta/test_zero_inflated_regressor.py` & `scikit-lego-0.6.9/tests/test_meta/test_zero_inflated_regressor.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_metrics/test_correlation_score.py` & `scikit-lego-0.6.9/tests/test_metrics/test_correlation_score.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_metrics/test_equal_opportunity.py` & `scikit-lego-0.6.9/tests/test_metrics/test_equal_opportunity.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_metrics/test_p_percent.py` & `scikit-lego-0.6.9/tests/test_metrics/test_p_percent.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_metrics/test_subset_metric.py` & `scikit-lego-0.6.9/tests/test_metrics/test_subset_metric.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_model_selection/test_klusterfold.py` & `scikit-lego-0.6.9/tests/test_model_selection/test_klusterfold.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_model_selection/test_timegapsplit.py` & `scikit-lego-0.6.9/tests/test_model_selection/test_timegapsplit.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_notinstalled.py` & `scikit-lego-0.6.9/tests/test_notinstalled.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_columncapper.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_columncapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, transformer_checks]),
         exclude=[
             "check_sample_weights_invariance",
-            "check_estimators_nan_inf"
+            "check_estimators_nan_inf",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     test_fn(ColumnCapper.__name__, ColumnCapper())
```

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_columndropper.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_columndropper.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_columnselector.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_columnselector.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_dictmapper.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_dictmapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, transformer_checks]),
         exclude=[
             "check_sample_weights_invariance",
-            "check_dtype_object"
+            "check_dtype_object",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     test_fn(DictMapper.__name__, DictMapper(mapper={"foo": 1}, default=-1))
```

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_identitytransformer.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_identitytransformer.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, transformer_checks]),
         exclude=[
             "check_sample_weights_invariance",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     test_fn(IdentityTransformer.__name__, IdentityTransformer())
```

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_informationfilter.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_informationfilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, transformer_checks, nonmeta_checks]),
         exclude=[
             "check_sample_weights_invariance",
-            "check_estimators_empty_data_messages"
+            "check_estimators_empty_data_messages",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     test_fn(InformationFilter.__name__, InformationFilter(columns=[0]))
```

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_interval_encoder.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_interval_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     flatten(
         [
             transformer_checks,
             general_checks,
             estimator_checks.check_estimators_dtypes,
             estimator_checks.check_fit_score_takes_y,
             # estimator_checks.check_dtype_object,
-            estimator_checks.check_sample_weights_pandas_series,
-            estimator_checks.check_sample_weights_list,
+            # estimator_checks.check_sample_weights_pandas_series,
+            # estimator_checks.check_sample_weights_list,
             # estimator_checks.check_sample_weights_invariance,
             estimator_checks.check_estimators_fit_returns_self,
             estimator_checks.check_complex_data,
             estimator_checks.check_estimators_empty_data_messages,
             estimator_checks.check_pipeline_consistency,
             estimator_checks.check_estimators_nan_inf,
             estimator_checks.check_estimators_overwrite_params,
```

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_orthogonal_transformer.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_orthogonal_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 @pytest.mark.parametrize(
     "test_fn",
     select_tests(
         flatten([general_checks, nonmeta_checks, transformer_checks]),
         exclude=[
             "check_sample_weights_invariance",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     test_fn(OrthogonalTransformer.__name__, OrthogonalTransformer())
```

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_outlier_remover.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_outlier_remover.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_pandastypeselector.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_pandastypeselector.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_patsy_transformer.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_patsy_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_randomadder.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_randomadder.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     "test_fn",
     select_tests(
         flatten([general_checks, transformer_checks, nonmeta_checks]),
         exclude=[
             "check_sample_weights_invariance",
             "check_methods_subset_invariance",
             "check_transformer_data_not_an_array",
-            "check_transformer_general"
+            "check_transformer_general",
+            "check_sample_weights_list",
+            "check_sample_weights_pandas_series"
         ]
     )
 )
 def test_estimator_checks(test_fn):
     adder = RandomAdder()
     test_fn(RandomAdder.__name__, adder)
```

### Comparing `scikit-lego-0.6.8/tests/test_preprocessing/test_repeatingbasisfunction.py` & `scikit-lego-0.6.9/tests/test_preprocessing/test_repeatingbasisfunction.py`

 * *Files identical despite different names*

