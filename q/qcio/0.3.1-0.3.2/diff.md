# Comparing `tmp/qcio-0.3.1.tar.gz` & `tmp/qcio-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcio-0.3.1.tar", max compression
+gzip compressed data, was "qcio-0.3.2.tar", max compression
```

## Comparing `qcio-0.3.1.tar` & `qcio-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2023-07-18 00:17:05.815752 qcio-0.3.1/LICENSE
--rw-r--r--   0        0        0      898 2023-07-18 00:17:05.815752 qcio-0.3.1/README.md
--rw-r--r--   0        0        0     1246 2023-07-18 00:17:05.819753 qcio-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      573 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/__init__.py
--rw-r--r--   0        0        0       89 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/constants.py
--rw-r--r--   0        0        0      346 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/helper_types.py
--rw-r--r--   0        0        0      272 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/__init__.py
--rw-r--r--   0        0        0     9738 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/base_models.py
--rw-r--r--   0        0        0     3082 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/inputs.py
--rw-r--r--   0        0        0     2236 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/inputs_base.py
--rw-r--r--   0        0        0     8187 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/molecule.py
--rw-r--r--   0        0        0     3585 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/outputs.py
--rw-r--r--   0        0        0     1935 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/outputs_base.py
--rw-r--r--   0        0        0     4462 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/results.py
--rw-r--r--   0        0        0     4413 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/qcel.py
--rw-r--r--   0        0        0      838 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/utils.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-18 01:10:31.845509 qcio-0.3.2/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-18 01:10:31.845509 qcio-0.3.2/README.md
+-rw-r--r--   0        0        0     1246 2023-07-18 01:10:31.845509 qcio-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      573 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/constants.py
+-rw-r--r--   0        0        0      346 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/helper_types.py
+-rw-r--r--   0        0        0      272 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/__init__.py
+-rw-r--r--   0        0        0     9738 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/base_models.py
+-rw-r--r--   0        0        0     3082 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/inputs.py
+-rw-r--r--   0        0        0     2236 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/inputs_base.py
+-rw-r--r--   0        0        0     8354 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/molecule.py
+-rw-r--r--   0        0        0     3585 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/outputs.py
+-rw-r--r--   0        0        0     1935 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/outputs_base.py
+-rw-r--r--   0        0        0     4462 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/results.py
+-rw-r--r--   0        0        0     4413 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/qcel.py
+-rw-r--r--   0        0        0      838 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/utils.py
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.3.2/PKG-INFO
```

### Comparing `qcio-0.3.1/LICENSE` & `qcio-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/README.md` & `qcio-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/pyproject.toml` & `qcio-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qcio"
-version = "0.3.1"
+version = "0.3.2"
 description = "Beautiful and user friendly data structures for quantum chemistry."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `qcio-0.3.1/qcio/__init__.py` & `qcio-0.3.2/qcio/__init__.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/qcio/models/base_models.py` & `qcio-0.3.2/qcio/models/base_models.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/qcio/models/inputs.py` & `qcio-0.3.2/qcio/models/inputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/qcio/models/inputs_base.py` & `qcio-0.3.2/qcio/models/inputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/qcio/models/molecule.py` & `qcio-0.3.2/qcio/models/molecule.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,20 +131,22 @@
         return "".join(
             f"{element}{count if count > 1 else ''}"
             for element, count in sorted_elements
         )
 
     def dict(self, **kwargs) -> Dict[str, Any]:
         """Handle tuple in connectivity"""
-        dict = super().dict(**kwargs)
-        # Must cast all values to floats as toml cannot handle mixed types
-        dict["connectivity"] = [
-            [float(val) for val in bond] for bond in dict["connectivity"]
-        ]
-        return dict
+        as_dict = super().dict(**kwargs)
+        # Connectivity may be empty and super().dict() will remove empty values
+        if (connectivity := as_dict.get("connectivity")) is not None:
+            # Must cast all values to floats as toml cannot handle mixed types
+            as_dict["connectivity"] = [
+                [float(val) for val in bond] for bond in connectivity
+            ]
+        return as_dict
 
     @classmethod
     def open(cls, filepath: Union[Path, str]) -> Self:
         """Open a molecule from a file.
 
         Args:
             filepath: The path to the file to open. Maybe a path to a JSON file or an
```

### Comparing `qcio-0.3.1/qcio/models/outputs.py` & `qcio-0.3.2/qcio/models/outputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/qcio/models/outputs_base.py` & `qcio-0.3.2/qcio/models/outputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/qcio/models/results.py` & `qcio-0.3.2/qcio/models/results.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/qcio/qcel.py` & `qcio-0.3.2/qcio/qcel.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/qcio/utils.py` & `qcio-0.3.2/qcio/utils.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.1/PKG-INFO` & `qcio-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcio
-Version: 0.3.1
+Version: 0.3.2
 Summary: Beautiful and user friendly data structures for quantum chemistry.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

