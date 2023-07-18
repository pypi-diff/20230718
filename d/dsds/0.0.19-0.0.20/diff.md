# Comparing `tmp/dsds-0.0.19.tar.gz` & `tmp/dsds-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsds-0.0.19.tar", last modified: Tue Jul 18 15:30:52 2023, max compression
+gzip compressed data, was "dsds-0.0.20.tar", last modified: Tue Jul 18 15:56:19 2023, max compression
```

## Comparing `dsds-0.0.19.tar` & `dsds-0.0.20.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 15:30:52.109959 dsds-0.0.19/
--rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.19/LICENSE
--rw-rw-rw-   0        0        0     6759 2023-07-18 15:30:52.109959 dsds-0.0.19/PKG-INFO
--rw-rw-rw-   0        0        0     4387 2023-07-11 16:38:19.000000 dsds-0.0.19/README.md
--rw-rw-rw-   0        0        0     1398 2023-07-18 15:30:24.000000 dsds-0.0.19/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 15:30:52.109959 dsds-0.0.19/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 15:30:52.078706 dsds-0.0.19/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 15:30:52.094333 dsds-0.0.19/src/dsds/
--rw-rw-rw-   0        0        0       87 2023-07-18 15:28:07.000000 dsds-0.0.19/src/dsds/__init__.py
--rw-rw-rw-   0        0        0     7692 2023-07-18 15:17:24.000000 dsds-0.0.19/src/dsds/blueprint.py
--rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.19/src/dsds/eda_text.py
--rw-rw-rw-   0        0        0    32902 2023-07-16 03:51:24.000000 dsds-0.0.19/src/dsds/fs.py
--rw-rw-rw-   0        0        0     9077 2023-07-13 03:33:56.000000 dsds-0.0.19/src/dsds/metrics.py
--rw-rw-rw-   0        0        0    30539 2023-07-18 15:20:27.000000 dsds-0.0.19/src/dsds/prescreen.py
--rw-rw-rw-   0        0        0    15697 2023-07-16 03:59:12.000000 dsds-0.0.19/src/dsds/sample.py
--rw-rw-rw-   0        0        0    44312 2023-07-18 15:26:06.000000 dsds-0.0.19/src/dsds/transform.py
--rw-rw-rw-   0        0        0     2684 2023-07-16 04:01:32.000000 dsds-0.0.19/src/dsds/type_alias.py
--rw-rw-rw-   0        0        0     2085 2023-07-09 00:29:00.000000 dsds-0.0.19/src/dsds/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 15:30:52.109959 dsds-0.0.19/src/dsds.egg-info/
--rw-rw-rw-   0        0        0     6759 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-18 15:30:52.000000 dsds-0.0.19/src/dsds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 15:56:19.311994 dsds-0.0.20/
+-rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.20/LICENSE
+-rw-rw-rw-   0        0        0     6759 2023-07-18 15:56:19.311994 dsds-0.0.20/PKG-INFO
+-rw-rw-rw-   0        0        0     4387 2023-07-11 16:38:19.000000 dsds-0.0.20/README.md
+-rw-rw-rw-   0        0        0     1398 2023-07-18 15:55:37.000000 dsds-0.0.20/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 15:56:19.311994 dsds-0.0.20/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 15:56:19.263303 dsds-0.0.20/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 15:56:19.296366 dsds-0.0.20/src/dsds/
+-rw-rw-rw-   0        0        0       87 2023-07-18 15:55:42.000000 dsds-0.0.20/src/dsds/__init__.py
+-rw-rw-rw-   0        0        0     7663 2023-07-18 15:54:32.000000 dsds-0.0.20/src/dsds/blueprint.py
+-rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.20/src/dsds/eda_text.py
+-rw-rw-rw-   0        0        0    32902 2023-07-16 03:51:24.000000 dsds-0.0.20/src/dsds/fs.py
+-rw-rw-rw-   0        0        0     9077 2023-07-13 03:33:56.000000 dsds-0.0.20/src/dsds/metrics.py
+-rw-rw-rw-   0        0        0    30539 2023-07-18 15:20:27.000000 dsds-0.0.20/src/dsds/prescreen.py
+-rw-rw-rw-   0        0        0    15697 2023-07-16 03:59:12.000000 dsds-0.0.20/src/dsds/sample.py
+-rw-rw-rw-   0        0        0    44312 2023-07-18 15:26:06.000000 dsds-0.0.20/src/dsds/transform.py
+-rw-rw-rw-   0        0        0     2986 2023-07-18 15:54:46.000000 dsds-0.0.20/src/dsds/type_alias.py
+-rw-rw-rw-   0        0        0     2085 2023-07-09 00:29:00.000000 dsds-0.0.20/src/dsds/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:56:19.311994 dsds-0.0.20/src/dsds.egg-info/
+-rw-rw-rw-   0        0        0     6759 2023-07-18 15:56:19.000000 dsds-0.0.20/src/dsds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-18 15:56:19.000000 dsds-0.0.20/src/dsds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 15:56:19.000000 dsds-0.0.20/src/dsds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-07-18 15:56:19.000000 dsds-0.0.20/src/dsds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-18 15:56:19.000000 dsds-0.0.20/src/dsds.egg-info/top_level.txt
```

### Comparing `dsds-0.0.19/LICENSE` & `dsds-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `dsds-0.0.19/PKG-INFO` & `dsds-0.0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsds
-Version: 0.0.19
+Version: 0.0.20
 Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
 Author-email: Tianren Qin <tq9695@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 T.Q
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dsds-0.0.19/README.md` & `dsds-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `dsds-0.0.19/pyproject.toml` & `dsds-0.0.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "dsds"
-version = "0.0.19"
+version = "0.0.20"
 requires-python = ">=3.9"
 readme = "README.md"
 description = "A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe."
 authors = [
     {name = "Tianren Qin", email = "tq9695@gmail.com"}
 ]
 license = {file = "LICENSE"}
```

### Comparing `dsds-0.0.19/src/dsds/blueprint.py` & `dsds-0.0.20/src/dsds/blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from polars import LazyFrame
 from dataclasses import dataclass
 from typing import (
     Any
     , Iterable
     , Optional
     , Callable
-    , Concatenate
-    , ParamSpec
+    # , Concatenate
+    # , ParamSpec
 )
 from polars.type_aliases import IntoExpr
 from .type_alias import (
     PolarsFrame
     , ActionType
-    # , PipeFunction
+    , PipeFunction
 )
 
-P = ParamSpec("P")
+# P = ParamSpec("P")
 
 @dataclass
 class MapDict:
     left_col: str # Join on this column, and this column will be replaced by right and dropped.
     ref: dict # The right table as a dictionary
     right_col: str
     default: Optional[Any]
@@ -136,15 +136,15 @@
             Step(action = "drop", associated_data = drop_cols)
         )
         return output
     
     # This doesn't work with the pipeline right now because it clears all steps before this.
     def add_func(self
         , df:LazyFrame # The input to the function that needs to be persisted.
-        , func:Callable[Concatenate[LazyFrame, P], LazyFrame]
+        , func:PipeFunction 
         , kwargs:dict[str, Any]
     ) -> LazyFrame:
         # df: The input lazyframe to the function that needs to be persisted. We need this because:
         # When running the function, the reference to df might be changed, therefore losing the steps
 
         # When this is called, the actual function should be already applied.
         output = self._ldf # .lazy()
```

### Comparing `dsds-0.0.19/src/dsds/eda_text.py` & `dsds-0.0.20/src/dsds/eda_text.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.19/src/dsds/fs.py` & `dsds-0.0.20/src/dsds/fs.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.19/src/dsds/metrics.py` & `dsds-0.0.20/src/dsds/metrics.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.19/src/dsds/prescreen.py` & `dsds-0.0.20/src/dsds/prescreen.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.19/src/dsds/sample.py` & `dsds-0.0.20/src/dsds/sample.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.19/src/dsds/transform.py` & `dsds-0.0.20/src/dsds/transform.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.19/src/dsds/type_alias.py` & `dsds-0.0.20/src/dsds/type_alias.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 from typing import (
-    TypeAlias
-    , Literal
+    Literal
     , Final
     , Tuple
-    , Callable
-    , Concatenate
-    , ParamSpec
-    , Self
 )
+
 import polars as pl
+import sys
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias, Concatenate, ParamSpec, Callable
+    P = ParamSpec('P')
+    PolarsFrame:TypeAlias = pl.DataFrame | pl.LazyFrame
+    PipeFunction = Callable[Concatenate[PolarsFrame, P], PolarsFrame]
+else:
+    from type_extensions import TypeAlias
+    PolarsFrame:TypeAlias = pl.DataFrame | pl.LazyFrame
+    PipeFunction = Callable
+
 import os
 import numpy as np
 from abc import ABC, abstractmethod
 
-P = ParamSpec('P')
+
 CPU_COUNT:Final[int] = os.cpu_count()
 POLARS_NUMERICAL_TYPES:Final[Tuple[pl.DataType]] = (pl.UInt8, pl.UInt16, pl.UInt32, pl.UInt64, pl.Float32, pl.Float64, pl.Int8, pl.Int16, pl.Int32, pl.Int64)  # noqa: E501
 POLARS_DATETIME_TYPES:Final[Tuple[pl.DataType]] = (pl.Datetime, pl.Date)
 
-PolarsFrame:TypeAlias = pl.DataFrame | pl.LazyFrame
-PipeFunction = Callable[Concatenate[PolarsFrame, P], PolarsFrame]
-ActionType = Literal["with_columns", "map_dict", "drop", "select", "add_func", "filter"]
-MRMRStrategy = Literal["fscore", "f", "f_score", "xgb", "xgboost", "rf", "random_forest", "mis"
+ActionType:TypeAlias = Literal["with_columns", "map_dict", "drop", "select", "add_func", "filter"]
+MRMRStrategy:TypeAlias = Literal["fscore", "f", "f_score", "xgb", "xgboost", "rf", "random_forest", "mis"
                        , "mutual_info_score", "lgbm", "lightgbm"]
-ScalingStrategy = Literal["standard", "min_max", "const", "constant"]
-ImputationStrategy = Literal["mean", "avg", "average", "median", "const", "constant", "mode", "most_frequent"]
-PowerTransformStrategy = Literal["yeo_johnson", "yeojohnson", "box_cox", "boxcox"]
+ScalingStrategy:TypeAlias = Literal["standard", "min_max", "const", "constant"]
+ImputationStrategy:TypeAlias = Literal["mean", "avg", "average", "median", "const", "constant", "mode", "most_frequent"]
+PowerTransformStrategy:TypeAlias = Literal["yeo_johnson", "yeojohnson", "box_cox", "boxcox"]
 KSAlternatives = Literal["two-sided", "greater", "less"]
 
-SimpleDtypes = Literal["numeric", "datetime", "bool", "string", "other/unknown"]
-BinaryModels = Literal["logistic", "lr", "lightgbm", "lgbm", "xgboost", "xgb", "random_forest", "rf"]
-DateExtract = Literal["year", "quarter", "month", "week", "day_of_week", "day_of_year"]
+SimpleDtypes:TypeAlias = Literal["numeric", "datetime", "bool", "string", "other/unknown"]
+BinaryModels:TypeAlias = Literal["logistic", "lr", "lightgbm", "lgbm", "xgboost", "xgb", "random_forest", "rf"]
+DateExtract:TypeAlias = Literal["year", "quarter", "month", "week", "day_of_week", "day_of_year"]
 # ArithmeticTransforms = Literal["log", "exp", "sqrt", "fourier"]
 # This is just a subset of Scipy.stats's distributions which can be named by strings. All scipy.stats's string-name-able
 # distributions should work when the arguments asks for a CommonContinuousDist.
-CommonContinuousDist = Literal["norm", "lognorm", "truncnorm", "uniform", "t", "beta", "cauchy", "expon", "gamma"]
+CommonContinuousDist:TypeAlias = Literal["norm", "lognorm", "truncnorm", "uniform", "t", "beta", "cauchy", "expon", "gamma"]
 
 def clean_strategy_str(s:str):
     '''Strategy strings will only have _, no -, and all lowercase.'''
     return s.strip().replace("-", "_").lower()
 
 class ClassifModel(ABC):
 
@@ -47,18 +52,18 @@
         ...
 
     @abstractmethod
     def predict_proba(self, X: np.ndarray|pl.DataFrame) -> np.ndarray:
         ...
 
     @abstractmethod
-    def fit(self, X:np.ndarray|pl.DataFrame, y:np.ndarray|pl.Series|pl.DataFrame) -> Self:
+    def fit(self, X:np.ndarray|pl.DataFrame, y:np.ndarray|pl.Series|pl.DataFrame): # Should return self
         ...
     
 class RegressionModel(ABC):
     @abstractmethod
     def predict(self, X: np.ndarray|pl.DataFrame) -> np.ndarray:
         ...
 
     @abstractmethod
-    def fit(self, X:np.ndarray|pl.DataFrame, y:np.ndarray|pl.Series|pl.DataFrame) -> Self:
+    def fit(self, X:np.ndarray|pl.DataFrame, y:np.ndarray|pl.Series|pl.DataFrame): # Should return self
         ...
```

### Comparing `dsds-0.0.19/src/dsds/utils.py` & `dsds-0.0.20/src/dsds/utils.py`

 * *Files identical despite different names*

### Comparing `dsds-0.0.19/src/dsds.egg-info/PKG-INFO` & `dsds-0.0.20/src/dsds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsds
-Version: 0.0.19
+Version: 0.0.20
 Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
 Author-email: Tianren Qin <tq9695@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 T.Q
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

