# Comparing `tmp/dicomset-0.0.5.tar.gz` & `tmp/dicomset-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomset-0.0.5.tar", last modified: Tue Jul 18 03:59:07 2023, max compression
+gzip compressed data, was "dicomset-0.0.6.tar", last modified: Tue Jul 18 04:30:16 2023, max compression
```

## Comparing `dicomset-0.0.5.tar` & `dicomset-0.0.6.tar`

### file list

```diff
@@ -1,119 +1,130 @@
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.050757 dicomset-0.0.5/
--rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 03:59:07.050589 dicomset-0.0.5/PKG-INFO
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:21.000000 dicomset-0.0.5/README.md
--rw-r--r--   0 clarkbrett (990701463) 678807148      597 2023-07-18 03:58:57.000000 dicomset-0.0.5/pyproject.toml
--rw-r--r--   0 clarkbrett (990701463) 678807148       38 2023-07-18 03:59:07.050799 dicomset-0.0.5/setup.cfg
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.018355 dicomset-0.0.5/src/
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.023347 dicomset-0.0.5/src/dicomset/
--rw-r--r--   0 clarkbrett (990701463) 678807148     2042 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/config.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.024930 dicomset-0.0.5/src/dicomset/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148     3879 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      795 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dataset.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.032206 dicomset-0.0.5/src/dicomset/dataset/dicom/
--rw-r--r--   0 clarkbrett (990701463) 678807148      825 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     4000 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/ct_series.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10067 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/dicom_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      170 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/dicom_file.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     7243 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/dicom_patient.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      458 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/dicom_series.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     9574 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/dicom_study.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    18397 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/index.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1638 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2965 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/region_map.py
--rw-r--r--   0 clarkbrett (990701463) 678807148       71 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/region_policy.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      283 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/roi_data.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3488 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/rtdose.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/rtdose_series.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1487 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/rtplan.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/rtplan_series.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10605 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/rtstruct.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    22735 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/rtstruct_converter.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2711 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/dicom/rtstruct_series.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.033026 dicomset-0.0.5/src/dicomset/dataset/nifti/
--rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/nifti/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     5163 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/nifti/nifti_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     5670 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/nifti/nifti_patient.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.033760 dicomset-0.0.5/src/dicomset/dataset/nrrd/
--rw-r--r--   0 clarkbrett (990701463) 678807148      698 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/nrrd/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     4055 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/nrrd/nrrd_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     4380 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/nrrd/nrrd_patient.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.034617 dicomset-0.0.5/src/dicomset/dataset/other/
--rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/other/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1198 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/other/other_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      777 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/other/other_sample.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.035404 dicomset-0.0.5/src/dicomset/dataset/training/
--rw-r--r--   0 clarkbrett (990701463) 678807148     1074 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/training/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     5404 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/training/training_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3419 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/dataset/training/training_sample.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.035802 dicomset-0.0.5/src/dicomset/evaluation/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/evaluation/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.036980 dicomset-0.0.5/src/dicomset/evaluation/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/evaluation/dataset/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    11935 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/evaluation/dataset/dicom.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    18224 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/evaluation/dataset/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    19129 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/evaluation/dataset/nrrd.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3893 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/evaluation/dataset/training.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10858 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/evaluation/model_evaluator.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.037977 dicomset-0.0.5/src/dicomset/geometry/
--rw-r--r--   0 clarkbrett (990701463) 678807148      187 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/geometry/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      328 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/geometry/box.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      992 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/geometry/centre.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2391 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/geometry/extent.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.038511 dicomset-0.0.5/src/dicomset/logging/
--rw-r--r--   0 clarkbrett (990701463) 678807148     1953 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/logging/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.039709 dicomset-0.0.5/src/dicomset/metrics/
--rw-r--r--   0 clarkbrett (990701463) 678807148      769 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/metrics/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3894 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/metrics/contrast.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1586 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/metrics/dice.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10609 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/metrics/distances.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      424 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/metrics/volume.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.040531 dicomset-0.0.5/src/dicomset/plotting/
--rw-r--r--   0 clarkbrett (990701463) 678807148       61 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/plotting/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.043405 dicomset-0.0.5/src/dicomset/plotting/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148     3300 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/plotting/dataset/dicom.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    19556 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/plotting/dataset/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    19808 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/plotting/dataset/nrrd.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      455 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/plotting/dataset/other.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3104 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/plotting/dataset/training.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    67448 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/plotting/plotter.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10901 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/plotting/results.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.043685 dicomset-0.0.5/src/dicomset/processing/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/processing/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.045209 dicomset-0.0.5/src/dicomset/processing/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/processing/dataset/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      166 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/processing/dataset/dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     7540 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/processing/dataset/dicom.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    21722 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/processing/dataset/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    21758 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/processing/dataset/nrrd.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3004 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/processing/dataset/other.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.046530 dicomset-0.0.5/src/dicomset/regions/
--rw-r--r--   0 clarkbrett (990701463) 678807148      821 2023-07-18 03:51:55.000000 dicomset-0.0.5/src/dicomset/regions/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1084 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/regions/colours.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1321 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/regions/list.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1527 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/regions/regions.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1264 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/regions/tolerances.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.048233 dicomset-0.0.5/src/dicomset/reporting/
--rw-r--r--   0 clarkbrett (990701463) 678807148       97 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.049706 dicomset-0.0.5/src/dicomset/reporting/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/dataset/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2737 2023-07-18 03:07:13.000000 dicomset-0.0.5/src/dicomset/reporting/dataset/dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     8233 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/dataset/dicom.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    30026 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/dataset/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    30008 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/dataset/nrrd.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    13148 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/dataset/training.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3524 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/gpu_usage.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    12593 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/loaders.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2716 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/models.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2012 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/reporter.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1271 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/tensorboard_reporter.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1817 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/reporting/wandb_reporter.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.050358 dicomset-0.0.5/src/dicomset/types/
--rw-r--r--   0 clarkbrett (990701463) 678807148       73 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/types/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1844 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/types/parser.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1006 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/types/types.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     9833 2023-07-18 03:06:08.000000 dicomset-0.0.5/src/dicomset/utils.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:59:07.024362 dicomset-0.0.5/src/dicomset.egg-info/
--rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 03:59:06.000000 dicomset-0.0.5/src/dicomset.egg-info/PKG-INFO
--rw-r--r--   0 clarkbrett (990701463) 678807148     3528 2023-07-18 03:59:07.000000 dicomset-0.0.5/src/dicomset.egg-info/SOURCES.txt
--rw-r--r--   0 clarkbrett (990701463) 678807148        1 2023-07-18 03:59:06.000000 dicomset-0.0.5/src/dicomset.egg-info/dependency_links.txt
--rw-r--r--   0 clarkbrett (990701463) 678807148        9 2023-07-18 03:59:06.000000 dicomset-0.0.5/src/dicomset.egg-info/top_level.txt
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.526393 dicomset-0.0.6/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 04:30:16.526232 dicomset-0.0.6/PKG-INFO
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:21.000000 dicomset-0.0.6/README.md
+-rw-r--r--   0 clarkbrett (990701463) 678807148      597 2023-07-18 04:08:12.000000 dicomset-0.0.6/pyproject.toml
+-rw-r--r--   0 clarkbrett (990701463) 678807148       38 2023-07-18 04:30:16.526435 dicomset-0.0.6/setup.cfg
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.497187 dicomset-0.0.6/src/
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.500800 dicomset-0.0.6/src/dicomset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2042 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/config.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.502362 dicomset-0.0.6/src/dicomset/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3879 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      795 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dataset.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.507349 dicomset-0.0.6/src/dicomset/dataset/dicom/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      825 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     4000 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/ct_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10067 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      170 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_file.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     7243 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_patient.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      458 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     9574 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_study.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    18397 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/index.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1638 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2965 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/region_map.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148       71 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/region_policy.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      283 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/roi_data.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3488 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtdose.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtdose_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1487 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtplan.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtplan_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10605 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    22735 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct_converter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2711 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct_series.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.508167 dicomset-0.0.6/src/dicomset/dataset/nifti/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nifti/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     5163 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nifti/nifti_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     5670 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nifti/nifti_patient.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.509303 dicomset-0.0.6/src/dicomset/dataset/nrrd/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      698 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nrrd/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     4055 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nrrd/nrrd_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     4380 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nrrd/nrrd_patient.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.510087 dicomset-0.0.6/src/dicomset/dataset/other/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/other/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1198 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/other/other_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      777 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/other/other_sample.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.510925 dicomset-0.0.6/src/dicomset/dataset/training/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1074 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/training/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     5404 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/training/training_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3419 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/training/training_sample.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.511427 dicomset-0.0.6/src/dicomset/evaluation/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.512672 dicomset-0.0.6/src/dicomset/evaluation/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    11935 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    18224 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    19129 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3893 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/training.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10858 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/model_evaluator.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.513589 dicomset-0.0.6/src/dicomset/geometry/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      187 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/geometry/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      328 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/geometry/box.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      992 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/geometry/centre.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2391 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/geometry/extent.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.513854 dicomset-0.0.6/src/dicomset/logging/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1953 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/logging/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.514989 dicomset-0.0.6/src/dicomset/metrics/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      769 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3894 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/contrast.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1586 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/dice.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10609 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/distances.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      424 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/volume.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.515862 dicomset-0.0.6/src/dicomset/plotting/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       61 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.517104 dicomset-0.0.6/src/dicomset/plotting/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3300 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    19556 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    19808 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      455 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/other.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3104 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/training.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    67448 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/plotter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10901 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/results.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.517330 dicomset-0.0.6/src/dicomset/processing/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.518696 dicomset-0.0.6/src/dicomset/processing/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      166 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     7540 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    21722 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    21758 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3004 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/other.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.519789 dicomset-0.0.6/src/dicomset/regions/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      821 2023-07-18 03:51:55.000000 dicomset-0.0.6/src/dicomset/regions/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1084 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/regions/colours.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1321 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/regions/list.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1527 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/regions/regions.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1264 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/regions/tolerances.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.521298 dicomset-0.0.6/src/dicomset/reporting/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       97 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.522690 dicomset-0.0.6/src/dicomset/reporting/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2737 2023-07-18 03:07:13.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     8233 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    30026 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    30008 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    13148 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/training.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3524 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/gpu_usage.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    12593 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/loaders.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2716 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/models.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2012 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/reporter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1271 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/tensorboard_reporter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1817 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/wandb_reporter.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.525406 dicomset-0.0.6/src/dicomset/transforms/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      401 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     9580 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/crop.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      504 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/custom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      360 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_elastic_deformation.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2601 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_intensity.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2484 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_resample.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3462 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_rotation.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3328 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_translation.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3637 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/resample.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      174 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/translate.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.526011 dicomset-0.0.6/src/dicomset/types/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       73 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/types/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1844 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/types/parser.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1006 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/types/types.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     9833 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/utils.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.501854 dicomset-0.0.6/src/dicomset.egg-info/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 04:30:16.000000 dicomset-0.0.6/src/dicomset.egg-info/PKG-INFO
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3933 2023-07-18 04:30:16.000000 dicomset-0.0.6/src/dicomset.egg-info/SOURCES.txt
+-rw-r--r--   0 clarkbrett (990701463) 678807148        1 2023-07-18 04:30:16.000000 dicomset-0.0.6/src/dicomset.egg-info/dependency_links.txt
+-rw-r--r--   0 clarkbrett (990701463) 678807148        9 2023-07-18 04:30:16.000000 dicomset-0.0.6/src/dicomset.egg-info/top_level.txt
```

### Comparing `dicomset-0.0.5/pyproject.toml` & `dicomset-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dicomset"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "Brett Clark", email = "clarkbab@gmail.com" }
 ]
 description = "Python library for DICOM processing and analysis"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `dicomset-0.0.5/src/dicomset/config.py` & `dicomset-0.0.6/src/dicomset/config.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/__init__.py` & `dicomset-0.0.6/src/dicomset/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dataset.py` & `dicomset-0.0.6/src/dicomset/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/__init__.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/ct_series.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/ct_series.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/dicom_dataset.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/dicom_patient.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_patient.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/dicom_study.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_study.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/index.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/index.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/nifti.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/region_map.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/region_map.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/rtdose.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/rtdose.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/rtdose_series.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/rtdose_series.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/rtplan.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/rtplan.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/rtplan_series.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/rtplan_series.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/rtstruct.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/rtstruct_converter.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct_converter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/dicom/rtstruct_series.py` & `dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct_series.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/nifti/__init__.py` & `dicomset-0.0.6/src/dicomset/dataset/nifti/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/nifti/nifti_dataset.py` & `dicomset-0.0.6/src/dicomset/dataset/nifti/nifti_dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/nifti/nifti_patient.py` & `dicomset-0.0.6/src/dicomset/dataset/nifti/nifti_patient.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/nrrd/__init__.py` & `dicomset-0.0.6/src/dicomset/dataset/nrrd/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/nrrd/nrrd_dataset.py` & `dicomset-0.0.6/src/dicomset/dataset/nrrd/nrrd_dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/nrrd/nrrd_patient.py` & `dicomset-0.0.6/src/dicomset/dataset/nrrd/nrrd_patient.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/other/__init__.py` & `dicomset-0.0.6/src/dicomset/dataset/other/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/other/other_dataset.py` & `dicomset-0.0.6/src/dicomset/dataset/other/other_dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/other/other_sample.py` & `dicomset-0.0.6/src/dicomset/dataset/other/other_sample.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/training/__init__.py` & `dicomset-0.0.6/src/dicomset/dataset/training/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/training/training_dataset.py` & `dicomset-0.0.6/src/dicomset/dataset/training/training_dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/dataset/training/training_sample.py` & `dicomset-0.0.6/src/dicomset/dataset/training/training_sample.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/evaluation/dataset/dicom.py` & `dicomset-0.0.6/src/dicomset/evaluation/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/evaluation/dataset/nifti.py` & `dicomset-0.0.6/src/dicomset/evaluation/dataset/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/evaluation/dataset/nrrd.py` & `dicomset-0.0.6/src/dicomset/evaluation/dataset/nrrd.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/evaluation/dataset/training.py` & `dicomset-0.0.6/src/dicomset/evaluation/dataset/training.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/evaluation/model_evaluator.py` & `dicomset-0.0.6/src/dicomset/evaluation/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/geometry/centre.py` & `dicomset-0.0.6/src/dicomset/geometry/centre.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/geometry/extent.py` & `dicomset-0.0.6/src/dicomset/geometry/extent.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/logging/__init__.py` & `dicomset-0.0.6/src/dicomset/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/metrics/__init__.py` & `dicomset-0.0.6/src/dicomset/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/metrics/contrast.py` & `dicomset-0.0.6/src/dicomset/metrics/contrast.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/metrics/dice.py` & `dicomset-0.0.6/src/dicomset/metrics/dice.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/metrics/distances.py` & `dicomset-0.0.6/src/dicomset/metrics/distances.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/plotting/dataset/dicom.py` & `dicomset-0.0.6/src/dicomset/plotting/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/plotting/dataset/nifti.py` & `dicomset-0.0.6/src/dicomset/plotting/dataset/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/plotting/dataset/nrrd.py` & `dicomset-0.0.6/src/dicomset/plotting/dataset/nrrd.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/plotting/dataset/training.py` & `dicomset-0.0.6/src/dicomset/plotting/dataset/training.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/plotting/plotter.py` & `dicomset-0.0.6/src/dicomset/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/plotting/results.py` & `dicomset-0.0.6/src/dicomset/plotting/results.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/processing/dataset/dicom.py` & `dicomset-0.0.6/src/dicomset/processing/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/processing/dataset/nifti.py` & `dicomset-0.0.6/src/dicomset/processing/dataset/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/processing/dataset/nrrd.py` & `dicomset-0.0.6/src/dicomset/processing/dataset/nrrd.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/processing/dataset/other.py` & `dicomset-0.0.6/src/dicomset/processing/dataset/other.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/regions/__init__.py` & `dicomset-0.0.6/src/dicomset/regions/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/regions/colours.py` & `dicomset-0.0.6/src/dicomset/regions/colours.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/regions/list.py` & `dicomset-0.0.6/src/dicomset/regions/list.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/regions/regions.py` & `dicomset-0.0.6/src/dicomset/regions/regions.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/regions/tolerances.py` & `dicomset-0.0.6/src/dicomset/regions/tolerances.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/dataset/dataset.py` & `dicomset-0.0.6/src/dicomset/reporting/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/dataset/dicom.py` & `dicomset-0.0.6/src/dicomset/reporting/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/dataset/nifti.py` & `dicomset-0.0.6/src/dicomset/reporting/dataset/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/dataset/nrrd.py` & `dicomset-0.0.6/src/dicomset/reporting/dataset/nrrd.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/dataset/training.py` & `dicomset-0.0.6/src/dicomset/reporting/dataset/training.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/gpu_usage.py` & `dicomset-0.0.6/src/dicomset/reporting/gpu_usage.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/loaders.py` & `dicomset-0.0.6/src/dicomset/reporting/loaders.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/models.py` & `dicomset-0.0.6/src/dicomset/reporting/models.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/reporter.py` & `dicomset-0.0.6/src/dicomset/reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/tensorboard_reporter.py` & `dicomset-0.0.6/src/dicomset/reporting/tensorboard_reporter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/reporting/wandb_reporter.py` & `dicomset-0.0.6/src/dicomset/reporting/wandb_reporter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/types/parser.py` & `dicomset-0.0.6/src/dicomset/types/parser.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/types/types.py` & `dicomset-0.0.6/src/dicomset/types/types.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset/utils.py` & `dicomset-0.0.6/src/dicomset/utils.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.5/src/dicomset.egg-info/SOURCES.txt` & `dicomset-0.0.6/src/dicomset.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -85,10 +85,20 @@
 src/dicomset/reporting/wandb_reporter.py
 src/dicomset/reporting/dataset/__init__.py
 src/dicomset/reporting/dataset/dataset.py
 src/dicomset/reporting/dataset/dicom.py
 src/dicomset/reporting/dataset/nifti.py
 src/dicomset/reporting/dataset/nrrd.py
 src/dicomset/reporting/dataset/training.py
+src/dicomset/transforms/__init__.py
+src/dicomset/transforms/crop.py
+src/dicomset/transforms/custom.py
+src/dicomset/transforms/random_elastic_deformation.py
+src/dicomset/transforms/random_intensity.py
+src/dicomset/transforms/random_resample.py
+src/dicomset/transforms/random_rotation.py
+src/dicomset/transforms/random_translation.py
+src/dicomset/transforms/resample.py
+src/dicomset/transforms/translate.py
 src/dicomset/types/__init__.py
 src/dicomset/types/parser.py
 src/dicomset/types/types.py
```

