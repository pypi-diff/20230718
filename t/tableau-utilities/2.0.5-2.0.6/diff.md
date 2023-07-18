# Comparing `tmp/tableau_utilities-2.0.5.tar.gz` & `tmp/tableau_utilities-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau_utilities-2.0.5.tar", last modified: Mon Jul 10 18:52:32 2023, max compression
+gzip compressed data, was "tableau_utilities-2.0.6.tar", last modified: Tue Jul 18 16:26:50 2023, max compression
```

## Comparing `tableau_utilities-2.0.5.tar` & `tableau_utilities-2.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.142441 tableau_utilities-2.0.5/
--rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.5/LICENSE
--rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-10 18:52:32.141781 tableau_utilities-2.0.5/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/README.md
--rw-r--r--   0 justin     (502) staff       (20)       38 2023-07-10 18:52:32.142865 tableau_utilities-2.0.5/setup.cfg
--rw-r--r--   0 justin     (502) staff       (20)     1107 2023-07-10 18:51:08.000000 tableau_utilities-2.0.5/setup.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.123024 tableau_utilities-2.0.5/tableau_utilities/
--rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/fetch_all_cols.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.129172 tableau_utilities-2.0.5/tableau_utilities/general/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/general/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/general/cli_styling.py
--rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/general/config_column_persona.py
--rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/general/funcs.py
--rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripted_testing.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.135174 tableau_utilities-2.0.5/tableau_utilities/scripts/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/cli.py
--rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/csv_config.py
--rw-r--r--   0 justin     (502) staff       (20)     7647 2023-07-10 18:51:08.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/datasource.py
--rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/gen_config.py
--rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/merge_config.py
--rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/server_info.py
--rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/scripts/server_operate.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.137055 tableau_utilities-2.0.5/tableau_utilities/tableau_file/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_file/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    11705 2023-07-10 18:51:08.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_file/tableau_file.py
--rw-r--r--   0 justin     (502) staff       (20)    37816 2023-07-10 18:51:08.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_file/tableau_file_objects.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.140457 tableau_utilities-2.0.5/tableau_utilities/tableau_server/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_server/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_server/tableau_server.py
--rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.5/tableau_utilities/tableau_server/tableau_server_objects.py
--rw-r--r--   0 justin     (502) staff       (20)    10765 2023-07-10 18:39:33.000000 tableau_utilities-2.0.5/tableau_utilities/test_tableau_utilities.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-10 18:52:32.126708 tableau_utilities-2.0.5/tableau_utilities.egg-info/
--rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     1205 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (502) staff       (20)        1 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (502) staff       (20)       73 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/entry_points.txt
--rw-r--r--   0 justin     (502) staff       (20)      112 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/requires.txt
--rw-r--r--   0 justin     (502) staff       (20)       18 2023-07-10 18:52:32.000000 tableau_utilities-2.0.5/tableau_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 16:26:50.212204 tableau_utilities-2.0.6/
+-rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.6/LICENSE
+-rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-18 16:26:50.211884 tableau_utilities-2.0.6/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/README.md
+-rw-r--r--   0 justin     (502) staff       (20)       38 2023-07-18 16:26:50.212316 tableau_utilities-2.0.6/setup.cfg
+-rw-r--r--   0 justin     (502) staff       (20)     1107 2023-07-18 16:25:27.000000 tableau_utilities-2.0.6/setup.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 16:26:50.194186 tableau_utilities-2.0.6/tableau_utilities/
+-rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/fetch_all_cols.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 16:26:50.201206 tableau_utilities-2.0.6/tableau_utilities/general/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/general/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/general/cli_styling.py
+-rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/general/config_column_persona.py
+-rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/general/funcs.py
+-rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/scripted_testing.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 16:26:50.207040 tableau_utilities-2.0.6/tableau_utilities/scripts/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/scripts/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/scripts/cli.py
+-rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/scripts/csv_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     7901 2023-07-18 16:25:27.000000 tableau_utilities-2.0.6/tableau_utilities/scripts/datasource.py
+-rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/scripts/gen_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/scripts/merge_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/scripts/server_info.py
+-rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/scripts/server_operate.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 16:26:50.208556 tableau_utilities-2.0.6/tableau_utilities/tableau_file/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/tableau_file/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    12393 2023-07-18 16:25:27.000000 tableau_utilities-2.0.6/tableau_utilities/tableau_file/tableau_file.py
+-rw-r--r--   0 justin     (502) staff       (20)    37816 2023-07-10 18:51:08.000000 tableau_utilities-2.0.6/tableau_utilities/tableau_file/tableau_file_objects.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 16:26:50.211091 tableau_utilities-2.0.6/tableau_utilities/tableau_server/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/tableau_server/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/tableau_server/tableau_server.py
+-rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.6/tableau_utilities/tableau_server/tableau_server_objects.py
+-rw-r--r--   0 justin     (502) staff       (20)    10765 2023-07-10 18:39:33.000000 tableau_utilities-2.0.6/tableau_utilities/test_tableau_utilities.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 16:26:50.198714 tableau_utilities-2.0.6/tableau_utilities.egg-info/
+-rw-r--r--   0 justin     (502) staff       (20)     8420 2023-07-18 16:26:50.000000 tableau_utilities-2.0.6/tableau_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     1205 2023-07-18 16:26:50.000000 tableau_utilities-2.0.6/tableau_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (502) staff       (20)        1 2023-07-18 16:26:50.000000 tableau_utilities-2.0.6/tableau_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (502) staff       (20)       73 2023-07-18 16:26:50.000000 tableau_utilities-2.0.6/tableau_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 justin     (502) staff       (20)      112 2023-07-18 16:26:50.000000 tableau_utilities-2.0.6/tableau_utilities.egg-info/requires.txt
+-rw-r--r--   0 justin     (502) staff       (20)       18 2023-07-18 16:26:50.000000 tableau_utilities-2.0.6/tableau_utilities.egg-info/top_level.txt
```

### Comparing `tableau_utilities-2.0.5/LICENSE` & `tableau_utilities-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/PKG-INFO` & `tableau_utilities-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau_utilities
-Version: 2.0.5
+Version: 2.0.6
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.5/README.md` & `tableau_utilities-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/setup.py` & `tableau_utilities-2.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     author_email="justin.grilli@gmail.com",
     license='MIT',
     url='http://pypi.python.org/pypi/tableau-utilities/',
     description='Utility for maintaining Tableau objects',
     long_description=readme,
     long_description_content_type='text/markdown',
     name="tableau_utilities",
-    version="2.0.5",
+    version="2.0.6",
     packages=[
         'tableau_utilities',
         'tableau_utilities.general',
         'tableau_utilities.tableau_file',
         'tableau_utilities.tableau_server',
         'tableau_utilities.scripts'
     ],
```

### Comparing `tableau_utilities-2.0.5/tableau_utilities/fetch_all_cols.py` & `tableau_utilities-2.0.6/tableau_utilities/fetch_all_cols.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/general/cli_styling.py` & `tableau_utilities-2.0.6/tableau_utilities/general/cli_styling.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/general/config_column_persona.py` & `tableau_utilities-2.0.6/tableau_utilities/general/config_column_persona.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/general/funcs.py` & `tableau_utilities-2.0.6/tableau_utilities/general/funcs.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/scripted_testing.py` & `tableau_utilities-2.0.6/tableau_utilities/scripted_testing.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/scripts/cli.py` & `tableau_utilities-2.0.6/tableau_utilities/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/scripts/csv_config.py` & `tableau_utilities-2.0.6/tableau_utilities/scripts/csv_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/scripts/datasource.py` & `tableau_utilities-2.0.6/tableau_utilities/scripts/datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,22 +54,24 @@
 
     # Print Styling
     color = Color()
     symbol = Symbol()
 
     # Downloads the datasource from Tableau Server if the datasource is not local
     if location == 'online':
+        print(f'{color.fg_cyan}...Downloading {datasource_name}...{color.reset}')
         d = server.get_datasource(datasource_id, datasource_name, project_name)
         datasource_path = server.download_datasource(d.id, include_extract=include_extract)
         print(f'{color.fg_green}{symbol.success}  Downloaded Datasource:', f'{color.fg_yellow}{datasource_path}{color.reset}', '\n')
 
     datasource_file_name = os.path.basename(datasource_path)
     ds = Datasource(datasource_path)
 
     if save_tds:
+        print(f'{color.fg_cyan}...Extracting {datasource_file_name}...{color.reset}')
         save_folder = f'{datasource_file_name} - BEFORE'
         os.makedirs(save_folder, exist_ok=True)
         if ds.extension == 'tds':
             xml_path = os.path.join(save_folder, datasource_file_name)
             shutil.copy(datasource_path, xml_path)
         else:
             xml_path = ds.unzip(extract_to=save_folder, unzip_all=True)
@@ -162,14 +164,15 @@
 
     # Save the datasource if an edit may have happened
     if column_name or folder_name or delete or enforce_connection:
         ds.save()
         print(f'{color.fg_green}{symbol.success}  Saved changes to: {color.fg_yellow}{datasource_path}{color.reset}')
 
     if save_tds:
+        print(f'{color.fg_cyan}...Extracting {datasource_file_name}...{color.reset}')
         save_folder = f'{datasource_file_name} - AFTER'
         os.makedirs(save_folder, exist_ok=True)
         if ds.extension == 'tds':
             xml_path = os.path.join(save_folder, datasource_file_name)
             shutil.copy(datasource_path, xml_path)
         else:
             xml_path = ds.unzip(extract_to=save_folder, unzip_all=True)
```

### Comparing `tableau_utilities-2.0.5/tableau_utilities/scripts/gen_config.py` & `tableau_utilities-2.0.6/tableau_utilities/scripts/gen_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/scripts/merge_config.py` & `tableau_utilities-2.0.6/tableau_utilities/scripts/merge_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/scripts/server_info.py` & `tableau_utilities-2.0.6/tableau_utilities/scripts/server_info.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/scripts/server_operate.py` & `tableau_utilities-2.0.6/tableau_utilities/scripts/server_operate.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/tableau_file/tableau_file.py` & `tableau_utilities-2.0.6/tableau_utilities/tableau_file/tableau_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import xml.etree.ElementTree as ET
 import os
+import shutil
 
 import xmltodict
 from zipfile import ZipFile
 
 import tableau_utilities.tableau_file.tableau_file_objects as tfo
 from tableau_utilities.general.funcs import transform_tableau_object
 
@@ -81,29 +82,42 @@
                 elif not unzip_all and ext in ['tds', 'twb']:
                     zip_file.extract(member=z, path=file_dir)
                     tableau_file_path = os.path.join(file_dir, z.filename)
         return tableau_file_path
 
     def save(self):
         """ Save/Update the Tableau file with the XML changes made """
-
         if self.extension in ['tdsx', 'twbx']:
             # Rebuild the TDSX / TWBX archive file, with the updated archived TDS / TWB
-            directory = os.path.dirname(self.file_path)
-            file_name = os.path.basename(self.file_path)
-            temp_path = os.path.join(directory, f'__temp_{file_name}')
-            with ZipFile(self.file_path, 'r') as zr, ZipFile(temp_path, 'w') as zw:
-                for file in zr.filelist:
-                    if file.filename.split('.')[-1] in ['tds', 'twb']:
-                        self._tree.write(zw.open(file.filename, 'w'),
-                                         encoding="utf-8", xml_declaration=True)
-                    else:
-                        zw.writestr(file, zr.read(file.filename))
-            os.remove(self.file_path)
-            os.rename(temp_path, self.file_path)
+            original_file = os.path.basename(self.file_path)
+            # Move the file into a temporary folder while updating
+            temp_folder = os.path.join(os.path.dirname(self.file_path),
+                                       f'__TEMP_{original_file.replace(".tdsx", "")}')
+            os.makedirs(temp_folder, exist_ok=False)
+            temp_path = os.path.join(temp_folder, original_file)
+            shutil.move(self.file_path, temp_path)
+            # Unzip the zipped files
+            extracted_files = list()
+            with ZipFile(temp_path) as z:
+                for f in z.filelist:
+                    ext = f.filename.split('.')[-1]
+                    path = z.extract(member=f, path=temp_folder)
+                    extracted_files.append(path)
+                    if ext in ['tds', 'twb']:
+                        xml_path = path
+            # Update XML file
+            self._tree.write(xml_path, encoding="utf-8", xml_declaration=True)
+            # Repack the unzipped file
+            with ZipFile(temp_path, 'w') as z:
+                for file in extracted_files:
+                    arcname = file.split(temp_folder)[-1]
+                    z.write(file, arcname=arcname)
+            # Move file back to the original folder and remove any unpacked contents
+            shutil.move(temp_path, self.file_path)
+            shutil.rmtree(temp_folder)
         else:
             # Update the Tableau file's contents
             self._tree.write(self.file_path, encoding="utf-8", xml_declaration=True)
 
 
 class Datasource(TableauFile):
     """
```

### Comparing `tableau_utilities-2.0.5/tableau_utilities/tableau_file/tableau_file_objects.py` & `tableau_utilities-2.0.6/tableau_utilities/tableau_file/tableau_file_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/tableau_server/tableau_server.py` & `tableau_utilities-2.0.6/tableau_utilities/tableau_server/tableau_server.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/tableau_server/tableau_server_objects.py` & `tableau_utilities-2.0.6/tableau_utilities/tableau_server/tableau_server_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities/test_tableau_utilities.py` & `tableau_utilities-2.0.6/tableau_utilities/test_tableau_utilities.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.5/tableau_utilities.egg-info/PKG-INFO` & `tableau_utilities-2.0.6/tableau_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau-utilities
-Version: 2.0.5
+Version: 2.0.6
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.5/tableau_utilities.egg-info/SOURCES.txt` & `tableau_utilities-2.0.6/tableau_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

