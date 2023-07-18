# Comparing `tmp/fyCursor-0.1.4.2.tar.gz` & `tmp/fyCursor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.1.4.2.tar", last modified: Tue Jul 18 04:02:09 2023, max compression
+gzip compressed data, was "fyCursor-0.1.5.tar", last modified: Tue Jul 18 04:35:41 2023, max compression
```

## Comparing `fyCursor-0.1.4.2.tar` & `fyCursor-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:02:09.600367 fyCursor-0.1.4.2/fyCursor/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/fyCursor/core/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/core/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/fyCursor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-18 04:02:09.000000 fyCursor-0.1.4.2/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 04:02:09.000000 fyCursor-0.1.4.2/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:02:09.000000 fyCursor-0.1.4.2/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 04:02:09.000000 fyCursor-0.1.4.2/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:35:41.435805 fyCursor-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 04:35:27.000000 fyCursor-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-18 04:35:41.435805 fyCursor-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-18 04:35:27.000000 fyCursor-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:35:41.431805 fyCursor-0.1.5/fyCursor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:35:41.435805 fyCursor-0.1.5/fyCursor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/sql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:35:41.431805 fyCursor-0.1.5/fyCursor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-18 04:35:41.000000 fyCursor-0.1.5/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 04:35:41.000000 fyCursor-0.1.5/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:35:41.000000 fyCursor-0.1.5/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 04:35:41.000000 fyCursor-0.1.5/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:35:41.435805 fyCursor-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-18 04:35:27.000000 fyCursor-0.1.5/setup.py
```

### Comparing `fyCursor-0.1.4.2/LICENSE` & `fyCursor-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.4.2/PKG-INFO` & `fyCursor-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.4.2
+Version: 0.1.5
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,15 +26,17 @@
 - New fyCursor methods:
     - create_table (BETA)
 - Table and Fields (‼️ BETA):
     - Table class:
         - TableError
         - ``insert`` method
         - ``create`` method
+        
     - Field class
+        - Field types
 - Type hints
 
 ### 🎎 v0.0.1 to v0.0.3
 - Basic fyCursor methods:
     - add
     - set
     - update
```

### Comparing `fyCursor-0.1.4.2/README.md` & `fyCursor-0.1.5/fyCursor.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: fyCursor
+Version: 0.1.5
+Summary: Simple sqlite3 cursor
+Author: felixyeahh
+Author-email: <felixyeah@outlook.com>
+License: MIT
+Keywords: python,sqlite3,database
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # fyCursor
 A simple cursor for managing sqlite3 databases
 
 ## Installation 
 You can simply use pip: &nbsp;
 \$`pip3 install fyCursor`
 
@@ -14,15 +26,17 @@
 - New fyCursor methods:
     - create_table (BETA)
 - Table and Fields (‼️ BETA):
     - Table class:
         - TableError
         - ``insert`` method
         - ``create`` method
+        
     - Field class
+        - Field types
 - Type hints
 
 ### 🎎 v0.0.1 to v0.0.3
 - Basic fyCursor methods:
     - add
     - set
     - update
```

### Comparing `fyCursor-0.1.4.2/fyCursor/__init__.py` & `fyCursor-0.1.5/fyCursor/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,23 @@
     fyCursor,
     Table,
     Field,
     TableError,
     TableInsert,
     NULL
 )
+from sql_types import (
+    DATATYPES,
+    INTEGER,
+    TEXT,
+    DATETIME,
+    VARCHAR,
+    BOOL,
+    TIMESTAMP
+)
 
 
 def connect(
     database: _os.PathLike[_typing.Any] | str,
 ) -> 'fyCursor':
     """
     Connect database and return cursor
@@ -32,15 +41,15 @@
         database=database,
     )
     return connection.cursor(fyCursor)  # type: ignore
 
 
 __title__ = "fyCursor"
 
-__version__ = "0.1.4.2"
+__version__ = "0.1.5"
 
 __author__ = "felixyeahh"
 __author_email__ = "<felixyeah@outlook.com>"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Baffu Team"
 
@@ -63,14 +72,21 @@
     "fyCursor",
     "Info",
     "Table",
     "Field",
     "TableError",
     "TableInsert",
     "NULL",
+    "DATATYPES",
+    "INTEGER",
+    "TEXT",
+    "DATETIME",
+    "VARCHAR",
+    "BOOL",
+    "TIMESTAMP",
     "__title__",
     "__version__",
     "__author__",
     "__author_email__",
     "__license__",
     "__copyright__",
     "__description__"
```

### Comparing `fyCursor-0.1.4.2/fyCursor/__main__.py` & `fyCursor-0.1.5/fyCursor/__main__.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.4.2/fyCursor/core/core.py` & `fyCursor-0.1.5/fyCursor/core/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # pyright: reportPrivateUsage=false
 import sqlite3
 import logging
 
 from .fields import Field
-from typing import Union, Any, Optional, TypeVar
+from typing import Union, Any, Optional
 
-T = TypeVar("T")
 NULL = None  # python None is same as "NULL" here
 
 
 class TableError(BaseException):
     """Raised if something went wrong while creating a table class"""
 
 
@@ -78,24 +77,32 @@
         values = ""
         for item in values_:
             values += generate_name(item)
 
         self.cursor.execute(
             f"INSERT INTO {self.name}({names[:-1]}) VALUES ({values[:-1]})"
         )
+        self.cursor.commit()
 
         return self
 
     def __lshift__(self, __b: dict[str, Any]) -> "Table":
         """Insert dict using left shift (<<) operator"""
         if not isinstance(__b, dict):  # type: ignore
             raise TableError("Wrong arguments")
         self.insert(**__b)
         return self
 
+    def __rshift__(self, __b: dict[str, Any]) -> "Table":
+        """Insert dict using right shift (>>) operator"""
+        if not isinstance(__b, dict):  # type: ignore
+            raise TableError("Wrong arguments")
+        self.insert(**__b)
+        return self
+
     def get_values(self) -> dict[str, Field]:
         return self._fields
 
     def create(self, if_not_exist: bool = False) -> "Table":
         return self.cursor.create_table(self, if_not_exist)
 
 
@@ -115,14 +122,15 @@
         Initialise a cursor.
 
         :param __cursor - sqlite3 connection
         :param logger - custom logger (Optional)
         """
         self.null = NULL
         self.NULL = self.null
+        self._query = None
 
         super().__init__(__cursor)
         self._logger = logging.getLogger(
             "fyCursor"
         ) if logger is None else logger
 
     def update(self, table: str) -> 'fyCursor':
@@ -190,15 +198,15 @@
         """
         self._query = f"SELECT {value}"
         if from_ is not None:
             self._from(from_)
         return self
 
     def _from(self, table: str) -> 'fyCursor':
-        self._query += f" FROM {table}"
+        self._query += f"FROM {table}"  # type: ignore
         return self
 
     def where(self, **kwargs: Any) -> 'fyCursor':
         if not self._query:
             raise sqlite3.ProgrammingError(
                 "You should use something before `where`"
             )
@@ -266,9 +274,10 @@
         fields = _prepare(insert.args)
         values_ = _prepare(values)
 
         super().execute(f"""
             INSERT INTO TABLE {insert.table.name} ({fields})
             VALUES ({values_})
         """)
+        super().connection.commit()
 
         return insert.table
```

### Comparing `fyCursor-0.1.4.2/fyCursor/core/fields.py` & `fyCursor-0.1.5/fyCursor/core/fields.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from typing import Optional, Any
+from ..sql_types import DATATYPES
 
 
 def _pass() -> str:
     return ''
 
 
 class Field():
     def __init__(
         self,
         name: Optional[str] = None,
         default: Any = None,
         nullable: bool = True,
-        primary_key: bool = False
+        primary_key: bool = False,
+        type: str = DATATYPES.TEXT
     ) -> None:
         self.name = name
         self.primary_key = primary_key
         self.default = default
         self.nullable = nullable
+        self.type = type
 
     def _generate_field(self) -> str:
         self._field = self.name or ''
+        self._field += self.type
         self._field += " PRIMARY KEY" if self.primary_key else _pass()
         self._field += (
             f"DEFAULT \"{self.default}\"" if self.default else _pass()
         )
         self._field += _pass() if self.nullable else " NOT NULL"
 
         return self._field
```

### Comparing `fyCursor-0.1.4.2/setup.py` & `fyCursor-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 # Setting up
 setup(
     name="fyCursor",
-    version="0.1.4.2",
+    version="0.1.5",
     description='Simple sqlite3 cursor',
     author="felixyeahh",
     author_email="<felixyeah@outlook.com>",
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

