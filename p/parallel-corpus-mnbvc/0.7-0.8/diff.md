# Comparing `tmp/parallel_corpus_mnbvc-0.7.tar.gz` & `tmp/parallel_corpus_mnbvc-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus_mnbvc-0.7.tar", last modified: Tue Jul 18 16:56:54 2023, max compression
+gzip compressed data, was "parallel_corpus_mnbvc-0.8.tar", last modified: Tue Jul 18 17:21:06 2023, max compression
```

## Comparing `parallel_corpus_mnbvc-0.7.tar` & `parallel_corpus_mnbvc-0.8.tar`

### file list

```diff
@@ -1,16 +1,27 @@
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/
--rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.7/LICENSE
--rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:06:49.000000 parallel_corpus_mnbvc-0.7/MANIFEST.in
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.7/README.md
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc/
--rw-rw-r--   0 ran       (1000) ran       (1000)      120 2023-07-18 16:52:38.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc/__init__.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)      313 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/SOURCES.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/dependency_links.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/requires.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       22 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/top_level.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.7/requirements.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/setup.cfg
--rw-rw-r--   0 ran       (1000) ran       (1000)      580 2023-07-18 16:56:44.000000 parallel_corpus_mnbvc-0.7/setup.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:21:06.441953 parallel_corpus_mnbvc-0.8/
+-rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.8/LICENSE
+-rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:06:49.000000 parallel_corpus_mnbvc-0.8/MANIFEST.in
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 17:21:06.441953 parallel_corpus_mnbvc-0.8/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.8/README.md
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:21:06.441953 parallel_corpus_mnbvc-0.8/alignment/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       41 2023-07-18 16:56:14.000000 parallel_corpus_mnbvc-0.8/alignment/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6084 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.8/alignment/batch_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    20466 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.8/alignment/batch_sequential_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1969 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.8/alignment/batch_sequential_for_one_file.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6764 2023-07-04 11:34:28.000000 parallel_corpus_mnbvc-0.8/alignment/evaluate_segmentation.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     8953 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.8/alignment/rule_based_detector.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)     6029 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.8/alignment/text_segmenter.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    12285 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.8/alignment/utils.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:21:06.441953 parallel_corpus_mnbvc-0.8/download_data/
+-rw-rw-r--   0 ran       (1000) ran       (1000)       45 2023-07-18 16:56:23.000000 parallel_corpus_mnbvc-0.8/download_data/__init__.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)    10603 2023-06-16 09:39:48.000000 parallel_corpus_mnbvc-0.8/download_data/download_un_corpus.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 17:21:06.441953 parallel_corpus_mnbvc-0.8/parallel_corpus_mnbvc.egg-info/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 17:21:06.000000 parallel_corpus_mnbvc-0.8/parallel_corpus_mnbvc.egg-info/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)      613 2023-07-18 17:21:06.000000 parallel_corpus_mnbvc-0.8/parallel_corpus_mnbvc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 17:21:06.000000 parallel_corpus_mnbvc-0.8/parallel_corpus_mnbvc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 17:21:06.000000 parallel_corpus_mnbvc-0.8/parallel_corpus_mnbvc.egg-info/requires.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       46 2023-07-18 17:21:06.000000 parallel_corpus_mnbvc-0.8/parallel_corpus_mnbvc.egg-info/top_level.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       83 2023-07-18 17:19:44.000000 parallel_corpus_mnbvc-0.8/parallel_corpus_mnbvc.py
+-rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.8/requirements.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 17:21:06.441953 parallel_corpus_mnbvc-0.8/setup.cfg
+-rw-rw-r--   0 ran       (1000) ran       (1000)      612 2023-07-18 17:21:02.000000 parallel_corpus_mnbvc-0.8/setup.py
```

### Comparing `parallel_corpus_mnbvc-0.7/LICENSE` & `parallel_corpus_mnbvc-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.7/README.md` & `parallel_corpus_mnbvc-0.8/README.md`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.7/setup.py` & `parallel_corpus_mnbvc-0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     required = f.read().splitlines()
 
 setup(
     name='parallel_corpus_mnbvc',
-    version='0.7',
+    version='0.8',
     author='ranWang',
     author_email='redamancy0326@gmail.com',
     description='parallel corpus dataset from the pypi repository of the mnbvc project',
     url='https://github.com/liyongsea/parallel_corpus_mnbvc',
-    packages=["parallel_corpus_mnbvc"],
+    packages=find_packages(),
+    py_modules=['parallel_corpus_mnbvc'],
     include_package_data=True,
     install_requires=required,
 )
```

