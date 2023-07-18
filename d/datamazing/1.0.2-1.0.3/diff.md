# Comparing `tmp/datamazing-1.0.2.tar.gz` & `tmp/datamazing-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-1.0.2.tar", max compression
+gzip compressed data, was "datamazing-1.0.3.tar", max compression
```

## Comparing `datamazing-1.0.2.tar` & `datamazing-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       21 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/__init__.py
--rw-r--r--   0        0        0      277 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/_conform.py
--rw-r--r--   0        0        0      295 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      267 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0      126 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      766 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     3818 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0      649 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     3353 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0      868 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      660 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pandas/types.py
--rw-r--r--   0        0        0      184 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/__init__.py
--rw-r--r--   0        0        0       92 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/testing/__init__.py
--rw-r--r--   0        0        0      295 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/testing/assertions.py
--rw-r--r--   0        0        0     2064 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/transformations/__init__.py
--rw-r--r--   0        0        0     3008 2023-07-17 11:54:32.142460 datamazing-1.0.2/datamazing/pyspark/transformations/grouping.py
--rw-r--r--   0        0        0      708 2023-07-17 11:54:32.142460 datamazing-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-07-18 07:44:09.104518 datamazing-1.0.3/datamazing/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-18 07:44:09.104518 datamazing-1.0.3/datamazing/_conform.py
+-rw-r--r--   0        0        0      295 2023-07-18 07:44:09.104518 datamazing-1.0.3/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      267 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     3818 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     3497 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0     1012 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      660 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2064 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0     3058 2023-07-18 07:44:09.108518 datamazing-1.0.3/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      708 2023-07-18 07:44:09.108518 datamazing-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-1.0.3/PKG-INFO
```

### Comparing `datamazing-1.0.2/datamazing/pandas/testing/assertions.py` & `datamazing-1.0.3/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.2/datamazing/pandas/testing/data.py` & `datamazing-1.0.3/datamazing/pandas/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.2/datamazing/pandas/transformations/basic.py` & `datamazing-1.0.3/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.2/datamazing/pandas/transformations/grouping.py` & `datamazing-1.0.3/datamazing/pandas/transformations/grouping.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import pandas as pd
 
 from datamazing._conform import _concat, _list
 
 
 class GrouperResampler:
-    def __init__(self, gb: "Grouper", on: str, resolution: pd.Timedelta):
+    def __init__(
+        self,
+        gb: "Grouper",
+        on: str,
+        resolution: pd.Timedelta,
+        edge: str,
+    ):
         self.gb = gb
         self.on = on
         self.resolution = resolution
+        self.edge = edge
 
     def agg(self, method: str):
         start_time = self.gb.df[self.on].min()
         end_time = self.gb.df[self.on].max()
 
         if method == "interpolate":
             aggregate_options = {"limit_area": "inside"}
         else:
             aggregate_options = {}
 
         df = self.gb.df.set_index(self.on)
 
         df = (
             df.groupby(self.gb.by, dropna=False)
-            .resample(rule=self.resolution)
+            .resample(rule=self.resolution, closed=self.edge, label=self.edge)
             .aggregate(method, **aggregate_options)
         )
 
         # depending on the resampling aggregation
         # method, pandas will include the group-by
         # columns in both the index and the columns
         df = df.drop(columns=self.gb.by, errors="ignore")
@@ -50,16 +57,16 @@
         return (
             self.df.set_index(self.by)
             .groupby(self.by, dropna=False)
             .aggregate(method)
             .reset_index()
         )
 
-    def resample(self, on: str, resolution: pd.Timedelta):
-        return GrouperResampler(self, on, resolution)
+    def resample(self, on: str, resolution: pd.Timedelta, edge: str = "left"):
+        return GrouperResampler(self, on, resolution, edge)
 
     def pivot(self, on: list[str], values: list[tuple[str]] = None):
         """
         Pivot table. Non-existing combinations will be filled
         with NaNs.
 
         Args:
```

### Comparing `datamazing-1.0.2/datamazing/pandas/types.py` & `datamazing-1.0.3/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.2/datamazing/pyspark/testing/data.py` & `datamazing-1.0.3/datamazing/pyspark/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-1.0.2/datamazing/pyspark/transformations/grouping.py` & `datamazing-1.0.3/datamazing/pyspark/transformations/grouping.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import pyspark.sql.functions as f
 
 from datamazing._conform import _concat, _list
 
 
 class GrouperResampler:
     def __init__(
-        self, gb: "Grouper", on: str, resolution: pd.Timedelta, edge: str = "left"
+        self,
+        gb: "Grouper",
+        on: str,
+        resolution: pd.Timedelta,
+        edge: str,
     ):
         self.gb = gb
         self.on = on
         self.resolution = resolution
         self.edge = edge
 
     def agg(self, method: str):
@@ -53,16 +57,16 @@
         version_window = ps.Window.partitionBy(self.by).orderBy(f.desc(on))
         return (
             self.df.withColumn("__version", f.row_number().over(version_window))
             .filter(f.col("__version") == 1)
             .drop("__version")
         )
 
-    def resample(self, on: str, resolution: pd.Timedelta):
-        return GrouperResampler(self, on, resolution)
+    def resample(self, on: str, resolution: pd.Timedelta, edge: str = "left"):
+        return GrouperResampler(self, on, resolution, edge)
 
     def pivot(self, on: list[str], values: list[tuple[str]] = None):
         """
         Pivot table. Non-existing combinations will be filled
         with NaNs.
 
         Args:
```

### Comparing `datamazing-1.0.2/pyproject.toml` & `datamazing-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "1.0.2"
+version = "1.0.3"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `datamazing-1.0.2/PKG-INFO` & `datamazing-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamazing
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for working with pandas Dataset, but wit specialized functions used for Energinet
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

