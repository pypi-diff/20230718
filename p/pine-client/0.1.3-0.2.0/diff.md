# Comparing `tmp/pine_client-0.1.3.tar.gz` & `tmp/pine_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pine_client-0.1.3.tar", max compression
+gzip compressed data, was "pine_client-0.2.0.tar", max compression
```

## Comparing `pine_client-0.1.3.tar` & `pine_client-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       95 2023-05-09 17:02:12.000000 pine_client-0.1.3/README.md
--rw-r--r--   0        0        0       60 2023-05-09 17:02:12.000000 pine_client-0.1.3/pine_client/__init__.py
--rw-r--r--   0        0        0    32329 2023-05-09 17:02:12.000000 pine_client-0.1.3/pine_client/client.py
--rw-r--r--   0        0        0     2659 2023-05-09 17:02:12.000000 pine_client-0.1.3/pine_client/utils.py
--rw-r--r--   0        0        0      505 2023-05-09 17:02:27.000000 pine_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 pine_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       95 2023-07-18 14:16:26.828669 pine_client-0.2.0/README.md
+-rw-r--r--   0        0        0       60 2023-07-18 14:16:26.828669 pine_client-0.2.0/pine_client/__init__.py
+-rw-r--r--   0        0        0    33672 2023-07-18 14:16:26.828669 pine_client-0.2.0/pine_client/client.py
+-rw-r--r--   0        0        0     2659 2023-07-18 14:16:26.828669 pine_client-0.2.0/pine_client/utils.py
+-rw-r--r--   0        0        0      505 2023-07-18 14:16:26.828669 pine_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 pine_client-0.2.0/PKG-INFO
```

### Comparing `pine_client-0.1.3/pine_client/client.py` & `pine_client-0.2.0/pine_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,26 @@
 FilterArray = List[Filter]
 
 # TODO: improve raw filter typing as it can be more than a string and use $string
 RawFilter = str
 
 Lambda = TypedDict("Lambda", {"$alias": str, "$expr": Filter})
 
+DurationValue = TypedDict(
+    "DurationValue",
+    {
+        "negative": bool,
+        "days": float,
+        "hours": float,
+        "minutes": float,
+        "seconds": float,
+    },
+    total=False,
+)
+
 FilterObj = TypedDict(
     "FilterObj",
     {
         "@": str,
         "$raw": RawFilter,
         "$": Union[str, List[str]],
         "$count": Filter,
@@ -78,14 +90,15 @@
         "$minute": FilterFunctionValue,
         "$second": FilterFunctionValue,
         "$fractionalseconds": FilterFunctionValue,
         "$date": FilterFunctionValue,
         "$time": FilterFunctionValue,
         "$totaloffsetminutes": FilterFunctionValue,
         "$now": FilterFunctionValue,
+        "$duration": DurationValue,
         "$maxdatetime": FilterFunctionValue,
         "$mindatetime": FilterFunctionValue,
         "$totalseconds": FilterFunctionValue,
         "$round": FilterFunctionValue,
         "$floor": FilterFunctionValue,
         "$ceiling": FilterFunctionValue,
         "$isof": FilterFunctionValue,
@@ -210,14 +223,20 @@
 #     "$format": str,
 #     "$index": Index
 # }, total=False)
 ODataOptions = AnyObject
 
 OptionTypes = Union[Filter, Expand, OrderBy, int, str, List[str], ParameterAlias]
 
+duration_timepart_flag_entries = (
+    ("hours", "H"),
+    ("minutes", "M"),
+    ("seconds", "S"),
+)
+
 
 class Params(TypedDict, total=False):
     api_prefix: str
     method: ODataMethod
     resource: str
     id: ResourceId
     url: str
@@ -605,14 +624,45 @@
         "$round",
         "$floor",
         "$ceiling",
         "$isof",
         "$cast",
     ]:
         return filter_function(filter, cast(FilterFunctionKey, operator), parent_key)
+
+    elif operator == "$duration":
+        if not isinstance(filter, dict):
+            raise Exception(f"Expected type for {operator}, got: {type(filter)}")
+
+        duration_value = cast(DurationValue, filter)
+        duration_string = "P"
+
+        days = duration_value.get("days")
+        if days is not None:
+            duration_string += f"{days}D"
+
+        time_part = ""
+        for part_key, part_flag in duration_timepart_flag_entries:
+            key = duration_value.get(part_key)
+            if key is not None:
+                time_part += f"{key}{part_flag}"
+
+        if len(time_part) > 0:
+            duration_string += f"T{time_part}"
+
+        if len(duration_string) <= 1:
+            raise Exception(
+                f"Expected {operator} to include duration properties, got: {type(filter)}"
+            )
+
+        if duration_value.get("negative"):
+            duration_string = f"-{duration_string}"
+
+        return add_parent_key(f"duration'{duration_string}'", parent_key)
+
     elif operator == "$raw":
         if isinstance(filter, str):
             f = f"({filter})"
             return add_parent_key(f, parent_key)
         elif not is_primitive(filter):
             if isinstance(filter, list):
                 raw_filter = filter[0]  # type: ignore
```

### Comparing `pine_client-0.1.3/pine_client/utils.py` & `pine_client-0.2.0/pine_client/utils.py`

 * *Files identical despite different names*

### Comparing `pine_client-0.1.3/PKG-INFO` & `pine_client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pine-client
-Version: 0.1.3
+Version: 0.2.0
 Summary: This module provides the core layer for python interface for the pinejs API
 Author: Balena
 Author-email: info@balena.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

