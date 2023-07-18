# Comparing `tmp/namespace_mahdimir-2.4.0.tar.gz` & `tmp/namespace_mahdimir-2.4.1.tar.gz`

## Comparing `namespace_mahdimir-2.4.0.tar` & `namespace_mahdimir-2.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.0/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.0/src/namespace_mahdimir/__init__.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.0/src/namespace_mahdimir/tse.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.0/src/namespace_mahdimir/tse_github_data_url.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.0/README.md
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/src/namespace_mahdimir/__init__.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/src/namespace_mahdimir/tse.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/src/namespace_mahdimir/tse_github_data_url.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/README.md
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 namespace_mahdimir-2.4.1/PKG-INFO
```

### Comparing `namespace_mahdimir-2.4.0/src/namespace_mahdimir/tse.py` & `namespace_mahdimir-2.4.1/src/namespace_mahdimir/tse.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     nlst = 'NomLast'
     nopn = 'NomOpen'
     nystrd = 'NomYesterdayClose'
     val = 'Value'
     vol = 'Volume'
     trd_count = 'TradeCount'
 
-class DOutstandingShares :
+class DOutstandingSharesCol :
     _c = Col()
 
     # cols from Col
     ftic = _c.ftic
     tse_id = _c.tse_id
     d = _c.d
     jd = _c.jd
```

### Comparing `namespace_mahdimir-2.4.0/src/namespace_mahdimir/tse_github_data_url.py` & `namespace_mahdimir-2.4.1/src/namespace_mahdimir/tse_github_data_url.py`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-2.4.0/.gitignore` & `namespace_mahdimir-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-2.4.0/LICENSE` & `namespace_mahdimir-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-2.4.0/pyproject.toml` & `namespace_mahdimir-2.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "namespace_mahdimir"
-version = "2.4.0"
+version = "2.4.1"
 authors = [{ name = "Mahdi Mir", email = "imahdimir@gmail.com" }]
 description = "Some Namespaces for Python"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
 
 ]
```

### Comparing `namespace_mahdimir-2.4.0/PKG-INFO` & `namespace_mahdimir-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namespace_mahdimir
-Version: 2.4.0
+Version: 2.4.1
 Summary: Some Namespaces for Python
 Project-URL: Homepage, https://github.com/imahdimir/namespace_mahdimir
 Project-URL: Bug Tracker, https://github.com/imahdimir/namespace_mahdimir/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
```

