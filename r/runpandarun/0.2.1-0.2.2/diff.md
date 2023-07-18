# Comparing `tmp/runpandarun-0.2.1.tar.gz` & `tmp/runpandarun-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpandarun-0.2.1.tar", max compression
+gzip compressed data, was "runpandarun-0.2.2.tar", max compression
```

## Comparing `runpandarun-0.2.1.tar` & `runpandarun-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-07-15 09:47:01.438078 runpandarun-0.2.1/LICENSE
--rw-r--r--   0        0        0     9271 2023-07-15 09:47:01.438078 runpandarun-0.2.1/README.md
--rw-r--r--   0        0        0     1345 2023-07-15 09:55:53.530736 runpandarun-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      145 2023-07-15 09:55:53.530736 runpandarun-0.2.1/runpandarun/__init__.py
--rw-r--r--   0        0        0      618 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/cli.py
--rw-r--r--   0        0        0       37 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/exceptions.py
--rw-r--r--   0        0        0     1853 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/io.py
--rw-r--r--   0        0        0     2304 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/playbook.py
--rw-r--r--   0        0        0     1770 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/util.py
--rw-r--r--   0        0        0    10496 1970-01-01 00:00:00.000000 runpandarun-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-15 09:47:01.438078 runpandarun-0.2.2/LICENSE
+-rw-r--r--   0        0        0     9271 2023-07-15 09:47:01.438078 runpandarun-0.2.2/README.md
+-rw-r--r--   0        0        0     1361 2023-07-18 13:05:52.678428 runpandarun-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-07-18 13:05:52.678428 runpandarun-0.2.2/runpandarun/__init__.py
+-rw-r--r--   0        0        0      618 2023-07-15 09:47:01.438078 runpandarun-0.2.2/runpandarun/cli.py
+-rw-r--r--   0        0        0       37 2023-07-15 09:47:01.438078 runpandarun-0.2.2/runpandarun/exceptions.py
+-rw-r--r--   0        0        0     2105 2023-07-18 12:54:26.558516 runpandarun-0.2.2/runpandarun/io.py
+-rw-r--r--   0        0        0     2337 2023-07-18 12:09:18.822717 runpandarun-0.2.2/runpandarun/playbook.py
+-rw-r--r--   0        0        0     1776 2023-07-18 12:54:26.558516 runpandarun-0.2.2/runpandarun/util.py
+-rw-r--r--   0        0        0    10525 1970-01-01 00:00:00.000000 runpandarun-0.2.2/PKG-INFO
```

### Comparing `runpandarun-0.2.1/LICENSE` & `runpandarun-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `runpandarun-0.2.1/README.md` & `runpandarun-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `runpandarun-0.2.1/pyproject.toml` & `runpandarun-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runpandarun"
-version = "0.2.1"
+version = "0.2.2"
 description = "Tell pandas what to do – easy tabular data I/O playbooks"
 authors = ["Simon Wörpel <simon@investigativedata.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://investigraph.dev"
 repository = "https://github.com/investigativedata/investigraph-etl"
 documentation = "https://docs.investigraph.dev/runpandarun"
@@ -24,20 +24,21 @@
 "Bug Tracker" = "https://github.com/investigativedata/runpandarun/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "2.0.3"
 requests = "2.31.0"
 typer = "0.9.0"
-pydantic = "^2.0.3"
+pydantic = "<2.0"
 banal = "^1.0.6"
 normality = "^2.4.0"
 fingerprints = "^1.1.0"
 fsspec = "^2023.6.0"
 s3fs = "^2023.6.0"
+orjson = "^3.9.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
```

### Comparing `runpandarun-0.2.1/runpandarun/cli.py` & `runpandarun-0.2.2/runpandarun/cli.py`

 * *Files identical despite different names*

### Comparing `runpandarun-0.2.1/runpandarun/io.py` & `runpandarun-0.2.2/runpandarun/io.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import sys
 from io import BytesIO, StringIO
 from typing import Any, TypeVar
 
+import fsspec
+import orjson
 import pandas as pd
-from pydantic import BaseModel, field_validator
+from pydantic import BaseModel
+from pydantic import validator as field_validator
 
 from .util import PathLike
 
 IO = TypeVar("IO", bound=StringIO | BytesIO)
 
 
 class Handler(BaseModel):
@@ -47,17 +50,19 @@
 
 def read_pandas(
     io: PathLike | IO,
     handler: str | None = "read_csv",
     mode: str | None = "rb",
     **kwargs
 ) -> pd.DataFrame:
-    handler = getattr(pd, handler)
     if io == "-":
         io = sys.stdin.buffer
+    if handler == "json_normalize":
+        io = read_json(io)
+    handler = getattr(pd, handler)
     res = handler(io, **kwargs)
     if hasattr(io, "close"):
         io.close()
     return res
 
 
 def write_pandas(
@@ -70,7 +75,13 @@
     handler = getattr(df, handler)
     if io == "-":
         io = sys.stdout.buffer
     res = handler(io, **kwargs)
     if hasattr(io, "close"):
         io.close()
     return res
+
+
+def read_json(io: PathLike | IO) -> Any:
+    with fsspec.open(io) as f:
+        data = f.read()
+    return orjson.loads(data)
```

### Comparing `runpandarun-0.2.1/runpandarun/playbook.py` & `runpandarun-0.2.2/runpandarun/playbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, TypeVar
 
 import yaml
 from pandas import DataFrame, Series
-from pydantic import BaseModel, field_validator
+from pydantic import BaseModel
+from pydantic import validator as field_validator
 
 from .exceptions import SpecError
 from .io import ReadHandler, WriteHandler
 from .util import PathLike, absolute_path, expandvars, getattr_by_path, safe_eval
 
 P = TypeVar("P", bound="Playbook")
```

### Comparing `runpandarun-0.2.1/runpandarun/util.py` & `runpandarun-0.2.2/runpandarun/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         return {k: expandvars(v) for k, v in dict(data).items()}
     return data
 
 
 def absolute_path(path: PathLike, base: PathLike) -> PathLike | str:
     if path == "-" or urlparse(str(path)).scheme:
         return path
-    return os.path.normpath((Path(base).parent / Path(path)).absolute().as_uri())
+    return Path(os.path.normpath((Path(base).parent / Path(path)).absolute())).as_uri()
 
 
 def getattr_by_path(thing: Any, path: str) -> Any:
     # getattr(foo, "bar.baz")
     for p in path.split("."):
         thing = getattr(thing, p)
     return thing
```

### Comparing `runpandarun-0.2.1/PKG-INFO` & `runpandarun-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpandarun
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tell pandas what to do – easy tabular data I/O playbooks
 Home-page: https://investigraph.dev
 License: MIT
 Author: Simon Wörpel
 Author-email: simon@investigativedata.org
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
@@ -14,16 +14,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: banal (>=1.0.6,<2.0.0)
 Requires-Dist: fingerprints (>=1.1.0,<2.0.0)
 Requires-Dist: fsspec (>=2023.6.0,<2024.0.0)
 Requires-Dist: normality (>=2.4.0,<3.0.0)
+Requires-Dist: orjson (>=3.9.2,<4.0.0)
 Requires-Dist: pandas (==2.0.3)
-Requires-Dist: pydantic (>=2.0.3,<3.0.0)
+Requires-Dist: pydantic (<2.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: s3fs (>=2023.6.0,<2024.0.0)
 Requires-Dist: typer (==0.9.0)
 Project-URL: Bug Tracker, https://github.com/investigativedata/runpandarun/issues
 Project-URL: Documentation, https://docs.investigraph.dev/runpandarun
 Project-URL: Repository, https://github.com/investigativedata/investigraph-etl
 Description-Content-Type: text/markdown
```

