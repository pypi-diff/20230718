# Comparing `tmp/BERTSimilar-0.1.4.tar.gz` & `tmp/BERTSimilar-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BERTSimilar-0.1.4.tar", last modified: Tue Jul 18 17:49:20 2023, max compression
+gzip compressed data, was "BERTSimilar-0.1.5.tar", last modified: Tue Jul 18 18:23:04 2023, max compression
```

## Comparing `BERTSimilar-0.1.4.tar` & `BERTSimilar-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:49:20.455296 BERTSimilar-0.1.4/
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:49:20.454002 BERTSimilar-0.1.4/BERTSimilar/
--rw-r--r--   0 rdp        (501) staff       (20)    25483 2023-07-18 17:48:46.000000 BERTSimilar-0.1.4/BERTSimilar/BERTSimilar.py
--rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.4/BERTSimilar/__init__.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:49:20.454804 BERTSimilar-0.1.4/BERTSimilar.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      255 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      147 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.4/LICENSE.txt
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 17:49:20.455030 BERTSimilar-0.1.4/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.4/README.md
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 17:49:20.455347 BERTSimilar-0.1.4/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-18 17:48:03.000000 BERTSimilar-0.1.4/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 18:23:04.691688 BERTSimilar-0.1.5/
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 18:23:04.690529 BERTSimilar-0.1.5/BERTSimilar/
+-rw-r--r--   0 rdp        (501) staff       (20)    25740 2023-07-18 18:21:52.000000 BERTSimilar-0.1.5/BERTSimilar/BERTSimilar.py
+-rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.5/BERTSimilar/__init__.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 18:23:04.691292 BERTSimilar-0.1.5/BERTSimilar.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 18:23:04.000000 BERTSimilar-0.1.5/BERTSimilar.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      255 2023-07-18 18:23:04.000000 BERTSimilar-0.1.5/BERTSimilar.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 18:23:04.000000 BERTSimilar-0.1.5/BERTSimilar.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      161 2023-07-18 18:23:04.000000 BERTSimilar-0.1.5/BERTSimilar.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-18 18:23:04.000000 BERTSimilar-0.1.5/BERTSimilar.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.5/LICENSE.txt
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 18:23:04.691502 BERTSimilar-0.1.5/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.5/README.md
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 18:23:04.691739 BERTSimilar-0.1.5/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-18 18:22:53.000000 BERTSimilar-0.1.5/setup.py
```

### Comparing `BERTSimilar-0.1.4/BERTSimilar/BERTSimilar.py` & `BERTSimilar-0.1.5/BERTSimilar/BERTSimilar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 from transformers import AutoModel, AutoTokenizer, logging
 import numpy as np
+import pandas as pd
 import warnings
 import docx
 import re
 import nltk
 import wikipedia
 import itertools
 from nltk.corpus import stopwords
@@ -34,14 +35,15 @@
     def __init__(self, model='bert-base-cased', max_heading_length = 10, max_document_length = 300, exclude_stopwords=[], embeddings_scaler=None):
 
         for i in tqdmn(range(2), unit=' it', desc='Initializing', postfix='Tokenizer and Model'): pass
         self.tokenizer = AutoTokenizer.from_pretrained(model)
         self.lemmatizer = WordNetLemmatizer()
         self.min_max_scaler = MinMaxScaler()
         self.scaler = embeddings_scaler
+        self.scaler_col_names = [str(i) for i in range(768)]
         self.model = AutoModel.from_pretrained(model)
         if torch.cuda.is_available():
             self.processor = 'GPU'
             self.cuda_current_device = torch.cuda.current_device()
             self.model = self.model.to(self.cuda_current_device)
         else:
             self.processor = 'CPU'
@@ -130,17 +132,21 @@
         self.bert_vectors_ngram[0] = self.bert_vectors
         self.bert_documents_ngram[0] = self.bert_documents
         self.cv_counts = self.count_vectorizer.fit_transform(self.count_vectorizer_words)
         self.cv_words = self.count_vectorizer.get_feature_names_out()
         self.bert_words_all = np.array(list(itertools.chain.from_iterable(self.bert_words_ngram)))
         self.bert_vectors_all = np.array(list(itertools.chain.from_iterable(self.bert_vectors_ngram)))
         if self.scaler is not None:
-            self.bert_vectors_all = self.scaler.transform(self.bert_vectors_all)
+            df = pd.DataFrame(self.bert_vectors_all, columns=self.scaler_col_names)
+            self.bert_vectors_all = self.scaler.transform(df)
+            del df
             for i in range(self.max_ngram):
-                self.bert_vectors_ngram[i] = self.scaler.transform(self.bert_vectors_ngram[i])
+                df = pd.DataFrame(self.bert_vectors_ngram[i], columns=self.scaler_col_names)
+                self.bert_vectors_ngram[i] = self.scaler.transform(df)
+                del df
         else:
             for i in range(self.max_ngram):
                 self.bert_vectors_ngram[i] = np.array(self.bert_vectors_ngram[i])
         return self
 
     def _process_wikipedia_dataset(self, page_content):
```

### Comparing `BERTSimilar-0.1.4/BERTSimilar.egg-info/PKG-INFO` & `BERTSimilar-0.1.5/BERTSimilar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.4
+Version: 0.1.5
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.4/LICENSE.txt` & `BERTSimilar-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.4/PKG-INFO` & `BERTSimilar-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.4
+Version: 0.1.5
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.4/README.md` & `BERTSimilar-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.4/setup.py` & `BERTSimilar-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='BERTSimilar',
-    version='0.1.4',
+    version='0.1.5',
     description="Get Similar Words and Embeddings using BERT Models",
     keywords="BERT NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

