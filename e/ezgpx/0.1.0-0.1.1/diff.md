# Comparing `tmp/ezGPX-0.1.0.tar.gz` & `tmp/ezgpx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezGPX-0.1.0.tar", last modified: Tue Jul 18 09:40:57 2023, max compression
+gzip compressed data, was "ezgpx-0.1.1.tar", last modified: Tue Jul 18 12:29:51 2023, max compression
```

## Comparing `ezGPX-0.1.0.tar` & `ezgpx-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 09:40:57.080281 ezGPX-0.1.0/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    35149 2023-06-06 11:52:29.000000 ezGPX-0.1.0/LICENSE
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2111 2023-07-18 09:40:57.080281 ezGPX-0.1.0/PKG-INFO
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1243 2023-07-16 16:02:43.000000 ezGPX-0.1.0/README.md
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 09:40:57.080281 ezGPX-0.1.0/ezGPX.egg-info/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2111 2023-07-18 09:40:56.000000 ezGPX-0.1.0/ezGPX.egg-info/PKG-INFO
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      226 2023-07-18 09:40:57.000000 ezGPX-0.1.0/ezGPX.egg-info/SOURCES.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        1 2023-07-18 09:40:56.000000 ezGPX-0.1.0/ezGPX.egg-info/dependency_links.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       12 2023-07-18 09:40:56.000000 ezGPX-0.1.0/ezGPX.egg-info/requires.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        6 2023-07-18 09:40:56.000000 ezGPX-0.1.0/ezGPX.egg-info/top_level.txt
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 09:40:57.080281 ezGPX-0.1.0/ezgpx/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       98 2023-06-08 09:27:44.000000 ezGPX-0.1.0/ezgpx/__init__.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       38 2023-07-18 09:40:57.080281 ezGPX-0.1.0/setup.cfg
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1642 2023-07-18 09:40:43.000000 ezGPX-0.1.0/setup.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 09:40:57.080281 ezGPX-0.1.0/tests/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2608 2023-06-28 12:23:09.000000 ezGPX-0.1.0/tests/test_GPX.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1689 2023-06-28 12:54:28.000000 ezGPX-0.1.0/tests/test_utils.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 12:29:51.776976 ezgpx-0.1.1/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    35149 2023-06-06 11:52:29.000000 ezgpx-0.1.1/LICENSE
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2111 2023-07-18 12:29:51.776976 ezgpx-0.1.1/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1243 2023-07-16 16:02:43.000000 ezgpx-0.1.1/README.md
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 12:29:51.776976 ezgpx-0.1.1/ezgpx/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       98 2023-06-08 09:27:44.000000 ezgpx-0.1.1/ezgpx/__init__.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 12:29:51.776976 ezgpx-0.1.1/ezgpx.egg-info/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2111 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      226 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        1 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       12 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/requires.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        6 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/top_level.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       38 2023-07-18 12:29:51.776976 ezgpx-0.1.1/setup.cfg
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1642 2023-07-18 09:45:47.000000 ezgpx-0.1.1/setup.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 12:29:51.776976 ezgpx-0.1.1/tests/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     3193 2023-07-18 12:25:14.000000 ezgpx-0.1.1/tests/test_GPX.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1747 2023-07-18 12:27:24.000000 ezgpx-0.1.1/tests/test_utils.py
```

### Comparing `ezGPX-0.1.0/LICENSE` & `ezgpx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezGPX-0.1.0/PKG-INFO` & `ezgpx-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ezGPX
-Version: 0.1.0
+Name: ezgpx
+Version: 0.1.1
 Summary: Easy to use Python GPX library
 Download-URL: https://github.com/FABallemand/ezGPX
 Author: Fabien ALLEMAND
 Author-email: allemand.fabien@orange.fr
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/FABallemand/ezGPX/issues
 Project-URL: Source Code, https://github.com/FABallemand/ezGPX
```

### Comparing `ezGPX-0.1.0/README.md` & `ezgpx-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ezGPX-0.1.0/ezGPX.egg-info/PKG-INFO` & `ezgpx-0.1.1/ezgpx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ezGPX
-Version: 0.1.0
+Name: ezgpx
+Version: 0.1.1
 Summary: Easy to use Python GPX library
 Download-URL: https://github.com/FABallemand/ezGPX
 Author: Fabien ALLEMAND
 Author-email: allemand.fabien@orange.fr
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/FABallemand/ezGPX/issues
 Project-URL: Source Code, https://github.com/FABallemand/ezGPX
```

### Comparing `ezGPX-0.1.0/setup.py` & `ezgpx-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the README file
 with open(os.path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    name='ezGPX',
-    version='0.1.0',
+    name='ezgpx',
+    version='0.1.1',
     description='Easy to use Python GPX library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['gpx', 'gpx-files', 'gpx-parser', 'gpx-reader', 'gpx-writer', 'gpx-data'],
     # url='https://medium-multiply.readthedocs.io/',
     download_url='https://github.com/FABallemand/ezGPX',
     project_urls={
```

### Comparing `ezGPX-0.1.0/tests/test_utils.py` & `ezgpx-0.1.1/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,43 +9,43 @@
 
 file_folder = os.path.dirname(__file__)
 parent_folder = os.path.realpath(os.path.dirname(file_folder)) # ie: ezGPX
 
 os.chdir(file_folder)
 sys.path.append(parent_folder + "/ezgpx")
 
-from ezgpx import utils, TrackPoint
+from ezgpx import utils, WayPoint
 
 class TestUtils():
 
     def test_haversine_distance(self):
         pass
 
     def _test_perpendicular_distance_horizontal_line(self):
-        start = TrackPoint(0, 0)
-        end = TrackPoint(0, 2)
-        point = TrackPoint(1, 1)
+        start = WayPoint("wpt", 0, 0)
+        end = WayPoint("wpt", 0, 2)
+        point = WayPoint("wpt", 1, 1)
         return math.isclose(utils.perpendicular_distance(start, end, point), 1)
 
     def _test_perpendicular_distance_vertical_line(self):
-        start = TrackPoint(0, 0)
-        end = TrackPoint(2, 0)
-        point = TrackPoint(1, 1)
+        start = WayPoint("wpt", 0, 0)
+        end = WayPoint("wpt", 2, 0)
+        point = WayPoint("wpt", 1, 1)
         return math.isclose(utils.perpendicular_distance(start, end, point), 1)
     
     def _test_perpendicular_distance_random_line(self):
-        start = TrackPoint(0, 0)
-        end = TrackPoint(1, 1)
-        point = TrackPoint(1, 0)
+        start = WayPoint("wpt", 0, 0)
+        end = WayPoint("wpt", 1, 1)
+        point = WayPoint("wpt", 1, 0)
         return math.isclose(utils.perpendicular_distance(start, end, point), math.sqrt(2)/2)
     
     def _test_perpendicular_distance_point_on_line(self):
-        start = TrackPoint(0, 0)
-        end = TrackPoint(1, 1)
-        point = TrackPoint(2, 2)
+        start = WayPoint("wpt", 0, 0)
+        end = WayPoint("wpt", 1, 1)
+        point = WayPoint("wpt", 2, 2)
         return math.isclose(utils.perpendicular_distance(start, end, point), 0)
     
     def test_perpendicular_distance(self):
         assert self._test_perpendicular_distance_horizontal_line()
         assert self._test_perpendicular_distance_vertical_line()
         assert self._test_perpendicular_distance_random_line()
         assert self._test_perpendicular_distance_point_on_line()
```

