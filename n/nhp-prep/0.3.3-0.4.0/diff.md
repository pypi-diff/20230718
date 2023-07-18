# Comparing `tmp/nhp-prep-0.3.3.tar.gz` & `tmp/nhp-prep-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhp-prep-0.3.3.tar", last modified: Mon Jun 26 13:01:59 2023, max compression
+gzip compressed data, was "nhp-prep-0.4.0.tar", last modified: Tue Jul 18 18:02:58 2023, max compression
```

## Comparing `nhp-prep-0.3.3.tar` & `nhp-prep-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.549883 nhp-prep-0.3.3/
--rw-r--r--   0 hugo       (501) staff       (20)       64 2023-03-31 19:18:02.000000 nhp-prep-0.3.3/MANIFEST.in
--rw-r--r--   0 hugo       (501) staff       (20)     3483 2023-06-26 13:01:59.549698 nhp-prep-0.3.3/PKG-INFO
--rw-r--r--   0 hugo       (501) staff       (20)     2830 2023-06-26 12:45:36.000000 nhp-prep-0.3.3/README.md
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.548194 nhp-prep-0.3.3/app/
--rw-r--r--   0 hugo       (501) staff       (20)      325 2023-06-26 13:00:06.000000 nhp-prep-0.3.3/app/__init__.py
--rw-r--r--   0 hugo       (501) staff       (20)    17482 2023-06-26 12:45:36.000000 nhp-prep-0.3.3/app/__main__.py
--rw-r--r--   0 hugo       (501) staff       (20)       57 2022-11-20 13:33:19.000000 nhp-prep-0.3.3/app/cli.py
--rw-r--r--   0 hugo       (501) staff       (20)      830 2022-11-20 13:33:19.000000 nhp-prep-0.3.3/app/column_mapper.py
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.548457 nhp-prep-0.3.3/app/config/
--rw-r--r--   0 hugo       (501) staff       (20)     1244 2023-02-24 03:59:57.000000 nhp-prep-0.3.3/app/config/columns__std_format.csv
--rw-r--r--   0 hugo       (501) staff       (20)      677 2022-11-22 20:27:38.000000 nhp-prep-0.3.3/app/config/logs.yaml
--rw-r--r--   0 hugo       (501) staff       (20)      274 2022-12-20 16:45:39.000000 nhp-prep-0.3.3/app/main_logger.py
--rw-r--r--   0 hugo       (501) staff       (20)     8045 2023-06-26 12:45:36.000000 nhp-prep-0.3.3/app/rename_files.py
--rw-r--r--   0 hugo       (501) staff       (20)     4300 2023-03-24 20:17:31.000000 nhp-prep-0.3.3/app/subject_changer.py
--rw-r--r--   0 hugo       (501) staff       (20)     1639 2023-02-27 04:12:49.000000 nhp-prep-0.3.3/app/timestamp_estimator.py
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.548616 nhp-prep-0.3.3/app/util/
--rw-r--r--   0 hugo       (501) staff       (20)     2519 2023-06-26 12:45:36.000000 nhp-prep-0.3.3/app/util/rough_estimate_std_files.py
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.549471 nhp-prep-0.3.3/nhp_prep.egg-info/
--rw-r--r--   0 hugo       (501) staff       (20)     3483 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (501) staff       (20)      487 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (501) staff       (20)        1 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (501) staff       (20)       47 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/entry_points.txt
--rw-r--r--   0 hugo       (501) staff       (20)       39 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/requires.txt
--rw-r--r--   0 hugo       (501) staff       (20)       13 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/top_level.txt
--rw-r--r--   0 hugo       (501) staff       (20)       38 2023-02-28 17:18:12.000000 nhp-prep-0.3.3/requirements.txt
--rw-r--r--   0 hugo       (501) staff       (20)       38 2023-06-26 13:01:59.549935 nhp-prep-0.3.3/setup.cfg
--rw-r--r--   0 hugo       (501) staff       (20)     1268 2023-06-26 12:59:48.000000 nhp-prep-0.3.3/setup.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-07-18 18:02:58.382469 nhp-prep-0.4.0/
+-rw-r--r--   0 hugo       (501) staff       (20)       64 2023-03-31 19:18:02.000000 nhp-prep-0.4.0/MANIFEST.in
+-rw-r--r--   0 hugo       (501) staff       (20)     3679 2023-07-18 18:02:58.382236 nhp-prep-0.4.0/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)     3026 2023-07-18 17:56:28.000000 nhp-prep-0.4.0/README.md
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-07-18 18:02:58.379995 nhp-prep-0.4.0/app/
+-rw-r--r--   0 hugo       (501) staff       (20)      325 2023-07-18 18:00:45.000000 nhp-prep-0.4.0/app/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)    20286 2023-07-18 17:56:28.000000 nhp-prep-0.4.0/app/__main__.py
+-rw-r--r--   0 hugo       (501) staff       (20)       57 2022-11-20 13:33:19.000000 nhp-prep-0.4.0/app/cli.py
+-rw-r--r--   0 hugo       (501) staff       (20)      830 2022-11-20 13:33:19.000000 nhp-prep-0.4.0/app/column_mapper.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-07-18 18:02:58.380435 nhp-prep-0.4.0/app/config/
+-rw-r--r--   0 hugo       (501) staff       (20)     1244 2023-02-24 03:59:57.000000 nhp-prep-0.4.0/app/config/columns__std_format.csv
+-rw-r--r--   0 hugo       (501) staff       (20)      677 2022-11-22 20:27:38.000000 nhp-prep-0.4.0/app/config/logs.yaml
+-rw-r--r--   0 hugo       (501) staff       (20)      274 2022-12-20 16:45:39.000000 nhp-prep-0.4.0/app/main_logger.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1058 2023-07-18 17:56:28.000000 nhp-prep-0.4.0/app/merge_csv.py
+-rw-r--r--   0 hugo       (501) staff       (20)     8045 2023-06-26 12:45:36.000000 nhp-prep-0.4.0/app/rename_files.py
+-rw-r--r--   0 hugo       (501) staff       (20)     4300 2023-03-24 20:17:31.000000 nhp-prep-0.4.0/app/subject_changer.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1639 2023-02-27 04:12:49.000000 nhp-prep-0.4.0/app/timestamp_estimator.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-07-18 18:02:58.380617 nhp-prep-0.4.0/app/util/
+-rw-r--r--   0 hugo       (501) staff       (20)     2519 2023-06-26 12:45:36.000000 nhp-prep-0.4.0/app/util/rough_estimate_std_files.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-07-18 18:02:58.381955 nhp-prep-0.4.0/nhp_prep.egg-info/
+-rw-r--r--   0 hugo       (501) staff       (20)     3679 2023-07-18 18:02:58.000000 nhp-prep-0.4.0/nhp_prep.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)      504 2023-07-18 18:02:58.000000 nhp-prep-0.4.0/nhp_prep.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (501) staff       (20)        1 2023-07-18 18:02:58.000000 nhp-prep-0.4.0/nhp_prep.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       47 2023-07-18 18:02:58.000000 nhp-prep-0.4.0/nhp_prep.egg-info/entry_points.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       39 2023-07-18 18:02:58.000000 nhp-prep-0.4.0/nhp_prep.egg-info/requires.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       13 2023-07-18 18:02:58.000000 nhp-prep-0.4.0/nhp_prep.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       38 2023-02-28 17:18:12.000000 nhp-prep-0.4.0/requirements.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       38 2023-07-18 18:02:58.382524 nhp-prep-0.4.0/setup.cfg
+-rw-r--r--   0 hugo       (501) staff       (20)     1268 2023-07-18 18:00:04.000000 nhp-prep-0.4.0/setup.py
```

### Comparing `nhp-prep-0.3.3/PKG-INFO` & `nhp-prep-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhp-prep
-Version: 0.3.3
+Version: 0.4.0
 Summary: Pre-processing data tool for NHP Lab @ CMU
 Home-page: https://caoslab.psy.cmu.edu:32443/monkeylab/preprocessing-scripts
 Author: Hugo Angulo, Zijun Zhao
 Author-email: hugoanda@andrew.cmu.edu, zijunzha@andrew.cmu.edu
 License: MIT
 Keywords: nhp-prep,caoslab,cmu,pre-processing
 Classifier: Development Status :: 5 - Production/Stable
@@ -96,14 +96,19 @@
 
 4. Renaming of Subject according to logs file (needs the file) (`sub-rename`)
 
 ```
 nhp-prep sub-rename -r <file_with_columns_and_reference_subject_names> -i <directory_with_files_OR_unique_CSV_file> -o <output_directory>
 ```
 
+5. Merge multiple CSV files into a single file. The input should be a directory and so is the output
+```
+nhp-prep merge-csv -i <directory_with_files_OR_unique_CSV_file> -o <output_directory>
+```
+
 You could also run `nhp-prep --help` to see the available commands and their corresponding usage.
 
 If you want to know all the options available for an specific command, run the following:
 
 ```
 nhp-prep COMMAND --help
 ```
```

### Comparing `nhp-prep-0.3.3/README.md` & `nhp-prep-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -79,14 +79,19 @@
 
 4. Renaming of Subject according to logs file (needs the file) (`sub-rename`)
 
 ```
 nhp-prep sub-rename -r <file_with_columns_and_reference_subject_names> -i <directory_with_files_OR_unique_CSV_file> -o <output_directory>
 ```
 
+5. Merge multiple CSV files into a single file. The input should be a directory and so is the output
+```
+nhp-prep merge-csv -i <directory_with_files_OR_unique_CSV_file> -o <output_directory>
+```
+
 You could also run `nhp-prep --help` to see the available commands and their corresponding usage.
 
 If you want to know all the options available for an specific command, run the following:
 
 ```
 nhp-prep COMMAND --help
 ```
```

### Comparing `nhp-prep-0.3.3/app/__main__.py` & `nhp-prep-0.4.0/app/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """
 This is the entrypoint for the CLI application.
 """
 
 from time import time
+from datetime import datetime
 import os
 import tempfile
 import click
 
 import pkg_resources
 
 import pandas as pd
+import glob
 
 from app import __app_name__, __version__
 from app.main_logger import logger
 from app.column_mapper import map_columns
 from app.subject_changer import change_sub
 from app.timestamp_estimator import change_timestamp
 from app.rename_files import file_rename
+from app.merge_csv import merge_csv_files
+
+from app.util.rough_estimate_std_files import dir_time_estimate
 from app.util.rough_estimate_std_files import dir_time_estimate
 
 
 FILE_TYPE = '.csv'
 FILE_COLUMNS_STD = 'config/columns__std_format.csv'
 
 
@@ -425,15 +430,85 @@
         'Cleaning up temporary directory for Steps 2 - 3: %s...', _tmp_dir_step2.name)
     _tmp_dir_step2.cleanup()
     logger.info(
         '[EXECUTION-TIME] Elapse time to execute all the preparation steps: '
         '%f seconds!', time() - start_time)
 
 
+@click.command(name='merge-csv', short_help='Merge multiple CSV files into a single file.')
+@click.option('--input', '-i', required=True, help='Input directory.')
+@click.option('--output', '-o', help='Output directory.')
+@click.pass_context
+def merge_csv(ctx, input, output):
+    """
+    Processes the file(s) from an input, and
+    returns the same file(s) to a different output
+    input, but with the format:
+
+    YYYY-MM-DD_HHmmh_<experiment_name>_<Subject_name>_<Researcher_name_or_initials>_data.csv
+
+    OUTPUT: 
+    If the output path does not exist, it will be created.
+    Also, if the Output path is not passed, nhp-prep will
+    proceed to use the path of each file and rename the original
+    file.
+    """
+    start_time = time()
+    logger.info(
+        '-------------------------- MERGE CSV(S) --------------------------')
+    logger.info('Input path: %s', input)
+    logger.info('Output path: %s', output)
+
+    # Check directories existence
+    if not os.path.isdir(input):
+        logger.error(
+            f'{input} is not a path. Please make sure the input is a directory!')
+        exit(1)
+
+    if not os.path.exists(input):
+        logger.error(
+            f'Path {input} does not exist. Please make sure the path is correct!')
+        exit(1)
+
+    if not os.path.exists(output):
+        os.makedirs(output)
+
+    # Get all csv files recursively
+    csv_files = glob.glob(os.path.join(input, "**/*.csv"), recursive=True)
+
+    try:
+        # Get all appended dataframes, and file amount to be logged 
+        dfs, _files_to_process, _error_files = merge_csv_files(csv_files)
+        # Concatenate all DataFrames into a single DataFrame
+        merged_data = pd.concat(dfs, ignore_index=True)
+        # Path and filename for the merged CSV file
+        now = datetime.now()
+        formatted_time = now.strftime("%Y-%m-%d_%H%Mh")
+
+        output_file = os.path.join(output, f'./{formatted_time}_merged.csv')
+        # Save the merged_data DataFrame to a CSV file
+        merged_data.to_csv(output_file, index=False)
+
+        _reordered_files = _files_to_process - _error_files
+        _percentage_success = (_reordered_files / _files_to_process) * 100
+        
+        # logs
+        logger.info('Successfully merged csv files')
+        logger.info(
+            f'Total files merged:  {_reordered_files}/{_files_to_process} => {_percentage_success} % success!')
+
+        logger.info('Total execution time: %f seconds', time() - start_time)
+
+
+    except Exception as e:
+        logger.error(f'An error has been detected while finalizing merged csv.\n Please check the following error: {e}')
+        exit(1)
+
 main.add_command(reorder_columns)
 main.add_command(rename)
 main.add_command(timestamp_estimate)
 main.add_command(sub_rename)
 main.add_command(preparation_steps)
+main.add_command(merge_csv)
 
 if __name__ == '__main__':
     main()
```

### Comparing `nhp-prep-0.3.3/app/column_mapper.py` & `nhp-prep-0.4.0/app/column_mapper.py`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.3/app/config/columns__std_format.csv` & `nhp-prep-0.4.0/app/config/columns__std_format.csv`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.3/app/config/logs.yaml` & `nhp-prep-0.4.0/app/config/logs.yaml`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.3/app/rename_files.py` & `nhp-prep-0.4.0/app/rename_files.py`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.3/app/subject_changer.py` & `nhp-prep-0.4.0/app/subject_changer.py`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.3/app/timestamp_estimator.py` & `nhp-prep-0.4.0/app/timestamp_estimator.py`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.3/app/util/rough_estimate_std_files.py` & `nhp-prep-0.4.0/app/util/rough_estimate_std_files.py`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.3/nhp_prep.egg-info/PKG-INFO` & `nhp-prep-0.4.0/nhp_prep.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhp-prep
-Version: 0.3.3
+Version: 0.4.0
 Summary: Pre-processing data tool for NHP Lab @ CMU
 Home-page: https://caoslab.psy.cmu.edu:32443/monkeylab/preprocessing-scripts
 Author: Hugo Angulo, Zijun Zhao
 Author-email: hugoanda@andrew.cmu.edu, zijunzha@andrew.cmu.edu
 License: MIT
 Keywords: nhp-prep,caoslab,cmu,pre-processing
 Classifier: Development Status :: 5 - Production/Stable
@@ -96,14 +96,19 @@
 
 4. Renaming of Subject according to logs file (needs the file) (`sub-rename`)
 
 ```
 nhp-prep sub-rename -r <file_with_columns_and_reference_subject_names> -i <directory_with_files_OR_unique_CSV_file> -o <output_directory>
 ```
 
+5. Merge multiple CSV files into a single file. The input should be a directory and so is the output
+```
+nhp-prep merge-csv -i <directory_with_files_OR_unique_CSV_file> -o <output_directory>
+```
+
 You could also run `nhp-prep --help` to see the available commands and their corresponding usage.
 
 If you want to know all the options available for an specific command, run the following:
 
 ```
 nhp-prep COMMAND --help
 ```
```

### Comparing `nhp-prep-0.3.3/setup.py` & `nhp-prep-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='nhp-prep',
-    version='0.3.3',
+    version='0.4.0',
     author='Hugo Angulo, Zijun Zhao',
     author_email='hugoanda@andrew.cmu.edu, zijunzha@andrew.cmu.edu',
     license='MIT',
     description='Pre-processing data tool for NHP Lab @ CMU',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://caoslab.psy.cmu.edu:32443/monkeylab/preprocessing-scripts',
```

