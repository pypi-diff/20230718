# Comparing `tmp/wtpsplit-1.2.2.tar.gz` & `tmp/wtpsplit-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/benjamin_cohere_com/wtpsplit/dist/.tmp-pbx5h2v6/wtpsplit-1.2.2.tar", last modified: Fri Jul 14 15:56:10 2023, max compression
+gzip compressed data, was "/home/benjamin_cohere_com/wtpsplit/dist/.tmp-ux__rqgg/wtpsplit-1.2.3.tar", last modified: Tue Jul 18 13:44:07 2023, max compression
```

## Comparing `wtpsplit-1.2.2.tar` & `wtpsplit-1.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-14 15:56:10.278079 wtpsplit-1.2.2/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1076 2023-06-19 12:40:26.000000 wtpsplit-1.2.2/LICENSE
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-14 15:56:10.278079 wtpsplit-1.2.2/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    13141 2023-07-14 15:52:54.000000 wtpsplit-1.2.2/README.md
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      173 2023-07-11 18:11:57.000000 wtpsplit-1.2.2/pyproject.toml
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-07-14 15:56:10.278079 wtpsplit-1.2.2/setup.cfg
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      637 2023-07-14 15:52:01.000000 wtpsplit-1.2.2/setup.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-14 15:56:10.274079 wtpsplit-1.2.2/wtpsplit/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    14632 2023-07-14 15:52:07.000000 wtpsplit-1.2.2/wtpsplit/__init__.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1055 2023-07-11 18:11:57.000000 wtpsplit-1.2.2/wtpsplit/configs.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-14 15:56:10.278079 wtpsplit-1.2.2/wtpsplit/data/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-06-19 12:40:26.000000 wtpsplit-1.2.2/wtpsplit/data/language_info.csv
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-06-19 12:40:26.000000 wtpsplit-1.2.2/wtpsplit/data/punctuation.json
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-06-19 12:40:26.000000 wtpsplit-1.2.2/wtpsplit/data/punctuation.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5384 2023-07-11 18:11:57.000000 wtpsplit-1.2.2/wtpsplit/extract.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    41378 2023-07-13 18:24:26.000000 wtpsplit-1.2.2/wtpsplit/models.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     6949 2023-07-14 15:48:34.000000 wtpsplit-1.2.2/wtpsplit/utils.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-14 15:56:10.274079 wtpsplit-1.2.2/wtpsplit.egg-info/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      401 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      103 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/requires.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-07-14 15:56:10.000000 wtpsplit-1.2.2/wtpsplit.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-18 13:44:07.080151 wtpsplit-1.2.3/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1076 2023-06-19 12:40:26.000000 wtpsplit-1.2.3/LICENSE
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-18 13:44:07.080151 wtpsplit-1.2.3/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    13141 2023-07-14 15:52:54.000000 wtpsplit-1.2.3/README.md
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      173 2023-07-11 18:11:57.000000 wtpsplit-1.2.3/pyproject.toml
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-07-18 13:44:07.080151 wtpsplit-1.2.3/setup.cfg
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      637 2023-07-18 13:42:08.000000 wtpsplit-1.2.3/setup.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-18 13:44:07.080151 wtpsplit-1.2.3/wtpsplit/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    14632 2023-07-18 13:42:14.000000 wtpsplit-1.2.3/wtpsplit/__init__.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     1055 2023-07-11 18:11:57.000000 wtpsplit-1.2.3/wtpsplit/configs.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-18 13:44:07.080151 wtpsplit-1.2.3/wtpsplit/data/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-06-19 12:40:26.000000 wtpsplit-1.2.3/wtpsplit/data/language_info.csv
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-06-19 12:40:26.000000 wtpsplit-1.2.3/wtpsplit/data/punctuation.json
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-06-19 12:40:26.000000 wtpsplit-1.2.3/wtpsplit/data/punctuation.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5596 2023-07-18 13:44:01.000000 wtpsplit-1.2.3/wtpsplit/extract.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    41378 2023-07-13 18:24:26.000000 wtpsplit-1.2.3/wtpsplit/models.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     6949 2023-07-14 15:48:34.000000 wtpsplit-1.2.3/wtpsplit/utils.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-07-18 13:44:07.080151 wtpsplit-1.2.3/wtpsplit.egg-info/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      268 2023-07-18 13:44:07.000000 wtpsplit-1.2.3/wtpsplit.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      401 2023-07-18 13:44:07.000000 wtpsplit-1.2.3/wtpsplit.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-07-18 13:44:07.000000 wtpsplit-1.2.3/wtpsplit.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      103 2023-07-18 13:44:07.000000 wtpsplit-1.2.3/wtpsplit.egg-info/requires.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-07-18 13:44:07.000000 wtpsplit-1.2.3/wtpsplit.egg-info/top_level.txt
```

### Comparing `wtpsplit-1.2.2/LICENSE` & `wtpsplit-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.2/README.md` & `wtpsplit-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.2/setup.py` & `wtpsplit-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="wtpsplit",
-    version="1.2.2",
+    version="1.2.3",
     packages=["wtpsplit"],
     description="Robust, adaptible sentence segmentation for 85 languages",
     author="Benjamin Minixhofer",
     author_email="bminixhofer@gmail.com",
     install_requires=[
         "onnxruntime>=1.13.1",
         "transformers>=4.22.2",
```

### Comparing `wtpsplit-1.2.2/wtpsplit/__init__.py` & `wtpsplit-1.2.3/wtpsplit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import skops.io as sio
 from transformers import AutoConfig, AutoModelForTokenClassification
 from transformers.utils.hub import cached_file
 
 from wtpsplit.extract import ORTWrapper, PyTorchWrapper, extract
 from wtpsplit.utils import Constants, indices_to_sentences, sigmoid
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 
 
 class WtP:
     def __init__(
         self,
         model_name_or_model,
         from_pretrained_kwargs=None,
```

### Comparing `wtpsplit-1.2.2/wtpsplit/configs.py` & `wtpsplit-1.2.3/wtpsplit/configs.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.2/wtpsplit/data/language_info.csv` & `wtpsplit-1.2.3/wtpsplit/data/language_info.csv`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.2/wtpsplit/data/punctuation.json` & `wtpsplit-1.2.3/wtpsplit/data/punctuation.json`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.2/wtpsplit/extract.py` & `wtpsplit-1.2.3/wtpsplit/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,18 @@
     pad_last_batch=False,
     verbose=False,
 ):
     text_lengths = [len(text) for text in batch_of_texts]
     # reduce block size if possible
     block_size = min(block_size, max(text_lengths))
 
+    # make sure block_size is a multiple of downsampling rate
+    downsampling_rate = getattr(model.config, "downsampling_rate", 1)
+    block_size = math.ceil(block_size / downsampling_rate) * downsampling_rate
+
     num_chunks = sum(math.ceil(max(length - block_size, 0) / stride) + 1 for length in text_lengths)
     input_hashes = np.zeros((num_chunks, block_size, model.config.num_hash_functions), dtype=np.int64)
     attention_mask = np.zeros((num_chunks, block_size), dtype=np.float16)
     locs = np.zeros((num_chunks, 3), dtype=np.int32)
 
     codec = "utf-32-le" if sys.byteorder == "little" else "utf-32-be"
     ordinals = np.frombuffer(bytearray("".join(batch_of_texts), encoding=codec), dtype=np.int32)
```

### Comparing `wtpsplit-1.2.2/wtpsplit/models.py` & `wtpsplit-1.2.3/wtpsplit/models.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.2.2/wtpsplit/utils.py` & `wtpsplit-1.2.3/wtpsplit/utils.py`

 * *Files identical despite different names*

