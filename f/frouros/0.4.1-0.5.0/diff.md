# Comparing `tmp/frouros-0.4.1.tar.gz` & `tmp/frouros-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.4.1.tar", last modified: Mon Jul  3 08:22:15 2023, max compression
+gzip compressed data, was "frouros-0.5.0.tar", last modified: Tue Jul 18 10:24:07 2023, max compression
```

## Comparing `frouros-0.4.1.tar` & `frouros-0.5.0.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.023203 frouros-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-03 08:22:02.000000 frouros-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-03 08:22:02.000000 frouros-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    23090 2023-07-03 08:22:15.023203 frouros-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    21469 2023-07-03 08:22:02.000000 frouros-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.011202 frouros-0.4.1/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.011202 frouros-0.4.1/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/batch/reset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5856 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.015202 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      637 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1701 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12875 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9163 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     7832 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    14974 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.019202 frouros-0.4.1/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.023203 frouros-0.4.1/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.023203 frouros-0.4.1/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-07-03 08:22:02.000000 frouros-0.4.1/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 08:22:15.011202 frouros-0.4.1/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    23090 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4865 2023-07-03 08:22:15.000000 frouros-0.4.1/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-03 08:22:14.000000 frouros-0.4.1/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-03 08:22:02.000000 frouros-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-03 08:22:15.023203 frouros-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-07-03 08:22:02.000000 frouros-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-18 10:23:52.000000 frouros-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-18 10:23:52.000000 frouros-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    23673 2023-07-18 10:24:07.517669 frouros-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    22052 2023-07-18 10:23:52.000000 frouros-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/batch/reset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5856 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1701 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12875 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9163 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7832 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15055 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    23673 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-18 10:23:53.000000 frouros-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 10:24:07.517669 frouros-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-07-18 10:23:53.000000 frouros-0.5.0/setup.py
```

### Comparing `frouros-0.4.1/LICENSE` & `frouros-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/PKG-INFO` & `frouros-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.4.1
+Version: 0.5.0
 Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
@@ -63,15 +63,19 @@
   </a>
   <!-- Python -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/pyversions/frouros" alt="python">
   </a>
   <!-- License -->
   <a href="https://opensource.org/licenses/BSD-3-Clause">
-    <img src="https://img.shields.io/badge/License-BSD%203--Clause-blue.svg" alt="bsd_3_license">
+    <img src="https://img.shields.io/badge/license-BSD%203--Clause-blue.svg" alt="bsd_3_license">
+  </a>
+  <!-- arXiv -->
+  <a href="https://arxiv.org/abs/2208.06868">
+    <img src="https://img.shields.io/badge/arXiv-2208.06868-blue.svg" alt="arxiv">
   </a>
 </p>
 
 Frouros is a Python library for drift detection in machine learning systems that provides a combination of classical and more recent algorithms for both concept and data drift detection.
 
 <p align="center">
     <i>
@@ -322,17 +326,23 @@
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">STEPD</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1007/978-3-540-75488-6_27">Nishida and Yamauchi (2007)</a></td>
   </tr>
   <tr>
-    <td rowspan="15" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
-    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
-    <td rowspan="8" style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
+    <td rowspan="16" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
+    <td rowspan="14" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
+    <td rowspan="9" style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Anderson-Darling test</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2288805">Scholz and Stephens (1987)</a></td>
+  </tr>
+  <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Bhattacharyya distance</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://www.jstor.org/stable/25047882">Bhattacharyya (1946)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.4.1 Summary: An open-source
+Metadata-Version: 2.1 Name: frouros Version: 0.5.0 Summary: An open-source
 Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Requires-Python: >=3.8,<3.12 Description-
 Content-Type: text/markdown Provides-Extra: docs Provides-Extra: notebooks
 License-File: LICENSE
                                     [logo]
 ---
        [ci]  [coverage]  [documentation]  [downloads]  [pypi]  [python]
-                                [bsd_3_license]
+                           [bsd_3_license]  [arxiv]
 Frouros is a Python library for drift detection in machine learning systems
 that provides a combination of classical and more recent algorithms for both
 concept and data drift detection.
                  "Everything changes and nothing stands still"
                 "You could not step twice into the same river"
                                            Heraclitus of Ephesus (535-475 BCE.)
 ---- ## â¡ï¸ Quickstart ### Concept drift As a quick example, we can use the
@@ -97,28 +97,30 @@
                                                                             (2014)
                                U            N           RDDM                Barros_et_al._(2017)
                                U            N           ADWIN               Bifet_and_Gavalda_
                    Window                                                   (2007)
                    based       U            N           KSWIN               Raab_et_al._(2020)
                                U            N           STEPD               Nishida_and_Yamauchi_
                                                                             (2007)
+                               U            N           Anderson-Darling    Scholz_and_Stephens_
+                                                        test                (1987)
                                U            N           Bhattacharyya       Bhattacharyya_(1946)
                                                         distance
                                U            N           Earth Mover's       Rubner_et_al._(2000)
                                                         distance
                                U            N           Hellinger distance  Hellinger_(1909)
-                                                        Histogram
-                   Distance    U            N           intersection        Swain_and_Ballard_
-                   based                                normalized          (1991)
+                   Distance                             Histogram
+                   based       U            N           intersection        Swain_and_Ballard_
+                                                        normalized          (1991)
                                                         complement
-                               U            N           Jensen-Shannon      Lin_(1991)
-         Batch                                          distance
-                               U            N           Kullback-Leibler    Kullback_and_Leibler_
-Data                                                    divergence          (1951)
-drift                          M            N           MMD                 Gretton_et_al._(2012)
+         Batch                 U            N           Jensen-Shannon      Lin_(1991)
+                                                        distance
+Data                           U            N           Kullback-Leibler    Kullback_and_Leibler_
+drift                                                   divergence          (1951)
+                               M            N           MMD                 Gretton_et_al._(2012)
                                U            N           PSI                 Wu_and_Olson_(2010)
                                U            C           Chi-square test     Pearson_(1900)
                                U            N           CramÃ©r-von Mises CramÃ©r_(1902)
                    Statistical                          test
                    test        U            N           Kolmogorov-Smirnov  Massey_Jr_(1951)
                                                         test
                                U            N           Mann-Whitney U test Mann_and_Whitney_(1947)
```

### Comparing `frouros-0.4.1/README.md` & `frouros-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,19 @@
   </a>
   <!-- Python -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/pyversions/frouros" alt="python">
   </a>
   <!-- License -->
   <a href="https://opensource.org/licenses/BSD-3-Clause">
-    <img src="https://img.shields.io/badge/License-BSD%203--Clause-blue.svg" alt="bsd_3_license">
+    <img src="https://img.shields.io/badge/license-BSD%203--Clause-blue.svg" alt="bsd_3_license">
+  </a>
+  <!-- arXiv -->
+  <a href="https://arxiv.org/abs/2208.06868">
+    <img src="https://img.shields.io/badge/arXiv-2208.06868-blue.svg" alt="arxiv">
   </a>
 </p>
 
 Frouros is a Python library for drift detection in machine learning systems that provides a combination of classical and more recent algorithms for both concept and data drift detection.
 
 <p align="center">
     <i>
@@ -286,17 +290,23 @@
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">STEPD</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1007/978-3-540-75488-6_27">Nishida and Yamauchi (2007)</a></td>
   </tr>
   <tr>
-    <td rowspan="15" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
-    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
-    <td rowspan="8" style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
+    <td rowspan="16" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
+    <td rowspan="14" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
+    <td rowspan="9" style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Anderson-Darling test</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2288805">Scholz and Stephens (1987)</a></td>
+  </tr>
+  <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Bhattacharyya distance</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://www.jstor.org/stable/25047882">Bhattacharyya (1946)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                                     [logo]
 ---
        [ci]  [coverage]  [documentation]  [downloads]  [pypi]  [python]
-                                [bsd_3_license]
+                           [bsd_3_license]  [arxiv]
 Frouros is a Python library for drift detection in machine learning systems
 that provides a combination of classical and more recent algorithms for both
 concept and data drift detection.
                  "Everything changes and nothing stands still"
                 "You could not step twice into the same river"
                                            Heraclitus of Ephesus (535-475 BCE.)
 ---- ## â¡ï¸ Quickstart ### Concept drift As a quick example, we can use the
@@ -75,28 +75,30 @@
                                                                             (2014)
                                U            N           RDDM                Barros_et_al._(2017)
                                U            N           ADWIN               Bifet_and_Gavalda_
                    Window                                                   (2007)
                    based       U            N           KSWIN               Raab_et_al._(2020)
                                U            N           STEPD               Nishida_and_Yamauchi_
                                                                             (2007)
+                               U            N           Anderson-Darling    Scholz_and_Stephens_
+                                                        test                (1987)
                                U            N           Bhattacharyya       Bhattacharyya_(1946)
                                                         distance
                                U            N           Earth Mover's       Rubner_et_al._(2000)
                                                         distance
                                U            N           Hellinger distance  Hellinger_(1909)
-                                                        Histogram
-                   Distance    U            N           intersection        Swain_and_Ballard_
-                   based                                normalized          (1991)
+                   Distance                             Histogram
+                   based       U            N           intersection        Swain_and_Ballard_
+                                                        normalized          (1991)
                                                         complement
-                               U            N           Jensen-Shannon      Lin_(1991)
-         Batch                                          distance
-                               U            N           Kullback-Leibler    Kullback_and_Leibler_
-Data                                                    divergence          (1951)
-drift                          M            N           MMD                 Gretton_et_al._(2012)
+         Batch                 U            N           Jensen-Shannon      Lin_(1991)
+                                                        distance
+Data                           U            N           Kullback-Leibler    Kullback_and_Leibler_
+drift                                                   divergence          (1951)
+                               M            N           MMD                 Gretton_et_al._(2012)
                                U            N           PSI                 Wu_and_Olson_(2010)
                                U            C           Chi-square test     Pearson_(1900)
                                U            N           CramÃ©r-von Mises CramÃ©r_(1902)
                    Statistical                          test
                    test        U            N           Kolmogorov-Smirnov  Massey_Jr_(1951)
                                                         test
                                U            N           Mann-Whitney U test Mann_and_Whitney_(1947)
```

### Comparing `frouros-0.4.1/frouros/callbacks/base.py` & `frouros-0.5.0/frouros/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/callbacks/batch/base.py` & `frouros-0.5.0/frouros/callbacks/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/callbacks/batch/permutation_test.py` & `frouros-0.5.0/frouros/callbacks/batch/permutation_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/callbacks/batch/reset.py` & `frouros-0.5.0/frouros/callbacks/batch/reset.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/callbacks/streaming/base.py` & `frouros-0.5.0/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/callbacks/streaming/history.py` & `frouros-0.5.0/frouros/callbacks/streaming/history.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/callbacks/streaming/msprt.py` & `frouros-0.5.0/frouros/callbacks/streaming/msprt.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.5.0/frouros/callbacks/streaming/warning_samples.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/datasets/base.py` & `frouros-0.5.0/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/datasets/real.py` & `frouros-0.5.0/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/datasets/synthetic.py` & `frouros-0.5.0/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/base.py` & `frouros-0.5.0/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/__init__.py` & `frouros-0.5.0/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/base.py` & `frouros-0.5.0/frouros/detectors/concept_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/base.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/cusum.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py` & `frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/__init__.py` & `frouros-0.5.0/frouros/detectors/data_drift/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Data drift detection methods init."""
 
 from .batch import (  # noqa: F401
+    AndersonDarlingTest,
     BhattacharyyaDistance,
     ChiSquareTest,
     CVMTest,
     EMD,
     HellingerDistance,
     HINormalizedComplement,
     JS,
@@ -15,14 +16,15 @@
     MMD,
     WelchTTest,
 )
 
 from .streaming import IncrementalKSTest, MMD as MMDStreaming  # noqa: N811
 
 __all__ = [
+    "AndersonDarlingTest",
     "BhattacharyyaDistance",
     "ChiSquareTest",
     "CVMTest",
     "EMD",
     "HellingerDistance",
     "HINormalizedComplement",
     "IncrementalKSTest",
```

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/base.py` & `frouros-0.5.0/frouros/detectors/data_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,24 @@
     HINormalizedComplement,
     JS,
     KL,
     PSI,
     MMD,
 )
 from .statistical_test import (
+    AndersonDarlingTest,
     ChiSquareTest,
     CVMTest,
     KSTest,
     MannWhitneyUTest,
     WelchTTest,
 )
 
 __all__ = [
+    "AndersonDarlingTest",
     "BhattacharyyaDistance",
     "ChiSquareTest",
     "CVMTest",
     "EMD",
     "HellingerDistance",
     "HINormalizedComplement",
     "JS",
```

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/base.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.5.0/frouros/detectors/data_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/metrics/base.py` & `frouros-0.5.0/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/metrics/prequential_error.py` & `frouros-0.5.0/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/tests/conftest.py` & `frouros-0.5.0/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/tests/integration/test_callback.py` & `frouros-0.5.0/frouros/tests/integration/test_callback.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/tests/integration/test_concept_drift.py` & `frouros-0.5.0/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/tests/integration/test_data_drift.py` & `frouros-0.5.0/frouros/tests/integration/test_data_drift.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     HINormalizedComplement,
     PSI,
     JS,
     KL,
     MMD,
 )
 from frouros.detectors.data_drift.batch import (
+    AndersonDarlingTest,
     ChiSquareTest,
     CVMTest,
     KSTest,
     MannWhitneyUTest,
     WelchTTest,
 )
 from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
@@ -156,14 +157,15 @@
 
     assert np.isclose(distance, expected_distance)
 
 
 @pytest.mark.parametrize(
     "detector, expected_statistic, expected_p_value",
     [
+        (AndersonDarlingTest(), 23171.19994366, 0.001),
         (CVMTest(), 3776.09848103, 5.38105056e-07),
         (KSTest(), 0.99576271, 0.0),
         (MannWhitneyUTest(), 6912.0, 0.0),
         (WelchTTest(), -287.92032554, 0.0),
     ],
 )
 def test_batch_statistical_univariate(
```

### Comparing `frouros-0.4.1/frouros/tests/integration/test_real.py` & `frouros-0.5.0/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/tests/integration/test_synthetic.py` & `frouros-0.5.0/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.5.0/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/utils/checks.py` & `frouros-0.5.0/frouros/utils/checks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/utils/data_structures.py` & `frouros-0.5.0/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros/utils/stats.py` & `frouros-0.5.0/frouros/utils/stats.py`

 * *Files identical despite different names*

### Comparing `frouros-0.4.1/frouros.egg-info/PKG-INFO` & `frouros-0.5.0/frouros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.4.1
+Version: 0.5.0
 Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
@@ -63,15 +63,19 @@
   </a>
   <!-- Python -->
   <a href="https://pypi.org/project/frouros">
     <img src="https://img.shields.io/pypi/pyversions/frouros" alt="python">
   </a>
   <!-- License -->
   <a href="https://opensource.org/licenses/BSD-3-Clause">
-    <img src="https://img.shields.io/badge/License-BSD%203--Clause-blue.svg" alt="bsd_3_license">
+    <img src="https://img.shields.io/badge/license-BSD%203--Clause-blue.svg" alt="bsd_3_license">
+  </a>
+  <!-- arXiv -->
+  <a href="https://arxiv.org/abs/2208.06868">
+    <img src="https://img.shields.io/badge/arXiv-2208.06868-blue.svg" alt="arxiv">
   </a>
 </p>
 
 Frouros is a Python library for drift detection in machine learning systems that provides a combination of classical and more recent algorithms for both concept and data drift detection.
 
 <p align="center">
     <i>
@@ -322,17 +326,23 @@
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">STEPD</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1007/978-3-540-75488-6_27">Nishida and Yamauchi (2007)</a></td>
   </tr>
   <tr>
-    <td rowspan="15" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
-    <td rowspan="13" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
-    <td rowspan="8" style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
+    <td rowspan="16" style="text-align: center; border: 1px solid grey; padding: 8px;">Data drift</td>
+    <td rowspan="14" style="text-align: center; border: 1px solid grey; padding: 8px;">Batch</td>
+    <td rowspan="9" style="text-align: center; border: 1px solid grey; padding: 8px;">Distance based</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;">Anderson-Darling test</td>
+    <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.2307/2288805">Scholz and Stephens (1987)</a></td>
+  </tr>
+  <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Bhattacharyya distance</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://www.jstor.org/stable/25047882">Bhattacharyya (1946)</a></td>
   </tr>
   <tr>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">U</td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.4.1 Summary: An open-source
+Metadata-Version: 2.1 Name: frouros Version: 0.5.0 Summary: An open-source
 Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 :: Only Requires-Python: >=3.8,<3.12 Description-
 Content-Type: text/markdown Provides-Extra: docs Provides-Extra: notebooks
 License-File: LICENSE
                                     [logo]
 ---
        [ci]  [coverage]  [documentation]  [downloads]  [pypi]  [python]
-                                [bsd_3_license]
+                           [bsd_3_license]  [arxiv]
 Frouros is a Python library for drift detection in machine learning systems
 that provides a combination of classical and more recent algorithms for both
 concept and data drift detection.
                  "Everything changes and nothing stands still"
                 "You could not step twice into the same river"
                                            Heraclitus of Ephesus (535-475 BCE.)
 ---- ## â¡ï¸ Quickstart ### Concept drift As a quick example, we can use the
@@ -97,28 +97,30 @@
                                                                             (2014)
                                U            N           RDDM                Barros_et_al._(2017)
                                U            N           ADWIN               Bifet_and_Gavalda_
                    Window                                                   (2007)
                    based       U            N           KSWIN               Raab_et_al._(2020)
                                U            N           STEPD               Nishida_and_Yamauchi_
                                                                             (2007)
+                               U            N           Anderson-Darling    Scholz_and_Stephens_
+                                                        test                (1987)
                                U            N           Bhattacharyya       Bhattacharyya_(1946)
                                                         distance
                                U            N           Earth Mover's       Rubner_et_al._(2000)
                                                         distance
                                U            N           Hellinger distance  Hellinger_(1909)
-                                                        Histogram
-                   Distance    U            N           intersection        Swain_and_Ballard_
-                   based                                normalized          (1991)
+                   Distance                             Histogram
+                   based       U            N           intersection        Swain_and_Ballard_
+                                                        normalized          (1991)
                                                         complement
-                               U            N           Jensen-Shannon      Lin_(1991)
-         Batch                                          distance
-                               U            N           Kullback-Leibler    Kullback_and_Leibler_
-Data                                                    divergence          (1951)
-drift                          M            N           MMD                 Gretton_et_al._(2012)
+         Batch                 U            N           Jensen-Shannon      Lin_(1991)
+                                                        distance
+Data                           U            N           Kullback-Leibler    Kullback_and_Leibler_
+drift                                                   divergence          (1951)
+                               M            N           MMD                 Gretton_et_al._(2012)
                                U            N           PSI                 Wu_and_Olson_(2010)
                                U            C           Chi-square test     Pearson_(1900)
                                U            N           CramÃ©r-von Mises CramÃ©r_(1902)
                    Statistical                          test
                    test        U            N           Kolmogorov-Smirnov  Massey_Jr_(1951)
                                                         test
                                U            N           Mann-Whitney U test Mann_and_Whitney_(1947)
```

### Comparing `frouros-0.4.1/frouros.egg-info/SOURCES.txt` & `frouros-0.5.0/frouros.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
 frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
 frouros/detectors/data_drift/batch/distance_based/js.py
 frouros/detectors/data_drift/batch/distance_based/kl.py
 frouros/detectors/data_drift/batch/distance_based/mmd.py
 frouros/detectors/data_drift/batch/distance_based/psi.py
 frouros/detectors/data_drift/batch/statistical_test/__init__.py
+frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py
 frouros/detectors/data_drift/batch/statistical_test/base.py
 frouros/detectors/data_drift/batch/statistical_test/chisquare.py
 frouros/detectors/data_drift/batch/statistical_test/cvm.py
 frouros/detectors/data_drift/batch/statistical_test/ks.py
 frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
 frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
 frouros/detectors/data_drift/streaming/__init__.py
```

### Comparing `frouros-0.4.1/pyproject.toml` & `frouros-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.4.1"
+version = "0.5.0"
 description = "An open-source Python library for drift detection in machine learning systems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
```

### Comparing `frouros-0.4.1/setup.py` & `frouros-0.5.0/setup.py`

 * *Files identical despite different names*

