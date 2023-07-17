# Comparing `tmp/socscikit-0.0.5.6.tar.gz` & `tmp/socscikit-0.0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socscikit-0.0.5.6.tar", last modified: Sun Jul 16 07:08:40 2023, max compression
+gzip compressed data, was "socscikit-0.0.5.7.tar", last modified: Mon Jul 17 22:10:09 2023, max compression
```

## Comparing `socscikit-0.0.5.6.tar` & `socscikit-0.0.5.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 07:08:40.834342 socscikit-0.0.5.6/
--rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.6/LICENSE.txt
--rw-rw-rw-   0        0        0      308 2023-07-16 06:56:47.000000 socscikit-0.0.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-16 07:08:40.834342 socscikit-0.0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.6/README.md
--rw-rw-rw-   0        0        0       86 2023-07-16 07:08:40.835307 socscikit-0.0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-07-16 07:08:23.000000 socscikit-0.0.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:08:40.803277 socscikit-0.0.5.6/socscikit/
--rw-rw-rw-   0        0        0     1548 2023-07-16 06:45:34.000000 socscikit-0.0.5.6/socscikit/CompliSent.py
--rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.6/socscikit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:08:40.791958 socscikit-0.0.5.6/socscikit/lexicon_dictionary/
-drwxrwxrwx   0        0        0        0 2023-07-16 07:08:40.820335 socscikit-0.0.5.6/socscikit/lexicon_dictionary/AFINN/
--rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 socscikit-0.0.5.6/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle
-drwxrwxrwx   0        0        0        0 2023-07-16 07:08:40.821275 socscikit-0.0.5.6/socscikit/lexicon_dictionary/Aigents/
--rw-rw-rw-   0        0        0   247057 2023-07-16 06:38:52.000000 socscikit-0.0.5.6/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-16 07:08:40.830275 socscikit-0.0.5.6/socscikit/lexicon_dictionary/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.6/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.6/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-16 07:08:40.833285 socscikit-0.0.5.6/socscikit/lexicon_dictionary/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.6/socscikit/lexicon_dictionary/VADER/VADER.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.6/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.6/socscikit/socialmedia.py
--rw-rw-rw-   0        0        0      136 2023-07-15 23:01:18.000000 socscikit-0.0.5.6/socscikit/test.py
--rw-rw-rw-   0        0        0     7570 2023-07-16 00:45:30.000000 socscikit-0.0.5.6/socscikit/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:08:40.819314 socscikit-0.0.5.6/socscikit.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-16 07:08:40.000000 socscikit-0.0.5.6/socscikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      649 2023-07-16 07:08:40.000000 socscikit-0.0.5.6/socscikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 07:08:40.000000 socscikit-0.0.5.6/socscikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-16 07:08:40.000000 socscikit-0.0.5.6/socscikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-16 07:08:40.000000 socscikit-0.0.5.6/socscikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.276915 socscikit-0.0.5.7/
+-rw-rw-rw-   0        0        0    11824 2023-04-24 07:09:30.000000 socscikit-0.0.5.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      308 2023-07-16 06:56:47.000000 socscikit-0.0.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-07-17 22:10:09.276915 socscikit-0.0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:09:42.000000 socscikit-0.0.5.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-17 22:10:09.277953 socscikit-0.0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-07-17 22:09:55.000000 socscikit-0.0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.206246 socscikit-0.0.5.7/socscikit/
+-rw-rw-rw-   0        0        0     1629 2023-07-17 21:58:34.000000 socscikit-0.0.5.7/socscikit/CompliSent.py
+-rw-rw-rw-   0        0        0       32 2023-07-13 23:55:12.000000 socscikit-0.0.5.7/socscikit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.191190 socscikit-0.0.5.7/socscikit/lexicon_dictionary/
+drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.228323 socscikit-0.0.5.7/socscikit/lexicon_dictionary/AFINN/
+-rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle
+drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.233342 socscikit-0.0.5.7/socscikit/lexicon_dictionary/Aigents/
+-rw-rw-rw-   0        0        0   247057 2023-07-16 06:38:52.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.261921 socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.275922 socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/VADER.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0    37805 2023-04-20 22:09:33.000000 socscikit-0.0.5.7/socscikit/socialmedia.py
+-rw-rw-rw-   0        0        0      136 2023-07-15 23:01:18.000000 socscikit-0.0.5.7/socscikit/test.py
+-rw-rw-rw-   0        0        0     8441 2023-07-17 22:09:16.000000 socscikit-0.0.5.7/socscikit/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 22:10:09.223429 socscikit-0.0.5.7/socscikit.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-17 22:10:08.000000 socscikit-0.0.5.7/socscikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      649 2023-07-17 22:10:09.000000 socscikit-0.0.5.7/socscikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 22:10:08.000000 socscikit-0.0.5.7/socscikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-17 22:10:08.000000 socscikit-0.0.5.7/socscikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-17 22:10:08.000000 socscikit-0.0.5.7/socscikit.egg-info/top_level.txt
```

### Comparing `socscikit-0.0.5.6/LICENSE.txt` & `socscikit-0.0.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.6/setup.py` & `socscikit-0.0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'socscikit',         # How you named your package folder (MyLib)
   packages = ['socscikit'],   
-  version = '0.0.5.6',      
+  version = '0.0.5.7',      
   license='Apache-2.0',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   #
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/nick-sh-oh/socscikit',  
-  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.6.tar.gz', 
+  download_url = 'https://github.com/nick-sh-oh/socscikit/archive/refs/tags/0.0.5.7.tar.gz', 
   keywords = ['AI', 'SOCIAL SCIENCE'],   # Keywords that define your package best
   install_requires=[            
           'tweepy',
           'plotly',
           'conlp',
           'spacy'
       ],
```

### Comparing `socscikit-0.0.5.6/socscikit/CompliSent.py` & `socscikit-0.0.5.7/socscikit/CompliSent.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,10 +27,13 @@
         elif idx == "Aigents+_v2022": 
             file_path = os.path.join(self.script_dir, 'lexicon_dictionary', 'Aigents', 'Aigents+_v2022.pickle')
             with open(file_path, 'rb') as handle: 
                 self.lex_dict = pickle.load(handle)
                 
         return self.lex_dict
     
-    def overview(self, dictionary:dict): 
+    def overview(self, dictionary:dict=None): 
         #dict:str = Consider if users simply come up with the lex_dict_idx
-        return CS().summarise_lex_dict(dictionary)
+        if dict is None: 
+            raise ValueError
+        else:
+            return CS().summarise_lex_dict(dictionary)
```

### Comparing `socscikit-0.0.5.6/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle` & `socscikit-0.0.5.7/socscikit/lexicon_dictionary/AFINN/AFINN_v2015.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.6/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle` & `socscikit-0.0.5.7/socscikit/lexicon_dictionary/Aigents/Aigents+_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.6/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv` & `socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.6/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle` & `socscikit-0.0.5.7/socscikit/lexicon_dictionary/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.6/socscikit/lexicon_dictionary/VADER/VADER.csv` & `socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/VADER.csv`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.6/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle` & `socscikit-0.0.5.7/socscikit/lexicon_dictionary/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.6/socscikit/socialmedia.py` & `socscikit-0.0.5.7/socscikit/socialmedia.py`

 * *Files identical despite different names*

### Comparing `socscikit-0.0.5.6/socscikit/utils.py` & `socscikit-0.0.5.7/socscikit/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from rich.progress import track
 from rich import print as pprint
 import itertools
 from itertools import combinations, chain
 import statistics
 from collections import Counter
 import spacy
+from spacymoji import Emoji
+import re 
 
 
 class CS:
     def __init__(self):
         self.spacy_nlp = spacy.load(
             "en_core_web_sm"
-        )  # could be removed to summarise_lex_dict if not used frequently
+        ).add_pipe("emoji", first=True)
 
+    def extract_emoticons(text):
+        emoticon_pattern = re.compile(r'(?::|;|=)(?:-)?(?:\)|D|P|O|S|\(|\||\\|\/|\[|\]|x|X|<|>|\'|\"|@|3|8|\$|_|{|}|;|\\|\*|,|\.|!|0|_|<|3|>|\^|¯|–|`|\*)[.,!?\'\"]*|[.,!?\'\"]*(?:\)|D|P|O|S|\(|\||\\|\/|\[|\]|x|X|<|>|\'|\"|@|3|8|\$|_|{|}|;|\\|\*|,|\.|!|0|_|<|3|>|\^|¯|–|`|\*)(?:-)?(?::|;|=)')
+        emoticons = re.findall(emoticon_pattern, text)
+        return emoticons
+    
     def count_categorical_labels(self, dictionary):
         label_counts = Counter()
         multi_label_counts = Counter()
 
         for sublist in track(
             dictionary.values(),
             description="Computing Summary Statistics of Sentiment Scores",
@@ -67,15 +74,15 @@
 
                 if multi_label in multi_label_counts:
                     multi_label_counts[multi_label] += 1
                 else:
                     multi_label_counts[multi_label] = 1
 
         output = {
-            "labels": list(label_counts.keys()),
+            "labels": sorted(list(label_counts.keys())),
             "label frequency": self.sort_dict(label_counts),
             "multi label frequency": self.sort_dict(multi_label_counts),
         }
 
         if not output["multi label frequency"]:
             del output["multi label frequency"]
 
@@ -164,27 +171,35 @@
         pos_tags = []
         general_dict = {
             "verbs": 0,
             "adjectives": 0,
             "adverbs": 0,
             "prepositions": 0,
             "nouns": 0,
+            "emo": 0,
             "miscellaneous": 0,
         }
         granular_dict = {}
         misc = []
 
         for key in track(
             lexicon_dictionary.keys(),
             description="Extracting Summary Insights from Sentiment Lexicons",
             transient=True
         ):
             doc = self.spacy_nlp(key)
             for token in doc:
-                pos_tags.append(token.tag_)
+                #check if token is emoji 
+                if token._.is_emoji: 
+                    pos_tags.append("EMOJI")
+                #check if token is emoticon 
+                elif token.text in self.extract_emoticons(token.text):
+                    pos_tags.append("EMOTICON")
+                else: 
+                     pos_tags.append(token.tag_)
 
         for element in pos_tags:
             if element in granular_dict:
                 granular_dict[element] += 1
             else:
                 granular_dict[element] = 1
 
@@ -195,14 +210,16 @@
                 general_dict["adjectives"] += value
             elif key.startswith("RB"):
                 general_dict["adverbs"] += value
             elif key.startswith("IN"):
                 general_dict["prepositions"] += value
             elif key.startswith("N"):
                 general_dict["nouns"] += value
+            elif key.startswith("EMO"):
+                general_dict["emos"] += value 
             else:
                 misc.append(key)
                 general_dict["miscellaneous"] += value
 
         part_of_speech = {
             "general": self.sort_dict(general_dict),
             "granular": self.sort_dict(granular_dict),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `socscikit-0.0.5.6/socscikit.egg-info/SOURCES.txt` & `socscikit-0.0.5.7/socscikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

