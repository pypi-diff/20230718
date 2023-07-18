# Comparing `tmp/patito-0.5.0.tar.gz` & `tmp/patito-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patito-0.5.0.tar", max compression
+gzip compressed data, was "patito-0.5.1.tar", max compression
```

## Comparing `patito-0.5.0.tar` & `patito-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1139 2023-06-21 23:24:02.891944 patito-0.5.0/LICENSE
--rw-r--r--   0        0        0    12944 2023-06-21 23:24:02.891944 patito-0.5.0/README.md
--rw-r--r--   0        0        0     3330 2023-06-21 23:24:02.895943 patito-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1169 2023-06-21 23:24:02.895943 patito-0.5.0/src/patito/__init__.py
--rw-r--r--   0        0        0      161 2023-06-21 23:24:02.895943 patito-0.5.0/src/patito/_docs.py
--rw-r--r--   0        0        0    27917 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/database.py
--rw-r--r--   0        0        0   111015 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/duckdb.py
--rw-r--r--   0        0        0     1262 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/exceptions.py
--rw-r--r--   0        0        0    26161 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/polars.py
--rw-r--r--   0        0        0    54832 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/pydantic.py
--rw-r--r--   0        0        0     3218 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/sql.py
--rw-r--r--   0        0        0    10659 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/validators.py
--rw-r--r--   0        0        0      686 2023-06-21 23:24:02.899944 patito-0.5.0/src/patito/xdg.py
--rw-r--r--   0        0        0    14562 1970-01-01 00:00:00.000000 patito-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1139 2023-07-18 14:28:19.187170 patito-0.5.1/LICENSE
+-rw-r--r--   0        0        0    12944 2023-07-18 14:28:19.187170 patito-0.5.1/README.md
+-rw-r--r--   0        0        0     3329 2023-07-18 14:28:19.191170 patito-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1169 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/__init__.py
+-rw-r--r--   0        0        0      161 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/_docs.py
+-rw-r--r--   0        0        0    27917 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/database.py
+-rw-r--r--   0        0        0   111015 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/duckdb.py
+-rw-r--r--   0        0        0     1262 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/exceptions.py
+-rw-r--r--   0        0        0    26161 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/polars.py
+-rw-r--r--   0        0        0    54832 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/pydantic.py
+-rw-r--r--   0        0        0     3218 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/sql.py
+-rw-r--r--   0        0        0    10670 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/validators.py
+-rw-r--r--   0        0        0      686 2023-07-18 14:28:19.191170 patito-0.5.1/src/patito/xdg.py
+-rw-r--r--   0        0        0    14569 1970-01-01 00:00:00.000000 patito-0.5.1/PKG-INFO
```

### Comparing `patito-0.5.0/LICENSE` & `patito-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/README.md` & `patito-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/pyproject.toml` & `patito-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "patito"
-version = "0.5.0"
+version = "0.5.1"
 description = "A dataframe modelling library built on top of polars and pydantic."
 authors = ["Jakob Gerhard Martinussen <jakobgm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/patito"
 repository = "https://github.com/kolonialno/patito"
 documentation = "https://patito.readthedocs.io"
 keywords = ["validation", "dataframe"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = ">=1.7.0"
-polars = ">=0.18.3"
+pydantic = "^1.7.0"
+polars = ">=0.18.7"
 # Required for typing.Literal in python3.7
 typing-extensions = "*"
 pandas = {version = "*", optional = true, python = "^3.8"}
 duckdb = {version = ">=0.6.0", optional = true, python = "^3.8"}
 pyarrow = {version = ">=5.0.0", optional = true, python = "^3.8"}
 # Optional docs dependencies
 Sphinx = {version = "<7", optional = true}
```

### Comparing `patito-0.5.0/src/patito/__init__.py` & `patito-0.5.1/src/patito/__init__.py`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/src/patito/database.py` & `patito-0.5.1/src/patito/database.py`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/src/patito/duckdb.py` & `patito-0.5.1/src/patito/duckdb.py`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/src/patito/exceptions.py` & `patito-0.5.1/src/patito/exceptions.py`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/src/patito/polars.py` & `patito-0.5.1/src/patito/polars.py`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/src/patito/pydantic.py` & `patito-0.5.1/src/patito/pydantic.py`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/src/patito/sql.py` & `patito-0.5.1/src/patito/sql.py`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/src/patito/validators.py` & `patito-0.5.1/src/patito/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
                     )
                 )
 
         if "constraints" in column_properties:
             custom_constraints = column_properties["constraints"]
             if isinstance(custom_constraints, pl.Expr):
                 custom_constraints = [custom_constraints]
-            constraints = pl.all(
+            constraints = pl.all_horizontal(
                 [constraint.is_not() for constraint in custom_constraints]
             )
             if "_" in constraints.meta.root_names():
                 # An underscore is an alias for the current field
                 illegal_rows = dataframe.with_columns(
                     pl.col(column_name).alias("_")
                 ).filter(constraints)
```

### Comparing `patito-0.5.0/src/patito/xdg.py` & `patito-0.5.1/src/patito/xdg.py`

 * *Files identical despite different names*

### Comparing `patito-0.5.0/PKG-INFO` & `patito-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patito
-Version: 0.5.0
+Version: 0.5.1
 Summary: A dataframe modelling library built on top of polars and pydantic.
 Home-page: https://github.com/kolonialno/patito
 License: MIT
 Keywords: validation,dataframe
 Author: Jakob Gerhard Martinussen
 Author-email: jakobgm@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,17 +17,17 @@
 Provides-Extra: caching
 Provides-Extra: docs
 Provides-Extra: duckdb
 Provides-Extra: pandas
 Requires-Dist: Sphinx (<7) ; extra == "docs"
 Requires-Dist: duckdb (>=0.6.0) ; (python_version >= "3.8" and python_version < "4.0") and (extra == "duckdb")
 Requires-Dist: pandas ; (python_version >= "3.8" and python_version < "4.0") and (extra == "pandas")
-Requires-Dist: polars (>=0.18.3)
+Requires-Dist: polars (>=0.18.7)
 Requires-Dist: pyarrow (>=5.0.0) ; (python_version >= "3.8" and python_version < "4.0") and (extra == "caching" or extra == "duckdb")
-Requires-Dist: pydantic (>=1.7.0)
+Requires-Dist: pydantic (>=1.7.0,<2.0.0)
 Requires-Dist: sphinx-autobuild ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: sphinx-toolbox ; extra == "docs"
 Requires-Dist: sphinxcontrib-mermaid ; extra == "docs"
 Requires-Dist: typing-extensions
 Project-URL: Documentation, https://patito.readthedocs.io
```

