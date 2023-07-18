# Comparing `tmp/parallel_corpus_mnbvc-1.0.2.tar.gz` & `tmp/parallel_corpus_mnbvc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus_mnbvc-1.0.2.tar", last modified: Tue Jul 18 17:57:07 2023, max compression
+gzip compressed data, was "parallel_corpus_mnbvc-1.0.3.tar", last modified: Tue Jul 18 18:04:42 2023, max compression
```

## Comparing `parallel_corpus_mnbvc-1.0.2.tar` & `parallel_corpus_mnbvc-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:57:07.375981 parallel_corpus_mnbvc-1.0.2/
--rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.2/LICENSE
--rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:06:49.000000 parallel_corpus_mnbvc-1.0.2/MANIFEST.in
--rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-18 17:57:07.375981 parallel_corpus_mnbvc-1.0.2/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.2/README.md
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:57:07.375981 parallel_corpus_mnbvc-1.0.2/alignment/
--rw-rw-r--   0 ran       (1000) ran       (1000)       58 2023-07-18 17:50:51.000000 parallel_corpus_mnbvc-1.0.2/alignment/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.2/alignment/batch_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.2/alignment/batch_sequential_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.2/alignment/batch_sequential_for_one_file.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-1.0.2/alignment/evaluate_segmentation.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.2/alignment/rule_based_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.2/alignment/text_segmenter.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.2/alignment/utils.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:57:07.375981 parallel_corpus_mnbvc-1.0.2/download_data/
--rw-rw-r--   0 ran       (1000) ran       (1000)       62 2023-07-18 17:50:58.000000 parallel_corpus_mnbvc-1.0.2/download_data/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.2/download_data/download_un_corpus.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:57:07.375981 parallel_corpus_mnbvc-1.0.2/parallel_corpus_mnbvc.egg-info/
--rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-18 17:57:07.000000 parallel_corpus_mnbvc-1.0.2/parallel_corpus_mnbvc.egg-info/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)      613 2023-07-18 17:57:07.000000 parallel_corpus_mnbvc-1.0.2/parallel_corpus_mnbvc.egg-info/SOURCES.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 17:57:07.000000 parallel_corpus_mnbvc-1.0.2/parallel_corpus_mnbvc.egg-info/dependency_links.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 17:57:07.000000 parallel_corpus_mnbvc-1.0.2/parallel_corpus_mnbvc.egg-info/requires.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 17:57:07.000000 parallel_corpus_mnbvc-1.0.2/parallel_corpus_mnbvc.egg-info/top_level.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       53 2023-07-18 17:56:48.000000 parallel_corpus_mnbvc-1.0.2/parallel_corpus_mnbvc.py
--rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.2/requirements.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 17:57:07.375981 parallel_corpus_mnbvc-1.0.2/setup.cfg
--rw-rw-r--   0 ran       (1000) ran       (1000)      614 2023-07-18 17:57:00.000000 parallel_corpus_mnbvc-1.0.2/setup.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 18:04:42.960639 parallel_corpus_mnbvc-1.0.3/
+-rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.3/LICENSE
+-rw-rw-r--   0 ran       (1000) ran       (1000)       80 2023-07-18 18:04:18.000000 parallel_corpus_mnbvc-1.0.3/MANIFEST.in
+-rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-18 18:04:42.960639 parallel_corpus_mnbvc-1.0.3/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.3/README.md
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 18:04:42.960639 parallel_corpus_mnbvc-1.0.3/alignment/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       58 2023-07-18 17:50:51.000000 parallel_corpus_mnbvc-1.0.3/alignment/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.3/alignment/batch_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.3/alignment/batch_sequential_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.3/alignment/batch_sequential_for_one_file.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-1.0.3/alignment/evaluate_segmentation.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.3/alignment/rule_based_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-1.0.3/alignment/text_segmenter.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.3/alignment/utils.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 18:04:42.960639 parallel_corpus_mnbvc-1.0.3/download_data/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       62 2023-07-18 17:50:58.000000 parallel_corpus_mnbvc-1.0.3/download_data/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-1.0.3/download_data/download_un_corpus.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 18:04:42.960639 parallel_corpus_mnbvc-1.0.3/parallel_corpus_mnbvc.egg-info/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      282 2023-07-18 18:04:42.000000 parallel_corpus_mnbvc-1.0.3/parallel_corpus_mnbvc.egg-info/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)      613 2023-07-18 18:04:42.000000 parallel_corpus_mnbvc-1.0.3/parallel_corpus_mnbvc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 18:04:42.000000 parallel_corpus_mnbvc-1.0.3/parallel_corpus_mnbvc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 18:04:42.000000 parallel_corpus_mnbvc-1.0.3/parallel_corpus_mnbvc.egg-info/requires.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 18:04:42.000000 parallel_corpus_mnbvc-1.0.3/parallel_corpus_mnbvc.egg-info/top_level.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       27 2023-07-18 18:03:43.000000 parallel_corpus_mnbvc-1.0.3/parallel_corpus_mnbvc.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-1.0.3/requirements.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 18:04:42.960639 parallel_corpus_mnbvc-1.0.3/setup.cfg
+-rw-rw-r--   0 ran       (1000) ran       (1000)      614 2023-07-18 18:04:41.000000 parallel_corpus_mnbvc-1.0.3/setup.py
```

### Comparing `parallel_corpus_mnbvc-1.0.2/LICENSE` & `parallel_corpus_mnbvc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/README.md` & `parallel_corpus_mnbvc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/alignment/batch_detector.py` & `parallel_corpus_mnbvc-1.0.3/alignment/batch_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/alignment/batch_sequential_detector.py` & `parallel_corpus_mnbvc-1.0.3/alignment/batch_sequential_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/alignment/batch_sequential_for_one_file.py` & `parallel_corpus_mnbvc-1.0.3/alignment/batch_sequential_for_one_file.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/alignment/evaluate_segmentation.py` & `parallel_corpus_mnbvc-1.0.3/alignment/evaluate_segmentation.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/alignment/rule_based_detector.py` & `parallel_corpus_mnbvc-1.0.3/alignment/rule_based_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/alignment/text_segmenter.py` & `parallel_corpus_mnbvc-1.0.3/alignment/text_segmenter.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/alignment/utils.py` & `parallel_corpus_mnbvc-1.0.3/alignment/utils.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/download_data/download_un_corpus.py` & `parallel_corpus_mnbvc-1.0.3/download_data/download_un_corpus.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/parallel_corpus_mnbvc.egg-info/SOURCES.txt` & `parallel_corpus_mnbvc-1.0.3/parallel_corpus_mnbvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-1.0.2/setup.py` & `parallel_corpus_mnbvc-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     required = f.read().splitlines()
 
 setup(
     name='parallel_corpus_mnbvc',
-    version='1.0.2',
+    version='1.0.3',
     author='ranWang',
     author_email='redamancy0326@gmail.com',
     description='parallel corpus dataset from the pypi repository of the mnbvc project',
     url='https://github.com/liyongsea/parallel_corpus_mnbvc',
     packages=find_packages(),
     py_modules=['parallel_corpus_mnbvc'],
     include_package_data=True,
```

