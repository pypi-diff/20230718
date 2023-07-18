# Comparing `tmp/fyCursor-0.1.5.tar.gz` & `tmp/fyCursor-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.1.5.tar", last modified: Tue Jul 18 04:35:41 2023, max compression
+gzip compressed data, was "fyCursor-0.1.5.1.tar", last modified: Tue Jul 18 04:56:42 2023, max compression
```

## Comparing `fyCursor-0.1.5.tar` & `fyCursor-0.1.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:35:41.435805 fyCursor-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 04:35:27.000000 fyCursor-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-18 04:35:41.435805 fyCursor-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-18 04:35:27.000000 fyCursor-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:35:41.431805 fyCursor-0.1.5/fyCursor/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:35:41.435805 fyCursor-0.1.5/fyCursor/core/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-18 04:35:27.000000 fyCursor-0.1.5/fyCursor/sql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:35:41.431805 fyCursor-0.1.5/fyCursor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-18 04:35:41.000000 fyCursor-0.1.5/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 04:35:41.000000 fyCursor-0.1.5/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:35:41.000000 fyCursor-0.1.5/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 04:35:41.000000 fyCursor-0.1.5/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:35:41.435805 fyCursor-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-18 04:35:27.000000 fyCursor-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:56:42.932288 fyCursor-0.1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 04:56:31.000000 fyCursor-0.1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-18 04:56:42.932288 fyCursor-0.1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-18 04:56:31.000000 fyCursor-0.1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:56:42.932288 fyCursor-0.1.5.1/fyCursor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-18 04:56:31.000000 fyCursor-0.1.5.1/fyCursor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 04:56:31.000000 fyCursor-0.1.5.1/fyCursor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:56:42.932288 fyCursor-0.1.5.1/fyCursor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-18 04:56:31.000000 fyCursor-0.1.5.1/fyCursor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-18 04:56:31.000000 fyCursor-0.1.5.1/fyCursor/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-18 04:56:31.000000 fyCursor-0.1.5.1/fyCursor/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-18 04:56:31.000000 fyCursor-0.1.5.1/fyCursor/sql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:56:42.932288 fyCursor-0.1.5.1/fyCursor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-18 04:56:42.000000 fyCursor-0.1.5.1/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 04:56:42.000000 fyCursor-0.1.5.1/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:56:42.000000 fyCursor-0.1.5.1/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 04:56:42.000000 fyCursor-0.1.5.1/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:56:42.932288 fyCursor-0.1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-18 04:56:31.000000 fyCursor-0.1.5.1/setup.py
```

### Comparing `fyCursor-0.1.5/LICENSE` & `fyCursor-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.5/PKG-INFO` & `fyCursor-0.1.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.5/README.md` & `fyCursor-0.1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.5/fyCursor/__init__.py` & `fyCursor-0.1.5.1/fyCursor/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     fyCursor,
     Table,
     Field,
     TableError,
     TableInsert,
     NULL
 )
-from sql_types import (
+from .sql_types import (
     DATATYPES,
     INTEGER,
     TEXT,
     DATETIME,
     VARCHAR,
     BOOL,
     TIMESTAMP
@@ -41,15 +41,15 @@
         database=database,
     )
     return connection.cursor(fyCursor)  # type: ignore
 
 
 __title__ = "fyCursor"
 
-__version__ = "0.1.5"
+__version__ = "0.1.5.1"
 
 __author__ = "felixyeahh"
 __author_email__ = "<felixyeah@outlook.com>"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Baffu Team"
```

### Comparing `fyCursor-0.1.5/fyCursor/__main__.py` & `fyCursor-0.1.5.1/fyCursor/__main__.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.5/fyCursor/core/core.py` & `fyCursor-0.1.5.1/fyCursor/core/core.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.5/fyCursor/core/fields.py` & `fyCursor-0.1.5.1/fyCursor/core/fields.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.5/fyCursor.egg-info/PKG-INFO` & `fyCursor-0.1.5.1/fyCursor.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fyCursor-0.1.5/setup.py` & `fyCursor-0.1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 # Setting up
 setup(
     name="fyCursor",
-    version="0.1.5",
+    version="0.1.5.1",
     description='Simple sqlite3 cursor',
     author="felixyeahh",
     author_email="<felixyeah@outlook.com>",
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

