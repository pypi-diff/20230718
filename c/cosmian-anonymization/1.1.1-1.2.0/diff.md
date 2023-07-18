# Comparing `tmp/cosmian_anonymization-1.1.1-py3-none-any.whl.zip` & `tmp/cosmian_anonymization-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20345 bytes, number of entries: 11
--rw-r--r--  2.0 unx      169 b- defN 80-Jan-01 00:00 cosmian_anonymization/__init__.py
--rw-r--r--  2.0 unx     8030 b- defN 80-Jan-01 00:00 cosmian_anonymization/anonymize.py
+Zip file size: 20456 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 cosmian_anonymization/__init__.py
+-rw-r--r--  2.0 unx     8273 b- defN 80-Jan-01 00:00 cosmian_anonymization/anonymize.py
 -rw-r--r--  2.0 unx     1954 b- defN 80-Jan-01 00:00 cosmian_anonymization/conversion_helper.py
 -rw-r--r--  2.0 unx     3628 b- defN 80-Jan-01 00:00 cosmian_anonymization/method_parser.py
 -rw-r--r--  2.0 unx     3784 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_correlation.py
 -rw-r--r--  2.0 unx     3887 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_parser.py
--rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1500 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1030 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.1.1.dist-info/RECORD
-11 files, 56418 bytes uncompressed, 18565 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1500 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1030 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.2.0.dist-info/RECORD
+11 files, 56754 bytes uncompressed, 18676 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: cosmian_anonymization/noise_correlation.py
 Comment: 
 
 Filename: cosmian_anonymization/noise_parser.py
 Comment: 
 
-Filename: cosmian_anonymization-1.1.1.dist-info/LICENSE.md
+Filename: cosmian_anonymization-1.2.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: cosmian_anonymization-1.1.1.dist-info/METADATA
+Filename: cosmian_anonymization-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: cosmian_anonymization-1.1.1.dist-info/WHEEL
+Filename: cosmian_anonymization-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: cosmian_anonymization-1.1.1.dist-info/entry_points.txt
+Filename: cosmian_anonymization-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cosmian_anonymization-1.1.1.dist-info/RECORD
+Filename: cosmian_anonymization-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cosmian_anonymization/__init__.py

```diff
@@ -1,4 +1,7 @@
 # -*- coding: utf-8 -*-
+import importlib.metadata
+
 from cosmian_anonymization.anonymize import anonymize_dataframe, anonymize_from_files
 
+__version__ = importlib.metadata.version(__package__ or __name__)
 __all__ = ["anonymize_dataframe", "anonymize_from_files"]
```

## cosmian_anonymization/anonymize.py

```diff
@@ -37,14 +37,17 @@
         col_name = column_metadata["name"]
         col_type = column_metadata["type"]
 
         if col_name not in df:
             # Column missing from the dataset
             raise ValueError(f"Missing column from data: {col_name}.")
 
+        if "method" in column_metadata and column_metadata["method"] == "DeleteColumn":
+            continue  # Do not add column to the output dataframe
+
         # Add this column as output to match the config's order
         sorted_output_columns.append(col_name)
 
         # Make sure the type of the pandas column is the same as the one in the config
         output_df[col_name] = convert_config_types(df[col_name], col_type)
 
     # Return the output dataframe with columns in the config's order
@@ -140,14 +143,18 @@
 
     # Init output dataframe to match the config columns
     output_df = create_output_dataframe(df, config, inplace)
 
     # Iterate over each column to anonymize.
     for column_metadata in config["metadata"]:
         col_name: str = column_metadata["name"]
+
+        if col_name not in output_df:
+            continue  # Column has been deleted
+
         # Anonymize the column
         output_df[col_name] = apply_anonymization_column(
             output_df[col_name],
             column_metadata.get("method", None),
             column_metadata.get("method_options", {}),
         )
```

## Comparing `cosmian_anonymization-1.1.1.dist-info/LICENSE.md` & `cosmian_anonymization-1.2.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `cosmian_anonymization-1.1.1.dist-info/METADATA` & `cosmian_anonymization-1.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmian-anonymization
-Version: 1.1.1
+Version: 1.2.0
 Summary: Cosmian Anonymization library in Python
 Author: Hugo Rosenkranz-Costa
 Author-email: hugo.rosenkranz@cosmian.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

