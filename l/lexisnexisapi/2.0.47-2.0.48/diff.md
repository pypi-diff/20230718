# Comparing `tmp/lexisnexisapi-2.0.47.tar.gz` & `tmp/lexisnexisapi-2.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexisnexisapi-2.0.47.tar", last modified: Tue Jul 18 14:22:09 2023, max compression
+gzip compressed data, was "lexisnexisapi-2.0.48.tar", last modified: Tue Jul 18 14:44:02 2023, max compression
```

## Comparing `lexisnexisapi-2.0.47.tar` & `lexisnexisapi-2.0.48.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 14:22:09.751333 lexisnexisapi-2.0.47/
--rw-rw-rw-   0        0        0      466 2022-12-20 12:40:20.000000 lexisnexisapi-2.0.47/LICENSE.txt
--rw-rw-rw-   0        0        0     6161 2023-07-18 14:22:09.735334 lexisnexisapi-2.0.47/PKG-INFO
--rw-rw-rw-   0        0        0     5637 2023-07-18 14:20:29.000000 lexisnexisapi-2.0.47/README.md
--rw-rw-rw-   0        0        0      588 2023-07-18 14:20:55.000000 lexisnexisapi-2.0.47/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 14:22:09.752334 lexisnexisapi-2.0.47/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-07-18 14:14:50.000000 lexisnexisapi-2.0.47/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:22:09.590331 lexisnexisapi-2.0.47/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 14:22:09.696332 lexisnexisapi-2.0.47/src/lexisnexisapi/
--rw-rw-rw-   0        0        0        0 2023-01-28 19:22:50.000000 lexisnexisapi-2.0.47/src/lexisnexisapi/__init__.py
--rw-rw-rw-   0        0        0     1863 2023-02-02 17:25:44.000000 lexisnexisapi-2.0.47/src/lexisnexisapi/credentials.py
--rw-rw-rw-   0        0        0     9920 2023-06-29 14:53:39.000000 lexisnexisapi-2.0.47/src/lexisnexisapi/metabase.py
-drwxrwxrwx   0        0        0        0 2023-07-18 14:22:09.726332 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/
--rw-rw-rw-   0        0        0     6161 2023-07-18 14:22:09.000000 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-18 14:22:09.000000 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 14:22:09.000000 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-18 14:22:09.000000 lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 14:44:02.663176 lexisnexisapi-2.0.48/
+-rw-rw-rw-   0        0        0      466 2022-12-20 12:40:20.000000 lexisnexisapi-2.0.48/LICENSE.txt
+-rw-rw-rw-   0        0        0     6195 2023-07-18 14:44:02.660178 lexisnexisapi-2.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0     5640 2023-07-18 14:34:02.000000 lexisnexisapi-2.0.48/README.md
+-rw-rw-rw-   0        0        0      619 2023-07-18 14:34:20.000000 lexisnexisapi-2.0.48/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 14:44:02.665180 lexisnexisapi-2.0.48/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-07-18 14:37:16.000000 lexisnexisapi-2.0.48/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:44:02.563174 lexisnexisapi-2.0.48/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 14:44:02.620174 lexisnexisapi-2.0.48/src/lexisnexisapi/
+-rw-rw-rw-   0        0        0        0 2023-01-28 19:22:50.000000 lexisnexisapi-2.0.48/src/lexisnexisapi/__init__.py
+-rw-rw-rw-   0        0        0     1863 2023-02-02 17:25:44.000000 lexisnexisapi-2.0.48/src/lexisnexisapi/credentials.py
+-rw-rw-rw-   0        0        0     9920 2023-06-29 14:53:39.000000 lexisnexisapi-2.0.48/src/lexisnexisapi/metabase.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:44:02.653177 lexisnexisapi-2.0.48/src/lexisnexisapi.egg-info/
+-rw-rw-rw-   0        0        0     6195 2023-07-18 14:44:02.000000 lexisnexisapi-2.0.48/src/lexisnexisapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-18 14:44:02.000000 lexisnexisapi-2.0.48/src/lexisnexisapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 14:44:02.000000 lexisnexisapi-2.0.48/src/lexisnexisapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 14:44:02.000000 lexisnexisapi-2.0.48/src/lexisnexisapi.egg-info/top_level.txt
```

### Comparing `lexisnexisapi-2.0.47/PKG-INFO` & `lexisnexisapi-2.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lexisnexisapi
-Version: 2.0.47
-Summary: A small example package
+Version: 2.0.48
+Summary: A module to support the lexisnexis metabase search api
 Home-page: 
 Author: Robert Cuffney
 Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
 License: MIT
 Keywords: example project
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 - Robert Cuffney
 - Ozgur Aycan
 - CS Integration Consultants @ LexisNexis
 
 ### Version
 
-Current version: 0.1
+Current version: 2.0.48
 
 ## 2. Installation
 
 ### Dependencies
 
 To use the `metabase.py` module, you need the following dependencies:
```

### Comparing `lexisnexisapi-2.0.47/README.md` & `lexisnexisapi-2.0.48/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 - Robert Cuffney
 - Ozgur Aycan
 - CS Integration Consultants @ LexisNexis
 
 ### Version
 
-Current version: 0.1
+Current version: 2.0.48
 
 ## 2. Installation
 
 ### Dependencies
 
 To use the `metabase.py` module, you need the following dependencies:
```

### Comparing `lexisnexisapi-2.0.47/pyproject.toml` & `lexisnexisapi-2.0.48/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lexisnexisapi"
-version = "2.0.47"
+version = "2.0.48"
 authors = [{ name = "Robert Cuffney", email = "robert.cuffney@lexisnexis.com" },
 		   { name = "Ozgur Aycan", email = "ozgur.aycan@lexisnexis.co.uk" }
 ]
-description = "A small example package"
+description = "A module to support the lexisnexis metabase search api"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `lexisnexisapi-2.0.47/setup.py` & `lexisnexisapi-2.0.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lexisnexisapi",
-    version='2.0.47',
+    version='2.0.48',
     license='MIT',
     author="Robert Cuffney",
     author_email='robert.cuffney@lexisnexis.com',
     description = 'a module to support the lexisnexis metabase search api',
     long_description = ' module provides a Python interface to interact with the Metabase API. It allows you to perform searches and retrieve articles using the Metabase API. The module facilitates the creation of Python objects representing the API response, making it easy to work with the data.',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `lexisnexisapi-2.0.47/src/lexisnexisapi/credentials.py` & `lexisnexisapi-2.0.48/src/lexisnexisapi/credentials.py`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-2.0.47/src/lexisnexisapi/metabase.py` & `lexisnexisapi-2.0.48/src/lexisnexisapi/metabase.py`

 * *Files identical despite different names*

### Comparing `lexisnexisapi-2.0.47/src/lexisnexisapi.egg-info/PKG-INFO` & `lexisnexisapi-2.0.48/src/lexisnexisapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lexisnexisapi
-Version: 2.0.47
-Summary: A small example package
+Version: 2.0.48
+Summary: A module to support the lexisnexis metabase search api
 Home-page: 
 Author: Robert Cuffney
 Author-email: Robert Cuffney <robert.cuffney@lexisnexis.com>, Ozgur Aycan <ozgur.aycan@lexisnexis.co.uk>
 License: MIT
 Keywords: example project
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 - Robert Cuffney
 - Ozgur Aycan
 - CS Integration Consultants @ LexisNexis
 
 ### Version
 
-Current version: 0.1
+Current version: 2.0.48
 
 ## 2. Installation
 
 ### Dependencies
 
 To use the `metabase.py` module, you need the following dependencies:
```

