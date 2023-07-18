# Comparing `tmp/bingo-bongo-cat-0.0.3.tar.gz` & `tmp/bingo_bongo_cat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingo-bongo-cat-0.0.3.tar", last modified: Tue Jul 18 17:09:49 2023, max compression
+gzip compressed data, was "bingo_bongo_cat-0.0.4.tar", last modified: Tue Jul 18 17:16:01 2023, max compression
```

## Comparing `bingo-bongo-cat-0.0.3.tar` & `bingo_bongo_cat-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:09:49.844233 bingo-bongo-cat-0.0.3/
--rw-rw-rw-   0        0        0        0 2023-07-18 16:57:14.000000 bingo-bongo-cat-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      646 2023-07-18 17:09:49.843233 bingo-bongo-cat-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-07-18 06:31:56.000000 bingo-bongo-cat-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 17:09:49.828235 bingo-bongo-cat-0.0.3/bingo-bongo-cat/
--rw-rw-rw-   0        0        0       29 2023-07-18 16:50:24.000000 bingo-bongo-cat-0.0.3/bingo-bongo-cat/__init__.py
--rw-rw-rw-   0        0        0     1698 2023-07-18 17:03:38.000000 bingo-bongo-cat-0.0.3/bingo-bongo-cat/bingo_bongo_cat.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:09:49.839233 bingo-bongo-cat-0.0.3/bingo_bongo_cat.egg-info/
--rw-rw-rw-   0        0        0      646 2023-07-18 17:09:49.000000 bingo-bongo-cat-0.0.3/bingo_bongo_cat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-07-18 17:09:49.000000 bingo-bongo-cat-0.0.3/bingo_bongo_cat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:09:49.000000 bingo-bongo-cat-0.0.3/bingo_bongo_cat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-18 17:09:49.000000 bingo-bongo-cat-0.0.3/bingo_bongo_cat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 17:09:49.844233 bingo-bongo-cat-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-07-18 17:07:58.000000 bingo-bongo-cat-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:16:01.401276 bingo_bongo_cat-0.0.4/
+-rw-rw-rw-   0        0        0        0 2023-07-18 16:57:14.000000 bingo_bongo_cat-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      646 2023-07-18 17:16:01.401276 bingo_bongo_cat-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-07-18 06:31:56.000000 bingo_bongo_cat-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 17:16:01.388414 bingo_bongo_cat-0.0.4/bingo_bongo_cat/
+-rw-rw-rw-   0        0        0       29 2023-07-18 16:50:24.000000 bingo_bongo_cat-0.0.4/bingo_bongo_cat/__init__.py
+-rw-rw-rw-   0        0        0     1698 2023-07-18 17:03:38.000000 bingo_bongo_cat-0.0.4/bingo_bongo_cat/bingo_bongo_cat.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:16:01.397415 bingo_bongo_cat-0.0.4/bingo_bongo_cat.egg-info/
+-rw-rw-rw-   0        0        0      646 2023-07-18 17:16:01.000000 bingo_bongo_cat-0.0.4/bingo_bongo_cat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-07-18 17:16:01.000000 bingo_bongo_cat-0.0.4/bingo_bongo_cat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:16:01.000000 bingo_bongo_cat-0.0.4/bingo_bongo_cat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-18 17:16:01.000000 bingo_bongo_cat-0.0.4/bingo_bongo_cat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:16:01.402284 bingo_bongo_cat-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      916 2023-07-18 17:15:34.000000 bingo_bongo_cat-0.0.4/setup.py
```

### Comparing `bingo-bongo-cat-0.0.3/PKG-INFO` & `bingo_bongo_cat-0.0.4/bingo_bongo_cat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingo-bongo-cat
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cat that prints messages.
 Author: Kyle Levy
 Author-email: 
 Keywords: python,debugging,cat,funny
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bingo-bongo-cat-0.0.3/README.md` & `bingo_bongo_cat-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bingo-bongo-cat-0.0.3/bingo-bongo-cat/bingo_bongo_cat.py` & `bingo_bongo_cat-0.0.4/bingo_bongo_cat/bingo_bongo_cat.py`

 * *Files identical despite different names*

### Comparing `bingo-bongo-cat-0.0.3/bingo_bongo_cat.egg-info/PKG-INFO` & `bingo_bongo_cat-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bingo-bongo-cat
-Version: 0.0.3
+Name: bingo_bongo_cat
+Version: 0.0.4
 Summary: Cat that prints messages.
 Author: Kyle Levy
 Author-email: 
 Keywords: python,debugging,cat,funny
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bingo-bongo-cat-0.0.3/setup.py` & `bingo_bongo_cat-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Cat that prints messages.'
 LONG_DESCRIPTION = 'A package which makes troubleshooting code a little less painful by adding a cute cat to let you know where you went wrong.'
 
 # Setting up
 setup(
-    name="bingo-bongo-cat",
+    name="bingo_bongo_cat",
     version=VERSION,
     author="Kyle Levy",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

