# Comparing `tmp/lexisnexisapi-2.0.46.tar.gz` & `tmp/lexisnexisapi-2.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexisnexisapi-2.0.46.tar", last modified: Thu Jun 29 15:42:40 2023, max compression
+gzip compressed data, was "lexisnexisapi-2.0.47.tar", last modified: Tue Jul 18 14:22:09 2023, max compression
```

## Comparing `lexisnexisapi-2.0.46.tar` & `lexisnexisapi-2.0.47.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 15:42:40.202756 lexisnexisapi-2.0.46/
--rw-rw-rw-   0        0        0      466 2022-12-20 12:40:20.000000 lexisnexisapi-2.0.46/LICENSE.txt
--rw-rw-rw-   0        0        0     1904 2023-06-29 15:42:40.111755 lexisnexisapi-2.0.46/PKG-INFO
--rw-rw-rw-   0        0        0     1382 2023-02-08 14:35:01.000000 lexisnexisapi-2.0.46/README.md
--rw-rw-rw-   0        0        0      588 2023-06-29 15:35:54.000000 lexisnexisapi-2.0.46/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 15:42:40.206756 lexisnexisapi-2.0.46/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-06-29 15:35:15.000000 lexisnexisapi-2.0.46/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:42:39.180367 lexisnexisapi-2.0.46/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 15:42:39.916697 lexisnexisapi-2.0.46/src/lexisnexisapi/
--rw-rw-rw-   0        0        0        0 2023-01-28 19:22:50.000000 lexisnexisapi-2.0.46/src/lexisnexisapi/__init__.py
--rw-rw-rw-   0        0        0     1863 2023-02-02 17:25:44.000000 lexisnexisapi-2.0.46/src/lexisnexisapi/credentials.py
--rw-rw-rw-   0        0        0     9920 2023-06-29 14:53:39.000000 lexisnexisapi-2.0.46/src/lexisnexisapi/metabase.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:42:40.103755 lexisnexisapi-2.0.46/src/lexisnexisapi.egg-info/
--rw-rw-rw-   0        0        0     1904 2023-06-29 15:42:37.000000 lexisnexisapi-2.0.46/src/lexisnexisapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-29 15:42:38.000000 lexisnexisapi-2.0.46/src/lexisnexisapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 15:42:38.000000 lexisnexisapi-2.0.46/src/lexisnexisapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-29 15:42:38.000000 lexisnexisapi-2.0.46/src/lexisnexisapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 14:22:09.751333 lexisnexisapi-2.0.47/
+-rw-rw-rw-   0        0        0      466 2022-12-20 12:40:20.000000 lexisnexisapi-2.0.47/LICENSE.txt
+-rw-rw-rw-   0        0        0     6161 2023-07-18 14:22:09.735334 lexisnexisapi-2.0.47/PKG-INFO
+-rw-rw-rw-   0        0        0     5637 2023-07-18 14:20:29.000000 lexisnexisapi-2.0.47/README.md
+-rw-rw-rw-   0        0        0      588 2023-07-18 14:20:55.000000 lexisnexisapi-2.0.47/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 14:22:09.752334 lexisnexisapi-2.0.47/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-07-18 14:14:50.000000 lexisnexisapi-2.0.47/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:22:09.590331 lexisnexisapi-2.0.47/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 14:22:09.696332 lexisnexisapi-2.0.47/src/lexisnexisapi/
+-rw-rw-rw-   0        0        0        0 2023-01-28 19:22:50.000000 lexisnexisapi-2.0.47/src/lexisnexisapi/__init__.py
+-rw-rw-rw-   0        0        0     1863 2023-02-02 17:25:44.000000 lexisnexisapi-2.0.47/src/lexisnexisapi/credentials.py
+-rw-rw-rw-   0        0        0     9920 2023-06-29 14:53:39.000000 lexisnexisapi-2.0.47/src/lexisnexisapi/metabase.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:22:09.726332 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/
+-rw-rw-rw-   0        0        0     6161 2023-07-18 14:22:09.000000 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-18 14:22:09.000000 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 14:22:09.000000 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 14:22:09.000000 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/top_level.txt
```

### Comparing `lexisnexisapi-2.0.46/pyproject.toml` & `lexisnexisapi-2.0.47/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexisnexisapi"
-version = "2.0.46"
+version = "2.0.47"
 authors = [{ name = "Robert Cuffney", email = "robert.cuffney@lexisnexis.com" },
 		   { name = "Ozgur Aycan", email = "ozgur.aycan@lexisnexis.co.uk" }
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lexisnexisapi-2.0.46/src/lexisnexisapi/credentials.py` & `lexisnexisapi-2.0.47/src/lexisnexisapi/credentials.py`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-2.0.46/src/lexisnexisapi/metabase.py` & `lexisnexisapi-2.0.47/src/lexisnexisapi/metabase.py`

 * *Files identical despite different names*

