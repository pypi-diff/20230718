# Comparing `tmp/BERTSimilar-0.1.3.tar.gz` & `tmp/BERTSimilar-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BERTSimilar-0.1.3.tar", last modified: Thu Jul 13 01:04:31 2023, max compression
+gzip compressed data, was "BERTSimilar-0.1.4.tar", last modified: Tue Jul 18 17:49:20 2023, max compression
```

## Comparing `BERTSimilar-0.1.3.tar` & `BERTSimilar-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 01:04:31.909895 BERTSimilar-0.1.3/
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 01:04:31.908310 BERTSimilar-0.1.3/BERTSimilar/
--rw-r--r--   0 rdp        (501) staff       (20)    25460 2023-07-13 01:03:56.000000 BERTSimilar-0.1.3/BERTSimilar/BERTSimilar.py
--rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.3/BERTSimilar/__init__.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-13 01:04:31.909282 BERTSimilar-0.1.3/BERTSimilar.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-13 01:04:31.000000 BERTSimilar-0.1.3/BERTSimilar.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      255 2023-07-13 01:04:31.000000 BERTSimilar-0.1.3/BERTSimilar.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-13 01:04:31.000000 BERTSimilar-0.1.3/BERTSimilar.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      147 2023-07-13 01:04:31.000000 BERTSimilar-0.1.3/BERTSimilar.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-13 01:04:31.000000 BERTSimilar-0.1.3/BERTSimilar.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.3/LICENSE.txt
--rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-13 01:04:31.909514 BERTSimilar-0.1.3/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.3/README.md
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-13 01:04:31.909951 BERTSimilar-0.1.3/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-13 01:04:26.000000 BERTSimilar-0.1.3/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:49:20.455296 BERTSimilar-0.1.4/
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:49:20.454002 BERTSimilar-0.1.4/BERTSimilar/
+-rw-r--r--   0 rdp        (501) staff       (20)    25483 2023-07-18 17:48:46.000000 BERTSimilar-0.1.4/BERTSimilar/BERTSimilar.py
+-rw-r--r--   0 rdp        (501) staff       (20)       37 2023-07-13 00:23:07.000000 BERTSimilar-0.1.4/BERTSimilar/__init__.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:49:20.454804 BERTSimilar-0.1.4/BERTSimilar.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      255 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      147 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       12 2023-07-18 17:49:20.000000 BERTSimilar-0.1.4/BERTSimilar.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)     1069 2023-01-01 19:42:33.000000 BERTSimilar-0.1.4/LICENSE.txt
+-rw-r--r--   0 rdp        (501) staff       (20)    11447 2023-07-18 17:49:20.455030 BERTSimilar-0.1.4/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)    10923 2023-07-13 00:45:32.000000 BERTSimilar-0.1.4/README.md
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 17:49:20.455347 BERTSimilar-0.1.4/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      849 2023-07-18 17:48:03.000000 BERTSimilar-0.1.4/setup.py
```

### Comparing `BERTSimilar-0.1.3/BERTSimilar/BERTSimilar.py` & `BERTSimilar-0.1.4/BERTSimilar/BERTSimilar.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from nltk.tokenize import sent_tokenize
 from nltk.stem import WordNetLemmatizer
 from sklearn.metrics.pairwise import cosine_similarity
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.preprocessing import MinMaxScaler
 try:
   ipython = get_ipython()
-  from tqdm.notebook import tqdm
+  from tqdm.notebook import tqdm as tqdmn
 except:
-  from tqdm import tqdm
+  from tqdm import tqdm as tqdmn
 
 logging.set_verbosity_error()
 logging.disable_progress_bar()
 warnings.filterwarnings('ignore')
 nltk.download('stopwords', quiet=True)
 nltk.download('punkt', quiet=True)
 nltk.download('wordnet', quiet=True)
@@ -29,15 +29,15 @@
 nltk.download('tagsets', quiet=True)
 nltk.download('averaged_perceptron_tagger', quiet=True)
 
 class SimilarWords:
 
     def __init__(self, model='bert-base-cased', max_heading_length = 10, max_document_length = 300, exclude_stopwords=[], embeddings_scaler=None):
 
-        for i in tqdm(range(2), unit=' it', desc='Initializing', postfix='Tokenizer and Model'): pass
+        for i in tqdmn(range(2), unit=' it', desc='Initializing', postfix='Tokenizer and Model'): pass
         self.tokenizer = AutoTokenizer.from_pretrained(model)
         self.lemmatizer = WordNetLemmatizer()
         self.min_max_scaler = MinMaxScaler()
         self.scaler = embeddings_scaler
         self.model = AutoModel.from_pretrained(model)
         if torch.cuda.is_available():
             self.processor = 'GPU'
@@ -93,15 +93,15 @@
                 if type(wikipedia_query) == str:
                     wikipedia_query = [wikipedia_query]
                 for query in wikipedia_query:
                     query_results += wikipedia.search(query, results=wikipedia_query_limit)
             else:
                 query_results = wikipedia_page_list
             page_content = []
-            for result in tqdm(query_results, unit=' pages', desc='Extracting', postfix='Data from Wikipedia'):
+            for result in tqdmn(query_results, unit=' pages', desc='Extracting', postfix='Data from Wikipedia'):
                 if '(disambiguation)' not in result and result not in self.wikipedia_dataset_info.keys():
                     try:
                         page = wikipedia.page(result, auto_suggest=False)
                     except:
                         continue
                     page_content += ['== New page =='] + page.content.split('\n\n\n')
                     self.wikipedia_dataset_info[page.title] = page.url
@@ -164,15 +164,15 @@
                                                                                  sentence_length)
                             flag = 1
         return document_list
 
     def _process_docx_dataset(self, docx_content):
 
         document_list = []
-        for paragraph in tqdm(docx_content.paragraphs, unit=' paragraphs', desc='Extracting',
+        for paragraph in tqdmn(docx_content.paragraphs, unit=' paragraphs', desc='Extracting',
                               postfix='Data from Dataset'):
             if 'Heading' in str(paragraph.style):
                 text = re.sub(self.doc_regex, '', paragraph.text)
                 if len(document_list) != 0 and len(document_list[-1].split()) <= self.max_heading_length:
                     document_list[-1] = text + '.'
                 else:
                     document_list.append(text + '.')
@@ -187,15 +187,15 @@
                         document_list = self._process_dataset_long_paragraph(document_list, sentence, sentence_length)
         return document_list
 
     def _process_txt_dataset(self, path):
 
         document_list = []
         with open(path) as file:
-            for line in tqdm(file.readlines(), unit=' paragraphs', desc='Extracting', postfix='Data from Dataset'):
+            for line in tqdmn(file.readlines(), unit=' paragraphs', desc='Extracting', postfix='Data from Dataset'):
                 line_text = line.strip()
                 line_text = re.sub(self.doc_regex, '', line_text)
                 line_length = len(line_text.split())
                 if 0 < line_length <= self.max_heading_length:
                     if len(document_list) != 0 and len(document_list[-1].split()) <= self.max_heading_length:
                         document_list[-1] = line_text + '.'
                     else:
@@ -236,15 +236,15 @@
             document_list.append(sentence)
         return document_list
 
     def _tokenize_and_embeddings(self, document_list):
 
         continous_index = 0
         document_index = 0
-        for document in tqdm(document_list, unit=' documents', desc='Processing', postfix='Word Embeddings'):
+        for document in tqdmn(document_list, unit=' documents', desc='Processing', postfix='Word Embeddings'):
             if self.processor == 'GPU':
                 tokens = self.tokenizer(document, truncation=True, return_tensors='pt').to(self.cuda_current_device)
             else:
                 tokens = self.tokenizer(document, truncation=True, return_tensors='pt')
             words = self.tokenizer.convert_ids_to_tokens(tokens['input_ids'][0])
             word_ids = tokens.word_ids()
             output = self.model(**tokens)
```

### Comparing `BERTSimilar-0.1.3/BERTSimilar.egg-info/PKG-INFO` & `BERTSimilar-0.1.4/BERTSimilar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.3
+Version: 0.1.4
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.3/LICENSE.txt` & `BERTSimilar-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.3/PKG-INFO` & `BERTSimilar-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BERTSimilar
-Version: 0.1.3
+Version: 0.1.4
 Summary: Get Similar Words and Embeddings using BERT Models
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: BERT NLP
 Platform: UNKNOWN
```

### Comparing `BERTSimilar-0.1.3/README.md` & `BERTSimilar-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `BERTSimilar-0.1.3/setup.py` & `BERTSimilar-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='BERTSimilar',
-    version='0.1.3',
+    version='0.1.4',
     description="Get Similar Words and Embeddings using BERT Models",
     keywords="BERT NLP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

