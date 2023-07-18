# Comparing `tmp/fyCursor-0.1.4.1.tar.gz` & `tmp/fyCursor-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.1.4.1.tar", last modified: Tue Jul 18 03:34:28 2023, max compression
+gzip compressed data, was "fyCursor-0.1.4.2.tar", last modified: Tue Jul 18 04:02:09 2023, max compression
```

## Comparing `fyCursor-0.1.4.1.tar` & `fyCursor-0.1.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:34:28.101484 fyCursor-0.1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 03:34:13.000000 fyCursor-0.1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-18 03:34:28.097484 fyCursor-0.1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 03:34:13.000000 fyCursor-0.1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:34:28.097484 fyCursor-0.1.4.1/fyCursor/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-18 03:34:13.000000 fyCursor-0.1.4.1/fyCursor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 03:34:13.000000 fyCursor-0.1.4.1/fyCursor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:34:28.097484 fyCursor-0.1.4.1/fyCursor/core/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 03:34:13.000000 fyCursor-0.1.4.1/fyCursor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-18 03:34:13.000000 fyCursor-0.1.4.1/fyCursor/core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-18 03:34:13.000000 fyCursor-0.1.4.1/fyCursor/core/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:34:28.097484 fyCursor-0.1.4.1/fyCursor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-18 03:34:28.000000 fyCursor-0.1.4.1/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 03:34:28.000000 fyCursor-0.1.4.1/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:34:28.000000 fyCursor-0.1.4.1/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 03:34:28.000000 fyCursor-0.1.4.1/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:34:28.101484 fyCursor-0.1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-18 03:34:13.000000 fyCursor-0.1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:02:09.600367 fyCursor-0.1.4.2/fyCursor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/fyCursor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/fyCursor/core/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/fyCursor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-18 04:02:09.000000 fyCursor-0.1.4.2/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 04:02:09.000000 fyCursor-0.1.4.2/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:02:09.000000 fyCursor-0.1.4.2/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 04:02:09.000000 fyCursor-0.1.4.2/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:02:09.604367 fyCursor-0.1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-18 04:01:55.000000 fyCursor-0.1.4.2/setup.py
```

### Comparing `fyCursor-0.1.4.1/LICENSE` & `fyCursor-0.1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.4.1/PKG-INFO` & `fyCursor-0.1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.4.1/README.md` & `fyCursor-0.1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.4.1/fyCursor/__init__.py` & `fyCursor-0.1.4.2/fyCursor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         database=database,
     )
     return connection.cursor(fyCursor)  # type: ignore
 
 
 __title__ = "fyCursor"
 
-__version__ = "0.1.4.1"
+__version__ = "0.1.4.2"
 
 __author__ = "felixyeahh"
 __author_email__ = "<felixyeah@outlook.com>"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Baffu Team"
```

### Comparing `fyCursor-0.1.4.1/fyCursor/__main__.py` & `fyCursor-0.1.4.2/fyCursor/__main__.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.4.1/fyCursor/core/core.py` & `fyCursor-0.1.4.2/fyCursor/core/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             self._table.append(value._generate_field())
 
     def insert(self, **kwargs: Any) -> "Table":
         names_ = list(kwargs.keys())
         values_ = list(kwargs.values())
 
         def generate_name(name: str):
-            return f"{name},"
+            return f"\"{name}\","
 
         names = ""
         for item in names_:
             names += generate_name(item)
 
         values = ""
         for item in values_:
@@ -247,14 +247,15 @@
         if_not_exist: bool = False
     ) -> "Table":
         exist = "IF NOT EXISTS" if if_not_exist else ""
         super().execute(f"""
             CREATE TABLE {exist}\
              {table.name}({table._sql[:-1]})
         """)
+        super().connection.commit()
 
         return table
 
     def insert_into(self, insert: "TableInsert", *values: Any) -> Table:
         def _prepare(args: tuple[Any]) -> str:
             values = str()
             for arg in args:
```

### Comparing `fyCursor-0.1.4.1/fyCursor/core/fields.py` & `fyCursor-0.1.4.2/fyCursor/core/fields.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.4.1/fyCursor.egg-info/PKG-INFO` & `fyCursor-0.1.4.2/fyCursor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.4.1/setup.py` & `fyCursor-0.1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 # Setting up
 setup(
     name="fyCursor",
-    version="0.1.4.1",
+    version="0.1.4.2",
     description='Simple sqlite3 cursor',
     author="felixyeahh",
     author_email="<felixyeah@outlook.com>",
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

