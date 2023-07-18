# Comparing `tmp/openghg_defs-0.0.1.tar.gz` & `tmp/openghg_defs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openghg_defs-0.0.1.tar", last modified: Tue Mar 14 16:04:18 2023, max compression
+gzip compressed data, was "openghg_defs-0.0.2.tar", last modified: Tue Jul 18 15:18:58 2023, max compression
```

## Comparing `openghg_defs-0.0.1.tar` & `openghg_defs-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-03-14 16:04:18.376131 openghg_defs-0.0.1/
--rw-r--r--   0 gar        (501) staff       (20)     1064 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/LICENSE
--rw-r--r--   0 gar        (501) staff       (20)      668 2023-03-14 16:04:18.375966 openghg_defs-0.0.1/PKG-INFO
--rw-r--r--   0 gar        (501) staff       (20)      327 2023-03-14 16:04:14.000000 openghg_defs-0.0.1/README.md
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-03-14 16:04:18.363936 openghg_defs-0.0.1/openghg_defs/
--rw-r--r--   0 gar        (501) staff       (20)      334 2023-03-14 16:00:22.000000 openghg_defs-0.0.1/openghg_defs/__init__.py
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-03-14 16:04:18.365107 openghg_defs-0.0.1/openghg_defs/data/
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-03-14 16:04:18.375698 openghg_defs-0.0.1/openghg_defs/data/domain/
--rw-r--r--   0 gar        (501) staff       (20)     5750 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/ARCTIC_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)    25879 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/ARCTIC_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     8523 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/EASTASIA_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     9775 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/EASTASIA_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     7325 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/EUROPE_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)    10054 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/EUROPE_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     7714 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/PACIFIC_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)    10300 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/PACIFIC_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     7599 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/SOUTHAFRICA_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     9918 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/SOUTHAFRICA_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     5475 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/USA_latitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     7436 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain/USA_longitude.dat
--rw-r--r--   0 gar        (501) staff       (20)     2297 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/domain_info.json
--rw-r--r--   0 gar        (501) staff       (20)    80395 2023-03-08 15:12:25.000000 openghg_defs-0.0.1/openghg_defs/data/site_info.json
--rw-r--r--   0 gar        (501) staff       (20)    18967 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/data/species_info.json
--rw-r--r--   0 gar        (501) staff       (20)        0 2023-01-25 10:16:17.000000 openghg_defs-0.0.1/openghg_defs/py.typed
-drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-03-14 16:04:18.364403 openghg_defs-0.0.1/openghg_defs.egg-info/
--rw-r--r--   0 gar        (501) staff       (20)      668 2023-03-14 16:04:18.000000 openghg_defs-0.0.1/openghg_defs.egg-info/PKG-INFO
--rw-r--r--   0 gar        (501) staff       (20)      883 2023-03-14 16:04:18.000000 openghg_defs-0.0.1/openghg_defs.egg-info/SOURCES.txt
--rw-r--r--   0 gar        (501) staff       (20)        1 2023-03-14 16:04:18.000000 openghg_defs-0.0.1/openghg_defs.egg-info/dependency_links.txt
--rw-r--r--   0 gar        (501) staff       (20)       18 2023-03-14 16:04:18.000000 openghg_defs-0.0.1/openghg_defs.egg-info/top_level.txt
--rw-r--r--   0 gar        (501) staff       (20)      557 2023-03-14 16:00:15.000000 openghg_defs-0.0.1/pyproject.toml
--rw-r--r--   0 gar        (501) staff       (20)       38 2023-03-14 16:04:18.376187 openghg_defs-0.0.1/setup.cfg
+drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.607221 openghg_defs-0.0.2/
+-rw-r--r--   0 gar        (501) staff       (20)     1064 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/LICENSE
+-rw-r--r--   0 gar        (501) staff       (20)     2632 2023-07-18 15:18:58.607082 openghg_defs-0.0.2/PKG-INFO
+-rw-r--r--   0 gar        (501) staff       (20)     2281 2023-07-18 11:11:37.000000 openghg_defs-0.0.2/README.md
+drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.600551 openghg_defs-0.0.2/openghg_defs/
+-rw-r--r--   0 gar        (501) staff       (20)      279 2023-07-18 11:11:37.000000 openghg_defs-0.0.2/openghg_defs/__init__.py
+drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.602426 openghg_defs-0.0.2/openghg_defs/__pycache__/
+-rw-r--r--   0 gar        (501) staff       (20)      571 2023-07-14 11:08:13.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 gar        (501) staff       (20)      791 2023-03-21 14:59:46.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 gar        (501) staff       (20)     1305 2023-03-21 14:54:07.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/_load.cpython-39.pyc
+-rw-r--r--   0 gar        (501) staff       (20)      822 2023-03-21 14:54:07.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/_paths.cpython-39.pyc
+-rw-r--r--   0 gar        (501) staff       (20)    14392 2023-07-14 11:08:13.000000 openghg_defs-0.0.2/openghg_defs/__pycache__/_version.cpython-310.pyc
+drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.603667 openghg_defs-0.0.2/openghg_defs/data/
+drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.606852 openghg_defs-0.0.2/openghg_defs/data/domain/
+-rw-r--r--   0 gar        (501) staff       (20)     5750 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/ARCTIC_latitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)    25879 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/ARCTIC_longitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)     8523 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/EASTASIA_latitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)     9775 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/EASTASIA_longitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)     7325 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/EUROPE_latitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)    10054 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/EUROPE_longitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)     7714 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/PACIFIC_latitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)    10300 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/PACIFIC_longitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)     7599 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/SOUTHAFRICA_latitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)     9918 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/SOUTHAFRICA_longitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)     5475 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/USA_latitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)     7436 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain/USA_longitude.dat
+-rw-r--r--   0 gar        (501) staff       (20)     2297 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/domain_info.json
+-rw-r--r--   0 gar        (501) staff       (20)    82852 2023-07-18 11:11:37.000000 openghg_defs-0.0.2/openghg_defs/data/site_info.json
+-rw-r--r--   0 gar        (501) staff       (20)    18967 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/data/species_info.json
+-rw-r--r--   0 gar        (501) staff       (20)        0 2023-01-25 10:16:17.000000 openghg_defs-0.0.2/openghg_defs/py.typed
+drwxr-xr-x   0 gar        (501) staff       (20)        0 2023-07-18 15:18:58.601037 openghg_defs-0.0.2/openghg_defs.egg-info/
+-rw-r--r--   0 gar        (501) staff       (20)     2632 2023-07-18 15:18:58.000000 openghg_defs-0.0.2/openghg_defs.egg-info/PKG-INFO
+-rw-r--r--   0 gar        (501) staff       (20)     1125 2023-07-18 15:18:58.000000 openghg_defs-0.0.2/openghg_defs.egg-info/SOURCES.txt
+-rw-r--r--   0 gar        (501) staff       (20)        1 2023-07-18 15:18:58.000000 openghg_defs-0.0.2/openghg_defs.egg-info/dependency_links.txt
+-rw-r--r--   0 gar        (501) staff       (20)       32 2023-07-18 15:18:58.000000 openghg_defs-0.0.2/openghg_defs.egg-info/top_level.txt
+-rw-r--r--   0 gar        (501) staff       (20)      578 2023-07-18 11:33:14.000000 openghg_defs-0.0.2/pyproject.toml
+-rw-r--r--   0 gar        (501) staff       (20)       38 2023-07-18 15:18:58.607262 openghg_defs-0.0.2/setup.cfg
```

### Comparing `openghg_defs-0.0.1/LICENSE` & `openghg_defs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/ARCTIC_latitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/ARCTIC_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/ARCTIC_longitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/ARCTIC_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/EASTASIA_latitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/EASTASIA_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/EASTASIA_longitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/EASTASIA_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/EUROPE_latitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/EUROPE_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/EUROPE_longitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/EUROPE_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/PACIFIC_latitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/PACIFIC_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/PACIFIC_longitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/PACIFIC_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/SOUTHAFRICA_latitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/SOUTHAFRICA_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/SOUTHAFRICA_longitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/SOUTHAFRICA_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/USA_latitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/USA_latitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain/USA_longitude.dat` & `openghg_defs-0.0.2/openghg_defs/data/domain/USA_longitude.dat`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/domain_info.json` & `openghg_defs-0.0.2/openghg_defs/data/domain_info.json`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs/data/site_info.json` & `openghg_defs-0.0.2/openghg_defs/data/site_info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9694246922821025%*

 * *Differences: {"'BIR'": "{'ICOS': {'height': {insert: [(1, '75m')]}, 'height_name': {insert: [(1, '75magl')]}, "*

 * *          "'height_station_masl': 219.0, 'latitude': 58.3886, 'longitude': 8.2519}}",*

 * * "'BRM'": "OrderedDict([('ICOS', OrderedDict([('height', ['212m']), ('height_name', ['212magl']), "*

 * *          "('height_station_masl', 797.0), ('latitude', 47.1896), ('long_name', 'Beromunster'), "*

 * *          "('longitude', 8.1755)]))])",*

 * * "'BSD'": "{'DECC': {'height_name': {insert: [(1, '108magl'), (2, '42magl')], delete: [2, […]*

```diff
@@ -351,23 +351,25 @@
             "long_name": "Baring Head, New Zealand",
             "longitude": 174.87
         }
     },
     "BIR": {
         "ICOS": {
             "height": [
-                "10m"
+                "10m",
+                "75m"
             ],
             "height_name": [
-                "10magl"
+                "10magl",
+                "75magl"
             ],
-            "height_station_masl": 190.0,
-            "latitude": 58.39,
+            "height_station_masl": 219.0,
+            "latitude": 58.3886,
             "long_name": "Birkenes Observatory, Norway",
-            "longitude": 8.25
+            "longitude": 8.2519
         }
     },
     "BKT": {
         "NOAA": {
             "height_station_masl": 845.0,
             "latitude": -0.202,
             "long_name": "Bukit Kototabang, Indonesia",
@@ -452,14 +454,28 @@
             ],
             "height_station_masl": 595.0,
             "latitude": 50.2017,
             "long_name": "Bratt's Lake Saskatchewan, Canada",
             "longitude": -104.7113
         }
     },
+    "BRM": {
+        "ICOS": {
+            "height": [
+                "212m"
+            ],
+            "height_name": [
+                "212magl"
+            ],
+            "height_station_masl": 797.0,
+            "latitude": 47.1896,
+            "long_name": "Beromunster",
+            "longitude": 8.1755
+        }
+    },
     "BRW": {
         "NOAA": {
             "height": [
                 "17m",
                 "11m",
                 "5m"
             ],
@@ -513,37 +529,37 @@
             "height": [
                 "248m",
                 "108m",
                 "42m"
             ],
             "height_name": [
                 "248magl",
-                "110magl",
-                "50magl"
+                "108magl",
+                "42magl"
             ],
             "height_station_masl": 382,
-            "latitude": 54.35846,
+            "latitude": 54.35861,
             "long_name": "Bilsdale, UK",
-            "longitude": -1.15018
+            "longitude": -1.15036
         },
         "NOAA": {
             "height": [
                 "108m",
                 "42m",
                 "248m"
             ],
             "height_name": [
-                "110magl",
-                "50magl",
+                "108magl",
+                "42magl",
                 "248magl"
             ],
             "height_station_masl": 382,
-            "latitude": 54.35846,
+            "latitude": 54.35861,
             "long_name": "Bilsdale, UK",
-            "longitude": -1.15018
+            "longitude": -1.15036
         }
     },
     "BTT": {
         "GAUGE": {
             "height": [
                 "185m"
             ],
@@ -636,15 +652,15 @@
                 "20magl",
                 "60magl",
                 "200magl"
             ],
             "height_station_masl": 213.0,
             "latitude": 51.9703,
             "long_name": "Cabauw Tower, Netherlands",
-            "longitude": 4.926
+            "longitude": 4.9264
         }
     },
     "CBY": {
         "EC": {
             "height": [
                 "12m"
             ],
@@ -827,23 +843,23 @@
             "height_station_masl": 2155.0,
             "latitude": 44.193889,
             "long_name": "Monte Cimone, Italy",
             "longitude": 10.701389
         },
         "ICOS": {
             "height": [
-                "10m"
+                "8m"
             ],
             "height_name": [
-                "10magl"
+                "500magl"
             ],
-            "height_station_masl": 2155.0,
-            "latitude": 44.193889,
+            "height_station_masl": 2165.0,
+            "latitude": 44.1936,
             "long_name": "Monte Cimone, Italy",
-            "longitude": 10.701389
+            "longitude": 10.6999
         },
         "NOAA": {
             "height": [
                 "7m"
             ],
             "height_name": [
                 "7magl"
@@ -906,23 +922,14 @@
             ],
             "height_station_masl": 3.0,
             "latitude": -12.417,
             "long_name": "Charles Point, Darwin, Australia",
             "longitude": 130.567
         }
     },
-    "CPI": {
-        "ICOS": {
-            "height_station_masl": 9.0,
-            "icos_sitecode": "CSP",
-            "latitude": 52.17,
-            "long_name": "Carnsore Point, Ireland",
-            "longitude": -6.35
-        }
-    },
     "CPS": {
         "EC": {
             "height": [
                 "8m"
             ],
             "height_name": [
                 "8magl"
@@ -986,14 +993,28 @@
             ],
             "height_station_masl": 60.0,
             "latitude": 15.08,
             "long_name": "Cape Rama, India",
             "longitude": 73.83
         }
     },
+    "CRP": {
+        "ICOS": {
+            "height": [
+                "10m"
+            ],
+            "height_name": [
+                "10magl"
+            ],
+            "height_station_masl": 9.0,
+            "latitude": 52.1775,
+            "long_name": "Carnsore Point, Ireland",
+            "longitude": -6.3677
+        }
+    },
     "CRV": {
         "NOAA": {
             "height": [
                 "10m"
             ],
             "height_name": [
                 "10magl"
@@ -1330,14 +1351,28 @@
             "height_station_masl": 334.3,
             "latitude": 44.66,
             "long_name": "Fairchild, Wisconsin, United States",
             "longitude": -90.96
         }
     },
     "GAT": {
+        "ICOS": {
+            "height": [
+                "132",
+                "341m"
+            ],
+            "height_name": [
+                "132",
+                "341magl"
+            ],
+            "height_station_masl": 70.0,
+            "latitude": 53.0657,
+            "long_name": "Gartow, Germany",
+            "longitude": 11.4429
+        },
         "NOAA": {
             "height": [
                 "132m"
             ],
             "height_name": [
                 "132magl"
             ],
@@ -1674,18 +1709,18 @@
         "ICOS": {
             "height": [
                 "30m"
             ],
             "height_name": [
                 "30magl"
             ],
-            "height_station_masl": 116.0,
-            "latitude": 49.417,
+            "height_station_masl": 113.0,
+            "latitude": 49.4172,
             "long_name": "Heidelberg, Germany",
-            "longitude": 8.674
+            "longitude": 8.675
         }
     },
     "HEL": {
         "ICOS": {
             "height": [
                 "110m"
             ],
@@ -1705,31 +1740,17 @@
                 "50m"
             ],
             "height_name": [
                 "100magl",
                 "50magl"
             ],
             "height_station_masl": 158,
-            "latitude": 50.97661,
-            "long_name": "Heathfield, UK",
-            "longitude": 0.23042
-        },
-        "GAUGE": {
-            "height": [
-                "100m",
-                "50m"
-            ],
-            "height_name": [
-                "100magl",
-                "50magl"
-            ],
-            "height_station_masl": 158,
-            "latitude": 50.97661,
+            "latitude": 50.97675,
             "long_name": "Heathfield, UK",
-            "longitude": 0.23042
+            "longitude": 0.23048
         }
     },
     "HFM": {
         "NOAA": {
             "height": [
                 "29m"
             ],
@@ -1840,17 +1861,17 @@
             "height": [
                 "115m"
             ],
             "height_name": [
                 "115magl"
             ],
             "height_station_masl": 248.0,
-            "latitude": 46.95,
+            "latitude": 46.9558,
             "long_name": "Hegyhatsal, Hungary",
-            "longitude": 16.65
+            "longitude": 16.6522
         },
         "NOAA": {
             "height_station_masl": 248.0,
             "latitude": 46.95,
             "long_name": "Hegyhatsal, Hungary",
             "longitude": 16.65
         }
@@ -2126,23 +2147,23 @@
             "height_station_masl": 3528,
             "latitude": 46.54753,
             "long_name": "Jungfraujoch, Switzerland",
             "longitude": 7.98498
         },
         "ICOS": {
             "height": [
-                "10m"
+                "5m"
             ],
             "height_name": [
-                "10magl"
+                "1000magl"
             ],
-            "height_station_masl": 3528,
-            "latitude": 46.54753,
+            "height_station_masl": 3580,
+            "latitude": 46.5475,
             "long_name": "Jungfraujoch, Switzerland",
-            "longitude": 7.98498
+            "longitude": 7.9851
         },
         "NOAA": {
             "height": [
                 "5m"
             ],
             "height_name": [
                 "5magl"
@@ -2171,14 +2192,28 @@
             ],
             "height_station_masl": 1.0,
             "latitude": 25.6654,
             "long_name": "Key Biscane, Florida",
             "longitude": -80.158
         }
     },
+    "KIT": {
+        "ICOS": {
+            "height": [
+                "200m"
+            ],
+            "height_name": [
+                "200magl"
+            ],
+            "height_station_masl": 110.0,
+            "latitude": 49.0915,
+            "long_name": "Karlsruhe, Germany",
+            "longitude": 8.4249
+        }
+    },
     "KJN": {
         "UEXETER": {
             "height": [
                 "5m"
             ],
             "height_name": [
                 "5magl"
@@ -2425,17 +2460,17 @@
             "height": [
                 "60m"
             ],
             "height_name": [
                 "60magl"
             ],
             "height_station_masl": 1.0,
-            "latitude": 53.404,
+            "latitude": 53.4036,
             "long_name": "Lutjewad, Netherlands",
-            "longitude": 6.353
+            "longitude": 6.3528
         },
         "NOAA": {
             "height": [
                 "60m"
             ],
             "height_name": [
                 "60magl"
@@ -2563,29 +2598,29 @@
             "height": [
                 "10m"
             ],
             "height_name": [
                 "10magl"
             ],
             "height_station_masl": 8.0,
-            "latitude": 53.32663,
+            "latitude": 53.32667,
             "long_name": "Mace Head, Ireland",
             "longitude": -9.90456
         },
         "ICOS": {
             "height": [
                 "10m"
             ],
             "height_name": [
                 "10magl"
             ],
             "height_station_masl": 8.0,
-            "latitude": 53.32663,
+            "latitude": 53.3261,
             "long_name": "Mace Head, Ireland",
-            "longitude": -9.90456
+            "longitude": -9.9036
         },
         "NOAA": {
             "height_station_masl": 8.0,
             "latitude": 53.32663,
             "long_name": "Mace Head, County Galway, Ireland",
             "longitude": -9.90456
         }
@@ -2618,14 +2653,28 @@
         "NOAA": {
             "height_station_masl": 3397.0,
             "latitude": 19.53,
             "long_name": "Mauna Loa, Hawaii, United States",
             "longitude": -155.58
         }
     },
+    "MLH": {
+        "ICOS": {
+            "height": [
+                "10m"
+            ],
+            "height_name": [
+                "10magl"
+            ],
+            "height_station_masl": 22.0,
+            "latitude": 55.3718,
+            "long_name": "Malin Head, Ireland",
+            "longitude": -7.3395
+        }
+    },
     "MLO": {
         "NOAA": {
             "height": [
                 "10m"
             ],
             "height_name": [
                 "10magl"
@@ -2811,14 +2860,26 @@
             "height_station_masl": 42.0,
             "latitude": -70.65,
             "long_name": "Neumayer, Antarctica",
             "longitude": -8.25
         }
     },
     "NOR": {
+        "ICOS": {
+            "height": [
+                "100m"
+            ],
+            "height_name": [
+                "100magl"
+            ],
+            "height_station_masl": 46.0,
+            "latitude": 60.0864,
+            "long_name": "Norunda, Sweden",
+            "longitude": 17.4794
+        },
         "NOAA": {
             "height": [
                 "32m"
             ],
             "height_name": [
                 "32magl"
             ],
@@ -2928,17 +2989,17 @@
             "height": [
                 "120m"
             ],
             "height_name": [
                 "120magl"
             ],
             "height_station_masl": 390.0,
-            "latitude": 48.562,
+            "latitude": 48.5619,
             "long_name": "Observatoire Perenne de l'Environnement, France",
-            "longitude": 5.504
+            "longitude": 5.5036
         },
         "NOAA": {
             "height": [
                 "10m"
             ],
             "height_name": [
                 "10magl"
@@ -2982,39 +3043,51 @@
             "height_station_masl": 40.0,
             "latitude": -38.522,
             "long_name": "Otway, Victoria, Australia",
             "longitude": 142.817
         }
     },
     "OXK": {
+        "ICOS": {
+            "height": [
+                "163m"
+            ],
+            "height_name": [
+                "163magl"
+            ],
+            "height_station_masl": 1022.0,
+            "latitude": 50.03,
+            "long_name": "Ochsenkopf, Germany",
+            "longitude": 11.8083
+        },
         "NOAA": {
             "height": [
                 "10m"
             ],
             "height_name": [
                 "10magl"
             ],
             "height_station_masl": 1022.0,
-            "latitude": 50.0301,
+            "latitude": 50.03,
             "long_name": "Ochsenkopf, Germany",
-            "longitude": 11.8084
+            "longitude": 11.8083
         }
     },
     "PAL": {
         "ICOS": {
             "height": [
-                "5m"
+                "12m"
             ],
             "height_name": [
-                "5magl"
+                "10magl"
             ],
             "height_station_masl": 565.0,
-            "latitude": 67.973,
+            "latitude": 67.9733,
             "long_name": "Pallas, Finland",
-            "longitude": 24.116
+            "longitude": 24.1157
         },
         "NOAA": {
             "height_station_masl": 565.0,
             "latitude": 67.9733,
             "long_name": "Pallas-Sammaltunturi, GAW Station, Finland",
             "longitude": 24.1157
         }
@@ -3240,31 +3313,31 @@
                 "45m"
             ],
             "height_name": [
                 "90magl",
                 "45magl"
             ],
             "height_station_masl": 207,
-            "latitude": 51.99738,
+            "latitude": 51.99747,
             "long_name": "Ridge Hill, UK",
-            "longitude": -2.53977
+            "longitude": -2.53992
         },
         "ICOS": {
             "height": [
                 "90m",
                 "45m"
             ],
             "height_name": [
                 "90magl",
                 "45magl"
             ],
             "height_station_masl": 207,
-            "latitude": 51.99738,
+            "latitude": 51.99747,
             "long_name": "Ridge Hill, UK",
-            "longitude": -2.53977
+            "longitude": -2.53992
         },
         "NOAA": {
             "height": [
                 "90m",
                 "45m"
             ],
             "height_name": [
@@ -3586,14 +3659,28 @@
         "NOAA": {
             "height_station_masl": 42.0,
             "latitude": -14.2474,
             "long_name": "Tutuila, American Samoa",
             "longitude": -170.5644
         }
     },
+    "SMR": {
+        "ICOS": {
+            "height": [
+                "125m"
+            ],
+            "height_name": [
+                "125magl"
+            ],
+            "height_station_masl": 181.0,
+            "latitude": 61.8474,
+            "long_name": "Hyytiala, Finland",
+            "longitude": 24.2947
+        }
+    },
     "SNG": {
         "IITM": {
             "height": [
                 "10m"
             ],
             "height_name": [
                 "10magl"
@@ -3630,23 +3717,25 @@
             "long_name": "South Pole, Antarctica",
             "longitude": -24.8
         }
     },
     "SSL": {
         "ICOS": {
             "height": [
-                "12m"
+                "12m",
+                "35m"
             ],
             "height_name": [
-                "12magl"
+                "12magl",
+                "35magl"
             ],
             "height_station_masl": 1205.0,
-            "latitude": 47.92,
+            "latitude": 47.9167,
             "long_name": "Schauinsland, Germany",
-            "longitude": 7.92
+            "longitude": 7.9166
         }
     },
     "STC": {
         "NOAA": {
             "height_station_masl": 6.0,
             "latitude": 54.0,
             "long_name": "Ocean Station Charlie, United States",
@@ -3765,27 +3854,27 @@
             "height": [
                 "185m",
                 "54m",
                 "100m"
             ],
             "height_name": [
                 "185magl",
-                "50magl",
-                "100magl"
+                "100magl",
+                "54magl"
             ],
             "height_station_masl": 64,
-            "latitude": 52.51811,
+            "latitude": 52.51882,
             "long_name": "Tacolneston Tower, UK",
-            "longitude": 1.13847
+            "longitude": 1.1387
         },
         "NOAA": {
             "height_station_masl": 64,
-            "latitude": 52.51811,
+            "latitude": 52.51882,
             "long_name": "Tacolneston, United Kingdom",
-            "longitude": 1.13847
+            "longitude": 1.1387
         }
     },
     "TAO": {
         "NOAA": {
             "height": [
                 "174m"
             ],
@@ -3934,17 +4023,17 @@
             "height": [
                 "12m"
             ],
             "height_name": [
                 "12magl"
             ],
             "height_station_masl": 825.0,
-            "latitude": 50.221884,
+            "latitude": 50.22188,
             "long_name": "Taunus, Germany",
-            "longitude": 8.446397
+            "longitude": 8.44639
         }
     },
     "TOH": {
         "ICOS": {
             "height": [
                 "147m"
             ],
@@ -4008,17 +4097,17 @@
             "height": [
                 "180m"
             ],
             "height_name": [
                 "180magl"
             ],
             "height_station_masl": 131.0,
-            "latitude": 47.965,
+            "latitude": 47.9647,
             "long_name": "Trainou, France",
-            "longitude": 2.112
+            "longitude": 2.1125
         },
         "NOAA": {
             "height": [
                 "5m"
             ],
             "height_name": [
                 "5magl"
@@ -4034,17 +4123,17 @@
             "height": [
                 "222m"
             ],
             "height_name": [
                 "222magl"
             ],
             "height_station_masl": 315,
-            "latitude": 56.55519,
+            "latitude": 56.55509,
             "long_name": "Angus Tower, UK",
-            "longitude": -2.98604
+            "longitude": -2.98598
         },
         "ICOS": {
             "height": [
                 "222m"
             ],
             "height_name": [
                 "222magl"
@@ -4099,14 +4188,26 @@
             "height_station_masl": 1327.0,
             "latitude": 39.9018,
             "long_name": "Wendover, Utah, United States",
             "longitude": -113.7181
         }
     },
     "UTO": {
+        "ICOS": {
+            "height": [
+                "57m"
+            ],
+            "height_name": [
+                "57magl"
+            ],
+            "height_station_masl": 8.0,
+            "latitude": 59.7839,
+            "long_name": "Uto, Finland",
+            "longitude": 21.3672
+        },
         "NOAA": {
             "height": [
                 "57m"
             ],
             "height_name": [
                 "57magl"
             ],
@@ -4126,14 +4227,27 @@
             ],
             "height_station_masl": 1007.0,
             "latitude": 44.452,
             "long_name": "Ulaan Uul, Mongolia",
             "longitude": 111.096
         }
     },
+    "VAL": {
+        "ICOS": {
+            "height": [
+                "10m"
+            ],
+            "height_name": [
+                "10magl"
+            ],
+            "latitude": 51.908,
+            "long_name": "Valentia, Ireland",
+            "longitude": -10.403
+        }
+    },
     "VGR": {
         "CNR": {
             "height": [
                 "5m"
             ],
             "height_name": [
                 "5magl"
@@ -4142,45 +4256,56 @@
             "latitude": 37.57111,
             "long_name": "Cape Granitola, Italy",
             "longitude": 12.65972
         }
     },
     "WAO": {
         "ICOS": {
+            "comments": "05/01/2023: Station elevation of 31m may be included within ICOS header but value above of 17m is more recently agreed upon value and should be correct.",
             "height": [
-                "21m"
-            ],
-            "height_name": [
-                "20magl"
+                "10m"
             ],
-            "height_station_masl": 10.0,
-            "latitude": 52.95042,
-            "long_name": "Weybourne Observatory, UK",
-            "longitude": 1.12194
+            "height_name": {
+                "10m": [
+                    "10magl",
+                    "20magl"
+                ]
+            },
+            "height_station_masl": 17.0,
+            "latitude": 52.9504,
+            "long_name": "WAO",
+            "longitude": 1.1219,
+            "reference": "https://meta.icos-cp.eu/resources/stations/AS_WAO"
         },
         "UCAM": {
             "height": [
-                "21m"
-            ],
-            "height_name": [
-                "20magl"
+                "10m"
             ],
-            "height_station_masl": 10.0,
+            "height_name": {
+                "10m": [
+                    "10magl",
+                    "20magl"
+                ]
+            },
+            "height_station_masl": 17.0,
             "latitude": 52.95042,
             "long_name": "Weybourne Observatory, UK",
             "longitude": 1.12194
         },
         "UEA": {
             "height": [
-                "21m"
-            ],
-            "height_name": [
-                "20magl"
+                "10m"
             ],
-            "height_station_masl": 10.0,
+            "height_name": {
+                "10m": [
+                    "10magl",
+                    "20magl"
+                ]
+            },
+            "height_station_masl": 17.0,
             "latitude": 52.95042,
             "long_name": "Weybourne Observatory, UK",
             "longitude": 1.12194
         }
     },
     "WBI": {
         "NOAA": {
@@ -4440,25 +4565,51 @@
             "long_name": "Yonagunijima, Japan",
             "longitude": 123.02
         }
     },
     "ZEP": {
         "AGAGE": {
             "height": [
-                "10m"
+                "12m"
             ],
             "height_name": [
-                "16magl"
+                "10magl"
             ],
             "height_station_masl": 474.0,
             "latitude": 78.925,
             "long_name": "Zeppelin, Ny Alesund, Norway",
             "longitude": 11.92222
         },
+        "ICOS": {
+            "height": [
+                "15m"
+            ],
+            "height_name": [
+                "10magl"
+            ],
+            "height_station_masl": 474.0,
+            "latitude": 78.9072,
+            "long_name": "Ny-Alesund, Svalbard, Norway and Sweden",
+            "longitude": 11.8867
+        },
         "NOAA": {
             "height_station_masl": 474.0,
             "latitude": 78.9067,
             "long_name": "Ny-Alesund, Svalbard, Norway and Sweden",
             "longitude": 11.8883
         }
+    },
+    "ZSF": {
+        "ICOS": {
+            "height": [
+                "3m"
+            ],
+            "height_name": [
+                "3magl"
+            ],
+            "height_station_masl": 2666,
+            "latitude": 47.4165,
+            "long_name": "Zugspitze Schneefernerhaus",
+            "longitude": 10.97964
+        }
     }
 }
```

### Comparing `openghg_defs-0.0.1/openghg_defs/data/species_info.json` & `openghg_defs-0.0.2/openghg_defs/data/species_info.json`

 * *Files identical despite different names*

### Comparing `openghg_defs-0.0.1/openghg_defs.egg-info/SOURCES.txt` & `openghg_defs-0.0.2/openghg_defs.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 pyproject.toml
 openghg_defs/__init__.py
 openghg_defs/py.typed
 openghg_defs.egg-info/PKG-INFO
 openghg_defs.egg-info/SOURCES.txt
 openghg_defs.egg-info/dependency_links.txt
 openghg_defs.egg-info/top_level.txt
+openghg_defs/__pycache__/__init__.cpython-310.pyc
+openghg_defs/__pycache__/__init__.cpython-39.pyc
+openghg_defs/__pycache__/_load.cpython-39.pyc
+openghg_defs/__pycache__/_paths.cpython-39.pyc
+openghg_defs/__pycache__/_version.cpython-310.pyc
 openghg_defs/data/domain_info.json
 openghg_defs/data/site_info.json
 openghg_defs/data/species_info.json
 openghg_defs/data/domain/ARCTIC_latitude.dat
 openghg_defs/data/domain/ARCTIC_longitude.dat
 openghg_defs/data/domain/EASTASIA_latitude.dat
 openghg_defs/data/domain/EASTASIA_longitude.dat
```

### Comparing `openghg_defs-0.0.1/pyproject.toml` & `openghg_defs-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = "openghg_defs"
-version = "0.0.1"
+version = "0.0.2"
 description = "Supplementary definition data for OpenGHG"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
+license = {text = "MIT License"}
 
 [project.urls]
-"Homepage" = "https://github.com/openghg/supplementary_data"
-"Bug Tracker" = "https://github.com/openghg/supplementary_data/issues"
+"Homepage" = "https://github.com/openghg/openghg_defs"
+"Bug Tracker" = "https://github.com/openghg/openghg_defs/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
```

