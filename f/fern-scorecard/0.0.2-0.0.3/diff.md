# Comparing `tmp/fern_scorecard-0.0.2.tar.gz` & `tmp/fern_scorecard-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_scorecard-0.0.2.tar", max compression
+gzip compressed data, was "fern_scorecard-0.0.3.tar", max compression
```

## Comparing `fern_scorecard-0.0.2.tar` & `fern_scorecard-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0        0 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/README.md
--rw-r--r--   0        0        0      378 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      519 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/__init__.py
--rw-r--r--   0        0        0     5036 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/client.py
--rw-r--r--   0        0        0      348 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      165 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/environment.py
--rw-r--r--   0        0        0      170 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/py.typed
--rw-r--r--   0        0        0      152 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/resources/runs/__init__.py
--rw-r--r--   0        0        0     5307 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/resources/runs/client.py
--rw-r--r--   0        0        0       65 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/resources/testrecords/__init__.py
--rw-r--r--   0        0        0     7727 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/resources/testrecords/client.py
--rw-r--r--   0        0        0       65 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/resources/testset/__init__.py
--rw-r--r--   0        0        0     2673 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/resources/testset/client.py
--rw-r--r--   0        0        0      361 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/types/__init__.py
--rw-r--r--   0        0        0      843 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/types/http_validation_error.py
--rw-r--r--   0        0        0      794 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/types/model_params.py
--rw-r--r--   0        0        0      869 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-18 10:22:11.420694 fern_scorecard-0.0.2/src/scorecard/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 fern_scorecard-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3326 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/README.md
+-rw-r--r--   0        0        0      378 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      519 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/__init__.py
+-rw-r--r--   0        0        0     5036 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/client.py
+-rw-r--r--   0        0        0      348 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      165 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/environment.py
+-rw-r--r--   0        0        0      170 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/py.typed
+-rw-r--r--   0        0        0      152 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/resources/runs/__init__.py
+-rw-r--r--   0        0        0     5307 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/resources/runs/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/resources/testrecords/__init__.py
+-rw-r--r--   0        0        0     7727 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/resources/testrecords/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/resources/testset/__init__.py
+-rw-r--r--   0        0        0     2673 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/resources/testset/client.py
+-rw-r--r--   0        0        0      361 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/types/http_validation_error.py
+-rw-r--r--   0        0        0      794 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/types/model_params.py
+-rw-r--r--   0        0        0      869 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-18 10:34:05.496625 fern_scorecard-0.0.3/src/scorecard/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 fern_scorecard-0.0.3/PKG-INFO
```

### Comparing `fern_scorecard-0.0.2/src/scorecard/__init__.py` & `fern_scorecard-0.0.3/src/scorecard/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_scorecard-0.0.2/src/scorecard/client.py` & `fern_scorecard-0.0.3/src/scorecard/client.py`

 * *Files identical despite different names*

### Comparing `fern_scorecard-0.0.2/src/scorecard/core/datetime_utils.py` & `fern_scorecard-0.0.3/src/scorecard/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_scorecard-0.0.2/src/scorecard/core/jsonable_encoder.py` & `fern_scorecard-0.0.3/src/scorecard/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_scorecard-0.0.2/src/scorecard/resources/runs/client.py` & `fern_scorecard-0.0.3/src/scorecard/resources/runs/client.py`

 * *Files identical despite different names*

### Comparing `fern_scorecard-0.0.2/src/scorecard/resources/testrecords/client.py` & `fern_scorecard-0.0.3/src/scorecard/resources/testrecords/client.py`

 * *Files identical despite different names*

### Comparing `fern_scorecard-0.0.2/src/scorecard/resources/testset/client.py` & `fern_scorecard-0.0.3/src/scorecard/resources/testset/client.py`

 * *Files identical despite different names*

### Comparing `fern_scorecard-0.0.2/src/scorecard/types/http_validation_error.py` & `fern_scorecard-0.0.3/src/scorecard/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_scorecard-0.0.2/src/scorecard/types/model_params.py` & `fern_scorecard-0.0.3/src/scorecard/types/model_params.py`

 * *Files identical despite different names*

### Comparing `fern_scorecard-0.0.2/src/scorecard/types/validation_error.py` & `fern_scorecard-0.0.3/src/scorecard/types/validation_error.py`

 * *Files identical despite different names*

