# Comparing `tmp/ign-pdal-tools-1.0.0.tar.gz` & `tmp/ign-pdal-tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-pdal-tools-1.0.0.tar", last modified: Wed Jun 28 14:19:10 2023, max compression
+gzip compressed data, was "ign-pdal-tools-1.1.0.tar", last modified: Tue Jul 18 06:54:23 2023, max compression
```

## Comparing `ign-pdal-tools-1.0.0.tar` & `ign-pdal-tools-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:19:10.428796 ign-pdal-tools-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-28 14:19:10.428796 ign-pdal-tools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:19:10.424796 ign-pdal-tools-1.0.0/ign_pdal_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-28 14:19:10.000000 ign-pdal-tools-1.0.0/ign_pdal_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-28 14:19:10.000000 ign-pdal-tools-1.0.0/ign_pdal_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 14:19:10.000000 ign-pdal-tools-1.0.0/ign_pdal_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-28 14:19:10.000000 ign-pdal-tools-1.0.0/ign_pdal_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:19:10.428796 ign-pdal-tools-1.0.0/pdaltools/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/pdaltools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/pdaltools/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/pdaltools/las_add_buffer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1193 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/pdaltools/las_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/pdaltools/las_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/pdaltools/las_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/pdaltools/replace_attribute_in_las.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/pdaltools/standardize_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 14:19:10.428796 ign-pdal-tools-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 14:19:10.428796 ign-pdal-tools-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/test/test_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/test/test_las_add_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/test/test_las_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/test/test_las_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/test/test_las_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/test/test_replace_attribute_in_las.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-28 14:18:42.000000 ign-pdal-tools-1.0.0/test/test_standardize_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:23.092310 ign-pdal-tools-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-18 06:54:23.092310 ign-pdal-tools-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:23.088310 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-18 06:54:23.000000 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-18 06:54:23.000000 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:54:23.000000 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 06:54:23.000000 ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:23.088310 ign-pdal-tools-1.1.0/pdaltools/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/las_add_buffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1193 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/las_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/las_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/las_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/replace_attribute_in_las.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/standardize_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pdaltools/unlock_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:54:23.092310 ign-pdal-tools-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:23.092310 ign-pdal-tools-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_las_add_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_las_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_las_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_las_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_replace_attribute_in_las.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_standardize_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-18 06:48:56.000000 ign-pdal-tools-1.1.0/test/test_unlock.py
```

### Comparing `ign-pdal-tools-1.0.0/LICENSE.md` & `ign-pdal-tools-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/PKG-INFO` & `ign-pdal-tools-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-pdal-tools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library for common LAS files manipulation with PDAL
 Author-email: Guillaume Liegard <guillaume.liegard@ign.fr>
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ign-pdal-tools
 
@@ -20,14 +20,15 @@
 # Content
 
 This library contains pdal-based tools to:
 * **colorize** a point cloud using images from [Geoportail](https://www.geoportail.gouv.fr/) (a portal
 from French government providing access to aerial imagery)
 * **stitch** together LAS files using their location
 * **standardize** LAS files
+* **unlock** LAS files generated by TerraSolid
 
 # Installation / Usage
 
 This library can be used in different ways:
 * installed with `pip` from pypi: ` pip install ign-pdal-tools`
 * used in a docker container: see documentation [Dockerfile](Dockerfile)
 
@@ -51,14 +52,20 @@
 
 * [standardize_format.py](pdaltools/standardize_format.py): re-write a LAS file in a standard format (see code for details)
 * [count_occurences](pdaltools/count_occurences): count occurences for each value of a given attribute in a set of LAS files (initially used for classification)
     * [count_occurences_for_attribute.py](pdaltools/count_occurences/count_occurences_for_attribute.py): count occurences in one or several files and save the result in a json file.
     * [merge_occurences_counts.py](pdaltools/count_occurences/merge_occurences_counts.py): merge counts from several results of [count_occurences_for_attribute](pdaltools/count_occurences/count_occurences_for_attribute.py) (json files) into a single json file (used for parallelization)
 * [replace_attribute_in_las.py](test/test_replace_attribute_in_las.py): using a json file containing a correspondance map, replace the occurences of each value in a LAS file by its corresponding value from the map.
 
+## Unlock
+
+[unlock_file.py](pdaltools/unlock_file.py): overwrite a LAS file in case PDAL raises this error:
+`readers.las: Global encoding WKT flag not set for point format 6 - 10.` which is due to TerraSolid
+malformed LAS output for LAS1.4 files with point format 6 to 10.
+
 # Dev / Build
 
 ## Contribute
 
 Every time the code is changed, think of updating the version file: [pdaltools/_version.py](pdaltools/_version.py`)
 
 Please log your changes in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `ign-pdal-tools-1.0.0/README.md` & `ign-pdal-tools-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Content
 
 This library contains pdal-based tools to:
 * **colorize** a point cloud using images from [Geoportail](https://www.geoportail.gouv.fr/) (a portal
 from French government providing access to aerial imagery)
 * **stitch** together LAS files using their location
 * **standardize** LAS files
+* **unlock** LAS files generated by TerraSolid
 
 # Installation / Usage
 
 This library can be used in different ways:
 * installed with `pip` from pypi: ` pip install ign-pdal-tools`
 * used in a docker container: see documentation [Dockerfile](Dockerfile)
 
@@ -43,14 +44,20 @@
 
 * [standardize_format.py](pdaltools/standardize_format.py): re-write a LAS file in a standard format (see code for details)
 * [count_occurences](pdaltools/count_occurences): count occurences for each value of a given attribute in a set of LAS files (initially used for classification)
     * [count_occurences_for_attribute.py](pdaltools/count_occurences/count_occurences_for_attribute.py): count occurences in one or several files and save the result in a json file.
     * [merge_occurences_counts.py](pdaltools/count_occurences/merge_occurences_counts.py): merge counts from several results of [count_occurences_for_attribute](pdaltools/count_occurences/count_occurences_for_attribute.py) (json files) into a single json file (used for parallelization)
 * [replace_attribute_in_las.py](test/test_replace_attribute_in_las.py): using a json file containing a correspondance map, replace the occurences of each value in a LAS file by its corresponding value from the map.
 
+## Unlock
+
+[unlock_file.py](pdaltools/unlock_file.py): overwrite a LAS file in case PDAL raises this error:
+`readers.las: Global encoding WKT flag not set for point format 6 - 10.` which is due to TerraSolid
+malformed LAS output for LAS1.4 files with point format 6 to 10.
+
 # Dev / Build
 
 ## Contribute
 
 Every time the code is changed, think of updating the version file: [pdaltools/_version.py](pdaltools/_version.py`)
 
 Please log your changes in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `ign-pdal-tools-1.0.0/ign_pdal_tools.egg-info/PKG-INFO` & `ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-pdal-tools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library for common LAS files manipulation with PDAL
 Author-email: Guillaume Liegard <guillaume.liegard@ign.fr>
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ign-pdal-tools
 
@@ -20,14 +20,15 @@
 # Content
 
 This library contains pdal-based tools to:
 * **colorize** a point cloud using images from [Geoportail](https://www.geoportail.gouv.fr/) (a portal
 from French government providing access to aerial imagery)
 * **stitch** together LAS files using their location
 * **standardize** LAS files
+* **unlock** LAS files generated by TerraSolid
 
 # Installation / Usage
 
 This library can be used in different ways:
 * installed with `pip` from pypi: ` pip install ign-pdal-tools`
 * used in a docker container: see documentation [Dockerfile](Dockerfile)
 
@@ -51,14 +52,20 @@
 
 * [standardize_format.py](pdaltools/standardize_format.py): re-write a LAS file in a standard format (see code for details)
 * [count_occurences](pdaltools/count_occurences): count occurences for each value of a given attribute in a set of LAS files (initially used for classification)
     * [count_occurences_for_attribute.py](pdaltools/count_occurences/count_occurences_for_attribute.py): count occurences in one or several files and save the result in a json file.
     * [merge_occurences_counts.py](pdaltools/count_occurences/merge_occurences_counts.py): merge counts from several results of [count_occurences_for_attribute](pdaltools/count_occurences/count_occurences_for_attribute.py) (json files) into a single json file (used for parallelization)
 * [replace_attribute_in_las.py](test/test_replace_attribute_in_las.py): using a json file containing a correspondance map, replace the occurences of each value in a LAS file by its corresponding value from the map.
 
+## Unlock
+
+[unlock_file.py](pdaltools/unlock_file.py): overwrite a LAS file in case PDAL raises this error:
+`readers.las: Global encoding WKT flag not set for point format 6 - 10.` which is due to TerraSolid
+malformed LAS output for LAS1.4 files with point format 6 to 10.
+
 # Dev / Build
 
 ## Contribute
 
 Every time the code is changed, think of updating the version file: [pdaltools/_version.py](pdaltools/_version.py`)
 
 Please log your changes in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `ign-pdal-tools-1.0.0/ign_pdal_tools.egg-info/SOURCES.txt` & `ign-pdal-tools-1.1.0/ign_pdal_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 pdaltools/color.py
 pdaltools/las_add_buffer.py
 pdaltools/las_clip.py
 pdaltools/las_info.py
 pdaltools/las_merge.py
 pdaltools/replace_attribute_in_las.py
 pdaltools/standardize_format.py
+pdaltools/unlock_file.py
 test/test_color.py
 test/test_las_add_buffer.py
 test/test_las_clip.py
 test/test_las_info.py
 test/test_las_merge.py
 test/test_replace_attribute_in_las.py
-test/test_standardize_format.py
+test/test_standardize_format.py
+test/test_unlock.py
```

### Comparing `ign-pdal-tools-1.0.0/pdaltools/color.py` & `ign-pdal-tools-1.1.0/pdaltools/color.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
-import os
-import shutil
 import subprocess as sp
 import tempfile
 import pdal
 import requests
 from osgeo.osr import SpatialReference
 import time
 import argparse
 
+from pdaltools.unlock_file import copy_and_hack_decorator
+
 
 def pretty_time_delta(seconds):
     sign_string = '-' if seconds < 0 else ''
     seconds = abs(int(seconds))
     days, seconds = divmod(seconds, 86400)
     hours, seconds = divmod(seconds, 3600)
     minutes, seconds = divmod(seconds, 60)
@@ -93,34 +93,14 @@
     if authority == "EPSG":
         proj = osr_crs.GetAttrValue("AUTHORITY", 1)
     else:
         proj = "2154"  # par defaut
     return proj
 
 
-def copy_and_hack_decorator(func):
-    def newfn(*args, **kwargs):
-        attempt = 0
-        try:
-            return func(*args, **kwargs)
-        except RuntimeError as e:
-            if (
-                "PDAL: readers.las: Global encoding WKT flag not set for point format 6 - 10."
-                in str(e)
-            ):
-                args = list(args)
-                input_file_tmp = copy_and_hack_the_laz_file(args[0])
-                args[0] = input_file_tmp
-                func(*args, **kwargs)
-                os.remove(input_file_tmp)
-            else:
-                raise e
-    return newfn
-
-
 def pdal_info_json(input_file: str):
     r = sp.run(["pdal", "info", "--metadata", input_file], stderr=sp.PIPE, stdout=sp.PIPE)
     if r.returncode == 1:
         msg = r.stderr.decode()
         print(msg)
         raise RuntimeError(msg)
 
@@ -131,15 +111,15 @@
     except:
         print(r.stderr.decode())
         raise
     return json_info
 
 
 @copy_and_hack_decorator
-def decomp_and_color(input_file: str, output_file :str,
+def color(input_file: str, output_file :str,
     proj="", pixel_per_meter=5, timeout_second=300,
     color_rvb_enabled=True, color_ir_enabled=True, veget_index_file=""
     ):
 
     json_info = pdal_info_json(input_file)
     metadata = json_info["metadata"]
     minx, maxx, miny, maxy = metadata["minx"], metadata["maxx"], metadata["miny"], metadata["maxy"]
@@ -174,38 +154,14 @@
     print("Traitement du nuage de point")
     pipeline.execute()
 
     # os.remove(tmp_ortho)
     # os.remove(tmp_ortho_irc)
 
 
-# https://gis.stackexchange.com/questions/413191/python-pdal-error-reading-format-1-4-las-file-readers-las-error-global-enco
-def unlock_file(finename: str):
-    f = open(finename, "rb+")
-    f.seek(6)
-    f.write(bytes([17, 0, 0, 0]))
-    f.close()
-
-
-def copy_and_hack_the_laz_file(laz_file):
-    with tempfile.NamedTemporaryFile() as tmp:
-        laz_file_tmp = tmp.name + ".laz"
-
-        print(
-            "Gestion de l'erreur en créeant un nouveau LAZ que l'on modifiera : "
-            + laz_file_tmp
-        )
-        shutil.copy(laz_file, laz_file_tmp)
-
-        unlock_file(laz_file_tmp)
-
-        print("Patch appliqué sur : " + laz_file_tmp)
-        return laz_file_tmp
-
-
 def parse_args():
     parser = argparse.ArgumentParser("Colorize tool")
     parser.add_argument(
         "--input", "-i",
         type=str,
         required=True,
         help="Input file")
@@ -227,24 +183,18 @@
     parser.add_argument(
         "--timeout", "-t",
         type=int,
         default = 300,
         help="Timeout, in seconds")
     parser.add_argument('--rvb', action='store_true', help="Colorize RVB")
     parser.add_argument('--ir', action='store_true', help="Colorize IR")
-    parser.add_argument('--unlock', action='store_true', help="Unlock")
     parser.add_argument(
         "--vegetation",
         type=str,
         default = "",
         help="Vegetation file, value will be stored in Deviation field")
     return  parser.parse_args()
 
 
 if __name__ == "__main__":
     args = parse_args()
-
-    if args.unlock:
-        unlock_file(args.input)
-    else:
-        decomp_and_color(args.input, args.output, args.proj, args.resolution, args.timeout, args.rvb, args.ir, args.vegetation)
-
+    color(args.input, args.output, args.proj, args.resolution, args.timeout, args.rvb, args.ir, args.vegetation)
```

### Comparing `ign-pdal-tools-1.0.0/pdaltools/las_add_buffer.py` & `ign-pdal-tools-1.1.0/pdaltools/las_add_buffer.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/pdaltools/las_clip.py` & `ign-pdal-tools-1.1.0/pdaltools/las_clip.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/pdaltools/las_info.py` & `ign-pdal-tools-1.1.0/pdaltools/las_info.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/pdaltools/las_merge.py` & `ign-pdal-tools-1.1.0/pdaltools/las_merge.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/pdaltools/replace_attribute_in_las.py` & `ign-pdal-tools-1.1.0/pdaltools/replace_attribute_in_las.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/pdaltools/standardize_format.py` & `ign-pdal-tools-1.1.0/pdaltools/standardize_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 import argparse
 import os
 import pdal
 import subprocess as sp
 import tempfile
 from typing import Dict
+from pdaltools.unlock_file import copy_and_hack_decorator
 
 STANDARD_PARAMETERS = dict(
     major_version="1",
     minor_version="4",  # Laz format version (pdal always write in 1.x format)
     global_encoding=17,  # store WKT projection in file
     compression="true",  # Save to compressed laz format
     extra_dims= [],  # Save no extra_dims
@@ -77,14 +78,15 @@
         raise RuntimeError(msg)
 
     output = r.stdout.decode()
     for line in output.splitlines():
         print(line)
 
 
+@copy_and_hack_decorator
 def standardize(input_file: str, output_file: str, params_from_parser: Dict) -> None:
     _, extension = os.path.splitext(output_file)
     with tempfile.NamedTemporaryFile(suffix=extension) as tmp:
         tmp.close()
         rewrite_with_pdal(input_file, tmp.name, params_from_parser)
         exec_las2las(tmp.name, output_file)
```

### Comparing `ign-pdal-tools-1.0.0/test/test_color.py` & `ign-pdal-tools-1.1.0/test/test_color.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import shutil
 import pytest
-import laspy
 
 from pdaltools import color
 
 import requests
 import requests_mock
 
 cwd = os.getcwd()
@@ -23,15 +22,15 @@
 INPUT_PATH = os.path.join(TEST_PATH, 'data/test_noepsg_043500_629205_IGN69.laz')
 
 OUTPUT_FILE = TMPDIR + "Semis_2021_0435_6292_LA93_IGN69.las"
 
 
 def test_epsg_fail():
     with pytest.raises(requests.exceptions.HTTPError, match="400 Client Error: BadRequest for url") :
-        color.decomp_and_color(INPUT_PATH, OUTPUT_FILE, "", 0.1, 15)
+        color.color(INPUT_PATH, OUTPUT_FILE, "", 0.1, 15)
 
 
 epsg = "2154"
 layer= "ORTHOIMAGERY.ORTHOPHOTOS"
 minx=435000
 miny=6291000
 maxx=436000
@@ -83,23 +82,7 @@
     def raise_server_error():
         raise requests.exceptions.HTTPError("Server Error")
 
     with pytest.raises(requests.exceptions.HTTPError):
         raise_server_error()
 
 
-def test_copy_and_hack_decorator():
-    # bug during laz opening in pdal (solved with copy_and_hack_decorator)
-    LAZ_FILE = os.path.join(TEST_PATH, 'data/test_pdalfail_0643_6319_LA93_IGN69.laz')
-    LAS_FILE = TMPDIR + "test_pdalfail_0643_6319_LA93_IGN69.las"
-
-    color.decomp_and_color(LAZ_FILE, LAS_FILE, "", 1)
-
-    las = laspy.read(LAS_FILE)
-    print(las.header)
-    print(list(las.point_format.dimension_names))
-    print(las.red)
-    print(las.green)
-    print(las.blue)
-    print(las.nir)
-
-    assert os.path.isfile(LAS_FILE)
```

### Comparing `ign-pdal-tools-1.0.0/test/test_las_add_buffer.py` & `ign-pdal-tools-1.1.0/test/test_las_add_buffer.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/test/test_las_clip.py` & `ign-pdal-tools-1.1.0/test/test_las_clip.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/test/test_las_info.py` & `ign-pdal-tools-1.1.0/test/test_las_info.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/test/test_las_merge.py` & `ign-pdal-tools-1.1.0/test/test_las_merge.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/test/test_replace_attribute_in_las.py` & `ign-pdal-tools-1.1.0/test/test_replace_attribute_in_las.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-1.0.0/test/test_standardize_format.py` & `ign-pdal-tools-1.1.0/test/test_standardize_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,10 +106,17 @@
     # if you want to see input_file warnings
     # assert_lasinfo_no_warning(input_file)
 
     standardize(input_file, output_file, multiple_params[0])
     assert_lasinfo_no_warning(output_file)
 
 
+def test_standardize_malformed_laz():
+    input_file = os.path.join(test_path, 'data/test_pdalfail_0643_6319_LA93_IGN69.laz')
+    output_file = os.path.join(tmp_path, 'standardize_pdalfail_0643_6319_LA93_IGN69.laz')
+    standardize(input_file, output_file, multiple_params[0])
+    assert os.path.isfile(output_file)
+
+
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     test_standardize_format()
```

