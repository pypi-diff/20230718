# Comparing `tmp/fyCursor-0.1.3.tar.gz` & `tmp/fyCursor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.1.3.tar", last modified: Fri Jun 30 14:01:36 2023, max compression
+gzip compressed data, was "fyCursor-0.1.4.tar", last modified: Tue Jul 18 03:21:19 2023, max compression
```

## Comparing `fyCursor-0.1.3.tar` & `fyCursor-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:01:36.754741 fyCursor-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 14:01:25.000000 fyCursor-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 14:01:36.754741 fyCursor-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-30 14:01:25.000000 fyCursor-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:01:36.754741 fyCursor-0.1.3/fyCursor/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:01:36.754741 fyCursor-0.1.3/fyCursor/core/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-30 14:01:25.000000 fyCursor-0.1.3/fyCursor/core/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:01:36.754741 fyCursor-0.1.3/fyCursor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 14:01:36.000000 fyCursor-0.1.3/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-30 14:01:36.000000 fyCursor-0.1.3/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:01:36.000000 fyCursor-0.1.3/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 14:01:36.000000 fyCursor-0.1.3/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:01:36.754741 fyCursor-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-30 14:01:25.000000 fyCursor-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:21:19.429620 fyCursor-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 03:21:05.000000 fyCursor-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-18 03:21:19.429620 fyCursor-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 03:21:05.000000 fyCursor-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:21:19.429620 fyCursor-0.1.4/fyCursor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-18 03:21:05.000000 fyCursor-0.1.4/fyCursor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 03:21:05.000000 fyCursor-0.1.4/fyCursor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:21:19.429620 fyCursor-0.1.4/fyCursor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-18 03:21:05.000000 fyCursor-0.1.4/fyCursor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-18 03:21:05.000000 fyCursor-0.1.4/fyCursor/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-18 03:21:05.000000 fyCursor-0.1.4/fyCursor/core/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:21:19.429620 fyCursor-0.1.4/fyCursor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-18 03:21:19.000000 fyCursor-0.1.4/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 03:21:19.000000 fyCursor-0.1.4/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:21:19.000000 fyCursor-0.1.4/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 03:21:19.000000 fyCursor-0.1.4/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:21:19.429620 fyCursor-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-18 03:21:05.000000 fyCursor-0.1.4/setup.py
```

### Comparing `fyCursor-0.1.3/LICENSE` & `fyCursor-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.3/PKG-INFO` & `fyCursor-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.3/README.md` & `fyCursor-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.3/fyCursor/__init__.py` & `fyCursor-0.1.4/fyCursor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import sqlite3 as _sq3
 import typing as _typing
 import os as _os
+
 from .core import (
     fyCursor,
     Table,
     Field,
-    TableError
+    TableError,
+    NULL
 )
 
 
 def connect(
     database: _os.PathLike[_typing.Any] | str,
 ) -> 'fyCursor':
     """
@@ -29,15 +31,15 @@
         database=database,
     )
     return connection.cursor(fyCursor)  # type: ignore
 
 
 __title__ = "fyCursor"
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 __author__ = "felixyeahh"
 __author_email__ = "<felixyeah@outlook.com>"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Baffu Team"
 
@@ -58,14 +60,15 @@
 __all__ = [
     "connect",
     "fyCursor",
     "Info",
     "Table",
     "Field",
     "TableError",
+    "NULL",
     "__title__",
     "__version__",
     "__author__",
     "__author_email__",
     "__license__",
     "__copyright__",
     "__description__"
```

### Comparing `fyCursor-0.1.3/fyCursor/__main__.py` & `fyCursor-0.1.4/fyCursor/__main__.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.3/fyCursor/core/core.py` & `fyCursor-0.1.4/fyCursor/core/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 # pyright: reportPrivateUsage=false
 import sqlite3
 import logging
 
 from .fields import Field
-from typing import Union, Any, Optional
+from typing import Union, Any, Optional, TypeVar
+
+T = TypeVar("T")
+NULL = None  # python None is same as "NULL" here
 
 
 class TableError(BaseException):
     """Raised if something went wrong while creating a table class"""
 
 
+class TableInsert():
+    def __init__(
+        self,
+        table: "Table",
+        *args: str
+    ) -> None:
+        self.table = table
+        self.args = args
+
+
 class Table():
     def __init__(
         self,
         name: str,
         cursor: "fyCursor",
         args_fields: Optional[list[Field]] = None,
         kwargs_fields: Optional[dict[str, Field]] = None
@@ -68,14 +81,21 @@
 
         self.cursor.execute(
             f"INSERT INTO {self.name}({names[:-1]}) VALUES ({values[:-1]})"
         )
 
         return self
 
+    def __lshift__(self, __b: dict[str, Any]) -> "Table":
+        """Insert dict using left shift (<<) operator"""
+        if not isinstance(__b, dict):  # type: ignore
+            raise TableError("Wrong arguments")
+        self.insert(**__b)
+        return self
+
     def get_values(self) -> dict[str, Field]:
         return self._fields
 
     def create(self, if_not_exist: bool = False) -> "Table":
         return self.cursor.create_table(self, if_not_exist)
 
 
@@ -93,14 +113,17 @@
     ) -> None:
         """
         Initialise a cursor.
 
         :param __cursor - sqlite3 connection
         :param logger - custom logger (Optional)
         """
+        self.null = NULL
+        self.NULL = self.null
+
         super().__init__(__cursor)
         self._logger = logging.getLogger(
             "fyCursor"
         ) if logger is None else logger
 
     def update(self, table: str) -> 'fyCursor':
         """
@@ -226,7 +249,25 @@
         exist = "IF NOT EXISTS" if if_not_exist else ""
         super().execute(f"""
             CREATE TABLE {exist}\
              {table.name}({table._sql[:-1]})
         """)
 
         return table
+
+    def insert_into(self, insert: "TableInsert", *values: Any) -> Table:
+        def _prepare(args: tuple[Any]) -> str:
+            values = str()
+            for arg in args:
+                values += f"{arg} ,"
+            values = values[:-1]
+            return values
+
+        fields = _prepare(insert.args)
+        values_ = _prepare(values)
+
+        super().execute(f"""
+            INSERT INTO TABLE {insert.table.name} ({fields})
+            VALUES ({values_})
+        """)
+
+        return insert.table
```

### Comparing `fyCursor-0.1.3/fyCursor/core/fields.py` & `fyCursor-0.1.4/fyCursor/core/fields.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.3/fyCursor.egg-info/PKG-INFO` & `fyCursor-0.1.4/fyCursor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.3/setup.py` & `fyCursor-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 # Setting up
 setup(
     name="fyCursor",
-    version="0.1.3",
+    version="0.1.4",
     description='Simple sqlite3 cursor',
     author="felixyeahh",
     author_email="<felixyeah@outlook.com>",
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

