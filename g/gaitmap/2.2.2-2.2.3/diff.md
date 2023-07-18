# Comparing `tmp/gaitmap-2.2.2.tar.gz` & `tmp/gaitmap-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap-2.2.2.tar", max compression
+gzip compressed data, was "gaitmap-2.2.3.tar", max compression
```

## Comparing `gaitmap-2.2.2.tar` & `gaitmap-2.2.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2032 2023-06-22 14:30:42.420161 gaitmap-2.2.2/LICENSE
--rw-r--r--   0        0        0    10679 2023-06-22 14:30:42.420161 gaitmap-2.2.2/README.md
--rw-r--r--   0        0        0       69 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/__init__.py
--rw-r--r--   0        0        0      164 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/_event_detection_common/__init__.py
--rw-r--r--   0        0        0     7510 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/_event_detection_common/_event_detection_mixin.py
--rw-r--r--   0        0        0    12216 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/base.py
--rw-r--r--   0        0        0     1316 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/data_transform/__init__.py
--rw-r--r--   0        0        0    15931 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/data_transform/_base.py
--rw-r--r--   0        0        0    12004 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/data_transform/_feature_transform.py
--rw-r--r--   0        0        0     3969 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/data_transform/_filter.py
--rw-r--r--   0        0        0    15524 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/data_transform/_scaler.py
--rw-r--r--   0        0        0      765 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/evaluation_utils/__init__.py
--rw-r--r--   0        0        0     6326 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/evaluation_utils/event_detection.py
--rw-r--r--   0        0        0    28925 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/evaluation_utils/parameter_errors.py
--rw-r--r--   0        0        0    11515 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/evaluation_utils/scores.py
--rw-r--r--   0        0        0    22255 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/evaluation_utils/stride_segmentation.py
--rw-r--r--   0        0        0      702 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/event_detection/__init__.py
--rw-r--r--   0        0        0    19385 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/event_detection/_herzer_event_detection.py
--rw-r--r--   0        0        0     6727 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/example_data.py
--rw-r--r--   0        0        0      542 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/gait_detection/__init__.py
--rw-r--r--   0        0        0      350 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/parameters/__init__.py
--rw-r--r--   0        0        0    21722 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/parameters/_spatial_parameters.py
--rw-r--r--   0        0        0     7836 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/parameters/_temporal_parameters.py
--rw-r--r--   0        0        0      287 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/preprocessing/__init__.py
--rw-r--r--   0        0        0      785 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0     5094 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
--rw-r--r--   0        0        0     3940 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
--rw-r--r--   0        0        0     6635 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
--rw-r--r--   0        0        0     1732 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/stride_segmentation/__init__.py
--rw-r--r--   0        0        0    14875 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/stride_segmentation/_roi_stride_segmentation.py
--rw-r--r--   0        0        0     2713 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/stride_segmentation/_utils.py
--rw-r--r--   0        0        0     1181 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/stride_segmentation/hmm.py
--rw-r--r--   0        0        0     1029 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0    21419 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
--rw-r--r--   0        0        0     9438 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
--rw-r--r--   0        0        0    10746 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
--rw-r--r--   0        0        0      317 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
--rw-r--r--   0        0        0     8096 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
--rw-r--r--   0        0        0     4858 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
--rw-r--r--   0        0        0      618 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0     7841 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
--rw-r--r--   0        0        0      243 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
--rw-r--r--   0        0        0    13664 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
--rw-r--r--   0        0        0    16637 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
--rw-r--r--   0        0        0       41 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/__init__.py
--rw-r--r--   0        0        0     1857 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/_algo_helper.py
--rw-r--r--   0        0        0     4695 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/_datatype_validation_helper.py
--rw-r--r--   0        0        0     1195 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/_gaitmap_mad.py
--rw-r--r--   0        0        0      381 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/_types.py
--rw-r--r--   0        0        0    17992 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/array_handling.py
--rw-r--r--   0        0        0     2555 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/consts.py
--rw-r--r--   0        0        0     6284 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/coordinate_conversion.py
--rw-r--r--   0        0        0    48845 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/datatype_helper.py
--rw-r--r--   0        0        0     1089 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/exceptions.py
--rw-r--r--   0        0        0     1865 2023-06-22 14:30:42.488161 gaitmap-2.2.2/gaitmap/utils/fast_quaternion_math.py
--rw-r--r--   0        0        0    18908 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/utils/rotations.py
--rw-r--r--   0        0        0     2372 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/utils/signal_processing.py
--rw-r--r--   0        0        0    14377 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/utils/static_moment_detection.py
--rw-r--r--   0        0        0     8512 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/utils/stride_list_conversion.py
--rw-r--r--   0        0        0     4115 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/utils/vector_math.py
--rw-r--r--   0        0        0      670 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/zupt_detection/__init__.py
--rw-r--r--   0        0        0     1582 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/zupt_detection/_base.py
--rw-r--r--   0        0        0     3068 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/zupt_detection/_combo_zupt_detector.py
--rw-r--r--   0        0        0    21964 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/zupt_detection/_moving_window_zupt_detector.py
--rw-r--r--   0        0        0     4897 2023-06-22 14:30:42.492161 gaitmap-2.2.2/gaitmap/zupt_detection/_stride_event_zupt_detector.py
--rw-r--r--   0        0        0     5175 2023-06-22 14:30:42.496161 gaitmap-2.2.2/pyproject.toml
--rw-r--r--   0        0        0    12012 1970-01-01 00:00:00.000000 gaitmap-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2032 2023-07-18 11:14:03.241988 gaitmap-2.2.3/LICENSE
+-rw-r--r--   0        0        0    10679 2023-07-18 11:14:03.241988 gaitmap-2.2.3/README.md
+-rw-r--r--   0        0        0       69 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/_event_detection_common/__init__.py
+-rw-r--r--   0        0        0     7510 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/_event_detection_common/_event_detection_mixin.py
+-rw-r--r--   0        0        0    12216 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/base.py
+-rw-r--r--   0        0        0     1316 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/data_transform/__init__.py
+-rw-r--r--   0        0        0    15931 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/data_transform/_base.py
+-rw-r--r--   0        0        0    12004 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/data_transform/_feature_transform.py
+-rw-r--r--   0        0        0     3969 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/data_transform/_filter.py
+-rw-r--r--   0        0        0    15524 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/data_transform/_scaler.py
+-rw-r--r--   0        0        0      765 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/evaluation_utils/__init__.py
+-rw-r--r--   0        0        0     6326 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/evaluation_utils/event_detection.py
+-rw-r--r--   0        0        0    28925 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/evaluation_utils/parameter_errors.py
+-rw-r--r--   0        0        0    11515 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/evaluation_utils/scores.py
+-rw-r--r--   0        0        0    22255 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/evaluation_utils/stride_segmentation.py
+-rw-r--r--   0        0        0      702 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/event_detection/__init__.py
+-rw-r--r--   0        0        0    19385 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/event_detection/_herzer_event_detection.py
+-rw-r--r--   0        0        0     6727 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/example_data.py
+-rw-r--r--   0        0        0      542 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/gait_detection/__init__.py
+-rw-r--r--   0        0        0      350 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/parameters/__init__.py
+-rw-r--r--   0        0        0    21773 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/parameters/_spatial_parameters.py
+-rw-r--r--   0        0        0     7836 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/parameters/_temporal_parameters.py
+-rw-r--r--   0        0        0      287 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/preprocessing/__init__.py
+-rw-r--r--   0        0        0      785 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0     5094 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
+-rw-r--r--   0        0        0     3940 2023-07-18 11:14:03.309987 gaitmap-2.2.3/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
+-rw-r--r--   0        0        0     6635 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
+-rw-r--r--   0        0        0     1732 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0    14875 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/stride_segmentation/_roi_stride_segmentation.py
+-rw-r--r--   0        0        0     2713 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/stride_segmentation/_utils.py
+-rw-r--r--   0        0        0     1181 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/stride_segmentation/hmm.py
+-rw-r--r--   0        0        0     1029 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0    21419 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
+-rw-r--r--   0        0        0     9438 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
+-rw-r--r--   0        0        0    10746 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
+-rw-r--r--   0        0        0      317 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
+-rw-r--r--   0        0        0     8096 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
+-rw-r--r--   0        0        0     4858 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
+-rw-r--r--   0        0        0      618 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0     7841 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
+-rw-r--r--   0        0        0      243 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
+-rw-r--r--   0        0        0    13664 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
+-rw-r--r--   0        0        0    16637 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
+-rw-r--r--   0        0        0       41 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/__init__.py
+-rw-r--r--   0        0        0     1857 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/_algo_helper.py
+-rw-r--r--   0        0        0     4695 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/_datatype_validation_helper.py
+-rw-r--r--   0        0        0     1195 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/_gaitmap_mad.py
+-rw-r--r--   0        0        0      381 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/_types.py
+-rw-r--r--   0        0        0    17992 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/array_handling.py
+-rw-r--r--   0        0        0     2555 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/consts.py
+-rw-r--r--   0        0        0     6284 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/coordinate_conversion.py
+-rw-r--r--   0        0        0    48845 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/datatype_helper.py
+-rw-r--r--   0        0        0     1089 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/exceptions.py
+-rw-r--r--   0        0        0     1865 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/fast_quaternion_math.py
+-rw-r--r--   0        0        0    18908 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/rotations.py
+-rw-r--r--   0        0        0     2372 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/signal_processing.py
+-rw-r--r--   0        0        0    14377 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/static_moment_detection.py
+-rw-r--r--   0        0        0     8512 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/stride_list_conversion.py
+-rw-r--r--   0        0        0     4115 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/utils/vector_math.py
+-rw-r--r--   0        0        0      670 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/zupt_detection/__init__.py
+-rw-r--r--   0        0        0     1582 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/zupt_detection/_base.py
+-rw-r--r--   0        0        0     3068 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/zupt_detection/_combo_zupt_detector.py
+-rw-r--r--   0        0        0    21964 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/zupt_detection/_moving_window_zupt_detector.py
+-rw-r--r--   0        0        0     4897 2023-07-18 11:14:03.313988 gaitmap-2.2.3/gaitmap/zupt_detection/_stride_event_zupt_detector.py
+-rw-r--r--   0        0        0     5175 2023-07-18 11:14:03.317988 gaitmap-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0    12012 1970-01-01 00:00:00.000000 gaitmap-2.2.3/PKG-INFO
```

### Comparing `gaitmap-2.2.2/LICENSE` & `gaitmap-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/README.md` & `gaitmap-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/_event_detection_common/_event_detection_mixin.py` & `gaitmap-2.2.3/gaitmap/_event_detection_common/_event_detection_mixin.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/base.py` & `gaitmap-2.2.3/gaitmap/base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/data_transform/__init__.py` & `gaitmap-2.2.3/gaitmap/data_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/data_transform/_base.py` & `gaitmap-2.2.3/gaitmap/data_transform/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/data_transform/_feature_transform.py` & `gaitmap-2.2.3/gaitmap/data_transform/_feature_transform.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/data_transform/_filter.py` & `gaitmap-2.2.3/gaitmap/data_transform/_filter.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/data_transform/_scaler.py` & `gaitmap-2.2.3/gaitmap/data_transform/_scaler.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/evaluation_utils/__init__.py` & `gaitmap-2.2.3/gaitmap/evaluation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/evaluation_utils/event_detection.py` & `gaitmap-2.2.3/gaitmap/evaluation_utils/event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/evaluation_utils/parameter_errors.py` & `gaitmap-2.2.3/gaitmap/evaluation_utils/parameter_errors.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/evaluation_utils/scores.py` & `gaitmap-2.2.3/gaitmap/evaluation_utils/scores.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/evaluation_utils/stride_segmentation.py` & `gaitmap-2.2.3/gaitmap/evaluation_utils/stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/event_detection/__init__.py` & `gaitmap-2.2.3/gaitmap/event_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/event_detection/_herzer_event_detection.py` & `gaitmap-2.2.3/gaitmap/event_detection/_herzer_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/example_data.py` & `gaitmap-2.2.3/gaitmap/example_data.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/gait_detection/__init__.py` & `gaitmap-2.2.3/gaitmap/gait_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/parameters/_spatial_parameters.py` & `gaitmap-2.2.3/gaitmap/parameters/_spatial_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,14 +463,16 @@
 
     x1 = (x1,y1), x2 = (x2,y2) define the line
     x = (x0,y0) is the point the distance is computed to
     d =  abs((x2-x1)(y1-y0) - (x1-x0)(y2-y1))/sqrt((x2-x1)**2+(y2-y1)**2)
       =  abs((x2-x1)(y1-y0) - (x1-x0)(y2-y1))/stride_length
 
     """
+    if positions.empty:
+        return pd.Series()
     start = positions.groupby(level="s_id").first()
     end = positions.groupby(level="s_id").last()
     stride_length = _calc_stride_length(positions)
 
     def _calc_per_stride(start, end, length, data):
         excursion = (
             (end["pos_x"] - start["pos_x"]) * (start["pos_y"] - data["pos_y"])
```

### Comparing `gaitmap-2.2.2/gaitmap/parameters/_temporal_parameters.py` & `gaitmap-2.2.3/gaitmap/parameters/_temporal_parameters.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/preprocessing/sensor_alignment/__init__.py` & `gaitmap-2.2.3/gaitmap/preprocessing/sensor_alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py` & `gaitmap-2.2.3/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py` & `gaitmap-2.2.3/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py` & `gaitmap-2.2.3/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/stride_segmentation/__init__.py` & `gaitmap-2.2.3/gaitmap/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/stride_segmentation/_roi_stride_segmentation.py` & `gaitmap-2.2.3/gaitmap/stride_segmentation/_roi_stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/stride_segmentation/_utils.py` & `gaitmap-2.2.3/gaitmap/stride_segmentation/_utils.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/stride_segmentation/hmm.py` & `gaitmap-2.2.3/gaitmap/stride_segmentation/hmm.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/__init__.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/_region_level_trajectory.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/_region_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/position_methods/__init__.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/position_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py` & `gaitmap-2.2.3/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/_algo_helper.py` & `gaitmap-2.2.3/gaitmap/utils/_algo_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/_datatype_validation_helper.py` & `gaitmap-2.2.3/gaitmap/utils/_datatype_validation_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/_gaitmap_mad.py` & `gaitmap-2.2.3/gaitmap/utils/_gaitmap_mad.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/array_handling.py` & `gaitmap-2.2.3/gaitmap/utils/array_handling.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/consts.py` & `gaitmap-2.2.3/gaitmap/utils/consts.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/coordinate_conversion.py` & `gaitmap-2.2.3/gaitmap/utils/coordinate_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/datatype_helper.py` & `gaitmap-2.2.3/gaitmap/utils/datatype_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/exceptions.py` & `gaitmap-2.2.3/gaitmap/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/fast_quaternion_math.py` & `gaitmap-2.2.3/gaitmap/utils/fast_quaternion_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/rotations.py` & `gaitmap-2.2.3/gaitmap/utils/rotations.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/signal_processing.py` & `gaitmap-2.2.3/gaitmap/utils/signal_processing.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/static_moment_detection.py` & `gaitmap-2.2.3/gaitmap/utils/static_moment_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/stride_list_conversion.py` & `gaitmap-2.2.3/gaitmap/utils/stride_list_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/utils/vector_math.py` & `gaitmap-2.2.3/gaitmap/utils/vector_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/zupt_detection/__init__.py` & `gaitmap-2.2.3/gaitmap/zupt_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/zupt_detection/_base.py` & `gaitmap-2.2.3/gaitmap/zupt_detection/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/zupt_detection/_combo_zupt_detector.py` & `gaitmap-2.2.3/gaitmap/zupt_detection/_combo_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/zupt_detection/_moving_window_zupt_detector.py` & `gaitmap-2.2.3/gaitmap/zupt_detection/_moving_window_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/gaitmap/zupt_detection/_stride_event_zupt_detector.py` & `gaitmap-2.2.3/gaitmap/zupt_detection/_stride_event_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.2.2/pyproject.toml` & `gaitmap-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap"
-version = "2.2.2"
+version = "2.2.3"
 description = "The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis."
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
```

### Comparing `gaitmap-2.2.2/PKG-INFO` & `gaitmap-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap
-Version: 2.2.2
+Version: 2.2.3
 Summary: The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis.
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: MIT
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

