# Comparing `tmp/socscikit-0.0.5.7.tar.gz` & `tmp/socscikit-0.0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.5.7.tar", last modified: Mon Jul 17 22:10:09 2023, max compression
+gzip compressed data, was "socscikit-0.0.5.8.tar", last modified: Tue Jul 18 00:17:58 2023, max compression
```

## Comparing `socscikit-0.0.5.7.tar` & `socscikit-0.0.5.8.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.276915 socscikit-0.0.5.7/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.7/LICENSE.txt
--rw-rw-rw-   0        0        0      308 2023-07-16 06:56:47.000000 socscikit-0.0.5.7/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-17 22:10:09.276915 socscikit-0.0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.7/README.md
--rw-rw-rw-   0        0        0       86 2023-07-17 22:10:09.277953 socscikit-0.0.5.7/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-07-17 22:09:55.000000 socscikit-0.0.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.206246 socscikit-0.0.5.7/socscikit/
--rw-rw-rw-   0        0        0     1629 2023-07-17 21:58:34.000000 socscikit-0.0.5.7/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.7/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.191190 socscikit-0.0.5.7/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.228323 socscikit-0.0.5.7/socscikit/lexicon_dictionary/AFINN/
--rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle
-drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.233342 socscikit-0.0.5.7/socscikit/lexicon_dictionary/Aigents/
--rw-rw-rw-   0        0        0   247057 2023-07-16 06:38:52.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.261921 socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.275922 socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/VADER.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.7/socscikit/socialmedia.py
--rw-rw-rw-   0        0        0      136 2023-07-15 23:01:18.000000 socscikit-0.0.5.7/socscikit/test.py
--rw-rw-rw-   0        0        0     8441 2023-07-17 22:09:16.000000 socscikit-0.0.5.7/socscikit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.223429 socscikit-0.0.5.7/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-17 22:10:08.000000 socscikit-0.0.5.7/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      649 2023-07-17 22:10:09.000000 socscikit-0.0.5.7/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 22:10:08.000000 socscikit-0.0.5.7/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-17 22:10:08.000000 socscikit-0.0.5.7/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-17 22:10:08.000000 socscikit-0.0.5.7/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.773663 socscikit-0.0.5.8/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      354 2023-07-18 00:17:48.000000 socscikit-0.0.5.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-07-18 00:17:58.773663 socscikit-0.0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.8/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-18 00:17:58.774666 socscikit-0.0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      781 2023-07-18 00:17:18.000000 socscikit-0.0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.662498 socscikit-0.0.5.8/socscikit/
+-rw-rw-rw-   0        0        0     1629 2023-07-17 21:58:34.000000 socscikit-0.0.5.8/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.8/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.697252 socscikit-0.0.5.8/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.703482 socscikit-0.0.5.8/socscikit/lexicon_dictionary/AFINN/
+-rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle
+drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.711847 socscikit-0.0.5.8/socscikit/lexicon_dictionary/Aigents/
+-rw-rw-rw-   0        0        0   247057 2023-07-16 06:38:52.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.753489 socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.772607 socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0     2977 2023-07-18 00:10:22.000000 socscikit-0.0.5.8/socscikit/lexicon_dictionary/emos.py
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.8/socscikit/socialmedia.py
+-rw-rw-rw-   0        0        0      139 2023-07-17 22:12:07.000000 socscikit-0.0.5.8/socscikit/test.py
+-rw-rw-rw-   0        0        0     8723 2023-07-18 00:15:19.000000 socscikit-0.0.5.8/socscikit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 00:17:58.696249 socscikit-0.0.5.8/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 00:17:58.000000 socscikit-0.0.5.8/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.5.7/LICENSE.txt` & `socscikit-0.0.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.7/setup.py` & `socscikit-0.0.5.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   
-  version = '0.0.5.7',      
+  version = '0.0.5.8',      
   license='Apache-2.0',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   #
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/nick-sh-oh/socscikit',  
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.7.tar.gz', 
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.8.tar.gz', 
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            
           'tweepy',
           'plotly',
           'conlp',
-          'spacy'
+          'spacy',
+          'spacymoji'
       ],
   include_package_data=True
 )
```

### Comparing `socscikit-0.0.5.7/socscikit/CompliSent.py` & `socscikit-0.0.5.8/socscikit/CompliSent.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.7/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle` & `socscikit-0.0.5.8/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.7/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle` & `socscikit-0.0.5.8/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.5.8/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/VADER.csv` & `socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/VADER.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle` & `socscikit-0.0.5.8/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.7/socscikit/socialmedia.py` & `socscikit-0.0.5.8/socscikit/socialmedia.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.7/socscikit/utils.py` & `socscikit-0.0.5.8/socscikit/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 from rich import print as pprint
 import itertools
 from itertools import combinations, chain
 import statistics
 from collections import Counter
 import spacy
 from spacymoji import Emoji
-import re 
+import re
+from lexicon_dictionary import emos
 
 
 class CS:
     def __init__(self):
-        self.spacy_nlp = spacy.load(
-            "en_core_web_sm"
-        ).add_pipe("emoji", first=True)
+        self.spacy_nlp = spacy.load("en_core_web_sm").add_pipe("emoji", first=True)
 
     def extract_emoticons(text):
-        emoticon_pattern = re.compile(r'(?::|;|=)(?:-)?(?:\)|D|P|O|S|\(|\||\\|\/|\[|\]|x|X|<|>|\'|\"|@|3|8|\$|_|{|}|;|\\|\*|,|\.|!|0|_|<|3|>|\^|¯|–|`|\*)[.,!?\'\"]*|[.,!?\'\"]*(?:\)|D|P|O|S|\(|\||\\|\/|\[|\]|x|X|<|>|\'|\"|@|3|8|\$|_|{|}|;|\\|\*|,|\.|!|0|_|<|3|>|\^|¯|–|`|\*)(?:-)?(?::|;|=)')
+        emoticon_pattern = re.compile(
+            r"(?::|;|=)(?:-)?(?:\)|D|P|O|S|\(|\||\\|\/|\[|\]|x|X|<|>|\'|\"|@|3|8|\$|_|{|}|;|\\|\*|,|\.|!|0|_|<|3|>|\^|¯|–|`|\*)[.,!?\'\"]*|[.,!?\'\"]*(?:\)|D|P|O|S|\(|\||\\|\/|\[|\]|x|X|<|>|\'|\"|@|3|8|\$|_|{|}|;|\\|\*|,|\.|!|0|_|<|3|>|\^|¯|–|`|\*)(?:-)?(?::|;|=)"
+        )
         emoticons = re.findall(emoticon_pattern, text)
         return emoticons
-    
+
     def count_categorical_labels(self, dictionary):
         label_counts = Counter()
         multi_label_counts = Counter()
 
         for sublist in track(
             dictionary.values(),
             description="Computing Summary Statistics of Sentiment Scores",
-            transient=True
+            transient=True,
         ):
             if isinstance(sublist, list):
                 if all(isinstance(item, str) for item in sublist):
                     labels = sublist
                     label_counts.update(labels)
 
                     combinations_set = set(
@@ -55,15 +56,15 @@
     def count_discrete_labels(self, dictionary):
         label_counts = {}
         multi_label_counts = {}
 
         for value_list in track(
             dictionary.values(),
             description="Computing Summary Statistics of Sentiment Scores",
-            transient=True
+            transient=True,
         ):
             unique_labels = set(value_list)
 
             for label in unique_labels:
                 if label in label_counts:
                     label_counts[label] += 1
                 else:
@@ -91,15 +92,15 @@
     def count_cont_variables(self, dictionary):
         value_range = [min(dictionary.values()), max(dictionary.values())]
         neg, pos, neu = [], [], []
 
         for value in track(
             dictionary.values(),
             description="Computing Summary Statistics of Sentiment Scores",
-            transient=True
+            transient=True,
         ):
             if value < 0:
                 neg.append(value)
             elif value > 0:
                 pos.append(value)
             else:
                 neu.append(value)
@@ -171,35 +172,39 @@
         pos_tags = []
         general_dict = {
             "verbs": 0,
             "adjectives": 0,
             "adverbs": 0,
             "prepositions": 0,
             "nouns": 0,
-            "emo": 0,
+            "emos": 0,
             "miscellaneous": 0,
         }
         granular_dict = {}
         misc = []
 
         for key in track(
             lexicon_dictionary.keys(),
             description="Extracting Summary Insights from Sentiment Lexicons",
-            transient=True
+            transient=True,
         ):
-            doc = self.spacy_nlp(key)
-            for token in doc:
-                #check if token is emoji 
-                if token._.is_emoji: 
-                    pos_tags.append("EMOJI")
-                #check if token is emoticon 
-                elif token.text in self.extract_emoticons(token.text):
-                    pos_tags.append("EMOTICON")
-                else: 
-                     pos_tags.append(token.tag_)
+            # check if token is emoticons
+            if key in emos.emoticons:
+                pos_tags.append("EMOTICON")
+            else:
+                with self.spacy_nlp.select_pipes(
+                    disable=["parser", "senter", "attribute_ruler", "lemmatizer", "ner"]
+                ):
+                    doc = self.spacy_nlp(key)
+                for token in doc:
+                    # check if token is emoji
+                    if token._.is_emoji:
+                        pos_tags.append("EMOJI")
+                    else:
+                        pos_tags.append(token.tag_)
 
         for element in pos_tags:
             if element in granular_dict:
                 granular_dict[element] += 1
             else:
                 granular_dict[element] = 1
 
@@ -210,16 +215,18 @@
                 general_dict["adjectives"] += value
             elif key.startswith("RB"):
                 general_dict["adverbs"] += value
             elif key.startswith("IN"):
                 general_dict["prepositions"] += value
             elif key.startswith("N"):
                 general_dict["nouns"] += value
-            elif key.startswith("EMO"):
-                general_dict["emos"] += value 
+            elif key == "EMOTICON":
+                general_dict["emos"] += value
+            elif key == "EMOJI":
+                general_dict["emos"] += value
             else:
                 misc.append(key)
                 general_dict["miscellaneous"] += value
 
         part_of_speech = {
             "general": self.sort_dict(general_dict),
             "granular": self.sort_dict(granular_dict),
```

### Comparing `socscikit-0.0.5.7/socscikit.egg-info/SOURCES.txt` & `socscikit-0.0.5.8/socscikit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 socscikit/test.py
 socscikit/utils.py
 socscikit.egg-info/PKG-INFO
 socscikit.egg-info/SOURCES.txt
 socscikit.egg-info/dependency_links.txt
 socscikit.egg-info/requires.txt
 socscikit.egg-info/top_level.txt
+socscikit/lexicon_dictionary/emos.py
 socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle
 socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle
 socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
 socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
 socscikit/lexicon_dictionary/VADER/VADER.csv
 socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
```

