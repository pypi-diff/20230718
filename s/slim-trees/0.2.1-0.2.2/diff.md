# Comparing `tmp/slim-trees-0.2.1.tar.gz` & `tmp/slim_trees-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slim-trees-0.2.1.tar", last modified: Wed May 31 09:39:37 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `slim-trees-0.2.1.tar` & `slim_trees-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:39:36.996528 slim-trees-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-31 09:39:25.000000 slim-trees-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 09:39:25.000000 slim-trees-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-31 09:39:36.996528 slim-trees-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-31 09:39:25.000000 slim-trees-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 09:39:25.000000 slim-trees-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-31 09:39:36.996528 slim-trees-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:39:36.992528 slim-trees-0.2.1/slim_trees/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/lgbm_booster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/sklearn_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-31 09:39:25.000000 slim-trees-0.2.1/slim_trees/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:39:36.996528 slim-trees-0.2.1/slim_trees.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 09:39:36.000000 slim-trees-0.2.1/slim_trees.egg-info/top_level.txt
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/compression_utils.py
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/lgbm_booster.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/pickling.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/sklearn_tree.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 slim_trees-0.2.2/slim_trees/utils.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 slim_trees-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 slim_trees-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 slim_trees-0.2.2/README.md
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 slim_trees-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 slim_trees-0.2.2/PKG-INFO
```

### Comparing `slim-trees-0.2.1/LICENSE` & `slim_trees-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slim-trees-0.2.1/PKG-INFO` & `slim_trees-0.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: slim-trees
-Version: 0.2.1
-Summary: A python package for efficient pickling of ML models.
-Home-page: https://github.com/quantco/slim-trees
-Author: Pavel Zwerschke
-Author-email: pavel.zwerschke@quantco.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: scikit-learn
-Provides-Extra: lightgbm
-License-File: LICENSE
-
 # Slim Trees
 
 [![CI](https://github.com/quantco/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/quantco/slim-trees/actions/workflows/ci.yml)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/slim-trees?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/slim-trees)
 [![pypi-version](https://img.shields.io/pypi/v/slim-trees.svg?logo=pypi&logoColor=white)](https://pypi.org/project/slim-trees)
 [![python-version](https://img.shields.io/pypi/pyversions/slim-trees?logoColor=white&logo=python)](https://pypi.org/project/slim-trees)
 
@@ -30,14 +12,16 @@
 
 ## Installation
 
 ```bash
 pip install slim-trees
 # or
 micromamba install slim-trees -c conda-forge
+# or
+pixi add slim-trees
 ```
 
 ## Usage
 
 Using `slim-trees` does not affect your training pipeline.
 Simply call `dump_sklearn_compressed` or `dump_lgbm_compressed` to save your model.
 
@@ -122,26 +106,38 @@
 # for lightgbm models
 with open("model.pkl", "wb") as f:
     lgbm_booster.dump(model, f)  # instead of pickle.dump(...)
 ```
 
 ## Development Installation
 
-You can install the package in development mode using:
+You can install the package in development mode using the new conda package manager [`pixi`](https://github.com/prefix-dev/pixi):
 
 ```bash
-git clone https://github.com/quantco/slim-trees.git
-cd slim-trees
+❯ git clone https://github.com/quantco/slim-trees.git
+❯ cd slim-trees
+
+❯ pixi install
+❯ pixi run pre-commit install
+❯ pixi run pip install --no-deps --disable-pip-version-check --no-build-isolation -e .
+❯ pixi run python
+>>> import slim_trees
+[...]
+❯ pixi run test
+[...]
+```
+
+Alternatively, you can use `micromamba` (or `mamba` or `conda`):
 
-# create and activate a fresh environment named slim_trees
-micromamba create -f environment.yml
-micromamba activate slim_trees
+```bash
+❯ micromamba create -f environment.yml
+❯ micromamba activate slim_trees
 
-pre-commit install
-pip install --no-build-isolation -e .
+❯ pre-commit install
+❯ pip install --no-build-isolation -e .
 ```
 
 ## Benchmark
 
 As a general overview on what you can expect in terms of savings:
 This is a 1.2G large sklearn `RandomForestRegressor`.
```

### Comparing `slim-trees-0.2.1/slim_trees/__init__.py` & `slim_trees-0.2.2/slim_trees/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 In this module, a custom pickling behavior for the sklearn Tree class is specified that compresses
 the internal values from int64 to int16 and from float64 to float32 (in the value field) and from
 float64 to a mixture between float64 and int16 (in the threshold field).
 You can pickle a model with custom picklers by specifying dump_function in dump_compressed in the
 pickling module.
 """
 
+import importlib.metadata
+import warnings
 from pathlib import Path
 from typing import Any, Optional, Union
 
-import pkg_resources
-
 from slim_trees.pickling import (
     dump_compressed,
     dumps_compressed,
     load_compressed,
     loads_compressed,
 )
 
 try:
-    __version__ = pkg_resources.get_distribution(__name__).version
-except Exception:
+    __version__ = importlib.metadata.version(__name__)
+except Exception as e:
+    warnings.warn(f"Could not determine version of {__name__}", stacklevel=1)
+    warnings.warn(str(e), stacklevel=1)
     __version__ = "unknown"
 
 __all__ = [
     "dump_compressed",
     "dumps_compressed",
     "load_compressed",
     "loads_compressed",
```

### Comparing `slim-trees-0.2.1/slim_trees/compression_utils.py` & `slim_trees-0.2.2/slim_trees/compression_utils.py`

 * *Files identical despite different names*

### Comparing `slim-trees-0.2.1/slim_trees/lgbm_booster.py` & `slim_trees-0.2.2/slim_trees/lgbm_booster.py`

 * *Files identical despite different names*

### Comparing `slim-trees-0.2.1/slim_trees/pickling.py` & `slim_trees-0.2.2/slim_trees/pickling.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 
 class _NoCompression:
     def __init__(self):
         self.open = open
         self.compress = lambda data: data
 
+    @staticmethod
+    def decompress(data):
+        return data
+
 
 def _get_compression_from_path(path: Union[str, pathlib.Path]) -> str:
     compressions = {
         ".gz": "gzip",
         ".lzma": "lzma",
         ".bz2": "bz2",
         ".pickle": "no",
@@ -116,46 +120,58 @@
 
     compression_method, kwargs = _unpack_compression_args(compression, None)
     data_uncompressed = dump_function(obj)
     return _get_compression_library(compression_method).compress(data_uncompressed)
 
 
 def load_compressed(
-    path: Union[str, pathlib.Path], compression: Optional[Union[str, dict]] = None
+    path: Union[str, pathlib.Path],
+    compression: Optional[Union[str, dict]] = None,
+    unpickler_class: type = pickle.Unpickler,
 ) -> Any:
     """
     Loads a compressed model.
     :param path: where to load the object from
     :param compression: the compression method used. Either a string or a dict with key 'method'
                         set to the compression method and other key-value pairs which are forwarded
                         to open() of the compression library.
                         Inspired by the pandas.to_csv interface.
+    :param unpickler_class: custom unpickler class derived from pickle.Unpickler.
+                            This is useful to restrict possible imports or to allow unpickling
+                            when required module or function names have been refactored.
     """
     compression_method, kwargs = _unpack_compression_args(compression, path)
     with _get_compression_library(compression_method).open(
         path, mode="rb", **kwargs
     ) as file:
-        return pickle.load(file)
+        return unpickler_class(file).load()
 
 
-def loads_compressed(data: bytes, compression: Optional[Union[str, dict]] = None):
+def loads_compressed(
+    data: bytes,
+    compression: Optional[Union[str, dict]] = None,
+    unpickler_class: type = pickle.Unpickler,
+) -> Any:
     """
     Loads a compressed model.
     :param data: bytes containing the pickled object.
     :param compression: the compression method used. Either a string or a dict with key 'method'
                         set to the compression method and other key-value pairs which are forwarded
                         to open() of the compression library. Defaults to 'no' compression.
                         Inspired by the pandas.to_csv interface.
+    :param unpickler_class: custom unpickler class derived from pickle.Unpickler.
+                            This is useful to restrict possible imports or to allow unpickling
+                            when required module or function names have been refactored.
     """
     if compression is None:
         compression = "no"
 
     compression_method, kwargs = _unpack_compression_args(compression, None)
     data_uncompressed = _get_compression_library(compression_method).decompress(data)
-    return pickle.loads(data_uncompressed)
+    return unpickler_class(io.BytesIO(data_uncompressed)).load()
 
 
 def get_pickled_size(
     obj: Any,
     compression: Union[str, dict] = "lzma",
     dump_function: Optional[Callable] = None,
 ) -> int:
```

### Comparing `slim-trees-0.2.1/slim_trees/sklearn_tree.py` & `slim_trees-0.2.2/slim_trees/sklearn_tree.py`

 * *Files identical despite different names*

### Comparing `slim-trees-0.2.1/slim_trees.egg-info/PKG-INFO` & `slim_trees-0.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: slim-trees
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package for efficient pickling of ML models.
-Home-page: https://github.com/quantco/slim-trees
-Author: Pavel Zwerschke
-Author-email: pavel.zwerschke@quantco.com
+Project-URL: Homepage, https://github.com/quantco/slim-trees
+Author-email: Pavel Zwerschke <pavel.zwerschke@quantco.com>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: scikit-learn
+Requires-Dist: numpy
 Provides-Extra: lightgbm
-License-File: LICENSE
+Requires-Dist: lightgbm<4.0; extra == 'lightgbm'
+Provides-Extra: scikit-learn
+Requires-Dist: scikit-learn<1.3.0; extra == 'scikit-learn'
+Description-Content-Type: text/markdown
 
 # Slim Trees
 
 [![CI](https://github.com/quantco/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/quantco/slim-trees/actions/workflows/ci.yml)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/slim-trees?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/slim-trees)
 [![pypi-version](https://img.shields.io/pypi/v/slim-trees.svg?logo=pypi&logoColor=white)](https://pypi.org/project/slim-trees)
 [![python-version](https://img.shields.io/pypi/pyversions/slim-trees?logoColor=white&logo=python)](https://pypi.org/project/slim-trees)
@@ -30,14 +33,16 @@
 
 ## Installation
 
 ```bash
 pip install slim-trees
 # or
 micromamba install slim-trees -c conda-forge
+# or
+pixi add slim-trees
 ```
 
 ## Usage
 
 Using `slim-trees` does not affect your training pipeline.
 Simply call `dump_sklearn_compressed` or `dump_lgbm_compressed` to save your model.
 
@@ -122,26 +127,38 @@
 # for lightgbm models
 with open("model.pkl", "wb") as f:
     lgbm_booster.dump(model, f)  # instead of pickle.dump(...)
 ```
 
 ## Development Installation
 
-You can install the package in development mode using:
+You can install the package in development mode using the new conda package manager [`pixi`](https://github.com/prefix-dev/pixi):
 
 ```bash
-git clone https://github.com/quantco/slim-trees.git
-cd slim-trees
+❯ git clone https://github.com/quantco/slim-trees.git
+❯ cd slim-trees
+
+❯ pixi install
+❯ pixi run pre-commit install
+❯ pixi run pip install --no-deps --disable-pip-version-check --no-build-isolation -e .
+❯ pixi run python
+>>> import slim_trees
+[...]
+❯ pixi run test
+[...]
+```
 
-# create and activate a fresh environment named slim_trees
-micromamba create -f environment.yml
-micromamba activate slim_trees
+Alternatively, you can use `micromamba` (or `mamba` or `conda`):
+
+```bash
+❯ micromamba create -f environment.yml
+❯ micromamba activate slim_trees
 
-pre-commit install
-pip install --no-build-isolation -e .
+❯ pre-commit install
+❯ pip install --no-build-isolation -e .
 ```
 
 ## Benchmark
 
 As a general overview on what you can expect in terms of savings:
 This is a 1.2G large sklearn `RandomForestRegressor`.
```

