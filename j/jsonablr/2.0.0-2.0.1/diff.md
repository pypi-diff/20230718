# Comparing `tmp/jsonablr-2.0.0.tar.gz` & `tmp/jsonablr-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonablr-2.0.0.tar", max compression
+gzip compressed data, was "jsonablr-2.0.1.tar", max compression
```

## Comparing `jsonablr-2.0.0.tar` & `jsonablr-2.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-06-26 17:24:04.431422 jsonablr-2.0.0/LICENSE
--rw-r--r--   0        0        0     1976 2023-07-04 20:21:45.058502 jsonablr-2.0.0/README.md
--rw-r--r--   0        0        0      118 2023-06-27 16:27:20.064626 jsonablr-2.0.0/jsonablr/__init__.py
--rw-r--r--   0        0        0     6364 2023-07-04 20:14:08.067419 jsonablr-2.0.0/jsonablr/main.py
--rw-r--r--   0        0        0      560 2023-07-04 20:24:06.354425 jsonablr-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 jsonablr-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-26 17:24:04.431422 jsonablr-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1976 2023-07-18 10:21:46.099534 jsonablr-2.0.1/README.md
+-rw-r--r--   0        0        0      118 2023-06-27 16:27:20.064626 jsonablr-2.0.1/jsonablr/__init__.py
+-rw-r--r--   0        0        0     6364 2023-07-18 10:21:46.099873 jsonablr-2.0.1/jsonablr/main.py
+-rw-r--r--   0        0        0      560 2023-07-18 10:22:09.460033 jsonablr-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 jsonablr-2.0.1/PKG-INFO
```

### Comparing `jsonablr-2.0.0/LICENSE` & `jsonablr-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonablr-2.0.0/README.md` & `jsonablr-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jsonablr-2.0.0/jsonablr/main.py` & `jsonablr-2.0.1/jsonablr/main.py`

 * *Files identical despite different names*

### Comparing `jsonablr-2.0.0/pyproject.toml` & `jsonablr-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Bernard van Niekerk <bernard.van.niekerk@icloud.com>"]
 description = "Serialize Pydantic models and non-JSONable types into a JSONable variable."
 name = "jsonablr"
 readme = "README.md"
 repository = "https://github.com/frizzy/jsonablr.git"
-version = "2.0.0"
+version = "2.0.1"
 
 [tool.poetry.dependencies]
 pydantic = "^2.0"
 python = "^3.8"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `jsonablr-2.0.0/PKG-INFO` & `jsonablr-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonablr
-Version: 2.0.0
+Version: 2.0.1
 Summary: Serialize Pydantic models and non-JSONable types into a JSONable variable.
 Home-page: https://github.com/frizzy/jsonablr.git
 Author: Bernard van Niekerk
 Author-email: bernard.van.niekerk@icloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

