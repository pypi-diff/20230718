# Comparing `tmp/tud_sumo-1.2.1.tar.gz` & `tmp/tud_sumo-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tud_sumo-1.2.1.tar", last modified: Mon Jul 10 12:41:08 2023, max compression
+gzip compressed data, was "tud_sumo-1.2.2.tar", last modified: Tue Jul 18 15:50:00 2023, max compression
```

## Comparing `tud_sumo-1.2.1.tar` & `tud_sumo-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-10 12:41:08.392556 tud_sumo-1.2.1/
--rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.2.1/.gitattributes
--rw-r--r--   0 callumevans (50765939) 1653728465       78 2023-05-26 14:50:47.000000 tud_sumo-1.2.1/.gitignore
--rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.2.1/LICENSE
--rw-r--r--   0 callumevans (50765939) 1653728465     4843 2023-07-10 12:41:08.392414 tud_sumo-1.2.1/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465     3236 2023-07-10 12:40:39.000000 tud_sumo-1.2.1/README.md
--rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-07-10 12:38:40.000000 tud_sumo-1.2.1/pyproject.toml
--rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-07-10 12:41:08.392600 tud_sumo-1.2.1/setup.cfg
--rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.2.1/setup.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-10 12:41:08.391305 tud_sumo-1.2.1/tud_sumo/
--rw-r--r--   0 callumevans (50765939) 1653728465    18624 2023-07-10 12:12:30.000000 tud_sumo-1.2.1/tud_sumo/tud_sumo.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-10 12:41:08.392208 tud_sumo-1.2.1/tud_sumo.egg-info/
--rw-r--r--   0 callumevans (50765939) 1653728465     4843 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/requires.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-07-10 12:41:08.000000 tud_sumo-1.2.1/tud_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-18 15:50:00.232788 tud_sumo-1.2.2/
+-rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.2.2/.gitattributes
+-rw-r--r--   0 callumevans (50765939) 1653728465       78 2023-05-26 14:50:47.000000 tud_sumo-1.2.2/.gitignore
+-rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.2.2/LICENSE
+-rw-r--r--   0 callumevans (50765939) 1653728465     4694 2023-07-18 15:50:00.232642 tud_sumo-1.2.2/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465     3087 2023-07-18 15:47:28.000000 tud_sumo-1.2.2/README.md
+-rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-07-18 15:47:40.000000 tud_sumo-1.2.2/pyproject.toml
+-rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-07-18 15:50:00.232833 tud_sumo-1.2.2/setup.cfg
+-rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.2.2/setup.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-18 15:50:00.231576 tud_sumo-1.2.2/tud_sumo/
+-rw-r--r--   0 callumevans (50765939) 1653728465    19186 2023-07-18 15:44:58.000000 tud_sumo-1.2.2/tud_sumo/tud_sumo.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-07-18 15:50:00.232460 tud_sumo-1.2.2/tud_sumo.egg-info/
+-rw-r--r--   0 callumevans (50765939) 1653728465     4694 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/requires.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-07-18 15:50:00.000000 tud_sumo-1.2.2/tud_sumo.egg-info/top_level.txt
```

### Comparing `tud_sumo-1.2.1/LICENSE` & `tud_sumo-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tud_sumo-1.2.1/PKG-INFO` & `tud_sumo-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud_sumo
-Version: 1.2.1
+Version: 1.2.2
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,20 +38,17 @@
 
 ## Requirements 
 
 Required packages are: `tqdm`, `matplotlib` and `traci`.
 
 ## Updates
 
-This is version '1.2.1', with the changelog:
-  - `sim.step_to()` is changed to `sim.step_through()` to better reflect usage
-  - Added `sim.vehicle_exists()` function
-  - `sim.all_curr_vehicle_ids` list
-  - Fixed heading and ts not updating in `sim.known_vehicles`
-  - Improved documentation
+This is version '1.2.2', with the changelog:
+  - Added `sim.get_vehicle_route()`
+  - Added `flatten` option to `sim.get_last_step_vehicles()`
 
 Check changes and previous versions through the project's [GitHub repository](https://github.com/calluume/tud_sumo).
 
 ## Usage examples
 
 ```python    
 from tud_sumo import tud_sumo
```

### Comparing `tud_sumo-1.2.1/README.md` & `tud_sumo-1.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,17 @@
 
 ## Requirements 
 
 Required packages are: `tqdm`, `matplotlib` and `traci`.
 
 ## Updates
 
-This is version '1.2.1', with the changelog:
-  - `sim.step_to()` is changed to `sim.step_through()` to better reflect usage
-  - Added `sim.vehicle_exists()` function
-  - `sim.all_curr_vehicle_ids` list
-  - Fixed heading and ts not updating in `sim.known_vehicles`
-  - Improved documentation
+This is version '1.2.2', with the changelog:
+  - Added `sim.get_vehicle_route()`
+  - Added `flatten` option to `sim.get_last_step_vehicles()`
 
 Check changes and previous versions through the project's [GitHub repository](https://github.com/calluume/tud_sumo).
 
 ## Usage examples
 
 ```python    
 from tud_sumo import tud_sumo
```

### Comparing `tud_sumo-1.2.1/pyproject.toml` & `tud_sumo-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tud_sumo"
-version = "1.2.1"
+version = "1.2.2"
 description = "TU Delft SUMO wrapper"
 readme = "README.md"
 authors = [{ name = "Callum Evans", email = "c.evans@tudelft.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `tud_sumo-1.2.1/tud_sumo/tud_sumo.py` & `tud_sumo-1.2.2/tud_sumo/tud_sumo.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,53 +272,52 @@
     def vehicle_exists(self, vehicle_id):
         """
         Tests if vehicle exists in the network
         :return bool: True if ID in list of current vehicle IDs 
         """
         return vehicle_id in self.all_curr_vehicle_ids
 
-    def get_last_step_vehicles(self, detector_ids = None) -> dict:
+    def get_last_step_vehicles(self, detector_ids = None, flatten = False) -> dict:
         """
         Get the IDs of vehicles that passed over the specified detectors
         :param detector_ids: detector ID or list of detector IDs (defaults to all)
-        :return dict: Dict containing vehicle IDs for each detector
+        :param flatten: If true, all IDs are returned in a 1D array, else a dict with vehicles for each detector
+        :return dict|list: Dict or list containing all vehicle IDs
         """
 
         detector_ids = list(self.available_detectors.keys()) if detector_ids == None else detector_ids
         detector_ids = [detector_ids] if not isinstance(detector_ids, list) else detector_ids
 
-        vehicle_ids = {}
+        vehicle_ids = [] if flatten else {}
         for detector_id in detector_ids:
             
             if detector_id not in self.available_detectors.keys(): raise KeyError("KeyError: Unknown detector_id '"+detector_id+"'")
             detector_type = self.available_detectors[detector_id]
 
             if detector_type == "inductionloop":
-                vehicle_ids[detector_id] = list(traci.inductionloop.getLastStepVehicleIDs(detector_id))
+                detected_vehicles = list(traci.inductionloop.getLastStepVehicleIDs(detector_id))
             elif detector_type == "multientryexit":
-                vehicle_ids[detector_id] = list(traci.multientryexit.getLastStepVehicleIDs(detector_id))
+                detected_vehicles = list(traci.multientryexit.getLastStepVehicleIDs(detector_id))
             else:
                 warn("Warning: Unknown detector type '"+detector_type+"'")
 
+            if flatten: vehicle_ids += detected_vehicles
+            else: vehicle_ids[detector_id] = detected_vehicles
+
         return vehicle_ids
     
     def get_vehicle_data(self, vehicle_id, vehicle_type = None):
         """
         Get data for specified vehicle, updating known_vehicles dict
         :param vehicle_id: vehicle ID
         :param vehicle_type: Vehicle type if known
         :return dict: Vehicle data dictionary, returns None if does not exist in simulation
         """
 
-        if vehicle_id not in self.all_curr_vehicle_ids: return None
-
-        if vehicle_type == None:
-            if "cbikes" in vehicle_id: vehicle_type = "cbikes"
-            elif "bikes" in vehicle_id: vehicle_type = "bikes"
-            else: vehicle_type = "cars"
+        if vehicle_id not in self.all_curr_vehicle_ids: raise KeyError("Vehicle '{0}' does not exist.".format(vehicle_id))
 
         speed = traci.vehicle.getSpeed(vehicle_id)
         lon, lat, alt = traci.vehicle.getPosition3D(vehicle_id)
         heading, ts = traci.vehicle.getAngle(vehicle_id), traci.vehicle.getDeparture(vehicle_id)
 
         if vehicle_id not in self.known_vehicles.keys():
             self.known_vehicles[vehicle_id] = {"type":      vehicle_type,
@@ -370,11 +369,22 @@
                 all_vehicle_data[vehicle_id] = vehicle_data
                     
                 total_vehicle_data["no_vehicles"] += 1
                 if vehicle_data["speed"] < 0.1: total_vehicle_data["no_waiting"] += 1
 
         return total_vehicle_data, all_vehicle_data
     
+    def get_vehicle_route(self, vehicle_id, get_edges = True):
+        """
+        Returns vehicle route, either route ID or array of edges.
+        :param vehicle_id: Vehicle ID
+        :param get_edges:  Denotes if to return list of edges or route ID
+        :return [str]|str: List of edges or route ID
+        """
+
+        if get_edges: return list(traci.vehicle.getRoute(vehicle_id))
+        else: return traci.vehicle.getRouteID(vehicle_id)
+    
 def get_cumulative_arr(arr, start) -> list:
     for i in range(start, len(arr)):
         arr[i] += arr[i - 1]
     return arr
```

### Comparing `tud_sumo-1.2.1/tud_sumo.egg-info/PKG-INFO` & `tud_sumo-1.2.2/tud_sumo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud-sumo
-Version: 1.2.1
+Version: 1.2.2
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,20 +38,17 @@
 
 ## Requirements 
 
 Required packages are: `tqdm`, `matplotlib` and `traci`.
 
 ## Updates
 
-This is version '1.2.1', with the changelog:
-  - `sim.step_to()` is changed to `sim.step_through()` to better reflect usage
-  - Added `sim.vehicle_exists()` function
-  - `sim.all_curr_vehicle_ids` list
-  - Fixed heading and ts not updating in `sim.known_vehicles`
-  - Improved documentation
+This is version '1.2.2', with the changelog:
+  - Added `sim.get_vehicle_route()`
+  - Added `flatten` option to `sim.get_last_step_vehicles()`
 
 Check changes and previous versions through the project's [GitHub repository](https://github.com/calluume/tud_sumo).
 
 ## Usage examples
 
 ```python    
 from tud_sumo import tud_sumo
```

