# Comparing `tmp/hhaven-0.1.0.tar.gz` & `tmp/hhaven-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhaven-0.1.0.tar", last modified: Tue Jul 18 12:43:42 2023, max compression
+gzip compressed data, was "hhaven-0.1.1.tar", last modified: Tue Jul 18 13:00:23 2023, max compression
```

## Comparing `hhaven-0.1.0.tar` & `hhaven-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 12:43:42.750860 hhaven-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-07-17 11:16:45.000000 hhaven-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3824 2023-07-18 12:43:42.750860 hhaven-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2727 2023-07-18 11:55:34.000000 hhaven-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 12:43:42.741861 hhaven-0.1.0/hhaven/
--rw-rw-rw-   0        0        0      267 2023-07-18 12:38:15.000000 hhaven-0.1.0/hhaven/__init__.py
--rw-rw-rw-   0        0        0    10241 2023-07-17 16:00:30.000000 hhaven-0.1.0/hhaven/client.py
--rw-rw-rw-   0        0        0     1180 2023-07-17 15:43:02.000000 hhaven-0.1.0/hhaven/decorators.py
--rw-rw-rw-   0        0        0     2273 2023-07-17 15:12:47.000000 hhaven-0.1.0/hhaven/exceptions.py
--rw-rw-rw-   0        0        0    15853 2023-07-17 15:50:40.000000 hhaven-0.1.0/hhaven/models.py
--rw-rw-rw-   0        0        0      789 2023-07-17 16:05:23.000000 hhaven-0.1.0/hhaven/utility.py
-drwxrwxrwx   0        0        0        0 2023-07-18 12:43:42.748859 hhaven-0.1.0/hhaven.egg-info/
--rw-rw-rw-   0        0        0     3824 2023-07-18 12:43:42.000000 hhaven-0.1.0/hhaven.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-18 12:43:42.000000 hhaven-0.1.0/hhaven.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 12:43:42.000000 hhaven-0.1.0/hhaven.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-18 12:43:42.000000 hhaven-0.1.0/hhaven.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-18 12:43:42.000000 hhaven-0.1.0/hhaven.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1050 2023-07-18 12:39:53.000000 hhaven-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 12:43:42.751859 hhaven-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1505 2023-07-18 12:37:51.000000 hhaven-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:23.712713 hhaven-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-07-17 11:16:45.000000 hhaven-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3487 2023-07-18 13:00:23.712713 hhaven-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2727 2023-07-18 11:55:34.000000 hhaven-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:23.703712 hhaven-0.1.1/hhaven/
+-rw-rw-rw-   0        0        0      267 2023-07-18 12:59:04.000000 hhaven-0.1.1/hhaven/__init__.py
+-rw-rw-rw-   0        0        0    10241 2023-07-17 16:00:30.000000 hhaven-0.1.1/hhaven/client.py
+-rw-rw-rw-   0        0        0     1180 2023-07-17 15:43:02.000000 hhaven-0.1.1/hhaven/decorators.py
+-rw-rw-rw-   0        0        0     2273 2023-07-17 15:12:47.000000 hhaven-0.1.1/hhaven/exceptions.py
+-rw-rw-rw-   0        0        0    15853 2023-07-17 15:50:40.000000 hhaven-0.1.1/hhaven/models.py
+-rw-rw-rw-   0        0        0      789 2023-07-17 16:05:23.000000 hhaven-0.1.1/hhaven/utility.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:00:23.710713 hhaven-0.1.1/hhaven.egg-info/
+-rw-rw-rw-   0        0        0     3487 2023-07-18 13:00:23.000000 hhaven-0.1.1/hhaven.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-18 13:00:23.000000 hhaven-0.1.1/hhaven.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:00:23.000000 hhaven-0.1.1/hhaven.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-18 13:00:23.000000 hhaven-0.1.1/hhaven.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 13:00:23.000000 hhaven-0.1.1/hhaven.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1055 2023-07-18 12:59:04.000000 hhaven-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:00:23.712713 hhaven-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1510 2023-07-18 12:59:04.000000 hhaven-0.1.1/setup.py
```

### Comparing `hhaven-0.1.0/LICENSE` & `hhaven-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.0/PKG-INFO` & `hhaven-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhaven
-Version: 0.1.0
+Version: 0.1.1
 Summary: A well-documented and typed API wrapper for Hentai Haven.
 Home-page: https://github.com/jokelbaf/hhaven
 Author: jokelbaf
 Author-email: jokelbaf@gmail.com
 License: MIT
 Project-URL: Documentation, https://jokelbaf.github.io/hhaven
 Project-URL: API Reference, https://jokelbaf.github.io/hhaven-api-reference
@@ -22,19 +22,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<picture>
-  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/JokelBaf/hhaven/assets/60827680/977e3964-e2f5-443a-b1c5-57f7a3089f6e">
-  <source media="(prefers-color-scheme: light)" srcset="https://github.com/JokelBaf/hhaven/assets/60827680/521c38e7-96d7-4781-9660-b2a61ee9fb17">
-  <img alt="Logo" src="https://github.com/JokelBaf/hhaven/assets/60827680/521c38e7-96d7-4781-9660-b2a61ee9fb17">
-</picture>
+![Logo](https://github.com/JokelBaf/hhaven/blob/master/docs/assets/logo-light.png?raw=true)
 
 
 # HHaven
 ![GitHub release (with filter)](https://img.shields.io/github/v/release/jokelbaf/hhaven?style=for-the-badge&logo=github&label=Version&labelColor=%23c7423e) ![PyPI](https://img.shields.io/pypi/v/hhaven?style=for-the-badge&logo=pypi&logoColor=white) ![Code Climate coverage](https://img.shields.io/codeclimate/coverage/JokelBaf/hhaven?style=for-the-badge&logo=codeclimate&logoColor=white)
 
 A well-documented and typed API wrapper for [**Hentai Haven**](https://hentaihaven.xxx/), providing efficient asynchronous requests, built-in cache support, and Pydantic Models for seamless autocompletion and linter support.
```

### Comparing `hhaven-0.1.0/README.md` & `hhaven-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.0/hhaven/client.py` & `hhaven-0.1.1/hhaven/client.py`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.0/hhaven/decorators.py` & `hhaven-0.1.1/hhaven/decorators.py`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.0/hhaven/exceptions.py` & `hhaven-0.1.1/hhaven/exceptions.py`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.0/hhaven/models.py` & `hhaven-0.1.1/hhaven/models.py`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.0/hhaven/utility.py` & `hhaven-0.1.1/hhaven/utility.py`

 * *Files identical despite different names*

### Comparing `hhaven-0.1.0/hhaven.egg-info/PKG-INFO` & `hhaven-0.1.1/hhaven.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hhaven
-Version: 0.1.0
+Version: 0.1.1
 Summary: A well-documented and typed API wrapper for Hentai Haven.
 Home-page: https://github.com/jokelbaf/hhaven
 Author: jokelbaf
 Author-email: jokelbaf@gmail.com
 License: MIT
 Project-URL: Documentation, https://jokelbaf.github.io/hhaven
 Project-URL: API Reference, https://jokelbaf.github.io/hhaven-api-reference
@@ -22,19 +22,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<picture>
-  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/JokelBaf/hhaven/assets/60827680/977e3964-e2f5-443a-b1c5-57f7a3089f6e">
-  <source media="(prefers-color-scheme: light)" srcset="https://github.com/JokelBaf/hhaven/assets/60827680/521c38e7-96d7-4781-9660-b2a61ee9fb17">
-  <img alt="Logo" src="https://github.com/JokelBaf/hhaven/assets/60827680/521c38e7-96d7-4781-9660-b2a61ee9fb17">
-</picture>
+![Logo](https://github.com/JokelBaf/hhaven/blob/master/docs/assets/logo-light.png?raw=true)
 
 
 # HHaven
 ![GitHub release (with filter)](https://img.shields.io/github/v/release/jokelbaf/hhaven?style=for-the-badge&logo=github&label=Version&labelColor=%23c7423e) ![PyPI](https://img.shields.io/pypi/v/hhaven?style=for-the-badge&logo=pypi&logoColor=white) ![Code Climate coverage](https://img.shields.io/codeclimate/coverage/JokelBaf/hhaven?style=for-the-badge&logo=codeclimate&logoColor=white)
 
 A well-documented and typed API wrapper for [**Hentai Haven**](https://hentaihaven.xxx/), providing efficient asynchronous requests, built-in cache support, and Pydantic Models for seamless autocompletion and linter support.
```

### Comparing `hhaven-0.1.0/pyproject.toml` & `hhaven-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "hhaven"
 license = "MIT"
-version = "0.1.0"
+version = "0.1.1"
 description = "A well-documented and typed API wrapper for Hentai Haven."
 authors = [
     "JokelBaf <jokelbaf@gmail.com>",
 ]
 maintainers = [
     "JokelBaf <jokelbaf@gmail.com>",
 ]
-readme = "README.md"
+readme = "README-pypi.md"
 homepage = "https://github.com/jokelbaf/hhaven"
 repository = "https://github.com/jokelbaf/hhaven"
 documentation = "https://jokelbaf.github.io/hhaven"
 keywords = ["hentai-haven", "hentai"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hhaven-0.1.0/setup.py` & `hhaven-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Run setuptools."""
 from setuptools import find_packages, setup
 
 setup(
     name = "hhaven",
-    version = "0.1.0",
+    version = "0.1.1",
     author = "jokelbaf",
     author_email = "jokelbaf@gmail.com",
     description = "A well-documented and typed API wrapper for Hentai Haven.",
     keywords = "hentai-haven hentai".split(),
     url = "https://github.com/jokelbaf/hhaven",
     project_urls = {
         "Documentation": "https://jokelbaf.github.io/hhaven",
@@ -15,15 +15,15 @@
         "Issue tracker": "https://github.com/jokelbaf/hhaven/issues",
     },
     packages = find_packages(exclude=["tests.*"]),
     python_requires = ">=3.8",
     install_requires = ["aiohttp", "pydantic", "aiocache"],
     include_package_data = True,
     package_data = {"hhaven": ["py.typed"]},
-    long_description = open("README.md", encoding="utf-8").read(),
+    long_description = open("README-pypi.md", encoding="utf-8").read(),
     long_description_content_type = "text/markdown",
     license = "MIT",
     classifiers = [
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Natural Language :: English",
```

