# Comparing `tmp/BERTSimilar-0.1.7.tar.gz` & `tmp/BERTSimilar-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BERTSimilar-0.1.7.tar", last modified: Tue Jul 18 18:54:36 2023, max compression
+gzip compressed data, was "BERTSimilar-0.1.8.tar", last modified: Tue Jul 18 19:01:26 2023, max compression
```

## Comparing `BERTSimilar-0.1.7.tar` & `BERTSimilar-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 18:54:36.404143 BERTSimilar-0.1.7/
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 18:54:36.402949 BERTSimilar-0.1.7/BERTSimilar/
--rw-r--r--   0 rdp        (501) staff       (20)    25845 2023-07-18 18:53:37.000000 BERTSimilar-0.1.7/BERTSimilar/BERTSimilar.py
--rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.7/BERTSimilar/__init__.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 18:54:36.403723 BERTSimilar-0.1.7/BERTSimilar.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 18:54:36.000000 BERTSimilar-0.1.7/BERTSimilar.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      255 2023-07-18 18:54:36.000000 BERTSimilar-0.1.7/BERTSimilar.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 18:54:36.000000 BERTSimilar-0.1.7/BERTSimilar.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      161 2023-07-18 18:54:36.000000 BERTSimilar-0.1.7/BERTSimilar.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-18 18:54:36.000000 BERTSimilar-0.1.7/BERTSimilar.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.7/LICENSE.txt
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 18:54:36.403951 BERTSimilar-0.1.7/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.7/README.md
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 18:54:36.404199 BERTSimilar-0.1.7/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-18 18:54:30.000000 BERTSimilar-0.1.7/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 19:01:26.396838 BERTSimilar-0.1.8/
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 19:01:26.395609 BERTSimilar-0.1.8/BERTSimilar/
+-rw-r--r--   0 rdp        (501) staff       (20)    25880 2023-07-18 19:01:01.000000 BERTSimilar-0.1.8/BERTSimilar/BERTSimilar.py
+-rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.8/BERTSimilar/__init__.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 19:01:26.396391 BERTSimilar-0.1.8/BERTSimilar.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      255 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      161 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-18 19:01:26.000000 BERTSimilar-0.1.8/BERTSimilar.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.8/LICENSE.txt
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 19:01:26.396625 BERTSimilar-0.1.8/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.8/README.md
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 19:01:26.396891 BERTSimilar-0.1.8/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-18 19:01:18.000000 BERTSimilar-0.1.8/setup.py
```

### Comparing `BERTSimilar-0.1.7/BERTSimilar/BERTSimilar.py` & `BERTSimilar-0.1.8/BERTSimilar/BERTSimilar.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,20 +135,20 @@
         self.cv_words = self.count_vectorizer.get_feature_names_out()
         self.bert_words_all = np.array(list(itertools.chain.from_iterable(self.bert_words_ngram)))
         self.bert_vectors_all = np.array(list(itertools.chain.from_iterable(self.bert_vectors_ngram)))
         if self.scaler is not None:
             df = pd.DataFrame(self.bert_vectors_all, columns=self.scaler_col_names)
             self.bert_vectors_all = self.scaler.transform(df)
             del df
-            for i in tqdmn(range(self.max_ngram), desc='Creating', postfix='N-gram Words'):
+            for i in tqdmn(range(self.max_ngram), desc='Creating', postfix='N-gram Words and Embeddings'):
                 df = pd.DataFrame(self.bert_vectors_ngram[i], columns=self.scaler_col_names)
                 self.bert_vectors_ngram[i] = self.scaler.transform(df)
                 del df
         else:
-            for i in tqdmn(range(self.max_ngram), desc='Creating', postfix='N-gram Words'):
+            for i in tqdmn(range(self.max_ngram), desc='Creating', postfix='N-gram Words and Embeddings'):
                 self.bert_vectors_ngram[i] = np.array(self.bert_vectors_ngram[i])
         return self
 
     def _process_wikipedia_dataset(self, page_content):
 
         document_list = []
         for section in page_content:
@@ -472,15 +472,15 @@
 
         single_word_split : whether to split n-gram words when given as input (boolean) (optional) (default: True)
 
         uncased_lemmatization : whether to uncase and lemmatize the input (boolean) (optional) (default: True)
 
         """
 
-        if input_embedding == 0:
+        if input_embedding.size == 0:
 
             input_context_split, input_words_split, input_words_max, input_context_words, input_context_words_max = self._process_input_context_words(
                 input_context, input_words, single_word_split, uncased_lemmatization)
 
             similar_documents, similarity_scores, similarity_factor = self._context_similarity_document_scores(
                 input_context_words, len(input_context_split), len(input_words_split), context_similarity_factor)
```

### Comparing `BERTSimilar-0.1.7/BERTSimilar.egg-info/PKG-INFO` & `BERTSimilar-0.1.8/BERTSimilar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.7
+Version: 0.1.8
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.7/LICENSE.txt` & `BERTSimilar-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.7/PKG-INFO` & `BERTSimilar-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.7
+Version: 0.1.8
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.7/README.md` & `BERTSimilar-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.7/setup.py` & `BERTSimilar-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='BERTSimilar',
-    version='0.1.7',
+    version='0.1.8',
     description="Get Similar Words and Embeddings using BERT Models",
     keywords="BERT NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

