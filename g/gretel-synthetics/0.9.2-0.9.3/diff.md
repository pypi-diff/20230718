# Comparing `tmp/gretel-synthetics-0.9.2.tar.gz` & `tmp/gretel-synthetics-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gretel-synthetics-0.9.2.tar", last modified: Tue May 26 15:10:27 2020, max compression
+gzip compressed data, was "dist/gretel-synthetics-0.9.3.tar", last modified: Wed Jun  3 21:53:53 2020, max compression
```

## Comparing `gretel-synthetics-0.9.2.tar` & `gretel-synthetics-0.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-26 15:10:27.000000 gretel-synthetics-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (116)     3050 2020-05-26 15:10:27.000000 gretel-synthetics-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2419 2020-05-26 15:10:19.000000 gretel-synthetics-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      108 2020-05-26 15:10:27.000000 gretel-synthetics-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      882 2020-05-26 15:10:19.000000 gretel-synthetics-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-26 15:10:27.000000 gretel-synthetics-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-26 15:10:27.000000 gretel-synthetics-0.9.2/src/gretel_synthetics/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-26 15:10:19.000000 gretel-synthetics-0.9.2/src/gretel_synthetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4514 2020-05-26 15:10:19.000000 gretel-synthetics-0.9.2/src/gretel_synthetics/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     7826 2020-05-26 15:10:19.000000 gretel-synthetics-0.9.2/src/gretel_synthetics/generate.py
--rw-r--r--   0 runner    (1001) docker     (116)     3001 2020-05-26 15:10:19.000000 gretel-synthetics-0.9.2/src/gretel_synthetics/model.py
--rw-r--r--   0 runner    (1001) docker     (116)     7911 2020-05-26 15:10:19.000000 gretel-synthetics-0.9.2/src/gretel_synthetics/train.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-26 15:10:27.000000 gretel-synthetics-0.9.2/src/gretel_synthetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3050 2020-05-26 15:10:26.000000 gretel-synthetics-0.9.2/src/gretel_synthetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      414 2020-05-26 15:10:27.000000 gretel-synthetics-0.9.2/src/gretel_synthetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-26 15:10:26.000000 gretel-synthetics-0.9.2/src/gretel_synthetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      153 2020-05-26 15:10:26.000000 gretel-synthetics-0.9.2/src/gretel_synthetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2020-05-26 15:10:26.000000 gretel-synthetics-0.9.2/src/gretel_synthetics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (116)     3050 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2419 2020-06-03 21:53:39.000000 gretel-synthetics-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      108 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      882 2020-06-03 21:53:39.000000 gretel-synthetics-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/src/gretel_synthetics/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-03 21:53:39.000000 gretel-synthetics-0.9.3/src/gretel_synthetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4543 2020-06-03 21:53:39.000000 gretel-synthetics-0.9.3/src/gretel_synthetics/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7826 2020-06-03 21:53:39.000000 gretel-synthetics-0.9.3/src/gretel_synthetics/generate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3001 2020-06-03 21:53:39.000000 gretel-synthetics-0.9.3/src/gretel_synthetics/model.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8285 2020-06-03 21:53:39.000000 gretel-synthetics-0.9.3/src/gretel_synthetics/train.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/src/gretel_synthetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3050 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/src/gretel_synthetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/src/gretel_synthetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/src/gretel_synthetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      153 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/src/gretel_synthetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2020-06-03 21:53:53.000000 gretel-synthetics-0.9.3/src/gretel_synthetics.egg-info/top_level.txt
```

### Comparing `gretel-synthetics-0.9.2/PKG-INFO` & `gretel-synthetics-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-synthetics
-Version: 0.9.2
+Version: 0.9.3
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Gretel Synthetics
         
         ![gretel-synthetics workflows](https://github.com/gretelai/gretel-synthetics/workflows/gretel-synthetics%20workflows/badge.svg)
```

### Comparing `gretel-synthetics-0.9.2/README.md` & `gretel-synthetics-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `gretel-synthetics-0.9.2/setup.py` & `gretel-synthetics-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     description='Synthetic Data Generation with optional Differential Privacy',
     long_description=long_description,
     long_description_content_type='text/markdown',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     install_requires=[
         'tensorflow_privacy==0.2.2',
-        'sentencepiece==0.1.85',
+        'sentencepiece==0.1.91',
         'smart_open==1.10.0',
         'tqdm<5.0',
         'pandas==1.0.3',
         'numpy==1.18.3'
     ],
     extras_require={
         'tf': ['tensorflow==2.1.0'],
```

### Comparing `gretel-synthetics-0.9.2/src/gretel_synthetics/config.py` & `gretel-synthetics-0.9.3/src/gretel_synthetics/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     batch_size: int = 64
     buffer_size: int = 10000
     seq_length: int = 100
     embedding_dim: int = 256
     rnn_units: int = 256
     dropout_rate: float = 0.2
     rnn_initializer: str = "glorot_uniform"
+    max_line_len: int = 2048
 
     # Input data configs
     field_delimiter: Optional[str] = None
     field_delimiter_token: str = "<d>"
 
     # Tokenizer settings
     vocab_size: int = 500
```

### Comparing `gretel-synthetics-0.9.2/src/gretel_synthetics/generate.py` & `gretel-synthetics-0.9.3/src/gretel_synthetics/generate.py`

 * *Files identical despite different names*

### Comparing `gretel-synthetics-0.9.2/src/gretel_synthetics/model.py` & `gretel-synthetics-0.9.3/src/gretel_synthetics/model.py`

 * *Files identical despite different names*

### Comparing `gretel-synthetics-0.9.2/src/gretel_synthetics/train.py` & `gretel-synthetics-0.9.3/src/gretel_synthetics/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,20 +155,31 @@
 
 def _train_tokenizer(store: _BaseConfig) -> spm.SentencePieceProcessor:
     """
     Trains SentencePiece tokenizer on training data
     """
     logging.info("Training SentencePiece tokenizer")
     spm.SentencePieceTrainer.Train(
+        input=store.training_data,
+        model_prefix=store.tokenizer_prefix,
+        user_defined_symbols=["<n>", store.field_delimiter_token],
+        vocab_size=store.vocab_size,
+        hard_vocab_limit=False,
+        max_sentence_length=store.max_line_len,
+        character_coverage=store.character_coverage
+    )
+    """
+    spm.SentencePieceTrainer.Train(
         f'--input={store.training_data} '
         f'--model_prefix={store.tokenizer_prefix} '
         f'--user_defined_symbols=<n>,{store.field_delimiter_token} '
         f'--vocab_size={store.vocab_size} '
         f'--hard_vocab_limit=false '
         f'--character_coverage={store.character_coverage}')
+    """
     _move_tokenizer_model(store)
 
     sp = spm.SentencePieceProcessor()
     logging.info(f"Loading tokenizer from: {Path(store.tokenizer_model).name}")
     sp.Load(store.tokenizer_model)
 
     # print sample output
```

### Comparing `gretel-synthetics-0.9.2/src/gretel_synthetics.egg-info/PKG-INFO` & `gretel-synthetics-0.9.3/src/gretel_synthetics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-synthetics
-Version: 0.9.2
+Version: 0.9.3
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Gretel Synthetics
         
         ![gretel-synthetics workflows](https://github.com/gretelai/gretel-synthetics/workflows/gretel-synthetics%20workflows/badge.svg)
```

