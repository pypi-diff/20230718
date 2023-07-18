# Comparing `tmp/parallel_corpus_mnbvc-0.6.tar.gz` & `tmp/parallel_corpus_mnbvc-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_corpus_mnbvc-0.6.tar", last modified: Tue Jul 18 16:53:26 2023, max compression
+gzip compressed data, was "parallel_corpus_mnbvc-0.7.tar", last modified: Tue Jul 18 16:56:54 2023, max compression
```

## Comparing `parallel_corpus_mnbvc-0.6.tar` & `parallel_corpus_mnbvc-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:53:26.843122 parallel_corpus_mnbvc-0.6/
--rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.6/LICENSE
--rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:06:49.000000 parallel_corpus_mnbvc-0.6/MANIFEST.in
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:53:26.843122 parallel_corpus_mnbvc-0.6/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.6/README.md
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:53:26.843122 parallel_corpus_mnbvc-0.6/parallel_corpus_mnbvc/
--rw-rw-r--   0 ran       (1000) ran       (1000)      120 2023-07-18 16:52:38.000000 parallel_corpus_mnbvc-0.6/parallel_corpus_mnbvc/__init__.py
-drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:53:26.843122 parallel_corpus_mnbvc-0.6/parallel_corpus_mnbvc.egg-info/
--rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:53:26.000000 parallel_corpus_mnbvc-0.6/parallel_corpus_mnbvc.egg-info/PKG-INFO
--rw-rw-r--   0 ran       (1000) ran       (1000)      313 2023-07-18 16:53:26.000000 parallel_corpus_mnbvc-0.6/parallel_corpus_mnbvc.egg-info/SOURCES.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 16:53:26.000000 parallel_corpus_mnbvc-0.6/parallel_corpus_mnbvc.egg-info/dependency_links.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 16:53:26.000000 parallel_corpus_mnbvc-0.6/parallel_corpus_mnbvc.egg-info/requires.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       22 2023-07-18 16:53:26.000000 parallel_corpus_mnbvc-0.6/parallel_corpus_mnbvc.egg-info/top_level.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.6/requirements.txt
--rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 16:53:26.843122 parallel_corpus_mnbvc-0.6/setup.cfg
--rw-rw-r--   0 ran       (1000) ran       (1000)      580 2023-07-18 16:53:08.000000 parallel_corpus_mnbvc-0.6/setup.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/
+-rw-rw-r--   0 ran       (1000) ran       (1000)    11357 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.7/LICENSE
+-rw-rw-r--   0 ran       (1000) ran       (1000)       24 2023-07-18 16:06:49.000000 parallel_corpus_mnbvc-0.7/MANIFEST.in
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)     1113 2023-06-09 04:45:49.000000 parallel_corpus_mnbvc-0.7/README.md
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      120 2023-07-18 16:52:38.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc/__init__.py
+drwxrwxr-x   0 ran       (1000) ran       (1000)        0 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/
+-rw-rw-r--   0 ran       (1000) ran       (1000)      280 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/PKG-INFO
+-rw-rw-r--   0 ran       (1000) ran       (1000)      313 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)        1 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       89 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/requires.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       22 2023-07-18 16:56:54.000000 parallel_corpus_mnbvc-0.7/parallel_corpus_mnbvc.egg-info/top_level.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       90 2023-07-18 15:29:34.000000 parallel_corpus_mnbvc-0.7/requirements.txt
+-rw-rw-r--   0 ran       (1000) ran       (1000)       38 2023-07-18 16:56:54.200160 parallel_corpus_mnbvc-0.7/setup.cfg
+-rw-rw-r--   0 ran       (1000) ran       (1000)      580 2023-07-18 16:56:44.000000 parallel_corpus_mnbvc-0.7/setup.py
```

### Comparing `parallel_corpus_mnbvc-0.6/LICENSE` & `parallel_corpus_mnbvc-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.6/README.md` & `parallel_corpus_mnbvc-0.7/README.md`

 * *Files identical despite different names*

### Comparing `parallel_corpus_mnbvc-0.6/setup.py` & `parallel_corpus_mnbvc-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     required = f.read().splitlines()
 
 setup(
     name='parallel_corpus_mnbvc',
-    version='0.6',
+    version='0.7',
     author='ranWang',
     author_email='redamancy0326@gmail.com',
     description='parallel corpus dataset from the pypi repository of the mnbvc project',
     url='https://github.com/liyongsea/parallel_corpus_mnbvc',
     packages=["parallel_corpus_mnbvc"],
     include_package_data=True,
     install_requires=required,
```

