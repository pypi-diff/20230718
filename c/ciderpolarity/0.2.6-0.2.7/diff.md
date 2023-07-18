# Comparing `tmp/ciderpolarity-0.2.6.tar.gz` & `tmp/ciderpolarity-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciderpolarity-0.2.6.tar", max compression
+gzip compressed data, was "ciderpolarity-0.2.7.tar", max compression
```

## Comparing `ciderpolarity-0.2.6.tar` & `ciderpolarity-0.2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.6/LICENSE
--rw-r--r--   0        0        0     5139 2023-07-13 10:21:11.115976 ciderpolarity-0.2.6/README.md
--rw-r--r--   0        0        0     9387 2023-07-13 12:33:45.157234 ciderpolarity-0.2.6/ciderpolarity/CIDER.py
--rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.6/ciderpolarity/__init__.py
--rw-r--r--   0        0        0     3260 2023-07-13 12:14:50.023897 ciderpolarity-0.2.6/ciderpolarity/create_embeddings.py
--rw-r--r--   0        0        0     2851 2023-07-12 13:59:04.693106 ciderpolarity-0.2.6/ciderpolarity/create_vader.py
--rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.6/ciderpolarity/load_polarities.py
--rw-r--r--   0        0        0     5331 2023-07-13 12:14:41.635977 ciderpolarity-0.2.6/ciderpolarity/run_bootstrapping.py
--rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.6/ciderpolarity/stopwords.py
--rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.6/ciderpolarity/suggest_seeds.py
--rw-r--r--   0        0        0     1181 2023-07-13 12:14:28.216105 ciderpolarity-0.2.6/ciderpolarity/utils_funcs.py
--rw-r--r--   0        0        0      518 2023-07-13 12:34:51.544613 ciderpolarity-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     6027 1970-01-01 00:00:00.000000 ciderpolarity-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-10 13:31:58.387500 ciderpolarity-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5197 2023-07-18 07:56:43.733452 ciderpolarity-0.2.7/README.md
+-rw-r--r--   0        0        0     9387 2023-07-13 12:33:45.157234 ciderpolarity-0.2.7/ciderpolarity/CIDER.py
+-rw-r--r--   0        0        0       25 2023-07-10 15:40:11.905503 ciderpolarity-0.2.7/ciderpolarity/__init__.py
+-rw-r--r--   0        0        0     3260 2023-07-13 12:14:50.023897 ciderpolarity-0.2.7/ciderpolarity/create_embeddings.py
+-rw-r--r--   0        0        0     2851 2023-07-12 13:59:04.693106 ciderpolarity-0.2.7/ciderpolarity/create_vader.py
+-rw-r--r--   0        0        0     2139 2023-07-07 15:18:44.907460 ciderpolarity-0.2.7/ciderpolarity/load_polarities.py
+-rw-r--r--   0        0        0     5331 2023-07-13 12:14:41.635977 ciderpolarity-0.2.7/ciderpolarity/run_bootstrapping.py
+-rw-r--r--   0        0        0     1862 2023-07-05 17:22:40.222786 ciderpolarity-0.2.7/ciderpolarity/stopwords.py
+-rw-r--r--   0        0        0     4905 2023-07-10 12:42:03.154967 ciderpolarity-0.2.7/ciderpolarity/suggest_seeds.py
+-rw-r--r--   0        0        0     1181 2023-07-13 12:14:28.216105 ciderpolarity-0.2.7/ciderpolarity/utils_funcs.py
+-rw-r--r--   0        0        0      518 2023-07-18 07:57:30.232993 ciderpolarity-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6085 1970-01-01 00:00:00.000000 ciderpolarity-0.2.7/PKG-INFO
```

### Comparing `ciderpolarity-0.2.6/LICENSE` & `ciderpolarity-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.6/README.md` & `ciderpolarity-0.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # CIDER Python Package
 
+**Preprint Available:** https://arxiv.org/abs/2307.07864
+
 CIDER (Context Informed Dictionary and sEntiment Reasoner) is a Python library used to improve domain-specific sentiment analysis.
 
 It generates, filters, and substitutes polarities into [VADER](https://github.com/cjhutto/vaderSentiment/). 
 The approach taken to generate polarities is taken from [SocialSent](https://github.com/williamleif/socialsent).
 
 ## Contents
```

### Comparing `ciderpolarity-0.2.6/ciderpolarity/CIDER.py` & `ciderpolarity-0.2.7/ciderpolarity/CIDER.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.6/ciderpolarity/create_embeddings.py` & `ciderpolarity-0.2.7/ciderpolarity/create_embeddings.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.6/ciderpolarity/create_vader.py` & `ciderpolarity-0.2.7/ciderpolarity/create_vader.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.6/ciderpolarity/load_polarities.py` & `ciderpolarity-0.2.7/ciderpolarity/load_polarities.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.6/ciderpolarity/run_bootstrapping.py` & `ciderpolarity-0.2.7/ciderpolarity/run_bootstrapping.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.6/ciderpolarity/stopwords.py` & `ciderpolarity-0.2.7/ciderpolarity/stopwords.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.6/ciderpolarity/suggest_seeds.py` & `ciderpolarity-0.2.7/ciderpolarity/suggest_seeds.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.6/ciderpolarity/utils_funcs.py` & `ciderpolarity-0.2.7/ciderpolarity/utils_funcs.py`

 * *Files identical despite different names*

### Comparing `ciderpolarity-0.2.6/pyproject.toml` & `ciderpolarity-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ciderpolarity"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["jcy204 <jcy204@exeter.ac.uk>"]
 readme = "README.md"
 homepage = "https://github.com/jcy204/ciderPolarity"
 repository = "https://github.com/jcy204/ciderPolarity"
 
 [tool.poetry.dependencies]
```

### Comparing `ciderpolarity-0.2.6/PKG-INFO` & `ciderpolarity-0.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciderpolarity
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Home-page: https://github.com/jcy204/ciderPolarity
 Author: jcy204
 Author-email: jcy204@exeter.ac.uk
 Requires-Python: >=3.7,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -20,14 +20,16 @@
 Requires-Dist: tqdm (>=4.55.0,<5.0.0)
 Requires-Dist: vadersentiment (>=3.3.2,<4.0.0)
 Project-URL: Repository, https://github.com/jcy204/ciderPolarity
 Description-Content-Type: text/markdown
 
 # CIDER Python Package
 
+**Preprint Available:** https://arxiv.org/abs/2307.07864
+
 CIDER (Context Informed Dictionary and sEntiment Reasoner) is a Python library used to improve domain-specific sentiment analysis.
 
 It generates, filters, and substitutes polarities into [VADER](https://github.com/cjhutto/vaderSentiment/). 
 The approach taken to generate polarities is taken from [SocialSent](https://github.com/williamleif/socialsent).
 
 ## Contents
```

