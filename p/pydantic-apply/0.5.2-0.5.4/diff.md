# Comparing `tmp/pydantic_apply-0.5.2.tar.gz` & `tmp/pydantic_apply-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_apply-0.5.2.tar", max compression
+gzip compressed data, was "pydantic_apply-0.5.4.tar", max compression
```

## Comparing `pydantic_apply-0.5.2.tar` & `pydantic_apply-0.5.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2023-07-16 13:02:14.725504 pydantic_apply-0.5.2/LICENSE
--rw-r--r--   0        0        0     2258 2023-07-16 13:02:14.725504 pydantic_apply-0.5.2/README.md
--rw-r--r--   0        0        0       35 2023-07-16 13:02:14.729504 pydantic_apply-0.5.2/pydantic_apply/__init__.py
--rw-r--r--   0        0        0     2453 2023-07-16 13:02:14.729504 pydantic_apply-0.5.2/pydantic_apply/_compat.py
--rw-r--r--   0        0        0     4851 2023-07-16 13:02:14.729504 pydantic_apply-0.5.2/pydantic_apply/apply.py
--rw-r--r--   0        0        0        0 2023-07-16 13:02:14.729504 pydantic_apply-0.5.2/pydantic_apply/py.typed
--rw-r--r--   0        0        0      821 2023-07-16 13:02:14.729504 pydantic_apply-0.5.2/pydantic_apply/utils.py
--rw-r--r--   0        0        0      849 2023-07-16 13:02:14.729504 pydantic_apply-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 pydantic_apply-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-18 19:21:19.949882 pydantic_apply-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2258 2023-07-18 19:21:19.949882 pydantic_apply-0.5.4/README.md
+-rw-r--r--   0        0        0       35 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/__init__.py
+-rw-r--r--   0        0        0     2453 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/_compat.py
+-rw-r--r--   0        0        0     5153 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/apply.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/py.typed
+-rw-r--r--   0        0        0      821 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/utils.py
+-rw-r--r--   0        0        0      849 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 pydantic_apply-0.5.4/PKG-INFO
```

### Comparing `pydantic_apply-0.5.2/LICENSE` & `pydantic_apply-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.2/README.md` & `pydantic_apply-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.2/pydantic_apply/_compat.py` & `pydantic_apply-0.5.4/pydantic_apply/_compat.py`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.2/pydantic_apply/apply.py` & `pydantic_apply-0.5.4/pydantic_apply/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import warnings
 from typing import Any, Dict, Union
 
 import pydantic
 
 from pydantic_apply._compat import PydanticCompat
 from pydantic_apply.utils import is_pydantic_apply_annotation
 
 
 class ApplyModelMixin(pydantic.BaseModel):
     """Mixin to allow models to apply partly changes to their data."""
 
-    def apply(
+    def model_apply(
         self,
         changes: Union[pydantic.BaseModel, Dict[str, Any]],
     ) -> None:
         """Apply (partly) changes to the model data."""
 
         self_compat = PydanticCompat(self)
 
@@ -59,15 +60,15 @@
                     # When validation on assignment is enabled we need to
                     # copy the current value first. Otherwise, the validation
                     # might have issues, see below.
                     if self_compat.get_model_config_value("validate_assignment"):
                         current_value = PydanticCompat(current_value).model_copy()
 
                     # ...then use `.apply(...)` on the current value to prepare changes
-                    current_value.apply(changed_field_value)
+                    current_value.model_apply(changed_field_value)
                     prepared_changes[field_name] = current_value
                     continue
 
             # Default apply: Just set new value
             prepared_changes[field_name] = changed_field_value
 
         # Apply changes
@@ -104,7 +105,17 @@
             for field_name, field_value in prepared_changes.items():
                 setattr(self, field_name, field_value)
 
         finally:
             # Ensure whatever happens here, the validate_assignment flag is reset
             # to its original value.
             self_compat.set_model_config_value("validate_assignment", had_validate_assignment)
+
+    def apply(
+        self,
+        changes: Union[pydantic.BaseModel, Dict[str, Any]],
+    ) -> None:
+        warnings.warn(
+            "apply(...) is deprecated, use model_apply(...) instead",
+            DeprecationWarning,
+        )
+        self.model_apply(changes)
```

### Comparing `pydantic_apply-0.5.2/pydantic_apply/utils.py` & `pydantic_apply-0.5.4/pydantic_apply/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.2/pyproject.toml` & `pydantic_apply-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-apply"
-version = "0.5.2"
+version = "0.5.4"
 description = "Apply changes as patches to pydanic models."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-apply"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `pydantic_apply-0.5.2/PKG-INFO` & `pydantic_apply-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-apply
-Version: 0.5.2
+Version: 0.5.4
 Summary: Apply changes as patches to pydanic models.
 Home-page: https://github.com/team23/pydantic-apply
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

