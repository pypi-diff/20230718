# Comparing `tmp/findlike-1.4.1.tar.gz` & `tmp/findlike-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findlike-1.4.1.tar", last modified: Tue Jul 11 17:46:01 2023, max compression
+gzip compressed data, was "findlike-1.4.2.tar", last modified: Tue Jul 18 16:44:30 2023, max compression
```

## Comparing `findlike-1.4.1.tar` & `findlike-1.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:01.052660 findlike-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-11 17:45:49.000000 findlike-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-11 17:46:01.052660 findlike-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-11 17:45:49.000000 findlike-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:01.052660 findlike-1.4.1/findlike/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:45:49.000000 findlike-1.4.1/findlike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 17:45:49.000000 findlike-1.4.1/findlike/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-11 17:45:49.000000 findlike-1.4.1/findlike/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-11 17:45:49.000000 findlike-1.4.1/findlike/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-11 17:45:49.000000 findlike-1.4.1/findlike/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-11 17:45:49.000000 findlike-1.4.1/findlike/markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-11 17:45:49.000000 findlike-1.4.1/findlike/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-11 17:45:49.000000 findlike-1.4.1/findlike/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-11 17:45:49.000000 findlike-1.4.1/findlike/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:01.052660 findlike-1.4.1/findlike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-11 17:46:01.000000 findlike-1.4.1/findlike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-11 17:46:01.000000 findlike-1.4.1/findlike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:46:01.000000 findlike-1.4.1/findlike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 17:46:01.000000 findlike-1.4.1/findlike.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 17:46:01.000000 findlike-1.4.1/findlike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 17:46:01.000000 findlike-1.4.1/findlike.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-11 17:45:49.000000 findlike-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:46:01.052660 findlike-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:46:01.052660 findlike-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-11 17:45:49.000000 findlike-1.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-11 17:45:49.000000 findlike-1.4.1/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-11 17:45:49.000000 findlike-1.4.1/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-11 17:45:49.000000 findlike-1.4.1/tests/test_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-11 17:45:49.000000 findlike-1.4.1/tests/test_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:44:30.251138 findlike-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 16:44:18.000000 findlike-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-18 16:44:30.251138 findlike-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-18 16:44:18.000000 findlike-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:44:30.251138 findlike-1.4.2/findlike/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:44:18.000000 findlike-1.4.2/findlike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-18 16:44:18.000000 findlike-1.4.2/findlike/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-18 16:44:18.000000 findlike-1.4.2/findlike/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-18 16:44:18.000000 findlike-1.4.2/findlike/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-18 16:44:18.000000 findlike-1.4.2/findlike/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-18 16:44:18.000000 findlike-1.4.2/findlike/markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-18 16:44:18.000000 findlike-1.4.2/findlike/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-18 16:44:18.000000 findlike-1.4.2/findlike/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-18 16:44:18.000000 findlike-1.4.2/findlike/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:44:30.251138 findlike-1.4.2/findlike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-18 16:44:30.000000 findlike-1.4.2/findlike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-18 16:44:30.000000 findlike-1.4.2/findlike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:44:30.000000 findlike-1.4.2/findlike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 16:44:30.000000 findlike-1.4.2/findlike.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-18 16:44:30.000000 findlike-1.4.2/findlike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 16:44:30.000000 findlike-1.4.2/findlike.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-18 16:44:18.000000 findlike-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 16:44:30.251138 findlike-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:44:30.251138 findlike-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-18 16:44:18.000000 findlike-1.4.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-18 16:44:18.000000 findlike-1.4.2/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 16:44:18.000000 findlike-1.4.2/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-18 16:44:18.000000 findlike-1.4.2/tests/test_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-18 16:44:18.000000 findlike-1.4.2/tests/test_processor.py
```

### Comparing `findlike-1.4.1/LICENSE` & `findlike-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/PKG-INFO` & `findlike-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findlike
-Version: 1.4.1
+Version: 1.4.2
 Summary: findlike is a package to retrieve similar documents
 Author-email: Bruno Arine <bruno.arine@runbox.com>
 Project-URL: Homepage, http://www.github.com/brunoarine/findlike
 Project-URL: Repository, https://github.com/brunoarine/findlike.git
 Project-URL: Bug Tracker, http://www.github.com/brunoarine/findlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `findlike-1.4.1/README.md` & `findlike-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/findlike/cli.py` & `findlike-1.4.2/findlike/cli.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/findlike/constants.py` & `findlike-1.4.2/findlike/constants.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/findlike/format.py` & `findlike-1.4.2/findlike/format.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/findlike/markup.py` & `findlike-1.4.2/findlike/markup.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/findlike/preprocessing.py` & `findlike-1.4.2/findlike/preprocessing.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/findlike/utils.py` & `findlike-1.4.2/findlike/utils.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/findlike/wrappers.py` & `findlike-1.4.2/findlike/wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,10 +55,11 @@
         clean_docs = [self.processor.preprocessor(d) for d in documents]
         self.tokenized_documents_ = [
             self.processor.tokenizer(d) for d in clean_docs
         ]
         self._model = BM25Okapi(self.tokenized_documents_)
 
     def get_scores(self, source: str):
-        tokenized_source = self.processor.tokenizer(source)
+        clean_source = self.processor.preprocessor(source)
+        tokenized_source = self.processor.tokenizer(clean_source)
         scores = self._model.get_scores(tokenized_source)
         return scores
```

### Comparing `findlike-1.4.1/findlike.egg-info/PKG-INFO` & `findlike-1.4.2/findlike.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findlike
-Version: 1.4.1
+Version: 1.4.2
 Summary: findlike is a package to retrieve similar documents
 Author-email: Bruno Arine <bruno.arine@runbox.com>
 Project-URL: Homepage, http://www.github.com/brunoarine/findlike
 Project-URL: Repository, https://github.com/brunoarine/findlike.git
 Project-URL: Bug Tracker, http://www.github.com/brunoarine/findlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `findlike-1.4.1/findlike.egg-info/SOURCES.txt` & `findlike-1.4.2/findlike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/pyproject.toml` & `findlike-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "findlike"
-version = "1.4.1"
+version = "1.4.2"
 authors = [{ name = "Bruno Arine", email = "bruno.arine@runbox.com" }]
 description = "findlike is a package to retrieve similar documents"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `findlike-1.4.1/tests/test_cli.py` & `findlike-1.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/tests/test_corpus.py` & `findlike-1.4.2/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/tests/test_format.py` & `findlike-1.4.2/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/tests/test_markup.py` & `findlike-1.4.2/tests/test_markup.py`

 * *Files identical despite different names*

### Comparing `findlike-1.4.1/tests/test_processor.py` & `findlike-1.4.2/tests/test_processor.py`

 * *Files identical despite different names*

