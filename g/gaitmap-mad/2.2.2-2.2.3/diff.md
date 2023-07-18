# Comparing `tmp/gaitmap_mad-2.2.2.tar.gz` & `tmp/gaitmap_mad-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap_mad-2.2.2.tar", max compression
+gzip compressed data, was "gaitmap_mad-2.2.3.tar", max compression
```

## Comparing `gaitmap_mad-2.2.2.tar` & `gaitmap_mad-2.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      734 2023-06-22 14:30:41.260965 gaitmap_mad-2.2.2/LICENSE
--rw-r--r--   0        0        0      597 2023-06-22 14:30:41.260965 gaitmap_mad-2.2.2/README.md
--rw-r--r--   0        0        0      481 2023-06-22 14:30:41.260965 gaitmap_mad-2.2.2/gaitmap_mad/__init__.py
--rw-r--r--   0        0        0      441 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/event_detection/__init__.py
--rw-r--r--   0        0        0     6013 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
--rw-r--r--   0        0        0    14317 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/event_detection/_rampp_event_detection.py
--rw-r--r--   0        0        0      340 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/gait_detection/__init__.py
--rw-r--r--   0        0        0    24779 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
--rw-r--r--   0        0        0      117 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/preprocessing/__init__.py
--rw-r--r--   0        0        0      234 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0    12666 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
--rw-r--r--   0        0        0     1114 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/__init__.py
--rw-r--r--   0        0        0      813 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/__init__.py
--rw-r--r--   0        0        0    15216 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
--rw-r--r--   0        0        0    36773 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
--rw-r--r--   0        0        0     8809 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
--rw-r--r--   0        0        0      436 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
--rw-r--r--   0        0        0     7513 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
--rw-r--r--   0        0        0    15956 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
--rw-r--r--   0        0        0     3589 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
--rw-r--r--   0        0        0     1184 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/__init__.py
--rw-r--r--   0        0        0    10922 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
--rw-r--r--   0        0        0    12589 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
--rw-r--r--   0        0        0        0 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
--rw-r--r--   0        0        0   397824 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
--rw-r--r--   0        0        0    27245 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
--rw-r--r--   0        0        0    19087 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
--rw-r--r--   0        0        0    26902 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_utils.py
--rw-r--r--   0        0        0      265 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0      263 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0    10862 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
--rw-r--r--   0        0        0      589 2023-06-22 14:30:41.264965 gaitmap_mad-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 gaitmap_mad-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/LICENSE
+-rw-r--r--   0        0        0      597 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/README.md
+-rw-r--r--   0        0        0      481 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/__init__.py
+-rw-r--r--   0        0        0      441 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/event_detection/__init__.py
+-rw-r--r--   0        0        0     6013 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
+-rw-r--r--   0        0        0    14317 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/event_detection/_rampp_event_detection.py
+-rw-r--r--   0        0        0      340 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/gait_detection/__init__.py
+-rw-r--r--   0        0        0    24779 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
+-rw-r--r--   0        0        0      117 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/preprocessing/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0    12666 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
+-rw-r--r--   0        0        0     1114 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/__init__.py
+-rw-r--r--   0        0        0    15216 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
+-rw-r--r--   0        0        0    36773 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
+-rw-r--r--   0        0        0     8809 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
+-rw-r--r--   0        0        0      436 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
+-rw-r--r--   0        0        0     7513 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
+-rw-r--r--   0        0        0    15956 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
+-rw-r--r--   0        0        0     3589 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
+-rw-r--r--   0        0        0     1184 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/__init__.py
+-rw-r--r--   0        0        0    10922 2023-07-18 11:14:03.400196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
+-rw-r--r--   0        0        0    12589 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
+-rw-r--r--   0        0        0   397824 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
+-rw-r--r--   0        0        0    27245 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
+-rw-r--r--   0        0        0    19087 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
+-rw-r--r--   0        0        0    26902 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_utils.py
+-rw-r--r--   0        0        0      265 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/gaitmap_mad/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0      263 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0    10862 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
+-rw-r--r--   0        0        0      589 2023-07-18 11:14:03.404196 gaitmap_mad-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 gaitmap_mad-2.2.3/PKG-INFO
```

### Comparing `gaitmap_mad-2.2.2/LICENSE` & `gaitmap_mad-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/README.md` & `gaitmap_mad-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py` & `gaitmap_mad-2.2.3/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/event_detection/_rampp_event_detection.py` & `gaitmap_mad-2.2.3/gaitmap_mad/event_detection/_rampp_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py` & `gaitmap_mad-2.2.3/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py` & `gaitmap_mad-2.2.3/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/__init__.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/__init__.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/__init__.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_simple_model.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_simple_model.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/stride_segmentation/hmm/_utils.py` & `gaitmap_mad-2.2.3/gaitmap_mad/stride_segmentation/hmm/_utils.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py` & `gaitmap_mad-2.2.3/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.2.2/pyproject.toml` & `gaitmap_mad-2.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap_mad"
-version = "2.2.2"
+version = "2.2.3"
 description = "Specific algorithm implementaions by the mad_lab"
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
```

### Comparing `gaitmap_mad-2.2.2/PKG-INFO` & `gaitmap_mad-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap-mad
-Version: 2.2.2
+Version: 2.2.3
 Summary: Specific algorithm implementaions by the mad_lab
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: AGPL-3.0
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

