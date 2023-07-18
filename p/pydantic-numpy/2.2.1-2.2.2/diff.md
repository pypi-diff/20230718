# Comparing `tmp/pydantic_numpy-2.2.1.tar.gz` & `tmp/pydantic_numpy-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_numpy-2.2.1.tar", max compression
+gzip compressed data, was "pydantic_numpy-2.2.2.tar", max compression
```

## Comparing `pydantic_numpy-2.2.1.tar` & `pydantic_numpy-2.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2022-08-02 10:04:40.699027 pydantic_numpy-2.2.1/LICENSE
--rw-r--r--   0        0        0     2055 2023-03-29 17:47:28.792977 pydantic_numpy-2.2.1/README.md
--rw-r--r--   0        0        0      215 2023-03-29 17:47:28.793977 pydantic_numpy-2.2.1/pydantic_numpy/__init__.py
--rw-r--r--   0        0        0     2572 2023-03-09 14:52:08.799312 pydantic_numpy-2.2.1/pydantic_numpy/dtype.py
--rw-r--r--   0        0        0     5232 2023-03-29 17:50:01.146968 pydantic_numpy-2.2.1/pydantic_numpy/model.py
--rw-r--r--   0        0        0     3153 2023-03-10 13:17:32.991257 pydantic_numpy-2.2.1/pydantic_numpy/ndarray.py
--rw-r--r--   0        0        0     1017 2023-03-29 17:50:01.148968 pydantic_numpy-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 pydantic_numpy-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-2.2.2/LICENSE
+-rw-r--r--   0        0        0     2055 2023-04-23 14:42:01.570137 pydantic_numpy-2.2.2/README.md
+-rw-r--r--   0        0        0      215 2023-04-23 14:42:01.571137 pydantic_numpy-2.2.2/pydantic_numpy/__init__.py
+-rw-r--r--   0        0        0     2580 2023-04-29 07:57:37.210284 pydantic_numpy-2.2.2/pydantic_numpy/dtype.py
+-rw-r--r--   0        0        0     5236 2023-07-18 10:02:41.536876 pydantic_numpy-2.2.2/pydantic_numpy/model.py
+-rw-r--r--   0        0        0     3153 2023-03-17 05:45:48.795212 pydantic_numpy-2.2.2/pydantic_numpy/ndarray.py
+-rw-r--r--   0        0        0     1023 2023-07-18 10:05:20.705498 pydantic_numpy-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3043 1970-01-01 00:00:00.000000 pydantic_numpy-2.2.2/PKG-INFO
```

### Comparing `pydantic_numpy-2.2.1/LICENSE` & `pydantic_numpy-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-2.2.1/README.md` & `pydantic_numpy-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-2.2.1/pydantic_numpy/dtype.py` & `pydantic_numpy-2.2.2/pydantic_numpy/dtype.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pydantic_numpy.ndarray import NDArray
 
 if TYPE_CHECKING:
     from pydantic.typing import CallableGenerator
 
 
-class _BaseDType:
+class _BaseDType(object):
     @classmethod
     def __modify_schema__(cls, field_schema: dict[str, Any]) -> None:
         field_schema.update({"type": cls.__name__})
 
     @classmethod
     def __get_validators__(cls) -> CallableGenerator:
         yield cls.validate
```

### Comparing `pydantic_numpy-2.2.1/pydantic_numpy/model.py` & `pydantic_numpy-2.2.2/pydantic_numpy/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     Callable,
     ClassVar,
     Dict,
     Iterable,
     Optional,
     Tuple,
     Type,
-    TypeVar, Union,
+    TypeVar,
+    Union,
 )
 
 import compress_pickle
 import numpy as np
 from pydantic import BaseModel, DirectoryPath, FilePath, validate_arguments
 from ruamel.yaml import YAML
```

### Comparing `pydantic_numpy-2.2.1/pydantic_numpy/ndarray.py` & `pydantic_numpy-2.2.2/pydantic_numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-2.2.1/pyproject.toml` & `pydantic_numpy-2.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_numpy"
-version = "2.2.1"
+version = "2.2.2"
 description = "Seamlessly integrate numpy arrays into pydantic models"
 authors = ["Can H. Tartanoglu <canhtart@gmail.com>", "Christoph Heindl"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/caniko/pydantic-numpy"
 
@@ -19,15 +19,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 compress-pickle = { version = "*", extras = ["lz4"] }
 ruamel-yaml = "^0.17.21"
 
 numpy = "*"
-pydantic = "*"
+pydantic = "^1.10.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 black = "*"
 isort = "*"
 pre-commit = "*"
```

### Comparing `pydantic_numpy-2.2.1/PKG-INFO` & `pydantic_numpy-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-numpy
-Version: 2.2.1
+Version: 2.2.2
 Summary: Seamlessly integrate numpy arrays into pydantic models
 Home-page: https://github.com/caniko/pydantic-numpy
 License: MIT
 Keywords: pydantic,numpy,typing
 Author: Can H. Tartanoglu
 Author-email: canhtart@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: compress-pickle[lz4]
 Requires-Dist: numpy
-Requires-Dist: pydantic
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Project-URL: Repository, https://github.com/caniko/pydantic-numpy
 Description-Content-Type: text/markdown
 
 # pydantic-numpy
 
 Integrate NumPy into Pydantic, and provide tooling! `NumpyModel` make it possible to dump and load `np.ndarray` within model fields!
```

