# Comparing `tmp/dicomset-0.0.2.tar.gz` & `tmp/dicomset-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomset-0.0.2.tar", last modified: Tue Jul 18 03:22:51 2023, max compression
+gzip compressed data, was "dicomset-0.0.3.tar", last modified: Tue Jul 18 03:46:26 2023, max compression
```

## Comparing `dicomset-0.0.2.tar` & `dicomset-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,122 @@
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.725281 dicomset-0.0.2/
--rw-r--r--   0 clarkbrett (990701463) 678807148      270 2023-07-18 03:22:51.725114 dicomset-0.0.2/PKG-INFO
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:21.000000 dicomset-0.0.2/README.md
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.722146 dicomset-0.0.2/dicomset.egg-info/
--rw-r--r--   0 clarkbrett (990701463) 678807148      270 2023-07-18 03:22:51.000000 dicomset-0.0.2/dicomset.egg-info/PKG-INFO
--rw-r--r--   0 clarkbrett (990701463) 678807148      441 2023-07-18 03:22:51.000000 dicomset-0.0.2/dicomset.egg-info/SOURCES.txt
--rw-r--r--   0 clarkbrett (990701463) 678807148        1 2023-07-18 03:22:51.000000 dicomset-0.0.2/dicomset.egg-info/dependency_links.txt
--rw-r--r--   0 clarkbrett (990701463) 678807148        5 2023-07-18 03:22:51.000000 dicomset-0.0.2/dicomset.egg-info/top_level.txt
--rw-r--r--   0 clarkbrett (990701463) 678807148       38 2023-07-18 03:22:51.725327 dicomset-0.0.2/setup.cfg
--rw-r--r--   0 clarkbrett (990701463) 678807148      506 2023-07-18 03:21:23.000000 dicomset-0.0.2/setup.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.722447 dicomset-0.0.2/test/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:21.000000 dicomset-0.0.2/test/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.722731 dicomset-0.0.2/test/code/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.722953 dicomset-0.0.2/test/code/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/dataset/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.723256 dicomset-0.0.2/test/code/dataset/raw/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/dataset/raw/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.723924 dicomset-0.0.2/test/code/dataset/raw/dicom/
--rw-r--r--   0 clarkbrett (990701463) 678807148       59 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/dataset/raw/dicom/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1680 2023-07-18 03:06:08.000000 dicomset-0.0.2/test/code/dataset/raw/dicom/test_rtstruct_converter.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.724831 dicomset-0.0.2/test/code/metrics/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/metrics/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1395 2023-07-18 03:06:08.000000 dicomset-0.0.2/test/code/metrics/test_dice.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2516 2023-07-18 03:06:08.000000 dicomset-0.0.2/test/code/metrics/test_hausdorff.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.261936 dicomset-0.0.3/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 03:46:26.261755 dicomset-0.0.3/PKG-INFO
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:21.000000 dicomset-0.0.3/README.md
+-rw-r--r--   0 clarkbrett (990701463) 678807148      597 2023-07-18 03:43:56.000000 dicomset-0.0.3/pyproject.toml
+-rw-r--r--   0 clarkbrett (990701463) 678807148       38 2023-07-18 03:46:26.261989 dicomset-0.0.3/setup.cfg
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.224587 dicomset-0.0.3/src/
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.229501 dicomset-0.0.3/src/dicomset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2042 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/config.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.230976 dicomset-0.0.3/src/dicomset/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3879 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      795 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dataset.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.236511 dicomset-0.0.3/src/dicomset/dataset/dicom/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      825 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     4000 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/ct_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10067 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/dicom_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      170 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/dicom_file.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     7243 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/dicom_patient.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      458 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/dicom_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     9574 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/dicom_study.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    18397 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/index.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1638 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2965 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/region_map.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148       71 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/region_policy.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      283 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/roi_data.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3488 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/rtdose.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/rtdose_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1487 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/rtplan.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/rtplan_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10605 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/rtstruct.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    22735 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/rtstruct_converter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2711 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/dicom/rtstruct_series.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.237216 dicomset-0.0.3/src/dicomset/dataset/nifti/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/nifti/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     5163 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/nifti/nifti_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     5670 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/nifti/nifti_patient.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.237917 dicomset-0.0.3/src/dicomset/dataset/nrrd/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      698 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/nrrd/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     4055 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/nrrd/nrrd_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     4380 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/nrrd/nrrd_patient.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.238638 dicomset-0.0.3/src/dicomset/dataset/other/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/other/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1198 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/other/other_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      777 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/other/other_sample.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.239433 dicomset-0.0.3/src/dicomset/dataset/training/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1074 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/training/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     5404 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/training/training_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3419 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/dataset/training/training_sample.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.239879 dicomset-0.0.3/src/dicomset/evaluation/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/evaluation/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.241094 dicomset-0.0.3/src/dicomset/evaluation/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/evaluation/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    11935 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/evaluation/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    18224 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/evaluation/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    19129 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/evaluation/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3893 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/evaluation/dataset/training.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10858 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/evaluation/model_evaluator.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.241969 dicomset-0.0.3/src/dicomset/geometry/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      187 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/geometry/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      328 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/geometry/box.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      992 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/geometry/centre.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2391 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/geometry/extent.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.242161 dicomset-0.0.3/src/dicomset/logging/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1953 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/logging/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.243277 dicomset-0.0.3/src/dicomset/metrics/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      769 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/metrics/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3894 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/metrics/contrast.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1586 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/metrics/dice.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10609 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/metrics/distances.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      424 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/metrics/volume.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.244029 dicomset-0.0.3/src/dicomset/plotting/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       61 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/plotting/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.245277 dicomset-0.0.3/src/dicomset/plotting/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3300 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/plotting/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    19556 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/plotting/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    19808 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/plotting/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      455 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/plotting/dataset/other.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3104 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/plotting/dataset/training.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    67448 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/plotting/plotter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10901 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/plotting/results.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.245503 dicomset-0.0.3/src/dicomset/processing/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/processing/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.246747 dicomset-0.0.3/src/dicomset/processing/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/processing/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      166 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/processing/dataset/dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     7540 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/processing/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    21722 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/processing/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    21758 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/processing/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3004 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/processing/dataset/other.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.248810 dicomset-0.0.3/src/dicomset/regions/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      967 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/regions/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1084 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/regions/colours.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      723 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/regions/dose_constraints.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      962 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/regions/limits.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1321 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/regions/list.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      901 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/regions/patch_sizes.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1527 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/regions/regions.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1264 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/regions/tolerances.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.253244 dicomset-0.0.3/src/dicomset/reporting/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       97 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.259911 dicomset-0.0.3/src/dicomset/reporting/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2737 2023-07-18 03:07:13.000000 dicomset-0.0.3/src/dicomset/reporting/dataset/dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     8233 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    30026 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    30008 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    13148 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/dataset/training.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3524 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/gpu_usage.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    12593 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/loaders.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2716 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/models.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2012 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/reporter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1271 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/tensorboard_reporter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1817 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/reporting/wandb_reporter.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.261412 dicomset-0.0.3/src/dicomset/types/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       73 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/types/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1844 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/types/parser.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1006 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/types/types.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     9833 2023-07-18 03:06:08.000000 dicomset-0.0.3/src/dicomset/utils.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:46:26.230484 dicomset-0.0.3/src/dicomset.egg-info/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 03:46:26.000000 dicomset-0.0.3/src/dicomset.egg-info/PKG-INFO
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3636 2023-07-18 03:46:26.000000 dicomset-0.0.3/src/dicomset.egg-info/SOURCES.txt
+-rw-r--r--   0 clarkbrett (990701463) 678807148        1 2023-07-18 03:46:26.000000 dicomset-0.0.3/src/dicomset.egg-info/dependency_links.txt
+-rw-r--r--   0 clarkbrett (990701463) 678807148        9 2023-07-18 03:46:26.000000 dicomset-0.0.3/src/dicomset.egg-info/top_level.txt
```

