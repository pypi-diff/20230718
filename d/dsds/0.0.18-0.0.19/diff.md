# Comparing `tmp/dsds-0.0.18.tar.gz` & `tmp/dsds-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsds-0.0.18.tar", last modified: Sun Jul 16 03:54:37 2023, max compression
+gzip compressed data, was "dsds-0.0.19.tar", last modified: Tue Jul 18 15:30:52 2023, max compression
```

## Comparing `dsds-0.0.18.tar` & `dsds-0.0.19.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 03:54:37.198434 dsds-0.0.18/
--rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.18/LICENSE
--rw-rw-rw-   0        0        0     6759 2023-07-16 03:54:37.198434 dsds-0.0.18/PKG-INFO
--rw-rw-rw-   0        0        0     4387 2023-07-11 16:38:19.000000 dsds-0.0.18/README.md
--rw-rw-rw-   0        0        0     1398 2023-07-16 03:51:44.000000 dsds-0.0.18/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-16 03:54:37.199434 dsds-0.0.18/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 03:54:37.161425 dsds-0.0.18/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 03:54:37.176429 dsds-0.0.18/src/dsds/
--rw-rw-rw-   0        0        0       87 2023-07-16 03:36:00.000000 dsds-0.0.18/src/dsds/__init__.py
--rw-rw-rw-   0        0        0     6875 2023-07-13 01:01:02.000000 dsds-0.0.18/src/dsds/blueprint.py
--rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.18/src/dsds/eda_text.py
--rw-rw-rw-   0        0        0    32902 2023-07-16 03:51:24.000000 dsds-0.0.18/src/dsds/fs.py
--rw-rw-rw-   0        0        0     9077 2023-07-13 03:33:56.000000 dsds-0.0.18/src/dsds/metrics.py
--rw-rw-rw-   0        0        0    29200 2023-07-14 19:43:13.000000 dsds-0.0.18/src/dsds/prescreen.py
--rw-rw-rw-   0        0        0    15707 2023-07-14 17:19:08.000000 dsds-0.0.18/src/dsds/sample.py
--rw-rw-rw-   0        0        0    43353 2023-07-15 03:30:38.000000 dsds-0.0.18/src/dsds/transform.py
--rw-rw-rw-   0        0        0     2686 2023-07-14 19:40:24.000000 dsds-0.0.18/src/dsds/type_alias.py
--rw-rw-rw-   0        0        0     2085 2023-07-09 00:29:00.000000 dsds-0.0.18/src/dsds/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 03:54:37.197433 dsds-0.0.18/src/dsds.egg-info/
--rw-rw-rw-   0        0        0     6759 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-16 03:54:37.000000 dsds-0.0.18/src/dsds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 15:30:52.109959 dsds-0.0.19/
+-rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.19/LICENSE
+-rw-rw-rw-   0        0        0     6759 2023-07-18 15:30:52.109959 dsds-0.0.19/PKG-INFO
+-rw-rw-rw-   0        0        0     4387 2023-07-11 16:38:19.000000 dsds-0.0.19/README.md
+-rw-rw-rw-   0        0        0     1398 2023-07-18 15:30:24.000000 dsds-0.0.19/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 15:30:52.109959 dsds-0.0.19/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 15:30:52.078706 dsds-0.0.19/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 15:30:52.094333 dsds-0.0.19/src/dsds/
+-rw-rw-rw-   0        0        0       87 2023-07-18 15:28:07.000000 dsds-0.0.19/src/dsds/__init__.py
+-rw-rw-rw-   0        0        0     7692 2023-07-18 15:17:24.000000 dsds-0.0.19/src/dsds/blueprint.py
+-rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.19/src/dsds/eda_text.py
+-rw-rw-rw-   0        0        0    32902 2023-07-16 03:51:24.000000 dsds-0.0.19/src/dsds/fs.py
+-rw-rw-rw-   0        0        0     9077 2023-07-13 03:33:56.000000 dsds-0.0.19/src/dsds/metrics.py
+-rw-rw-rw-   0        0        0    30539 2023-07-18 15:20:27.000000 dsds-0.0.19/src/dsds/prescreen.py
+-rw-rw-rw-   0        0        0    15697 2023-07-16 03:59:12.000000 dsds-0.0.19/src/dsds/sample.py
+-rw-rw-rw-   0        0        0    44312 2023-07-18 15:26:06.000000 dsds-0.0.19/src/dsds/transform.py
+-rw-rw-rw-   0        0        0     2684 2023-07-16 04:01:32.000000 dsds-0.0.19/src/dsds/type_alias.py
+-rw-rw-rw-   0        0        0     2085 2023-07-09 00:29:00.000000 dsds-0.0.19/src/dsds/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:30:52.109959 dsds-0.0.19/src/dsds.egg-info/
+-rw-rw-rw-   0        0        0     6759 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/top_level.txt
```

### Comparing `dsds-0.0.18/LICENSE` & `dsds-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `dsds-0.0.18/PKG-INFO` & `dsds-0.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsds
-Version: 0.0.18
+Version: 0.0.19
 Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
 Author-email: Tianren Qin <tq9695@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 T.Q
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dsds-0.0.18/README.md` & `dsds-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `dsds-0.0.18/pyproject.toml` & `dsds-0.0.19/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "dsds"
-version = "0.0.18"
+version = "0.0.19"
 requires-python = ">=3.9"
 readme = "README.md"
 description = "A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe."
 authors = [
     {name = "Tianren Qin", email = "tq9695@gmail.com"}
 ]
 license = {file = "LICENSE"}
```

### Comparing `dsds-0.0.18/src/dsds/blueprint.py` & `dsds-0.0.19/src/dsds/blueprint.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pickle
 import polars as pl
 import importlib
+import polars.selectors as cs
 from pathlib import Path
 from polars import LazyFrame
 from dataclasses import dataclass
 from typing import (
     Any
     , Iterable
     , Optional
@@ -27,20 +28,20 @@
     ref: dict # The right table as a dictionary
     right_col: str
     default: Optional[Any]
 
 @dataclass
 class Step:
     action:ActionType
-    associated_data: Iterable[IntoExpr] | MapDict | list[str] | dict[str, Any] | pl.Expr
-    # First is everything that can be done with with_columns
-    # Second is a 1-to-1 encoder
-    # Third is a drop/select
-    # Fourth is apply_func
-    # Fifth is a filter statement
+    associated_data: Iterable[IntoExpr] | MapDict | list[str] | cs._selector_proxy_ | dict[str, Any] | pl.Expr
+    # First is everything that can be done with with_columns (Iterable[IntoExpr], but list[pl.Expr] is recommended)
+    # Second is a 1-to-1 encoder (MapDict)
+    # Third is a drop/select (list[str] and cs._selector_proxy_)
+    # Fourth is add_func (dict[str, Any])
+    # Fifth is a filter statement (pl.Expr)
 
 
 @pl.api.register_lazyframe_namespace("blueprint")
 class Blueprint:
     def __init__(self, ldf: LazyFrame):
         self._ldf = ldf
         self.steps:list[Step] = []
@@ -133,45 +134,61 @@
         output.blueprint.steps = self.steps.copy() 
         output.blueprint.steps.append(
             Step(action = "drop", associated_data = drop_cols)
         )
         return output
     
     # This doesn't work with the pipeline right now because it clears all steps before this.
-    def apply_func(self
+    def add_func(self
         , df:LazyFrame # The input to the function that needs to be persisted.
         , func:Callable[Concatenate[LazyFrame, P], LazyFrame]
         , kwargs:dict[str, Any]
     ) -> LazyFrame:
         # df: The input lazyframe to the function that needs to be persisted. We need this because:
         # When running the function, the reference to df might be changed, therefore losing the steps
 
         # When this is called, the actual function should be already applied.
         output = self._ldf # .lazy()
         output.blueprint.steps = df.blueprint.steps.copy() 
         output.blueprint.steps.append(
-            Step(action="apply_func", associated_data={"module":func.__module__, "name":func.__name__, "kwargs":kwargs})
+            Step(action="add_func", associated_data={"module":func.__module__, "name":func.__name__, "kwargs":kwargs})
         )
         return output
         
     def preserve(self, path:str|Path):
+        '''
+        Writes the blueprint to disk as a Python pickle file at the given path.
+        '''
         f = open(path, "wb")
         pickle.dump(self, f)
         f.close()
 
-    def apply(self, df:PolarsFrame) -> PolarsFrame:
-        for s in self.steps:
-            if s.action == "drop":
-                df = df.drop(s.associated_data)
-            elif s.action == "with_columns":
-                df = df.with_columns(s.associated_data)
-            elif s.action == "map_dict":
-                df = self._map_dict(df, s.associated_data)
-            elif s.action == "select":
-                df = df.select(s.associated_data)
-            elif s.action == "filter":
-                df = df.filter(s.associated_data)
-            elif s.action == "apply_func":
-                func = getattr(importlib.import_module(s.associated_data["module"]), s.associated_data["name"])
-                df = df.pipe(func, **s.associated_data["kwargs"])
-            
+    def apply(self, df:PolarsFrame, up_to:int=-1) -> PolarsFrame:
+        '''
+        Apply all the steps to the given df. The result will be lazy if df is lazy, and eager if df is eager.
+
+        Parameters
+        ----------
+        df
+            Either an eager or lazy Polars Dataframe
+        up_to
+            If > 0, will perform the steps up to this number
+        '''
+        _up_to = len(self.steps) if up_to <=0 else min(up_to, len(self.steps))
+        for i,s in enumerate(self.steps):
+            if i < _up_to:
+                if s.action == "drop":
+                    df = df.drop(s.associated_data)
+                elif s.action == "with_columns":
+                    df = df.with_columns(s.associated_data)
+                elif s.action == "map_dict":
+                    df = self._map_dict(df, s.associated_data)
+                elif s.action == "select":
+                    df = df.select(s.associated_data)
+                elif s.action == "filter":
+                    df = df.filter(s.associated_data)
+                elif s.action == "add_func":
+                    func = getattr(importlib.import_module(s.associated_data["module"]), s.associated_data["name"])
+                    df = df.pipe(func, **s.associated_data["kwargs"])
+            else:
+                break
         return df
```

### Comparing `dsds-0.0.18/src/dsds/eda_text.py` & `dsds-0.0.19/src/dsds/eda_text.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.18/src/dsds/fs.py` & `dsds-0.0.19/src/dsds/fs.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.18/src/dsds/metrics.py` & `dsds-0.0.19/src/dsds/metrics.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.18/src/dsds/prescreen.py` & `dsds-0.0.19/src/dsds/prescreen.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 from .sample import (
     lazy_sample
 )
 from .blueprint import(
     Blueprint
 )
-
+import re
 import polars.selectors as cs
 import polars as pl
 import logging  
 from datetime import datetime 
 from typing import Any, Optional, Tuple
 from itertools import combinations
 from scipy.stats import (
@@ -58,25 +58,63 @@
     '''Returns boolean columns.'''
     return df.select(cs.by_dtype(pl.Boolean)).columns
 
 def get_cols_regex(df:PolarsFrame, pattern:str) -> list[str]:
     '''Returns columns that have names matching the regex pattern.'''
     return df.select(cs.matches(pattern=pattern)).columns
 
-def lowercase_columns(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
+def lowercase(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
     '''
     Lowercases all column names.
 
     Set persist = True if this needs to be remembered by the blueprint.
     '''
     output = df.rename({c: c.lower() for c in df.columns})
     if isinstance(df, pl.LazyFrame) and persist:
-        return output.blueprint.apply_func(df, lowercase_columns, kwargs = {})
+        return output.blueprint.add_func(df, lowercase, kwargs = {})
     return output
 
+def rename(df:PolarsFrame, rename_dict:dict[str, str], persist:bool=False) -> PolarsFrame:
+    '''
+    A wrapper function for df.rename() so that it works with pipeline.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    output = df.rename(rename_dict)
+    if isinstance(df, pl.LazyFrame) and persist:
+        return output.blueprint.add_func(df, rename, kwargs = {"rename_dict", rename_dict})
+    return output
+
+def snake_case(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
+    '''
+    Turn all camel case column names into snake case.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    pat = re.compile(r"(?<!^)(?=[A-Z])")
+    return rename(df, {c: pat.sub('_', c).lower() for c in df.columns}, persist)
+
+def select(
+    df:PolarsFrame
+    , selector: list[str] | cs._selector_proxy_
+    , persist:bool=False
+) -> PolarsFrame:
+    '''
+    A select wrapper that makes it pipeline compatible
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    if cs.is_selector(selector):
+        if isinstance(df, pl.LazyFrame) and persist:
+            return df.blueprint.select(selector)
+        else:
+            return df.select(selector)
+    else:
+        raise TypeError("The selector is not a valid selector.")
+
 def drop_nulls(
     df:PolarsFrame
     , subset:Optional[list[str]] = None
     , persist:bool=False
 ) -> PolarsFrame:
     '''
     A wrapper function for Polars' drop_nulls so that it can be used in pipeline.
```

### Comparing `dsds-0.0.18/src/dsds/sample.py` & `dsds-0.0.19/src/dsds/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             raise ValueError("Sample amount must be > 0.")
         
         output = df.with_columns(pl.all().shuffle(seed=seed)).with_row_count()\
         .filter(pl.col("row_nr") < sample_amt)\
         .select(df.columns)
 
     if persist:
-        output = output.blueprint.apply_func(df, lazy_sample, kwargs = {"sample_frac":sample_frac
+        output = output.blueprint.add_func(df, lazy_sample, kwargs = {"sample_frac":sample_frac
                                                                         , "sample_amt":sample_amt, "seed":seed})
     return output
 
 def deduplicate(
     df: PolarsFrame
     , subset: list[str]
     , keep: UniqueKeepStrategy = "any"
@@ -80,15 +80,15 @@
     keep
         One of 'first', 'last', 'any', 'none'. Default is 'any', which is somewhat random.
     persist
         If true, this step will be kept in the blueprint
     '''
     output = df.unique(subset=subset, keep = keep)
     if isinstance(df, pl.LazyFrame) and persist:
-        return output.blueprint.apply_func(df, deduplicate, kwargs = {"subset":subset,"keep":keep})
+        return output.blueprint.add_func(df, deduplicate, kwargs = {"subset":subset,"keep":keep})
     return output
 
 def simple_upsample(
     df: PolarsFrame
     , subgroup: dict[str, list] | pl.Expr
     , count:int
     , epsilon: float = 1e-2
@@ -198,15 +198,15 @@
         # NaN occurs when we add null with a number. Leave it null.
         new_c = pl.Series(c, sub[c].to_numpy() + noise).fill_nan(None) 
         sub = sub.replace_at_idx(sub.find_idx_by_name(c), new_c)
 
     if isinstance(df, pl.LazyFrame):
         output = pl.concat([df, sub.lazy()])
         if persist:
-            output = output.blueprint.apply_func(df, simple_upsample, kwargs = {"subgroup":subgroup,"count":count
+            output = output.blueprint.add_func(df, simple_upsample, kwargs = {"subgroup":subgroup,"count":count
                                                                                 ,"epsilon":epsilon,"include":include
                                                                                 ,"exclude":exclude,"positive":positive
                                                                                 , "seed":seed})
         return output
     return pl.concat([df, sub])
 
 def simple_downsample(
@@ -251,15 +251,15 @@
     ).filter(
         (~pl.col("~!"))
         | (pl.int_range(0, pl.count()).over("~!").shuffle() < pl.count().over("~!").max() * sample_frac)
     ).select(df.columns)
 
     if isinstance(df, pl.LazyFrame):
         if persist:
-            output = output.blueprint.apply_func(df, simple_downsample
+            output = output.blueprint.add_func(df, simple_downsample
                                                 , kwargs={"subgroup":subgroup,"sample_frac":sample_frac})
         return output
     return output
 
 
 def stratified_downsample(
     df: PolarsFrame
@@ -301,15 +301,15 @@
     else:
         raise TypeError("The argument `keep` must either be a Python int or float.")
 
     output = df.filter(
         pl.int_range(0, pl.count(), dtype=pl.UInt64).shuffle().over(group) < rhs
     )
     if isinstance(df, pl.LazyFrame) and persist:
-        return output.blueprint.apply_func(df, stratified_downsample
+        return output.blueprint.add_func(df, stratified_downsample
                                         , kwargs={"group":group, "keep":keep, "min_keep":min_keep})
     return output
 
 def train_test_split(
     df: PolarsFrame
     , train_frac:float = 0.75
     , seed:int = 42
```

### Comparing `dsds-0.0.18/src/dsds/transform.py` & `dsds-0.0.19/src/dsds/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -712,63 +712,84 @@
         return df.blueprint.with_columns(exprs)
     return df.with_columns(exprs)
 
 def custom_binning(
     df:PolarsFrame
     , cols:list[str]
     , cuts:list[float]
+    , suffix:str = ""
 ) -> PolarsFrame:
     '''
     Bins according to the cuts provided. The same cuts will be applied to all columns in cols.
 
     This will be remembered by blueprint by default.
 
     Parameters
     ----------
     df
         Either a lazy or eager Polars DataFrame
     cols
-        Numerical columns that will be replaced by the bins
+        Numerical columns that will be binned
     cuts
         A list of floats representing break points in the intervals
+    suffix
+        If you don't want to replace the original columns, you have the option to give the binned column a suffix
     '''
     if isinstance(df, pl.LazyFrame):
         exprs = [
-            pl.col(c).cut(cuts).cast(pl.Utf8) for c in cols
+            pl.col(c).cut(cuts).cast(pl.Utf8).suffix(suffix) for c in cols
         ]
         return df.blueprint.with_columns(exprs)
     else:
         return df.with_columns(
-            pl.col(c).cut(cuts).cast(pl.Utf8) for c in cols
+            pl.col(c).cut(cuts).cast(pl.Utf8).suffix(suffix) for c in cols
         )
     
 def fixed_sized_binning(
     df:PolarsFrame
     , cols:list[str]
     , interval: float
+    , suffix:str = ""
 ) -> PolarsFrame:
-    
+    '''
+    Bins according to fixed interval size. The same cuts will be applied to all columns in cols. Bin will 
+    start from min(feature) to max(feature) + interval with step length = interval.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        Numerical columns that will be binned
+    interval
+        The fixed sized interval
+    suffix
+        If you don't want to replace the original columns, you have the option to give the binned column a suffix
+    '''
     bounds = df.lazy().select(cols).select(
         pl.all().min().prefix("min:")
         , pl.all().max().prefix("max:")
     ).collect().row(0)
     exprs = []
     n = len(cols)
     for i, c in enumerate(cols):
         cut = np.arange(bounds[i], bounds[n+i] + interval, step=interval).tolist()
-        exprs.append(pl.col(c).cut(cut).cast(pl.Utf8).alias(c))
+        exprs.append(pl.col(c).cut(cut).cast(pl.Utf8).suffix(suffix))
 
     if isinstance(df, pl.LazyFrame):
         return df.blueprint.with_columns(exprs)
     return df.with_columns(exprs)
 
 def quantile_binning(
     df:PolarsFrame
     , cols:list[str]
     , n_bins:int
+    , suffix:str = ""
 ) -> PolarsFrame:
     '''
     Bin a continuous variable into categories, based on quantile. Null values will be its own category. The same binning
     rule will be applied to all columns in cols. If you want different n_bins for different columns, chain another 
     quantile_binning with different cols and n_bins.
 
     This will be remembered by blueprint by default.
@@ -780,14 +801,16 @@
     cols
         A list of numeric columns. This has to be supplied by the user because it is not recommended
         to bin all numerical variables
     n_bins
         The number of desired bins. If n_bins = 4, the quantile cuts will be [0.25,0.5,0.74], and 4 
         categories will be created, which represent values ranging from (-inf, 0.25 quantile value],
         (0.25 quantile value, 0.5 quantile value],...(0.75 quantile value, inf]
+    suffix
+        If you don't want to replace the original columns, you have the option to give the binned column a suffix
 
     Example
     -------
     >>> df = pl.DataFrame({
     ...     "a":range(5)
     ... })
     >>> df
@@ -821,20 +844,20 @@
     qcuts = np.arange(start=1/n_bins, stop=1.0, step = 1/n_bins)
     if isinstance(df, pl.LazyFrame):
         cuts = df.select(cols).select(
             pl.all().qcut(qcuts).unique().cast(pl.Utf8).str.extract(r"\((.*?),")
             .cast(pl.Float64).sort().tail(len(qcuts))
         ).collect()
         exprs = [
-            pl.col(c).cut(cuts.drop_in_place(c).to_list()).cast(pl.Utf8) for c in cols
+            pl.col(c).cut(cuts.drop_in_place(c).to_list()).cast(pl.Utf8).suffix(suffix) for c in cols
         ]
         return df.blueprint.with_columns(exprs)
     else: # Eager frame
         return df.with_columns(
-            pl.col(c).qcut(qcuts).cast(pl.Utf8) for c in cols 
+            pl.col(c).qcut(qcuts).cast(pl.Utf8).suffix(suffix) for c in cols 
         )
 
 def woe_cat_encode(
     df:PolarsFrame
     , target:str
     , cols:Optional[list[str]]=None
     , min_count:float = 1.
```

### Comparing `dsds-0.0.18/src/dsds/type_alias.py` & `dsds-0.0.19/src/dsds/type_alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 P = ParamSpec('P')
 CPU_COUNT:Final[int] = os.cpu_count()
 POLARS_NUMERICAL_TYPES:Final[Tuple[pl.DataType]] = (pl.UInt8, pl.UInt16, pl.UInt32, pl.UInt64, pl.Float32, pl.Float64, pl.Int8, pl.Int16, pl.Int32, pl.Int64)  # noqa: E501
 POLARS_DATETIME_TYPES:Final[Tuple[pl.DataType]] = (pl.Datetime, pl.Date)
 
 PolarsFrame:TypeAlias = pl.DataFrame | pl.LazyFrame
 PipeFunction = Callable[Concatenate[PolarsFrame, P], PolarsFrame]
-ActionType = Literal["with_columns", "map_dict", "drop", "select", "apply_func", "filter"]
+ActionType = Literal["with_columns", "map_dict", "drop", "select", "add_func", "filter"]
 MRMRStrategy = Literal["fscore", "f", "f_score", "xgb", "xgboost", "rf", "random_forest", "mis"
                        , "mutual_info_score", "lgbm", "lightgbm"]
 ScalingStrategy = Literal["standard", "min_max", "const", "constant"]
 ImputationStrategy = Literal["mean", "avg", "average", "median", "const", "constant", "mode", "most_frequent"]
 PowerTransformStrategy = Literal["yeo_johnson", "yeojohnson", "box_cox", "boxcox"]
 KSAlternatives = Literal["two-sided", "greater", "less"]
```

### Comparing `dsds-0.0.18/src/dsds/utils.py` & `dsds-0.0.19/src/dsds/utils.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.18/src/dsds.egg-info/PKG-INFO` & `dsds-0.0.19/src/dsds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsds
-Version: 0.0.18
+Version: 0.0.19
 Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
 Author-email: Tianren Qin <tq9695@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 T.Q
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

