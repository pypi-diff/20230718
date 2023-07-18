# Comparing `tmp/playcli-0.1.1.tar.gz` & `tmp/playcli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playcli-0.1.1.tar", max compression
+gzip compressed data, was "playcli-0.2.0.tar", max compression
```

## Comparing `playcli-0.1.1.tar` & `playcli-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0      332 2023-07-18 01:33:53.159538 playcli-0.1.1/README.md
--rw-r--r--   0        0        0      118 2023-07-18 01:34:53.887753 playcli-0.1.1/playcli/__init__.py
--rw-r--r--   0        0        0       38 2023-07-18 00:53:27.591450 playcli-0.1.1/playcli/__main__.py
--rw-r--r--   0        0        0      432 2023-07-18 00:53:27.591450 playcli-0.1.1/playcli/cli.py
--rw-r--r--   0        0        0        0 2023-07-18 00:53:27.591450 playcli-0.1.1/playcli/core/__init__.py
--rw-r--r--   0        0        0      114 2023-07-18 00:53:27.591450 playcli-0.1.1/playcli/core/commands/__init__.py
--rw-r--r--   0        0        0      186 2023-07-18 00:53:27.591450 playcli-0.1.1/playcli/core/commands/credits.py
--rw-r--r--   0        0        0      768 2023-07-18 00:53:27.591450 playcli-0.1.1/playcli/core/commands/search.py
--rw-r--r--   0        0        0      534 2023-07-18 00:53:27.591450 playcli-0.1.1/playcli/core/web.py
--rw-r--r--   0        0        0      107 2023-07-18 00:53:27.591450 playcli-0.1.1/playcli/main.py
--rw-r--r--   0        0        0      143 2023-07-18 00:53:27.592450 playcli-0.1.1/playcli/values.py
--rw-r--r--   0        0        0     1092 2023-07-18 01:37:56.853386 playcli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 playcli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      332 2023-07-18 01:33:53.159538 playcli-0.2.0/README.md
+-rw-r--r--   0        0        0      118 2023-07-18 04:16:35.684649 playcli-0.2.0/playcli/__init__.py
+-rw-r--r--   0        0        0       38 2023-07-18 00:53:27.591450 playcli-0.2.0/playcli/__main__.py
+-rw-r--r--   0        0        0      562 2023-07-18 04:24:42.758691 playcli-0.2.0/playcli/cli.py
+-rw-r--r--   0        0        0        0 2023-07-18 00:53:27.591450 playcli-0.2.0/playcli/core/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-18 00:53:27.591450 playcli-0.2.0/playcli/core/commands/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-18 00:53:27.591450 playcli-0.2.0/playcli/core/commands/credits.py
+-rw-r--r--   0        0        0     1290 2023-07-18 04:35:40.671563 playcli-0.2.0/playcli/core/commands/search.py
+-rw-r--r--   0        0        0      116 2023-07-18 03:54:06.313154 playcli-0.2.0/playcli/core/platforms/__init__.py
+-rw-r--r--   0        0        0      901 2023-07-18 03:54:40.098741 playcli-0.2.0/playcli/core/platforms/elamigos.py
+-rw-r--r--   0        0        0      884 2023-07-18 04:16:33.227679 playcli-0.2.0/playcli/core/platforms/steamunlocked.py
+-rw-r--r--   0        0        0      502 2023-07-18 03:29:19.739292 playcli-0.2.0/playcli/core/web.py
+-rw-r--r--   0        0        0      107 2023-07-18 00:53:27.591450 playcli-0.2.0/playcli/main.py
+-rw-r--r--   0        0        0      100 2023-07-18 03:33:34.984211 playcli-0.2.0/playcli/models/__init__.py
+-rw-r--r--   0        0        0      360 2023-07-18 03:54:06.326154 playcli-0.2.0/playcli/models/driver.py
+-rw-r--r--   0        0        0      646 2023-07-18 04:23:21.243688 playcli-0.2.0/playcli/models/platforms.py
+-rw-r--r--   0        0        0     1092 2023-07-18 04:35:22.073793 playcli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 playcli-0.2.0/PKG-INFO
```

### Comparing `playcli-0.1.1/pyproject.toml` & `playcli-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "playcli"
-version = "0.1.1"
+version = "0.2.0"
 description = "Browse and search games with ease"
 authors = ["Alekyo4 <alexsandergomes4742@gmail.com>"]
 license = "BeerWare"
 readme = "README.md"
 
 classifiers = [
     "Natural Language :: Portuguese (Brazilian)",
```

### Comparing `playcli-0.1.1/PKG-INFO` & `playcli-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playcli
-Version: 0.1.1
+Version: 0.2.0
 Summary: Browse and search games with ease
 License: Beerware
 Author: Alekyo4
 Author-email: alexsandergomes4742@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Customer Service
```

