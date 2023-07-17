# Comparing `tmp/climatePy-0.4.32.tar.gz` & `tmp/climatePy-0.4.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.32.tar", last modified: Sun Jul 16 12:54:45 2023, max compression
+gzip compressed data, was "climatePy-0.4.33.tar", last modified: Mon Jul 17 22:08:41 2023, max compression
```

## Comparing `climatePy-0.4.32.tar` & `climatePy-0.4.33.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.252102 climatePy-0.4.32/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-16 12:54:42.000000 climatePy-0.4.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-16 12:54:45.252102 climatePy-0.4.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-16 12:54:42.000000 climatePy-0.4.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.200102 climatePy-0.4.32/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    62112 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    30062 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.204102 climatePy-0.4.32/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-16 12:54:42.000000 climatePy-0.4.32/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.204102 climatePy-0.4.32/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 12:54:45.000000 climatePy-0.4.32/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:54:45.252102 climatePy-0.4.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-16 12:54:44.000000 climatePy-0.4.32/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:45.252102 climatePy-0.4.32/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:54:42.000000 climatePy-0.4.32/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-16 12:54:42.000000 climatePy-0.4.32/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-16 12:54:42.000000 climatePy-0.4.32/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.430617 climatePy-0.4.33/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-17 22:08:37.000000 climatePy-0.4.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-17 22:08:41.430617 climatePy-0.4.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-17 22:08:37.000000 climatePy-0.4.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.386617 climatePy-0.4.33/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22670 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63216 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32241 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.386617 climatePy-0.4.33/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-17 22:08:37.000000 climatePy-0.4.33/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.386617 climatePy-0.4.33/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 22:08:41.000000 climatePy-0.4.33/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:08:41.430617 climatePy-0.4.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-17 22:08:39.000000 climatePy-0.4.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:41.430617 climatePy-0.4.33/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:08:37.000000 climatePy-0.4.33/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-17 22:08:37.000000 climatePy-0.4.33/tests/test_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-17 22:08:37.000000 climatePy-0.4.33/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-17 22:08:37.000000 climatePy-0.4.33/tests/test_utils.py
```

### Comparing `climatePy-0.4.32/LICENSE` & `climatePy-0.4.33/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.32/PKG-INFO` & `climatePy-0.4.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.32
+Version: 0.4.33
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.32/README.md` & `climatePy-0.4.33/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.32/climatePy/__init__.py` & `climatePy-0.4.33/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.32/climatePy/_climatepy_filter.py` & `climatePy-0.4.33/climatePy/_climatepy_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # import climatePy._utils as utils
 # from climatePy import params
 
 # warnings lib
 import warnings
 
 # suppress warnings
-warnings.filterwarnings('ignore', category=Warning)
+# warnings.filterwarnings('ignore', category=Warning)
 
 ################################
 
 # Find the maximum bounding box of the AOI
 def get_max_bbox(AOI):
     """Find the maximum bounding box of the AOI.
 
@@ -178,30 +178,46 @@
     
     # 1. model filter
     if model is not None:
 
         # unique models
         u = catalog['model'].unique()
 
+        # if model is an integer or float, randomly select that many models
+        if isinstance(model, (int, float)):
+            # convert float to integer
+            if isinstance(model, float):
+                model = int(model)
+            if len(u) >= model:
+                model = np.random.choice(u, model, replace=False).tolist()
+            else:
+                raise ValueError(f"There are only {len(u)} unique models.")
         if isinstance(model, str):
-            if model not in u:
+            if model in u:
+                catalog = catalog[catalog['model'] == model]
+                # catalog = catalog[catalog['model'].str.contains(model, na=False)]
+
+                # set model to list
+                model = [model]
+            else:
+            # if model not in u:
                 bad = model
                 m = catalog[['model', 'ensemble']].drop_duplicates()
                 message = f"'{bad}' not avaliable model for '{catalog.iloc[0]['id']}'. Try: \n\t{'> ' + m['model'] + ' [' + m['ensemble'] + ']' }"
                 raise Exception(message)
-            catalog = catalog[catalog['model'].str.contains(model)]
+            # catalog = catalog[catalog['model'].str.contains(model, na=False)]
         elif isinstance(model, list):
-            if not all(elem in u for elem in model):
+            if all(elem in u for elem in model):
+                catalog = catalog[catalog['model'].isin(model)]
+                # catalog = catalog[catalog['model'].str.contains('|'.join(model), na=False)]
+            else:
                 bad = list(set(model) - set(u))
                 m = catalog[['model', 'ensemble']].drop_duplicates()
                 message = f"'{bad}' not avaliable model for '{catalog.iloc[0]['id']}'. Try: \n\t{'> ' + m['model'] + ' [' + m['ensemble'] + ']' }"
                 raise Exception(message)
-            catalog = catalog[catalog['model'].str.contains('|'.join(model))]
-        # else:
-        #     catalog = catalog[catalog['model'].str.contains('|'.join(model))]
 
     # 2. varname filter 
     if varname is not None:
         
         # make sure varname is a list type
         if isinstance(varname, str):
             varname = [varname]
@@ -242,33 +258,66 @@
     # 4. scenario filter
     if scenario is not None:
         if "historical" in catalog["scenario"].unique():
             scenario = ["historical", scenario]
 
         if scenario is not None:
             if isinstance(scenario, str):
-                catalog = catalog[catalog['scenario'].str.contains(scenario)]
+                catalog = catalog[catalog['scenario'].str.contains(scenario, na=False)]
+                # catalog = catalog[catalog['scenario'].str.contains(scenario)]
             elif isinstance(scenario, list):
-                catalog = catalog[catalog['scenario'].str.contains('|'.join(scenario))]
+                catalog = catalog[catalog['scenario'].str.contains('|'.join(scenario), na=False)]
+                # catalog = catalog[catalog['scenario'].str.contains('|'.join(scenario))]
 
+    # 5. ensemble filter
+    if ensemble is not None:
+        if isinstance(ensemble, str):
+            ensemble = [ensemble]
+
+        # if ensemble is not None and there are more or less ensembles than there are models, groupby model and ensemble:
+        if model is not None and len(ensemble) != len(model):
+            catalog = (catalog
+                        .groupby(['model', 'ensemble'])
+                        .first()
+                        .reset_index()
+                        )
+        else:
+            # unique ensembles
+            u = catalog['ensemble'].unique()
+
+            # if there are more than one ensemble and ensemble is NULL, default to the first ensemble
+            if len(u) > 1 and ensemble is None:
+                warnings.warn(f"There are {len(u)} ensembles available. Since ensemble was left NULL, we default to {u[0]}.", UserWarning)
+                catalog = catalog[catalog['ensemble'].isin([u[0]])]
+            elif ensemble is None:
+                catalog = catalog
+            else:
+                if all(item in u for item in ensemble):
+                    catalog = catalog[catalog['ensemble'].isin(ensemble)]
+                else:
+                    bad = list(set(ensemble) - set(u))
+                    m = catalog[['model', 'ensemble']].drop_duplicates()
+                    message = f"'{bad}' not avaliable ensemble for '{catalog.iloc[0]['id']}'. Try: \n\t{'> ' + m['model'] + ' [' + m['ensemble'] + ']' }"
+                    raise Exception(message)
+            
     # # # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
     # if isinstance(AOI, (shapely.geometry.point.Point, 
     #         shapely.geometry.multipoint.MultiPoint,
     #         shapely.geometry.linestring.LineString, 
     #         shapely.geometry.multilinestring.MultiLineString, 
     #         shapely.geometry.polygon.Polygon, 
     #         shapely.geometry.multipolygon.MultiPolygon)):
         
     #     # convert shapely geometry to geopandas dataframe
     #     AOI = utils.shapely_to_gpd(AOI)
 
     # check that AOI meets requirements, if a shapely geometry the AOI is transformed into a geodataframe
     AOI = utils.check_aoi(AOI)
 
-    # 5. AOI filter
+    # 6. AOI filter
     if AOI is not None:
         catalog = find_intersects(
             catalog = catalog,
             AOI     = AOI
             )
         
     # remove duplicates
```

### Comparing `climatePy-0.4.32/climatePy/_dap.py` & `climatePy-0.4.33/climatePy/_dap.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,25 +563,41 @@
     # clean up timeseries names
     names_ts = "_".join([vars, dap_row["model"], dap_row["ensemble"], dap_row["scenario"]])
     names_ts = names_ts.replace("_NA", "")
     names_ts = names_ts.replace("_na", "")
     names_ts = names_ts.replace("__", "_")
     names_ts = names_ts.rstrip("_")
 
+    # # if dap_row has 1 column and 1 row, or 1 key/value
+    # if len(dap_row.keys()) == 1 and len(dap_row.values()) == 1:
+    #     # reshape var into a 2D array
+    #     var_2d = var.reshape((len(dates), -1))
+
+    #     # create a dictionary of column names and values
+    #     var_dict = {f'var_{i}': var_2d[:, i] for i in range(var_2d.shape[1])}
+    #     var_dict = {key.replace("var_", f'{names_ts}_'): var_dict[key] for key in var_dict.keys()}
+
+    #     # create a DataFrame with dates and var_dict as columns
+    #     df = pd.DataFrame({'date': dates, **var_dict})
+
     # if dap_row has 1 column and 1 row, or 1 key/value
-    if len(dap_row.keys()) == 1 and len(dap_row.values()) == 1:
+    if dap_row['ncols'] == 1 and dap_row['nrows'] == 1:
         # reshape var into a 2D array
-        var_2d = var.reshape((len(dates), -1))
-
+        # var_2d = var.reshape((len(dates), -1))
+ 
         # create a dictionary of column names and values
-        var_dict = {f'var_{i}': var_2d[:, i] for i in range(var_2d.shape[1])}
-        var_dict = {key.replace("var_", f'{names_ts}_'): var_dict[key] for key in var_dict.keys()}
+        # var_dict = {f'var_{i}': var_2d[:, i] for i in range(var_2d.shape[1])}
+        # var_dict = {key.replace("var_", f'{names_ts}_'): var_dict[key] for key in var_dict.keys()}
 
         # create a DataFrame with dates and var_dict as columns
-        df = pd.DataFrame({'date': dates, **var_dict})
+        # df = pd.DataFrame({'date': dates, **var_dict})
+        # create a DataArray with dates and the variable array as the other column
+        df = pd.DataFrame({'date': dates, names_ts:np.squeeze(var.values)})
+        
+        return df
 
     # x resolution
     resx = (dap_row['Xn'] - dap_row['X1'])/(dap_row['ncols'] - 1)
 
     # y resolution
     resy = (dap_row['Yn'] - dap_row['Y1'])/(dap_row['nrows'] - 1)
 
@@ -789,14 +805,22 @@
         # # next is to loop over each row in dap_data and call go_get_dap_data
         for i in range(len(dap_data)):
             if verbose:
                 print(f'Getting dap data: ({i+1}/{n})')
 
             x = go_get_dap_data(dap_row = dap_data.iloc[i].to_dict())
             out.append(x)
+
+    # If out returns a list of dataframes (typically because a single point was given as the AOI),
+    # then process the list of dataframes into a single dataframe and return it (timeseries data of the point)
+    if isinstance(out[0], pd.core.frame.DataFrame):
+        
+        out = utils.aggreg_pt_dataframes(out)
+
+        return out
     
     # add variable name attribute to each DataArray in the output list
     add_varname_attr(
         out      = out,
         dap_data = dap_data, 
         verbose  = verbose
         )
```

### Comparing `climatePy-0.4.32/climatePy/_netrc_utils.py` & `climatePy-0.4.33/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.32/climatePy/_shortcuts.py` & `climatePy-0.4.33/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.32/climatePy/_utils.py` & `climatePy-0.4.33/climatePy/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,60 @@
 
 # warnings lib
 import warnings
 
 # suppress warnings
 warnings.filterwarnings('ignore', category=Warning)
 
+def aggreg_pt_dataframes(df_list):
+    """
+    Process, concatenate, and pivot a list of Pandas DataFrames and return a wide DataFrame
+    with a column for the 'date' and a separate column for each variable that data was retrieved for.
+
+    This function is for internal use only and runs only if a list of dataframes is returned from 'go_get_dap_data'. 
+    Handles the cases when a point is given to `dap()` and the return data results in a single grid cell.
+
+    Args:
+        out (list): A list of pandas DataFrames returned from 'go_get_dap_data' function calls.
+
+    Returns:
+        pandas.DataFrame: A wide DataFrame with a 'date' column and separate columns for each variable.
+    """
+
+    # Loop through each dataframe in df_list
+    for i in range(len(df_list)):
+        # print(f"i: {i}")
+        
+        # Column names of dataframe
+        colnames = df_list[i].columns
+        
+        # Extract column names that are NOT the "date" column
+        id_row = "".join(colnames[colnames != "date"])
+        # [c for c in out[i].columns if c != "date"]
+        # print(f"id_row: {id_row}")
+        
+        # Set column names to "date" and "value"
+        df_list[i].columns = ["date", "value"]
+        
+        # Give the original dataset name, that was stored as a column header, as a new "name" column in the dataframe
+        df_list[i]["name"] = id_row
+        
+        # print(f'-----------')
+    
+    # Concatenate the list of dataframes into a single dataframe
+    df_list = pd.concat(df_list, axis=0)
+    
+    # Pivot data from long to wide
+    df_list = df_list.pivot(index="date", columns="name", values="value")
+    
+    # Reset date index
+    df_list = df_list.reset_index()
+    
+    return df_list
+
 def shapely_to_gpd(AOI):
 
     """Convert a Shapely object to a GeoDataFrame.
 
     Args:
         AOI (shapely.geometry.base.BaseGeometry): The area of interest as a Shapely object.
 
@@ -93,14 +139,23 @@
             xmin, ymin, xmax, ymax = AOI.geometry.total_bounds
             AOI = gpd.GeoDataFrame(geometry=[shapely.geometry.box(xmin, ymin, xmax, ymax)], crs=AOI.crs)
             # bb = AOI.geometry.total_bounds
             # AOI = gpd.GeoDataFrame(geometry=[shapely.geometry.box(bb[0], bb[1], bb[2], bb[3])], crs=AOI.crs)
 
             return AOI
         
+        # if single geometry and its a point, create a bounding box around the point w/ a small buffer
+        if AOI.geometry.geom_type.to_list()[0] == "Point":
+            xmin, ymin, xmax, ymax = AOI.buffer(0.005).geometry.total_bounds
+            # xmin, ymin, xmax, ymax = AOI.geometry.total_bounds
+            
+            AOI = gpd.GeoDataFrame(geometry=[shapely.geometry.box(xmin, ymin, xmax, ymax)], crs=AOI.crs)
+
+            return AOI
+        
     # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
     if isinstance(AOI, (shapely.geometry.point.Point, 
                         shapely.geometry.multipoint.MultiPoint,
                         shapely.geometry.linestring.LineString, 
                         shapely.geometry.multilinestring.MultiLineString, 
                         shapely.geometry.polygon.Polygon, 
                         shapely.geometry.multipolygon.MultiPolygon)):
```

### Comparing `climatePy-0.4.32/climatePy/data/catalog.csv` & `climatePy-0.4.33/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.32/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.33/climatePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.32
+Version: 0.4.33
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.32/setup.py` & `climatePy-0.4.33/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.32',
+    version='0.4.33',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.32/tests/test_shortcuts.py` & `climatePy-0.4.33/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.32/tests/test_utils.py` & `climatePy-0.4.33/tests/test_utils.py`

 * *Files identical despite different names*

