# Comparing `tmp/camminapy-1.1.8.tar.gz` & `tmp/camminapy-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camminapy-1.1.8.tar", max compression
+gzip compressed data, was "camminapy-1.1.9.tar", max compression
```

## Comparing `camminapy-1.1.8.tar` & `camminapy-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-05-25 18:22:20.279949 camminapy-1.1.8/LICENSE
--rw-r--r--   0        0        0      361 2023-05-26 10:37:06.478390 camminapy-1.1.8/README.md
--rw-r--r--   0        0        0      119 2023-05-26 10:37:06.478678 camminapy-1.1.8/camminapy/__init__.py
--rw-r--r--   0        0        0      343 2023-05-25 18:22:20.280553 camminapy-1.1.8/camminapy/data/__init__.py
--rw-r--r--   0        0        0     6671 2023-07-18 06:14:58.928442 camminapy-1.1.8/camminapy/data/resample.py
--rw-r--r--   0        0        0      163 2023-05-25 18:22:20.280877 camminapy-1.1.8/camminapy/plot/__init__.py
--rw-r--r--   0        0        0     1085 2023-05-25 18:22:20.280996 camminapy-1.1.8/camminapy/plot/altair_config.py
--rw-r--r--   0        0        0     6242 2023-05-25 18:43:33.297938 camminapy-1.1.8/camminapy/plot/altair_theme.py
--rw-r--r--   0        0        0     2633 2023-05-25 18:22:20.281263 camminapy-1.1.8/camminapy/plot/footer.py
--rw-r--r--   0        0        0        0 2023-05-25 18:22:20.281378 camminapy-1.1.8/camminapy/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-05-25 18:22:20.281505 camminapy-1.1.8/camminapy/utils/config.py
--rw-r--r--   0        0        0      734 2023-05-26 07:06:53.398496 camminapy-1.1.8/camminapy/utils/logger.py
--rw-r--r--   0        0        0     1125 2023-07-18 06:18:42.874319 camminapy-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 camminapy-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-25 18:22:20.279949 camminapy-1.1.9/LICENSE
+-rw-r--r--   0        0        0      361 2023-05-26 10:37:06.478390 camminapy-1.1.9/README.md
+-rw-r--r--   0        0        0      119 2023-05-26 10:37:06.478678 camminapy-1.1.9/camminapy/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-25 18:22:20.280553 camminapy-1.1.9/camminapy/data/__init__.py
+-rw-r--r--   0        0        0     6671 2023-07-18 06:14:58.928442 camminapy-1.1.9/camminapy/data/resample.py
+-rw-r--r--   0        0        0      163 2023-05-25 18:22:20.280877 camminapy-1.1.9/camminapy/plot/__init__.py
+-rw-r--r--   0        0        0     1085 2023-05-25 18:22:20.280996 camminapy-1.1.9/camminapy/plot/altair_config.py
+-rw-r--r--   0        0        0     6242 2023-05-25 18:43:33.297938 camminapy-1.1.9/camminapy/plot/altair_theme.py
+-rw-r--r--   0        0        0     2633 2023-05-25 18:22:20.281263 camminapy-1.1.9/camminapy/plot/footer.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:22:20.281378 camminapy-1.1.9/camminapy/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-25 18:22:20.281505 camminapy-1.1.9/camminapy/utils/config.py
+-rw-r--r--   0        0        0      734 2023-05-26 07:06:53.398496 camminapy-1.1.9/camminapy/utils/logger.py
+-rw-r--r--   0        0        0     1125 2023-07-18 06:22:35.596182 camminapy-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 camminapy-1.1.9/PKG-INFO
```

### Comparing `camminapy-1.1.8/LICENSE` & `camminapy-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.8/camminapy/data/resample.py` & `camminapy-1.1.9/camminapy/data/resample.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.8/camminapy/plot/altair_config.py` & `camminapy-1.1.9/camminapy/plot/altair_config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.8/camminapy/plot/altair_theme.py` & `camminapy-1.1.9/camminapy/plot/altair_theme.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.8/camminapy/plot/footer.py` & `camminapy-1.1.9/camminapy/plot/footer.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.8/camminapy/utils/config.py` & `camminapy-1.1.9/camminapy/utils/config.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.8/camminapy/utils/logger.py` & `camminapy-1.1.9/camminapy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `camminapy-1.1.8/pyproject.toml` & `camminapy-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camminapy"
-version = "1.1.8"
+version = "1.1.9"
 description = "My personal code collection."
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 readme = "README.md"
 repository = "https://github.com/thomascamminady/camminapy"
 homepage = "https://thomascamminady.github.io/camminapy/camminapy.html"
 
 [tool.poetry.dependencies]
```

### Comparing `camminapy-1.1.8/PKG-INFO` & `camminapy-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camminapy
-Version: 1.1.8
+Version: 1.1.9
 Summary: My personal code collection.
 Home-page: https://thomascamminady.github.io/camminapy/camminapy.html
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

