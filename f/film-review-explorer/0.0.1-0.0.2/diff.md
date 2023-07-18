# Comparing `tmp/film_review_explorer-0.0.1.tar.gz` & `tmp/film_review_explorer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "film_review_explorer-0.0.1.tar", last modified: Mon Jul 17 12:33:34 2023, max compression
+gzip compressed data, was "film_review_explorer-0.0.2.tar", last modified: Tue Jul 18 14:26:01 2023, max compression
```

## Comparing `film_review_explorer-0.0.1.tar` & `film_review_explorer-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 pipchang   (501) staff       (20)        0 2023-07-17 12:33:34.756064 film_review_explorer-0.0.1/
--rw-r--r--   0 pipchang   (501) staff       (20)     1062 2023-07-06 12:21:46.000000 film_review_explorer-0.0.1/LICENSE
--rw-r--r--   0 pipchang   (501) staff       (20)      803 2023-07-17 12:33:34.755517 film_review_explorer-0.0.1/PKG-INFO
--rw-r--r--   0 pipchang   (501) staff       (20)      323 2023-07-06 14:54:48.000000 film_review_explorer-0.0.1/README.md
--rw-r--r--   0 pipchang   (501) staff       (20)      561 2023-07-17 12:28:34.000000 film_review_explorer-0.0.1/pyproject.toml
--rw-r--r--   0 pipchang   (501) staff       (20)       38 2023-07-17 12:33:34.756200 film_review_explorer-0.0.1/setup.cfg
-drwxr-xr-x   0 pipchang   (501) staff       (20)        0 2023-07-17 12:33:34.744203 film_review_explorer-0.0.1/src/
-drwxr-xr-x   0 pipchang   (501) staff       (20)        0 2023-07-17 12:33:34.747909 film_review_explorer-0.0.1/src/film_review_explorer/
--rw-r--r--   0 pipchang   (501) staff       (20)        0 2023-07-07 19:08:31.000000 film_review_explorer-0.0.1/src/film_review_explorer/__init__.py
--rw-r--r--   0 pipchang   (501) staff       (20)     2817 2023-07-13 09:37:08.000000 film_review_explorer-0.0.1/src/film_review_explorer/dataframe_preprocessor.py
--rw-r--r--   0 pipchang   (501) staff       (20)      156 2023-07-12 10:52:43.000000 film_review_explorer-0.0.1/src/film_review_explorer/topic_modeler.py
-drwxr-xr-x   0 pipchang   (501) staff       (20)        0 2023-07-17 12:33:34.753513 film_review_explorer-0.0.1/src/film_review_explorer.egg-info/
--rw-r--r--   0 pipchang   (501) staff       (20)      803 2023-07-17 12:33:34.000000 film_review_explorer-0.0.1/src/film_review_explorer.egg-info/PKG-INFO
--rw-r--r--   0 pipchang   (501) staff       (20)      354 2023-07-17 12:33:34.000000 film_review_explorer-0.0.1/src/film_review_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 pipchang   (501) staff       (20)        1 2023-07-17 12:33:34.000000 film_review_explorer-0.0.1/src/film_review_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 pipchang   (501) staff       (20)       21 2023-07-17 12:33:34.000000 film_review_explorer-0.0.1/src/film_review_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 pipchang   (501) staff       (20)        0 2023-07-18 14:26:01.004608 film_review_explorer-0.0.2/
+-rw-r--r--   0 pipchang   (501) staff       (20)     1062 2023-07-06 12:21:46.000000 film_review_explorer-0.0.2/LICENSE
+-rw-r--r--   0 pipchang   (501) staff       (20)     2374 2023-07-18 14:26:00.994059 film_review_explorer-0.0.2/PKG-INFO
+-rw-r--r--   0 pipchang   (501) staff       (20)      637 2023-07-17 13:32:44.000000 film_review_explorer-0.0.2/README.md
+-rw-r--r--   0 pipchang   (501) staff       (20)      652 2023-07-18 14:25:41.000000 film_review_explorer-0.0.2/pyproject.toml
+-rw-r--r--   0 pipchang   (501) staff       (20)       38 2023-07-18 14:26:01.005063 film_review_explorer-0.0.2/setup.cfg
+drwxr-xr-x   0 pipchang   (501) staff       (20)        0 2023-07-18 14:26:00.933250 film_review_explorer-0.0.2/src/
+drwxr-xr-x   0 pipchang   (501) staff       (20)        0 2023-07-18 14:26:00.948813 film_review_explorer-0.0.2/src/film_review_explorer/
+-rw-r--r--   0 pipchang   (501) staff       (20)       75 2023-07-18 11:09:07.000000 film_review_explorer-0.0.2/src/film_review_explorer/__init__.py
+-rw-r--r--   0 pipchang   (501) staff       (20)     7718 2023-07-18 14:16:56.000000 film_review_explorer-0.0.2/src/film_review_explorer/dataframe_preprocessor.py
+-rw-r--r--   0 pipchang   (501) staff       (20)     3070 2023-07-18 11:37:23.000000 film_review_explorer-0.0.2/src/film_review_explorer/topic_modeler.py
+drwxr-xr-x   0 pipchang   (501) staff       (20)        0 2023-07-18 14:26:00.992686 film_review_explorer-0.0.2/src/film_review_explorer.egg-info/
+-rw-r--r--   0 pipchang   (501) staff       (20)     2374 2023-07-18 14:26:00.000000 film_review_explorer-0.0.2/src/film_review_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 pipchang   (501) staff       (20)      401 2023-07-18 14:26:00.000000 film_review_explorer-0.0.2/src/film_review_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 pipchang   (501) staff       (20)        1 2023-07-18 14:26:00.000000 film_review_explorer-0.0.2/src/film_review_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 pipchang   (501) staff       (20)       15 2023-07-18 14:26:00.000000 film_review_explorer-0.0.2/src/film_review_explorer.egg-info/requires.txt
+-rw-r--r--   0 pipchang   (501) staff       (20)       21 2023-07-18 14:26:00.000000 film_review_explorer-0.0.2/src/film_review_explorer.egg-info/top_level.txt
```

### Comparing `film_review_explorer-0.0.1/LICENSE` & `film_review_explorer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `film_review_explorer-0.0.1/pyproject.toml` & `film_review_explorer-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "film_review_explorer"
-version = "0.0.1"
-authors = [
-  { name="Chang Jianghan", email="jianghanchang@hotmail.com" },
-]
+version = "0.0.2"
 description = "A python package for exploring film reviews."
 readme = "README.md"
 requires-python = ">=3.7"
+license = {file = "LICENSE"}
+keywords = ["film"]
+authors = [
+  {name="Chang Jianghan", email="jianghanchang@hotmail.com"},
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "pandas",
+  "seaborn",
+]
 
 [project.urls]
-"Homepage" = "https://github.com/pip-chang/film_review_explorer"
+Repository = "https://github.com/pip-chang/film_review_explorer"
```

