# Comparing `tmp/horus-media-client-0.9.5.tar.gz` & `tmp/horus-media-client-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horus-media-client-0.9.5.tar", last modified: Tue May 16 08:01:28 2023, max compression
+gzip compressed data, was "horus-media-client-0.9.6.tar", last modified: Tue Jul 18 04:38:20 2023, max compression
```

## Comparing `horus-media-client-0.9.5.tar` & `horus-media-client-0.9.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_camera/
--rw-r--r--   0 runner    (1001) docker     (123)    21170 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_camera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_db/
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_geometries/
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_geometries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_geopandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_gis/
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_gis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_media/
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_media_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/horus_media_examples/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/clustering_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/example_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/export_orthographic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/export_spherical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/export_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/geosuite_database_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/recordings_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/single_measurement_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/spherical_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/spherical_camera_single_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/spherical_camera_single_measurement_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/spherical_camera_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/triangulate_spherical_camera_single_measurement_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/horus_spatialite/
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_spatialite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/tests/test_geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/tests/test_gis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/tests/test_media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.669551 horus-media-client-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-18 04:38:20.669551 horus-media-client-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.657551 horus-media-client-0.9.6/horus_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.661551 horus-media-client-0.9.6/horus_camera/
+-rw-r--r--   0 runner    (1001) docker     (123)    21170 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_camera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.661551 horus-media-client-0.9.6/horus_db/
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.661551 horus-media-client-0.9.6/horus_geometries/
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_geometries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.661551 horus-media-client-0.9.6/horus_geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_geopandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.661551 horus-media-client-0.9.6/horus_gis/
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_gis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.661551 horus-media-client-0.9.6/horus_media/
+-rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.661551 horus-media-client-0.9.6/horus_media_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-18 04:38:20.000000 horus-media-client-0.9.6/horus_media_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-18 04:38:20.000000 horus-media-client-0.9.6/horus_media_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:38:20.000000 horus-media-client-0.9.6/horus_media_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 04:38:20.000000 horus-media-client-0.9.6/horus_media_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-18 04:38:20.000000 horus-media-client-0.9.6/horus_media_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.669551 horus-media-client-0.9.6/horus_media_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/clustering_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/example_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/export_orthographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/export_spherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/export_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/geosuite_database_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/recordings_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/single_measurement_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/spherical_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/spherical_camera_single_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/spherical_camera_single_measurement_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/spherical_camera_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/triangulate_spherical_camera_single_measurement_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_media_examples/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.669551 horus-media-client-0.9.6/horus_spatialite/
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/horus_spatialite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:38:20.669551 horus-media-client-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:38:20.669551 horus-media-client-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/tests/test_geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/tests/test_gis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-18 04:38:09.000000 horus-media-client-0.9.6/tests/test_media.py
```

### Comparing `horus-media-client-0.9.5/LICENSE.txt` & `horus-media-client-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/PKG-INFO` & `horus-media-client-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horus-media-client
-Version: 0.9.5
+Version: 0.9.6
 Summary: Horus Media Server Client
 Home-page: https://github.com/horus-view-and-explore/horus-media-client
 Author: Horus View and Explore B.V.
 Author-email: info@horus.nu
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
```

### Comparing `horus-media-client-0.9.5/README.md` & `horus-media-client-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_analytics/__init__.py` & `horus-media-client-0.9.6/horus_analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_camera/__init__.py` & `horus-media-client-0.9.6/horus_camera/__init__.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_db/__init__.py` & `horus-media-client-0.9.6/horus_db/__init__.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_geometries/__init__.py` & `horus-media-client-0.9.6/horus_geometries/__init__.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_geopandas/__init__.py` & `horus-media-client-0.9.6/horus_geopandas/__init__.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_gis/__init__.py` & `horus-media-client-0.9.6/horus_gis/__init__.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media/__init__.py` & `horus-media-client-0.9.6/horus_media/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Horus Media"""
-# Copyright(C) 2019, 2020 Horus View and Explore B.V.
+# Copyright(C) 2019, 2020, 2023 Horus View and Explore B.V.
 
 
 from dataclasses import dataclass
 from PIL import Image
 from itertools import chain
 from enum import Enum
 
@@ -220,35 +220,52 @@
     altitude: float
 
 
 class Client:
     def __init__(self, url="http://localhost:5050/web/", timeout=4):
         self.url = url
         self.__parsed_url = urllib.parse.urlparse(url)
+        self.__timeout = timeout
         self.__connection = http.client.HTTPConnection(
-            self.__parsed_url.hostname, self.__parsed_url.port, timeout=timeout
+            self.__parsed_url.hostname, self.__parsed_url.port, timeout=self.__timeout
         )
-        self.__connection.connect()
         self.attempts = 5
         self.attempts_interval = 3  # seconds
 
     def fetch(self, request):
         request.url = urllib.parse.urljoin(self.__parsed_url.path, request.resource)
-        self.__connection.request("GET", request.url)
+        response = None
         attempts = self.attempts
-        while attempts > 0:
+        while response is None and attempts > 0:
             attempts -= 1
             try:
+                self.__connection.request("GET", request.url)
                 response = self.__connection.getresponse()
-                attempts = 0
+            except (
+                ConnectionError,
+                http.client.ImproperConnectionState,
+            ) as connection_error:
+                logging.error(f'{connection_error}. Requesting "{request.url}".')
+                logging.error(f"New connection attempt in {self.attempts_interval}s.")
+                time.sleep(self.attempts_interval)
+                self.__connection = http.client.HTTPConnection(
+                    self.__parsed_url.hostname,
+                    self.__parsed_url.port,
+                    timeout=self.__timeout,
+                )
+                logging.error(f"New request attempt in {self.attempts_interval}s.")
+                time.sleep(self.attempts_interval)
             except Exception as exception:
                 logging.error(f'{exception}. Requesting "{request.url}".')
-                logging.error(f"New attempt in {self.attempts_interval}s .")
+                logging.error(f"New attempt in {self.attempts_interval}s.")
                 time.sleep(self.attempts_interval)
-
+        if response is None:
+            raise Exception(
+                f'No response after {self.attempts} attempts while requesting "{request.url}".'
+            )
         request.response = response
         result = response.read()
         if type(request.local_file) == str:
             with open(request.local_file, "wb") as file:
                 file.write(result)
         request.set_result(result)
         return request
```

### Comparing `horus-media-client-0.9.5/horus_media_client.egg-info/PKG-INFO` & `horus-media-client-0.9.6/horus_media_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horus-media-client
-Version: 0.9.5
+Version: 0.9.6
 Summary: Horus Media Server Client
 Home-page: https://github.com/horus-view-and-explore/horus-media-client
 Author: Horus View and Explore B.V.
 Author-email: info@horus.nu
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
```

### Comparing `horus-media-client-0.9.5/horus_media_client.egg-info/SOURCES.txt` & `horus-media-client-0.9.6/horus_media_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/clustering_analytics.py` & `horus-media-client-0.9.6/horus_media_examples/clustering_analytics.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/example_strategy.py` & `horus-media-client-0.9.6/horus_media_examples/example_strategy.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/export_orthographic.py` & `horus-media-client-0.9.6/horus_media_examples/export_orthographic.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/export_spherical.py` & `horus-media-client-0.9.6/horus_media_examples/export_spherical.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/export_time_interval.py` & `horus-media-client-0.9.6/horus_media_examples/export_time_interval.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/geosuite_database_info.py` & `horus-media-client-0.9.6/horus_media_examples/geosuite_database_info.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/recordings_tool.py` & `horus-media-client-0.9.6/horus_media_examples/recordings_tool.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/single_measurement_clustering.py` & `horus-media-client-0.9.6/horus_media_examples/single_measurement_clustering.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/snapshots.py` & `horus-media-client-0.9.6/horus_media_examples/snapshots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,57 @@
 from horus_camera import SphericalCamera
 from horus_gis import GeographicLocation
-from horus_db import Recordings, Frames, Frame
+from horus_db import Frames, Frame
 from horus_spatialite import Spatialite, FrameMatchedIterator
 from pyproj import Geod
 from horus_geometries import Geometry_proj
 import geopandas as gpd
 import pandas as pd
 import sys
 from os import path
 import traceback
 import math
 
 from . import util
 
-parser = util.create_argument_parser()
 
+parser = util.create_argument_parser()
 parser.add_argument("--sqlite-db", type=str, help="the geosuite_database name")
-
 parser.add_argument(
     "--sqlite-framenr", type=str, help="the field specifying the framenr"
 )
-
 parser.add_argument(
     "--sqlite-recording", type=str, help="the field specifying the recordingname"
 )
-
 parser.add_argument(
     "--sqlite-geometry",
     type=str,
     help="the field specifying an alternative geometry blob",
 )
-
 # Not tested
 parser.add_argument(
     "--recordings-on-disk", type=str, help="Optionally provide a recording folder"
 )
-
 # Not tested
 parser.add_argument(
     "--recording-id", type=int, help="Optionally provide a the static recording id."
 )
-
-
 util.add_database_arguments(parser)
 util.add_server_arguments(parser)
 
-
 args = parser.parse_args()
-client = util.get_client(args)
-connection = util.get_connection(args)
-recordings = Recordings(connection)
-
 if args.sqlite_db is None:
     print("A sqlite database should be provided")
     exit()
 
+connection = util.get_connection(args)
+
+sp_camera = SphericalCamera()
+sp_camera.set_network_client(util.get_client(args))
+
 # sqlite_frame_idx_field = "Frame_numb"
 output_database = None
 geod = Geod(ellps="WGS84")
 
 
 def compute_heading(long_0, lat_0, long_1, lat_1):
     long_0 = math.radians(long_0)
@@ -125,28 +118,31 @@
         self.geometry = geometry
         self.gp = Geometry_proj()
 
     def to_geographic_loc_list(self):
         return self.gp.to_geographic(self.geometry)
 
 
-def add_to_output(frame, geometry, filename, nr, matched_frame):
+def add_to_output(db, frame, geometry, filename, error, sub_id, matched_frame):
     """
     Add the current geometry and attributes to the output database
     """
     global output_database
 
     record = {}
     record["geometry"] = gpd.GeoSeries(geometry)
     record["snapshot"] = filename
-    record["sub_id"] = nr
-    record["frame_index"] = frame.index
-    record["recording_id"] = frame.recordingid
-    record["distance"] = geod.line_length(
-        *zip(*[frame.get_location()[:2], geometry.centroid.coords[0]])
+    record["snapshot_error"] = error
+    record["sub_id"] = sub_id
+    record["frame_index"] = frame.index if frame else None
+    record["recording_id"] = frame.recordingid if frame else None
+    record["distance"] = (
+        geod.line_length(*zip(*[frame.get_location()[:2], geometry.centroid.coords[0]]))
+        if frame
+        else None
     )
 
     for k, v in matched_frame.metadata.items():
         record[k] = v
 
     gdf = gpd.GeoDataFrame(record)
 
@@ -156,44 +152,47 @@
         output_database = pd.concat([output_database, gdf])
 
 
 def try_find_frame(geometry, mf: FrameMatchedIterator.MatchedFrame):
     """
     Try to find a frame from the same recording that is within (DISTANCE_MIN, DISTANCE_MAX)
     """
-    frames = Frames(connection)
-    cursor = frames.query(
-        within=(*geometry.centroid.coords, DISTANCE_MAX),
-        recordingid=mf.recording.id,
-        distance=(*geometry.centroid.coords, "> %s", DISTANCE_MIN),
-        limit=FRAME_LIMIT,
-    )
-    return GEOM_HEADING_FRAME_SELECTOR(geometry, cursor)
+    if mf.recording == None:
+        return None
+    else:
+        frames = Frames(connection)
+        cursor = frames.query(
+            within=(*geometry.centroid.coords, DISTANCE_MAX),
+            recordingid=mf.recording.id,
+            distance=(*geometry.centroid.coords, "> %s", DISTANCE_MIN),
+            limit=FRAME_LIMIT,
+        )
+        return GEOM_HEADING_FRAME_SELECTOR(geometry, cursor)
 
 
 def look_at_point(point, mf: FrameMatchedIterator.MatchedFrame, side):
     """
-    Transforms a 'Point' geometry into a square of sides 'side'x'side'
-    in meters
+    Transform a 'Point' geometry into a square of sides 'side'x'side' in meters.
     """
+    assert point.geom_type == "Point"
     gp = Geometry_proj()
     square = gp.point_to_square(point, side)
     return [Look_at(mf.frame, square)]
 
 
 def look_at_linestring(
     linestring,
     mf: FrameMatchedIterator.MatchedFrame,
     max_length,
     offset,
 ):
     """
-    Transforms a 'LineString' geometry into sub LineStrings of maximum length
-    of 'max_length' in meters.
+    Transform a 'LineString' geometry into sub LineStrings of maximum length of 'max_length' in meters.
     """
+    assert linestring.geom_type == "LineString"
     gp = Geometry_proj()
 
     if geod.geometry_length(linestring) > max_length:
         linestrings = gp.split_linestring(linestring, max_length)
 
         look_at_all_sub_string = []
         for w in linestrings:
@@ -209,127 +208,120 @@
         return look_at_all_sub_string
 
     return [Look_at(mf.frame, gp.buffer(linestring, offset))]
 
 
 def look_at_polygon(polygon, mf: FrameMatchedIterator.MatchedFrame):
     """
-    Transforms a 'Polygon' geometry into a collection of Polygons..
+    Transform a 'Polygon' geometry into a collection of Polygons.
     """
+    assert polygon.geom_type == "Polygon"
     return [Look_at(mf.frame, polygon)]
 
 
-def take_snapshot(db, mf: FrameMatchedIterator.MatchedFrame, geod):
-    geometries = []
-    geo = db.get_geometry(mf.spatialite_cursor)[db.geometry_field_name]
+def take_snapshot(db, mf: FrameMatchedIterator.MatchedFrame):
+    geometry = db.get_geometry(mf.spatialite_cursor)[db.geometry_field_name]
 
-    if geo.geom_type.startswith("Multi"):
-        for g in geo.geoms:
-            geometries.append(g)
+    geometries = []
+    if geometry.geom_type.startswith("Multi"):
+        for geom in geometry.geoms:
+            geometries.append(geom)
     else:
-        geometries.append(geo)
+        geometries.append(geometry)
 
     width = 800
     look_at_all: [Look_at] = []
-
     for geom in geometries:
         if geom.geom_type == "Polygon":
             look_at_all = [*look_at_all, *look_at_polygon(geom, mf)]
         elif geom.geom_type == "LineString":
             look_at_all = [*look_at_all, *look_at_linestring(geom, mf, 5, 0.1)]
         elif geom.geom_type == "Point":
             look_at_all = [*look_at_all, *look_at_point(geom, mf, 0.5)]
         else:
             print("Not supported", geom.geom_type)
 
     nr_snapshots = len(look_at_all)
 
     for x, look_at in enumerate(look_at_all):
         look_at_geometry = look_at.to_geographic_loc_list()
-
-        sp_camera.set_frame(mf.recording, look_at.frame)
-        size = sp_camera.look_at_all(look_at_geometry, width)
-        spherical_image = sp_camera.crop_to_geometry(
-            sp_camera.acquire(size), look_at_geometry
-        )
-
-        # Write output
         db_id = mf.spatialite_cursor[db.field_info_map["rowid"].idx]
         print(
-            "Snapshot:", "db id", db_id, "nr", x + 1, "/", nr_snapshots, geom.geom_type
+            "Snapshot:",
+            "db id",
+            db_id,
+            "nr",
+            x + 1,
+            "/",
+            nr_snapshots,
+            geometry.geom_type,
         )
-
         filename = (
             "output/snapshot_db_id:"
             + str(db_id)
             + "_"
             + str(x + 1)
             + "_"
-            + geom.geom_type
+            + geometry.geom_type
             + ".jpeg"
         )
-
-        add_to_output(look_at.frame, look_at.geometry, filename, x + 1, mf)
-
-        with open(filename, "wb") as image_file:
-            image_file.write(spherical_image.get_image().getvalue())
-            spherical_image.get_image().close()
+        error = ""
+        if mf.recording != None and look_at.frame != None:
+            try:
+                sp_camera.set_frame(mf.recording, look_at.frame)
+                size = sp_camera.look_at_all(look_at_geometry, width)
+                spherical_image = sp_camera.crop_to_geometry(
+                    sp_camera.acquire(size), look_at_geometry
+                )
+                with open(filename, "wb") as image_file:
+                    image_file.write(spherical_image.get_image().getvalue())
+                    spherical_image.get_image().close()
+            except Exception as e:
+                error = str(e)
+                print("Exception:", error)
+                print("Properties:", mf.properties)
+                print("Metadata:", mf.metadata)
+        else:
+            error = f"No frame found within {DISTANCE_MIN}-{DISTANCE_MAX} meters from centroid of geometry."
+            print("Error:", error)
+            print("Spatialite cursor:", mf.spatialite_cursor)
+        add_to_output(db, look_at.frame, look_at.geometry, filename, error, x + 1, mf)
 
 
 db = Spatialite(args.sqlite_db)
-
-
 if not args.recordings_on_disk is None:
     db.set_recordings_on_disk_root_folder(args.recordings_on_disk)
-
 if not args.sqlite_recording is None:
     db.set_recording_field(args.sqlite_recording)
-
 if not args.sqlite_framenr is None:
     db.set_frame_index_field(args.sqlite_framenr)
-
 if not args.sqlite_geometry is None:
     db.set_geometry_field_name(args.sqlite_geometry)
     db.blob_contains_geometry(args.sqlite_geometry)
-
 db.set_remote_db_connection(connection)
-
 db.open()
 db.resolve()
 db.show_info()
 
-sp_camera = SphericalCamera()
-sp_camera.set_network_client(client)
-
 fmi: FrameMatchedIterator = db.get_matched_frames_iterator()
 fmi.set_distance_limits(DISTANCE_MIN, DISTANCE_MAX)
 fmi.set_frame_limit(FRAME_LIMIT)
 fmi.set_frame_selector(GEOM_HEADING_FRAME_SELECTOR)
-
 if not args.recording_id is None:
     fmi.set_static_recording_by_id(args.recording_id)
 
-
 mf: FrameMatchedIterator.MatchedFrame = next(fmi, None)
 
 while mf != None:
+    assert mf.spatialite_cursor != None
     try:
-        if mf.oke():
-            take_snapshot(db, mf, geod)
-        else:
-            print("\nIncomplete match")
-            print(mf.dump())
+        take_snapshot(db, mf)
     except Exception as e:
-        if str(e) == "Request-sent":
-            # reset network connection
-            client = util.get_client(args)
-            sp_camera.set_network_client(client)
         print("Exception:", e)
         print("Properties:", mf.properties)
         print("Metadata:", mf.metadata)
-        pass
     mf = next(fmi, None)
 
 db.close()
 
 if not output_database is None:
     output_database.to_file("output/snapshots.geojson", driver="GeoJSON")
```

### Comparing `horus-media-client-0.9.5/horus_media_examples/spherical_camera.py` & `horus-media-client-0.9.6/horus_media_examples/spherical_camera.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/spherical_camera_single_measurement.py` & `horus-media-client-0.9.6/horus_media_examples/spherical_camera_single_measurement.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/spherical_camera_single_measurement_reconstruction.py` & `horus-media-client-0.9.6/horus_media_examples/spherical_camera_single_measurement_reconstruction.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/spherical_camera_snapshot.py` & `horus-media-client-0.9.6/horus_media_examples/spherical_camera_snapshot.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/test_tool.py` & `horus-media-client-0.9.6/horus_media_examples/test_tool.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/triangulate_spherical_camera_single_measurement_clusters.py` & `horus-media-client-0.9.6/horus_media_examples/triangulate_spherical_camera_single_measurement_clusters.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_media_examples/util.py` & `horus-media-client-0.9.6/horus_media_examples/util.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/horus_spatialite/__init__.py` & `horus-media-client-0.9.6/horus_spatialite/__init__.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/setup.py` & `horus-media-client-0.9.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     long_description = f.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="horus-media-client",
-    version="0.9.5",
+    version="0.9.6",
     description="Horus Media Server Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/horus-view-and-explore/horus-media-client",
     author_email="info@horus.nu",
     author="Horus View and Explore B.V.",
     license="MIT",
```

### Comparing `horus-media-client-0.9.5/tests/test_db.py` & `horus-media-client-0.9.6/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/tests/test_geopandas.py` & `horus-media-client-0.9.6/tests/test_geopandas.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/tests/test_gis.py` & `horus-media-client-0.9.6/tests/test_gis.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.5/tests/test_media.py` & `horus-media-client-0.9.6/tests/test_media.py`

 * *Files identical despite different names*

