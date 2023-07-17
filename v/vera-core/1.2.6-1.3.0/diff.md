# Comparing `tmp/vera-core-1.2.6.tar.gz` & `tmp/vera-core-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vera-core-1.2.6.tar", last modified: Thu Jul 13 00:36:42 2023, max compression
+gzip compressed data, was "vera-core-1.3.0.tar", last modified: Mon Jul 17 22:14:41 2023, max compression
```

## Comparing `vera-core-1.2.6.tar` & `vera-core-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/
--rw-r--r--   0 root         (0) root         (0)      583 2023-07-13 00:35:53.000000 vera-core-1.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-13 00:35:53.000000 vera-core-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2023-07-13 00:36:42.010626 vera-core-1.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1639 2023-07-13 00:35:53.000000 vera-core-1.2.6/README.rst
--rw-r--r--   0 root         (0) root         (0)     1149 2023-07-13 00:36:42.010626 vera-core-1.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 00:35:53.000000 vera-core-1.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.002626 vera-core-1.2.6/vera_core/
--rw-r--r--   0 root         (0) root         (0)      583 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/LICENSE
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.006626 vera-core-1.2.6/vera_core/app/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.006626 vera-core-1.2.6/vera_core/app/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7741 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/core/vera_out_file.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1379 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.006626 vera-core-1.2.6/vera_core/app/ui/
--rw-r--r--   0 root         (0) root         (0)    12376 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/assembly_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/vera_core/app/ui/assets/
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4962 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/assets/logo.svg
--rw-r--r--   0 root         (0) root         (0)     3131 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/axial_plot.py
--rw-r--r--   0 root         (0) root         (0)     2011 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/core_view.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/empty.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/table_view.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/time_plot.py
--rw-r--r--   0 root         (0) root         (0)     6973 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/volume_view.py
--rw-r--r--   0 root         (0) root         (0)     3080 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/x_axial_view.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/y_axial_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/vera_core/module/
--rw-r--r--   0 root         (0) root         (0)      476 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/vera_core/module/serve/
--rw-r--r--   0 root         (0) root         (0)      365 2023-07-13 00:36:38.000000 vera-core-1.2.6/vera_core/module/serve/vue-vera_core.css
--rw-r--r--   0 root         (0) root         (0)   233904 2023-07-13 00:36:38.000000 vera-core-1.2.6/vera_core/module/serve/vue-vera_core.umd.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/vera_core/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/widgets/vera.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.002626 vera-core-1.2.6/vera_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      981 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.442061 vera-core-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-17 22:14:05.000000 vera-core-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-17 22:14:05.000000 vera-core-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-07-17 22:14:41.442061 vera-core-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-07-17 22:14:05.000000 vera-core-1.3.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-07-17 22:14:41.442061 vera-core-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 22:14:05.000000 vera-core-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.438061 vera-core-1.3.0/vera_core/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/LICENSE
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.438061 vera-core-1.3.0/vera_core/app/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.438061 vera-core-1.3.0/vera_core/app/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8274 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/core/vera_out_file.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.442061 vera-core-1.3.0/vera_core/app/ui/
+-rw-r--r--   0 root         (0) root         (0)    12190 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/assembly_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.442061 vera-core-1.3.0/vera_core/app/ui/assets/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4962 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/assets/logo.svg
+-rw-r--r--   0 root         (0) root         (0)     3131 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/axial_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/core_view.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/empty.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/table_view.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/time_plot.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/volume_view.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/x_axial_view.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/app/ui/y_axial_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.442061 vera-core-1.3.0/vera_core/module/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.442061 vera-core-1.3.0/vera_core/module/serve/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-07-17 22:14:38.000000 vera-core-1.3.0/vera_core/module/serve/vue-vera_core.css
+-rw-r--r--   0 root         (0) root         (0)   233904 2023-07-17 22:14:38.000000 vera-core-1.3.0/vera_core/module/serve/vue-vera_core.umd.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.442061 vera-core-1.3.0/vera_core/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-07-17 22:14:05.000000 vera-core-1.3.0/vera_core/widgets/vera.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 22:14:41.438061 vera-core-1.3.0/vera_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-07-17 22:14:41.000000 vera-core-1.3.0/vera_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      981 2023-07-17 22:14:41.000000 vera-core-1.3.0/vera_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 22:14:41.000000 vera-core-1.3.0/vera_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-17 22:14:41.000000 vera-core-1.3.0/vera_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-17 22:14:41.000000 vera-core-1.3.0/vera_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-17 22:14:41.000000 vera-core-1.3.0/vera_core.egg-info/top_level.txt
```

### Comparing `vera-core-1.2.6/LICENSE` & `vera-core-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/PKG-INFO` & `vera-core-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vera-core
-Version: 1.2.6
+Version: 1.3.0
 Summary: VERACore let you visualize and interpret the output data from VERA codes
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vera-core-1.2.6/README.rst` & `vera-core-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/setup.cfg` & `vera-core-1.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vera-core
-version = 1.2.6
+version = 1.3.0
 description = VERACore let you visualize and interpret the output data from VERA codes
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `vera-core-1.2.6/vera_core/LICENSE` & `vera-core-1.3.0/vera_core/LICENSE`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/app/core/vera_out_file.py` & `vera-core-1.3.0/vera_core/app/core/vera_out_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -205,21 +205,30 @@
 
     def reduced_core_map_column_label(self, assembly_idx):
         i, j = self.reduced_core_map_ij(assembly_idx)
         return self.reduced_core_map_column_labels[i]
 
 
 class VeraOutState(LazyHDF5Loader):
-    # These are the attributes that will be read from the HDF5 file
-    boron: H5_ARRAY_TYPE = None
-    detector_response: H5_ARRAY_TYPE = None
-    exposure: H5_ARRAY_TYPE = None
-    keff: H5_ARRAY_TYPE = None
-    pin_max_clad_surface_temp: H5_ARRAY_TYPE = None
-    pin_fuel_temp: H5_ARRAY_TYPE = None
-    pin_mod_dens: H5_ARRAY_TYPE = None
-    pin_mod_temp: H5_ARRAY_TYPE = None
-    pin_powers: H5_ARRAY_TYPE = None
-
     def __init__(self, f, idx):
+        # These are the attributes that will be read from the HDF5 file
+        self.__annotations__ = dict()
+
+        self.full_core_datasets = dict()
+        self.scalar_datasets = dict()
+        self.search_for_datasets(f, idx)
+        self.__annotations__.update(self.full_core_datasets)
+        self.__annotations__.update(self.scalar_datasets)
         super().__init__(f, f"/STATE_{idx:04}", list(self.__annotations__))
         self._index = idx
+
+    def search_for_datasets(self, f, idx):
+        # Search for available full core/scalar datasets at each state point
+        state = f[f"/STATE_{idx:04}"]
+        pin_powers = state["pin_powers"]
+        core_shape = np.shape(pin_powers)
+        for dataset_name in state.keys():
+            dataset_shape = np.shape(state[dataset_name])
+            if dataset_shape == core_shape:
+                self.full_core_datasets.update({dataset_name: "H5_ARRAY_TYPE = NONE"})
+            if dataset_shape in [(1,), ()]:
+                self.scalar_datasets.update({dataset_name: "H5_ARRAY_TYPE = NONE"})
```

### Comparing `vera-core-1.2.6/vera_core/app/jupyter.py` & `vera-core-1.3.0/vera_core/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/app/main.py` & `vera-core-1.3.0/vera_core/app/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 def _reload(vera_out_file):
     server = get_server()
     dev.reload(ui)
     ui.initialize(server, vera_out_file)
 
 
 def main(server=None, **kwargs):
-
     # Get or create server
     if server is None:
         server = get_server()
 
     if isinstance(server, str):
         server = get_server(server)
```

### Comparing `vera-core-1.2.6/vera_core/app/ui/__init__.py` & `vera-core-1.3.0/vera_core/app/ui/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     def selected_time_changed(selected_time, **kwargs):
         selected_time = int(selected_time)
         vera_out_file.active_state_index = selected_time
 
         ctrl.on_vera_out_active_state_index_changed(
             selected_time=selected_time, **kwargs
         )
+        # Automatically normalize color scale to current state
+        selected_array_changed(state.selected_array)
 
     @state.change("selected_array")
     def selected_array_changed(selected_array, **kwargs):
         array = vera_out_file.array(selected_array)
         state.color_range = (np.nanmin(array), np.nanmax(array))
 
     # Keep selected_assembly and selected_assembly_ij in sync
@@ -196,20 +198,16 @@
                 )
 
             vuetify.VSelect(
                 v_model=("selected_array", "pin_powers"),
                 items=(
                     "available_arrays",
                     [
-                        dict(text="Pin Powers", value="pin_powers"),
-                        dict(text="Pin Clad Temps", value="pin_max_clad_surface_temp"),
-                        dict(text="Pin Fuel Temps", value="pin_fuel_temp"),
-                        dict(text="Pin Moderator Density", value="pin_mod_dens"),
-                        dict(text="Pin Moderator Temps", value="pin_mod_temp"),
-                        dict(text="Pin Volumes", value="pin_volumes"),
+                        dict(text=key.replace("_", " ").title(), value=key)
+                        for key in vera_out_file.active_state.full_core_datasets.keys()
                     ],
                 ),
                 hide_details=True,
                 dense=True,
                 style="max-width: 220px",
             )
```

### Comparing `vera-core-1.2.6/vera_core/app/ui/assembly_view.py` & `vera-core-1.3.0/vera_core/app/ui/assembly_view.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/app/ui/assets/logo.svg` & `vera-core-1.3.0/vera_core/app/ui/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/app/ui/axial_plot.py` & `vera-core-1.3.0/vera_core/app/ui/axial_plot.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/app/ui/core_view.py` & `vera-core-1.3.0/vera_core/app/ui/core_view.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/app/ui/table_view.py` & `vera-core-1.3.0/vera_core/app/ui/table_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,20 +33,23 @@
     ):
         indices = (selected_j, selected_i, selected_layer, selected_assembly)
         indices = tuple(map(int, indices))
 
         array = vera_out_file.array(selected_array)
         value = array[indices]
 
-        data_dict = {
-            selected_array: value,
-            "boron": vera_out_file.active_state.boron[0],
-            "exposure": vera_out_file.active_state.exposure[0],
-            "keff": vera_out_file.active_state.keff[0],
-        }
+        data_dict = {selected_array.replace("_", " ").title(): value}
+        for scalar_dataset in vera_out_file.active_state.scalar_datasets.keys():
+            data_dict.update(
+                {
+                    scalar_dataset.replace("_", " ").title(): vera_out_file.array(
+                        scalar_dataset
+                    )[0]
+                }
+            )
 
         # Round floats so we don't display too many sig figs.
         # 7 sig figs matches veraview.
         sig_figs = 7
         data_dict = {
             k: float(f"{v:0.{sig_figs}g}")
             for k, v in data_dict.items()
```

### Comparing `vera-core-1.2.6/vera_core/app/ui/time_plot.py` & `vera-core-1.3.0/vera_core/app/ui/time_plot.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/app/ui/volume_view.py` & `vera-core-1.3.0/vera_core/app/ui/volume_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,17 +55,20 @@
     # FIXME: I'm not sure if this is accurate, so it is disabled for now
     # orientation_marker.EnabledOn()
     # orientation_marker.InteractiveOn()
 
     # FIXME: for now, let's make it fully opaque so it matches veraview
     # exactly.
     opacity_points = [
-        (0.00, 0),
-        (0.01, 1),
-        (1.95, 1),
+        (-10.0, 1),
+        (-0.00000000000000000001, 1),
+        (-0.000000000000000000005, 0.0),
+        (0.000000000000000000005, 0.0),
+        (0.00000000000000000001, 1),
+        (10.0, 1),
     ]
 
     # Create transfer mapping scalar value to opacity.
     opacity_transfer_function = vtkPiecewiseFunction()
     for point in opacity_points:
         opacity_transfer_function.AddPoint(*point)
```

### Comparing `vera-core-1.2.6/vera_core/app/ui/x_axial_view.py` & `vera-core-1.3.0/vera_core/app/ui/x_axial_view.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/app/ui/y_axial_view.py` & `vera-core-1.3.0/vera_core/app/ui/y_axial_view.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/module/serve/vue-vera_core.umd.min.js` & `vera-core-1.3.0/vera_core/module/serve/vue-vera_core.umd.min.js`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core/widgets/vera.py` & `vera-core-1.3.0/vera_core/widgets/vera.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.6/vera_core.egg-info/PKG-INFO` & `vera-core-1.3.0/vera_core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vera-core
-Version: 1.2.6
+Version: 1.3.0
 Summary: VERACore let you visualize and interpret the output data from VERA codes
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vera-core-1.2.6/vera_core.egg-info/SOURCES.txt` & `vera-core-1.3.0/vera_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

