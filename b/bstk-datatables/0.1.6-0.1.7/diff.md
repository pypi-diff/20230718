# Comparing `tmp/bstk_datatables-0.1.6.tar.gz` & `tmp/bstk_datatables-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_datatables-0.1.6.tar", max compression
+gzip compressed data, was "bstk_datatables-0.1.7.tar", max compression
```

## Comparing `bstk_datatables-0.1.6.tar` & `bstk_datatables-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4244 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/README.md
--rw-r--r--   0        0        0     2358 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/__init__.py
--rw-r--r--   0        0        0     2311 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/entry.py
--rw-r--r--   0        0        0      560 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/enum.py
--rw-r--r--   0        0        0     3248 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/merge.py
--rw-r--r--   0        0        0     6968 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/schema.py
--rw-r--r--   0        0        0     1565 2023-07-04 06:48:59.690092 bstk_datatables-0.1.6/bstk_datatables/table.py
--rw-r--r--   0        0        0      669 2023-07-04 06:49:21.782220 bstk_datatables-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4244 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/README.md
+-rw-r--r--   0        0        0     2358 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/__init__.py
+-rw-r--r--   0        0        0     2311 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/entry.py
+-rw-r--r--   0        0        0      560 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/enum.py
+-rw-r--r--   0        0        0     3248 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/merge.py
+-rw-r--r--   0        0        0     7133 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/schema.py
+-rw-r--r--   0        0        0     1565 2023-07-18 01:23:17.068178 bstk_datatables-0.1.7/bstk_datatables/table.py
+-rw-r--r--   0        0        0      669 2023-07-18 01:23:42.316528 bstk_datatables-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.1.7/PKG-INFO
```

### Comparing `bstk_datatables-0.1.6/README.md` & `bstk_datatables-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.6/bstk_datatables/__init__.py` & `bstk_datatables-0.1.7/bstk_datatables/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.6/bstk_datatables/entry.py` & `bstk_datatables-0.1.7/bstk_datatables/entry.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.6/bstk_datatables/enum.py` & `bstk_datatables-0.1.7/bstk_datatables/enum.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.6/bstk_datatables/merge.py` & `bstk_datatables-0.1.7/bstk_datatables/merge.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.6/bstk_datatables/schema.py` & `bstk_datatables-0.1.7/bstk_datatables/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         return rtn
 
 
 @dataclass
 class SchemaField:
     name: typing.AnyStr
     format: SchemaFieldFormat
+    description: typing.AnyStr = field(default=None)
     code: typing.AnyStr = field(default=None)
     _value: typing.Any = field(init=False, default=None)
 
     def __post_init__(self):
         if not self.code:
             self.code = name_to_code(self.name)
 
@@ -125,19 +126,22 @@
         return self._value
 
     @value.setter
     def value(self, value):
         self._value = value
 
     def export(self) -> typing.Dict[typing.AnyStr, typing.Any]:
-        return {
+        _rtn = {
             "name": self.__dict__["name"],
             "code": self.__dict__["code"],
             "format": self.format.export(),
         }
+        if self.description:
+            _rtn["description"] = self.__dict__["description"]
+        return _rtn
 
 
 @dataclass
 class SchemaFieldFormat:
     type: typing.Optional[typing.AnyStr]
     values: typing.Optional[typing.Any] = None
     lookup: typing.Optional[typing.Any] = None
```

### Comparing `bstk_datatables-0.1.6/bstk_datatables/table.py` & `bstk_datatables-0.1.7/bstk_datatables/table.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.1.6/pyproject.toml` & `bstk_datatables-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk-datatables"
-version = "0.1.6"
+version = "0.1.7"
 description = "A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!"
 authors = ["colin <colin@broadstack.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bstk_datatables" }]
 
 [tool.poetry.dependencies]
```

### Comparing `bstk_datatables-0.1.6/PKG-INFO` & `bstk_datatables-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk-datatables
-Version: 0.1.6
+Version: 0.1.7
 Summary: A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!
 License: MIT
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

