# Comparing `tmp/parallel_corpus_mnbvc-1.0.0.tar.gz` & `tmp/parallel_corpus_mnbvc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus_mnbvc-1.0.0.tar", last modified: Tue Jul 18 17:37:44 2023, max compression
+gzip compressed data, was "parallel_corpus_mnbvc-1.0.1.tar", last modified: Tue Jul 18 17:51:24 2023, max compression
```

## Comparing `parallel_corpus_mnbvc-1.0.0.tar` & `parallel_corpus_mnbvc-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:37:44.720902 parallel_corpus_mnbvc-1.0.0/
--rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.0/LICENSE
--rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:06:49.000000 parallel_corpus_mnbvc-1.0.0/MANIFEST.in
--rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-18 17:37:44.720902 parallel_corpus_mnbvc-1.0.0/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.0/README.md
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:37:44.720902 parallel_corpus_mnbvc-1.0.0/alignment/
--rw-rw-r--   0 ran       (1000) ran       (1000)       41 2023-07-18 16:56:14.000000 parallel_corpus_mnbvc-1.0.0/alignment/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.0/alignment/batch_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.0/alignment/batch_sequential_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.0/alignment/batch_sequential_for_one_file.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-1.0.0/alignment/evaluate_segmentation.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.0/alignment/rule_based_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.0/alignment/text_segmenter.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.0/alignment/utils.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:37:44.720902 parallel_corpus_mnbvc-1.0.0/download_data/
--rw-rw-r--   0 ran       (1000) ran       (1000)       45 2023-07-18 16:56:23.000000 parallel_corpus_mnbvc-1.0.0/download_data/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.0/download_data/download_un_corpus.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:37:44.720902 parallel_corpus_mnbvc-1.0.0/parallel_corpus_mnbvc.egg-info/
--rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-18 17:37:44.000000 parallel_corpus_mnbvc-1.0.0/parallel_corpus_mnbvc.egg-info/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)      613 2023-07-18 17:37:44.000000 parallel_corpus_mnbvc-1.0.0/parallel_corpus_mnbvc.egg-info/SOURCES.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 17:37:44.000000 parallel_corpus_mnbvc-1.0.0/parallel_corpus_mnbvc.egg-info/dependency_links.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 17:37:44.000000 parallel_corpus_mnbvc-1.0.0/parallel_corpus_mnbvc.egg-info/requires.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 17:37:44.000000 parallel_corpus_mnbvc-1.0.0/parallel_corpus_mnbvc.egg-info/top_level.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       39 2023-07-18 17:28:13.000000 parallel_corpus_mnbvc-1.0.0/parallel_corpus_mnbvc.py
--rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.0/requirements.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 17:37:44.720902 parallel_corpus_mnbvc-1.0.0/setup.cfg
--rw-rw-r--   0 ran       (1000) ran       (1000)      614 2023-07-18 17:37:32.000000 parallel_corpus_mnbvc-1.0.0/setup.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:51:24.251670 parallel_corpus_mnbvc-1.0.1/
+-rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.1/LICENSE
+-rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:06:49.000000 parallel_corpus_mnbvc-1.0.1/MANIFEST.in
+-rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-18 17:51:24.251670 parallel_corpus_mnbvc-1.0.1/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.1/README.md
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:51:24.251670 parallel_corpus_mnbvc-1.0.1/alignment/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       58 2023-07-18 17:50:51.000000 parallel_corpus_mnbvc-1.0.1/alignment/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.1/alignment/batch_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.1/alignment/batch_sequential_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.1/alignment/batch_sequential_for_one_file.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-1.0.1/alignment/evaluate_segmentation.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.1/alignment/rule_based_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.1/alignment/text_segmenter.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.1/alignment/utils.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:51:24.251670 parallel_corpus_mnbvc-1.0.1/download_data/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       62 2023-07-18 17:50:58.000000 parallel_corpus_mnbvc-1.0.1/download_data/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.1/download_data/download_un_corpus.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:51:24.251670 parallel_corpus_mnbvc-1.0.1/parallel_corpus_mnbvc.egg-info/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-18 17:51:24.000000 parallel_corpus_mnbvc-1.0.1/parallel_corpus_mnbvc.egg-info/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)      613 2023-07-18 17:51:24.000000 parallel_corpus_mnbvc-1.0.1/parallel_corpus_mnbvc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 17:51:24.000000 parallel_corpus_mnbvc-1.0.1/parallel_corpus_mnbvc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 17:51:24.000000 parallel_corpus_mnbvc-1.0.1/parallel_corpus_mnbvc.egg-info/requires.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 17:51:24.000000 parallel_corpus_mnbvc-1.0.1/parallel_corpus_mnbvc.egg-info/top_level.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       39 2023-07-18 17:28:13.000000 parallel_corpus_mnbvc-1.0.1/parallel_corpus_mnbvc.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.1/requirements.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 17:51:24.251670 parallel_corpus_mnbvc-1.0.1/setup.cfg
+-rw-rw-r--   0 ran       (1000) ran       (1000)      614 2023-07-18 17:51:18.000000 parallel_corpus_mnbvc-1.0.1/setup.py
```

### Comparing `parallel_corpus_mnbvc-1.0.0/LICENSE` & `parallel_corpus_mnbvc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/README.md` & `parallel_corpus_mnbvc-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/alignment/batch_detector.py` & `parallel_corpus_mnbvc-1.0.1/alignment/batch_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/alignment/batch_sequential_detector.py` & `parallel_corpus_mnbvc-1.0.1/alignment/batch_sequential_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/alignment/batch_sequential_for_one_file.py` & `parallel_corpus_mnbvc-1.0.1/alignment/batch_sequential_for_one_file.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/alignment/evaluate_segmentation.py` & `parallel_corpus_mnbvc-1.0.1/alignment/evaluate_segmentation.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/alignment/rule_based_detector.py` & `parallel_corpus_mnbvc-1.0.1/alignment/rule_based_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/alignment/text_segmenter.py` & `parallel_corpus_mnbvc-1.0.1/alignment/text_segmenter.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/alignment/utils.py` & `parallel_corpus_mnbvc-1.0.1/alignment/utils.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/download_data/download_un_corpus.py` & `parallel_corpus_mnbvc-1.0.1/download_data/download_un_corpus.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/parallel_corpus_mnbvc.egg-info/SOURCES.txt` & `parallel_corpus_mnbvc-1.0.1/parallel_corpus_mnbvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.0/setup.py` & `parallel_corpus_mnbvc-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     required = f.read().splitlines()
 
 setup(
     name='parallel_corpus_mnbvc',
-    version='1.0.0',
+    version='1.0.1',
     author='ranWang',
     author_email='redamancy0326@gmail.com',
     description='parallel corpus dataset from the pypi repository of the mnbvc project',
     url='https://github.com/liyongsea/parallel_corpus_mnbvc',
     packages=find_packages(),
     py_modules=['parallel_corpus_mnbvc'],
     include_package_data=True,
```

