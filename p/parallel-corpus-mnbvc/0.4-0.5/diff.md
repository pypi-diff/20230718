# Comparing `tmp/parallel_corpus_mnbvc-0.4.tar.gz` & `tmp/parallel_corpus_mnbvc-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus_mnbvc-0.4.tar", last modified: Tue Jul 18 16:02:20 2023, max compression
+gzip compressed data, was "parallel_corpus_mnbvc-0.5.tar", last modified: Tue Jul 18 16:09:52 2023, max compression
```

## Comparing `parallel_corpus_mnbvc-0.4.tar` & `parallel_corpus_mnbvc-0.5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/
--rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.4/LICENSE
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.4/README.md
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/alignment/
--rw-rw-r--   0 ran       (1000) ran       (1000)       43 2023-07-18 15:33:15.000000 parallel_corpus_mnbvc-0.4/alignment/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.4/alignment/batch_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.4/alignment/batch_sequential_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.4/alignment/batch_sequential_for_one_file.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-0.4/alignment/evaluate_segmentation.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.4/alignment/rule_based_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.4/alignment/text_segmenter.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.4/alignment/utils.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/download_data/
--rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 15:33:02.000000 parallel_corpus_mnbvc-0.4/download_data/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-0.4/download_data/download_un_corpus.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)      559 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/SOURCES.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/dependency_links.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/requires.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/top_level.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/setup.cfg
--rw-rw-r--   0 ran       (1000) ran       (1000)      869 2023-07-18 16:02:13.000000 parallel_corpus_mnbvc-0.4/setup.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:09:52.882780 parallel_corpus_mnbvc-0.5/
+-rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.5/LICENSE
+-rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:06:49.000000 parallel_corpus_mnbvc-0.5/MANIFEST.in
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:09:52.882780 parallel_corpus_mnbvc-0.5/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.5/README.md
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:09:52.882780 parallel_corpus_mnbvc-0.5/alignment/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       43 2023-07-18 15:33:15.000000 parallel_corpus_mnbvc-0.5/alignment/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.5/alignment/batch_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.5/alignment/batch_sequential_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.5/alignment/batch_sequential_for_one_file.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-0.5/alignment/evaluate_segmentation.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.5/alignment/rule_based_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.5/alignment/text_segmenter.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.5/alignment/utils.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:09:52.882780 parallel_corpus_mnbvc-0.5/download_data/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 15:33:02.000000 parallel_corpus_mnbvc-0.5/download_data/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-0.5/download_data/download_un_corpus.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:09:52.882780 parallel_corpus_mnbvc-0.5/parallel_corpus_mnbvc.egg-info/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:09:52.000000 parallel_corpus_mnbvc-0.5/parallel_corpus_mnbvc.egg-info/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)      588 2023-07-18 16:09:52.000000 parallel_corpus_mnbvc-0.5/parallel_corpus_mnbvc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 16:09:52.000000 parallel_corpus_mnbvc-0.5/parallel_corpus_mnbvc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 16:09:52.000000 parallel_corpus_mnbvc-0.5/parallel_corpus_mnbvc.egg-info/requires.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:09:52.000000 parallel_corpus_mnbvc-0.5/parallel_corpus_mnbvc.egg-info/top_level.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.5/requirements.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 16:09:52.882780 parallel_corpus_mnbvc-0.5/setup.cfg
+-rw-rw-r--   0 ran       (1000) ran       (1000)      570 2023-07-18 16:07:30.000000 parallel_corpus_mnbvc-0.5/setup.py
```

### Comparing `parallel_corpus_mnbvc-0.4/LICENSE` & `parallel_corpus_mnbvc-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/README.md` & `parallel_corpus_mnbvc-0.5/README.md`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/alignment/batch_detector.py` & `parallel_corpus_mnbvc-0.5/alignment/batch_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/alignment/batch_sequential_detector.py` & `parallel_corpus_mnbvc-0.5/alignment/batch_sequential_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/alignment/batch_sequential_for_one_file.py` & `parallel_corpus_mnbvc-0.5/alignment/batch_sequential_for_one_file.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/alignment/evaluate_segmentation.py` & `parallel_corpus_mnbvc-0.5/alignment/evaluate_segmentation.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/alignment/rule_based_detector.py` & `parallel_corpus_mnbvc-0.5/alignment/rule_based_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/alignment/text_segmenter.py` & `parallel_corpus_mnbvc-0.5/alignment/text_segmenter.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/alignment/utils.py` & `parallel_corpus_mnbvc-0.5/alignment/utils.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/download_data/download_un_corpus.py` & `parallel_corpus_mnbvc-0.5/download_data/download_un_corpus.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/SOURCES.txt` & `parallel_corpus_mnbvc-0.5/parallel_corpus_mnbvc.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 alignment/__init__.py
 alignment/batch_detector.py
 alignment/batch_sequential_detector.py
 alignment/batch_sequential_for_one_file.py
 alignment/evaluate_segmentation.py
 alignment/rule_based_detector.py
```

