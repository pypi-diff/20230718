# Comparing `tmp/socscikit-0.0.5.8.tar.gz` & `tmp/socscikit-0.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.5.8.tar", last modified: Tue Jul 18 00:17:58 2023, max compression
+gzip compressed data, was "socscikit-0.0.5.9.tar", last modified: Tue Jul 18 00:26:19 2023, max compression
```

## Comparing `socscikit-0.0.5.8.tar` & `socscikit-0.0.5.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.773663 socscikit-0.0.5.8/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.8/LICENSE.txt
--rw-rw-rw-   0        0        0      354 2023-07-18 00:17:48.000000 socscikit-0.0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-18 00:17:58.773663 socscikit-0.0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.8/README.md
--rw-rw-rw-   0        0        0       86 2023-07-18 00:17:58.774666 socscikit-0.0.5.8/setup.cfg
--rw-rw-rw-   0        0        0      781 2023-07-18 00:17:18.000000 socscikit-0.0.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.662498 socscikit-0.0.5.8/socscikit/
--rw-rw-rw-   0        0        0     1629 2023-07-17 21:58:34.000000 socscikit-0.0.5.8/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.8/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.697252 socscikit-0.0.5.8/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.703482 socscikit-0.0.5.8/socscikit/lexicon_dictionary/AFINN/
--rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle
-drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.711847 socscikit-0.0.5.8/socscikit/lexicon_dictionary/Aigents/
--rw-rw-rw-   0        0        0   247057 2023-07-16 06:38:52.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.753489 socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.772607 socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/VADER.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0     2977 2023-07-18 00:10:22.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/emos.py
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.8/socscikit/socialmedia.py
--rw-rw-rw-   0        0        0      139 2023-07-17 22:12:07.000000 socscikit-0.0.5.8/socscikit/test.py
--rw-rw-rw-   0        0        0     8723 2023-07-18 00:15:19.000000 socscikit-0.0.5.8/socscikit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.696249 socscikit-0.0.5.8/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 00:26:19.781421 socscikit-0.0.5.9/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      354 2023-07-18 00:17:48.000000 socscikit-0.0.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-07-18 00:26:19.781421 socscikit-0.0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.9/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-18 00:26:19.782421 socscikit-0.0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      781 2023-07-18 00:26:04.000000 socscikit-0.0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 00:26:19.749424 socscikit-0.0.5.9/socscikit/
+-rw-rw-rw-   0        0        0     1629 2023-07-17 21:58:34.000000 socscikit-0.0.5.9/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.9/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 00:26:19.767422 socscikit-0.0.5.9/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-18 00:26:19.768422 socscikit-0.0.5.9/socscikit/lexicon_dictionary/AFINN/
+-rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 socscikit-0.0.5.9/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle
+drwxrwxrwx   0        0        0        0 2023-07-18 00:26:19.769421 socscikit-0.0.5.9/socscikit/lexicon_dictionary/Aigents/
+-rw-rw-rw-   0        0        0   247057 2023-07-16 06:38:52.000000 socscikit-0.0.5.9/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-18 00:26:19.778421 socscikit-0.0.5.9/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.9/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.9/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-18 00:26:19.780421 socscikit-0.0.5.9/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.9/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.9/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0     2977 2023-07-18 00:10:22.000000 socscikit-0.0.5.9/socscikit/lexicon_dictionary/emos.py
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.9/socscikit/socialmedia.py
+-rw-rw-rw-   0        0        0      122 2023-07-18 00:22:52.000000 socscikit-0.0.5.9/socscikit/test.py
+-rw-rw-rw-   0        0        0     8284 2023-07-18 00:25:33.000000 socscikit-0.0.5.9/socscikit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 00:26:19.766422 socscikit-0.0.5.9/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-18 00:26:19.000000 socscikit-0.0.5.9/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-18 00:26:19.000000 socscikit-0.0.5.9/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 00:26:19.000000 socscikit-0.0.5.9/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-18 00:26:19.000000 socscikit-0.0.5.9/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 00:26:19.000000 socscikit-0.0.5.9/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.5.8/LICENSE.txt` & `socscikit-0.0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/setup.py` & `socscikit-0.0.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   
-  version = '0.0.5.8',      
+  version = '0.0.5.9',      
   license='Apache-2.0',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   #
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/nick-sh-oh/socscikit',  
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.8.tar.gz', 
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.9.tar.gz', 
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            
           'tweepy',
           'plotly',
           'conlp',
           'spacy',
           'spacymoji'
```

### Comparing `socscikit-0.0.5.8/socscikit/CompliSent.py` & `socscikit-0.0.5.9/socscikit/CompliSent.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle` & `socscikit-0.0.5.9/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle` & `socscikit-0.0.5.9/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.5.9/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.5.9/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/VADER.csv` & `socscikit-0.0.5.9/socscikit/lexicon_dictionary/VADER/VADER.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle` & `socscikit-0.0.5.9/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/socscikit/lexicon_dictionary/emos.py` & `socscikit-0.0.5.9/socscikit/lexicon_dictionary/emos.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/socscikit/socialmedia.py` & `socscikit-0.0.5.9/socscikit/socialmedia.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.8/socscikit/utils.py` & `socscikit-0.0.5.9/socscikit/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,21 +10,14 @@
 from lexicon_dictionary import emos
 
 
 class CS:
     def __init__(self):
         self.spacy_nlp = spacy.load("en_core_web_sm").add_pipe("emoji", first=True)
 
-    def extract_emoticons(text):
-        emoticon_pattern = re.compile(
-            r"(?::|;|=)(?:-)?(?:\)|D|P|O|S|\(|\||\\|\/|\[|\]|x|X|<|>|\'|\"|@|3|8|\$|_|{|}|;|\\|\*|,|\.|!|0|_|<|3|>|\^|¯|–|`|\*)[.,!?\'\"]*|[.,!?\'\"]*(?:\)|D|P|O|S|\(|\||\\|\/|\[|\]|x|X|<|>|\'|\"|@|3|8|\$|_|{|}|;|\\|\*|,|\.|!|0|_|<|3|>|\^|¯|–|`|\*)(?:-)?(?::|;|=)"
-        )
-        emoticons = re.findall(emoticon_pattern, text)
-        return emoticons
-
     def count_categorical_labels(self, dictionary):
         label_counts = Counter()
         multi_label_counts = Counter()
 
         for sublist in track(
             dictionary.values(),
             description="Computing Summary Statistics of Sentiment Scores",
@@ -187,18 +180,18 @@
             description="Extracting Summary Insights from Sentiment Lexicons",
             transient=True,
         ):
             # check if token is emoticons
             if key in emos.emoticons:
                 pos_tags.append("EMOTICON")
             else:
-                with self.spacy_nlp.select_pipes(
-                    disable=["parser", "senter", "attribute_ruler", "lemmatizer", "ner"]
-                ):
-                    doc = self.spacy_nlp(key)
+                # with self.spacy_nlp.select_pipes(
+                #     disable=["parser", "senter", "attribute_ruler", "lemmatizer", "ner"]
+                # ):
+                doc = self.spacy_nlp(key)
                 for token in doc:
                     # check if token is emoji
                     if token._.is_emoji:
                         pos_tags.append("EMOJI")
                     else:
                         pos_tags.append(token.tag_)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `socscikit-0.0.5.8/socscikit.egg-info/SOURCES.txt` & `socscikit-0.0.5.9/socscikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

