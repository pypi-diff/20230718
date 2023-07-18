# Comparing `tmp/PH-Baseliner-1.2.1.tar.gz` & `tmp/PH-Baseliner-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-Baseliner-1.2.1.tar", last modified: Wed Jul  5 20:28:52 2023, max compression
+gzip compressed data, was "dist/PH-Baseliner-1.3.0.tar", last modified: Tue Jul 18 14:24:19 2023, max compression
```

## Comparing `PH-Baseliner-1.2.1.tar` & `PH-Baseliner-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35149 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      762 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PH_Baseliner.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1589 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/README.md
--rw-r--r--   0 runner     (501) staff       (20)       44 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/ph_baseliner/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/
--rw-r--r--   0 runner     (501) staff       (20)    13031 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/ECCCNYS_2020.json
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2071 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/lighting_space_types.py
--rw-r--r--   0 runner     (501) staff       (20)    17467 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/model.py
--rw-r--r--   0 runner     (501) staff       (20)     1406 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/codes/options.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4685 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/areas.py
--rw-r--r--   0 runner     (501) staff       (20)     1484 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/components.py
--rw-r--r--   0 runner     (501) staff       (20)     1725 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/lighting.py
--rw-r--r--   0 runner     (501) staff       (20)     3285 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/u_values.py
--rw-r--r--   0 runner     (501) staff       (20)     5410 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phpp/windows.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2526 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/areas.py
--rw-r--r--   0 runner     (501) staff       (20)     2583 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/constructions.py
--rw-r--r--   0 runner     (501) staff       (20)      488 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/lighting.py
--rw-r--r--   0 runner     (501) staff       (20)     6888 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/ph_baseliner/phx/windows.py
--rw-r--r--   0 runner     (501) staff       (20)       87 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      839 2023-07-05 20:28:52.000000 PH-Baseliner-1.2.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-07-05 20:25:27.000000 PH-Baseliner-1.2.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/PH_Baseliner.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/PH_Baseliner.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      762 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/PH_Baseliner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/PH_Baseliner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/PH_Baseliner.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       44 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/ph_baseliner/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/ph_baseliner/codes/
+-rw-r--r--   0 runner     (501) staff       (20)    13031 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/codes/ECCCNYS_2020.json
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/codes/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2072 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/codes/lighting_space_types.py
+-rw-r--r--   0 runner     (501) staff       (20)    17467 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/codes/model.py
+-rw-r--r--   0 runner     (501) staff       (20)     1406 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/codes/options.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/ph_baseliner/phpp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phpp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4691 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phpp/areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     1484 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phpp/components.py
+-rw-r--r--   0 runner     (501) staff       (20)     2510 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phpp/lighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     3285 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phpp/u_values.py
+-rw-r--r--   0 runner     (501) staff       (20)     5618 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phpp/windows.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/ph_baseliner/phx/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phx/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2526 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phx/areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     2583 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phx/constructions.py
+-rw-r--r--   0 runner     (501) staff       (20)      488 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phx/lighting.py
+-rw-r--r--   0 runner     (501) staff       (20)     6888 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/ph_baseliner/phx/windows.py
+-rw-r--r--   0 runner     (501) staff       (20)       87 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)      839 2023-07-18 14:24:19.000000 PH-Baseliner-1.3.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2023-07-18 14:20:26.000000 PH-Baseliner-1.3.0/setup.py
```

### Comparing `PH-Baseliner-1.2.1/.github/workflows/ci.yaml` & `PH-Baseliner-1.3.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/LICENSE` & `PH-Baseliner-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/PH_Baseliner.egg-info/PKG-INFO` & `PH-Baseliner-1.3.0/PH_Baseliner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-Baseliner
-Version: 1.2.1
+Version: 1.3.0
 Summary: Tools to automatically setup the code-minimum Baseline values for Passive House models.
 Home-page: https://github.com/PH-Tools/PH_Baseliner
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Baseliner:
         Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
```

### Comparing `PH-Baseliner-1.2.1/PH_Baseliner.egg-info/SOURCES.txt` & `PH-Baseliner-1.3.0/PH_Baseliner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/PKG-INFO` & `PH-Baseliner-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-Baseliner
-Version: 1.2.1
+Version: 1.3.0
 Summary: Tools to automatically setup the code-minimum Baseline values for Passive House models.
 Home-page: https://github.com/PH-Tools/PH_Baseliner
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Baseliner:
         Tools to automatically setup the code-minimum 'Baseline' values for Passive House models.
```

### Comparing `PH-Baseliner-1.2.1/README.md` & `PH-Baseliner-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/codes/ECCCNYS_2020.json` & `PH-Baseliner-1.3.0/ph_baseliner/codes/ECCCNYS_2020.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986111111111112%*

 * *Differences: {"'tables'": "{'lighting_area_method': {'LPD': {replace: OrderedDict([('AUTOMOTIVE FACILITY', "*

 * *             "0.71), ('CONVENTION CENTER', 0.76), ('COURTHOUSE', 0.9), ('DINING: BAR "*

 * *             "LOUNGE/LEISURE', 0.9), ('DINING: CAFETERIA/FAST FOOD', 0.79), ('DINING: FAMILY', "*

 * *             "0.78), ('DORMITORY', 0.61), ('EXERCISE CENTER', 0.65), ('FIRE STATION', 0.53), "*

 * *             "('GYMNASIUM', 0.68), ('HEALTH CARE CLINIC', 0.82), ('HOSPITAL', 1.05), "*

 * *             "('HOTEL/MOTEL', 0.75), ('LIBRARY', 0 […]*

```diff
@@ -148,46 +148,46 @@
                 }
             },
             "source_url": "https://up.codes/viewer/new_york/ny-energy-conservation-code-2020/chapter/CE_4/ce-commercial-energy-efficiency#C402.4",
             "units": "Btu/hr-ft2-F"
         },
         "lighting_area_method": {
             "LPD": {
-                "Automotive facility": 0.71,
-                "Convention center": 0.76,
-                "Courthouse": 0.9,
-                "Dining: bar lounge/leisure": 0.9,
-                "Dining: cafeteria/fast food": 0.79,
-                "Dining: family": 0.78,
-                "Dormitory": 0.61,
-                "Exercise center": 0.65,
-                "Fire station": 0.53,
-                "Gymnasium": 0.68,
-                "Health care clinic": 0.82,
-                "Hospital": 1.05,
-                "Hotel/Motel": 0.75,
-                "Library": 0.78,
-                "Manufacturing facility": 0.9,
-                "Motion picture theater": 0.83,
-                "Multifamily": 0.68,
-                "Museum": 1.06,
-                "Office": 0.79,
-                "Parking garage": 0.15,
-                "Penitentiary": 0.75,
-                "Performing arts theater": 1.18,
-                "Police station": 0.8,
-                "Post office": 0.67,
-                "Religious building": 0.94,
-                "Retail": 1.06,
-                "School/university": 0.81,
-                "Sports arena": 0.87,
-                "Town hall": 0.8,
-                "Transportation": 0.61,
-                "Warehouse": 0.48,
-                "Workshop": 0.9
+                "AUTOMOTIVE FACILITY": 0.71,
+                "CONVENTION CENTER": 0.76,
+                "COURTHOUSE": 0.9,
+                "DINING: BAR LOUNGE/LEISURE": 0.9,
+                "DINING: CAFETERIA/FAST FOOD": 0.79,
+                "DINING: FAMILY": 0.78,
+                "DORMITORY": 0.61,
+                "EXERCISE CENTER": 0.65,
+                "FIRE STATION": 0.53,
+                "GYMNASIUM": 0.68,
+                "HEALTH CARE CLINIC": 0.82,
+                "HOSPITAL": 1.05,
+                "HOTEL/MOTEL": 0.75,
+                "LIBRARY": 0.78,
+                "MANUFACTURING FACILITY": 0.9,
+                "MOTION PICTURE THEATER": 0.83,
+                "MULTIFAMILY": 0.68,
+                "MUSEUM": 1.06,
+                "OFFICE": 0.79,
+                "PARKING GARAGE": 0.15,
+                "PENITENTIARY": 0.75,
+                "PERFORMING ARTS THEATER": 1.18,
+                "POLICE STATION": 0.8,
+                "POST OFFICE": 0.67,
+                "RELIGIOUS BUILDING": 0.94,
+                "RETAIL": 1.06,
+                "SCHOOL/UNIVERSITY": 0.81,
+                "SPORTS ARENA": 0.87,
+                "TOWN HALL": 0.8,
+                "TRANSPORTATION": 0.61,
+                "WAREHOUSE": 0.48,
+                "WORKSHOP": 0.9
             },
             "name": "Interior Lighting Power Allowances: Building Area Method",
             "section": "C405.3.2(1)",
             "source_url": "https://up.codes/viewer/new_york/ny-energy-conservation-code-2020/chapter/CE_4/ce-commercial-energy-efficiency#C405.3.2",
             "units": "W/FT2"
         },
         "maximum_u_factors": {
```

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/codes/model.py` & `PH-Baseliner-1.3.0/ph_baseliner/codes/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
     LPD: dict
 
     @validator("LPD", pre=False)
     @classmethod
     def convert_units(cls, v: Dict, values: Dict):
         units = values["units"]
         for key, val in v.items():
-            v[key] = convert(val, units, "W/m2")
+            v[key] = convert(val, units, "W/M2")
         return v
 
 
 # -----------------------------------------------------------------------------
 
 
 class SectionMaximumFenestrationArea(BaseModel):
```

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/codes/options.py` & `PH-Baseliner-1.3.0/ph_baseliner/codes/options.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/phpp/areas.py` & `PH-Baseliner-1.3.0/ph_baseliner/phpp/areas.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     )
     reset_phpp_areas_constructions(phpp_conn, construction_phpp_ids)
 
 
 def reset_phpp_areas_constructions(
     phpp_conn: phpp_app.PHPPConnection, construction_ids: BaselineConstructionPHPPids
 ) -> None:
-    """Reset the PHPP Areas worksheet to the baseline constructions."""
+    """Reset the PHPP Areas worksheet rows to the baseline constructions."""
 
     def row_is_exposed_wall(row_data: ExistingSurfaceRow) -> bool:
         """Exposed wall is a wall that is not a ground floor."""
         return (
             row_data.face_type == ComponentFaceType.WALL
             and row_data.face_exposure == ComponentExposureExterior.EXTERIOR
         )
@@ -84,15 +84,15 @@
         """Exposed floor is a floor that is not a ground floor."""
         return (
             row_data.face_type == ComponentFaceType.FLOOR
             and row_data.face_exposure == ComponentExposureExterior.EXTERIOR
         )
 
     for i, surface_row_data in phpp_conn.areas.surfaces.all_surface_rows:
-        if surface_row_data.no_name:
+        if surface_row_data.is_empty:
             continue
 
         if row_is_roof(surface_row_data):
             phpp_conn.areas.set_surface_row_construction(i, construction_ids.roof)
             phpp_conn.areas.set_surface_row_solar_absorptivity(i, 0.75)
             phpp_conn.areas.set_surface_row_emissivity(i, 0.90)
         elif row_is_exposed_wall(surface_row_data):
```

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/phpp/components.py` & `PH-Baseliner-1.3.0/ph_baseliner/phpp/components.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/phpp/lighting.py` & `PH-Baseliner-1.3.0/ph_baseliner/phpp/lighting.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,53 @@
 # -*- coding: utf-8 -*-
 # -*- Python Version: 3.7 -*-
 
 """Functions to set baseline PHPP lighting."""
 
+from typing import Optional
+
 from PHX.PHPP.phpp_app import PHPPConnection
 
 from ph_baseliner.codes.model import BaselineCode
 from ph_baseliner.codes.lighting_space_types import space_type_map
 
 
 def find_lighting_installed_power(
     _baseline_code: BaselineCode, _program_name: str
-) -> float:
-    """Find the baseline lighting installed power density for a given PHPP space."""
+) -> Optional[float]:
+    """Find the baseline lighting installed power density for a given PHPP space.
+
+    Arguments:
+    ----------
+        * _baseline_code: BaselineCode
+            The BaselineCode object
+        * _program_name: str
+            The PHPP space type name
+
+    Returns:
+    --------
+        * code_LPD: Optional[float]
+            The baseline lighting installed power density for the given PHPP space type
+    """
 
-    # -- First, find the building-code name for the PHPP space type
-    code_name = space_type_map.get(_program_name, None)
+    # -- First, find the building-code name which corresponds to the PHPP space type
+    code_name = space_type_map.get(_program_name.upper().strip(), None)
 
-    if not code_name:
+    if (
+        not code_name
+        or code_name not in _baseline_code.tables.lighting_area_method.LPD.keys()
+    ):
         msg = (
-            f"Error: The PHPP Space-Type name {_program_name} does not have a "
-            "corresponding building-code name?"
+            f"> Warning: The PHPP Space-Type: '{_program_name}' does not have a corresponding "
+            "building-code lighting-space-type? Cannot set electric lighting baseline. "
+            "You should set the electric lighting installer power density manually on the "
+            "PHPP 'Electricity non-res' worksheet."
         )
-        raise Exception(msg)
+        print(msg)
+        return None
 
     # -- Then, find the lighting installed power density for that building-code name
     return _baseline_code.tables.lighting_area_method.LPD[code_name]
 
 
 def set_baseline_lighting_installed_power_density(
     _phpp_conn: PHPPConnection, _baseline_code: BaselineCode
@@ -42,8 +63,12 @@
     """
 
     for row_num in _phpp_conn.elec_non_res.lighting.used_lighting_row_numbers:
         row_data = _phpp_conn.elec_non_res.lighting.get_lighting_row_data(row_num)
         code_LPD = find_lighting_installed_power(
             _baseline_code, row_data.utilization_profile_name
         )
-        _phpp_conn.elec_non_res.lighting.set_lighting_power_density(row_num, code_LPD)
+        if not code_LPD:
+            continue
+        _phpp_conn.elec_non_res.lighting.set_lighting_power_density(
+            row_num, code_LPD, "W/M2"
+        )
```

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/phpp/u_values.py` & `PH-Baseliner-1.3.0/ph_baseliner/phpp/u_values.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/phpp/windows.py` & `PH-Baseliner-1.3.0/ph_baseliner/phpp/windows.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,26 +90,30 @@
     #
     # -- So be sure to use the GROSS wall area, BEFORE the windows
     # -- have been punched out of them.
 
     maximum_wwr = _baseline_code.get_baseline_max_wwr()
     current_net_wall_area = _phpp_conn.areas.get_total_net_wall_area()
     current_window_area = _phpp_conn.windows.get_total_window_area()
-    current_wwr = current_window_area / (current_net_wall_area + current_window_area)
+    total_gross_wall_area = current_net_wall_area + current_window_area
+    current_wwr = current_window_area / total_gross_wall_area
 
     if current_wwr < maximum_wwr:
-        print(f"Current WWR {current_wwr:.2%} is less than maximum {maximum_wwr:.0%}.")
+        print(
+            f"Current WWR {current_wwr.value :.2%} is less than maximum {maximum_wwr :.0%}."
+        )
         return None
 
     print(
-        f"Current WWR {current_wwr:.2%} is greater than maximum {maximum_wwr:.0%}. Scaling windows."
+        f"Current WWR {current_wwr.value :.2%} is greater than "
+        f"maximum {maximum_wwr :.0%}. Scaling windows."
     )
 
     # -- Figure out the right scale factor
-    scale_factor = maximum_wwr / current_wwr
+    scale_factor = maximum_wwr / current_wwr.value
 
     # -- Scale the window areas
     for row_num in _phpp_conn.windows.used_window_row_numbers:
         if not _phpp_conn.windows.row_is_window(row_num):
             continue
 
         _phpp_conn.windows.scale_window_size(row_num, scale_factor)
@@ -126,26 +130,30 @@
             The PHPPConnection object
         baseline_code: BaselineCode
             The BaselineCode object
     """
     maximum_srr = _baseline_code.get_baseline_max_srr()
     current_roof_area = _phpp_conn.areas.get_total_net_roof_area()
     current_skylight_area = _phpp_conn.windows.get_total_skylight_area()
-    current_srr = current_skylight_area / (current_roof_area + current_skylight_area)
+    total_gross_roof_area = current_roof_area + current_skylight_area
+    current_srr = current_skylight_area / total_gross_roof_area
 
     if current_srr < maximum_srr:
-        print(f"Current SRR {current_srr:.2%} is less than maximum {maximum_srr:.0%}.")
+        print(
+            f"Current SRR {current_srr.value :.2%} is less than maximum {maximum_srr :.0%}."
+        )
         return None
 
     print(
-        f"Current SRR {current_srr:.2%} is greater than maximum {maximum_srr:.0%}. Scaling Skylights."
+        f"Current SRR {current_srr.value :.2%} is greater than "
+        f"maximum {maximum_srr :.0%}. Scaling Skylights."
     )
 
     # -- Figure out the right scale factor
-    scale_factor = maximum_srr / current_srr
+    scale_factor = maximum_srr / current_srr.value
 
     # -- Scale the window areas
     for row_num in _phpp_conn.windows.used_window_row_numbers:
         if not _phpp_conn.windows.row_is_skylight(row_num):
             continue
 
         _phpp_conn.windows.scale_window_size(row_num, scale_factor)
```

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/phx/areas.py` & `PH-Baseliner-1.3.0/ph_baseliner/phx/areas.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/phx/constructions.py` & `PH-Baseliner-1.3.0/ph_baseliner/phx/constructions.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/ph_baseliner/phx/windows.py` & `PH-Baseliner-1.3.0/ph_baseliner/phx/windows.py`

 * *Files identical despite different names*

### Comparing `PH-Baseliner-1.2.1/setup.cfg` & `PH-Baseliner-1.3.0/setup.cfg`

 * *Files identical despite different names*

