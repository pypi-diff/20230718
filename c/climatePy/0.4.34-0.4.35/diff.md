# Comparing `tmp/climatePy-0.4.34.tar.gz` & `tmp/climatePy-0.4.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.34.tar", last modified: Mon Jul 17 22:39:15 2023, max compression
+gzip compressed data, was "climatePy-0.4.35.tar", last modified: Tue Jul 18 17:09:07 2023, max compression
```

## Comparing `climatePy-0.4.34.tar` & `climatePy-0.4.35.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.495348 climatePy-0.4.34/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-17 22:39:12.000000 climatePy-0.4.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-17 22:39:15.495348 climatePy-0.4.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-17 22:39:12.000000 climatePy-0.4.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.451347 climatePy-0.4.34/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22670 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    63216 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    32241 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.451347 climatePy-0.4.34/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-17 22:39:12.000000 climatePy-0.4.34/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.451347 climatePy-0.4.34/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 22:39:15.000000 climatePy-0.4.34/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:39:15.495348 climatePy-0.4.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-17 22:39:14.000000 climatePy-0.4.34/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:15.495348 climatePy-0.4.34/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:39:12.000000 climatePy-0.4.34/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-17 22:39:12.000000 climatePy-0.4.34/tests/test_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-17 22:39:12.000000 climatePy-0.4.34/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-17 22:39:12.000000 climatePy-0.4.34/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.926550 climatePy-0.4.35/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-18 17:09:04.000000 climatePy-0.4.35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-18 17:09:07.922550 climatePy-0.4.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-18 17:09:04.000000 climatePy-0.4.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.878549 climatePy-0.4.35/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22670 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63216 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32241 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.882550 climatePy-0.4.35/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.882550 climatePy-0.4.35/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:09:07.926550 climatePy-0.4.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-18 17:09:06.000000 climatePy-0.4.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.922550 climatePy-0.4.35/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:04.000000 climatePy-0.4.35/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-18 17:09:04.000000 climatePy-0.4.35/tests/test_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-18 17:09:04.000000 climatePy-0.4.35/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-18 17:09:04.000000 climatePy-0.4.35/tests/test_utils.py
```

### Comparing `climatePy-0.4.34/LICENSE` & `climatePy-0.4.35/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/PKG-INFO` & `climatePy-0.4.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.34
+Version: 0.4.35
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.34/README.md` & `climatePy-0.4.35/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/climatePy/__init__.py` & `climatePy-0.4.35/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/climatePy/_climatepy_filter.py` & `climatePy-0.4.35/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/climatePy/_dap.py` & `climatePy-0.4.35/climatePy/_dap.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/climatePy/_extract_sites.py` & `climatePy-0.4.35/climatePy/_extract_sites.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import re
 import numpy as np
 import xarray as xr
 import pandas as pd
 import geopandas as gpd
 
 def clean_time(df, col, inplace=False):
+    # regular expression to extract numbers between dashes (date strings)
+    regex_pat = r'(\d+)-'
 
-    regex = r".*?(\d{4}-\d{2}-\d{2}-\d{2}-\d{2}-\d{2})"
-
-    clean_time = [re.match(regex, value).group(1) for value in df[col]]
+    # find all regular expression matches
+    clean_time = ["-".join(re.findall(regex_pat, value)) for value in df[col]]
 
     def correct_date(input_string):
         match = re.match(r'(\d{4}-\d{2}-\d{2})-(.*)', input_string)
 
         if match:
             date_part = match.group(1)
             time_part = match.group(2)
@@ -25,31 +26,14 @@
             raise ValueError("Invalid input string format.")
     if inplace:
         df['date'] = [np.datetime64(correct_date(input_string)) for input_string in clean_time]
         return df
     else:
         return [np.datetime64(correct_date(input_string)) for input_string in clean_time]
     
-def clean_varname(df, col, inplace=False):
-
-    # regular expression
-    regex = r'^(.*?)\d{4}-\d{2}-\d{2}-\d{2}-\d{2}-\d{2}$'
-
-    # extract text BEFORE date
-    extracted_text = [re.match(regex, value).group(1) for value in df[col]]
-
-    # remove trailing underscores
-    extracted_text = [s.rstrip('_') for s in extracted_text]
-
-    if inplace:
-        df['varname'] = extracted_text
-        return df
-    else:
-        return extracted_text
-    
 def pts_extracter(r, pts, id=None):
     """
     Extracts data from an xarray DataArray at specific points based on a GeoDataFrame of points.
 
     Args:
         r (xarray.DataArray): The xarray DataArray object containing the data.
         pts (geopandas.GeoDataFrame): The GeoDataFrame containing the points of interest.
@@ -73,14 +57,17 @@
 
     if id is not None and id not in pts.columns:
         raise ValueError(f"id column '{id}' not found in pts GeoDataFrame.")
     
     if id is None:
         pts['uid'] = pts.index
         id = 'uid'
+    
+    # make a hashmap of names and index values
+    names_map = {i: v[0] for i, v in enumerate(zip(pts[id], pts.index))}
 
     # transform point to CRS of xarray
     pts = pts.to_crs(r['crs'].values.tolist()) 
     
     # get X and Y coordinates of points as data arrays
     target_x = xr.DataArray(pts.geometry.x, dims=id)
     target_y = xr.DataArray(pts.geometry.y, dims=id)
@@ -91,26 +78,34 @@
     
     # # preserve original data variable name
     varname = r.name
 
     # select columns of interest
     pts_df = pts_df[['time', varname, id]]
     
+    # replace the dataframe index with the hashmap values
+    pts_df[id] = pts_df[id].map(names_map)
+
     # pivot data wide
     pts_df = pts_df.pivot(index='time', columns=id, values=varname)
 
     # reset index
     pts_df = pts_df.reset_index()
-
-    # extract varname from time column
-    pts_df['varname'] = clean_varname(pts_df, "time", inplace=False)
-    # pts_df['varname'] = varname
+    
+    # # extract varname from time column
+    # pts_df['varname'] = clean_varname(pts_df, "time", inplace=False)
+    # # pts_df['varname'] = varname
 
     # convert time column to datetime
-    pts_df['time'] = clean_time(pts_df, "time")
+    pts_df['time'] = clean_time(df = pts_df, col = "time", inplace=False)
+    # pts_df['time'] = clean_time(pts_df, "time")
+
+    # extract varname from time column
+    pts_df['varname'] = varname
+    # pts_df['varname'] = clean_varname(pts_df, "time", inplace=False)
 
     # rename "time" column to "date"
     pts_df.rename(columns={'time': 'date'}, inplace=True)
 
     # reorder columns putting date and varname first
     pts_df = pts_df[['date', 'varname'] + [x for x in pts_df.columns if x not in ['date', 'varname']]]
 
@@ -144,14 +139,57 @@
 
         res = []
 
         for key, value in r.items():
             # print(f"key: {key}")
             # print(f"EXTRACTING POINTS FOR VARIABLE: {key}")
 
-            res.append(pts_extracter(r=value, pts=pts, id=None))
+            res.append(pts_extracter(r=value, pts=pts, id=id))
 
             # print(f'---------')
 
         res = pd.concat(res, ignore_index=True)
 
-    return res
+    return res
+
+# def clean_time(df, col, inplace=False):
+
+#     regex = r".*?(\d{4}-\d{2}-\d{2}-\d{2}-\d{2}-\d{2})"
+
+#     clean_time = [re.match(regex, value).group(1) for value in df[col]]
+
+#     def correct_date(input_string):
+#         match = re.match(r'(\d{4}-\d{2}-\d{2})-(.*)', input_string)
+
+#         if match:
+#             date_part = match.group(1)
+#             time_part = match.group(2)
+
+#             formatted_time = re.sub(r'[^a-zA-Z0-9]', ':', time_part)
+
+#             return date_part + 'T' + formatted_time
+
+#         else:
+#             raise ValueError("Invalid input string format.")
+#     if inplace:
+#         df['date'] = [np.datetime64(correct_date(input_string)) for input_string in clean_time]
+#         return df
+#     else:
+#         return [np.datetime64(correct_date(input_string)) for input_string in clean_time]
+    
+# def clean_varname(df, col, inplace=False):
+
+#     # regular expression
+#     regex = r'^(.*?)\d{4}-\d{2}-\d{2}-\d{2}-\d{2}-\d{2}$'
+
+#     # extract text BEFORE date
+#     extracted_text = [re.match(regex, value).group(1) for value in df[col]]
+
+#     # remove trailing underscores
+#     extracted_text = [s.rstrip('_') for s in extracted_text]
+
+#     if inplace:
+#         df['varname'] = extracted_text
+#         return df
+#     else:
+#         return extracted_text
+
```

### Comparing `climatePy-0.4.34/climatePy/_netrc_utils.py` & `climatePy-0.4.35/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/climatePy/_shortcuts.py` & `climatePy-0.4.35/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/climatePy/_utils.py` & `climatePy-0.4.35/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/climatePy/data/catalog.csv` & `climatePy-0.4.35/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.35/climatePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.34
+Version: 0.4.35
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.34/setup.py` & `climatePy-0.4.35/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.34',
+    version='0.4.35',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.34/tests/test_extract_sites.py` & `climatePy-0.4.35/tests/test_extract_sites.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/tests/test_shortcuts.py` & `climatePy-0.4.35/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.34/tests/test_utils.py` & `climatePy-0.4.35/tests/test_utils.py`

 * *Files identical despite different names*

