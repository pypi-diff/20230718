# Comparing `tmp/parallel_corpus_mnbvc-0.3.tar.gz` & `tmp/parallel_corpus_mnbvc-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus_mnbvc-0.3.tar", last modified: Tue Jul 18 15:53:40 2023, max compression
+gzip compressed data, was "parallel_corpus_mnbvc-0.4.tar", last modified: Tue Jul 18 16:02:20 2023, max compression
```

## Comparing `parallel_corpus_mnbvc-0.3.tar` & `parallel_corpus_mnbvc-0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:53:40.160878 parallel_corpus_mnbvc-0.3/
--rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.3/LICENSE
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 15:53:40.160878 parallel_corpus_mnbvc-0.3/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.3/README.md
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:53:40.160878 parallel_corpus_mnbvc-0.3/alignment/
--rw-rw-r--   0 ran       (1000) ran       (1000)       43 2023-07-18 15:33:15.000000 parallel_corpus_mnbvc-0.3/alignment/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.3/alignment/batch_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.3/alignment/batch_sequential_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.3/alignment/batch_sequential_for_one_file.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-0.3/alignment/evaluate_segmentation.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.3/alignment/rule_based_detector.py
--rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.3/alignment/text_segmenter.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.3/alignment/utils.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:53:40.160878 parallel_corpus_mnbvc-0.3/download_data/
--rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 15:33:02.000000 parallel_corpus_mnbvc-0.3/download_data/__init__.py
--rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-0.3/download_data/download_un_corpus.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 15:53:40.160878 parallel_corpus_mnbvc-0.3/parallel_corpus_mnbvc.egg-info/
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 15:53:40.000000 parallel_corpus_mnbvc-0.3/parallel_corpus_mnbvc.egg-info/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)      559 2023-07-18 15:53:40.000000 parallel_corpus_mnbvc-0.3/parallel_corpus_mnbvc.egg-info/SOURCES.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 15:53:40.000000 parallel_corpus_mnbvc-0.3/parallel_corpus_mnbvc.egg-info/dependency_links.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 15:53:40.000000 parallel_corpus_mnbvc-0.3/parallel_corpus_mnbvc.egg-info/requires.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 15:53:40.000000 parallel_corpus_mnbvc-0.3/parallel_corpus_mnbvc.egg-info/top_level.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 15:53:40.160878 parallel_corpus_mnbvc-0.3/setup.cfg
--rw-rw-r--   0 ran       (1000) ran       (1000)      652 2023-07-18 15:53:28.000000 parallel_corpus_mnbvc-0.3/setup.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/
+-rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.4/LICENSE
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.4/README.md
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/alignment/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       43 2023-07-18 15:33:15.000000 parallel_corpus_mnbvc-0.4/alignment/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.4/alignment/batch_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.4/alignment/batch_sequential_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.4/alignment/batch_sequential_for_one_file.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-0.4/alignment/evaluate_segmentation.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.4/alignment/rule_based_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.4/alignment/text_segmenter.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.4/alignment/utils.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/download_data/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 15:33:02.000000 parallel_corpus_mnbvc-0.4/download_data/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-0.4/download_data/download_un_corpus.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)      559 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/requires.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:02:20.000000 parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/top_level.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 16:02:20.522669 parallel_corpus_mnbvc-0.4/setup.cfg
+-rw-rw-r--   0 ran       (1000) ran       (1000)      869 2023-07-18 16:02:13.000000 parallel_corpus_mnbvc-0.4/setup.py
```

### Comparing `parallel_corpus_mnbvc-0.3/LICENSE` & `parallel_corpus_mnbvc-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/README.md` & `parallel_corpus_mnbvc-0.4/README.md`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/alignment/batch_detector.py` & `parallel_corpus_mnbvc-0.4/alignment/batch_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/alignment/batch_sequential_detector.py` & `parallel_corpus_mnbvc-0.4/alignment/batch_sequential_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/alignment/batch_sequential_for_one_file.py` & `parallel_corpus_mnbvc-0.4/alignment/batch_sequential_for_one_file.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/alignment/evaluate_segmentation.py` & `parallel_corpus_mnbvc-0.4/alignment/evaluate_segmentation.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/alignment/rule_based_detector.py` & `parallel_corpus_mnbvc-0.4/alignment/rule_based_detector.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/alignment/text_segmenter.py` & `parallel_corpus_mnbvc-0.4/alignment/text_segmenter.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/alignment/utils.py` & `parallel_corpus_mnbvc-0.4/alignment/utils.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/download_data/download_un_corpus.py` & `parallel_corpus_mnbvc-0.4/download_data/download_un_corpus.py`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/parallel_corpus_mnbvc.egg-info/SOURCES.txt` & `parallel_corpus_mnbvc-0.4/parallel_corpus_mnbvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.3/setup.py` & `parallel_corpus_mnbvc-0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import os
 from setuptools import setup, find_packages
 
 # 获取当前脚本的绝对路径
 here = os.path.abspath(os.path.dirname(__file__))
 
+requirements_file_loacl = os.path.join(here, "requirements.txt")
+
+if not os.path.exists(requirements_file_loacl):
+    requirements_file_loacl = os.path.join(here, "parallel_corpus_mnbvc.egg-info","requirements.txt")
+
 # 使用这个路径找到requirements.txt文件
 with open(os.path.join(here, "requirements.txt"), "r") as f:
     install_requires = [line.strip() for line in f]
  
 setup(
     name='parallel_corpus_mnbvc',
-    version='0.3',
+    version='0.4',
     author='ranWang',
     author_email='redamancy0326@gmail.com',
     description='parallel corpus dataset from the pypi repository of the mnbvc project',
     url='https://github.com/liyongsea/parallel_corpus_mnbvc',
     packages=find_packages(),
     install_requires=install_requires
 )
```

