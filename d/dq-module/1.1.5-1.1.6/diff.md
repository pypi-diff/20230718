# Comparing `tmp/dq_module-1.1.5.tar.gz` & `tmp/dq_module-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dq_module-1.1.5.tar", last modified: Wed Jul 12 14:02:49 2023, max compression
+gzip compressed data, was "dist/dq_module-1.1.6.tar", last modified: Tue Jul 18 12:53:37 2023, max compression
```

## Comparing `dq_module-1.1.5.tar` & `dq_module-1.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:02:49.000000 dq_module-1.1.5/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-07-12 14:02:49.000000 dq_module-1.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11346 2023-07-12 14:02:39.000000 dq_module-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:02:49.000000 dq_module-1.1.5/dataqualitycheck/
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10482 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/consistencycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    37781 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/dataprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:02:49.000000 dq_module-1.1.5/dataqualitycheck/datasources/
--rw-rw-rw-   0 root         (0) root         (0)     7917 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/azureblobdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5534 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/databricksfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/databrickssqldf.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/localfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     5366 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/enumfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    42396 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheckpolars.py
--rw-rw-rw-   0 root         (0) root         (0)    50981 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheckspark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:02:49.000000 dq_module-1.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-12 14:02:39.000000 dq_module-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:53:37.000000 dq_module-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-07-18 12:53:37.000000 dq_module-1.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11346 2023-07-18 12:53:23.000000 dq_module-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:53:37.000000 dq_module-1.1.6/dataqualitycheck/
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10482 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/consistencycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    37781 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/dataprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:53:37.000000 dq_module-1.1.6/dataqualitycheck/datasources/
+-rw-rw-rw-   0 root         (0) root         (0)     7917 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/datasources/azureblobdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/datasources/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5534 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/datasources/databricksfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/datasources/databrickssqldf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/datasources/localfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5366 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/enumfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/singledatasetqualitycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    42396 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/singledatasetqualitycheckpolars.py
+-rw-rw-rw-   0 root         (0) root         (0)    51653 2023-07-18 12:53:23.000000 dq_module-1.1.6/dataqualitycheck/singledatasetqualitycheckspark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:53:37.000000 dq_module-1.1.6/dq_module.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-07-18 12:53:37.000000 dq_module-1.1.6/dq_module.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-07-18 12:53:37.000000 dq_module-1.1.6/dq_module.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 12:53:37.000000 dq_module-1.1.6/dq_module.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-18 12:53:37.000000 dq_module-1.1.6/dq_module.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-18 12:53:37.000000 dq_module-1.1.6/dq_module.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 12:53:37.000000 dq_module-1.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-18 12:53:23.000000 dq_module-1.1.6/setup.py
```

### Comparing `dq_module-1.1.5/PKG-INFO` & `dq_module-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_module
-Version: 1.1.5
+Version: 1.1.6
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.5/README.md` & `dq_module-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/commonutilities.py` & `dq_module-1.1.6/dataqualitycheck/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/consistencycheck.py` & `dq_module-1.1.6/dataqualitycheck/consistencycheck.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/dataprofile.py` & `dq_module-1.1.6/dataqualitycheck/dataprofile.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/datasources/azureblobdf.py` & `dq_module-1.1.6/dataqualitycheck/datasources/azureblobdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/datasources/commonutilities.py` & `dq_module-1.1.6/dataqualitycheck/datasources/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/datasources/databricksfilesystemdf.py` & `dq_module-1.1.6/dataqualitycheck/datasources/databricksfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/datasources/databrickssqldf.py` & `dq_module-1.1.6/dataqualitycheck/datasources/databrickssqldf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/datasources/localfilesystemdf.py` & `dq_module-1.1.6/dataqualitycheck/datasources/localfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/enumfile.py` & `dq_module-1.1.6/dataqualitycheck/enumfile.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheck.py` & `dq_module-1.1.6/dataqualitycheck/singledatasetqualitycheck.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheckpolars.py` & `dq_module-1.1.6/dataqualitycheck/singledatasetqualitycheckpolars.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheckspark.py` & `dq_module-1.1.6/dataqualitycheck/singledatasetqualitycheckspark.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 schema_enforce_structure(column_names, ",".join(['str']*len(column_names.split(','))))))
             total_records_df = total_records_df.dropDuplicates(total_records_df.columns)
         except Exception as e:
             raise Exception(e)
         return total_records_df
     
     def null_check_V1(self,df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         columnList = list(rule["column_to_be_checked"].split(","))
 
         result = self.spark.createDataFrame([], df.schema)
         column_passed = []
         column_failed = []
@@ -124,15 +124,15 @@
      
         failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if column have any null value.
     def null_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(col(rule["column_to_be_checked"]).isNull())
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
             test_status = "PASS"
@@ -144,15 +144,15 @@
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
        # ----- Function to check if all the required columns exist.
 
     def schema_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         date_col_config = eval(
             rule["date_column_config"]) if rule["date_column_config"] and rule["date_column_config"] != 'null' else {}
         total_row_count = df.count()
         failed_records_count = 0
         failed_records_write_location = 'N/A'
         reason = ''
@@ -241,15 +241,15 @@
             failed_df = df.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit("All columns")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag, False)
         return data_quality_test_summary_tuple(self.job_id, rule, test_status + reason, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     def range_min_check_V1(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         columnList = list(rule["column_to_be_checked"].split(","))
         valueList = list(rule["value"].split(','))
 
         if len(columnList)==len(valueList):
             combined_list = zip(columnList,valueList)
@@ -285,15 +285,15 @@
         failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if values not be less than the given value
 
     def range_min_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         df = df.filter(col(rule["column_to_be_checked"]).isNotNull())
         result = df.filter(
             col(rule["column_to_be_checked"]) < float(rule["value"]))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
@@ -306,15 +306,15 @@
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
   #  # ----- Function to check if values should not be less than or equal to the required value
   #  def range_min_inclusive_check(self, df, rule, write_failed_records_flag):
-  #     run_date = date.today().strftime("%Y/%m/%d")
+  #     run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
   #      start = time.time()
   #     total_row_count = df.count()
   #     df = df.filter(col(rule["column_to_be_checked"]).isNotNull())
   #     result = df.filter(
   #          col(rule["column_to_be_checked"]) <= float(rule["value"]))
   #      failed_records_count = result.count()
   #      failed_records_write_location = 'N/A'
@@ -325,15 +325,15 @@
   #          failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
   #             .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
   #         failed_records_write_location = self.write_failed_records(
   #             rule, failed_df, write_failed_records_flag)
   #
   #      return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
     def range_max_check_V1(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         columnList = list(rule["column_to_be_checked"].split(","))
         valueList = list(rule["value"].split(','))
 
         if len(columnList)==len(valueList):
             combined_list = zip(columnList,valueList)
@@ -367,15 +367,15 @@
         failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"])).withColumn("Column_Tested", lit(rule["column_to_be_checked"])).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
     
         failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
     # ----- Function to check if values should not be greater then the given value
     def range_max_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         df = df.filter(col(rule["column_to_be_checked"]).isNotNull())
         result = df.filter(
             col(rule["column_to_be_checked"]) > float(rule["value"]))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
@@ -387,15 +387,15 @@
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
     
     def length_check_V1(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         columnList = list(rule["column_to_be_checked"].split(","))
         valueList = list(rule["value"].split(','))
 
         if len(columnList)==len(valueList):
             combined_list = zip(columnList,valueList)
@@ -431,15 +431,15 @@
         failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
     
     
     # ----- Function to check if the values in the column have given length or not.
     def length_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             length(col(rule["column_to_be_checked"])) > int(rule["value"]))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
@@ -451,15 +451,15 @@
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if all the records are unique or not in the table.
     def unique_records_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         columnList = df.columns
         d = df.groupBy(columnList).count().filter(
             col("count") == 1).drop("count")
         result = df.exceptAll(d)
         failed_records_count = result.count()
@@ -473,15 +473,15 @@
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag, False)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date, False, ",".join(df.columns))
 
     # ----- Function to check if all the records are unique for all given input columns.It takes a list of columns as an arguement
     def unique_keys_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         columnList = list(rule["column_to_be_checked"].split(","))
         d = df.groupBy(columnList).count().filter(col("count") > 1).drop("count")
         d= d.withColumn("concat_col", concat_ws("//", *columnList))
         df1 = df.withColumn("concat_col", concat_ws("//", *columnList))
         result = df1.join(d, on="concat_col", how='leftsemi').select(df.columns)
@@ -496,15 +496,15 @@
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function takes a list of allowed values for a particular column and check if the values of the column belongs to that list or not.
     def allowed_values_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(~col(rule["column_to_be_checked"]).isin(
             rule["value"].strip().split(',')) | col(rule["column_to_be_checked"]).isNull())
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
@@ -515,15 +515,15 @@
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
     
     def min_length_check_V1(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         columnList = list(rule["column_to_be_checked"].split(","))
         valueList = list(rule["value"].split(','))
 
         if len(columnList)==len(valueList):
             combined_list = zip(columnList,valueList)
@@ -558,15 +558,15 @@
     
         failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
     
     # ----- Function to check that if the values in the column has the required minimum length or not.
     def min_length_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             length(col(rule["column_to_be_checked"])) < int(rule["value"]))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
@@ -578,15 +578,15 @@
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check that the table has required column count or not.
     def column_count_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         total_col_count = len(df.columns)
         failed_records_count = total_col_count - int(rule["value"])
         failed_records_write_location = 'N/A'
         if total_col_count == int(rule["value"]):
             test_status = "PASS"
@@ -599,15 +599,15 @@
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag, False)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function takes a list of not allowed values for a particular column and check if the column has not allowed values or not.
     def not_allowed_values_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             col(rule["column_to_be_checked"]).isin(rule["value"].strip().split(',')))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         if failed_records_count == 0:
@@ -619,15 +619,15 @@
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if the date lies in the given range or not.
     def date_range_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         value = eval(rule["value"]) 
         date_column_config = eval(rule["date_column_config"])
         
         min_value= parse( value["min_value"] )
         max_value= parse( value["max_value"] )
@@ -657,15 +657,15 @@
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     # ----- Function to check if the given column matches the given regex pattern or not.
     def regex_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             ~col(rule["column_to_be_checked"]).rlike(rule["value"]))
         failed_records_count = result.count()
         failed_records_write_location = 'N/A'
         test_status = "PASS" if failed_records_count == 0 else "FAIL"
@@ -675,15 +675,15 @@
                 f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
     def row_count_check(self, df, rule, write_failed_records_flag):
-        run_date = date.today().strftime("%Y/%m/%d")
+        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
         start = time.time()
         total_row_count = df.count()
         failed_records_write_location = 'N/A'
         failed_records_count = total_row_count - int(rule["value"])
         if total_row_count == int(rule["value"]):
             test_status = "PASS"
         else:
@@ -724,21 +724,21 @@
     def df_rules_validation(self, rule_set, write_summary_on_database, failed_schema_source_list, result_summary_folder_path, write_failed_records_flag):
         test_summary = []
         try:
             for rule in rule_set:
                 try:
                     source = f'''{rule["source_type"]}_{rule["layer"]}_{rule["source_name"]}_{rule["filename"]}'''
                     if "failed_schema_source_list" in rule and rule['failed_schema_source_list'] in failed_schema_source_list:
-                        run_date = date.today().strftime("%Y/%m/%d")
+                        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
                         test_summary.append(data_quality_test_summary_tuple(
                             self.job_id, rule, "schema check fail", "", "", "", 0, run_date, modify_active=True))
                         continue
 
                     if 'active' in rule and int(rule['active']) == 0:
-                        run_date = date.today().strftime("%Y/%m/%d")
+                        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
                         test_summary.append(data_quality_test_summary_tuple(
                             self.job_id, rule, "", "", "", "", 0, run_date))
                         continue
 
                     if rule["rule_name"] == "null_check" and len(list(rule["column_to_be_checked"].split(",")))==1:
                         result_df = self.null_check(
                             self.dataframes[source], rule, write_failed_records_flag)
@@ -827,20 +827,20 @@
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "row_count_check":
                         result_df = self.row_count_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
 
                     else:
-                        run_date = date.today().strftime("%Y/%m/%d")
+                        run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
                         test_summary.append(data_quality_test_summary_tuple(
                             self.job_id, rule, "invalid rule name", "", "", "", 0, run_date))
                         continue
                 except Exception as e:
-                    run_date = date.today().strftime("%Y/%m/%d")
+                    run_date = datetime.now(tz=self.time_zone).strftime("%d/%m/%Y_%H:%M:%S")
                     test_summary.append(data_quality_test_summary_tuple(
                         self.job_id, rule, f"Exception :: {e}", "", "", "", 0, run_date))
                     continue
 
             summary_df = data_check_summarization_spark_df(
                 self.spark, test_summary)
             if write_summary_on_database and self.data_right_structure == 'file':
```

### Comparing `dq_module-1.1.5/dq_module.egg-info/PKG-INFO` & `dq_module-1.1.6/dq_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq-module
-Version: 1.1.5
+Version: 1.1.6
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.5/dq_module.egg-info/SOURCES.txt` & `dq_module-1.1.6/dq_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.5/setup.py` & `dq_module-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # COMMAND ----------
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read() 
     
 setuptools.setup(
     name="dq_module",
-    version="1.1.5",
+    version="1.1.6",
     author="Sweta",
     author_email="sweta.swami@decisionpoint.in",
     description="data profiling and basic data quality rules check",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # packages=setuptools.find_packages(include=['*']),
     packages=['dataqualitycheck', 'dataqualitycheck.datasources'],
```

