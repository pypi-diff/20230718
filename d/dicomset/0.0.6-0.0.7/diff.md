# Comparing `tmp/dicomset-0.0.6.tar.gz` & `tmp/dicomset-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomset-0.0.6.tar", last modified: Tue Jul 18 04:30:16 2023, max compression
+gzip compressed data, was "dicomset-0.0.7.tar", last modified: Tue Jul 18 04:35:27 2023, max compression
```

## Comparing `dicomset-0.0.6.tar` & `dicomset-0.0.7.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.526393 dicomset-0.0.6/
--rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 04:30:16.526232 dicomset-0.0.6/PKG-INFO
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:21.000000 dicomset-0.0.6/README.md
--rw-r--r--   0 clarkbrett (990701463) 678807148      597 2023-07-18 04:08:12.000000 dicomset-0.0.6/pyproject.toml
--rw-r--r--   0 clarkbrett (990701463) 678807148       38 2023-07-18 04:30:16.526435 dicomset-0.0.6/setup.cfg
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.497187 dicomset-0.0.6/src/
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.500800 dicomset-0.0.6/src/dicomset/
--rw-r--r--   0 clarkbrett (990701463) 678807148     2042 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/config.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.502362 dicomset-0.0.6/src/dicomset/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148     3879 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      795 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dataset.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.507349 dicomset-0.0.6/src/dicomset/dataset/dicom/
--rw-r--r--   0 clarkbrett (990701463) 678807148      825 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     4000 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/ct_series.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10067 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      170 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_file.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     7243 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_patient.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      458 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_series.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     9574 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_study.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    18397 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/index.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1638 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2965 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/region_map.py
--rw-r--r--   0 clarkbrett (990701463) 678807148       71 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/region_policy.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      283 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/roi_data.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3488 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtdose.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtdose_series.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1487 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtplan.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtplan_series.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10605 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    22735 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct_converter.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2711 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct_series.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.508167 dicomset-0.0.6/src/dicomset/dataset/nifti/
--rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nifti/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     5163 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nifti/nifti_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     5670 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nifti/nifti_patient.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.509303 dicomset-0.0.6/src/dicomset/dataset/nrrd/
--rw-r--r--   0 clarkbrett (990701463) 678807148      698 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nrrd/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     4055 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nrrd/nrrd_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     4380 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/nrrd/nrrd_patient.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.510087 dicomset-0.0.6/src/dicomset/dataset/other/
--rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/other/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1198 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/other/other_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      777 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/other/other_sample.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.510925 dicomset-0.0.6/src/dicomset/dataset/training/
--rw-r--r--   0 clarkbrett (990701463) 678807148     1074 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/training/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     5404 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/training/training_dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3419 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/dataset/training/training_sample.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.511427 dicomset-0.0.6/src/dicomset/evaluation/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.512672 dicomset-0.0.6/src/dicomset/evaluation/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    11935 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/dicom.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    18224 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    19129 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/nrrd.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3893 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/dataset/training.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10858 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/evaluation/model_evaluator.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.513589 dicomset-0.0.6/src/dicomset/geometry/
--rw-r--r--   0 clarkbrett (990701463) 678807148      187 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/geometry/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      328 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/geometry/box.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      992 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/geometry/centre.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2391 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/geometry/extent.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.513854 dicomset-0.0.6/src/dicomset/logging/
--rw-r--r--   0 clarkbrett (990701463) 678807148     1953 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/logging/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.514989 dicomset-0.0.6/src/dicomset/metrics/
--rw-r--r--   0 clarkbrett (990701463) 678807148      769 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3894 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/contrast.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1586 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/dice.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10609 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/distances.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      424 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/metrics/volume.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.515862 dicomset-0.0.6/src/dicomset/plotting/
--rw-r--r--   0 clarkbrett (990701463) 678807148       61 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.517104 dicomset-0.0.6/src/dicomset/plotting/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148     3300 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/dicom.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    19556 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    19808 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/nrrd.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      455 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/other.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3104 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/dataset/training.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    67448 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/plotter.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    10901 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/plotting/results.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.517330 dicomset-0.0.6/src/dicomset/processing/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.518696 dicomset-0.0.6/src/dicomset/processing/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      166 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     7540 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/dicom.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    21722 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    21758 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/nrrd.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3004 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/processing/dataset/other.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.519789 dicomset-0.0.6/src/dicomset/regions/
--rw-r--r--   0 clarkbrett (990701463) 678807148      821 2023-07-18 03:51:55.000000 dicomset-0.0.6/src/dicomset/regions/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1084 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/regions/colours.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1321 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/regions/list.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1527 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/regions/regions.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1264 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/regions/tolerances.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.521298 dicomset-0.0.6/src/dicomset/reporting/
--rw-r--r--   0 clarkbrett (990701463) 678807148       97 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/__init__.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.522690 dicomset-0.0.6/src/dicomset/reporting/dataset/
--rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2737 2023-07-18 03:07:13.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/dataset.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     8233 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/dicom.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    30026 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/nifti.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    30008 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/nrrd.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    13148 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/dataset/training.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3524 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/gpu_usage.py
--rw-r--r--   0 clarkbrett (990701463) 678807148    12593 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/loaders.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2716 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/models.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2012 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/reporter.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1271 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/tensorboard_reporter.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1817 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/reporting/wandb_reporter.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.525406 dicomset-0.0.6/src/dicomset/transforms/
--rw-r--r--   0 clarkbrett (990701463) 678807148      401 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     9580 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/crop.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      504 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/custom.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      360 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_elastic_deformation.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2601 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_intensity.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     2484 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_resample.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3462 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_rotation.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3328 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/random_translation.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     3637 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/resample.py
--rw-r--r--   0 clarkbrett (990701463) 678807148      174 2023-07-18 04:07:27.000000 dicomset-0.0.6/src/dicomset/transforms/translate.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.526011 dicomset-0.0.6/src/dicomset/types/
--rw-r--r--   0 clarkbrett (990701463) 678807148       73 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/types/__init__.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1844 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/types/parser.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     1006 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/types/types.py
--rw-r--r--   0 clarkbrett (990701463) 678807148     9833 2023-07-18 03:06:08.000000 dicomset-0.0.6/src/dicomset/utils.py
-drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:30:16.501854 dicomset-0.0.6/src/dicomset.egg-info/
--rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 04:30:16.000000 dicomset-0.0.6/src/dicomset.egg-info/PKG-INFO
--rw-r--r--   0 clarkbrett (990701463) 678807148     3933 2023-07-18 04:30:16.000000 dicomset-0.0.6/src/dicomset.egg-info/SOURCES.txt
--rw-r--r--   0 clarkbrett (990701463) 678807148        1 2023-07-18 04:30:16.000000 dicomset-0.0.6/src/dicomset.egg-info/dependency_links.txt
--rw-r--r--   0 clarkbrett (990701463) 678807148        9 2023-07-18 04:30:16.000000 dicomset-0.0.6/src/dicomset.egg-info/top_level.txt
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.379433 dicomset-0.0.7/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 04:35:27.379264 dicomset-0.0.7/PKG-INFO
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:21.000000 dicomset-0.0.7/README.md
+-rw-r--r--   0 clarkbrett (990701463) 678807148      597 2023-07-18 04:35:05.000000 dicomset-0.0.7/pyproject.toml
+-rw-r--r--   0 clarkbrett (990701463) 678807148       38 2023-07-18 04:35:27.379475 dicomset-0.0.7/setup.cfg
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.348344 dicomset-0.0.7/src/
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.353858 dicomset-0.0.7/src/dicomset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2042 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/config.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.355454 dicomset-0.0.7/src/dicomset/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3879 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      795 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dataset.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.360710 dicomset-0.0.7/src/dicomset/dataset/dicom/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      825 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     4000 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/ct_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10071 2023-07-18 04:34:45.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/dicom_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      170 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/dicom_file.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     7243 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/dicom_patient.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      458 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/dicom_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     9574 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/dicom_study.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    18397 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/index.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1638 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2965 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/region_map.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148       71 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/region_policy.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      283 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/roi_data.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3488 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/rtdose.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/rtdose_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1487 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/rtplan.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1861 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/rtplan_series.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10605 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/rtstruct.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    22735 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/rtstruct_converter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2711 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/dicom/rtstruct_series.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.361399 dicomset-0.0.7/src/dicomset/dataset/nifti/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/nifti/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     5163 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/nifti/nifti_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     5670 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/nifti/nifti_patient.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.362117 dicomset-0.0.7/src/dicomset/dataset/nrrd/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      698 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/nrrd/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     4055 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/nrrd/nrrd_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     4380 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/nrrd/nrrd_patient.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.362804 dicomset-0.0.7/src/dicomset/dataset/other/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      704 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/other/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1198 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/other/other_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      777 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/other/other_sample.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.363652 dicomset-0.0.7/src/dicomset/dataset/training/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1074 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/training/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     5404 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/training/training_dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3419 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/dataset/training/training_sample.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.364252 dicomset-0.0.7/src/dicomset/evaluation/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/evaluation/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.365389 dicomset-0.0.7/src/dicomset/evaluation/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/evaluation/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    11935 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/evaluation/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    18224 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/evaluation/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    19129 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/evaluation/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3893 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/evaluation/dataset/training.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10858 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/evaluation/model_evaluator.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.366304 dicomset-0.0.7/src/dicomset/geometry/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      187 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/geometry/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      328 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/geometry/box.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      992 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/geometry/centre.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2391 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/geometry/extent.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.366536 dicomset-0.0.7/src/dicomset/logging/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1953 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/logging/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.367750 dicomset-0.0.7/src/dicomset/metrics/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      769 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/metrics/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3894 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/metrics/contrast.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1586 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/metrics/dice.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10609 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/metrics/distances.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      424 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/metrics/volume.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.368544 dicomset-0.0.7/src/dicomset/plotting/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       61 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/plotting/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.369682 dicomset-0.0.7/src/dicomset/plotting/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3300 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/plotting/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    19556 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/plotting/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    19808 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/plotting/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      455 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/plotting/dataset/other.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3104 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/plotting/dataset/training.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    67448 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/plotting/plotter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    10901 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/plotting/results.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.369945 dicomset-0.0.7/src/dicomset/processing/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/processing/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.371224 dicomset-0.0.7/src/dicomset/processing/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/processing/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      166 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/processing/dataset/dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     7540 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/processing/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    21722 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/processing/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    21758 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/processing/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3004 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/processing/dataset/other.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.372505 dicomset-0.0.7/src/dicomset/regions/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      821 2023-07-18 03:51:55.000000 dicomset-0.0.7/src/dicomset/regions/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1084 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/regions/colours.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1321 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/regions/list.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1527 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/regions/regions.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1264 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/regions/tolerances.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.374265 dicomset-0.0.7/src/dicomset/reporting/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       97 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.375837 dicomset-0.0.7/src/dicomset/reporting/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/dataset/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2737 2023-07-18 03:07:13.000000 dicomset-0.0.7/src/dicomset/reporting/dataset/dataset.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     8233 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/dataset/dicom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    30026 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/dataset/nifti.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    30008 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/dataset/nrrd.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    13148 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/dataset/training.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3524 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/gpu_usage.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148    12593 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/loaders.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2716 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/models.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2012 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/reporter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1271 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/tensorboard_reporter.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1817 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/reporting/wandb_reporter.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.378398 dicomset-0.0.7/src/dicomset/transforms/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      401 2023-07-18 04:07:27.000000 dicomset-0.0.7/src/dicomset/transforms/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     9588 2023-07-18 04:34:45.000000 dicomset-0.0.7/src/dicomset/transforms/crop.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      504 2023-07-18 04:07:27.000000 dicomset-0.0.7/src/dicomset/transforms/custom.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      360 2023-07-18 04:07:27.000000 dicomset-0.0.7/src/dicomset/transforms/random_elastic_deformation.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2601 2023-07-18 04:07:27.000000 dicomset-0.0.7/src/dicomset/transforms/random_intensity.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2484 2023-07-18 04:07:27.000000 dicomset-0.0.7/src/dicomset/transforms/random_resample.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3462 2023-07-18 04:07:27.000000 dicomset-0.0.7/src/dicomset/transforms/random_rotation.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3328 2023-07-18 04:07:27.000000 dicomset-0.0.7/src/dicomset/transforms/random_translation.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3641 2023-07-18 04:34:45.000000 dicomset-0.0.7/src/dicomset/transforms/resample.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148      174 2023-07-18 04:07:27.000000 dicomset-0.0.7/src/dicomset/transforms/translate.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.379014 dicomset-0.0.7/src/dicomset/types/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       73 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/types/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1844 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/types/parser.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1006 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/types/types.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     9833 2023-07-18 03:06:08.000000 dicomset-0.0.7/src/dicomset/utils.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 04:35:27.354874 dicomset-0.0.7/src/dicomset.egg-info/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      496 2023-07-18 04:35:27.000000 dicomset-0.0.7/src/dicomset.egg-info/PKG-INFO
+-rw-r--r--   0 clarkbrett (990701463) 678807148     3933 2023-07-18 04:35:27.000000 dicomset-0.0.7/src/dicomset.egg-info/SOURCES.txt
+-rw-r--r--   0 clarkbrett (990701463) 678807148        1 2023-07-18 04:35:27.000000 dicomset-0.0.7/src/dicomset.egg-info/dependency_links.txt
+-rw-r--r--   0 clarkbrett (990701463) 678807148        9 2023-07-18 04:35:27.000000 dicomset-0.0.7/src/dicomset.egg-info/top_level.txt
```

### Comparing `dicomset-0.0.6/pyproject.toml` & `dicomset-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dicomset"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Brett Clark", email = "clarkbab@gmail.com" }
 ]
 description = "Python library for DICOM processing and analysis"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `dicomset-0.0.6/src/dicomset/config.py` & `dicomset-0.0.7/src/dicomset/config.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/__init__.py` & `dicomset-0.0.7/src/dicomset/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dataset.py` & `dicomset-0.0.7/src/dicomset/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/__init__.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/ct_series.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/ct_series.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_dataset.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/dicom_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         return self._type
 
     def has_patient(
         self,
         id: PatientID) -> bool:
         return id in self.list_patients()
 
-    # Copied from 'mymi/reporting/dataset/dicom.py' to avoid circular dependency.
+    # Copied from 'dicomset/reporting/dataset/dicom.py' to avoid circular dependency.
     def __load_patient_regions_report(
         self,
         exists_only: bool = False,
         use_mapping: bool = True) -> None:
         filename = 'region-count.csv' if use_mapping else 'region-count-unmapped.csv'
         filepath = os.path.join(self.__path, 'reports', filename)
         if os.path.exists(filepath):
```

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_patient.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/dicom_patient.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/dicom_study.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/dicom_study.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/index.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/index.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/nifti.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/region_map.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/region_map.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/rtdose.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/rtdose.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/rtdose_series.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/rtdose_series.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/rtplan.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/rtplan.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/rtplan_series.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/rtplan_series.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/rtstruct.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct_converter.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/rtstruct_converter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/dicom/rtstruct_series.py` & `dicomset-0.0.7/src/dicomset/dataset/dicom/rtstruct_series.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/nifti/__init__.py` & `dicomset-0.0.7/src/dicomset/dataset/nifti/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/nifti/nifti_dataset.py` & `dicomset-0.0.7/src/dicomset/dataset/nifti/nifti_dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/nifti/nifti_patient.py` & `dicomset-0.0.7/src/dicomset/dataset/nifti/nifti_patient.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/nrrd/__init__.py` & `dicomset-0.0.7/src/dicomset/dataset/nrrd/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/nrrd/nrrd_dataset.py` & `dicomset-0.0.7/src/dicomset/dataset/nrrd/nrrd_dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/nrrd/nrrd_patient.py` & `dicomset-0.0.7/src/dicomset/dataset/nrrd/nrrd_patient.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/other/__init__.py` & `dicomset-0.0.7/src/dicomset/dataset/other/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/other/other_dataset.py` & `dicomset-0.0.7/src/dicomset/dataset/other/other_dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/other/other_sample.py` & `dicomset-0.0.7/src/dicomset/dataset/other/other_sample.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/training/__init__.py` & `dicomset-0.0.7/src/dicomset/dataset/training/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/training/training_dataset.py` & `dicomset-0.0.7/src/dicomset/dataset/training/training_dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/dataset/training/training_sample.py` & `dicomset-0.0.7/src/dicomset/dataset/training/training_sample.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/evaluation/dataset/dicom.py` & `dicomset-0.0.7/src/dicomset/evaluation/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/evaluation/dataset/nifti.py` & `dicomset-0.0.7/src/dicomset/evaluation/dataset/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/evaluation/dataset/nrrd.py` & `dicomset-0.0.7/src/dicomset/evaluation/dataset/nrrd.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/evaluation/dataset/training.py` & `dicomset-0.0.7/src/dicomset/evaluation/dataset/training.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/evaluation/model_evaluator.py` & `dicomset-0.0.7/src/dicomset/evaluation/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/geometry/centre.py` & `dicomset-0.0.7/src/dicomset/geometry/centre.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/geometry/extent.py` & `dicomset-0.0.7/src/dicomset/geometry/extent.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/logging/__init__.py` & `dicomset-0.0.7/src/dicomset/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/metrics/__init__.py` & `dicomset-0.0.7/src/dicomset/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/metrics/contrast.py` & `dicomset-0.0.7/src/dicomset/metrics/contrast.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/metrics/dice.py` & `dicomset-0.0.7/src/dicomset/metrics/dice.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/metrics/distances.py` & `dicomset-0.0.7/src/dicomset/metrics/distances.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/plotting/dataset/dicom.py` & `dicomset-0.0.7/src/dicomset/plotting/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/plotting/dataset/nifti.py` & `dicomset-0.0.7/src/dicomset/plotting/dataset/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/plotting/dataset/nrrd.py` & `dicomset-0.0.7/src/dicomset/plotting/dataset/nrrd.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/plotting/dataset/training.py` & `dicomset-0.0.7/src/dicomset/plotting/dataset/training.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/plotting/plotter.py` & `dicomset-0.0.7/src/dicomset/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/plotting/results.py` & `dicomset-0.0.7/src/dicomset/plotting/results.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/processing/dataset/dicom.py` & `dicomset-0.0.7/src/dicomset/processing/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/processing/dataset/nifti.py` & `dicomset-0.0.7/src/dicomset/processing/dataset/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/processing/dataset/nrrd.py` & `dicomset-0.0.7/src/dicomset/processing/dataset/nrrd.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/processing/dataset/other.py` & `dicomset-0.0.7/src/dicomset/processing/dataset/other.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/regions/__init__.py` & `dicomset-0.0.7/src/dicomset/regions/__init__.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/regions/colours.py` & `dicomset-0.0.7/src/dicomset/regions/colours.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/regions/list.py` & `dicomset-0.0.7/src/dicomset/regions/list.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/regions/regions.py` & `dicomset-0.0.7/src/dicomset/regions/regions.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/regions/tolerances.py` & `dicomset-0.0.7/src/dicomset/regions/tolerances.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/dataset/dataset.py` & `dicomset-0.0.7/src/dicomset/reporting/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/dataset/dicom.py` & `dicomset-0.0.7/src/dicomset/reporting/dataset/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/dataset/nifti.py` & `dicomset-0.0.7/src/dicomset/reporting/dataset/nifti.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/dataset/nrrd.py` & `dicomset-0.0.7/src/dicomset/reporting/dataset/nrrd.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/dataset/training.py` & `dicomset-0.0.7/src/dicomset/reporting/dataset/training.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/gpu_usage.py` & `dicomset-0.0.7/src/dicomset/reporting/gpu_usage.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/loaders.py` & `dicomset-0.0.7/src/dicomset/reporting/loaders.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/models.py` & `dicomset-0.0.7/src/dicomset/reporting/models.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/reporter.py` & `dicomset-0.0.7/src/dicomset/reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/tensorboard_reporter.py` & `dicomset-0.0.7/src/dicomset/reporting/tensorboard_reporter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/reporting/wandb_reporter.py` & `dicomset-0.0.7/src/dicomset/reporting/wandb_reporter.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/transforms/crop.py` & `dicomset-0.0.7/src/dicomset/transforms/crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from typing import Any, Dict, Literal, Optional, Tuple, Union
 
-from mymi.geometry import get_box
-from mymi.types import Box2D, Box3D, ImageSize3D, Point2D, Point3D
+from dicomset.geometry import get_box
+from dicomset.types import Box2D, Box3D, ImageSize3D, Point2D, Point3D
 
 def crop_or_pad_2D(
     data: np.ndarray,
     bounding_box: Box2D,
     fill: Union[float, Literal['min']] = 'min') -> np.ndarray:
     # Convert args to 3D.
     data = np.expand_dims(data, axis=2)
```

### Comparing `dicomset-0.0.6/src/dicomset/transforms/random_intensity.py` & `dicomset-0.0.7/src/dicomset/transforms/random_intensity.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/transforms/random_resample.py` & `dicomset-0.0.7/src/dicomset/transforms/random_resample.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/transforms/random_rotation.py` & `dicomset-0.0.7/src/dicomset/transforms/random_rotation.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/transforms/random_translation.py` & `dicomset-0.0.7/src/dicomset/transforms/random_translation.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/transforms/resample.py` & `dicomset-0.0.7/src/dicomset/transforms/resample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import SimpleITK as sitk
 from typing import Any, Dict, Optional
 
-from mymi import types
+from dicomset import types
 
 def resample_4D(
     input: np.ndarray,
     **kwargs: Dict[str, Any]) -> np.ndarray:
     ds = []
     for d in input:
         d = resample_3D(d, **kwargs)
```

### Comparing `dicomset-0.0.6/src/dicomset/types/parser.py` & `dicomset-0.0.7/src/dicomset/types/parser.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/types/types.py` & `dicomset-0.0.7/src/dicomset/types/types.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset/utils.py` & `dicomset-0.0.7/src/dicomset/utils.py`

 * *Files identical despite different names*

### Comparing `dicomset-0.0.6/src/dicomset.egg-info/SOURCES.txt` & `dicomset-0.0.7/src/dicomset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

