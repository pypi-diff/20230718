# Comparing `tmp/pickled_carrots-1.0.5.tar.gz` & `tmp/pickled_carrots-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickled_carrots-1.0.5.tar", max compression
+gzip compressed data, was "pickled_carrots-1.0.6.tar", max compression
```

## Comparing `pickled_carrots-1.0.5.tar` & `pickled_carrots-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-1.0.5/README.md
--rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-1.0.5/pickled_carrots/DPData.py
--rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-1.0.5/pickled_carrots/DPPlot.py
--rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-1.0.5/pickled_carrots/DPUtil.py
--rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-1.0.5/pickled_carrots/__init__.py
--rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-1.0.5/pickled_carrots/database.py
--rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-1.0.5/pickled_carrots/dataclass.py
--rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-1.0.5/pickled_carrots/mathutil.py
--rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-1.0.5/pickled_carrots/plot.py
--rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-1.0.5/pickled_carrots/resources/event_type_lookup.pickle
--rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-1.0.5/pickled_carrots/vinegar/__init__.py
--rw-r--r--   0        0        0    13845 2023-05-26 13:00:40.817419 pickled_carrots-1.0.5/pickled_carrots/vinegar/core.py
--rw-r--r--   0        0        0     9312 2023-05-29 12:55:11.279181 pickled_carrots-1.0.5/pickled_carrots/vinegar/event.py
--rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-1.0.5/pickled_carrots/vinegar/inventory.py
--rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-1.0.5/pickled_carrots/vinegar/tests/test_read_hsf.py
--rw-r--r--   0        0        0   138987 2023-05-24 17:57:38.942953 pickled_carrots-1.0.5/pickled_carrots/waveforms.py
--rw-r--r--   0        0        0      678 2023-05-29 12:55:31.232108 pickled_carrots-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 pickled_carrots-1.0.5/setup.py
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-1.0.6/README.md
+-rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-1.0.6/pickled_carrots/DPData.py
+-rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-1.0.6/pickled_carrots/DPPlot.py
+-rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-1.0.6/pickled_carrots/DPUtil.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-1.0.6/pickled_carrots/__init__.py
+-rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-1.0.6/pickled_carrots/database.py
+-rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-1.0.6/pickled_carrots/dataclass.py
+-rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-1.0.6/pickled_carrots/mathutil.py
+-rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-1.0.6/pickled_carrots/plot.py
+-rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-1.0.6/pickled_carrots/resources/event_type_lookup.pickle
+-rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-1.0.6/pickled_carrots/vinegar/__init__.py
+-rw-r--r--   0        0        0    13845 2023-05-26 13:00:40.817419 pickled_carrots-1.0.6/pickled_carrots/vinegar/core.py
+-rw-r--r--   0        0        0     9312 2023-05-29 12:55:11.279181 pickled_carrots-1.0.6/pickled_carrots/vinegar/event.py
+-rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-1.0.6/pickled_carrots/vinegar/inventory.py
+-rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-1.0.6/pickled_carrots/vinegar/tests/test_read_hsf.py
+-rw-r--r--   0        0        0   138987 2023-05-24 17:57:38.942953 pickled_carrots-1.0.6/pickled_carrots/waveforms.py
+-rw-r--r--   0        0        0      678 2023-07-18 13:22:15.302246 pickled_carrots-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-1.0.6/PKG-INFO
```

### Comparing `pickled_carrots-1.0.5/README.md` & `pickled_carrots-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/DPData.py` & `pickled_carrots-1.0.6/pickled_carrots/DPData.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/DPPlot.py` & `pickled_carrots-1.0.6/pickled_carrots/DPPlot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/DPUtil.py` & `pickled_carrots-1.0.6/pickled_carrots/DPUtil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/database.py` & `pickled_carrots-1.0.6/pickled_carrots/database.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/dataclass.py` & `pickled_carrots-1.0.6/pickled_carrots/dataclass.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/mathutil.py` & `pickled_carrots-1.0.6/pickled_carrots/mathutil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/plot.py` & `pickled_carrots-1.0.6/pickled_carrots/plot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/resources/event_type_lookup.pickle` & `pickled_carrots-1.0.6/pickled_carrots/resources/event_type_lookup.pickle`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/vinegar/core.py` & `pickled_carrots-1.0.6/pickled_carrots/vinegar/core.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/vinegar/event.py` & `pickled_carrots-1.0.6/pickled_carrots/vinegar/event.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/vinegar/inventory.py` & `pickled_carrots-1.0.6/pickled_carrots/vinegar/inventory.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/vinegar/tests/test_read_hsf.py` & `pickled_carrots-1.0.6/pickled_carrots/vinegar/tests/test_read_hsf.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pickled_carrots/waveforms.py` & `pickled_carrots-1.0.6/pickled_carrots/waveforms.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.5/pyproject.toml` & `pickled_carrots-1.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pickled_carrots"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 authors = ["pickled cattots team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 plotly = "^5.14.1"
```

### Comparing `pickled_carrots-1.0.5/PKG-INFO` & `pickled_carrots-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickled-carrots
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 Author: pickled cattots team
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

