# Comparing `tmp/parallel_corpus_mnbvc-0.1.tar.gz` & `tmp/parallel_corpus_mnbvc-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus_mnbvc-0.1.tar", last modified: Tue Jul 18 15:35:24 2023, max compression
+gzip compressed data, was "parallel_corpus_mnbvc-0.2.tar", last modified: Tue Jul 18 15:40:21 2023, max compression
```

## Comparing `parallel_corpus_mnbvc-0.1.tar` & `parallel_corpus_mnbvc-0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:35:24.342303 parallel_corpus_mnbvc-0.1/
--rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.1/LICENSE
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 15:35:24.342303 parallel_corpus_mnbvc-0.1/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.1/README.md
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:35:24.342303 parallel_corpus_mnbvc-0.1/alignment/
--rw-rw-r--   0 ran       (1000) ran       (1000)       43 2023-07-18 15:33:15.000000 parallel_corpus_mnbvc-0.1/alignment/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.1/alignment/batch_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.1/alignment/batch_sequential_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.1/alignment/batch_sequential_for_one_file.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-0.1/alignment/evaluate_segmentation.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.1/alignment/rule_based_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.1/alignment/text_segmenter.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.1/alignment/utils.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:35:24.342303 parallel_corpus_mnbvc-0.1/download_data/
--rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 15:33:02.000000 parallel_corpus_mnbvc-0.1/download_data/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-0.1/download_data/download_un_corpus.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:35:24.342303 parallel_corpus_mnbvc-0.1/parallel_corpus_mnbvc.egg-info/
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 15:35:24.000000 parallel_corpus_mnbvc-0.1/parallel_corpus_mnbvc.egg-info/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)      559 2023-07-18 15:35:24.000000 parallel_corpus_mnbvc-0.1/parallel_corpus_mnbvc.egg-info/SOURCES.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 15:35:24.000000 parallel_corpus_mnbvc-0.1/parallel_corpus_mnbvc.egg-info/dependency_links.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 15:35:24.000000 parallel_corpus_mnbvc-0.1/parallel_corpus_mnbvc.egg-info/requires.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 15:35:24.000000 parallel_corpus_mnbvc-0.1/parallel_corpus_mnbvc.egg-info/top_level.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 15:35:24.342303 parallel_corpus_mnbvc-0.1/setup.cfg
--rw-rw-r--   0 ran       (1000) ran       (1000)      488 2023-07-18 15:35:18.000000 parallel_corpus_mnbvc-0.1/setup.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:40:21.068487 parallel_corpus_mnbvc-0.2/
+-rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.2/LICENSE
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 15:40:21.068487 parallel_corpus_mnbvc-0.2/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.2/README.md
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:40:21.068487 parallel_corpus_mnbvc-0.2/alignment/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       43 2023-07-18 15:33:15.000000 parallel_corpus_mnbvc-0.2/alignment/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.2/alignment/batch_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.2/alignment/batch_sequential_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.2/alignment/batch_sequential_for_one_file.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-0.2/alignment/evaluate_segmentation.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.2/alignment/rule_based_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.2/alignment/text_segmenter.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.2/alignment/utils.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:40:21.068487 parallel_corpus_mnbvc-0.2/download_data/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 15:33:02.000000 parallel_corpus_mnbvc-0.2/download_data/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-0.2/download_data/download_un_corpus.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:40:21.068487 parallel_corpus_mnbvc-0.2/parallel_corpus_mnbvc.egg-info/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 15:40:21.000000 parallel_corpus_mnbvc-0.2/parallel_corpus_mnbvc.egg-info/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)      559 2023-07-18 15:40:21.000000 parallel_corpus_mnbvc-0.2/parallel_corpus_mnbvc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 15:40:21.000000 parallel_corpus_mnbvc-0.2/parallel_corpus_mnbvc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 15:40:21.000000 parallel_corpus_mnbvc-0.2/parallel_corpus_mnbvc.egg-info/requires.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 15:40:21.000000 parallel_corpus_mnbvc-0.2/parallel_corpus_mnbvc.egg-info/top_level.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 15:40:21.068487 parallel_corpus_mnbvc-0.2/setup.cfg
+-rw-rw-r--   0 ran       (1000) ran       (1000)      486 2023-07-18 15:40:14.000000 parallel_corpus_mnbvc-0.2/setup.py
```

### Comparing `parallel_corpus_mnbvc-0.1/LICENSE` & `parallel_corpus_mnbvc-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/README.md` & `parallel_corpus_mnbvc-0.2/README.md`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/alignment/batch_detector.py` & `parallel_corpus_mnbvc-0.2/alignment/batch_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/alignment/batch_sequential_detector.py` & `parallel_corpus_mnbvc-0.2/alignment/batch_sequential_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/alignment/batch_sequential_for_one_file.py` & `parallel_corpus_mnbvc-0.2/alignment/batch_sequential_for_one_file.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/alignment/evaluate_segmentation.py` & `parallel_corpus_mnbvc-0.2/alignment/evaluate_segmentation.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/alignment/rule_based_detector.py` & `parallel_corpus_mnbvc-0.2/alignment/rule_based_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/alignment/text_segmenter.py` & `parallel_corpus_mnbvc-0.2/alignment/text_segmenter.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/alignment/utils.py` & `parallel_corpus_mnbvc-0.2/alignment/utils.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/download_data/download_un_corpus.py` & `parallel_corpus_mnbvc-0.2/download_data/download_un_corpus.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.1/parallel_corpus_mnbvc.egg-info/SOURCES.txt` & `parallel_corpus_mnbvc-0.2/parallel_corpus_mnbvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

