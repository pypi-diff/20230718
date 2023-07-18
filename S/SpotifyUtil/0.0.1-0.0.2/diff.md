# Comparing `tmp/SpotifyUtil-0.0.1.tar.gz` & `tmp/SpotifyUtil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpotifyUtil-0.0.1.tar", last modified: Mon Jul 17 13:24:27 2023, max compression
+gzip compressed data, was "SpotifyUtil-0.0.2.tar", last modified: Tue Jul 18 19:17:18 2023, max compression
```

## Comparing `SpotifyUtil-0.0.1.tar` & `SpotifyUtil-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 13:24:27.001940 SpotifyUtil-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-07-13 08:37:27.000000 SpotifyUtil-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1954 2023-07-17 13:24:27.000937 SpotifyUtil-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1284 2023-07-17 13:09:57.000000 SpotifyUtil-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 13:24:26.978936 SpotifyUtil-0.0.1/SpotifyUtil/
--rw-rw-rw-   0        0        0     7552 2023-07-17 13:21:34.000000 SpotifyUtil-0.0.1/SpotifyUtil/SpotifyUtil.py
--rw-rw-rw-   0        0        0      139 2023-07-15 08:09:48.000000 SpotifyUtil-0.0.1/SpotifyUtil/__init__.py
--rw-rw-rw-   0        0        0     1387 2023-07-17 13:05:55.000000 SpotifyUtil-0.0.1/SpotifyUtil/config.py
--rw-rw-rw-   0        0        0      262 2023-07-16 14:31:36.000000 SpotifyUtil-0.0.1/SpotifyUtil/file_reader.py
--rw-rw-rw-   0        0        0      139 2023-07-14 03:49:04.000000 SpotifyUtil-0.0.1/SpotifyUtil/secret.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:24:26.998938 SpotifyUtil-0.0.1/SpotifyUtil.egg-info/
--rw-rw-rw-   0        0        0     1954 2023-07-17 13:24:26.000000 SpotifyUtil-0.0.1/SpotifyUtil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-07-17 13:24:26.000000 SpotifyUtil-0.0.1/SpotifyUtil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 13:24:26.000000 SpotifyUtil-0.0.1/SpotifyUtil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-17 13:24:26.000000 SpotifyUtil-0.0.1/SpotifyUtil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-17 13:24:26.000000 SpotifyUtil-0.0.1/SpotifyUtil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      678 2023-07-17 13:23:37.000000 SpotifyUtil-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 13:24:27.002937 SpotifyUtil-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-07-17 13:23:42.000000 SpotifyUtil-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 19:17:18.680165 SpotifyUtil-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-13 08:37:27.000000 SpotifyUtil-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2006 2023-07-18 19:17:18.677212 SpotifyUtil-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1284 2023-07-17 13:09:57.000000 SpotifyUtil-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 19:17:18.647158 SpotifyUtil-0.0.2/SpotifyUtil/
+-rw-rw-rw-   0        0        0    14027 2023-07-18 19:06:13.000000 SpotifyUtil-0.0.2/SpotifyUtil/SpotifyUtil.py
+-rw-rw-rw-   0        0        0      139 2023-07-18 16:53:30.000000 SpotifyUtil-0.0.2/SpotifyUtil/__init__.py
+-rw-rw-rw-   0        0        0     1387 2023-07-17 18:50:45.000000 SpotifyUtil-0.0.2/SpotifyUtil/config.py
+-rw-rw-rw-   0        0        0      262 2023-07-16 14:31:36.000000 SpotifyUtil-0.0.2/SpotifyUtil/file_reader.py
+-rw-rw-rw-   0        0        0      157 2023-07-17 14:31:47.000000 SpotifyUtil-0.0.2/SpotifyUtil/secret.py
+drwxrwxrwx   0        0        0        0 2023-07-18 19:17:18.673155 SpotifyUtil-0.0.2/SpotifyUtil.egg-info/
+-rw-rw-rw-   0        0        0     2006 2023-07-18 19:17:18.000000 SpotifyUtil-0.0.2/SpotifyUtil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-07-18 19:17:18.000000 SpotifyUtil-0.0.2/SpotifyUtil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 19:17:18.000000 SpotifyUtil-0.0.2/SpotifyUtil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 19:17:18.000000 SpotifyUtil-0.0.2/SpotifyUtil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 19:17:18.000000 SpotifyUtil-0.0.2/SpotifyUtil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      768 2023-07-18 19:16:56.000000 SpotifyUtil-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 19:17:18.682155 SpotifyUtil-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      962 2023-07-18 19:17:00.000000 SpotifyUtil-0.0.2/setup.py
```

### Comparing `SpotifyUtil-0.0.1/LICENSE` & `SpotifyUtil-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.1/PKG-INFO` & `SpotifyUtil-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: SpotifyUtil
-Version: 0.0.1
+Version: 0.0.2
 Summary: SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.
 Home-page: https://github.com/Arg0naut18/SpotifyUtil
 Author: Arg0naut18
 Author-email: Arg0naut18 <gaming.genos1729@gmail.com>
 Project-URL: Homepage, https://github.com/Arg0naut18/SpotifyUtil
+Keywords: Spotify,Spotipy,SpotifyUtil,SpotifyUtils
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >= 3.6
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SpotifyUtil
 SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.
 
 ## Features
```

### Comparing `SpotifyUtil-0.0.1/README.md` & `SpotifyUtil-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.1/SpotifyUtil/config.py` & `SpotifyUtil-0.0.2/SpotifyUtil/config.py`

 * *Files identical despite different names*

### Comparing `SpotifyUtil-0.0.1/SpotifyUtil.egg-info/PKG-INFO` & `SpotifyUtil-0.0.2/SpotifyUtil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: SpotifyUtil
-Version: 0.0.1
+Version: 0.0.2
 Summary: SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.
 Home-page: https://github.com/Arg0naut18/SpotifyUtil
 Author: Arg0naut18
 Author-email: Arg0naut18 <gaming.genos1729@gmail.com>
 Project-URL: Homepage, https://github.com/Arg0naut18/SpotifyUtil
+Keywords: Spotify,Spotipy,SpotifyUtil,SpotifyUtils
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >= 3.6
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SpotifyUtil
 SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.
 
 ## Features
```

### Comparing `SpotifyUtil-0.0.1/pyproject.toml` & `SpotifyUtil-0.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,30 @@
-[project]
-name = "SpotifyUtil"
-version = "0.0.1"
-authors = [
-    { name="Arg0naut18", email="gaming.genos1729@gmail.com" },
-]
-description = "SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks."
-readme = "README.md"
-requires-python = ">=3.6"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent",
-]
+import setuptools
 
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+with open("README.md", "r", encoding="utf-8", errors="ignore") as fh:
+    long_description = fh.read()
 
-[project.urls]
-"Homepage" = "https://github.com/Arg0naut18/SpotifyUtil"
+setuptools.setup(
+    name="SpotifyUtil",
+    version="0.0.2",
+    author="Arg0naut18",
+    description="SpotifyUtils is a very useful library made over Spotipy to automate some rather tiring tasks.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Arg0naut18/SpotifyUtil",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Development Status :: 3 - Alpha",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Operating System :: OS Independent",
+    ],
+    keywords = [
+    "Spotify",
+    "Spotipy",
+    "SpotifyUtil",
+    "SpotifyUtils",
+    ],
+    python_requires=">= 3.8",
+    include_package_data=True,
+    install_requires=["spotipy"]
+)
```

