# Comparing `tmp/tab2neo-1.3.0.3.tar.gz` & `tmp/tab2neo-1.3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tab2neo-1.3.0.3.tar", last modified: Tue Jun  6 15:02:14 2023, max compression
+gzip compressed data, was "tab2neo-1.3.9.0.tar", last modified: Tue Jul 18 11:07:22 2023, max compression
```

## Comparing `tab2neo-1.3.0.3.tar` & `tab2neo-1.3.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.883385 tab2neo-1.3.0.3/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11357 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/LICENSE
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-06-06 15:02:14.879385 tab2neo-1.3.0.3/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     5418 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/README.md
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.863385 tab2neo-1.3.0.3/data_loaders/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      241 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3401 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/azure_data_loader.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    18843 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/file_data_loader.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1492 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/hive_data_loader.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1157 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/sql_server_data_loader.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.863385 tab2neo-1.3.0.3/data_providers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       54 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_providers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10972 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_providers/data_provider.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.867385 tab2neo-1.3.0.3/derivation_method/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      229 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)   104146 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/action.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    68853 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/derivation_method.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3784 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/method.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3223 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/predict_links.cql
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1043 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/predict_output_classes.cql
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    48787 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/super_method.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10250 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/utils.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.867385 tab2neo-1.3.0.3/logger/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/logger/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1217 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/logger/logger.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.871385 tab2neo-1.3.0.3/model_appliers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/model_appliers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    29312 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/model_appliers/model_applier.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.871385 tab2neo-1.3.0.3/model_managers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/model_managers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    55794 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/model_managers/model_manager.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      103 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/pyproject.toml
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.875385 tab2neo-1.3.0.3/query_builders/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/query_builders/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    40776 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/query_builders/query_builder.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2023-06-06 15:02:14.883385 tab2neo-1.3.0.3/setup.cfg
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2318 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/setup.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.879385 tab2neo-1.3.0.3/tab2neo.egg-info/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      933 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/SOURCES.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/dependency_links.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      544 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/requires.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       98 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/top_level.txt
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.879385 tab2neo-1.3.0.3/tests/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11269 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/tests/test_comparison_utilities.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.527385 tab2neo-1.3.9.0/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11357 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/LICENSE
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-07-18 11:07:22.527385 tab2neo-1.3.9.0/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     5418 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/README.md
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.503385 tab2neo-1.3.9.0/data_loaders/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      241 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/data_loaders/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3401 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/data_loaders/azure_data_loader.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    19450 2023-07-18 11:05:04.000000 tab2neo-1.3.9.0/data_loaders/file_data_loader.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1492 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/data_loaders/hive_data_loader.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1157 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/data_loaders/sql_server_data_loader.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.503385 tab2neo-1.3.9.0/data_providers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       54 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/data_providers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10972 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/data_providers/data_provider.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.507385 tab2neo-1.3.9.0/derivation_method/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      229 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/derivation_method/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)   104968 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/derivation_method/action.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    69122 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/derivation_method/derivation_method.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3784 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/derivation_method/method.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3223 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/derivation_method/predict_links.cql
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1043 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/derivation_method/predict_output_classes.cql
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    51508 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/derivation_method/super_method.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10250 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/derivation_method/utils.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.507385 tab2neo-1.3.9.0/logger/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/logger/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1217 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/logger/logger.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.507385 tab2neo-1.3.9.0/model_appliers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/model_appliers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    29312 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/model_appliers/model_applier.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.507385 tab2neo-1.3.9.0/model_managers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/model_managers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    66458 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/model_managers/model_manager.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      103 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/pyproject.toml
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.507385 tab2neo-1.3.9.0/query_builders/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/query_builders/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    40776 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/query_builders/query_builder.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2023-07-18 11:07:22.527385 tab2neo-1.3.9.0/setup.cfg
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2318 2023-07-18 11:05:04.000000 tab2neo-1.3.9.0/setup.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.527385 tab2neo-1.3.9.0/tab2neo.egg-info/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-07-18 11:07:22.000000 tab2neo-1.3.9.0/tab2neo.egg-info/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      933 2023-07-18 11:07:22.000000 tab2neo-1.3.9.0/tab2neo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2023-07-18 11:07:22.000000 tab2neo-1.3.9.0/tab2neo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      560 2023-07-18 11:07:22.000000 tab2neo-1.3.9.0/tab2neo.egg-info/requires.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       98 2023-07-18 11:07:22.000000 tab2neo-1.3.9.0/tab2neo.egg-info/top_level.txt
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-07-18 11:07:22.527385 tab2neo-1.3.9.0/tests/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11269 2023-07-18 10:30:56.000000 tab2neo-1.3.9.0/tests/test_comparison_utilities.py
```

### Comparing `tab2neo-1.3.0.3/LICENSE` & `tab2neo-1.3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/PKG-INFO` & `tab2neo-1.3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab2neo
-Version: 1.3.0.3
+Version: 1.3.9.0
 Summary: Clinical Linked Data: High-level Python classes to load, model and reshape tabular data imported into Neo4j database
 Home-page: UNKNOWN
 Author: Alexey Kuznetsov
 License:                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
```

### Comparing `tab2neo-1.3.0.3/README.md` & `tab2neo-1.3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/data_loaders/azure_data_loader.py` & `tab2neo-1.3.9.0/data_loaders/azure_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/data_loaders/file_data_loader.py` & `tab2neo-1.3.9.0/data_loaders/file_data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,19 @@
             # Todo: N.B CDISC Library provides csv files where values are quoted (i.e. "variabel 1","Another variable")
             #  Therefore option quotechar is used, which means that " will not appear in data.
             #  Have not tested or thought of scenarios what would happen if values are not quoted
             df = pd.read_csv(os.path.join(folder, filename), quotechar='"')
             meta = {'column_names': list(df.columns)}
             if metadataonly:
                 df = pd.DataFrame(columns = df.columns)
+        elif ext in ["parquet"]:
+            df = pd.read_parquet(os.path.join(folder, filename))
+            meta = {'column_names': list(df.columns)}
+            if metadataonly:
+                df = pd.DataFrame(columns = df.columns)
         else:
             raise Exception(f"Unsupported file format - unrecognized filename extension: {ext}")
 
         # EXAMPLE of a value for meta:
         #   {'column_names': ['STUDYID', 'SITEID', 'AGE']}
 
         if test_run:
@@ -113,15 +118,15 @@
         if query:
             df = df.query(query)
 
         return (df, meta)
 
 
     def load_file(self, folder:str, filename:str, sheet_name=0, query=None, metadataonly = False, dataonly = False, test_run = False,
-                        load_to_neo = True, colcharsbl =r'[^A-Za-z0-9_]+'):
+                        load_to_neo = True, colcharsbl =r'[^A-Za-z0-9_]+', extended_sdc:bool = False):
         """
         Read in an external file as a Pandas data frame.
 
         Can read in file types: rda, xpt, sas7bdat, xls, csv
         It can OPTIONALLY only retrieve the metadata from the source file.
         It OPTIONALLY loads into Neo4j the metadata (creating 3 node labels: `Source Data Folder`, `Source Data Table`, `Source Data Column`),
                 and, if imported, the data (creating nodes with the label `Source Data Row`,
@@ -147,14 +152,15 @@
         :param load_to_neo:     If True then data (INCL. metadata) is loaded into Neo4j nodes with `Source Data Row` labels
         :param colcharsbl:      The column names of the input files are renamed in such a way that the symbols
                                     specified by the regex pattern are excluded
                                     (e.g. for cleaning special characters in the colnames of excel files)
                                     EXAMPLE: r'[^A-Za-z0-9_]+' will only keep A-Z, a-z, 0-9 and the underscore
                                     TODO: Perhaps default it to None, and if not None, then apply it
                                           regardless of the file extension (currently, only applied to Excel files)
+        :param extended_sdc:    If True also creates `Source Data Column` nodes for _domain_, _filename_ and _folder_
 
         :return:                 A Pandas data frame.  EXAMPLE:
                                              STUDYID    SITEID    USUBJID  ...        TRTETM   BRTHDT      BRTHDTC
                                         0    mid987650  214356.0  987650.000001  ...  33420.0  1983-06-30  1983.0
                                         1    mid987650  214356.0  987650.000002  ...  33420.0  1956-06-30  1956.0
         """
         (df, meta) = self.read_file(folder=folder, filename=filename, sheet_name=sheet_name, query=query, metadataonly=metadataonly,
@@ -194,14 +200,16 @@
 
         # If the meta dictionary contains, as expected, the key 'column_names',
         #       and if the data (and metadata) is to be loaded into Neo4j,
         #       then handle the loading of the metadata
         if not dataonly:
             if 'column_names' in meta.keys() and load_to_neo:
                 self.load_file_metadata(folder, filename, meta['column_names'], domain)
+                if extended_sdc:
+                    self.load_file_metadata(folder, filename, ['_domain_', '_filename_', '_folder_'], domain)
 
         # Create the 'HAS_DATA' relationships between the 'Source Data Table' node and all the 'Source Data Row' nodes
         self.link_nodes_on_matching_property_value(label1='Source Data Table', label2='Source Data Row',
                                                 prop_name='_domain_', prop_value=domain,
                                                 rel='HAS_DATA')
         return df
 
@@ -240,34 +248,35 @@
         params = {'folder':folder, 'filename': filename, 'columns': columns, 'domain': domain}
         res = self.query(q, params)
         if self.verbose:
             logger.debug(f"        Query : {q}")
             logger.debug(f"        Query parameters: {params}")
 
 
-    def load_folder(self, folder="", only_files=None, metadataonly = False, test_run = False):
+    def load_folder(self, folder="", only_files=None, metadataonly = False, test_run = False, extended_sdc:bool = False):
         """
         Loop over all files in the folder, and load them as detailed in load_file()
 
         :param folder:
         :param only_files:
         :param metadataonly:
         :param test_run:
+        :param extended_sdc
         :return:
         """
         if not only_files:
             only_files = []
         self.load_df(df=pd.DataFrame([{'_folder_': folder}]), label="Source Data Folder", merge=True,
                      primary_key='_folder_')
         for filename in os.listdir(folder):
             # if only_files is empty list, then loads all files
             if (not only_files) or filename in only_files:
                 if self.verbose:
                     logger.info(f"Loading {filename}")
-                self.load_file(folder, filename, metadataonly = metadataonly, test_run = test_run)
+                self.load_file(folder, filename, metadataonly = metadataonly, test_run = test_run, extended_sdc=extended_sdc)
 
     def delete_source_data(self):
         """
         Deletes all (Non-reshaped) data
         :return:
         """
         q = """
```

### Comparing `tab2neo-1.3.0.3/data_loaders/hive_data_loader.py` & `tab2neo-1.3.9.0/data_loaders/hive_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/data_loaders/sql_server_data_loader.py` & `tab2neo-1.3.9.0/data_loaders/sql_server_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/data_providers/data_provider.py` & `tab2neo-1.3.9.0/data_providers/data_provider.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/derivation_method/action.py` & `tab2neo-1.3.9.0/derivation_method/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,28 +805,31 @@
         params = self.meta.get('params')
 
         if params:
             params = json.loads(params)
         else:
             params = {}
 
+        remove_col_prefixes = params.get('remove_col_prefixes', 'true')
+
         if self.meta.get('include_data') == 'true':
             if df is not None:
                 if df.empty:
                     logger.warning(f"RunCypher Action including data with empty df!")
                 params['data'] = df.to_dict(orient='records')
             else:
                 raise AttributeError('RunCypher Action unable to include data because self.df is None')
 
         res = self.method.interface.query(query, params, return_type='pd')
         params['action_node_id'] = self.action_node_id
 
         if self.meta.get('update_df') == 'true':
-            new_column_name_map = {col: col.split('.')[-1] for col in res.columns}
-            res.rename(columns=new_column_name_map, inplace=True)
+            if remove_col_prefixes == 'true':
+                new_column_name_map = {col: col.split('.')[-1] for col in res.columns}
+                res.rename(columns=new_column_name_map, inplace=True)
             self.df = res
             logger.debug(f"DataFrame: \n{res.to_string(max_rows=10)}")
 
         return res
 
     def retrieve_json(self):
         logger.info(f"Building json: {self.action_id}")
@@ -1507,15 +1510,15 @@
         if self.meta.get('use_uri'):
             it=None
             if self.meta.get('link_how')=='merge_on_uri': it='to'
             elif self.meta.get('link_how')=='merge_from_on_uri': it='from'
             if it is not None:    
                 if "_uri_"+self.meta.get(f'{it}_short_label') in list(self.df.columns):
                     uri_col = "_uri_"+self.meta.get(f'{it}_short_label')     
-                    if self.df[uri_col].squeeze().is_unique is False:
+                    if len(self.df[uri_col])>1 and self.df[uri_col].squeeze().is_unique is False:
                         logger.warning(f"More than 1 identical uri exists in column {uri_col}")     
 
         if "from_class" not in self.meta.keys():
             raise ValueError("from_class not found")
         if "to_class" not in self.meta.keys():
             raise ValueError("to_class not found")
         logger.info(f"\t{self}: `{self.meta.get('from_class')}` to `{self.meta.get('to_class')}`")
@@ -2017,14 +2020,15 @@
         WITH action, 
             apoc.coll.sortMaps(collect(DISTINCT uri_for), 'label') as uri_fors, 
             apoc.coll.sortMaps(collect(DISTINCT uri_by), 'label') as uri_bys,
             apoc.coll.sortMaps(collect(DISTINCT uri_label), 'label') as uri_labels
         RETURN 
            action{.*} as m,
            action.prefix as prefix,
+           action.store_on_existing_nodes as store_on_existing_nodes,
            [x in uri_fors | x.short_label] as uri_fors,
            [x in uri_fors | x.label] as uri_fors_long,
            [x in uri_bys | x.short_label] as uri_bys,
            [x in uri_bys | x.label] as uri_bys_long,
            [x in uri_labels | x.short_label] as uri_labels,
            [x in uri_labels | x.label] as uri_labels_long
         """
@@ -2048,14 +2052,28 @@
         # uri_fors, uri_fors_long, uri_bys, uri_bys_long, uri_labels, uri_labels_long
         for i, f in enumerate(self.meta.get("uri_fors")):
             self.df["_uri_" + f] = self.df[[by for by in self.meta.get("uri_bys")]].apply(
                 lambda row: prefix + "_" + f + "_by_" + "/".join([
                     key + ":" + str(item) for key, item in row.items()]), axis=1)
             if self.meta.get("uri_labels"):
                 self.df["_uri_" + f] = self.df["_uri_" + f].map(lambda x: x + "_label_" + "/".join(self.meta.get("uri_labels")))
+
+            if self.meta.get("store_on_existing_nodes") == "true":
+                uri_property_name = "_uri_" + f
+                id_property_name = "_id_" + f
+                df = self.df[[uri_property_name, id_property_name]]
+                
+                q = f"""
+                UNWIND $data as row
+                MATCH (node)
+                WHERE id(node) = row['{id_property_name}']
+                SET node.uri = row['{uri_property_name}']
+                """    
+                params = {"data": df.to_dict(orient='records')}
+                self.method.interface.query(q, params)
         return self.df
 
     def retrieve_json(self):
 
         def get_unique_key(node, label, prop_filter):
             key = node['properties'][prop_filter] + ' ' + label
             return key
```

### Comparing `tab2neo-1.3.0.3/derivation_method/derivation_method.py` & `tab2neo-1.3.9.0/derivation_method/derivation_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,20 @@
         self.batch = False
         self.data = data
         self.name = name
         self._db_id = None
         self._actions = None
         if study is None:
             res = self.interface.query(f"""
-            MATCH (study:Study) 
+            MATCH (s)
+            WHERE s:Study or s:`Study Pool`
+            WITH apoc.text.join(labels(s),'|') as lbl, collect(s) as coll
+            WITH apoc.map.fromPairs(collect([lbl, coll])) as mp
+            WITH coalesce(mp['Study Pool'], mp['Study']) as coll
+            UNWIND coll as study
             RETURN study.`{RDFSLABEL}` as STUDYID 
             ORDER BY STUDYID""")
             assert len(
                 res) == 1, "Provide 'study' id at init of DerivationMethod, as there are 0 or >1 studies in the database"
             if res:
                 study = res[0]['STUDYID']
         self.study = study
```

### Comparing `tab2neo-1.3.0.3/derivation_method/method.py` & `tab2neo-1.3.9.0/derivation_method/method.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/derivation_method/predict_links.cql` & `tab2neo-1.3.9.0/derivation_method/predict_links.cql`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/derivation_method/predict_output_classes.cql` & `tab2neo-1.3.9.0/derivation_method/predict_output_classes.cql`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/derivation_method/super_method.py` & `tab2neo-1.3.9.0/derivation_method/super_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,15 +326,16 @@
                 "script": "remap_term_values",
                 "lang": "python",
                 "package": "basic_df_ops",
                 "params": json.dumps(
                     {
                         "original_col": self.meta['from_class_short_label'],
                         "new_col": self.meta['to_class_short_label'],
-                        "term_pairs": self.meta['term_pairs']
+                        "term_pairs": self.meta['term_pairs'],
+                        "remove_unmapped_rows": True if self.meta["m"].get("remove_unmapped_rows") is None or self.meta["m"].get("remove_unmapped_rows")=='true' else False
                     }
                 ),
                 "github_repo": "gsk-tech/cldnb",  # TODO: update with open-source (future) repository 
                 "github_branch": "main",
                 "repo_scripts_path": "src/utils",
             }, self, dont_fetch=True),
             Link({
@@ -350,15 +351,15 @@
                 "merge": True,
             }, self, dont_fetch=True)
         ]
         return actions
 
     def retrieve_json(self):
         q1 = """
-        CALL apoc.create.vNode(["Method"], {id: $method_id, type: 'decode'}) YIELD node as method
+        CALL apoc.create.vNode(["Method"], {id: $method_id, type: 'decode', remove_unmapped_rows: $remove_unmapped_rows}) YIELD node as method
         WITH method
         MATCH (from_class:Class) WHERE from_class.label = $from_class
         WITH method, from_class
         MATCH (to_class:Class) WHERE to_class.label = $to_class
         CALL apoc.create.vNode(["Class"], apoc.map.submap(from_class, ['label'])) YIELD node as from_class_
         CALL apoc.create.vNode(["Class"], apoc.map.submap(to_class, ['label'])) YIELD node as to_class_
         CALL apoc.create.vRelationship(method, "FROM_CLASS", {}, from_class_) YIELD rel as from_rel
@@ -367,15 +368,16 @@
         UNWIND coll as item
         WITH item[0] as x, item[1] as r, item[2] as y
         """
 
         params = {
             'from_class': self.meta.get('from_class_label'),
             'to_class': self.meta.get('to_class_label'),
-            'method_id': self.action_id
+            'method_id': self.action_id,
+            'remove_unmapped_rows': self.meta['m'].get('remove_unmapped_rows') if self.meta['m'].get('remove_unmapped_rows') is not None else 'true'
         }
 
         res1 = get_arrows_json_cypher(
             neo=self.interface,
             q=q1,
             params=params,
             hide_labels=Action.hide_labels,
@@ -412,15 +414,16 @@
                 OPTIONAL MATCH (action)-[:Statistic]->(statistic:Class)
                 WITH *
                 ORDER BY dimension.short_label, statistic.short_label
                 WITH action, results, results_long,
                     collect(distinct {
                         dimension: coalesce(dimension.short_label, dimension_rel.short_label), 
                         required: dim_r.required,
-                        denominator: dim_r.denominator
+                        denominator: dim_r.denominator,
+                        all_ct: dim_r.all_ct
                     }) as dimensions,
                     collect(distinct {
                         dimension: dimension.label, 
                         required: dim_r.required,
                         denominator: dim_r.denominator
                     }) as dimensions_long,                   
                     collect(distinct statistic.short_label) as statistics,
@@ -441,14 +444,30 @@
         res["m"]["node_id"] = self.method_node_id
         assert res["m"], f"Method node from ApplyStat action {self.action_info} not found"
 
         if res.get('dimensions_long', False):
             for class_dct in res.get('dimensions_long'):
                 self.build_terms_for_distinct_values(class_dct)
 
+        additional_ct_classes = []
+        for dim in res.get('dimensions', []):
+            # TODO: Validation eg cant be all_ct and denominator?
+            if dim.get('all_ct') == 'true':
+                additional_ct_classes.append(dim.get('dimension'))
+
+        if additional_ct_classes:
+            q = """
+            UNWIND $ct_classes as class_short
+            MATCH (c:Class)-[:HAS_CONTROLLED_TERM]->(t:Term)
+            WHERE c.short_label = class_short
+            RETURN c.short_label as short_label, collect([id(t), t.`rdfs:label`]) as ct
+            """
+            res1 = self.interface.query(q, {'ct_classes': additional_ct_classes})
+            res["m"]["additional_ct"] = res1
+
         return res
 
     def build_terms_for_distinct_values(self, class_dct):
         """
         Creates (or merges) term nodes for each value in a class if at least one of those values is not unique.
         E.G. Class Status has two values of 'Attended' and 'Not Attended' but a subject has both Attended and
         Not Attended status' for a single visit. There will be two Attended nodes where we only want one. So we create a
@@ -546,14 +565,37 @@
                             for dct_short, dct_long in zip(self.meta.get("dimensions"), self.meta.get("dimensions_long"))
                         ]
                     }),
                     "include_data": "true",
                     "update_df": "true",
                 }, self, dont_fetch=True)
             )
+
+        additional_ct = self.meta['m'].get('additional_ct', False)
+        if additional_ct:
+            actions.append(
+                CallAPI({
+                    "id": self.meta["m"]["id"] + "_run_script_ct_cartesian_product",
+                    "type": "call_api",
+                    "node_id": self.method_node_id,
+                    "script": 'ct_cartesian_product',
+                    "lang": "python",
+                    "package": "basic_df_ops",
+                    "params": json.dumps(
+                        {
+                            "dimensions": [dim_dict.get('dimension') for dim_dict in self.meta.get("dimensions")],
+                            "dimension_ct": additional_ct
+                        },
+                    ),
+                    "github_repo": "gsk-tech/cldnb",  # TODO: update with open-source (future) repository
+                    "github_branch": "main",
+                    "repo_scripts_path": "src/utils",
+                }, self, dont_fetch=True),
+            )
+
         actions.append(
             BranchSave({
                 "id": self.meta["m"]["id"] + "_branch1",
                 "type": "branch_save"  # saves the current state of self.df into self.branch_load_dfs dict
             }, self, dont_fetch=True)
             )
 
@@ -873,25 +915,26 @@
                         {id: $method_id, type: 'apply_stat', script: 'group_by', lang: 'python', package: 'basic_df_ops', 
                         percentage_dp: $percentage_dp}
                         ELSE
                         {id: $method_id, type: 'apply_stat', script: 'group_by', lang: 'python', package: 'basic_df_ops'}
                         END
                     ) YIELD node as method
                 WITH method, $dimensions as dims, $req_dims as req_dims, $denom_dims as denom_dims
+                WITH method, $dimensions as dims 
                 MATCH (x:Class) WHERE x.label IN dims
+                WITH x, method, 
+                    CASE WHEN x.label IN $req_dims THEN 'true' ELSE NULL END as is_required, 
+                    CASE WHEN x.label IN $denom_dims THEN 'true' ELSE NULL END as is_denominator,
+                    CASE WHEN x.label IN $all_ct_dims THEN 'true' ELSE NULL END as should_all_ct
                 CALL apoc.create.vNode(["Class"], apoc.map.submap(x, ['label'])) YIELD node as x_
-                CALL apoc.create.vRelationship(method, "Dimension", 
-                    CASE
-                        WHEN (x.label IN req_dims) AND (x.label IN denom_dims) THEN {required: 'true', denominator: 'true'}
-                        WHEN (x.label IN req_dims) AND NOT (x.label IN denom_dims) THEN {required: 'true'}
-                        WHEN NOT (x.label IN req_dims) AND (x.label IN denom_dims) THEN {denominator: 'true'}
-                        ELSE {}
-                        END
-                    , 
-                    x_) YIELD rel
+                CALL apoc.create.vRelationship(method, "Dimension", {
+                    denominator: is_denominator,
+                    required: is_required,
+                    `all_ct`: should_all_ct
+                }
                 WITH [[method, rel, x_]] as coll
                 UNWIND coll as item
                 WITH item[0] as x, item[1] as r, item[2] as y
                 """
 
         q2 = """
                 CALL apoc.create.vNode(["Method"], {id: $method_id, type: 'apply_stat', script: 'group_by', lang: 'python',
@@ -921,29 +964,33 @@
         assert len(self.meta.get('results_long')) == 1, \
             f"Expected result to be a list of len 1, it was: {self.meta.get('results_long')}"
         result = self.meta.get('results_long')[0]
 
         dimensions = []
         dimensions_required = []
         dimensions_denominator = []
+        all_ct_dims = []
 
         for dim in self.meta.get('dimensions_long'):
             if dim.get('dimension'):
                 dimensions.append(dim.get('dimension'))
             if dim.get('required'):
                 dimensions_required.append(dim.get('dimension'))
             if dim.get('denominator'):
                 dimensions_denominator.append(dim.get('dimension'))
+            if dim.get('all_ct'):
+                dimensions_denominator.append(dim.get('dimension'))
 
         params = {
             'dimensions': dimensions,
             'statistics': self.meta.get('statistics_long'),
             'result': result,
             'req_dims': dimensions_required,
             'denom_dims': dimensions_denominator,
+            'all_ct_dims': all_ct_dims,
             'percentage_dp': self.meta.get('m').get('percentage_dp') if dimensions_denominator else None,
             'method_id': self.action_id
         }
 
         res1 = get_arrows_json_cypher(
             neo=self.interface,
             q=q1,
@@ -982,14 +1029,23 @@
             'Term': 'rdfs:label',
             'Method': 'id',
             # 'Relationship': 'relationship_type'
         }
 
         # go through each res and compile them (without duplicates)
         for res in [res1, res2, res3]:
+            # Cleanup null v-relationship values
+            for rel in res['relationships']:
+                clean_props = {}
+                rel_properties = rel.get('properties')
+                for key, value in rel_properties.items():
+                    if value is not None:
+                        clean_props[key] = value
+                rel['properties'] = clean_props
+
             node_indexes_to_skip = []
             for node_index, node in enumerate(res['nodes']):
                 for label in filter_node_dict.keys():
                     if label in node['labels']:
                         prop_filter = filter_node_dict[label]  # label or id
                         unique_node_key = self.get_unique_key(node, label, prop_filter)
                         # eg Analysis Value Class, apply_stat Method
```

### Comparing `tab2neo-1.3.0.3/derivation_method/utils.py` & `tab2neo-1.3.9.0/derivation_method/utils.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/logger/logger.py` & `tab2neo-1.3.9.0/logger/logger.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/model_appliers/model_applier.py` & `tab2neo-1.3.9.0/model_appliers/model_applier.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/model_managers/model_manager.py` & `tab2neo-1.3.9.0/model_managers/model_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,14 +213,42 @@
 
         class_list = sorted(list(class_set))  # Convert the final set back to list
 
         self.create_relationship(rel_list, identifier, match_classes=False)
 
         return class_list
 
+    def create_subclass(self, subclass_list: List[List[str]], identifier='label', match_classes=True)-> [str]:
+        """
+        An additional label is added to a class node ('variable') if some of the variables need to be grouped of the class as defined in subclass_list.
+        For example:
+            With subclass_list = [ ['parent', 'child'] ]
+            A new class label with name as "SUBCLASS_OF", as specified by the
+            identifier will be created between "parent" and "child".
+        """
+
+        q= f"""
+        UNWIND $class_list as class_
+        WITH class_[0] as class_label, class_[1] as subclass_label
+        {'MATCH' if match_classes else 'MERGE'} (c1:Class {{`{identifier}`:class_label}})
+        {'MATCH' if match_classes else 'MERGE'} (c2:Class {{`{identifier}`:subclass_label}})   
+        MERGE (c1)<-[:SUBCLASS_OF]-(c2)
+        RETURN collect([c1.`{identifier}`, c2.`{identifier}`]) as classes
+        """
+        res = self.query(q, {
+            "class_list": [sc for sc in subclass_list]
+        })
+
+        if res:
+            self.propagate_rels_to_child_class()
+            self.propagate_terms_to_parent_class()
+            return res[0]['classes']
+        else:
+            return []
+    
     def create_relationship(self, rel_list: List[List[str]], identifier='label', match_classes=True) -> [str]:
         """
         Create relationship nodes between two specified classes as defined in rel_list.
         For example:
         1.  With rel_list = [ ['class1', 'class2', 'example'] ]
             A new relationship node will be created between nodes with "label", as specified by the
             identifier, 'class1' and 'class2' with a relationship_type property = 'example'.
@@ -271,14 +299,71 @@
 
         if res:
             result = [np.array(i).flatten().tolist() for i in res[0].get('rels')]
             return result
         else:
             return []
 
+    def delete_terms_of_parent_class(self, subclass_list: [[str, str]], identifier='label'):
+        if self.verbose:
+            logger.info("Deleting propgated terms of 'parent' classes where (child)-[:SUBCLASS_OF]->(parent) and the  subclass rel no longer exists")
+
+        match_rel = f'(:Class{{`{identifier}`:child}})-[:SUBCLASS_OF*1..50]->(source:Class)'
+
+        q=f"""
+        UNWIND $subclass_rel as subclass_rel
+        WITH subclass_rel[0] as parent, subclass_rel[1] as child
+        MATCH (:Class{{`{identifier}`:child}})-[:HAS_CONTROLLED_TERM]->(term:Term), {match_rel}, (source)-[has_term:HAS_CONTROLLED_TERM]->(term)
+        DETACH DELETE has_term 
+        """
+
+        params = {"subclass_rel": subclass_list}  
+        return self.query(q, params, return_type='neo4j.Result')
+
+    def delete_rels_of_child_class(self, subclass_list: [[str, str]], identifier='label'):
+        if self.verbose:
+            logger.info("Deleting propagated relationships from 'child' classes where (child)-[:SUBCLASS_OF]->(parent) and the subclass rel no longer exists")
+        
+        match_rel = '(source:Class)-[:SUBCLASS_OF*1..50]->(c)'
+
+        q = f"""
+        UNWIND $subclass_rel as subclass_rel
+        WITH subclass_rel[0] as parent, subclass_rel[1] as child
+        MATCH (c:Class{{`{identifier}`:parent}})<-[r1:TO|FROM]-(r:Relationship)-[r2:TO|FROM]-(target:Class), {match_rel}, (source)<-[:FROM]-(del_rel:Relationship{{`relationship_type`:r.relationship_type}})-[:TO]->(target)
+        DETACH DELETE del_rel
+        """
+
+        params = {"subclass_rel": subclass_list}  
+        return self.query(q, params, return_type='neo4j.Result')
+
+    def delete_subclasses(self, subclass_list: [[str, str]], identifier='label'):
+        """
+        Deletes the propagated terms and relationship and subclass relationships between specified classes.
+        :param rel_list: List of parent ad child classes to be deleted in the following format:
+                         [parent_class, child_class]
+                         For example: With identifier = 'label' and
+                         subclass_list = [['class1', 'class2'], ...]
+                         'SUBCLASS_OF'relationships between classes with labels = 'class1' and 'class2'
+                         would be deleted.
+        :param identifier: String class property to be used when identifying classes.
+        :return:
+        """
+
+        self.delete_terms_of_parent_class(subclass_list, identifier)
+        self.delete_rels_of_child_class(subclass_list, identifier)
+
+        q = f"""
+        UNWIND $subclass as subclass
+        WITH subclass[0] as parent, subclass[1] as child
+        MATCH (:Class{{`{identifier}`:parent}})<-[subclass_rel:SUBCLASS_OF]-(:Class{{`{identifier}`:child}})
+        DETACH DELETE subclass_rel
+        """
+        params = {"subclass": subclass_list}
+        return self.query(q, params, return_type='neo4j.Result')
+
     def delete_relationship(self, rel_list: [[str, str, str]], identifier='label'):
         """
         Deletes specified relationships between classes.
         :param rel_list: List of relationships to be deleted in the following format:
                          [from class prop value, to class prop value, relationship type]
                          For example: With identifier = 'label' and
                          rel_list = [['class1', 'class2', 'Example'], ...]
@@ -344,14 +429,25 @@
         q = f"""
         MATCH (c:Class)
         {q_return}
         """
 
         return self.query(q)
 
+    def get_subclasses_where(self, where_clause=None, identifier='label') -> [{}]:
+        
+        q=f"""MATCH (c1:Class)<-[:SUBCLASS_OF]-(c2:Class)
+            {where_clause if where_clause else ""}
+            RETURN {{parent: c1.`{identifier}`, child: c2.`{identifier}`}} as classes"""
+
+        res = self.query(q)
+
+        return [x['classes'] for x in res]       
+
+
     def get_rels_where(self, where_clause=None, return_prop="label") -> [{}]:
         """
         Returns a list of dictionaries representing relationships between all classes or a subset of classes and/or
         relationships if filtered with a cypher where clause.
         :param where_clause: Optional string cypher where clause, For example:
                              `WHERE from_class.short_label IS NOT NULL` - Only relationships from_classes with a short_label
         :param return_prop: Property to identify class in returned relationships. For example with
@@ -888,29 +984,63 @@
         {where_clause}
         DETACH DELETE rel
         """
 
         return self.query(q, {'same_as_terms': same_as_terms}, return_type='neo4j.Result')
 
     def propagate_rels_to_parent_class(self):
+            if self.verbose:
+                logger.info("Copying Relationships to 'parent' Classes where (child)-[:SUBCLASS_OF]->(parent)")
+            self.query("""
+            MATCH (c:Class)<-[r1:TO|FROM]-(r:Relationship)-[r2:TO|FROM]-(target:Class), (c)-[:SUBCLASS_OF*1..50]->(source:Class)
+            WHERE type(r1) <> type(r2)
+            WITH *,
+            "
+                WITH $source as source, $target as target
+                MERGE (source)<-[:`"+type(r1)+"`]-(:Relationship{relationship_type:$type})-[:`"+type(r2)+"`]->(target)
+                RETURN count(*)
+            " as q, 
+            {type: r.relationship_type, source: source , target: target} as params
+            CALL apoc.cypher.doIt(q, params) YIELD value
+            RETURN value, q, params         
+            """)
+
+    def propagate_rels_to_child_class(self):
         if self.verbose:
-            logger.info("Copying Relationships to 'parent' Classes where (child)-[:SUBCLASS_OF]->(parent)")
-        self.query("""
-        MATCH (c:Class)<-[r1:TO|FROM]-(r:Relationship)-[r2:TO|FROM]-(target:Class), (c)-[:SUBCLASS_OF*1..50]->(source:Class)
+            logger.info("Copying Relationships to 'child' Classes where (child)-[:SUBCLASS_OF]->(parent)")
+        
+        match_rel = '(source:Class)-[:SUBCLASS_OF*1..50]->(c)'
+
+        self.query(f"""
+        MATCH (c:Class)<-[r1:TO|FROM]-(r:Relationship)-[r2:TO|FROM]-(target:Class), {match_rel}
         WHERE type(r1) <> type(r2)
         WITH *,
         "
             WITH $source as source, $target as target
-            MERGE (source)<-[:`"+type(r1)+"`]-(:Relationship{relationship_type:$type})-[:`"+type(r2)+"`]->(target)
+            MERGE (source)<-[:`"+type(r1)+"`]-(:Relationship{{relationship_type:$type}})-[:`"+type(r2)+"`]->(target)
             RETURN count(*)
         " as q, 
-        {type: r.relationship_type, source: source , target: target} as params
+        {{type: r.relationship_type, source: source , target: target}} as params
         CALL apoc.cypher.doIt(q, params) YIELD value
         RETURN value, q, params         
+        """)  
+
+
+    def propagate_terms_to_parent_class(self):
+        if self.verbose:
+            logger.info("Copying terms to 'parent' where (child)-[:SUBCLASS_OF]->(parent)")
+        
+        match_rel = '(c)-[:SUBCLASS_OF*1..50]->(source:Class)'
+
+        self.query(f"""
+        MATCH (c:Class)-[:HAS_CONTROLLED_TERM]->(term:Term), {match_rel}
+        MERGE (source)-[:HAS_CONTROLLED_TERM]->(term) 
+        RETURN term     
         """)
+  
 
     def remove_unmapped_classes(self):
         if self.verbose:
             logger.info("Removing Unmapped Classes")
         q = """
         MATCH (c:Class)
         WHERE NOT EXISTS (
@@ -1103,25 +1233,23 @@
             self,
             data_label: str = "Source Data Row",
             data_table_label: str = "Source Data Table",
             domain_property: str = "_domain_",
             no_domain_label: str = "Thing",
             data_column_label: str = "Source Data Column",
             columnname_property: str = "_columnname_",
-            exclude_properties: list = None,
+            exclude_properties: list = ["_filename_", "_folder_"],
     ):
         """
         Creates Class and Relationship nodes to represent a trivial schema to reshape data ingested e.g. with
         FileDataLoader - Tables loaded into nodes one row to one node, column names used as property names.
 
         data_labels: labels of the nodes where loaded data is stored (mm with use OR btw labels to fetch data nodes)
         domain_property: property where the name of the table/domain can be found
         """
-        if exclude_properties is None:
-            exclude_properties = ["_filename_", "_folder_"]
         q = f"""
         MATCH (data:`{data_label}`)<-[:HAS_DATA]-(dt:`{data_table_label}`)        
         WITH distinct dt, dt._domain_ as domain, keys(data) as ks
         WITH *, CASE WHEN domain IS NULL THEN $no_domain_label ELSE domain END as domain
         WITH dt, domain, [k in ks WHERE NOT k IN $exclude_properties] as ks
         WITH dt, domain, apoc.coll.flatten(apoc.coll.toSet(ks)) as ks
         MERGE (c:Class{{label: domain, short_label: domain, create: True}})
@@ -1134,8 +1262,125 @@
         MERGE (c)<-[:FROM]-(r:Relationship{{relationship_type: k}})-[:TO]->(c2)
         MERGE (col)-[:MAPS_TO_CLASS]->(c2)        
         """
         params = {
             "exclude_properties": exclude_properties + [domain_property],
             "no_domain_label": no_domain_label
         }
-        self.query(q, params)
+        self.query(q, params)
+        
+    def export_model_to_linkml(self):
+        """
+        Read the Class/Relationship/Term model from Neo4j and returns a linkml like dict.
+        More about linkml:
+            https://linkml.io/linkml/
+            https://github.com/linkml/linkml
+        One can then easily create a yaml file from the dict with the following code:
+        import yaml
+        cld_schema_dict = mm.export_model_to_linkml()
+        yaml_serialized = yaml.dump(cld_schema_dict)
+        with open(f"cld.yaml", "w") as f:
+            f.write(yaml_serialized)        
+        """
+        
+        q = """
+        MATCH (c:Class)
+        WITH c, apoc.map.fromPairs(
+                [k in [k in ['label', 'short_label', 'derived', 'data_type', 'is_stat', 'uri'] WHERE NOT c[k] IS NULL] | [k,c[k]]]
+            ) as class_map
+        OPTIONAL MATCH (c)-[:FROM]-(r:Relationship)-[:TO]->(c2:Class)
+        WITH c, class_map, {alias: r.relationship_type, name: c.label + " " + r.relationship_type, uri: r.uri} as _attr, c2
+        ORDER BY c.label, c2.label, r.relationship_type
+        WITH c, class_map, [x in collect( 
+            apoc.map.fromPairs(
+                [k in [k in ['alias', 'name', 'uri'] WHERE NOT _attr[k] IS NULL] | [k, _attr[k]]] + [['range', c2.label]]
+            )
+        ) WHERE NOT x = {range: NULL}]
+        + CASE WHEN c.create = True THEN [] ELSE [{
+            alias: 'rdfs:label', name:c.label + ' rdfs:label', 
+            range: 
+                CASE WHEN EXISTS ((c)-[:HAS_CONTROLLED_TERM]->(:Term)) THEN c.label + ' CT' ELSE coalesce(c.data_type, 'string') END
+        }] END 
+        as attributes
+        WITH c, class_map, attributes
+        WITH collect(apoc.map.merge(class_map, {attributes: attributes})) as classes
+        OPTIONAL MATCH (c:Class)-[:HAS_CONTROLLED_TERM]->(t:Term)
+        WITH classes, c, {permissible_values: apoc.map.fromPairs(collect(
+            [t.`rdfs:label`, {description: t.`Codelist Code` + '_' + t.`Term Code`}]
+        ))} as pv
+        WITH classes, apoc.map.fromPairs(collect([c.label + ' CT', pv])) as enums        
+        WITH {classes: classes, enums: enums} as res
+        RETURN apoc.map.fromPairs([k in [k in keys(res) WHERE NOT (res[k] IS NULL or res[k] = {} or res[k] = [])] | [k, res[k]]]) as res
+        """
+        #TODO: currently linkml range for rdfs:label is set to Class.data_type, need to check that these are aligned with linkml types
+        return self.query(q)[0]['res']
+            
+    def create_model_from_linkml(self, linkml_dict: dict):
+        """
+        Create Class/Relationship/Term schema from a linkml-like dict (see export_model_to_linkml above)
+        One can read linkml schema from a yaml file with the following code:
+        
+        import yaml
+        with open("cld.yaml", "r") as stream:
+            cld_schema_dict = yaml.safe_load(stream)
+            
+        Args:
+            linkml_dict (dict): linkml-like dict
+        """
+        classes = linkml_dict.get('classes')
+        for class_ in classes:
+            attrs = class_.pop("attributes")
+            self.create_class([class_], merge_on=["label"])
+            self.create_relationship(
+                [
+                    [class_.get("label"), attr_.get("range"), attr_.get("alias")] 
+                    for attr_ in attrs
+                    if not attr_.get("alias") == "rdfs:label"
+                ]
+            )
+            
+        ct = {}
+        for class_, dct_1 in linkml_dict.get("enums").items():
+            ct[class_[:-3]] = [
+                {
+                    'rdfs:label': rdfs_label,
+                    'Codelist Code': dct_2.get("description").split("_")[0],
+                    'Term Code': dct_2.get("description").split("_")[1]
+                }
+                for rdfs_label, dct_2 in dct_1.get("permissible_values").items()
+            ]
+        self.create_ct(
+            ct,
+            merge_on=['Codelist Code', 'Term Code']
+        )
+
+    def delete_from_graph(self):
+        actions = [
+            f"""
+            MATCH (m:Method)
+            OPTIONAL MATCH path = (m)-[r:METHOD_ACTION|NEXT*1..10]->(x:`Method`)
+            OPTIONAL MATCH path2 = (x)-[r2]->(y)
+            DETACH DELETE r2, x
+            """,
+            f"""
+            MATCH (m:Method)
+            OPTIONAL MATCH (m)-[r]-()
+            DELETE r
+            DELETE m
+            """,
+            f"""
+            MATCH (class:Class)
+            WHERE class.derived IS NOT NULL
+            OPTIONAL MATCH (class)-[r:HAS_CONTROLLED_TERM]-(term:Term)
+            OPTIONAL MATCH (class)-[r1:TO|FROM]-(rel:Relationship)-[r2:TO|FROM]-(class2:Class)
+            DELETE r, r1
+            DETACH DELETE term, class, rel
+            """,
+            f"""
+            MATCH (term1:Term)-[r:SAME_AS]->(term2:Term)
+            DELETE r
+            """
+        ]
+        for q in actions:
+            self.query(q)
+
+
```

### Comparing `tab2neo-1.3.0.3/query_builders/query_builder.py` & `tab2neo-1.3.9.0/query_builders/query_builder.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/setup.py` & `tab2neo-1.3.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             print('Dependency to a git repository should have the format:')
             print('git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name')
     else:
         required.append(line)
 
 setuptools.setup(
     name="tab2neo",                         # This is the name of the package
-    version="1.3.0.3",                      # Release.Major Feature.Minor Feature.Bug Fix
+    version="1.3.9.0",                      # Release.Major Feature.Minor Feature.Bug Fix
     author="Alexey Kuznetsov",              # Full name of the author
     description="Clinical Linked Data: High-level Python classes to load, model and reshape tabular data imported into Neo4j database",
     long_description="https://github.com/GSK-Biostatistics/tab2neo/blob/main/README.md",      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(include=[
         "logger",
         "analysis_metadata",
```

### Comparing `tab2neo-1.3.0.3/tab2neo.egg-info/PKG-INFO` & `tab2neo-1.3.9.0/tab2neo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab2neo
-Version: 1.3.0.3
+Version: 1.3.9.0
 Summary: Clinical Linked Data: High-level Python classes to load, model and reshape tabular data imported into Neo4j database
 Home-page: UNKNOWN
 Author: Alexey Kuznetsov
 License:                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
```

### Comparing `tab2neo-1.3.0.3/tab2neo.egg-info/SOURCES.txt` & `tab2neo-1.3.9.0/tab2neo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.3/tab2neo.egg-info/requires.txt` & `tab2neo-1.3.9.0/tab2neo.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 et-xmlfile==1.1.0
 isodate==0.6.1
 JayDeBeApi==1.2.3
 JPype1==1.4.1
 msal==1.20.0
 msal-extensions==0.3.1
 msrest==0.7.1
-neointerface==3.1.9
+neointerface==3.3.1
 oauthlib==3.2.2
 openpyxl==3.0.7
 portalocker==2.6.0
+pyarrow==12.0.1
 pycparser==2.21
 PyGithub==1.55
 PyJWT==2.6.0
 PyNaCl==1.5.0
 pyreadr==0.4.0
 pyreadstat==1.0.8
 requests-oauthlib==1.3.1
```

### Comparing `tab2neo-1.3.0.3/tests/test_comparison_utilities.py` & `tab2neo-1.3.9.0/tests/test_comparison_utilities.py`

 * *Files identical despite different names*

