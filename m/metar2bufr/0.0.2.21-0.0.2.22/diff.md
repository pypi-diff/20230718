# Comparing `tmp/metar2bufr-0.0.2.21.tar.gz` & `tmp/metar2bufr-0.0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metar2bufr-0.0.2.21.tar", last modified: Fri Jul 14 17:44:18 2023, max compression
+gzip compressed data, was "metar2bufr-0.0.2.22.tar", last modified: Mon Jul 17 23:04:07 2023, max compression
```

## Comparing `metar2bufr-0.0.2.21.tar` & `metar2bufr-0.0.2.22.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.492391 metar2bufr-0.0.2.21/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.21/LICENSE
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.21/MANIFEST.in
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-14 17:44:18.492391 metar2bufr-0.0.2.21/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.21/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-07-14 17:43:34.000000 metar2bufr-0.0.2.21/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-14 17:44:18.492391 metar2bufr-0.0.2.21/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.485391 metar2bufr-0.0.2.21/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.488391 metar2bufr-0.0.2.21/src/metar2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.21/src/metar2bufr/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.489391 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.486391 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/build/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.486391 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/build/lib/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.489391 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.490391 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.486391 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/docs/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.490391 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/docs/source/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/docs/source/conf.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/setup.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.490391 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/tests/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.491391 metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/metarDecoders.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/tpg.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/xmlConfig.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/xmlUtilities.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    20665 2023-07-14 17:42:57.000000 metar2bufr-0.0.2.21/src/metar2bufr/metar_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.492391 metar2bufr-0.0.2.21/src/metar2bufr/resources/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.21/src/metar2bufr/resources/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.21/src/metar2bufr/resources/metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.21/src/metar2bufr/resources/metar-mappings2.json
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-14 17:44:18.489391 metar2bufr-0.0.2.21/src/metar2bufr.egg-info/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-14 17:44:18.000000 metar2bufr-0.0.2.21/src/metar2bufr.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1021 2023-07-14 17:44:18.000000 metar2bufr-0.0.2.21/src/metar2bufr.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-14 17:44:18.000000 metar2bufr-0.0.2.21/src/metar2bufr.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-07-14 17:44:18.000000 metar2bufr-0.0.2.21/src/metar2bufr.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.806541 metar2bufr-0.0.2.22/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.22/LICENSE
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.22/MANIFEST.in
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-17 23:04:07.806541 metar2bufr-0.0.2.22/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.22/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-07-17 23:03:21.000000 metar2bufr-0.0.2.22/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-17 23:04:07.806541 metar2bufr-0.0.2.22/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.799541 metar2bufr-0.0.2.22/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.801541 metar2bufr-0.0.2.22/src/metar2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.22/src/metar2bufr/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.802541 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.799541 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/build/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.800541 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/build/lib/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.803541 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.803541 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.800541 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/docs/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.804541 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/docs/source/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/docs/source/conf.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/setup.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.804541 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/tests/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.805541 metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/metarDecoders.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/tpg.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/xmlConfig.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/xmlUtilities.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    23865 2023-07-17 23:02:50.000000 metar2bufr-0.0.2.22/src/metar2bufr/metar_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.805541 metar2bufr-0.0.2.22/src/metar2bufr/resources/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.22/src/metar2bufr/resources/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.22/src/metar2bufr/resources/metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.22/src/metar2bufr/resources/metar-mappings2.json
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-17 23:04:07.802541 metar2bufr-0.0.2.22/src/metar2bufr.egg-info/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-17 23:04:07.000000 metar2bufr-0.0.2.22/src/metar2bufr.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1021 2023-07-17 23:04:07.000000 metar2bufr-0.0.2.22/src/metar2bufr.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-17 23:04:07.000000 metar2bufr-0.0.2.22/src/metar2bufr.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-07-17 23:04:07.000000 metar2bufr-0.0.2.22/src/metar2bufr.egg-info/top_level.txt
```

### Comparing `metar2bufr-0.0.2.21/LICENSE` & `metar2bufr-0.0.2.22/LICENSE`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/PKG-INFO` & `metar2bufr-0.0.2.22/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.21
+Version: 0.0.2.22
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.21/pyproject.toml` & `metar2bufr-0.0.2.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metar2bufr"
-version = "0.0.2.21"
+version = "0.0.2.22"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting METAR TAC messages or an individual METAR message to BUFR4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py` & `metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py` & `metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/csv2bufr/__init__.py` & `metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/csv2bufr/cli.py` & `metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/docs/source/conf.py` & `metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/setup.py` & `metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/setup.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py` & `metar2bufr-0.0.2.22/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/metarDecoders.py` & `metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/metarDecoders.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/tpg.py` & `metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/tpg.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/xmlConfig.py` & `metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/metarDecoder/xmlUtilities.py` & `metar2bufr-0.0.2.22/src/metar2bufr/metarDecoder/xmlUtilities.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/metar_bufr_encoder.py` & `metar2bufr-0.0.2.22/src/metar2bufr/metar_bufr_encoder.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import csv
 from io import StringIO
 import logging
 import json
 import math
 import os
 from csv2bufr import BUFRMessage
+import urllib.request as request
 
 LOGGER = logging.getLogger(__name__)
 
 FAILED = 0
 PASSED = 1
 
 fmh = MD.FMH1()
@@ -29,20 +30,20 @@
 # metar = "METAR KRZT 221615Z AUTO 08007KT 10SM SCT023 OVC038 20/13 A3003 RMK AO2 PWINO="
 # metar = "METAR SPTN 102000Z 23013KT 9999 SCT050 SCT120 27/17 Q1013 RMK PP000="
 # metar = "METAR KOGS 221610Z AUTO VRB03G11KT 10SM FEW049 26/14 A3017 RMK AO2="
 # metar = "METAR KOWX 221615Z AUTO 08010KT 10SM BKN033 23/11 A3006 RMK AO1="
 # metar = "METAR KABC 121755Z AUTO 21016G24KT 180V240 1SM R11/P6000FT -RA BR BKN015 OVC025 06/04 A2990="
 # BKN015 OVC025
 
-metar = "METAR KAFF 121755Z AUTO 21016G24KT 180V240 1SM R11/6000FT R12/P6000 R01L/0600VP6000FT -RA VA PO BKN015 OVC025TCU 06/04 A2990="
+# metar = "METAR KAFF 121755Z AUTO 21016G24KT 180V240 1SM R11/6000FT R12/P6000 R01L/0600VP6000FT -RA VA PO BKN015 OVC025TCU 06/04 A2990="
 # metar = "METAR KABC 121755Z AUTO 21016G24KT 180V240 1SM R11/P6000FT -RA BR BKN015 OVC025 06/04 A2990="
 
 
 _keys = ['report_type',
-         'tsi', 'icao_location_identifier', 'station_type'
+         'tsi', 'icao_location_identifier', 'station_type',
          'year', 'month', 'day', 'hour', 'minute',
          'wind_direction', 'wind_speed', 'gust_speed', 'wind_uom', 'variable_extreme_ccw', 'variable_extreme_cw',
          'visibility', 'visibility_uom', 'visibility_variation', 'visiblity_variation_direction',
         #  'runway_designator_1', 'rvr_1_mean', 'rvr_1_low', 'rvr_1_high', 'tend_1',
         #  'runway_designator_2', 'rvr_2_mean', 'rvr_2_low', 'rvr_2_high', 'tend_2',
         #  'runway_designator_3', 'rvr_3_mean', 'rvr_3_low', 'rvr_3_high', 'tend_3',
         #  'runway_designator_4', 'rvr_4_mean', 'rvr_4_low', 'rvr_4_high', 'tend_4',
@@ -53,41 +54,73 @@
          'air_temp', 'dew_point_temp',
          'altimeter', 'altimeter_uom']
 
 metar_template = dict.fromkeys(_keys)
 
 THISDIR = os.path.dirname(os.path.realpath(__file__))
 MAPPINGS = f"{THISDIR}{os.sep}resources{os.sep}metar-mappings2.json"
+ICAOSTATIONSURL = "https://www.aviationweather.gov/docs/metar/stations.txt"
 
 # MAPPINGS = "/home/alexander.thompson/metar2bufr/src/metar-mappings2.json"
 
 # Load template mappings file, this will be updated for each message.
 with open(MAPPINGS) as fh:
     _mapping = json.load(fh)
 
+def extract_metar(data: str) -> list:
+    if not data.__contains__("="):
+        LOGGER.error((
+            "Delimiters (=) are not present in the string,"
+            " thus unable to identify separate SYNOP reports."
+            ))  # noqa
+        raise ValueError
+    
+    start_position = data.find("METAR")
+    if start_position == -1:
+        start_position = data.find("SPECI")
+        if start_position == -1:
+            raise ValueError("Invalid METAR message. 'METAR' or 'SPECI' could not be found.")
+        
+    data = re.split('=', data[start_position:])
+
+    for i in range(len(data)):
+        data[i] = data[i]+"="
+
+    # print(data[:len(data)-1])
+    return data[:len(data)-1]
+
 def parse_metar(message: str, year: int, month: int) -> dict:
     icaoID = re_ID.match(message).group('id')
     if deu.isUSIdentifier(icaoID):
         decoded = fmh(message)
     else:
         decoded = annex3(message)
 
     output = deepcopy(metar_template)
 
     output['report_type'] = message[0:5]
     output['year'] = year
     output['month'] = month
 
     if 'ident' in decoded:
-        # output['station_id'] = decoded['ident']['str']
+        icao = decoded['ident']['str']
+        output['icao_location_identifier'] = icao
 
-        output['icao_location_identifier'] = decoded['ident']['str']
+        #   match icao id to wigos id using the aviation weather url for station list
+        response = request.urlopen(ICAOSTATIONSURL)
+        html = response.read().decode('utf-8').split('\n')
+        for line in html:
+            if f' {icao} ' in line:
+                # print(line)
+                # print(re.search('[0-9]{5}', line))
+                tsi = str(re.search('[0-9]{5}', line).group())
+                # print(f'Mapping {icao} to {tsi}')
+                break
 
-        try:    # placeholder until we can convert from ICAO to traditional station identifier (tsi)
-            tsi = '72403'
+        try:
             output['tsi'] = tsi
             output['block_no'] = tsi[0:2]
             output['station_no'] = tsi[2:5]
         except Exception:
             tsi = None
             output['tsi'] = None
             output['block_no'] = None
@@ -101,29 +134,48 @@
     # metar station type is binary, either AUTOMATIC (0) or MANNED(1)
     if 'auto' in decoded:
         output['station_type'] = 0
     else:
         output['station_type'] = 1
 
     if 'wind' in decoded:
-        # Metar reports wind speed in knots and direction in degrees, both of which are compatible with bufr
+        wind_uom = decoded['wind']['uom']
+        wind_speed = decoded['wind']['ff']
+        #   this bufr template records wind speed in m/s
+        #   if wind speed reported in m/s, can copy directly to output
+        if wind_uom == 'm/s':
+            output['wind_speed'] = wind_speed
+        #   if wind speed report in knots, need to convert to m/s for bufr
+        elif wind_uom == '[kn_i]':
+            output['wind_speed'] = round(int(wind_speed)*0.514444, 2)
+        
         output['wind_direction'] = decoded['wind']['dd']
-        output['wind_speed'] = decoded['wind']['ff']
+
+        #   perform same unit conversions on gust speed if recorded
         if 'gg' in decoded['wind']:
-            output['gust_speed'] = decoded['wind']['gg']
+            gust_speed = decoded['wind']['gg']
+            if wind_uom == 'm/s':
+                output['gust_speed'] = gust_speed
+            elif wind_uom == '[kn_i]':
+                output['gust_speed'] = round(int(wind_speed)*0.514444, 2)
         output['wind_uom'] = decoded['wind']['uom']
         if 'ccw' in decoded['wind']:
             output['variable_extreme_ccw'] = int(decoded['wind']['ccw'])
         if 'cw' in decoded['wind']:
             output['variable_extreme_cw'] = int(decoded['wind']['cw'])
 
     if 'vsby' in decoded:
-        # Metar reports visibility in statute miles. Need to convert value to meters to be bufr compatible
-        vis_miles = float(decoded['vsby']['value'])
-        output['visibility'] = math.floor(vis_miles * 1609.34)
+        vis_uom = decoded['vsby']['uom']
+        visibility = decoded['vsby']['value']
+        #   bufr uses meters for visibility. if reported in meters, just copy to output
+        if vis_uom == 'm':
+            output['visibility'] == visibility
+        #   if reported in Statute Miles (SM), convert to m/s
+        elif vis_uom == '[mi_i]':
+            output['visibility'] == math.floor(float(visibility)*1609.34)
         output['visibility_uom'] = decoded['vsby']['uom']
 
     # TODO need to incorporate visibility variation as outlined in section 15.6.2 in FM-15 manual
 
     num_rvr = 0
     if 'rvr' in decoded:
         num_rvr = len(decoded['rvr']['str'])
@@ -291,179 +343,203 @@
                 LOGGER.error(e)
 
         fh.close()
         # metadata = metadata_dict[wsi]
     else:
         LOGGER.error("Invalid metadata")
         raise ValueError
-    
-    result = dict()
 
-    mapping = deepcopy(_mapping)
-    # print(mapping)
+    try:
+        messages = extract_metar(data)
+        # print(messages)
+    except Exception as e:
+        LOGGER.error(e)
+        return None
 
+     # Count how many conversions were successful using a dictionary
     conversion_success = {}
 
-    try:
-        msg, num_rvr, num_vrbrvr, num_pcp, num_obv, num_sky = parse_metar(data, year, month)
-        tsi = msg['tsi']
-    except Exception as e:
-        LOGGER.error(f"Error parsing METAR report: {data}. {str(e)}")
-    
-    try:
-        wsi = tsi_mapping[tsi]
-    except Exception:
-        conversion_success[tsi] = False
-        LOGGER.warning(f"Station {tsi} not found in station file")
+    for metar in messages:
+        # print(metar)
+        result = dict()
 
-    # parse WSI to get sections
-    try:
-        wsi_series, wsi_issuer, wsi_issue_number, wsi_local = wsi.split("-")   # noqa
-        # get other required metadata
-        latitude = metadata_dict[wsi]["latitude"]
-        longitude = metadata_dict[wsi]["longitude"]
-        station_height = metadata_dict[wsi]["elevation"]
-        # add these values to the data dictionary
-        msg['_wsi_series'] = wsi_series
-        msg['_wsi_issuer'] = wsi_issuer
-        msg['_wsi_issue_number'] = wsi_issue_number
-        msg['_wsi_local'] = wsi_local
-        msg['_latitude'] = latitude
-        msg['_longitude'] = longitude
-        msg['_station_height'] = station_height
-        conversion_success[tsi] = True
-    except Exception:
-        conversion_success[tsi] = False
-        if wsi == "":
-            LOGGER.warning(f"Missing WSI for station {tsi}")
-        else:
-            LOGGER.warning((f"Invalid WSI ({wsi}) found in station file,"
-                            " unable to parse"))
+        mapping = deepcopy(_mapping)
+        # print(mapping)
 
-    # TODO: update mappings based on number of precipitation observations and observed phenomena
+        conversion_success = {}
 
-    # for idx in range(num_rvr):
-    #     rvr_mappings = [
-    #         {"eccodes_key": f"#{idx+1}#runwayDesignator", "value": f"data:rvr_{idx+1}_designator"},
-    #         {"eccodes_key": f"#{idx+1}#qualifierForRunwayVisualRange", "value": f"data:rvr_{idx+1}_qualifier"},
-    #         {"eccodes_key": f"#{idx+1}#runwayVisualRangeRvr", "value": f"data:rvr_{idx+1}_mean"},
-    #         {"eccodes_key": f"#{idx+1}#tendencyOfRunwayVisualRange", "value": f"data:rvr_{idx+1}_tend"}
-    #     ]
-    #     # print(rvr_mappings)
-    #     for i in range(4):
-    #         print(f"Updating mapping with {rvr_mappings[i]}")
-    #         mapping.update(rvr_mappings[i])
-    #     # mapping.update(rvr_mappings[i] for i in range(4))
-
-    # for item in mapping:
-    #     print(item)
-    # for idx in range(num_sky):
-    #     if 'vertical_visibility' in msg:    
-    #         sky_cover_mappings = [
-    #             {"eccodes_key": "#1#verticalVisibility", "value": "data:vertical_visibility"}
-    #         ]
-    #     else:
-    #         sky_cover_mappings = [
-    #             {"eccodes_key": f"#{idx+1}#cloudAmount", "value": f"data:cloud_amount_{idx+1}"},
-    #             {"eccodes_key": f"#{idx+1}#heightOfBaseOfCloud", "value": f"data:cloud_height_{idx+1}"}
-    #         ]
-    #     print(sky_cover_mappings)
-    #     # mapping.update(sky_cover_mappings[i] for i in range(len(sky_cover_mappings)))
-    #     mapping.update(sky_cover_mappings[1])
+        try:
+            msg, num_rvr, num_vrbrvr, num_pcp, num_obv, num_sky = parse_metar(metar, year, month)
+            tsi = msg['tsi']
+        except Exception as e:
+            LOGGER.error(f"Error parsing METAR report: {data}. {str(e)}")
 
+        try:
+            wsi = tsi_mapping[tsi]
+        except Exception:
+            conversion_success[tsi] = False
+            LOGGER.warning(f"Station {tsi} not found in station file")
 
+        # parse WSI to get sections
+        try:
+            wsi_series, wsi_issuer, wsi_issue_number, wsi_local = wsi.split("-")   # noqa
+            # get other required metadata
+            latitude = metadata_dict[wsi]["latitude"]
+            longitude = metadata_dict[wsi]["longitude"]
+            station_height = metadata_dict[wsi]["elevation"]
+            # add these values to the data dictionary
+            msg['_wsi_series'] = wsi_series
+            msg['_wsi_issuer'] = wsi_issuer
+            msg['_wsi_issue_number'] = wsi_issue_number
+            msg['_wsi_local'] = wsi_local
+            msg['_latitude'] = latitude
+            msg['_longitude'] = longitude
+            msg['_station_height'] = station_height
+            conversion_success[tsi] = True
+        except Exception:
+            conversion_success[tsi] = False
+            if wsi == "":
+                LOGGER.warning(f"Missing WSI for station {tsi}")
+            else:
+                LOGGER.warning((f"Invalid WSI ({wsi}) found in station file,"
+                                " unable to parse"))
+
+        # TODO: update mappings based on number of precipitation observations and observed phenomena
+
+        # for idx in range(num_rvr):
+        #     rvr_mappings = [
+        #         {"eccodes_key": f"#{idx+1}#runwayDesignator", "value": f"data:rvr_{idx+1}_designator"},
+        #         {"eccodes_key": f"#{idx+1}#qualifierForRunwayVisualRange", "value": f"data:rvr_{idx+1}_qualifier"},
+        #         {"eccodes_key": f"#{idx+1}#runwayVisualRangeRvr", "value": f"data:rvr_{idx+1}_mean"},
+        #         {"eccodes_key": f"#{idx+1}#tendencyOfRunwayVisualRange", "value": f"data:rvr_{idx+1}_tend"}
+        #     ]
+        #     # print(rvr_mappings)
+        #     for i in range(4):
+        #         print(f"Updating mapping with {rvr_mappings[i]}")
+        #         mapping.update(rvr_mappings[i])
+        #     # mapping.update(rvr_mappings[i] for i in range(4))
+
+        # for item in mapping:
+        #     print(item)
+        # for idx in range(num_sky):
+        #     if 'vertical_visibility' in msg:    
+        #         sky_cover_mappings = [
+        #             {"eccodes_key": "#1#verticalVisibility", "value": "data:vertical_visibility"}
+        #         ]
+        #     else:
+        #         sky_cover_mappings = [
+        #             {"eccodes_key": f"#{idx+1}#cloudAmount", "value": f"data:cloud_amount_{idx+1}"},
+        #             {"eccodes_key": f"#{idx+1}#heightOfBaseOfCloud", "value": f"data:cloud_height_{idx+1}"}
+        #         ]
+        #     print(sky_cover_mappings)
+        #     # mapping.update(sky_cover_mappings[i] for i in range(len(sky_cover_mappings)))
+        #     mapping.update(sky_cover_mappings[1])
 
-    # for item in mapping['data']:
-    #     print(item)
-
-    # unexpanded_descriptors = [301150, 307080]
-    # unexpanded_descriptors = [307011, 307012]
-    unexpanded_descriptors = [301150, 307021]
-    short_delayed_replications = []
-    delayed_replications = []
-    extended_delayed_replications = []
-    table_version = 37
 
-    try:
-        # import pdb; pdb.set_trace()
 
-        # create new BUFR msg
-        message = BUFRMessage(
-            unexpanded_descriptors,
-            short_delayed_replications,
-            delayed_replications,
-            extended_delayed_replications,
-            table_version)
-    except Exception as e:
-        LOGGER.error(e)
-        LOGGER.error("Error creating BUFRMessage")
-        conversion_success[tsi] = False
+        # for item in mapping['data']:
+        #     print(item)
+
+        # unexpanded_descriptors = [301150, 307080]
+        # unexpanded_descriptors = [307011, 307012]
+        unexpanded_descriptors = [301150, 307021]
+        short_delayed_replications = []
+        delayed_replications = []
+        extended_delayed_replications = []
+        table_version = 37
 
-    # parse
-    if conversion_success[tsi]:
-        # try:
-        #     import pdb; pdb.set_trace()
-        #     message.parse(msg, mapping)
-        # except Exception as e:
-        #     # import pdb; pdb.set_trace()
-        #     LOGGER.error(e)
-        #     LOGGER.error("Error parsing message")
-        #     conversion_success[tsi] = False
-        message.parse(msg, mapping)
-    # Only convert to BUFR if there's no errors so far
-    if conversion_success[tsi]:
         try:
-            result["bufr4"] = message.as_bufr()  # encode to BUFR
-            status = {"code": PASSED}
+            # import pdb; pdb.set_trace()
+
+            # create new BUFR msg
+            message = BUFRMessage(
+                unexpanded_descriptors,
+                short_delayed_replications,
+                delayed_replications,
+                extended_delayed_replications,
+                table_version)
         except Exception as e:
-            LOGGER.error("Error encoding BUFR, null returned")
             LOGGER.error(e)
-            result["bufr4"] = None
-            status = {
-                "code": FAILED,
-                "message": f"Error encoding, BUFR set to None:\n\t\tError: {e}\n\t\tMessage: {msg}"  # noqa
-            }
+            LOGGER.error("Error creating BUFRMessage")
             conversion_success[tsi] = False
 
-        # now identifier based on WSI and observation date as identifier
-        isodate = message.get_datetime().strftime('%Y%m%dT%H%M%S')
-        rmk = f"WIGOS_{wsi}_{isodate}"
-
-        # now additional metadata elements
-        result["_meta"] = {
-            "id": rmk,
-            "geometry": {
-                "type": "Point",
-                "coordinates": [
-                    message.get_element('#1#longitude'),
-                    message.get_element('#1#latitude')
-                ]
-            },
-            "properties": {
-                "md5": message.md5(),
-                "wigos_station_identifier": wsi,
-                "datetime": message.get_datetime(),
-                "originating_centre":
-                message.get_element("bufrHeaderCentre"),
-                "data_category": message.get_element("dataCategory")
-            },
-            "result": status
-        }
-
-    # now yield result back to caller
-    yield result
-
-    # Output conversion status to user
-    if conversion_success[tsi]:
-        LOGGER.info(f"Station {tsi} report converted")
-    else:
-        LOGGER.info(f"Station {tsi} report failed to convert")
+        # parse
+        if conversion_success[tsi]:
+            try:
+                message.parse(msg, mapping)
+            except Exception as e:
+                LOGGER.error(e)
+                LOGGER.error("Error parsing message")
+                conversion_success[tsi] = False
+            message.parse(msg, mapping)
+        # Only convert to BUFR if there's no errors so far
+        if conversion_success[tsi]:
+            try:
+                result["bufr4"] = message.as_bufr()  # encode to BUFR
+                status = {"code": PASSED}
+            except Exception as e:
+                LOGGER.error("Error encoding BUFR, null returned")
+                LOGGER.error(e)
+                result["bufr4"] = None
+                status = {
+                    "code": FAILED,
+                    "message": f"Error encoding, BUFR set to None:\n\t\tError: {e}\n\t\tMessage: {msg}"  # noqa
+                }
+                conversion_success[tsi] = False
+
+            # now identifier based on WSI and observation date as identifier
+            isodate = message.get_datetime().strftime('%Y%m%dT%H%M%S')
+            rmk = f"WIGOS_{wsi}_{isodate}"
+
+            # now additional metadata elements
+            result["_meta"] = {
+                "id": rmk,
+                "geometry": {
+                    "type": "Point",
+                    "coordinates": [
+                        message.get_element('#1#longitude'),
+                        message.get_element('#1#latitude')
+                    ]
+                },
+                "properties": {
+                    "md5": message.md5(),
+                    "wigos_station_identifier": wsi,
+                    "datetime": message.get_datetime(),
+                    "originating_centre":
+                    message.get_element("bufrHeaderCentre"),
+                    "data_category": message.get_element("dataCategory")
+                },
+                "result": status
+            }
 
-    
-# with open("/home/alexander.thompson/metar2bufr/station_list.csv") as fh:
+        # now yield result back to caller
+        yield result
+
+        # Output conversion status to user
+        if conversion_success[tsi]:
+            LOGGER.info(f"Station {tsi} report converted")
+        else:
+            LOGGER.info(f"Station {tsi} report failed to convert")
+
+    # calculate number of successful conversions
+    conversion_count = sum(tsi for tsi in conversion_success.values())
+    # print number of messages converted
+    LOGGER.info((f"{conversion_count} / {len(messages)}"
+            " reports converted successfully"))
+
+
+# metar = "SAAG SABM 012200\
+# SPECI DNPO 180700Z 00000KT 5000 BR BKN008\
+#     24/24 Q1015 BECMG 7000=\
+# SPECI DNPO 180700Z 00000KT 5000 BR BKN008 24/24\
+#         Q1015 BECMG 7000=\
+# SPECI DNPO 180700Z\
+#             00000KT 5000 BR BKN008 24/24 Q1015 BECMG 7000="
+
+# with open("/home/alexander.thompson/metar2bufr/src/resources/station_list.csv") as fh:
 #     station_metadata = fh.read()
 
 # result = transform(metar, station_metadata, 2023, 7)
 
 # for item in result:
 #     print(item)
 #     bufr4 = item['bufr4']
```

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/resources/metar-mappings.json` & `metar2bufr-0.0.2.22/src/metar2bufr/resources/metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr/resources/metar-mappings2.json` & `metar2bufr-0.0.2.22/src/metar2bufr/resources/metar-mappings2.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr.egg-info/PKG-INFO` & `metar2bufr-0.0.2.22/src/metar2bufr.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.21
+Version: 0.0.2.22
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.21/src/metar2bufr.egg-info/SOURCES.txt` & `metar2bufr-0.0.2.22/src/metar2bufr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

