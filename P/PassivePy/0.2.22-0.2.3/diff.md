# Comparing `tmp/PassivePy-0.2.22.tar.gz` & `tmp/PassivePy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PassivePy-0.2.22.tar", last modified: Mon Jul 17 23:03:14 2023, max compression
+gzip compressed data, was "PassivePy-0.2.3.tar", last modified: Sat Jan  8 09:51:57 2022, max compression
```

## Comparing `PassivePy-0.2.22.tar` & `PassivePy-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 23:03:14.653567 PassivePy-0.2.22/
--rw-rw-rw-   0        0        0     1094 2022-07-26 21:56:07.000000 PassivePy-0.2.22/LICENSE
--rw-rw-rw-   0        0        0     5987 2023-07-17 23:03:14.652566 PassivePy-0.2.22/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 23:03:14.596946 PassivePy-0.2.22/PassivePyCode/
-drwxrwxrwx   0        0        0        0 2023-07-17 23:03:14.642076 PassivePy-0.2.22/PassivePyCode/PassivePy.egg-info/
--rw-rw-rw-   0        0        0     5987 2023-07-17 23:03:13.000000 PassivePy-0.2.22/PassivePyCode/PassivePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-07-17 23:03:14.000000 PassivePy-0.2.22/PassivePyCode/PassivePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 23:03:13.000000 PassivePy-0.2.22/PassivePyCode/PassivePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-17 23:03:14.000000 PassivePy-0.2.22/PassivePyCode/PassivePy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-17 23:03:14.000000 PassivePy-0.2.22/PassivePyCode/PassivePy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 23:03:14.650571 PassivePy-0.2.22/PassivePyCode/PassivePySrc/
--rw-rw-rw-   0        0        0    24240 2023-04-17 15:56:08.000000 PassivePy-0.2.22/PassivePyCode/PassivePySrc/PassivePy.py
--rw-rw-rw-   0        0        0        0 2022-07-26 21:56:07.000000 PassivePy-0.2.22/PassivePyCode/PassivePySrc/__init__.py
--rw-rw-rw-   0        0        0     4153 2023-04-17 15:56:08.000000 PassivePy-0.2.22/PassivePyCode/PassivePySrc/rules_for_all_passives.py
--rw-rw-rw-   0        0        0     4012 2023-04-17 15:56:08.000000 PassivePy-0.2.22/PassivePyCode/PassivePySrc/rules_for_full_passives.py
--rw-rw-rw-   0        0        0     2692 2023-04-17 15:56:08.000000 PassivePy-0.2.22/PassivePyCode/PassivePySrc/rules_for_truncated_passives.py
--rw-rw-rw-   0        0        0     5248 2023-07-17 23:02:21.000000 PassivePy-0.2.22/README.md
--rw-rw-rw-   0        0        0      160 2022-10-20 22:55:16.000000 PassivePy-0.2.22/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 23:03:14.653567 PassivePy-0.2.22/setup.cfg
--rw-rw-rw-   0        0        0     1179 2023-07-17 23:02:07.000000 PassivePy-0.2.22/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-08 09:51:57.194876 PassivePy-0.2.3/
+-rw-rw-rw-   0        0        0       66 2021-09-13 06:57:40.000000 PassivePy-0.2.3/.gitignore
+drwxrwxrwx   0        0        0        0 2022-01-08 09:51:57.090921 PassivePy-0.2.3/Data/
+drwxrwxrwx   0        0        0        0 2022-01-08 09:51:57.090921 PassivePy-0.2.3/Data/Output files/
+-rw-rw-rw-   0        0        0    65578 2021-10-24 10:30:26.000000 PassivePy-0.2.3/Data/Output files/CoLA_dataset_output.csv
+-rw-rw-rw-   0        0        0    61688 2021-10-24 16:22:19.000000 PassivePy-0.2.3/Data/Output files/CoLA_dataset_sentence_level_output.csv
+-rw-rw-rw-   0        0        0    89774 2021-10-24 10:26:20.000000 PassivePy-0.2.3/Data/Output files/crowdsource_dataset_output.csv
+-rw-rw-rw-   0        0        0   105593 2021-07-08 07:20:21.000000 PassivePy-0.2.3/Data/paper_abstract_50_samples.csv
+-rw-rw-rw-   0        0        0    70528 2021-07-08 06:05:23.000000 PassivePy-0.2.3/Data/passivepy_humancoding_match.xlsx
+-rw-rw-rw-   0        0        0     1094 2021-06-30 05:26:13.000000 PassivePy-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     6484 2022-01-08 09:51:57.194876 PassivePy-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0   157311 2021-12-23 13:11:17.000000 PassivePy-0.2.3/PassivePy notebook.ipynb
+-rw-rw-rw-   0        0        0   102549 2021-12-02 14:59:27.000000 PassivePy-0.2.3/PassivePy.ipynb
+drwxrwxrwx   0        0        0        0 2022-01-08 09:51:57.075299 PassivePy-0.2.3/PassivePyCode/
+drwxrwxrwx   0        0        0        0 2022-01-08 09:51:57.105761 PassivePy-0.2.3/PassivePyCode/PassivePy.egg-info/
+-rw-rw-rw-   0        0        0     6484 2022-01-08 09:51:56.000000 PassivePy-0.2.3/PassivePyCode/PassivePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1188 2022-01-08 09:51:56.000000 PassivePy-0.2.3/PassivePyCode/PassivePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-08 09:51:56.000000 PassivePy-0.2.3/PassivePyCode/PassivePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2022-01-08 09:51:56.000000 PassivePy-0.2.3/PassivePyCode/PassivePy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-01-08 09:51:56.000000 PassivePy-0.2.3/PassivePyCode/PassivePy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-01-08 09:51:57.111556 PassivePy-0.2.3/PassivePyCode/PassivePySrc/
+-rw-rw-rw-   0        0        0    24764 2021-11-15 19:46:02.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/PassivePy.py
+-rw-rw-rw-   0        0        0        0 2021-07-07 16:24:26.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-08 09:51:57.194876 PassivePy-0.2.3/PassivePyCode/PassivePySrc/__pycache__/
+-rw-rw-rw-   0        0        0      155 2021-11-15 19:21:19.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1716 2021-12-02 14:59:21.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/__pycache__/rules_for_all_passives.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1733 2021-12-02 14:59:21.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/__pycache__/rules_for_full_passives.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1566 2021-12-02 14:59:21.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/__pycache__/rules_for_truncated_passives.cpython-38.pyc
+-rw-rw-rw-   0        0        0      186 2021-11-07 07:27:14.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/requirements_lg.txt
+-rw-rw-rw-   0        0        0      186 2021-11-07 07:27:14.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/requirements_sm.txt
+-rw-rw-rw-   0        0        0     4415 2021-11-15 19:35:18.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/rules_for_all_passives.py
+-rw-rw-rw-   0        0        0     4461 2021-11-15 19:35:18.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/rules_for_full_passives.py
+-rw-rw-rw-   0        0        0     3421 2021-11-15 19:35:18.000000 PassivePy-0.2.3/PassivePyCode/PassivePySrc/rules_for_truncated_passives.py
+-rw-rw-rw-   0        0        0     4952 2022-01-08 09:49:45.000000 PassivePy-0.2.3/README.md
+-rw-rw-rw-   0        0        0      160 2021-07-05 11:04:14.000000 PassivePy-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-01-08 09:51:57.194876 PassivePy-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1178 2022-01-08 09:48:42.000000 PassivePy-0.2.3/setup.py
```

### Comparing `PassivePy-0.2.22/LICENSE` & `PassivePy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PassivePy-0.2.22/PKG-INFO` & `PassivePy-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,119 @@
 Metadata-Version: 2.1
 Name: PassivePy
-Version: 0.2.22
+Version: 0.2.3
 Summary: A package for processing large corpora and detecting passive voice.
 Home-page: https://github.com/mitramir55/PassivePy
 Author: Mitra Mirshafiee
 Author-email: mitra.mirshafiee@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Description: # PassivePy: A Tool to Automatically Identify Passive Voice in Big Text Data
+        
+        
+        Our aim with this work is to create a reliable (e.g., passive voice judgments are consistent), valid (e.g., passive voice judgments are accurate), flexible (e.g., texts can be assessed at different units of analysis), replicable (e.g., the approach can be performed by a range of research teams with varying levels of computational expertise), and scalable way (e.g., small and large collections of texts can be analyzed) to capture passive voice from different corpora for social and psychological evaluations of text. To achieve these aims, we introduce PassivePy, a fully transparent and documented Python library.
+        
+        For accessing the datasets in our paper, please click on [this link](https://osf.io/j2b6u/?view_only=0e78d7f4028041b693d6b64547b514ca). 
+        
+        If you haven't used Python before or need detailed instructions about how to use this package please visit [our website](https://mitramir55.github.io/PassivePyWeb/).
+        
+        
+        First we have to install the requirements in the following way (all requirements are needed for spaCy or other libraries we use.):
+        ```
+        !pip install -r https://raw.githubusercontent.com/mitramir55/PassivePy/main/PassivePyCode/PassivePySrc/requirements_lg.txt
+        !pip install PassivePy==0.2.3
+        
+        ```
+        Then, import PassivePy and initiate the analyzer:
+        
+        ```
+        from PassivePySrc import PassivePy
+        
+        spacy_model = "en_core_web_lg"
+        passivepy = PassivePy.PassivePyAnalyzer(spacy_model)
+        ```
+        Use passivepy for single sentences:
+        ```
+        # Try changing the sentence below:
+        sample_text = "The painting has been drawn."
+        passivepy.passivepy.match_text(sample_text, full_passive=True, truncated_passive=True)
+        ```
+        The output will be:
+        ```
+        sentence : the input sentence
+        binary : Whether any passive voice is detected 
+        passive_match(es) : The span of passive form in text
+        raw_passive_count : Number of passive voices
+        ```
+        You can set the full_passive or truncated_passive to true if you want the same sort of output for these two types of passive. (truncated is a passive without an object of preposition, while a full passive is one with the object of preposition - e.g., this was broken by him.)
+        
+        
+        For processing datasets, we have can either analyze the records sentence- or corpus-level. Your dataset can be in any format (e.g., CSV, XLSX or XLS).; however, make sure to that it has at least one column with the text that needs to be analyzed.
+        
+        In case of large datasets, you can also add `batch_size = ...` and `n_process=...` to speed up the analysis (the default for both is 1).
+        
+        
+        ``` 
+        # sentence level:
+        df_detected_s = passivepy.match_sentence_level(df, column_name='documents', n_process = 1,
+                                                        batch_size = 1000, add_other_columns=True,
+                                                        truncated_passive=False, full_passive=False)
+        
+        # corpus level
+        df_detected_c = passivepy.match_corpus_level(df, column_name='sentences', n_process = 1,
+                                                    batch_size = 1000, add_other_columns=True,
+                                                    truncated_passive=False, full_passive=False)
+        ```
+        In the output you will have a data frame with the following columns:
+        
+        ```
+        # corpus level
+        document : Records in the input data frame
+        binary : Whether a passive was detected in that document
+        passive_match(es) : Parts of the document detected as passive
+        raw_passive_count : Number of passive voices detected in the sentence
+        raw_passive_sents_count : Number of sentences with passive voice
+        raw_sentence_count : Number of sentences detected in the document
+        passive_sents_percentage : Proportion of passive sentences to total number of sentences
+        
+        # Sentence level
+        docId : Initial index of the record in the input file
+        sentenceId : The ith sentence in one specific record
+        sentence : The detected sentence
+        binary : Whether a passive was detected in that sentence
+        passive_match(es) : The part of the record detected as passive voice
+        raw_passive_count : Number of passive forms detected in the sentence
+        
+        ```
+        
+        If you needed to analyze each token of a sentence, i.g., print out the `DEP` (dependency), `POS` (coarse-grained POS tags), `TAG` (fine-grained part of speech tags), `LEMMA` (canonical form) of a word,  you can use the `parse_sentence` method of passivepy in the following way:
+        
+        ```
+        sample_sentence = "She has been killed"
+        passivepy.parse_sentence(sample_sentence)
+        ```
+        And the output will be like the sample below:
+        ```
+        word: She 
+        pos: PRON 
+        dependency: nsubjpass 
+        tag:  PRP 
+        lemma:  she
+        ...
+        ```
+        
+        
+        
+        If you do not need any columns to be appended to the main dataset, simply add `add_other_columns = False`, or if you don't what the percentages to show up add `percentage_of_passive_sentences = False` in any of the following functions.
+        
+        
+        Accuracy on the CoLA dataset: 0.97
+        Accuracy on the CrowdSource Dataset: 0.98
+        
 Keywords: passive voice,text analysis,spacy,dependency parsing,part of speech tagging
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PassivePy: A Tool to Automatically Identify Passive Voice in Big Text Data
-
-**_This repository is the code of the following paper, so if you use this package, please cite the work as:
-Sepehri, A., Markowitz, D. M., & Mir, M. (2022, February 3). PassivePy: A Tool to Automatically Identify Passive Voice in Big Text Data. [Preprint available](https://psyarxiv.com/bwp3t/)**
-
-
-Our aim with this work is to create a reliable (e.g., passive voice judgments are consistent), valid (e.g., passive voice judgments are accurate), flexible (e.g., texts can be assessed at different units of analysis), replicable (e.g., the approach can be performed by a range of research teams with varying levels of computational expertise), and scalable way (e.g., small and large collections of texts can be analyzed) to capture passive voice from different corpora for social and psychological evaluations of text. To achieve these aims, we introduce PassivePy, a fully transparent and documented Python library.
-
-For accessing the datasets in our paper, please click on [this link](https://osf.io/j2b6u/?view_only=0e78d7f4028041b693d6b64547b514ca). 
-
-If you haven't used Python before or need detailed instructions about how to use this package please visit [our website](https://passivepy.streamlit.app/).
-
-
-First we have to install the requirements in the following way (all requirements are needed for spaCy or other libraries we use.):
-```
-!pip install -r https://raw.githubusercontent.com/mitramir55/PassivePy/main/PassivePyCode/PassivePySrc/requirements_lg.txt
-!pip install PassivePy==0.2.22
-
-```
-Then, import PassivePy and initiate the analyzer:
-
-```
-from PassivePySrc import PassivePy
-
-passivepy = PassivePy.PassivePyAnalyzer(spacy_model = "en_core_web_lg")
-```
-Use passivepy for single sentences:
-```
-# Try changing the sentence below:
-sample_text = "The painting has been drawn."
-passivepy.passivepy.match_text(sample_text, full_passive=True, truncated_passive=True)
-```
-The output will be:
-```
-sentence : the input sentence
-binary : Whether any passive voice is detected 
-passive_match(es) : The span of passive form in text
-raw_passive_count : Number of passive voices
-```
-You can set the full_passive or truncated_passive to true if you want the same sort of output for these two types of passive. (truncated is a passive without an object of preposition, while a full passive is one with the object of preposition - e.g., this was broken by him.)
-
-
-For processing datasets, we have can either analyze the records sentence- or corpus-level. Your dataset can be in any format (e.g., CSV, XLSX or XLS).; however, make sure to that it has at least one column with the text that needs to be analyzed.
-
-In case of large datasets, you can also add `batch_size = ...` and `n_process=...` to speed up the analysis (the default for both is 1).
-
-
-``` 
-# sentence level:
-df_detected_s = passivepy.match_sentence_level(df, column_name='documents', n_process = 1,
-                                                batch_size = 1000, add_other_columns=True,
-                                                truncated_passive=False, full_passive=False)
-
-# corpus level
-df_detected_c = passivepy.match_corpus_level(df, column_name='sentences', n_process = 1,
-                                            batch_size = 1000, add_other_columns=True,
-                                            truncated_passive=False, full_passive=False)
-```
-In the output you will have a data frame with the following columns:
-
-```
-# corpus level
-document : Records in the input data frame
-binary : Whether a passive was detected in that document
-passive_match(es) : Parts of the document detected as passive
-raw_passive_count : Number of passive voices detected in the sentence
-raw_passive_sents_count : Number of sentences with passive voice
-raw_sentence_count : Number of sentences detected in the document
-passive_sents_percentage : Proportion of passive sentences to total number of sentences
-
-# Sentence level
-docId : Initial index of the record in the input file
-sentenceId : The ith sentence in one specific record
-sentence : The detected sentence
-binary : Whether a passive was detected in that sentence
-passive_match(es) : The part of the record detected as passive voice
-raw_passive_count : Number of passive forms detected in the sentence
-
-```
-
-If you needed to analyze each token of a sentence, i.g., print out the `DEP` (dependency), `POS` (coarse-grained part of speech tags), `TAG` (fine-grained part of speech tags), `LEMMA` (canonical form) of a word,  you can use the `parse_sentence` method of passivepy in the following way:
-
-```
-sample_sentence = "She has been killed"
-passivepy.parse_sentence(sample_sentence)
-```
-And the output will be like the sample below:
-```
-word: She 
-pos: PRON 
-dependency: nsubjpass 
-tag:  PRP 
-lemma:  she
-...
-```
-
-
-
-If you do not need any columns to be appended to the main dataset, simply add `add_other_columns = False`, or if you don't what the percentages to show up add `percentage_of_passive_sentences = False` in any of the following functions.
-
-
-Accuracy on the CoLA dataset: 0.97
-Accuracy on the CrowdSource Dataset: 0.98
-
-
-
-
-
```

### Comparing `PassivePy-0.2.22/PassivePyCode/PassivePy.egg-info/PKG-INFO` & `PassivePy-0.2.3/PassivePyCode/PassivePy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,119 @@
 Metadata-Version: 2.1
 Name: PassivePy
-Version: 0.2.22
+Version: 0.2.3
 Summary: A package for processing large corpora and detecting passive voice.
 Home-page: https://github.com/mitramir55/PassivePy
 Author: Mitra Mirshafiee
 Author-email: mitra.mirshafiee@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Description: # PassivePy: A Tool to Automatically Identify Passive Voice in Big Text Data
+        
+        
+        Our aim with this work is to create a reliable (e.g., passive voice judgments are consistent), valid (e.g., passive voice judgments are accurate), flexible (e.g., texts can be assessed at different units of analysis), replicable (e.g., the approach can be performed by a range of research teams with varying levels of computational expertise), and scalable way (e.g., small and large collections of texts can be analyzed) to capture passive voice from different corpora for social and psychological evaluations of text. To achieve these aims, we introduce PassivePy, a fully transparent and documented Python library.
+        
+        For accessing the datasets in our paper, please click on [this link](https://osf.io/j2b6u/?view_only=0e78d7f4028041b693d6b64547b514ca). 
+        
+        If you haven't used Python before or need detailed instructions about how to use this package please visit [our website](https://mitramir55.github.io/PassivePyWeb/).
+        
+        
+        First we have to install the requirements in the following way (all requirements are needed for spaCy or other libraries we use.):
+        ```
+        !pip install -r https://raw.githubusercontent.com/mitramir55/PassivePy/main/PassivePyCode/PassivePySrc/requirements_lg.txt
+        !pip install PassivePy==0.2.3
+        
+        ```
+        Then, import PassivePy and initiate the analyzer:
+        
+        ```
+        from PassivePySrc import PassivePy
+        
+        spacy_model = "en_core_web_lg"
+        passivepy = PassivePy.PassivePyAnalyzer(spacy_model)
+        ```
+        Use passivepy for single sentences:
+        ```
+        # Try changing the sentence below:
+        sample_text = "The painting has been drawn."
+        passivepy.passivepy.match_text(sample_text, full_passive=True, truncated_passive=True)
+        ```
+        The output will be:
+        ```
+        sentence : the input sentence
+        binary : Whether any passive voice is detected 
+        passive_match(es) : The span of passive form in text
+        raw_passive_count : Number of passive voices
+        ```
+        You can set the full_passive or truncated_passive to true if you want the same sort of output for these two types of passive. (truncated is a passive without an object of preposition, while a full passive is one with the object of preposition - e.g., this was broken by him.)
+        
+        
+        For processing datasets, we have can either analyze the records sentence- or corpus-level. Your dataset can be in any format (e.g., CSV, XLSX or XLS).; however, make sure to that it has at least one column with the text that needs to be analyzed.
+        
+        In case of large datasets, you can also add `batch_size = ...` and `n_process=...` to speed up the analysis (the default for both is 1).
+        
+        
+        ``` 
+        # sentence level:
+        df_detected_s = passivepy.match_sentence_level(df, column_name='documents', n_process = 1,
+                                                        batch_size = 1000, add_other_columns=True,
+                                                        truncated_passive=False, full_passive=False)
+        
+        # corpus level
+        df_detected_c = passivepy.match_corpus_level(df, column_name='sentences', n_process = 1,
+                                                    batch_size = 1000, add_other_columns=True,
+                                                    truncated_passive=False, full_passive=False)
+        ```
+        In the output you will have a data frame with the following columns:
+        
+        ```
+        # corpus level
+        document : Records in the input data frame
+        binary : Whether a passive was detected in that document
+        passive_match(es) : Parts of the document detected as passive
+        raw_passive_count : Number of passive voices detected in the sentence
+        raw_passive_sents_count : Number of sentences with passive voice
+        raw_sentence_count : Number of sentences detected in the document
+        passive_sents_percentage : Proportion of passive sentences to total number of sentences
+        
+        # Sentence level
+        docId : Initial index of the record in the input file
+        sentenceId : The ith sentence in one specific record
+        sentence : The detected sentence
+        binary : Whether a passive was detected in that sentence
+        passive_match(es) : The part of the record detected as passive voice
+        raw_passive_count : Number of passive forms detected in the sentence
+        
+        ```
+        
+        If you needed to analyze each token of a sentence, i.g., print out the `DEP` (dependency), `POS` (coarse-grained POS tags), `TAG` (fine-grained part of speech tags), `LEMMA` (canonical form) of a word,  you can use the `parse_sentence` method of passivepy in the following way:
+        
+        ```
+        sample_sentence = "She has been killed"
+        passivepy.parse_sentence(sample_sentence)
+        ```
+        And the output will be like the sample below:
+        ```
+        word: She 
+        pos: PRON 
+        dependency: nsubjpass 
+        tag:  PRP 
+        lemma:  she
+        ...
+        ```
+        
+        
+        
+        If you do not need any columns to be appended to the main dataset, simply add `add_other_columns = False`, or if you don't what the percentages to show up add `percentage_of_passive_sentences = False` in any of the following functions.
+        
+        
+        Accuracy on the CoLA dataset: 0.97
+        Accuracy on the CrowdSource Dataset: 0.98
+        
 Keywords: passive voice,text analysis,spacy,dependency parsing,part of speech tagging
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PassivePy: A Tool to Automatically Identify Passive Voice in Big Text Data
-
-**_This repository is the code of the following paper, so if you use this package, please cite the work as:
-Sepehri, A., Markowitz, D. M., & Mir, M. (2022, February 3). PassivePy: A Tool to Automatically Identify Passive Voice in Big Text Data. [Preprint available](https://psyarxiv.com/bwp3t/)**
-
-
-Our aim with this work is to create a reliable (e.g., passive voice judgments are consistent), valid (e.g., passive voice judgments are accurate), flexible (e.g., texts can be assessed at different units of analysis), replicable (e.g., the approach can be performed by a range of research teams with varying levels of computational expertise), and scalable way (e.g., small and large collections of texts can be analyzed) to capture passive voice from different corpora for social and psychological evaluations of text. To achieve these aims, we introduce PassivePy, a fully transparent and documented Python library.
-
-For accessing the datasets in our paper, please click on [this link](https://osf.io/j2b6u/?view_only=0e78d7f4028041b693d6b64547b514ca). 
-
-If you haven't used Python before or need detailed instructions about how to use this package please visit [our website](https://passivepy.streamlit.app/).
-
-
-First we have to install the requirements in the following way (all requirements are needed for spaCy or other libraries we use.):
-```
-!pip install -r https://raw.githubusercontent.com/mitramir55/PassivePy/main/PassivePyCode/PassivePySrc/requirements_lg.txt
-!pip install PassivePy==0.2.22
-
-```
-Then, import PassivePy and initiate the analyzer:
-
-```
-from PassivePySrc import PassivePy
-
-passivepy = PassivePy.PassivePyAnalyzer(spacy_model = "en_core_web_lg")
-```
-Use passivepy for single sentences:
-```
-# Try changing the sentence below:
-sample_text = "The painting has been drawn."
-passivepy.passivepy.match_text(sample_text, full_passive=True, truncated_passive=True)
-```
-The output will be:
-```
-sentence : the input sentence
-binary : Whether any passive voice is detected 
-passive_match(es) : The span of passive form in text
-raw_passive_count : Number of passive voices
-```
-You can set the full_passive or truncated_passive to true if you want the same sort of output for these two types of passive. (truncated is a passive without an object of preposition, while a full passive is one with the object of preposition - e.g., this was broken by him.)
-
-
-For processing datasets, we have can either analyze the records sentence- or corpus-level. Your dataset can be in any format (e.g., CSV, XLSX or XLS).; however, make sure to that it has at least one column with the text that needs to be analyzed.
-
-In case of large datasets, you can also add `batch_size = ...` and `n_process=...` to speed up the analysis (the default for both is 1).
-
-
-``` 
-# sentence level:
-df_detected_s = passivepy.match_sentence_level(df, column_name='documents', n_process = 1,
-                                                batch_size = 1000, add_other_columns=True,
-                                                truncated_passive=False, full_passive=False)
-
-# corpus level
-df_detected_c = passivepy.match_corpus_level(df, column_name='sentences', n_process = 1,
-                                            batch_size = 1000, add_other_columns=True,
-                                            truncated_passive=False, full_passive=False)
-```
-In the output you will have a data frame with the following columns:
-
-```
-# corpus level
-document : Records in the input data frame
-binary : Whether a passive was detected in that document
-passive_match(es) : Parts of the document detected as passive
-raw_passive_count : Number of passive voices detected in the sentence
-raw_passive_sents_count : Number of sentences with passive voice
-raw_sentence_count : Number of sentences detected in the document
-passive_sents_percentage : Proportion of passive sentences to total number of sentences
-
-# Sentence level
-docId : Initial index of the record in the input file
-sentenceId : The ith sentence in one specific record
-sentence : The detected sentence
-binary : Whether a passive was detected in that sentence
-passive_match(es) : The part of the record detected as passive voice
-raw_passive_count : Number of passive forms detected in the sentence
-
-```
-
-If you needed to analyze each token of a sentence, i.g., print out the `DEP` (dependency), `POS` (coarse-grained part of speech tags), `TAG` (fine-grained part of speech tags), `LEMMA` (canonical form) of a word,  you can use the `parse_sentence` method of passivepy in the following way:
-
-```
-sample_sentence = "She has been killed"
-passivepy.parse_sentence(sample_sentence)
-```
-And the output will be like the sample below:
-```
-word: She 
-pos: PRON 
-dependency: nsubjpass 
-tag:  PRP 
-lemma:  she
-...
-```
-
-
-
-If you do not need any columns to be appended to the main dataset, simply add `add_other_columns = False`, or if you don't what the percentages to show up add `percentage_of_passive_sentences = False` in any of the following functions.
-
-
-Accuracy on the CoLA dataset: 0.97
-Accuracy on the CrowdSource Dataset: 0.98
-
-
-
-
-
```

### Comparing `PassivePy-0.2.22/PassivePyCode/PassivePySrc/PassivePy.py` & `PassivePy-0.2.3/PassivePyCode/PassivePySrc/PassivePy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-#  Copyright Mitra Mirshafiee, 2022 Licensed under MIT License.
-#  See the LICENSE.txt for more information.
-
 import pandas as pd
 import numpy as np
 import spacy
 from termcolor import colored
 import regex as re
 from itertools import chain 
+from tqdm import tqdm
+import tqdm.notebook as tq
 import os, sys
 
 
 try: 
     from PassivePyCode.PassivePySrc.rules_for_all_passives import create_matcher
     from PassivePyCode.PassivePySrc.rules_for_full_passives import create_matcher_full
     from PassivePyCode.PassivePySrc.rules_for_truncated_passives import create_matcher_truncated
@@ -19,30 +18,38 @@
     from PassivePySrc.rules_for_full_passives import create_matcher_full
     from PassivePySrc.rules_for_truncated_passives  import create_matcher_truncated
 
 class PassivePyAnalyzer:
     
         """
             Get the data from a dataframe.
-            identify sentences
+
+            Clean the dataset based on the given regex patterns.
             Match passive voice sentence level or corpus level.
             save the output to a file
 
         """
-        def __init__(self, nlp:spacy.language.Language=None, spacy_model:str = "en_core_web_lg"):
+        def __init__(self, spacy_model = "en_core_web_lg"):
 
             """
             Create the Detector
 
+            n_processses: number of core to use
+            batch_size: size of batches of records passed onto the matcher
+            regex_patterns: Patterns that should be detected and cleaned from the data
+            
+            
             """
-            self.nlp, self.matcher = create_matcher(nlp=nlp, spacy_model=spacy_model)
-            self.matcher_t = create_matcher_truncated(self.nlp)
-            self.matcher_f = create_matcher_full(self.nlp)
+            # os.system('pip install -r https://raw.githubusercontent.com/mitramir55/PassivePy/main/PassivePyCode/PassivePySrc/requirements.txt')
+            self.nlp, self.matcher_t = create_matcher_truncated(spacy_model)
+            self.nlp, self.matcher_f = create_matcher_full(spacy_model)
+            self.nlp, self.matcher = create_matcher(spacy_model)
 
-        def print_matches(self, sentence, truncated_passive=False, full_passive=False):
+        def print_matches(self, sentence,
+         truncated_passive=False, full_passive=False):
             """
             prints match span - I removed this from parse_sentence after changing its 
             structure. It is used by the author for testing.
             """
             doc = self.nlp(sentence)
             if truncated_passive: matches = self.matcher_t(doc)
             elif full_passive:matches = self.matcher_f(doc)
@@ -79,29 +86,32 @@
             print('Detecting Sentences...')
 
             """
             Separates sentences from each other in each record
              and puts them in a list along side the count of sentences in each 
              document in another list
              """
-            # document = [corpus.lower() for corpus in document]
+            document = [corpus.lower() for corpus in document]
 
             all_sentences = []
             count_sents = []
+            unwanted = []
 
             # go through all the records
             m = 0
-            for record_doc in self.nlp.pipe(document, batch_size=batch_size, n_process = n_process):
+            for record_doc in tq.tqdm(self.nlp.pipe(document, batch_size=batch_size, n_process = n_process), 
+                                    leave=True,
+                                    position=0,
+                                    total=len(document)):
 
 
                 sentences = list(record_doc.sents)
                 sentences = [str(sentence) if len(sentence)>=2 else 'Not a Sentence' for sentence in sentences] 
 
 
-                unwanted = []
                 for sentence in sentences:
                     i = sentences.index(sentence)
                 
                     
                     #...........................joining with the previous one.............................#
                     # ones that start with but and their previous record doesn't have dot at its end
                     if i!=0:
@@ -149,21 +159,22 @@
                             sentences[i] = ' '.join([sentences[i], sentences[i+1]])
                             unwanted.append(i+1)
 
 
                 m+=1
                 for index in sorted(set(unwanted), reverse=True):
                     del sentences[index]
+                unwanted = []
 
-
+                
                 count_sents.append(len(sentences))
                 all_sentences.append(sentences) 
 
             all_sentences = list(chain.from_iterable(all_sentences))
-            # print(f'Total number of sentences = {len(all_sentences)}')
+            print(f'Total number of sentences = {len(all_sentences)}')
 
 
             return np.array(count_sents, dtype='object'), np.array(all_sentences, dtype='object')
 
 
         def _find_doc_idx(self, count_sents):
 
@@ -175,15 +186,14 @@
             for i in count_sents:
                 n = 1
                 for j in range(i):
                     sent_indices.append(n)
                     doc_indices.append(m)
                     n+=1
                 m+=1
-
             return pd.DataFrame(sent_indices), pd.DataFrame(doc_indices)
 
 
         def _add_other_cols(self, df, column_name, count_sents):
 
             """ creates a dataframe of all the other columns
             with the required number of repetitions for each """
@@ -271,20 +281,22 @@
             raw_truncated_passive_count = []
             truncated_passive_matches = []
             binary_truncated_passive = []
             # -----------------------------------------------------------------
 
 
             
-            for doc in self.nlp.pipe(sentences, batch_size=batch_size, n_process=n_process):
+            for doc in tq.tqdm(self.nlp.pipe(sentences, batch_size=batch_size, n_process=n_process), 
+                                    leave=True,
+                                    position=0,
+                                    total=len(sentences)):
 
                 binary_f = 0
                 binary_t = 0
                 binary_i = 0
-
                 # truncated passive voice ----------------------------------
                 if truncated_passive:
 
                     truncated_matches_i = self._find_unique_spans(doc, truncated_passive, full_passive=False)
                     if truncated_matches_i != []:
                         
                         # because the truncated version adds one token at the end
@@ -351,15 +363,15 @@
             
             return output_dict
 
 
         def match_sentence_level(self, df, column_name, n_process = 1,
                                 batch_size = 1000, add_other_columns=True,
                                 truncated_passive=False, full_passive=False):
-                                
+
             """
             Parameters
 
             column_name: name of the column with text
             level: whether the user wants corpus level or sentence level results
             n_process: number of cores to use can be any number
             between 1 and the maximum number of cores available
@@ -389,22 +401,24 @@
             
             # add indices
             df_output.insert(0, "docId", doc_indices)
             df_output.insert(1, "sentenceId", sent_indices)
 
 
             # concatenating the results with the initial df -------------------
-            if len(df.columns) == 1: 
-                add_other_columns=False
-            if add_other_columns:
+            if add_other_columns==True:
 
                 other_cols_df = self._add_other_cols(df, column_name, count_sents)
                 assert len(other_cols_df) == len(df_output)
-                df_output = pd.concat([df_output, other_cols_df], axis = 1)
-            return df_output
+                df_final = pd.concat([df_output, other_cols_df], axis = 1)
+
+                return df_final
+
+            else:
+                return df_output
 
 
         def _all_elements_in_one_list(self, series_: pd.Series(list)) -> list:
             """
             a function for reducing the size of a series
             """
             # output: 1d list
@@ -444,59 +458,55 @@
 
             df_output = self.match_sentence_level(
                 df, column_name, n_process,
                 batch_size, add_other_columns,
                 truncated_passive, full_passive
                 )
 
-            # declare variables -----------------------------------------
+            # define parameters-----------------------------------------
             # full passive
-            if full_passive:
-                full_passive_matches = []
-                full_passive_count = []
-                binary_full_passive = []
-                full_passive_percentages = []
-                full_passive_sents_count = []
+            full_passive_matches = []
+            full_passive_count = []
+            binary_full_passive = []
+            full_passive_percentages = []
+            full_passive_sents_count = []
 
             # truncated
-            if truncated_passive:
-                truncated_passive_matches = []
-                truncated_passive_count = []
-                binary_truncated_passive = []
-                truncated_passive_percentages = []
-                truncated_passive_sents_count = []
+            truncated_passive_matches = []
+            truncated_passive_count = []
+            binary_truncated_passive = []
+            truncated_passive_percentages = []
+            truncated_passive_sents_count = []
             
-            # all passives
+            # truncated
             all_passives = []
             passive_count = []
             binary = []
             passive_percentages = []
             passive_sents_count = []
             # -------------------------------------------------------------------
 
             # general
             count_sents = []
             output_dict = {}
             columns = [
                 document, count_sents, all_passives, passive_count, 
                 passive_sents_count, passive_percentages, binary
                 ]
-
             # list all the docs
             ids_ = df_output.docId.unique()
             
 
-            for i in ids_:
+            for i in tq.tqdm(ids_, leave=True, position=0, total=len(ids_)):
 
                 # select all the sentences of a doc
                 rows = df_output[df_output['docId'] == i]
 
-                # concatenate all the properties ------------------------------------
+                # concatenate all the proberties ------------------------------------
                 count_sents.append(len(rows))
-
                 # all_passives 
                 count_passive_s = sum(rows.binary)
                 passive_sents_count.append(count_passive_s)
                 passive_percentages.append(count_passive_s/ len(rows))
 
                 # binary will be =1 if there is even one 1 
                 if any(rows.binary) == 1: binary.append(1)
@@ -550,36 +560,35 @@
                         ]
 
 
             # put all properties in a df ------------------------------------------------------
             
             for element in columns:
                 # name of variables will be the name of columns 
-                element_name = [ k for k,v in locals().items() if v is element ][0]
+                element_name = [ k for k,v in locals().items() if v is element][0]
                 output_dict[str(element_name)] = pd.Series(element, dtype='object')
 
             df_output = pd.DataFrame(output_dict)
                
             # add other columns in the initial df -------------------------------------------
-            if len(df.columns) == 1: 
-                add_other_columns=False
-
-            if add_other_columns:
+            if add_other_columns==True:
                 
                 # create a list of all the col names
                 fields = df.columns.tolist()
 
                 # remove column_name
                 del fields[fields.index(column_name)]
 
                 assert len(df[fields]) == len(df_output)
+
                 df_output = pd.concat([df_output, df[fields]], axis = 1)
             
             return df_output
 
+
 # for stopping the print statements in one sample sentences
 class HiddenPrints:
     def __enter__(self):
         self._original_stdout = sys.stdout
         sys.stdout = open(os.devnull, 'w')
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `PassivePy-0.2.22/PassivePyCode/PassivePySrc/rules_for_all_passives.py` & `PassivePy-0.2.3/PassivePyCode/PassivePySrc/rules_for_all_passives.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,260 +1,276 @@
-00000000: 0d0a 2320 2043 6f70 7972 6967 6874 204d  ..#  Copyright M
-00000010: 6974 7261 204d 6972 7368 6166 6965 652c  itra Mirshafiee,
-00000020: 2032 3032 3220 4c69 6365 6e73 6564 2075   2022 Licensed u
-00000030: 6e64 6572 204d 4954 204c 6963 656e 7365  nder MIT License
-00000040: 2e0d 0a23 2020 5365 6520 7468 6520 4c49  ...#  See the LI
-00000050: 4345 4e53 452e 7478 7420 666f 7220 6d6f  CENSE.txt for mo
-00000060: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e0d  re information..
-00000070: 0a0d 0a69 6d70 6f72 7420 7370 6163 790d  ...import spacy.
-00000080: 0a66 726f 6d20 7370 6163 792e 6d61 7463  .from spacy.matc
-00000090: 6865 7220 696d 706f 7274 204d 6174 6368  her import Match
-000000a0: 6572 0d0a 0d0a 6465 6620 6372 6561 7465  er....def create
-000000b0: 5f6d 6174 6368 6572 2873 7061 6379 5f6d  _matcher(spacy_m
-000000c0: 6f64 656c 203d 2022 656e 5f63 6f72 655f  odel = "en_core_
-000000d0: 7765 625f 6c67 222c 206e 6c70 3a73 7061  web_lg", nlp:spa
-000000e0: 6379 2e6c 616e 6775 6167 652e 4c61 6e67  cy.language.Lang
-000000f0: 7561 6765 203d 204e 6f6e 6529 3a0d 0a0d  uage = None):...
-00000100: 0a20 2020 2022 2222 0d0a 2020 2020 6372  .    """..    cr
-00000110: 6561 7465 7320 6120 6d61 7463 6865 7220  eates a matcher 
-00000120: 7769 7468 2061 2053 7061 4379 206e 6c70  with a SpaCy nlp
-00000130: 206d 6f64 656c 2e20 5468 6520 6465 6661   model. The defa
-00000140: 756c 7420 6d6f 6465 6c20 6973 3a0d 0a20  ult model is:.. 
-00000150: 2020 2068 7474 7073 3a2f 2f73 7061 6379     https://spacy
-00000160: 2e69 6f2f 6d6f 6465 6c73 2f65 6e23 656e  .io/models/en#en
-00000170: 5f63 6f72 655f 7765 625f 6c67 0d0a 2020  _core_web_lg..  
-00000180: 2020 0d0a 2020 2020 2222 220d 0a20 2020    ..    """..   
-00000190: 2069 6620 6e6f 7420 6e6c 703a 0d0a 2020   if not nlp:..  
-000001a0: 2020 2020 2020 6e6c 7020 3d20 7370 6163        nlp = spac
-000001b0: 792e 6c6f 6164 2873 7061 6379 5f6d 6f64  y.load(spacy_mod
-000001c0: 656c 2c20 6469 7361 626c 653d 5b22 6e65  el, disable=["ne
-000001d0: 7222 5d29 0d0a 2020 2020 6d61 7463 6865  r"])..    matche
-000001e0: 7220 3d20 4d61 7463 6865 7228 6e6c 702e  r = Matcher(nlp.
-000001f0: 766f 6361 6229 0d0a 0d0a 2020 2020 2320  vocab)....    # 
-00000200: 6c69 7374 206f 6620 7665 7262 7320 7468  list of verbs th
-00000210: 6174 2074 6865 6972 2061 646a 6563 7469  at their adjecti
-00000220: 7665 2066 6f72 6d20 0d0a 2020 2020 2320  ve form ..    # 
-00000230: 6973 2073 6f6d 6574 696d 6573 206d 6973  is sometimes mis
-00000240: 7461 6b65 6e20 6173 2061 2076 6572 620d  taken as a verb.
-00000250: 0a20 2020 2076 6572 6273 5f6c 6973 7420  .    verbs_list 
-00000260: 3d20 5b22 6173 736f 6369 6174 6522 2c20  = ["associate", 
-00000270: 2269 6e76 6f6c 7665 222c 2022 6578 6861  "involve", "exha
-00000280: 7573 7422 2c20 2262 6173 6522 2c20 0d0a  ust", "base", ..
-00000290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002a0: 226c 6561 6422 2c20 2273 7475 6e22 2c20  "lead", "stun", 
-000002b0: 226f 7665 7272 6174 6522 2c20 2022 6669  "overrate",  "fi
-000002c0: 6c6c 222c 2022 6265 6172 222c 0d0a 2020  ll", "bear",..  
-000002d0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-000002e0: 6f6d 706c 6963 6174 6522 2c20 2272 6573  omplicate", "res
-000002f0: 6572 7665 222c 2022 636f 6d70 6c69 6361  erve", "complica
-00000300: 7465 222c 2022 6865 6174 222c 0d0a 2020  te", "heat",..  
-00000310: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00000320: 6372 6577 222c 5d0d 0a0d 0a20 2020 2023  crew",]....    #
-00000330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000340: 2d2d 2d2d 2d2d 2d2d 2d2d 7275 6c65 732d  ----------rules-
-00000350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000360: 2d2d 2d23 0d0a 0d0a 2020 2020 0d0a 2020  ---#....    ..  
-00000370: 2020 7061 7373 6976 655f 7275 6c65 5f31    passive_rule_1
-00000380: 203d 205b 0d0a 2020 2020 2020 2020 7b22   = [..        {"
-00000390: 504f 5322 3a22 4155 5822 2c20 2244 4550  POS":"AUX", "DEP
-000003a0: 223a 2022 6175 7822 2c20 224f 5022 3a22  ": "aux", "OP":"
-000003b0: 2a22 7d2c 0d0a 2020 2020 2020 2020 7b22  *"},..        {"
-000003c0: 504f 5322 3a22 4155 5822 2c20 2244 4550  POS":"AUX", "DEP
-000003d0: 223a 2022 6175 7870 6173 7322 2c20 224f  ": "auxpass", "O
-000003e0: 5022 3a22 2b22 7d2c 0d0a 2020 2020 2020  P":"+"},..      
-000003f0: 2020 7b22 4445 5022 3a22 6e65 6722 2c20    {"DEP":"neg", 
-00000400: 2254 4147 223a 2252 4222 2c20 224f 5022  "TAG":"RB", "OP"
-00000410: 3a22 2a22 7d2c 0d0a 2020 2020 2020 2020  :"*"},..        
-00000420: 7b22 4445 5022 3a22 4859 5048 222c 2022  {"DEP":"HYPH", "
-00000430: 4f50 223a 222a 227d 2c0d 0a20 2020 2020  OP":"*"},..     
-00000440: 2020 207b 2244 4550 223a 2261 6476 6d6f     {"DEP":"advmo
-00000450: 6422 2c20 2254 4147 223a 2252 4222 2c20  d", "TAG":"RB", 
-00000460: 224f 5022 3a22 2a22 7d2c 0d0a 2020 2020  "OP":"*"},..    
-00000470: 2020 2020 7b22 504f 5322 3a22 5645 5242      {"POS":"VERB
-00000480: 222c 2022 5441 4722 3a22 5642 4e22 2c20  ", "TAG":"VBN", 
-00000490: 224c 454d 4d41 223a 7b22 4e4f 545f 494e  "LEMMA":{"NOT_IN
-000004a0: 2220 3a20 7665 7262 735f 6c69 7374 202b  " : verbs_list +
-000004b0: 205b 2762 6527 5d7d 7d0d 0a20 2020 205d   ['be']}}..    ]
-000004c0: 0d0a 0d0a 2020 2020 2222 220d 0a20 2020  ....    """..   
-000004d0: 2073 656e 7465 6e63 6520 3a20 5468 6520   sentence : The 
-000004e0: 626f 6f6b 2077 6173 2072 6561 6420 6279  book was read by
-000004f0: 2068 696d 2e0d 0a20 2020 2064 6570 656e   him...    depen
-00000500: 6465 6e63 6965 7320 3a20 5b27 6465 7427  dencies : ['det'
-00000510: 2c20 276e 7375 626a 7061 7373 272c 2027  , 'nsubjpass', '
-00000520: 6175 7870 6173 7327 2c20 2752 4f4f 5427  auxpass', 'ROOT'
-00000530: 2c20 2761 6765 6e74 272c 2027 706f 626a  , 'agent', 'pobj
-00000540: 272c 2027 7075 6e63 7427 5d0d 0a20 2020  ', 'punct']..   
-00000550: 2054 6167 7320 3a20 5b27 4454 272c 2027   Tags : ['DT', '
-00000560: 4e4e 272c 2027 5642 4427 2c20 2756 424e  NN', 'VBD', 'VBN
-00000570: 272c 2027 494e 272c 2027 5052 5027 2c20  ', 'IN', 'PRP', 
-00000580: 272e 275d 0d0a 2020 2020 2222 220d 0a20  '.']..    """.. 
-00000590: 2020 2070 6173 7369 7665 5f72 756c 655f     passive_rule_
-000005a0: 3220 3d20 5b0d 0a20 2020 2020 2020 207b  2 = [..        {
-000005b0: 2244 4550 223a 207b 2249 4e22 3a20 5b22  "DEP": {"IN": ["
-000005c0: 6174 7472 222c 2027 6e73 7562 6a70 6173  attr", 'nsubjpas
-000005d0: 7327 2c20 2761 7070 6f73 275d 7d7d 2c0d  s', 'appos']}},.
-000005e0: 0a20 2020 2020 2020 207b 2254 4147 223a  .        {"TAG":
-000005f0: 2022 5242 222c 2022 4445 5022 3a20 2261   "RB", "DEP": "a
-00000600: 6476 6d6f 6422 2c20 224f 5022 203a 2022  dvmod", "OP" : "
-00000610: 2a22 7d2c 0d0a 2020 2020 2020 2020 7b22  *"},..        {"
-00000620: 4445 5022 3a20 2250 554e 4354 222c 2022  DEP": "PUNCT", "
-00000630: 4f50 2220 3a20 222a 227d 2c0d 0a20 2020  OP" : "*"},..   
-00000640: 2020 2020 207b 2254 4147 223a 2022 5642       {"TAG": "VB
-00000650: 4e22 2c20 2244 4550 223a 2022 6163 6c22  N", "DEP": "acl"
-00000660: 2c22 4c45 4d4d 4122 3a20 7b22 4e4f 545f  ,"LEMMA": {"NOT_
-00000670: 494e 2220 3a20 7665 7262 735f 6c69 7374  IN" : verbs_list
-00000680: 7d7d 0d0a 2020 2020 5d0d 0a0d 0a20 2020  }}..    ]....   
-00000690: 2022 2222 0d0a 2020 2020 7365 6e74 656e   """..    senten
-000006a0: 6365 203a 2074 6865 7265 2077 6173 206e  ce : there was n
-000006b0: 6f20 6368 616e 6765 2064 6574 6563 7465  o change detecte
-000006c0: 6420 696e 2068 6572 2062 6568 6176 696f  d in her behavio
-000006d0: 722e 0d0a 2020 2020 6465 7065 6e64 656e  r...    dependen
-000006e0: 6369 6573 203a 205b 2765 7870 6c27 2c20  cies : ['expl', 
-000006f0: 2752 4f4f 5427 2c20 2764 6574 272c 2027  'ROOT', 'det', '
-00000700: 6174 7472 272c 2027 6163 6c27 2c20 2770  attr', 'acl', 'p
-00000710: 7265 7027 2c20 2770 6f73 7327 2c20 2770  rep', 'poss', 'p
-00000720: 6f62 6a27 2c20 2770 756e 6374 275d 0d0a  obj', 'punct']..
-00000730: 2020 2020 7461 6773 203a 205b 2745 5827      tags : ['EX'
-00000740: 2c20 2756 4244 272c 2027 4454 272c 2027  , 'VBD', 'DT', '
-00000750: 4e4e 272c 2027 5642 4e27 2c20 2749 4e27  NN', 'VBN', 'IN'
-00000760: 2c20 2750 5250 2427 2c20 274e 4e27 2c20  , 'PRP$', 'NN', 
-00000770: 272e 275d 0d0a 2020 2020 2222 220d 0a0d  '.']..    """...
-00000780: 0a0d 0a20 2020 2070 6173 7369 7665 5f72  ...    passive_r
-00000790: 756c 655f 3320 3d20 5b0d 0a20 2020 2020  ule_3 = [..     
-000007a0: 2020 207b 2250 4f53 223a 2241 5558 222c     {"POS":"AUX",
-000007b0: 2022 4445 5022 3a20 2261 7578 222c 2022   "DEP": "aux", "
-000007c0: 4f50 223a 222a 227d 2c0d 0a20 2020 2020  OP":"*"},..     
-000007d0: 2020 207b 2250 4f53 223a 2241 5558 222c     {"POS":"AUX",
-000007e0: 2022 4445 5022 3a20 2261 7578 7061 7373   "DEP": "auxpass
-000007f0: 222c 2022 4f50 223a 222b 227d 2c0d 0a20  ", "OP":"+"},.. 
-00000800: 2020 2020 2020 207b 2244 4550 223a 226e         {"DEP":"n
-00000810: 6567 222c 2022 5441 4722 3a22 5242 222c  eg", "TAG":"RB",
-00000820: 2022 4f50 223a 222a 227d 2c0d 0a20 2020   "OP":"*"},..   
-00000830: 2020 2020 207b 2244 4550 223a 2248 5950       {"DEP":"HYP
-00000840: 4822 2c20 224f 5022 3a22 2a22 7d2c 0d0a  H", "OP":"*"},..
-00000850: 2020 2020 2020 2020 7b22 4445 5022 3a22          {"DEP":"
-00000860: 6164 766d 6f64 222c 2022 5441 4722 3a22  advmod", "TAG":"
-00000870: 5242 222c 2022 4f50 223a 222a 227d 2c0d  RB", "OP":"*"},.
-00000880: 0a20 2020 2020 2020 207b 2250 4f53 223a  .        {"POS":
-00000890: 2256 4552 4222 2c20 2244 4550 223a 2252  "VERB", "DEP":"R
-000008a0: 4f4f 5422 2c20 224c 454d 4d41 223a 7b22  OOT", "LEMMA":{"
-000008b0: 4e4f 545f 494e 2220 3a20 7665 7262 735f  NOT_IN" : verbs_
-000008c0: 6c69 7374 7d7d 2c0d 0a20 2020 2020 2020  list}},..       
-000008d0: 207b 2244 4550 223a 2263 6322 7d2c 0d0a   {"DEP":"cc"},..
-000008e0: 2020 2020 2020 2020 7b22 4445 5022 3a22          {"DEP":"
-000008f0: 6164 766d 6f64 222c 2022 5441 4722 3a22  advmod", "TAG":"
-00000900: 5642 4e22 2c20 224f 5022 3a20 222a 222c  VBN", "OP": "*",
-00000910: 2022 4c45 4d4d 4122 3a20 7b22 4e4f 545f   "LEMMA": {"NOT_
-00000920: 494e 223a 5b22 7072 6522 5d7d 7d2c 0d0a  IN":["pre"]}},..
-00000930: 2020 2020 2020 2020 7b22 4445 5022 3a20          {"DEP": 
-00000940: 2263 6f6e 6a22 2c20 224c 454d 4d41 223a  "conj", "LEMMA":
-00000950: 7b22 4e4f 545f 494e 2220 3a20 7665 7262  {"NOT_IN" : verb
-00000960: 735f 6c69 7374 7d7d 2c0d 0a20 2020 2020  s_list}},..     
-00000970: 2020 207b 2244 4550 223a 2270 6f62 6a22     {"DEP":"pobj"
-00000980: 2c20 224f 5022 3a22 2122 7d0d 0a20 2020  , "OP":"!"}..   
-00000990: 205d 0d0a 0d0a 2020 2020 2222 220d 0a20   ]....    """.. 
-000009a0: 2020 2055 7365 6420 666f 7220 7468 6520     Used for the 
-000009b0: 7365 636f 6e64 2070 6172 7420 7769 7468  second part with
-000009c0: 2022 616e 6420 2e2e 2e22 200d 0a20 2020   "and ..." ..   
-000009d0: 2073 656e 7465 6e63 6520 3a20 6974 2077   sentence : it w
-000009e0: 6173 2064 6574 6572 6d69 6e65 6420 616e  as determined an
-000009f0: 6420 666f 726d 6564 2e0d 0a20 2020 2064  d formed...    d
-00000a00: 6570 656e 6465 6e63 6965 7320 3a20 5b27  ependencies : ['
-00000a10: 6e73 7562 6a70 6173 7327 2c20 2761 7578  nsubjpass', 'aux
-00000a20: 7061 7373 272c 2027 524f 4f54 272c 2027  pass', 'ROOT', '
-00000a30: 6363 272c 2027 636f 6e6a 272c 2027 7075  cc', 'conj', 'pu
-00000a40: 6e63 7427 5d0d 0a20 2020 2074 6167 7320  nct']..    tags 
-00000a50: 3a20 5b27 5052 5027 2c20 2756 4244 272c  : ['PRP', 'VBD',
-00000a60: 2027 5642 4e27 2c20 2743 4327 2c20 2756   'VBN', 'CC', 'V
-00000a70: 424e 272c 2027 2e27 5d0d 0a20 2020 2022  BN', '.']..    "
-00000a80: 2222 0d0a 0d0a 2020 2020 7061 7373 6976  ""....    passiv
-00000a90: 655f 7275 6c65 5f34 203d 205b 0d0a 2020  e_rule_4 = [..  
-00000aa0: 2020 2020 2020 7b22 4445 5022 3a22 6164        {"DEP":"ad
-00000ab0: 7663 6c22 2c20 2254 4147 223a 2256 424e  vcl", "TAG":"VBN
-00000ac0: 227d 2c0d 0a20 2020 2020 2020 207b 2244  "},..        {"D
-00000ad0: 4550 223a 2022 6167 656e 7422 2c20 2254  EP": "agent", "T
-00000ae0: 4147 223a 2249 4e22 7d2c 0d0a 2020 2020  AG":"IN"},..    
-00000af0: 2020 2020 7b22 4f50 223a 222a 227d 2c0d      {"OP":"*"},.
-00000b00: 0a20 2020 2020 2020 207b 2244 4550 223a  .        {"DEP":
-00000b10: 2022 706f 626a 227d 2c0d 0a20 2020 205d   "pobj"},..    ]
-00000b20: 0d0a 0d0a 2020 2020 2222 220d 0a20 2020  ....    """..   
-00000b30: 2073 656e 7465 6e63 6520 3a20 6b69 6c6c   sentence : kill
-00000b40: 6564 2062 7920 7468 6520 706f 6c69 6365  ed by the police
-00000b50: 2c20 6865 206e 6576 6572 2074 686f 7567  , he never thoug
-00000b60: 6874 2074 6869 7320 776f 756c 6420 6265  ht this would be
-00000b70: 2068 6973 2065 6e64 2e0d 0a20 2020 2064   his end...    d
-00000b80: 6570 656e 6465 6e63 6965 7320 3a20 5b27  ependencies : ['
-00000b90: 6164 7663 6c27 2c20 2761 6765 6e74 272c  advcl', 'agent',
-00000ba0: 2027 6465 7427 2c20 2770 6f62 6a27 2c20   'det', 'pobj', 
-00000bb0: 2770 756e 6374 272c 2027 6e73 7562 6a27  'punct', 'nsubj'
-00000bc0: 2c20 276e 6567 272c 2027 524f 4f54 272c  , 'neg', 'ROOT',
-00000bd0: 2027 6e73 7562 6a27 2c20 2761 7578 272c   'nsubj', 'aux',
-00000be0: 2027 6363 6f6d 7027 2c20 2770 6f73 7327   'ccomp', 'poss'
-00000bf0: 2c20 2761 7474 7227 5d0d 0a20 2020 2074  , 'attr']..    t
-00000c00: 6167 7320 3a20 5b27 5642 4e27 2c20 2749  ags : ['VBN', 'I
-00000c10: 4e27 2c20 2744 5427 2c20 274e 4e27 2c20  N', 'DT', 'NN', 
-00000c20: 272c 272c 2027 5052 5027 2c20 2752 4227  ',', 'PRP', 'RB'
-00000c30: 2c20 2756 4244 272c 2027 4454 272c 2027  , 'VBD', 'DT', '
-00000c40: 4d44 272c 2027 5642 272c 2027 5052 5024  MD', 'VB', 'PRP$
-00000c50: 272c 2027 4e4e 275d 0d0a 2020 2020 2222  ', 'NN']..    ""
-00000c60: 220d 0a0d 0a0d 0a20 2020 2070 6173 7369  "......    passi
-00000c70: 7665 5f72 756c 655f 3520 3d20 5b0d 0a20  ve_rule_5 = [.. 
-00000c80: 2020 2020 2020 207b 224c 454d 4d41 223a         {"LEMMA":
-00000c90: 207b 2249 4e22 3a20 7665 7262 735f 6c69   {"IN": verbs_li
-00000ca0: 7374 7d7d 2c0d 0a20 2020 2020 2020 207b  st}},..        {
-00000cb0: 224c 4f57 4552 223a 2262 7922 7d0d 0a20  "LOWER":"by"}.. 
-00000cc0: 2020 205d 0d0a 0d0a 0d0a 2020 2020 2222     ]......    ""
-00000cd0: 220d 0a20 2020 2074 6f20 6176 6f69 6420  "..    to avoid 
-00000ce0: 7468 6520 636f 6e66 7573 696f 6e20 6265  the confusion be
-00000cf0: 7477 6565 6e20 7468 6520 6164 6a65 6374  tween the adject
-00000d00: 6976 6520 616e 6420 7061 7373 6976 6520  ive and passive 
-00000d10: 7665 7273 696f 6e20 6f66 2073 7065 6369  version of speci
-00000d20: 6669 6320 0d0a 2020 2020 7665 7262 732c  fic ..    verbs,
-00000d30: 2077 6520 6465 6469 6361 7465 6420 6120   we dedicated a 
-00000d40: 6e65 7720 7275 6c65 2074 6f20 736f 6d65  new rule to some
-00000d50: 2076 6572 6273 2074 6f20 6265 2064 6574   verbs to be det
-00000d60: 6563 7465 6420 7768 656e 2075 7365 6420  ected when used 
-00000d70: 7769 7468 200d 0a20 2020 2061 6e20 6167  with ..    an ag
-00000d80: 656e 7420 2862 7929 0d0a 0d0a 2020 2020  ent (by)....    
-00000d90: 7365 6e74 656e 6365 203a 204e 6174 7572  sentence : Natur
-00000da0: 616c 2072 6573 6f75 7263 6573 2061 7265  al resources are
-00000db0: 2065 7868 6175 7374 6564 2062 7920 6875   exhausted by hu
-00000dc0: 6d61 6e73 2e0d 0a20 2020 2064 6570 656e  mans...    depen
-00000dd0: 6465 6e63 6965 7320 3a20 5b27 616d 6f64  dencies : ['amod
-00000de0: 272c 2027 6e73 7562 6a70 6173 7327 2c20  ', 'nsubjpass', 
-00000df0: 2761 7578 7061 7373 272c 2027 524f 4f54  'auxpass', 'ROOT
-00000e00: 272c 2027 6167 656e 7427 2c20 2770 6f62  ', 'agent', 'pob
-00000e10: 6a27 5d0d 0a20 2020 2074 6167 7320 3a20  j']..    tags : 
-00000e20: 5b27 4a4a 272c 2027 4e4e 5327 2c20 2756  ['JJ', 'NNS', 'V
-00000e30: 4250 272c 2027 5642 4e27 2c20 2749 4e27  BP', 'VBN', 'IN'
-00000e40: 2c20 274e 4e53 275d 0d0a 2020 2020 2222  , 'NNS']..    ""
-00000e50: 220d 0a0d 0a0d 0a20 2020 2023 202d 2d2d  "......    # ---
-00000e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d61  ---------------a
-00000e70: 6464 696e 6720 7275 6c65 7320 746f 2074  dding rules to t
-00000e80: 6865 206d 6174 6368 6572 2d2d 2d2d 2d2d  he matcher------
-00000e90: 2d2d 2d2d 230d 0a0d 0a20 2020 206d 6174  ----#....    mat
-00000ea0: 6368 6572 2e61 6464 2822 7061 7373 6976  cher.add("passiv
-00000eb0: 655f 7275 6c65 5f31 222c 205b 7061 7373  e_rule_1", [pass
-00000ec0: 6976 655f 7275 6c65 5f31 5d2c 2067 7265  ive_rule_1], gre
-00000ed0: 6564 793d 274c 4f4e 4745 5354 2729 0d0a  edy='LONGEST')..
-00000ee0: 2020 2020 6d61 7463 6865 722e 6164 6428      matcher.add(
-00000ef0: 2270 6173 7369 7665 5f72 756c 655f 3222  "passive_rule_2"
-00000f00: 2c20 5b70 6173 7369 7665 5f72 756c 655f  , [passive_rule_
-00000f10: 325d 2c20 6772 6565 6479 3d27 4c4f 4e47  2], greedy='LONG
-00000f20: 4553 5427 290d 0a20 2020 206d 6174 6368  EST')..    match
-00000f30: 6572 2e61 6464 2822 7061 7373 6976 655f  er.add("passive_
-00000f40: 7275 6c65 5f33 222c 205b 7061 7373 6976  rule_3", [passiv
-00000f50: 655f 7275 6c65 5f33 5d2c 2067 7265 6564  e_rule_3], greed
-00000f60: 793d 274c 4f4e 4745 5354 2729 0d0a 2020  y='LONGEST')..  
-00000f70: 2020 6d61 7463 6865 722e 6164 6428 2270    matcher.add("p
-00000f80: 6173 7369 7665 5f72 756c 655f 3422 2c20  assive_rule_4", 
-00000f90: 5b70 6173 7369 7665 5f72 756c 655f 345d  [passive_rule_4]
-00000fa0: 2c20 6772 6565 6479 3d27 4c4f 4e47 4553  , greedy='LONGES
-00000fb0: 5427 290d 0a20 2020 206d 6174 6368 6572  T')..    matcher
-00000fc0: 2e61 6464 2822 7061 7373 6976 655f 7275  .add("passive_ru
-00000fd0: 6c65 5f35 222c 205b 7061 7373 6976 655f  le_5", [passive_
-00000fe0: 7275 6c65 5f35 5d2c 2067 7265 6564 793d  rule_5], greedy=
-00000ff0: 274c 4f4e 4745 5354 2729 0d0a 0d0a 2020  'LONGEST')....  
-00001000: 2020 2320 7072 696e 7428 274d 6174 6368    # print('Match
-00001010: 6572 2069 7320 6275 696c 742e 2729 0d0a  er is built.')..
-00001020: 0d0a 2020 2020 7265 7475 726e 206e 6c70  ..    return nlp
-00001030: 2c20 6d61 7463 6865 72                   , matcher
+00000000: 696d 706f 7274 2073 7061 6379 0d0a 6672  import spacy..fr
+00000010: 6f6d 2073 7061 6379 2e6d 6174 6368 6572  om spacy.matcher
+00000020: 2069 6d70 6f72 7420 4d61 7463 6865 720d   import Matcher.
+00000030: 0a0d 0a0d 0a0d 0a64 6566 2063 7265 6174  .......def creat
+00000040: 655f 6d61 7463 6865 7228 7370 6163 795f  e_matcher(spacy_
+00000050: 6d6f 6465 6c20 3d20 2265 6e5f 636f 7265  model = "en_core
+00000060: 5f77 6562 5f6c 6722 293a 0d0a 0d0a 2020  _web_lg"):....  
+00000070: 2020 2222 2263 7265 6174 6573 2061 206d    """creates a m
+00000080: 6174 6368 6572 206f 6e20 7468 6520 666f  atcher on the fo
+00000090: 6c6c 6f77 696e 6720 766f 6361 6275 6c61  llowing vocabula
+000000a0: 7279 2222 220d 0a20 2020 206e 6c70 203d  ry"""..    nlp =
+000000b0: 2073 7061 6379 2e6c 6f61 6428 7370 6163   spacy.load(spac
+000000c0: 795f 6d6f 6465 6c2c 2064 6973 6162 6c65  y_model, disable
+000000d0: 3d5b 226e 6572 225d 290d 0a20 2020 206d  =["ner"])..    m
+000000e0: 6174 6368 6572 203d 204d 6174 6368 6572  atcher = Matcher
+000000f0: 286e 6c70 2e76 6f63 6162 290d 0a0d 0a20  (nlp.vocab).... 
+00000100: 2020 2023 206c 6973 7420 6f66 2076 6572     # list of ver
+00000110: 6273 2074 6861 7420 7468 6569 7220 6164  bs that their ad
+00000120: 6a65 6374 6976 6520 666f 726d 200d 0a20  jective form .. 
+00000130: 2020 2023 2069 7320 736f 6d65 7469 6d65     # is sometime
+00000140: 7320 6d69 7374 616b 656e 2061 7320 6120  s mistaken as a 
+00000150: 7665 7262 0d0a 2020 2020 7665 7262 735f  verb..    verbs_
+00000160: 6c69 7374 203d 205b 2261 7373 6f63 6961  list = ["associa
+00000170: 7465 222c 2022 696e 766f 6c76 6522 2c20  te", "involve", 
+00000180: 2265 7868 6175 7374 222c 2022 6261 7365  "exhaust", "base
+00000190: 222c 200d 0a20 2020 2020 2020 2020 2020  ", ..           
+000001a0: 2020 2020 2022 6c65 6164 222c 2022 7374       "lead", "st
+000001b0: 756e 222c 2022 6f76 6572 7261 7465 222c  un", "overrate",
+000001c0: 2020 2266 696c 6c22 2c20 2262 6561 7222    "fill", "bear"
+000001d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000001e0: 2020 2022 636f 6d70 6c69 6361 7465 222c     "complicate",
+000001f0: 2022 7265 7365 7276 6522 2c20 2263 6f6d   "reserve", "com
+00000200: 706c 6963 6174 6522 2c20 2268 6561 7422  plicate", "heat"
+00000210: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000220: 2020 2022 7363 7265 7722 2c5d 0d0a 0d0a     "screw",]....
+00000230: 2020 2020 232d 2d2d 2d2d 2d2d 2d2d 2d2d      #-----------
+00000240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d72  ---------------r
+00000250: 756c 6573 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ules------------
+00000260: 2d2d 2d2d 2d2d 2d2d 230d 0a0d 0a20 2020  --------#....   
+00000270: 200d 0a20 2020 2070 6173 7369 7665 5f72   ..    passive_r
+00000280: 756c 655f 3120 3d20 5b0d 0a20 2020 2020  ule_1 = [..     
+00000290: 2020 207b 2250 4f53 223a 2241 5558 222c     {"POS":"AUX",
+000002a0: 2022 4445 5022 3a20 2261 7578 222c 2022   "DEP": "aux", "
+000002b0: 4f50 223a 222a 227d 2c0d 0a20 2020 2020  OP":"*"},..     
+000002c0: 2020 207b 2250 4f53 223a 2241 5558 222c     {"POS":"AUX",
+000002d0: 2022 4445 5022 3a20 2261 7578 7061 7373   "DEP": "auxpass
+000002e0: 222c 2022 4f50 223a 222b 227d 2c0d 0a20  ", "OP":"+"},.. 
+000002f0: 2020 2020 2020 207b 2244 4550 223a 226e         {"DEP":"n
+00000300: 6567 222c 2022 5441 4722 3a22 5242 222c  eg", "TAG":"RB",
+00000310: 2022 4f50 223a 222a 227d 2c0d 0a20 2020   "OP":"*"},..   
+00000320: 2020 2020 207b 2244 4550 223a 2248 5950       {"DEP":"HYP
+00000330: 4822 2c20 224f 5022 3a22 2a22 7d2c 0d0a  H", "OP":"*"},..
+00000340: 2020 2020 2020 2020 7b22 4445 5022 3a22          {"DEP":"
+00000350: 6164 766d 6f64 222c 2022 5441 4722 3a22  advmod", "TAG":"
+00000360: 5242 222c 2022 4f50 223a 222a 227d 2c0d  RB", "OP":"*"},.
+00000370: 0a20 2020 2020 2020 207b 2250 4f53 223a  .        {"POS":
+00000380: 2256 4552 4222 2c20 2254 4147 223a 2256  "VERB", "TAG":"V
+00000390: 424e 222c 2022 4c45 4d4d 4122 3a7b 224e  BN", "LEMMA":{"N
+000003a0: 4f54 5f49 4e22 203a 2076 6572 6273 5f6c  OT_IN" : verbs_l
+000003b0: 6973 7420 2b20 5b27 6265 275d 7d7d 0d0a  ist + ['be']}}..
+000003c0: 2020 2020 5d0d 0a0d 0a20 2020 2022 2222      ]....    """
+000003d0: 0d0a 2020 2020 7365 6e74 656e 6365 203a  ..    sentence :
+000003e0: 2054 6865 2062 6f6f 6b20 7761 7320 7265   The book was re
+000003f0: 6164 2062 7920 6869 6d2e 0d0a 2020 2020  ad by him...    
+00000400: 6465 7065 6e64 656e 6369 6573 203a 205b  dependencies : [
+00000410: 2764 6574 272c 2027 6e73 7562 6a70 6173  'det', 'nsubjpas
+00000420: 7327 2c20 2761 7578 7061 7373 272c 2027  s', 'auxpass', '
+00000430: 524f 4f54 272c 2027 6167 656e 7427 2c20  ROOT', 'agent', 
+00000440: 2770 6f62 6a27 2c20 2770 756e 6374 275d  'pobj', 'punct']
+00000450: 0d0a 2020 2020 5461 6773 203a 205b 2744  ..    Tags : ['D
+00000460: 5427 2c20 274e 4e27 2c20 2756 4244 272c  T', 'NN', 'VBD',
+00000470: 2027 5642 4e27 2c20 2749 4e27 2c20 2750   'VBN', 'IN', 'P
+00000480: 5250 272c 2027 2e27 5d0d 0a20 2020 2022  RP', '.']..    "
+00000490: 2222 0d0a 2020 2020 7061 7373 6976 655f  ""..    passive_
+000004a0: 7275 6c65 5f32 203d 205b 0d0a 2020 2020  rule_2 = [..    
+000004b0: 2020 2020 7b22 4445 5022 3a20 7b22 494e      {"DEP": {"IN
+000004c0: 223a 205b 2261 7474 7222 2c20 276e 7375  ": ["attr", 'nsu
+000004d0: 626a 7061 7373 272c 2027 6170 706f 7327  bjpass', 'appos'
+000004e0: 5d7d 7d2c 0d0a 2020 2020 2020 2020 7b22  ]}},..        {"
+000004f0: 5441 4722 3a20 2252 4222 2c20 2244 4550  TAG": "RB", "DEP
+00000500: 223a 2022 6164 766d 6f64 222c 2022 4f50  ": "advmod", "OP
+00000510: 2220 3a20 222a 227d 2c0d 0a20 2020 2020  " : "*"},..     
+00000520: 2020 207b 2244 4550 223a 2022 5055 4e43     {"DEP": "PUNC
+00000530: 5422 2c20 224f 5022 203a 2022 2a22 7d2c  T", "OP" : "*"},
+00000540: 0d0a 2020 2020 2020 2020 7b22 5441 4722  ..        {"TAG"
+00000550: 3a20 2256 424e 222c 2022 4445 5022 3a20  : "VBN", "DEP": 
+00000560: 2261 636c 222c 224c 454d 4d41 223a 207b  "acl","LEMMA": {
+00000570: 224e 4f54 5f49 4e22 203a 2076 6572 6273  "NOT_IN" : verbs
+00000580: 5f6c 6973 747d 7d0d 0a20 2020 205d 0d0a  _list}}..    ]..
+00000590: 0d0a 2020 2020 2222 220d 0a20 2020 2073  ..    """..    s
+000005a0: 656e 7465 6e63 6520 3a20 7468 6572 6520  entence : there 
+000005b0: 7761 7320 6e6f 2063 6861 6e67 6520 6465  was no change de
+000005c0: 7465 6374 6564 2069 6e20 6865 7220 6265  tected in her be
+000005d0: 6861 7669 6f72 2e0d 0a20 2020 2064 6570  havior...    dep
+000005e0: 656e 6465 6e63 6965 7320 3a20 5b27 6578  endencies : ['ex
+000005f0: 706c 272c 2027 524f 4f54 272c 2027 6465  pl', 'ROOT', 'de
+00000600: 7427 2c20 2761 7474 7227 2c20 2761 636c  t', 'attr', 'acl
+00000610: 272c 2027 7072 6570 272c 2027 706f 7373  ', 'prep', 'poss
+00000620: 272c 2027 706f 626a 272c 2027 7075 6e63  ', 'pobj', 'punc
+00000630: 7427 5d0d 0a20 2020 2074 6167 7320 3a20  t']..    tags : 
+00000640: 5b27 4558 272c 2027 5642 4427 2c20 2744  ['EX', 'VBD', 'D
+00000650: 5427 2c20 274e 4e27 2c20 2756 424e 272c  T', 'NN', 'VBN',
+00000660: 2027 494e 272c 2027 5052 5024 272c 2027   'IN', 'PRP$', '
+00000670: 4e4e 272c 2027 2e27 5d0d 0a20 2020 2022  NN', '.']..    "
+00000680: 2222 0d0a 0d0a 0d0a 2020 2020 7061 7373  ""......    pass
+00000690: 6976 655f 7275 6c65 5f33 203d 205b 0d0a  ive_rule_3 = [..
+000006a0: 2020 2020 2020 2020 7b22 504f 5322 3a22          {"POS":"
+000006b0: 4155 5822 2c20 2244 4550 223a 2022 6175  AUX", "DEP": "au
+000006c0: 7822 2c20 224f 5022 3a22 2a22 7d2c 0d0a  x", "OP":"*"},..
+000006d0: 2020 2020 2020 2020 7b22 504f 5322 3a22          {"POS":"
+000006e0: 4155 5822 2c20 2244 4550 223a 2022 6175  AUX", "DEP": "au
+000006f0: 7870 6173 7322 2c20 224f 5022 3a22 2b22  xpass", "OP":"+"
+00000700: 7d2c 0d0a 2020 2020 2020 2020 7b22 4445  },..        {"DE
+00000710: 5022 3a22 6e65 6722 2c20 2254 4147 223a  P":"neg", "TAG":
+00000720: 2252 4222 2c20 224f 5022 3a22 2a22 7d2c  "RB", "OP":"*"},
+00000730: 0d0a 2020 2020 2020 2020 7b22 4445 5022  ..        {"DEP"
+00000740: 3a22 4859 5048 222c 2022 4f50 223a 222a  :"HYPH", "OP":"*
+00000750: 227d 2c0d 0a20 2020 2020 2020 207b 2244  "},..        {"D
+00000760: 4550 223a 2261 6476 6d6f 6422 2c20 2254  EP":"advmod", "T
+00000770: 4147 223a 2252 4222 2c20 224f 5022 3a22  AG":"RB", "OP":"
+00000780: 2a22 7d2c 0d0a 2020 2020 2020 2020 7b22  *"},..        {"
+00000790: 504f 5322 3a22 5645 5242 222c 2022 4445  POS":"VERB", "DE
+000007a0: 5022 3a22 524f 4f54 222c 2022 4c45 4d4d  P":"ROOT", "LEMM
+000007b0: 4122 3a7b 224e 4f54 5f49 4e22 203a 2076  A":{"NOT_IN" : v
+000007c0: 6572 6273 5f6c 6973 747d 7d2c 0d0a 2020  erbs_list}},..  
+000007d0: 2020 2020 2020 7b22 4445 5022 3a22 6363        {"DEP":"cc
+000007e0: 227d 2c0d 0a20 2020 2020 2020 207b 2244  "},..        {"D
+000007f0: 4550 223a 2261 6476 6d6f 6422 2c20 2254  EP":"advmod", "T
+00000800: 4147 223a 2256 424e 222c 2022 4f50 223a  AG":"VBN", "OP":
+00000810: 2022 2a22 2c20 224c 454d 4d41 223a 207b   "*", "LEMMA": {
+00000820: 224e 4f54 5f49 4e22 3a5b 2270 7265 225d  "NOT_IN":["pre"]
+00000830: 7d7d 2c0d 0a20 2020 2020 2020 207b 2244  }},..        {"D
+00000840: 4550 223a 2022 636f 6e6a 222c 2022 4c45  EP": "conj", "LE
+00000850: 4d4d 4122 3a7b 224e 4f54 5f49 4e22 203a  MMA":{"NOT_IN" :
+00000860: 2076 6572 6273 5f6c 6973 747d 7d2c 0d0a   verbs_list}},..
+00000870: 2020 2020 2020 2020 7b22 4445 5022 3a22          {"DEP":"
+00000880: 706f 626a 222c 2022 4f50 223a 2221 227d  pobj", "OP":"!"}
+00000890: 0d0a 2020 2020 5d0d 0a0d 0a20 2020 2022  ..    ]....    "
+000008a0: 2222 0d0a 2020 2020 5573 6564 2066 6f72  ""..    Used for
+000008b0: 2074 6865 2073 6563 6f6e 6420 7061 7274   the second part
+000008c0: 2077 6974 6820 2261 6e64 202e 2e2e 2220   with "and ..." 
+000008d0: 0d0a 2020 2020 7365 6e74 656e 6365 203a  ..    sentence :
+000008e0: 2069 7420 7761 7320 6465 7465 726d 696e   it was determin
+000008f0: 6564 2061 6e64 2066 6f72 6d65 642e 0d0a  ed and formed...
+00000900: 2020 2020 6465 7065 6e64 656e 6369 6573      dependencies
+00000910: 203a 205b 276e 7375 626a 7061 7373 272c   : ['nsubjpass',
+00000920: 2027 6175 7870 6173 7327 2c20 2752 4f4f   'auxpass', 'ROO
+00000930: 5427 2c20 2763 6327 2c20 2763 6f6e 6a27  T', 'cc', 'conj'
+00000940: 2c20 2770 756e 6374 275d 0d0a 2020 2020  , 'punct']..    
+00000950: 7461 6773 203a 205b 2750 5250 272c 2027  tags : ['PRP', '
+00000960: 5642 4427 2c20 2756 424e 272c 2027 4343  VBD', 'VBN', 'CC
+00000970: 272c 2027 5642 4e27 2c20 272e 275d 0d0a  ', 'VBN', '.']..
+00000980: 2020 2020 2222 220d 0a0d 0a20 2020 2070      """....    p
+00000990: 6173 7369 7665 5f72 756c 655f 3420 3d20  assive_rule_4 = 
+000009a0: 5b0d 0a20 2020 2020 2020 207b 2244 4550  [..        {"DEP
+000009b0: 223a 2261 6476 636c 222c 2022 5441 4722  ":"advcl", "TAG"
+000009c0: 3a22 5642 4e22 7d2c 0d0a 2020 2020 2020  :"VBN"},..      
+000009d0: 2020 7b22 4445 5022 3a20 2261 6765 6e74    {"DEP": "agent
+000009e0: 222c 2022 5441 4722 3a22 494e 227d 2c0d  ", "TAG":"IN"},.
+000009f0: 0a20 2020 2020 2020 207b 224f 5022 3a22  .        {"OP":"
+00000a00: 2a22 7d2c 0d0a 2020 2020 2020 2020 7b22  *"},..        {"
+00000a10: 4445 5022 3a20 2270 6f62 6a22 7d2c 0d0a  DEP": "pobj"},..
+00000a20: 2020 2020 5d0d 0a0d 0a20 2020 2022 2222      ]....    """
+00000a30: 0d0a 2020 2020 7365 6e74 656e 6365 203a  ..    sentence :
+00000a40: 206b 696c 6c65 6420 6279 2074 6865 2070   killed by the p
+00000a50: 6f6c 6963 652c 2068 6520 6e65 7665 7220  olice, he never 
+00000a60: 7468 6f75 6768 7420 7468 6973 2077 6f75  thought this wou
+00000a70: 6c64 2062 6520 6869 7320 656e 642e 0d0a  ld be his end...
+00000a80: 2020 2020 6465 7065 6e64 656e 6369 6573      dependencies
+00000a90: 203a 205b 2761 6476 636c 272c 2027 6167   : ['advcl', 'ag
+00000aa0: 656e 7427 2c20 2764 6574 272c 2027 706f  ent', 'det', 'po
+00000ab0: 626a 272c 2027 7075 6e63 7427 2c20 276e  bj', 'punct', 'n
+00000ac0: 7375 626a 272c 2027 6e65 6727 2c20 2752  subj', 'neg', 'R
+00000ad0: 4f4f 5427 2c20 276e 7375 626a 272c 2027  OOT', 'nsubj', '
+00000ae0: 6175 7827 2c20 2763 636f 6d70 272c 2027  aux', 'ccomp', '
+00000af0: 706f 7373 272c 2027 6174 7472 275d 0d0a  poss', 'attr']..
+00000b00: 2020 2020 7461 6773 203a 205b 2756 424e      tags : ['VBN
+00000b10: 272c 2027 494e 272c 2027 4454 272c 2027  ', 'IN', 'DT', '
+00000b20: 4e4e 272c 2027 2c27 2c20 2750 5250 272c  NN', ',', 'PRP',
+00000b30: 2027 5242 272c 2027 5642 4427 2c20 2744   'RB', 'VBD', 'D
+00000b40: 5427 2c20 274d 4427 2c20 2756 4227 2c20  T', 'MD', 'VB', 
+00000b50: 2750 5250 2427 2c20 274e 4e27 5d0d 0a20  'PRP$', 'NN'].. 
+00000b60: 2020 2022 2222 0d0a 0d0a 2020 2020 7061     """....    pa
+00000b70: 7373 6976 655f 7275 6c65 5f35 203d 205b  ssive_rule_5 = [
+00000b80: 0d0a 2020 2020 2020 2020 7b22 4445 5022  ..        {"DEP"
+00000b90: 3a20 226e 7375 626a 227d 2c0d 0a20 2020  : "nsubj"},..   
+00000ba0: 2020 2020 207b 2244 4550 223a 2022 524f       {"DEP": "RO
+00000bb0: 4f54 227d 2c0d 0a20 2020 2020 2020 207b  OT"},..        {
+00000bc0: 2244 4550 223a 2022 6174 7472 222c 2022  "DEP": "attr", "
+00000bd0: 5441 4722 3a20 2256 424e 222c 2022 4c45  TAG": "VBN", "LE
+00000be0: 4d4d 4122 3a7b 224e 4f54 5f49 4e22 203a  MMA":{"NOT_IN" :
+00000bf0: 2076 6572 6273 5f6c 6973 747d 7d2c 0d0a   verbs_list}},..
+00000c00: 2020 2020 2020 2020 7b22 4445 5022 3a20          {"DEP": 
+00000c10: 2270 7265 7022 2c20 2254 4147 223a 2022  "prep", "TAG": "
+00000c20: 494e 222c 2022 4f50 223a 222a 227d 0d0a  IN", "OP":"*"}..
+00000c30: 2020 2020 5d0d 0a0d 0a20 2020 2022 2222      ]....    """
+00000c40: 0d0a 2020 2020 7365 6e74 656e 6365 203a  ..    sentence :
+00000c50: 2042 6561 7273 2061 7265 2064 7265 616d   Bears are dream
+00000c60: 7420 6f66 2069 6e20 796f 7572 2066 616e  t of in your fan
+00000c70: 7461 7369 6573 210d 0a20 2020 2064 6570  tasies!..    dep
+00000c80: 656e 6465 6e63 6965 7320 3a20 5b27 6e73  endencies : ['ns
+00000c90: 7562 6a70 6173 7327 2c20 2761 7578 7061  ubjpass', 'auxpa
+00000ca0: 7373 272c 2027 524f 4f54 272c 2027 7072  ss', 'ROOT', 'pr
+00000cb0: 6570 272c 2027 7072 6570 272c 2027 706f  ep', 'prep', 'po
+00000cc0: 7373 272c 2027 706f 626a 272c 2027 7075  ss', 'pobj', 'pu
+00000cd0: 6e63 7427 5d0d 0a20 2020 2074 6167 7320  nct']..    tags 
+00000ce0: 3a20 5b27 4e4e 5327 2c20 2756 4250 272c  : ['NNS', 'VBP',
+00000cf0: 2027 5642 4e27 2c20 2749 4e27 2c20 2749   'VBN', 'IN', 'I
+00000d00: 4e27 2c20 2750 5250 2427 2c20 274e 4e53  N', 'PRP$', 'NNS
+00000d10: 272c 2027 2e27 5d0d 0a20 2020 2022 2222  ', '.']..    """
+00000d20: 0d0a 0d0a 0d0a 2020 2020 7061 7373 6976  ......    passiv
+00000d30: 655f 7275 6c65 5f36 203d 205b 0d0a 2020  e_rule_6 = [..  
+00000d40: 2020 2020 2020 7b22 4c45 4d4d 4122 3a20        {"LEMMA": 
+00000d50: 7b22 494e 223a 2076 6572 6273 5f6c 6973  {"IN": verbs_lis
+00000d60: 747d 7d2c 0d0a 2020 2020 2020 2020 7b22  t}},..        {"
+00000d70: 4c4f 5745 5222 3a22 6279 227d 0d0a 2020  LOWER":"by"}..  
+00000d80: 2020 5d0d 0a0d 0a0d 0a20 2020 2022 2222    ]......    """
+00000d90: 0d0a 2020 2020 746f 2061 766f 6964 2074  ..    to avoid t
+00000da0: 6865 2063 6f6e 6675 7369 6f6e 2062 6574  he confusion bet
+00000db0: 7765 656e 2074 6865 2061 646a 6563 7469  ween the adjecti
+00000dc0: 7665 2061 6e64 2070 6173 7369 7665 2076  ve and passive v
+00000dd0: 6572 7369 6f6e 206f 6620 7370 6563 6966  ersion of specif
+00000de0: 6963 200d 0a20 2020 2076 6572 6273 2c20  ic ..    verbs, 
+00000df0: 7765 2064 6564 6963 6174 6564 2061 206e  we dedicated a n
+00000e00: 6577 2072 756c 6520 746f 2073 6f6d 6520  ew rule to some 
+00000e10: 7665 7262 7320 746f 2062 6520 6465 7465  verbs to be dete
+00000e20: 6374 6564 2077 6865 6e20 7573 6564 2077  cted when used w
+00000e30: 6974 6820 0d0a 2020 2020 616e 2061 6765  ith ..    an age
+00000e40: 6e74 2028 6279 290d 0a0d 0a20 2020 2073  nt (by)....    s
+00000e50: 656e 7465 6e63 6520 3a20 4e61 7475 7261  entence : Natura
+00000e60: 6c20 7265 736f 7572 6365 7320 6172 6520  l resources are 
+00000e70: 6578 6861 7573 7465 6420 6279 2068 756d  exhausted by hum
+00000e80: 616e 732e 0d0a 2020 2020 6465 7065 6e64  ans...    depend
+00000e90: 656e 6369 6573 203a 205b 2761 6d6f 6427  encies : ['amod'
+00000ea0: 2c20 276e 7375 626a 7061 7373 272c 2027  , 'nsubjpass', '
+00000eb0: 6175 7870 6173 7327 2c20 2752 4f4f 5427  auxpass', 'ROOT'
+00000ec0: 2c20 2761 6765 6e74 272c 2027 706f 626a  , 'agent', 'pobj
+00000ed0: 275d 0d0a 2020 2020 7461 6773 203a 205b  ']..    tags : [
+00000ee0: 274a 4a27 2c20 274e 4e53 272c 2027 5642  'JJ', 'NNS', 'VB
+00000ef0: 5027 2c20 2756 424e 272c 2027 494e 272c  P', 'VBN', 'IN',
+00000f00: 2027 4e4e 5327 5d0d 0a20 2020 2022 2222   'NNS']..    """
+00000f10: 0d0a 0d0a 0d0a 2020 2020 2320 2d2d 2d2d  ......    # ----
+00000f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 6164  --------------ad
+00000f30: 6469 6e67 2072 756c 6573 2074 6f20 7468  ding rules to th
+00000f40: 6520 6d61 7463 6865 722d 2d2d 2d2d 2d2d  e matcher-------
+00000f50: 2d2d 2d23 0d0a 0d0a 2020 2020 6d61 7463  ---#....    matc
+00000f60: 6865 722e 6164 6428 2270 6173 7369 7665  her.add("passive
+00000f70: 5f72 756c 655f 3122 2c20 5b70 6173 7369  _rule_1", [passi
+00000f80: 7665 5f72 756c 655f 315d 2c20 6772 6565  ve_rule_1], gree
+00000f90: 6479 3d27 4c4f 4e47 4553 5427 290d 0a20  dy='LONGEST').. 
+00000fa0: 2020 206d 6174 6368 6572 2e61 6464 2822     matcher.add("
+00000fb0: 7061 7373 6976 655f 7275 6c65 5f32 222c  passive_rule_2",
+00000fc0: 205b 7061 7373 6976 655f 7275 6c65 5f32   [passive_rule_2
+00000fd0: 5d2c 2067 7265 6564 793d 274c 4f4e 4745  ], greedy='LONGE
+00000fe0: 5354 2729 0d0a 2020 2020 6d61 7463 6865  ST')..    matche
+00000ff0: 722e 6164 6428 2270 6173 7369 7665 5f72  r.add("passive_r
+00001000: 756c 655f 3322 2c20 5b70 6173 7369 7665  ule_3", [passive
+00001010: 5f72 756c 655f 335d 2c20 6772 6565 6479  _rule_3], greedy
+00001020: 3d27 4c4f 4e47 4553 5427 290d 0a20 2020  ='LONGEST')..   
+00001030: 206d 6174 6368 6572 2e61 6464 2822 7061   matcher.add("pa
+00001040: 7373 6976 655f 7275 6c65 5f34 222c 205b  ssive_rule_4", [
+00001050: 7061 7373 6976 655f 7275 6c65 5f34 5d2c  passive_rule_4],
+00001060: 2067 7265 6564 793d 274c 4f4e 4745 5354   greedy='LONGEST
+00001070: 2729 0d0a 2020 2020 6d61 7463 6865 722e  ')..    matcher.
+00001080: 6164 6428 2270 6173 7369 7665 5f72 756c  add("passive_rul
+00001090: 655f 3522 2c20 5b70 6173 7369 7665 5f72  e_5", [passive_r
+000010a0: 756c 655f 355d 2c20 6772 6565 6479 3d27  ule_5], greedy='
+000010b0: 4c4f 4e47 4553 5427 290d 0a20 2020 206d  LONGEST')..    m
+000010c0: 6174 6368 6572 2e61 6464 2822 7061 7373  atcher.add("pass
+000010d0: 6976 655f 7275 6c65 5f36 222c 205b 7061  ive_rule_6", [pa
+000010e0: 7373 6976 655f 7275 6c65 5f36 5d2c 2067  ssive_rule_6], g
+000010f0: 7265 6564 793d 274c 4f4e 4745 5354 2729  reedy='LONGEST')
+00001100: 0d0a 0d0a 2020 2020 2320 7072 696e 7428  ....    # print(
+00001110: 274d 6174 6368 6572 2069 7320 6275 696c  'Matcher is buil
+00001120: 742e 2729 0d0a 0d0a 2020 2020 7265 7475  t.')....    retu
+00001130: 726e 206e 6c70 2c20 6d61 7463 6865 72    rn nlp, matcher
```

### Comparing `PassivePy-0.2.22/PassivePyCode/PassivePySrc/rules_for_full_passives.py` & `PassivePy-0.2.3/PassivePyCode/PassivePySrc/rules_for_full_passives.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,251 +1,279 @@
-00000000: 0d0a 2320 2043 6f70 7972 6967 6874 204d  ..#  Copyright M
-00000010: 6974 7261 204d 6972 7368 6166 6965 652c  itra Mirshafiee,
-00000020: 2032 3032 3220 4c69 6365 6e73 6564 2075   2022 Licensed u
-00000030: 6e64 6572 204d 4954 204c 6963 656e 7365  nder MIT License
-00000040: 2e0d 0a23 2020 5365 6520 7468 6520 4c49  ...#  See the LI
-00000050: 4345 4e53 452e 7478 7420 666f 7220 6d6f  CENSE.txt for mo
-00000060: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e0d  re information..
-00000070: 0a0d 0a0d 0a69 6d70 6f72 7420 7370 6163  .....import spac
-00000080: 790d 0a66 726f 6d20 7370 6163 792e 6d61  y..from spacy.ma
-00000090: 7463 6865 7220 696d 706f 7274 204d 6174  tcher import Mat
-000000a0: 6368 6572 0d0a 0d0a 0d0a 6465 6620 6372  cher......def cr
-000000b0: 6561 7465 5f6d 6174 6368 6572 5f66 756c  eate_matcher_ful
-000000c0: 6c28 6e6c 703a 7370 6163 792e 6c61 6e67  l(nlp:spacy.lang
-000000d0: 7561 6765 2e4c 616e 6775 6167 6520 3d20  uage.Language = 
-000000e0: 4e6f 6e65 293a 0d0a 0d0a 2020 2020 2222  None):....    ""
-000000f0: 2263 7265 6174 6573 2061 206d 6174 6368  "creates a match
-00000100: 6572 206f 6e20 7468 6520 666f 6c6c 6f77  er on the follow
-00000110: 696e 6720 766f 6361 6275 6c61 7279 2222  ing vocabulary""
-00000120: 220d 0a20 2020 206d 6174 6368 6572 203d  "..    matcher =
-00000130: 204d 6174 6368 6572 286e 6c70 2e76 6f63   Matcher(nlp.voc
-00000140: 6162 290d 0a0d 0a0d 0a20 2020 2023 206c  ab)......    # l
-00000150: 6973 7420 6f66 2076 6572 6273 2074 6861  ist of verbs tha
-00000160: 7420 7468 6569 7220 6164 6a65 6374 6976  t their adjectiv
-00000170: 6520 666f 726d 200d 0a20 2020 2023 2069  e form ..    # i
-00000180: 7320 736f 6d65 7469 6d65 7320 6d69 7374  s sometimes mist
-00000190: 616b 656e 2061 7320 6120 7665 7262 0d0a  aken as a verb..
-000001a0: 2020 2020 7665 7262 735f 6c69 7374 203d      verbs_list =
-000001b0: 205b 2261 7373 6f63 6961 7465 222c 2022   ["associate", "
-000001c0: 696e 766f 6c76 6522 2c20 2265 7868 6175  involve", "exhau
-000001d0: 7374 222c 2022 6261 7365 222c 200d 0a20  st", "base", .. 
-000001e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000001f0: 6c65 6164 222c 2022 7374 756e 222c 2022  lead", "stun", "
-00000200: 6f76 6572 7261 7465 222c 2020 2266 696c  overrate",  "fil
-00000210: 6c22 2c20 2262 6561 7222 2c0d 0a20 2020  l", "bear",..   
-00000220: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00000230: 6d70 6c69 6361 7465 222c 2022 7265 7365  mplicate", "rese
-00000240: 7276 6522 2c20 2263 6f6d 706c 6963 6174  rve", "complicat
-00000250: 6522 2c20 2268 6561 7422 2c0d 0a20 2020  e", "heat",..   
-00000260: 2020 2020 2020 2020 2020 2020 2022 7363               "sc
-00000270: 7265 7722 2c5d 0d0a 0d0a 2020 2020 232d  rew",]....    #-
-00000280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000290: 2d2d 2d2d 2d2d 2d2d 2d72 756c 6573 2d2d  ---------rules--
-000002a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000002b0: 2d2d 230d 0a0d 0a20 2020 200d 0a20 2020  --#....    ..   
-000002c0: 2070 6173 7369 7665 5f72 756c 655f 3120   passive_rule_1 
-000002d0: 3d20 5b0d 0a20 2020 2020 2020 207b 2250  = [..        {"P
-000002e0: 4f53 223a 2241 5558 222c 2022 4445 5022  OS":"AUX", "DEP"
-000002f0: 3a20 2261 7578 222c 2022 4f50 223a 222a  : "aux", "OP":"*
-00000300: 227d 2c0d 0a20 2020 2020 2020 207b 2250  "},..        {"P
-00000310: 4f53 223a 2241 5558 222c 2022 4445 5022  OS":"AUX", "DEP"
-00000320: 3a20 2261 7578 7061 7373 222c 2022 4f50  : "auxpass", "OP
-00000330: 223a 222b 227d 2c0d 0a20 2020 2020 2020  ":"+"},..       
-00000340: 207b 2244 4550 223a 226e 6567 222c 2022   {"DEP":"neg", "
-00000350: 5441 4722 3a22 5242 222c 2022 4f50 223a  TAG":"RB", "OP":
-00000360: 222a 227d 2c0d 0a20 2020 2020 2020 207b  "*"},..        {
-00000370: 2244 4550 223a 2248 5950 4822 2c20 224f  "DEP":"HYPH", "O
-00000380: 5022 3a22 2a22 7d2c 0d0a 2020 2020 2020  P":"*"},..      
-00000390: 2020 7b22 4445 5022 3a22 6164 766d 6f64    {"DEP":"advmod
-000003a0: 222c 2022 5441 4722 3a22 5242 222c 2022  ", "TAG":"RB", "
-000003b0: 4f50 223a 222a 227d 2c0d 0a20 2020 2020  OP":"*"},..     
-000003c0: 2020 207b 2250 4f53 223a 2256 4552 4222     {"POS":"VERB"
-000003d0: 2c20 2254 4147 223a 2256 424e 222c 2022  , "TAG":"VBN", "
-000003e0: 4c45 4d4d 4122 3a7b 224e 4f54 5f49 4e22  LEMMA":{"NOT_IN"
-000003f0: 203a 2076 6572 6273 5f6c 6973 7420 2b20   : verbs_list + 
-00000400: 5b27 6265 275d 7d7d 2c0d 0a20 2020 2020  ['be']}},..     
-00000410: 2020 207b 224c 4f57 4552 223a 2262 7922     {"LOWER":"by"
-00000420: 7d0d 0a20 2020 205d 0d0a 0d0a 2020 2020  }..    ]....    
-00000430: 2222 220d 0a20 2020 2073 656e 7465 6e63  """..    sentenc
-00000440: 6520 3a20 5468 6520 626f 6f6b 2077 6173  e : The book was
-00000450: 2072 6561 6420 6279 2068 696d 2e0d 0a20   read by him... 
-00000460: 2020 2064 6570 656e 6465 6e63 6965 7320     dependencies 
-00000470: 3a20 5b27 6465 7427 2c20 276e 7375 626a  : ['det', 'nsubj
-00000480: 7061 7373 272c 2027 6175 7870 6173 7327  pass', 'auxpass'
-00000490: 2c20 2752 4f4f 5427 2c20 2761 6765 6e74  , 'ROOT', 'agent
-000004a0: 272c 2027 706f 626a 272c 2027 7075 6e63  ', 'pobj', 'punc
-000004b0: 7427 5d0d 0a20 2020 2054 6167 7320 3a20  t']..    Tags : 
-000004c0: 5b27 4454 272c 2027 4e4e 272c 2027 5642  ['DT', 'NN', 'VB
-000004d0: 4427 2c20 2756 424e 272c 2027 494e 272c  D', 'VBN', 'IN',
-000004e0: 2027 5052 5027 2c20 272e 275d 0d0a 2020   'PRP', '.']..  
-000004f0: 2020 2222 220d 0a20 2020 2070 6173 7369    """..    passi
-00000500: 7665 5f72 756c 655f 3220 3d20 5b0d 0a20  ve_rule_2 = [.. 
-00000510: 2020 2020 2020 207b 2244 4550 223a 207b         {"DEP": {
-00000520: 2249 4e22 3a20 5b22 6174 7472 222c 2027  "IN": ["attr", '
-00000530: 6e73 7562 6a70 6173 7327 2c20 2761 7070  nsubjpass', 'app
-00000540: 6f73 275d 7d7d 2c0d 0a20 2020 2020 2020  os']}},..       
-00000550: 207b 2254 4147 223a 2022 5242 222c 2022   {"TAG": "RB", "
-00000560: 4445 5022 3a20 2261 6476 6d6f 6422 2c20  DEP": "advmod", 
-00000570: 224f 5022 203a 2022 2a22 7d2c 0d0a 2020  "OP" : "*"},..  
-00000580: 2020 2020 2020 7b22 4445 5022 3a20 2250        {"DEP": "P
-00000590: 554e 4354 222c 2022 4f50 2220 3a20 222a  UNCT", "OP" : "*
-000005a0: 227d 2c0d 0a20 2020 2020 2020 207b 2254  "},..        {"T
-000005b0: 4147 223a 2022 5642 4e22 2c20 2244 4550  AG": "VBN", "DEP
-000005c0: 223a 2022 6163 6c22 2c22 4c45 4d4d 4122  ": "acl","LEMMA"
-000005d0: 3a20 7b22 4e4f 545f 494e 2220 3a20 7665  : {"NOT_IN" : ve
-000005e0: 7262 735f 6c69 7374 7d7d 2c0d 0a20 2020  rbs_list}},..   
-000005f0: 2020 2020 207b 224c 4f57 4552 223a 2262       {"LOWER":"b
-00000600: 7922 7d0d 0a20 2020 205d 0d0a 0d0a 2020  y"}..    ]....  
-00000610: 2020 2222 220d 0a20 2020 2073 656e 7465    """..    sente
-00000620: 6e63 6520 3a20 7468 6572 6520 7761 7320  nce : there was 
-00000630: 6e6f 2063 6861 6e67 6520 6465 7465 6374  no change detect
-00000640: 6564 2069 6e20 6865 7220 6265 6861 7669  ed in her behavi
-00000650: 6f72 2e0d 0a20 2020 2064 6570 656e 6465  or...    depende
-00000660: 6e63 6965 7320 3a20 5b27 6578 706c 272c  ncies : ['expl',
-00000670: 2027 524f 4f54 272c 2027 6465 7427 2c20   'ROOT', 'det', 
-00000680: 2761 7474 7227 2c20 2761 636c 272c 2027  'attr', 'acl', '
-00000690: 7072 6570 272c 2027 706f 7373 272c 2027  prep', 'poss', '
-000006a0: 706f 626a 272c 2027 7075 6e63 7427 5d0d  pobj', 'punct'].
-000006b0: 0a20 2020 2074 6167 7320 3a20 5b27 4558  .    tags : ['EX
-000006c0: 272c 2027 5642 4427 2c20 2744 5427 2c20  ', 'VBD', 'DT', 
-000006d0: 274e 4e27 2c20 2756 424e 272c 2027 494e  'NN', 'VBN', 'IN
-000006e0: 272c 2027 5052 5024 272c 2027 4e4e 272c  ', 'PRP$', 'NN',
-000006f0: 2027 2e27 5d0d 0a20 2020 2022 2222 0d0a   '.']..    """..
-00000700: 0d0a 0d0a 2020 2020 7061 7373 6976 655f  ....    passive_
-00000710: 7275 6c65 5f33 203d 205b 0d0a 2020 2020  rule_3 = [..    
-00000720: 2020 2020 7b22 504f 5322 3a22 4155 5822      {"POS":"AUX"
-00000730: 2c20 2244 4550 223a 2022 6175 7822 2c20  , "DEP": "aux", 
-00000740: 224f 5022 3a22 2a22 7d2c 0d0a 2020 2020  "OP":"*"},..    
-00000750: 2020 2020 7b22 504f 5322 3a22 4155 5822      {"POS":"AUX"
-00000760: 2c20 2244 4550 223a 2022 6175 7870 6173  , "DEP": "auxpas
-00000770: 7322 2c20 224f 5022 3a22 2b22 7d2c 0d0a  s", "OP":"+"},..
-00000780: 2020 2020 2020 2020 7b22 4445 5022 3a22          {"DEP":"
-00000790: 6e65 6722 2c20 2254 4147 223a 2252 4222  neg", "TAG":"RB"
-000007a0: 2c20 224f 5022 3a22 2a22 7d2c 0d0a 2020  , "OP":"*"},..  
-000007b0: 2020 2020 2020 7b22 4445 5022 3a22 4859        {"DEP":"HY
-000007c0: 5048 222c 2022 4f50 223a 222a 227d 2c0d  PH", "OP":"*"},.
-000007d0: 0a20 2020 2020 2020 207b 2244 4550 223a  .        {"DEP":
-000007e0: 2261 6476 6d6f 6422 2c20 2254 4147 223a  "advmod", "TAG":
-000007f0: 2252 4222 2c20 224f 5022 3a22 2a22 7d2c  "RB", "OP":"*"},
-00000800: 0d0a 2020 2020 2020 2020 7b22 504f 5322  ..        {"POS"
-00000810: 3a22 5645 5242 222c 2022 4445 5022 3a22  :"VERB", "DEP":"
-00000820: 524f 4f54 222c 2022 4c45 4d4d 4122 3a7b  ROOT", "LEMMA":{
-00000830: 224e 4f54 5f49 4e22 203a 2076 6572 6273  "NOT_IN" : verbs
-00000840: 5f6c 6973 747d 7d2c 0d0a 2020 2020 2020  _list}},..      
-00000850: 2020 7b22 4445 5022 3a22 6363 227d 2c0d    {"DEP":"cc"},.
-00000860: 0a20 2020 2020 2020 207b 2244 4550 223a  .        {"DEP":
-00000870: 2261 6476 6d6f 6422 2c20 2254 4147 223a  "advmod", "TAG":
-00000880: 2256 424e 222c 2022 4f50 223a 2022 2a22  "VBN", "OP": "*"
-00000890: 2c20 224c 454d 4d41 223a 207b 224e 4f54  , "LEMMA": {"NOT
-000008a0: 5f49 4e22 3a5b 2270 7265 225d 7d7d 2c0d  _IN":["pre"]}},.
-000008b0: 0a20 2020 2020 2020 207b 2244 4550 223a  .        {"DEP":
-000008c0: 2022 636f 6e6a 222c 2022 4c45 4d4d 4122   "conj", "LEMMA"
-000008d0: 3a7b 224e 4f54 5f49 4e22 203a 2076 6572  :{"NOT_IN" : ver
-000008e0: 6273 5f6c 6973 747d 7d2c 200d 0a20 2020  bs_list}}, ..   
-000008f0: 2020 2020 207b 224c 4f57 4552 223a 2262       {"LOWER":"b
-00000900: 7922 7d0d 0a20 2020 205d 0d0a 0d0a 2020  y"}..    ]....  
-00000910: 2020 2222 220d 0a20 2020 2055 7365 6420    """..    Used 
-00000920: 666f 7220 7468 6520 7365 636f 6e64 2070  for the second p
-00000930: 6172 7420 7769 7468 2022 616e 6420 2e2e  art with "and ..
-00000940: 2e22 200d 0a20 2020 2073 656e 7465 6e63  ." ..    sentenc
-00000950: 6520 3a20 6974 2077 6173 2064 6574 6572  e : it was deter
-00000960: 6d69 6e65 6420 616e 6420 666f 726d 6564  mined and formed
-00000970: 2e0d 0a20 2020 2064 6570 656e 6465 6e63  ...    dependenc
-00000980: 6965 7320 3a20 5b27 6e73 7562 6a70 6173  ies : ['nsubjpas
-00000990: 7327 2c20 2761 7578 7061 7373 272c 2027  s', 'auxpass', '
-000009a0: 524f 4f54 272c 2027 6363 272c 2027 636f  ROOT', 'cc', 'co
-000009b0: 6e6a 272c 2027 7075 6e63 7427 5d0d 0a20  nj', 'punct'].. 
-000009c0: 2020 2074 6167 7320 3a20 5b27 5052 5027     tags : ['PRP'
-000009d0: 2c20 2756 4244 272c 2027 5642 4e27 2c20  , 'VBD', 'VBN', 
-000009e0: 2743 4327 2c20 2756 424e 272c 2027 2e27  'CC', 'VBN', '.'
-000009f0: 5d0d 0a20 2020 2022 2222 0d0a 0d0a 2020  ]..    """....  
-00000a00: 2020 7061 7373 6976 655f 7275 6c65 5f34    passive_rule_4
-00000a10: 203d 205b 0d0a 2020 2020 2020 2020 7b22   = [..        {"
-00000a20: 4445 5022 3a22 6164 7663 6c22 2c20 2254  DEP":"advcl", "T
-00000a30: 4147 223a 2256 424e 227d 2c0d 0a20 2020  AG":"VBN"},..   
-00000a40: 2020 2020 207b 2244 4550 223a 2022 6167       {"DEP": "ag
-00000a50: 656e 7422 2c20 2254 4147 223a 2249 4e22  ent", "TAG":"IN"
-00000a60: 7d2c 0d0a 2020 2020 2020 2020 7b22 4f50  },..        {"OP
-00000a70: 223a 222a 227d 2c0d 0a20 2020 2020 2020  ":"*"},..       
-00000a80: 207b 2244 4550 223a 2022 706f 626a 227d   {"DEP": "pobj"}
-00000a90: 2c0d 0a20 2020 205d 0d0a 0d0a 2020 2020  ,..    ]....    
-00000aa0: 2222 220d 0a20 2020 2073 656e 7465 6e63  """..    sentenc
-00000ab0: 6520 3a20 6b69 6c6c 6564 2062 7920 7468  e : killed by th
-00000ac0: 6520 706f 6c69 6365 2c20 6865 206e 6576  e police, he nev
-00000ad0: 6572 2074 686f 7567 6874 2074 6869 7320  er thought this 
-00000ae0: 776f 756c 6420 6265 2068 6973 2065 6e64  would be his end
-00000af0: 2e0d 0a20 2020 2064 6570 656e 6465 6e63  ...    dependenc
-00000b00: 6965 7320 3a20 5b27 6164 7663 6c27 2c20  ies : ['advcl', 
-00000b10: 2761 6765 6e74 272c 2027 6465 7427 2c20  'agent', 'det', 
-00000b20: 2770 6f62 6a27 2c20 2770 756e 6374 272c  'pobj', 'punct',
-00000b30: 2027 6e73 7562 6a27 2c20 276e 6567 272c   'nsubj', 'neg',
-00000b40: 2027 524f 4f54 272c 2027 6e73 7562 6a27   'ROOT', 'nsubj'
-00000b50: 2c20 2761 7578 272c 2027 6363 6f6d 7027  , 'aux', 'ccomp'
-00000b60: 2c20 2770 6f73 7327 2c20 2761 7474 7227  , 'poss', 'attr'
-00000b70: 5d0d 0a20 2020 2074 6167 7320 3a20 5b27  ]..    tags : ['
-00000b80: 5642 4e27 2c20 2749 4e27 2c20 2744 5427  VBN', 'IN', 'DT'
-00000b90: 2c20 274e 4e27 2c20 272c 272c 2027 5052  , 'NN', ',', 'PR
-00000ba0: 5027 2c20 2752 4227 2c20 2756 4244 272c  P', 'RB', 'VBD',
-00000bb0: 2027 4454 272c 2027 4d44 272c 2027 5642   'DT', 'MD', 'VB
-00000bc0: 272c 2027 5052 5024 272c 2027 4e4e 275d  ', 'PRP$', 'NN']
-00000bd0: 0d0a 2020 2020 2222 220d 0a0d 0a0d 0a20  ..    """...... 
-00000be0: 2020 2070 6173 7369 7665 5f72 756c 655f     passive_rule_
-00000bf0: 3520 3d20 5b0d 0a20 2020 2020 2020 207b  5 = [..        {
-00000c00: 224c 454d 4d41 223a 207b 2249 4e22 3a20  "LEMMA": {"IN": 
-00000c10: 7665 7262 735f 6c69 7374 7d7d 2c0d 0a20  verbs_list}},.. 
-00000c20: 2020 2020 2020 207b 224c 4f57 4552 223a         {"LOWER":
-00000c30: 2262 7922 7d0d 0a20 2020 205d 0d0a 0d0a  "by"}..    ]....
-00000c40: 0d0a 2020 2020 2222 220d 0a20 2020 2074  ..    """..    t
-00000c50: 6f20 6176 6f69 6420 7468 6520 636f 6e66  o avoid the conf
-00000c60: 7573 696f 6e20 6265 7477 6565 6e20 7468  usion between th
-00000c70: 6520 6164 6a65 6374 6976 6520 616e 6420  e adjective and 
-00000c80: 7061 7373 6976 6520 7665 7273 696f 6e20  passive version 
-00000c90: 6f66 2073 7065 6369 6669 6320 0d0a 2020  of specific ..  
-00000ca0: 2020 7665 7262 732c 2077 6520 6465 6469    verbs, we dedi
-00000cb0: 6361 7465 6420 6120 6e65 7720 7275 6c65  cated a new rule
-00000cc0: 2074 6f20 736f 6d65 2076 6572 6273 2074   to some verbs t
-00000cd0: 6f20 6265 2064 6574 6563 7465 6420 7768  o be detected wh
-00000ce0: 656e 2075 7365 6420 7769 7468 200d 0a20  en used with .. 
-00000cf0: 2020 2061 6e20 6167 656e 7420 2862 7929     an agent (by)
-00000d00: 0d0a 0d0a 2020 2020 7365 6e74 656e 6365  ....    sentence
-00000d10: 203a 204e 6174 7572 616c 2072 6573 6f75   : Natural resou
-00000d20: 7263 6573 2061 7265 2065 7868 6175 7374  rces are exhaust
-00000d30: 6564 2062 7920 6875 6d61 6e73 2e0d 0a20  ed by humans... 
-00000d40: 2020 2064 6570 656e 6465 6e63 6965 7320     dependencies 
-00000d50: 3a20 5b27 616d 6f64 272c 2027 6e73 7562  : ['amod', 'nsub
-00000d60: 6a70 6173 7327 2c20 2761 7578 7061 7373  jpass', 'auxpass
-00000d70: 272c 2027 524f 4f54 272c 2027 6167 656e  ', 'ROOT', 'agen
-00000d80: 7427 2c20 2770 6f62 6a27 5d0d 0a20 2020  t', 'pobj']..   
-00000d90: 2074 6167 7320 3a20 5b27 4a4a 272c 2027   tags : ['JJ', '
-00000da0: 4e4e 5327 2c20 2756 4250 272c 2027 5642  NNS', 'VBP', 'VB
-00000db0: 4e27 2c20 2749 4e27 2c20 274e 4e53 275d  N', 'IN', 'NNS']
-00000dc0: 0d0a 2020 2020 2222 220d 0a0d 0a0d 0a20  ..    """...... 
-00000dd0: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d     # -----------
-00000de0: 2d2d 2d2d 2d2d 2d61 6464 696e 6720 7275  -------adding ru
-00000df0: 6c65 7320 746f 2074 6865 206d 6174 6368  les to the match
-00000e00: 6572 2d2d 2d2d 2d2d 2d2d 2d2d 230d 0a0d  er----------#...
-00000e10: 0a20 2020 206d 6174 6368 6572 2e61 6464  .    matcher.add
-00000e20: 2822 7061 7373 6976 655f 7275 6c65 5f31  ("passive_rule_1
-00000e30: 222c 205b 7061 7373 6976 655f 7275 6c65  ", [passive_rule
-00000e40: 5f31 5d2c 2067 7265 6564 793d 274c 4f4e  _1], greedy='LON
-00000e50: 4745 5354 2729 0d0a 2020 2020 6d61 7463  GEST')..    matc
-00000e60: 6865 722e 6164 6428 2270 6173 7369 7665  her.add("passive
-00000e70: 5f72 756c 655f 3222 2c20 5b70 6173 7369  _rule_2", [passi
-00000e80: 7665 5f72 756c 655f 325d 2c20 6772 6565  ve_rule_2], gree
-00000e90: 6479 3d27 4c4f 4e47 4553 5427 290d 0a20  dy='LONGEST').. 
-00000ea0: 2020 206d 6174 6368 6572 2e61 6464 2822     matcher.add("
-00000eb0: 7061 7373 6976 655f 7275 6c65 5f33 222c  passive_rule_3",
-00000ec0: 205b 7061 7373 6976 655f 7275 6c65 5f33   [passive_rule_3
-00000ed0: 5d2c 2067 7265 6564 793d 274c 4f4e 4745  ], greedy='LONGE
-00000ee0: 5354 2729 0d0a 2020 2020 6d61 7463 6865  ST')..    matche
-00000ef0: 722e 6164 6428 2270 6173 7369 7665 5f72  r.add("passive_r
-00000f00: 756c 655f 3422 2c20 5b70 6173 7369 7665  ule_4", [passive
-00000f10: 5f72 756c 655f 345d 2c20 6772 6565 6479  _rule_4], greedy
-00000f20: 3d27 4c4f 4e47 4553 5427 290d 0a20 2020  ='LONGEST')..   
-00000f30: 206d 6174 6368 6572 2e61 6464 2822 7061   matcher.add("pa
-00000f40: 7373 6976 655f 7275 6c65 5f35 222c 205b  ssive_rule_5", [
-00000f50: 7061 7373 6976 655f 7275 6c65 5f35 5d2c  passive_rule_5],
-00000f60: 2067 7265 6564 793d 274c 4f4e 4745 5354   greedy='LONGEST
-00000f70: 2729 0d0a 0d0a 2020 2020 2320 7072 696e  ')....    # prin
-00000f80: 7428 274d 6174 6368 6572 2069 7320 6275  t('Matcher is bu
-00000f90: 696c 742e 2729 0d0a 0d0a 2020 2020 7265  ilt.')....    re
-00000fa0: 7475 726e 206d 6174 6368 6572            turn matcher
+00000000: 696d 706f 7274 2073 7061 6379 0d0a 6672  import spacy..fr
+00000010: 6f6d 2073 7061 6379 2e6d 6174 6368 6572  om spacy.matcher
+00000020: 2069 6d70 6f72 7420 4d61 7463 6865 720d   import Matcher.
+00000030: 0a0d 0a0d 0a0d 0a64 6566 2063 7265 6174  .......def creat
+00000040: 655f 6d61 7463 6865 725f 6675 6c6c 2873  e_matcher_full(s
+00000050: 7061 6379 5f6d 6f64 656c 203d 2022 656e  pacy_model = "en
+00000060: 5f63 6f72 655f 7765 625f 6c67 2229 3a0d  _core_web_lg"):.
+00000070: 0a0d 0a20 2020 2022 2222 6372 6561 7465  ...    """create
+00000080: 7320 6120 6d61 7463 6865 7220 6f6e 2074  s a matcher on t
+00000090: 6865 2066 6f6c 6c6f 7769 6e67 2076 6f63  he following voc
+000000a0: 6162 756c 6172 7922 2222 0d0a 2020 2020  abulary"""..    
+000000b0: 6e6c 7020 3d20 7370 6163 792e 6c6f 6164  nlp = spacy.load
+000000c0: 2873 7061 6379 5f6d 6f64 656c 2c20 6469  (spacy_model, di
+000000d0: 7361 626c 653d 5b22 6e65 7222 5d29 0d0a  sable=["ner"])..
+000000e0: 2020 2020 6d61 7463 6865 7220 3d20 4d61      matcher = Ma
+000000f0: 7463 6865 7228 6e6c 702e 766f 6361 6229  tcher(nlp.vocab)
+00000100: 0d0a 0d0a 2020 2020 2320 6c69 7374 206f  ....    # list o
+00000110: 6620 7665 7262 7320 7468 6174 2074 6865  f verbs that the
+00000120: 6972 2061 646a 6563 7469 7665 2066 6f72  ir adjective for
+00000130: 6d20 0d0a 2020 2020 2320 6973 2073 6f6d  m ..    # is som
+00000140: 6574 696d 6573 206d 6973 7461 6b65 6e20  etimes mistaken 
+00000150: 6173 2061 2076 6572 620d 0a20 2020 2076  as a verb..    v
+00000160: 6572 6273 5f6c 6973 7420 3d20 5b22 6173  erbs_list = ["as
+00000170: 736f 6369 6174 6522 2c20 2269 6e76 6f6c  sociate", "invol
+00000180: 7665 222c 2022 6578 6861 7573 7422 2c20  ve", "exhaust", 
+00000190: 2262 6173 6522 2c20 0d0a 2020 2020 2020  "base", ..      
+000001a0: 2020 2020 2020 2020 2020 226c 6561 6422            "lead"
+000001b0: 2c20 2273 7475 6e22 2c20 226f 7665 7272  , "stun", "overr
+000001c0: 6174 6522 2c20 2022 6669 6c6c 222c 2022  ate",  "fill", "
+000001d0: 6265 6172 222c 0d0a 2020 2020 2020 2020  bear",..        
+000001e0: 2020 2020 2020 2020 2263 6f6d 706c 6963          "complic
+000001f0: 6174 6522 2c20 2272 6573 6572 7665 222c  ate", "reserve",
+00000200: 2022 636f 6d70 6c69 6361 7465 222c 2022   "complicate", "
+00000210: 6865 6174 222c 0d0a 2020 2020 2020 2020  heat",..        
+00000220: 2020 2020 2020 2020 2273 6372 6577 222c          "screw",
+00000230: 5d0d 0a0d 0a20 2020 2023 2d2d 2d2d 2d2d  ]....    #------
+00000240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000250: 2d2d 2d2d 7275 6c65 732d 2d2d 2d2d 2d2d  ----rules-------
+00000260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d23 0d0a  -------------#..
+00000270: 0d0a 2020 2020 0d0a 2020 2020 7061 7373  ..    ..    pass
+00000280: 6976 655f 7275 6c65 5f31 203d 205b 0d0a  ive_rule_1 = [..
+00000290: 2020 2020 2020 2020 7b22 504f 5322 3a22          {"POS":"
+000002a0: 4155 5822 2c20 2244 4550 223a 2022 6175  AUX", "DEP": "au
+000002b0: 7822 2c20 224f 5022 3a22 2a22 7d2c 0d0a  x", "OP":"*"},..
+000002c0: 2020 2020 2020 2020 7b22 504f 5322 3a22          {"POS":"
+000002d0: 4155 5822 2c20 2244 4550 223a 2022 6175  AUX", "DEP": "au
+000002e0: 7870 6173 7322 2c20 224f 5022 3a22 2b22  xpass", "OP":"+"
+000002f0: 7d2c 0d0a 2020 2020 2020 2020 7b22 4445  },..        {"DE
+00000300: 5022 3a22 6e65 6722 2c20 2254 4147 223a  P":"neg", "TAG":
+00000310: 2252 4222 2c20 224f 5022 3a22 2a22 7d2c  "RB", "OP":"*"},
+00000320: 0d0a 2020 2020 2020 2020 7b22 4445 5022  ..        {"DEP"
+00000330: 3a22 4859 5048 222c 2022 4f50 223a 222a  :"HYPH", "OP":"*
+00000340: 227d 2c0d 0a20 2020 2020 2020 207b 2244  "},..        {"D
+00000350: 4550 223a 2261 6476 6d6f 6422 2c20 2254  EP":"advmod", "T
+00000360: 4147 223a 2252 4222 2c20 224f 5022 3a22  AG":"RB", "OP":"
+00000370: 2a22 7d2c 0d0a 2020 2020 2020 2020 7b22  *"},..        {"
+00000380: 504f 5322 3a22 5645 5242 222c 2022 5441  POS":"VERB", "TA
+00000390: 4722 3a22 5642 4e22 2c20 224c 454d 4d41  G":"VBN", "LEMMA
+000003a0: 223a 7b22 4e4f 545f 494e 2220 3a20 7665  ":{"NOT_IN" : ve
+000003b0: 7262 735f 6c69 7374 202b 205b 2762 6527  rbs_list + ['be'
+000003c0: 5d7d 7d2c 0d0a 2020 2020 2020 2020 7b22  ]}},..        {"
+000003d0: 4c4f 5745 5222 3a22 6279 227d 0d0a 2020  LOWER":"by"}..  
+000003e0: 2020 5d0d 0a0d 0a20 2020 2022 2222 0d0a    ]....    """..
+000003f0: 2020 2020 7365 6e74 656e 6365 203a 2054      sentence : T
+00000400: 6865 2062 6f6f 6b20 7761 7320 7265 6164  he book was read
+00000410: 2062 7920 6869 6d2e 0d0a 2020 2020 6465   by him...    de
+00000420: 7065 6e64 656e 6369 6573 203a 205b 2764  pendencies : ['d
+00000430: 6574 272c 2027 6e73 7562 6a70 6173 7327  et', 'nsubjpass'
+00000440: 2c20 2761 7578 7061 7373 272c 2027 524f  , 'auxpass', 'RO
+00000450: 4f54 272c 2027 6167 656e 7427 2c20 2770  OT', 'agent', 'p
+00000460: 6f62 6a27 2c20 2770 756e 6374 275d 0d0a  obj', 'punct']..
+00000470: 2020 2020 5461 6773 203a 205b 2744 5427      Tags : ['DT'
+00000480: 2c20 274e 4e27 2c20 2756 4244 272c 2027  , 'NN', 'VBD', '
+00000490: 5642 4e27 2c20 2749 4e27 2c20 2750 5250  VBN', 'IN', 'PRP
+000004a0: 272c 2027 2e27 5d0d 0a20 2020 2022 2222  ', '.']..    """
+000004b0: 0d0a 2020 2020 7061 7373 6976 655f 7275  ..    passive_ru
+000004c0: 6c65 5f32 203d 205b 0d0a 2020 2020 2020  le_2 = [..      
+000004d0: 2020 7b22 4445 5022 3a20 7b22 494e 223a    {"DEP": {"IN":
+000004e0: 205b 2261 7474 7222 2c20 276e 7375 626a   ["attr", 'nsubj
+000004f0: 7061 7373 272c 2027 6170 706f 7327 5d7d  pass', 'appos']}
+00000500: 7d2c 0d0a 2020 2020 2020 2020 7b22 5441  },..        {"TA
+00000510: 4722 3a20 2252 4222 2c20 2244 4550 223a  G": "RB", "DEP":
+00000520: 2022 6164 766d 6f64 222c 2022 4f50 2220   "advmod", "OP" 
+00000530: 3a20 222a 227d 2c0d 0a20 2020 2020 2020  : "*"},..       
+00000540: 207b 2244 4550 223a 2022 5055 4e43 5422   {"DEP": "PUNCT"
+00000550: 2c20 224f 5022 203a 2022 2a22 7d2c 0d0a  , "OP" : "*"},..
+00000560: 2020 2020 2020 2020 7b22 5441 4722 3a20          {"TAG": 
+00000570: 2256 424e 222c 2022 4445 5022 3a20 2261  "VBN", "DEP": "a
+00000580: 636c 222c 224c 454d 4d41 223a 207b 224e  cl","LEMMA": {"N
+00000590: 4f54 5f49 4e22 203a 2076 6572 6273 5f6c  OT_IN" : verbs_l
+000005a0: 6973 747d 7d2c 0d0a 2020 2020 2020 2020  ist}},..        
+000005b0: 7b22 4c4f 5745 5222 3a22 6279 227d 0d0a  {"LOWER":"by"}..
+000005c0: 2020 2020 5d0d 0a0d 0a20 2020 2022 2222      ]....    """
+000005d0: 0d0a 2020 2020 7365 6e74 656e 6365 203a  ..    sentence :
+000005e0: 2074 6865 7265 2077 6173 206e 6f20 6368   there was no ch
+000005f0: 616e 6765 2064 6574 6563 7465 6420 696e  ange detected in
+00000600: 2068 6572 2062 6568 6176 696f 722e 0d0a   her behavior...
+00000610: 2020 2020 6465 7065 6e64 656e 6369 6573      dependencies
+00000620: 203a 205b 2765 7870 6c27 2c20 2752 4f4f   : ['expl', 'ROO
+00000630: 5427 2c20 2764 6574 272c 2027 6174 7472  T', 'det', 'attr
+00000640: 272c 2027 6163 6c27 2c20 2770 7265 7027  ', 'acl', 'prep'
+00000650: 2c20 2770 6f73 7327 2c20 2770 6f62 6a27  , 'poss', 'pobj'
+00000660: 2c20 2770 756e 6374 275d 0d0a 2020 2020  , 'punct']..    
+00000670: 7461 6773 203a 205b 2745 5827 2c20 2756  tags : ['EX', 'V
+00000680: 4244 272c 2027 4454 272c 2027 4e4e 272c  BD', 'DT', 'NN',
+00000690: 2027 5642 4e27 2c20 2749 4e27 2c20 2750   'VBN', 'IN', 'P
+000006a0: 5250 2427 2c20 274e 4e27 2c20 272e 275d  RP$', 'NN', '.']
+000006b0: 0d0a 2020 2020 2222 220d 0a0d 0a0d 0a20  ..    """...... 
+000006c0: 2020 2070 6173 7369 7665 5f72 756c 655f     passive_rule_
+000006d0: 3320 3d20 5b0d 0a20 2020 2020 2020 207b  3 = [..        {
+000006e0: 2250 4f53 223a 2241 5558 222c 2022 4445  "POS":"AUX", "DE
+000006f0: 5022 3a20 2261 7578 222c 2022 4f50 223a  P": "aux", "OP":
+00000700: 222a 227d 2c0d 0a20 2020 2020 2020 207b  "*"},..        {
+00000710: 2250 4f53 223a 2241 5558 222c 2022 4445  "POS":"AUX", "DE
+00000720: 5022 3a20 2261 7578 7061 7373 222c 2022  P": "auxpass", "
+00000730: 4f50 223a 222b 227d 2c0d 0a20 2020 2020  OP":"+"},..     
+00000740: 2020 207b 2244 4550 223a 226e 6567 222c     {"DEP":"neg",
+00000750: 2022 5441 4722 3a22 5242 222c 2022 4f50   "TAG":"RB", "OP
+00000760: 223a 222a 227d 2c0d 0a20 2020 2020 2020  ":"*"},..       
+00000770: 207b 2244 4550 223a 2248 5950 4822 2c20   {"DEP":"HYPH", 
+00000780: 224f 5022 3a22 2a22 7d2c 0d0a 2020 2020  "OP":"*"},..    
+00000790: 2020 2020 7b22 4445 5022 3a22 6164 766d      {"DEP":"advm
+000007a0: 6f64 222c 2022 5441 4722 3a22 5242 222c  od", "TAG":"RB",
+000007b0: 2022 4f50 223a 222a 227d 2c0d 0a20 2020   "OP":"*"},..   
+000007c0: 2020 2020 207b 2250 4f53 223a 2256 4552       {"POS":"VER
+000007d0: 4222 2c20 2244 4550 223a 2252 4f4f 5422  B", "DEP":"ROOT"
+000007e0: 2c20 224c 454d 4d41 223a 7b22 4e4f 545f  , "LEMMA":{"NOT_
+000007f0: 494e 2220 3a20 7665 7262 735f 6c69 7374  IN" : verbs_list
+00000800: 7d7d 2c0d 0a20 2020 2020 2020 207b 2244  }},..        {"D
+00000810: 4550 223a 2263 6322 7d2c 0d0a 2020 2020  EP":"cc"},..    
+00000820: 2020 2020 7b22 4445 5022 3a22 6164 766d      {"DEP":"advm
+00000830: 6f64 222c 2022 5441 4722 3a22 5642 4e22  od", "TAG":"VBN"
+00000840: 2c20 224f 5022 3a20 222a 222c 2022 4c45  , "OP": "*", "LE
+00000850: 4d4d 4122 3a20 7b22 4e4f 545f 494e 223a  MMA": {"NOT_IN":
+00000860: 5b22 7072 6522 5d7d 7d2c 0d0a 2020 2020  ["pre"]}},..    
+00000870: 2020 2020 7b22 4445 5022 3a20 2263 6f6e      {"DEP": "con
+00000880: 6a22 2c20 224c 454d 4d41 223a 7b22 4e4f  j", "LEMMA":{"NO
+00000890: 545f 494e 2220 3a20 7665 7262 735f 6c69  T_IN" : verbs_li
+000008a0: 7374 7d7d 2c20 0d0a 2020 2020 2020 2020  st}}, ..        
+000008b0: 7b22 4c4f 5745 5222 3a22 6279 227d 0d0a  {"LOWER":"by"}..
+000008c0: 2020 2020 5d0d 0a0d 0a20 2020 2022 2222      ]....    """
+000008d0: 0d0a 2020 2020 5573 6564 2066 6f72 2074  ..    Used for t
+000008e0: 6865 2073 6563 6f6e 6420 7061 7274 2077  he second part w
+000008f0: 6974 6820 2261 6e64 202e 2e2e 2220 0d0a  ith "and ..." ..
+00000900: 2020 2020 7365 6e74 656e 6365 203a 2069      sentence : i
+00000910: 7420 7761 7320 6465 7465 726d 696e 6564  t was determined
+00000920: 2061 6e64 2066 6f72 6d65 642e 0d0a 2020   and formed...  
+00000930: 2020 6465 7065 6e64 656e 6369 6573 203a    dependencies :
+00000940: 205b 276e 7375 626a 7061 7373 272c 2027   ['nsubjpass', '
+00000950: 6175 7870 6173 7327 2c20 2752 4f4f 5427  auxpass', 'ROOT'
+00000960: 2c20 2763 6327 2c20 2763 6f6e 6a27 2c20  , 'cc', 'conj', 
+00000970: 2770 756e 6374 275d 0d0a 2020 2020 7461  'punct']..    ta
+00000980: 6773 203a 205b 2750 5250 272c 2027 5642  gs : ['PRP', 'VB
+00000990: 4427 2c20 2756 424e 272c 2027 4343 272c  D', 'VBN', 'CC',
+000009a0: 2027 5642 4e27 2c20 272e 275d 0d0a 2020   'VBN', '.']..  
+000009b0: 2020 2222 220d 0a0d 0a20 2020 2070 6173    """....    pas
+000009c0: 7369 7665 5f72 756c 655f 3420 3d20 5b0d  sive_rule_4 = [.
+000009d0: 0a20 2020 2020 2020 207b 2244 4550 223a  .        {"DEP":
+000009e0: 2261 6476 636c 222c 2022 5441 4722 3a22  "advcl", "TAG":"
+000009f0: 5642 4e22 7d2c 0d0a 2020 2020 2020 2020  VBN"},..        
+00000a00: 7b22 4445 5022 3a20 2261 6765 6e74 222c  {"DEP": "agent",
+00000a10: 2022 5441 4722 3a22 494e 227d 2c0d 0a20   "TAG":"IN"},.. 
+00000a20: 2020 2020 2020 207b 224f 5022 3a22 2a22         {"OP":"*"
+00000a30: 7d2c 0d0a 2020 2020 2020 2020 7b22 4445  },..        {"DE
+00000a40: 5022 3a20 2270 6f62 6a22 7d2c 0d0a 2020  P": "pobj"},..  
+00000a50: 2020 5d0d 0a0d 0a20 2020 2022 2222 0d0a    ]....    """..
+00000a60: 2020 2020 7365 6e74 656e 6365 203a 206b      sentence : k
+00000a70: 696c 6c65 6420 6279 2074 6865 2070 6f6c  illed by the pol
+00000a80: 6963 652c 2068 6520 6e65 7665 7220 7468  ice, he never th
+00000a90: 6f75 6768 7420 7468 6973 2077 6f75 6c64  ought this would
+00000aa0: 2062 6520 6869 7320 656e 642e 0d0a 2020   be his end...  
+00000ab0: 2020 6465 7065 6e64 656e 6369 6573 203a    dependencies :
+00000ac0: 205b 2761 6476 636c 272c 2027 6167 656e   ['advcl', 'agen
+00000ad0: 7427 2c20 2764 6574 272c 2027 706f 626a  t', 'det', 'pobj
+00000ae0: 272c 2027 7075 6e63 7427 2c20 276e 7375  ', 'punct', 'nsu
+00000af0: 626a 272c 2027 6e65 6727 2c20 2752 4f4f  bj', 'neg', 'ROO
+00000b00: 5427 2c20 276e 7375 626a 272c 2027 6175  T', 'nsubj', 'au
+00000b10: 7827 2c20 2763 636f 6d70 272c 2027 706f  x', 'ccomp', 'po
+00000b20: 7373 272c 2027 6174 7472 275d 0d0a 2020  ss', 'attr']..  
+00000b30: 2020 7461 6773 203a 205b 2756 424e 272c    tags : ['VBN',
+00000b40: 2027 494e 272c 2027 4454 272c 2027 4e4e   'IN', 'DT', 'NN
+00000b50: 272c 2027 2c27 2c20 2750 5250 272c 2027  ', ',', 'PRP', '
+00000b60: 5242 272c 2027 5642 4427 2c20 2744 5427  RB', 'VBD', 'DT'
+00000b70: 2c20 274d 4427 2c20 2756 4227 2c20 2750  , 'MD', 'VB', 'P
+00000b80: 5250 2427 2c20 274e 4e27 5d0d 0a20 2020  RP$', 'NN']..   
+00000b90: 2022 2222 0d0a 0d0a 2020 2020 7061 7373   """....    pass
+00000ba0: 6976 655f 7275 6c65 5f35 203d 205b 0d0a  ive_rule_5 = [..
+00000bb0: 2020 2020 2020 2020 7b22 4445 5022 3a20          {"DEP": 
+00000bc0: 226e 7375 626a 227d 2c0d 0a20 2020 2020  "nsubj"},..     
+00000bd0: 2020 207b 2244 4550 223a 2022 524f 4f54     {"DEP": "ROOT
+00000be0: 227d 2c0d 0a20 2020 2020 2020 207b 2244  "},..        {"D
+00000bf0: 4550 223a 2022 6174 7472 222c 2022 5441  EP": "attr", "TA
+00000c00: 4722 3a20 2256 424e 222c 2022 4c45 4d4d  G": "VBN", "LEMM
+00000c10: 4122 3a7b 224e 4f54 5f49 4e22 203a 2076  A":{"NOT_IN" : v
+00000c20: 6572 6273 5f6c 6973 747d 7d2c 0d0a 2020  erbs_list}},..  
+00000c30: 2020 2020 2020 7b22 4445 5022 3a20 2270        {"DEP": "p
+00000c40: 7265 7022 2c20 2254 4147 223a 2022 494e  rep", "TAG": "IN
+00000c50: 222c 2022 4f50 223a 222a 227d 0d0a 2020  ", "OP":"*"}..  
+00000c60: 2020 5d0d 0a0d 0a20 2020 2022 2222 0d0a    ]....    """..
+00000c70: 2020 2020 7365 6e74 656e 6365 203a 2042      sentence : B
+00000c80: 6561 7273 2061 7265 2064 7265 616d 7420  ears are dreamt 
+00000c90: 6f66 2069 6e20 796f 7572 2066 616e 7461  of in your fanta
+00000ca0: 7369 6573 210d 0a20 2020 2064 6570 656e  sies!..    depen
+00000cb0: 6465 6e63 6965 7320 3a20 5b27 6e73 7562  dencies : ['nsub
+00000cc0: 6a70 6173 7327 2c20 2761 7578 7061 7373  jpass', 'auxpass
+00000cd0: 272c 2027 524f 4f54 272c 2027 7072 6570  ', 'ROOT', 'prep
+00000ce0: 272c 2027 7072 6570 272c 2027 706f 7373  ', 'prep', 'poss
+00000cf0: 272c 2027 706f 626a 272c 2027 7075 6e63  ', 'pobj', 'punc
+00000d00: 7427 5d0d 0a20 2020 2074 6167 7320 3a20  t']..    tags : 
+00000d10: 5b27 4e4e 5327 2c20 2756 4250 272c 2027  ['NNS', 'VBP', '
+00000d20: 5642 4e27 2c20 2749 4e27 2c20 2749 4e27  VBN', 'IN', 'IN'
+00000d30: 2c20 2750 5250 2427 2c20 274e 4e53 272c  , 'PRP$', 'NNS',
+00000d40: 2027 2e27 5d0d 0a20 2020 2022 2222 0d0a   '.']..    """..
+00000d50: 0d0a 0d0a 2020 2020 7061 7373 6976 655f  ....    passive_
+00000d60: 7275 6c65 5f36 203d 205b 0d0a 2020 2020  rule_6 = [..    
+00000d70: 2020 2020 7b22 4c45 4d4d 4122 3a20 7b22      {"LEMMA": {"
+00000d80: 494e 223a 2076 6572 6273 5f6c 6973 747d  IN": verbs_list}
+00000d90: 7d2c 0d0a 2020 2020 2020 2020 7b22 4c4f  },..        {"LO
+00000da0: 5745 5222 3a22 6279 227d 0d0a 2020 2020  WER":"by"}..    
+00000db0: 5d0d 0a0d 0a0d 0a20 2020 2022 2222 0d0a  ]......    """..
+00000dc0: 2020 2020 746f 2061 766f 6964 2074 6865      to avoid the
+00000dd0: 2063 6f6e 6675 7369 6f6e 2062 6574 7765   confusion betwe
+00000de0: 656e 2074 6865 2061 646a 6563 7469 7665  en the adjective
+00000df0: 2061 6e64 2070 6173 7369 7665 2076 6572   and passive ver
+00000e00: 7369 6f6e 206f 6620 7370 6563 6966 6963  sion of specific
+00000e10: 200d 0a20 2020 2076 6572 6273 2c20 7765   ..    verbs, we
+00000e20: 2064 6564 6963 6174 6564 2061 206e 6577   dedicated a new
+00000e30: 2072 756c 6520 746f 2073 6f6d 6520 7665   rule to some ve
+00000e40: 7262 7320 746f 2062 6520 6465 7465 6374  rbs to be detect
+00000e50: 6564 2077 6865 6e20 7573 6564 2077 6974  ed when used wit
+00000e60: 6820 0d0a 2020 2020 616e 2061 6765 6e74  h ..    an agent
+00000e70: 2028 6279 290d 0a0d 0a20 2020 2073 656e   (by)....    sen
+00000e80: 7465 6e63 6520 3a20 4e61 7475 7261 6c20  tence : Natural 
+00000e90: 7265 736f 7572 6365 7320 6172 6520 6578  resources are ex
+00000ea0: 6861 7573 7465 6420 6279 2068 756d 616e  hausted by human
+00000eb0: 732e 0d0a 2020 2020 6465 7065 6e64 656e  s...    dependen
+00000ec0: 6369 6573 203a 205b 2761 6d6f 6427 2c20  cies : ['amod', 
+00000ed0: 276e 7375 626a 7061 7373 272c 2027 6175  'nsubjpass', 'au
+00000ee0: 7870 6173 7327 2c20 2752 4f4f 5427 2c20  xpass', 'ROOT', 
+00000ef0: 2761 6765 6e74 272c 2027 706f 626a 275d  'agent', 'pobj']
+00000f00: 0d0a 2020 2020 7461 6773 203a 205b 274a  ..    tags : ['J
+00000f10: 4a27 2c20 274e 4e53 272c 2027 5642 5027  J', 'NNS', 'VBP'
+00000f20: 2c20 2756 424e 272c 2027 494e 272c 2027  , 'VBN', 'IN', '
+00000f30: 4e4e 5327 5d0d 0a20 2020 2022 2222 0d0a  NNS']..    """..
+00000f40: 0d0a 0d0a 2020 2020 2320 2d2d 2d2d 2d2d  ....    # ------
+00000f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 6164 6469  ------------addi
+00000f60: 6e67 2072 756c 6573 2074 6f20 7468 6520  ng rules to the 
+00000f70: 6d61 7463 6865 722d 2d2d 2d2d 2d2d 2d2d  matcher---------
+00000f80: 2d23 0d0a 0d0a 2020 2020 6d61 7463 6865  -#....    matche
+00000f90: 722e 6164 6428 2270 6173 7369 7665 5f72  r.add("passive_r
+00000fa0: 756c 655f 3122 2c20 5b70 6173 7369 7665  ule_1", [passive
+00000fb0: 5f72 756c 655f 315d 2c20 6772 6565 6479  _rule_1], greedy
+00000fc0: 3d27 4c4f 4e47 4553 5427 290d 0a20 2020  ='LONGEST')..   
+00000fd0: 206d 6174 6368 6572 2e61 6464 2822 7061   matcher.add("pa
+00000fe0: 7373 6976 655f 7275 6c65 5f32 222c 205b  ssive_rule_2", [
+00000ff0: 7061 7373 6976 655f 7275 6c65 5f32 5d2c  passive_rule_2],
+00001000: 2067 7265 6564 793d 274c 4f4e 4745 5354   greedy='LONGEST
+00001010: 2729 0d0a 2020 2020 6d61 7463 6865 722e  ')..    matcher.
+00001020: 6164 6428 2270 6173 7369 7665 5f72 756c  add("passive_rul
+00001030: 655f 3322 2c20 5b70 6173 7369 7665 5f72  e_3", [passive_r
+00001040: 756c 655f 335d 2c20 6772 6565 6479 3d27  ule_3], greedy='
+00001050: 4c4f 4e47 4553 5427 290d 0a20 2020 206d  LONGEST')..    m
+00001060: 6174 6368 6572 2e61 6464 2822 7061 7373  atcher.add("pass
+00001070: 6976 655f 7275 6c65 5f34 222c 205b 7061  ive_rule_4", [pa
+00001080: 7373 6976 655f 7275 6c65 5f34 5d2c 2067  ssive_rule_4], g
+00001090: 7265 6564 793d 274c 4f4e 4745 5354 2729  reedy='LONGEST')
+000010a0: 0d0a 2020 2020 6d61 7463 6865 722e 6164  ..    matcher.ad
+000010b0: 6428 2270 6173 7369 7665 5f72 756c 655f  d("passive_rule_
+000010c0: 3522 2c20 5b70 6173 7369 7665 5f72 756c  5", [passive_rul
+000010d0: 655f 355d 2c20 6772 6565 6479 3d27 4c4f  e_5], greedy='LO
+000010e0: 4e47 4553 5427 290d 0a20 2020 206d 6174  NGEST')..    mat
+000010f0: 6368 6572 2e61 6464 2822 7061 7373 6976  cher.add("passiv
+00001100: 655f 7275 6c65 5f36 222c 205b 7061 7373  e_rule_6", [pass
+00001110: 6976 655f 7275 6c65 5f36 5d2c 2067 7265  ive_rule_6], gre
+00001120: 6564 793d 274c 4f4e 4745 5354 2729 0d0a  edy='LONGEST')..
+00001130: 0d0a 2020 2020 2320 7072 696e 7428 274d  ..    # print('M
+00001140: 6174 6368 6572 2069 7320 6275 696c 742e  atcher is built.
+00001150: 2729 0d0a 0d0a 2020 2020 7265 7475 726e  ')....    return
+00001160: 206e 6c70 2c20 6d61 7463 6865 72          nlp, matcher
```

### Comparing `PassivePy-0.2.22/PassivePyCode/PassivePySrc/rules_for_truncated_passives.py` & `PassivePy-0.2.3/PassivePyCode/PassivePySrc/rules_for_truncated_passives.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,169 +1,214 @@
-00000000: 0d0a 2320 2043 6f70 7972 6967 6874 204d  ..#  Copyright M
-00000010: 6974 7261 204d 6972 7368 6166 6965 652c  itra Mirshafiee,
-00000020: 2032 3032 3220 4c69 6365 6e73 6564 2075   2022 Licensed u
-00000030: 6e64 6572 204d 4954 204c 6963 656e 7365  nder MIT License
-00000040: 2e0d 0a23 2020 5365 6520 7468 6520 4c49  ...#  See the LI
-00000050: 4345 4e53 452e 7478 7420 666f 7220 6d6f  CENSE.txt for mo
-00000060: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e0d  re information..
-00000070: 0a0d 0a69 6d70 6f72 7420 7370 6163 790d  ...import spacy.
-00000080: 0a66 726f 6d20 7370 6163 792e 6d61 7463  .from spacy.matc
-00000090: 6865 7220 696d 706f 7274 204d 6174 6368  her import Match
-000000a0: 6572 0d0a 0d0a 0d0a 6465 6620 6372 6561  er......def crea
-000000b0: 7465 5f6d 6174 6368 6572 5f74 7275 6e63  te_matcher_trunc
-000000c0: 6174 6564 286e 6c70 3a73 7061 6379 2e6c  ated(nlp:spacy.l
-000000d0: 616e 6775 6167 652e 4c61 6e67 7561 6765  anguage.Language
-000000e0: 203d 204e 6f6e 6529 3a0d 0a0d 0a20 2020   = None):....   
-000000f0: 2022 2222 6372 6561 7465 7320 6120 6d61   """creates a ma
-00000100: 7463 6865 7220 6f6e 2074 6865 2066 6f6c  tcher on the fol
-00000110: 6c6f 7769 6e67 2076 6f63 6162 756c 6172  lowing vocabular
-00000120: 7922 2222 0d0a 0d0a 2020 2020 6d61 7463  y"""....    matc
-00000130: 6865 7220 3d20 4d61 7463 6865 7228 6e6c  her = Matcher(nl
-00000140: 702e 766f 6361 6229 0d0a 0d0a 0d0a 2020  p.vocab)......  
-00000150: 2020 2320 6c69 7374 206f 6620 7665 7262    # list of verb
-00000160: 7320 7468 6174 2074 6865 6972 2061 646a  s that their adj
-00000170: 6563 7469 7665 2066 6f72 6d20 0d0a 2020  ective form ..  
-00000180: 2020 2320 6973 2073 6f6d 6574 696d 6573    # is sometimes
-00000190: 206d 6973 7461 6b65 6e20 6173 2061 2076   mistaken as a v
-000001a0: 6572 620d 0a20 2020 2076 6572 6273 5f6c  erb..    verbs_l
-000001b0: 6973 7420 3d20 5b22 6173 736f 6369 6174  ist = ["associat
-000001c0: 6522 2c20 2269 6e76 6f6c 7665 222c 2022  e", "involve", "
-000001d0: 6578 6861 7573 7422 2c20 2262 6173 6522  exhaust", "base"
-000001e0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-000001f0: 2020 2020 226c 6561 6422 2c20 2273 7475      "lead", "stu
-00000200: 6e22 2c20 226f 7665 7272 6174 6522 2c20  n", "overrate", 
-00000210: 2022 6669 6c6c 222c 2022 6265 6172 222c   "fill", "bear",
-00000220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000230: 2020 2263 6f6d 706c 6963 6174 6522 2c20    "complicate", 
-00000240: 2272 6573 6572 7665 222c 2022 636f 6d70  "reserve", "comp
-00000250: 6c69 6361 7465 222c 2022 6865 6174 222c  licate", "heat",
-00000260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000270: 2020 2273 6372 6577 222c 5d0d 0a0d 0a20    "screw",].... 
-00000280: 2020 2023 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     #------------
-00000290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7275  --------------ru
-000002a0: 6c65 732d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  les-------------
-000002b0: 2d2d 2d2d 2d2d 2d23 0d0a 0d0a 2020 2020  -------#....    
-000002c0: 0d0a 2020 2020 7061 7373 6976 655f 7275  ..    passive_ru
-000002d0: 6c65 5f31 203d 205b 0d0a 2020 2020 2020  le_1 = [..      
-000002e0: 2020 7b22 504f 5322 3a22 4155 5822 2c20    {"POS":"AUX", 
-000002f0: 2244 4550 223a 2022 6175 7822 2c20 224f  "DEP": "aux", "O
-00000300: 5022 3a22 2a22 7d2c 0d0a 2020 2020 2020  P":"*"},..      
-00000310: 2020 7b22 504f 5322 3a22 4155 5822 2c20    {"POS":"AUX", 
-00000320: 2244 4550 223a 2022 6175 7870 6173 7322  "DEP": "auxpass"
-00000330: 2c20 224f 5022 3a22 2b22 7d2c 0d0a 2020  , "OP":"+"},..  
-00000340: 2020 2020 2020 7b22 4445 5022 3a22 6e65        {"DEP":"ne
-00000350: 6722 2c20 2254 4147 223a 2252 4222 2c20  g", "TAG":"RB", 
-00000360: 224f 5022 3a22 2a22 7d2c 0d0a 2020 2020  "OP":"*"},..    
-00000370: 2020 2020 7b22 4445 5022 3a22 4859 5048      {"DEP":"HYPH
-00000380: 222c 2022 4f50 223a 222a 227d 2c0d 0a20  ", "OP":"*"},.. 
-00000390: 2020 2020 2020 207b 2244 4550 223a 2261         {"DEP":"a
-000003a0: 6476 6d6f 6422 2c20 2254 4147 223a 2252  dvmod", "TAG":"R
-000003b0: 4222 2c20 224f 5022 3a22 2a22 7d2c 0d0a  B", "OP":"*"},..
-000003c0: 2020 2020 2020 2020 7b22 504f 5322 3a22          {"POS":"
-000003d0: 5645 5242 222c 2022 5441 4722 3a22 5642  VERB", "TAG":"VB
-000003e0: 4e22 2c20 224c 454d 4d41 223a 7b22 4e4f  N", "LEMMA":{"NO
-000003f0: 545f 494e 2220 3a20 7665 7262 735f 6c69  T_IN" : verbs_li
-00000400: 7374 202b 205b 2762 6527 5d7d 7d2c 0d0a  st + ['be']}},..
-00000410: 2020 2020 2020 2020 7b22 4445 5022 3a22          {"DEP":"
-00000420: 6167 656e 7422 2c20 224f 5022 3a22 2122  agent", "OP":"!"
-00000430: 7d0d 0a20 2020 205d 0d0a 0d0a 2020 2020  }..    ]....    
-00000440: 2222 220d 0a20 2020 2073 656e 7465 6e63  """..    sentenc
-00000450: 6520 3a20 5468 6520 626f 6f6b 2077 6173  e : The book was
-00000460: 2072 6561 6420 6279 2068 696d 2e0d 0a20   read by him... 
-00000470: 2020 2064 6570 656e 6465 6e63 6965 7320     dependencies 
-00000480: 3a20 5b27 6465 7427 2c20 276e 7375 626a  : ['det', 'nsubj
-00000490: 7061 7373 272c 2027 6175 7870 6173 7327  pass', 'auxpass'
-000004a0: 2c20 2752 4f4f 5427 2c20 2761 6765 6e74  , 'ROOT', 'agent
-000004b0: 272c 2027 706f 626a 272c 2027 7075 6e63  ', 'pobj', 'punc
-000004c0: 7427 5d0d 0a20 2020 2054 6167 7320 3a20  t']..    Tags : 
-000004d0: 5b27 4454 272c 2027 4e4e 272c 2027 5642  ['DT', 'NN', 'VB
-000004e0: 4427 2c20 2756 424e 272c 2027 494e 272c  D', 'VBN', 'IN',
-000004f0: 2027 5052 5027 2c20 272e 275d 0d0a 2020   'PRP', '.']..  
-00000500: 2020 2222 220d 0a20 2020 2070 6173 7369    """..    passi
-00000510: 7665 5f72 756c 655f 3220 3d20 5b0d 0a20  ve_rule_2 = [.. 
-00000520: 2020 2020 2020 207b 2244 4550 223a 207b         {"DEP": {
-00000530: 2249 4e22 3a20 5b22 6174 7472 222c 2027  "IN": ["attr", '
-00000540: 6e73 7562 6a70 6173 7327 2c20 2761 7070  nsubjpass', 'app
-00000550: 6f73 275d 7d7d 2c0d 0a20 2020 2020 2020  os']}},..       
-00000560: 207b 2254 4147 223a 2022 5242 222c 2022   {"TAG": "RB", "
-00000570: 4445 5022 3a20 2261 6476 6d6f 6422 2c20  DEP": "advmod", 
-00000580: 224f 5022 203a 2022 2a22 7d2c 0d0a 2020  "OP" : "*"},..  
-00000590: 2020 2020 2020 7b22 4445 5022 3a20 2250        {"DEP": "P
-000005a0: 554e 4354 222c 2022 4f50 2220 3a20 222a  UNCT", "OP" : "*
-000005b0: 227d 2c0d 0a20 2020 2020 2020 207b 2254  "},..        {"T
-000005c0: 4147 223a 2022 5642 4e22 2c20 2244 4550  AG": "VBN", "DEP
-000005d0: 223a 2022 6163 6c22 2c22 4c45 4d4d 4122  ": "acl","LEMMA"
-000005e0: 3a20 7b22 4e4f 545f 494e 2220 3a20 7665  : {"NOT_IN" : ve
-000005f0: 7262 735f 6c69 7374 7d7d 2c0d 0a20 2020  rbs_list}},..   
-00000600: 2020 2020 207b 2244 4550 223a 2261 6765       {"DEP":"age
-00000610: 6e74 222c 2022 4f50 223a 2221 227d 0d0a  nt", "OP":"!"}..
-00000620: 2020 2020 5d0d 0a0d 0a20 2020 2022 2222      ]....    """
-00000630: 0d0a 2020 2020 7365 6e74 656e 6365 203a  ..    sentence :
-00000640: 2074 6865 7265 2077 6173 206e 6f20 6368   there was no ch
-00000650: 616e 6765 2064 6574 6563 7465 6420 696e  ange detected in
-00000660: 2068 6572 2062 6568 6176 696f 722e 0d0a   her behavior...
-00000670: 2020 2020 6465 7065 6e64 656e 6369 6573      dependencies
-00000680: 203a 205b 2765 7870 6c27 2c20 2752 4f4f   : ['expl', 'ROO
-00000690: 5427 2c20 2764 6574 272c 2027 6174 7472  T', 'det', 'attr
-000006a0: 272c 2027 6163 6c27 2c20 2770 7265 7027  ', 'acl', 'prep'
-000006b0: 2c20 2770 6f73 7327 2c20 2770 6f62 6a27  , 'poss', 'pobj'
-000006c0: 2c20 2770 756e 6374 275d 0d0a 2020 2020  , 'punct']..    
-000006d0: 7461 6773 203a 205b 2745 5827 2c20 2756  tags : ['EX', 'V
-000006e0: 4244 272c 2027 4454 272c 2027 4e4e 272c  BD', 'DT', 'NN',
-000006f0: 2027 5642 4e27 2c20 2749 4e27 2c20 2750   'VBN', 'IN', 'P
-00000700: 5250 2427 2c20 274e 4e27 2c20 272e 275d  RP$', 'NN', '.']
-00000710: 0d0a 2020 2020 2222 220d 0a0d 0a0d 0a20  ..    """...... 
-00000720: 2020 2070 6173 7369 7665 5f72 756c 655f     passive_rule_
-00000730: 3320 3d20 5b0d 0a20 2020 2020 2020 207b  3 = [..        {
-00000740: 2250 4f53 223a 2241 5558 222c 2022 4445  "POS":"AUX", "DE
-00000750: 5022 3a20 2261 7578 222c 2022 4f50 223a  P": "aux", "OP":
-00000760: 222a 227d 2c0d 0a20 2020 2020 2020 207b  "*"},..        {
-00000770: 2250 4f53 223a 2241 5558 222c 2022 4445  "POS":"AUX", "DE
-00000780: 5022 3a20 2261 7578 7061 7373 222c 2022  P": "auxpass", "
-00000790: 4f50 223a 222b 227d 2c0d 0a20 2020 2020  OP":"+"},..     
-000007a0: 2020 207b 2244 4550 223a 226e 6567 222c     {"DEP":"neg",
-000007b0: 2022 5441 4722 3a22 5242 222c 2022 4f50   "TAG":"RB", "OP
-000007c0: 223a 222a 227d 2c0d 0a20 2020 2020 2020  ":"*"},..       
-000007d0: 207b 2244 4550 223a 2248 5950 4822 2c20   {"DEP":"HYPH", 
-000007e0: 224f 5022 3a22 2a22 7d2c 0d0a 2020 2020  "OP":"*"},..    
-000007f0: 2020 2020 7b22 4445 5022 3a22 6164 766d      {"DEP":"advm
-00000800: 6f64 222c 2022 5441 4722 3a22 5242 222c  od", "TAG":"RB",
-00000810: 2022 4f50 223a 222a 227d 2c0d 0a20 2020   "OP":"*"},..   
-00000820: 2020 2020 207b 2250 4f53 223a 2256 4552       {"POS":"VER
-00000830: 4222 2c20 2244 4550 223a 2252 4f4f 5422  B", "DEP":"ROOT"
-00000840: 2c20 224c 454d 4d41 223a 7b22 4e4f 545f  , "LEMMA":{"NOT_
-00000850: 494e 2220 3a20 7665 7262 735f 6c69 7374  IN" : verbs_list
-00000860: 7d7d 2c0d 0a20 2020 2020 2020 207b 2244  }},..        {"D
-00000870: 4550 223a 2263 6322 7d2c 0d0a 2020 2020  EP":"cc"},..    
-00000880: 2020 2020 7b22 4445 5022 3a22 6164 766d      {"DEP":"advm
-00000890: 6f64 222c 2022 5441 4722 3a22 5642 4e22  od", "TAG":"VBN"
-000008a0: 2c20 224f 5022 3a20 222a 222c 2022 4c45  , "OP": "*", "LE
-000008b0: 4d4d 4122 3a20 7b22 4e4f 545f 494e 223a  MMA": {"NOT_IN":
-000008c0: 5b22 7072 6522 5d7d 7d2c 0d0a 2020 2020  ["pre"]}},..    
-000008d0: 2020 2020 7b22 4445 5022 3a20 2263 6f6e      {"DEP": "con
-000008e0: 6a22 2c20 224c 454d 4d41 223a 7b22 4e4f  j", "LEMMA":{"NO
-000008f0: 545f 494e 2220 3a20 7665 7262 735f 6c69  T_IN" : verbs_li
-00000900: 7374 7d7d 2c0d 0a20 2020 2020 2020 207b  st}},..        {
-00000910: 2244 4550 223a 2261 6765 6e74 222c 2022  "DEP":"agent", "
-00000920: 4f50 223a 2221 227d 0d0a 2020 2020 5d0d  OP":"!"}..    ].
-00000930: 0a0d 0a20 2020 2023 202d 2d2d 2d2d 2d2d  ...    # -------
-00000940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d61 6464 696e  -----------addin
-00000950: 6720 7275 6c65 7320 746f 2074 6865 206d  g rules to the m
-00000960: 6174 6368 6572 2d2d 2d2d 2d2d 2d2d 2d2d  atcher----------
-00000970: 230d 0a0d 0a20 2020 206d 6174 6368 6572  #....    matcher
-00000980: 2e61 6464 2822 7061 7373 6976 655f 7275  .add("passive_ru
-00000990: 6c65 5f31 222c 205b 7061 7373 6976 655f  le_1", [passive_
-000009a0: 7275 6c65 5f31 5d2c 2067 7265 6564 793d  rule_1], greedy=
-000009b0: 274c 4f4e 4745 5354 2729 0d0a 2020 2020  'LONGEST')..    
-000009c0: 6d61 7463 6865 722e 6164 6428 2270 6173  matcher.add("pas
-000009d0: 7369 7665 5f72 756c 655f 3222 2c20 5b70  sive_rule_2", [p
-000009e0: 6173 7369 7665 5f72 756c 655f 325d 2c20  assive_rule_2], 
-000009f0: 6772 6565 6479 3d27 4c4f 4e47 4553 5427  greedy='LONGEST'
-00000a00: 290d 0a20 2020 206d 6174 6368 6572 2e61  )..    matcher.a
-00000a10: 6464 2822 7061 7373 6976 655f 7275 6c65  dd("passive_rule
-00000a20: 5f33 222c 205b 7061 7373 6976 655f 7275  _3", [passive_ru
-00000a30: 6c65 5f33 5d2c 2067 7265 6564 793d 274c  le_3], greedy='L
-00000a40: 4f4e 4745 5354 2729 0d0a 0d0a 2020 2020  ONGEST')....    
-00000a50: 2320 7072 696e 7428 274d 6174 6368 6572  # print('Matcher
-00000a60: 2069 7320 6275 696c 742e 2729 0d0a 0d0a   is built.')....
-00000a70: 2020 2020 7265 7475 726e 206d 6174 6368      return match
-00000a80: 6572 0d0a                                er..
+00000000: 696d 706f 7274 2073 7061 6379 0d0a 6672  import spacy..fr
+00000010: 6f6d 2073 7061 6379 2e6d 6174 6368 6572  om spacy.matcher
+00000020: 2069 6d70 6f72 7420 4d61 7463 6865 720d   import Matcher.
+00000030: 0a0d 0a0d 0a0d 0a64 6566 2063 7265 6174  .......def creat
+00000040: 655f 6d61 7463 6865 725f 7472 756e 6361  e_matcher_trunca
+00000050: 7465 6428 7370 6163 795f 6d6f 6465 6c20  ted(spacy_model 
+00000060: 3d20 2265 6e5f 636f 7265 5f77 6562 5f6c  = "en_core_web_l
+00000070: 6722 293a 0d0a 0d0a 2020 2020 2222 2263  g"):....    """c
+00000080: 7265 6174 6573 2061 206d 6174 6368 6572  reates a matcher
+00000090: 206f 6e20 7468 6520 666f 6c6c 6f77 696e   on the followin
+000000a0: 6720 766f 6361 6275 6c61 7279 2222 220d  g vocabulary""".
+000000b0: 0a20 2020 206e 6c70 203d 2073 7061 6379  .    nlp = spacy
+000000c0: 2e6c 6f61 6428 7370 6163 795f 6d6f 6465  .load(spacy_mode
+000000d0: 6c2c 2064 6973 6162 6c65 3d5b 226e 6572  l, disable=["ner
+000000e0: 225d 290d 0a20 2020 206d 6174 6368 6572  "])..    matcher
+000000f0: 203d 204d 6174 6368 6572 286e 6c70 2e76   = Matcher(nlp.v
+00000100: 6f63 6162 290d 0a0d 0a20 2020 2023 206c  ocab)....    # l
+00000110: 6973 7420 6f66 2076 6572 6273 2074 6861  ist of verbs tha
+00000120: 7420 7468 6569 7220 6164 6a65 6374 6976  t their adjectiv
+00000130: 6520 666f 726d 200d 0a20 2020 2023 2069  e form ..    # i
+00000140: 7320 736f 6d65 7469 6d65 7320 6d69 7374  s sometimes mist
+00000150: 616b 656e 2061 7320 6120 7665 7262 0d0a  aken as a verb..
+00000160: 2020 2020 7665 7262 735f 6c69 7374 203d      verbs_list =
+00000170: 205b 2261 7373 6f63 6961 7465 222c 2022   ["associate", "
+00000180: 696e 766f 6c76 6522 2c20 2265 7868 6175  involve", "exhau
+00000190: 7374 222c 2022 6261 7365 222c 200d 0a20  st", "base", .. 
+000001a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000001b0: 6c65 6164 222c 2022 7374 756e 222c 2022  lead", "stun", "
+000001c0: 6f76 6572 7261 7465 222c 2020 2266 696c  overrate",  "fil
+000001d0: 6c22 2c20 2262 6561 7222 2c0d 0a20 2020  l", "bear",..   
+000001e0: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+000001f0: 6d70 6c69 6361 7465 222c 2022 7265 7365  mplicate", "rese
+00000200: 7276 6522 2c20 2263 6f6d 706c 6963 6174  rve", "complicat
+00000210: 6522 2c20 2268 6561 7422 2c0d 0a20 2020  e", "heat",..   
+00000220: 2020 2020 2020 2020 2020 2020 2022 7363               "sc
+00000230: 7265 7722 2c5d 0d0a 0d0a 2020 2020 232d  rew",]....    #-
+00000240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000250: 2d2d 2d2d 2d2d 2d2d 2d72 756c 6573 2d2d  ---------rules--
+00000260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000270: 2d2d 230d 0a0d 0a20 2020 200d 0a20 2020  --#....    ..   
+00000280: 2070 6173 7369 7665 5f72 756c 655f 3120   passive_rule_1 
+00000290: 3d20 5b0d 0a20 2020 2020 2020 207b 2250  = [..        {"P
+000002a0: 4f53 223a 2241 5558 222c 2022 4445 5022  OS":"AUX", "DEP"
+000002b0: 3a20 2261 7578 222c 2022 4f50 223a 222a  : "aux", "OP":"*
+000002c0: 227d 2c0d 0a20 2020 2020 2020 207b 2250  "},..        {"P
+000002d0: 4f53 223a 2241 5558 222c 2022 4445 5022  OS":"AUX", "DEP"
+000002e0: 3a20 2261 7578 7061 7373 222c 2022 4f50  : "auxpass", "OP
+000002f0: 223a 222b 227d 2c0d 0a20 2020 2020 2020  ":"+"},..       
+00000300: 207b 2244 4550 223a 226e 6567 222c 2022   {"DEP":"neg", "
+00000310: 5441 4722 3a22 5242 222c 2022 4f50 223a  TAG":"RB", "OP":
+00000320: 222a 227d 2c0d 0a20 2020 2020 2020 207b  "*"},..        {
+00000330: 2244 4550 223a 2248 5950 4822 2c20 224f  "DEP":"HYPH", "O
+00000340: 5022 3a22 2a22 7d2c 0d0a 2020 2020 2020  P":"*"},..      
+00000350: 2020 7b22 4445 5022 3a22 6164 766d 6f64    {"DEP":"advmod
+00000360: 222c 2022 5441 4722 3a22 5242 222c 2022  ", "TAG":"RB", "
+00000370: 4f50 223a 222a 227d 2c0d 0a20 2020 2020  OP":"*"},..     
+00000380: 2020 207b 2250 4f53 223a 2256 4552 4222     {"POS":"VERB"
+00000390: 2c20 2254 4147 223a 2256 424e 222c 2022  , "TAG":"VBN", "
+000003a0: 4c45 4d4d 4122 3a7b 224e 4f54 5f49 4e22  LEMMA":{"NOT_IN"
+000003b0: 203a 2076 6572 6273 5f6c 6973 7420 2b20   : verbs_list + 
+000003c0: 5b27 6265 275d 7d7d 2c0d 0a20 2020 2020  ['be']}},..     
+000003d0: 2020 207b 2244 4550 223a 2261 6765 6e74     {"DEP":"agent
+000003e0: 222c 2022 4f50 223a 2221 227d 0d0a 2020  ", "OP":"!"}..  
+000003f0: 2020 5d0d 0a0d 0a20 2020 2022 2222 0d0a    ]....    """..
+00000400: 2020 2020 7365 6e74 656e 6365 203a 2054      sentence : T
+00000410: 6865 2062 6f6f 6b20 7761 7320 7265 6164  he book was read
+00000420: 2062 7920 6869 6d2e 0d0a 2020 2020 6465   by him...    de
+00000430: 7065 6e64 656e 6369 6573 203a 205b 2764  pendencies : ['d
+00000440: 6574 272c 2027 6e73 7562 6a70 6173 7327  et', 'nsubjpass'
+00000450: 2c20 2761 7578 7061 7373 272c 2027 524f  , 'auxpass', 'RO
+00000460: 4f54 272c 2027 6167 656e 7427 2c20 2770  OT', 'agent', 'p
+00000470: 6f62 6a27 2c20 2770 756e 6374 275d 0d0a  obj', 'punct']..
+00000480: 2020 2020 5461 6773 203a 205b 2744 5427      Tags : ['DT'
+00000490: 2c20 274e 4e27 2c20 2756 4244 272c 2027  , 'NN', 'VBD', '
+000004a0: 5642 4e27 2c20 2749 4e27 2c20 2750 5250  VBN', 'IN', 'PRP
+000004b0: 272c 2027 2e27 5d0d 0a20 2020 2022 2222  ', '.']..    """
+000004c0: 0d0a 2020 2020 7061 7373 6976 655f 7275  ..    passive_ru
+000004d0: 6c65 5f32 203d 205b 0d0a 2020 2020 2020  le_2 = [..      
+000004e0: 2020 7b22 4445 5022 3a20 7b22 494e 223a    {"DEP": {"IN":
+000004f0: 205b 2261 7474 7222 2c20 276e 7375 626a   ["attr", 'nsubj
+00000500: 7061 7373 272c 2027 6170 706f 7327 5d7d  pass', 'appos']}
+00000510: 7d2c 0d0a 2020 2020 2020 2020 7b22 5441  },..        {"TA
+00000520: 4722 3a20 2252 4222 2c20 2244 4550 223a  G": "RB", "DEP":
+00000530: 2022 6164 766d 6f64 222c 2022 4f50 2220   "advmod", "OP" 
+00000540: 3a20 222a 227d 2c0d 0a20 2020 2020 2020  : "*"},..       
+00000550: 207b 2244 4550 223a 2022 5055 4e43 5422   {"DEP": "PUNCT"
+00000560: 2c20 224f 5022 203a 2022 2a22 7d2c 0d0a  , "OP" : "*"},..
+00000570: 2020 2020 2020 2020 7b22 5441 4722 3a20          {"TAG": 
+00000580: 2256 424e 222c 2022 4445 5022 3a20 2261  "VBN", "DEP": "a
+00000590: 636c 222c 224c 454d 4d41 223a 207b 224e  cl","LEMMA": {"N
+000005a0: 4f54 5f49 4e22 203a 2076 6572 6273 5f6c  OT_IN" : verbs_l
+000005b0: 6973 747d 7d2c 0d0a 2020 2020 2020 2020  ist}},..        
+000005c0: 7b22 4445 5022 3a22 6167 656e 7422 2c20  {"DEP":"agent", 
+000005d0: 224f 5022 3a22 2122 7d0d 0a20 2020 205d  "OP":"!"}..    ]
+000005e0: 0d0a 0d0a 2020 2020 2222 220d 0a20 2020  ....    """..   
+000005f0: 2073 656e 7465 6e63 6520 3a20 7468 6572   sentence : ther
+00000600: 6520 7761 7320 6e6f 2063 6861 6e67 6520  e was no change 
+00000610: 6465 7465 6374 6564 2069 6e20 6865 7220  detected in her 
+00000620: 6265 6861 7669 6f72 2e0d 0a20 2020 2064  behavior...    d
+00000630: 6570 656e 6465 6e63 6965 7320 3a20 5b27  ependencies : ['
+00000640: 6578 706c 272c 2027 524f 4f54 272c 2027  expl', 'ROOT', '
+00000650: 6465 7427 2c20 2761 7474 7227 2c20 2761  det', 'attr', 'a
+00000660: 636c 272c 2027 7072 6570 272c 2027 706f  cl', 'prep', 'po
+00000670: 7373 272c 2027 706f 626a 272c 2027 7075  ss', 'pobj', 'pu
+00000680: 6e63 7427 5d0d 0a20 2020 2074 6167 7320  nct']..    tags 
+00000690: 3a20 5b27 4558 272c 2027 5642 4427 2c20  : ['EX', 'VBD', 
+000006a0: 2744 5427 2c20 274e 4e27 2c20 2756 424e  'DT', 'NN', 'VBN
+000006b0: 272c 2027 494e 272c 2027 5052 5024 272c  ', 'IN', 'PRP$',
+000006c0: 2027 4e4e 272c 2027 2e27 5d0d 0a20 2020   'NN', '.']..   
+000006d0: 2022 2222 0d0a 0d0a 0d0a 2020 2020 7061   """......    pa
+000006e0: 7373 6976 655f 7275 6c65 5f33 203d 205b  ssive_rule_3 = [
+000006f0: 0d0a 2020 2020 2020 2020 7b22 504f 5322  ..        {"POS"
+00000700: 3a22 4155 5822 2c20 2244 4550 223a 2022  :"AUX", "DEP": "
+00000710: 6175 7822 2c20 224f 5022 3a22 2a22 7d2c  aux", "OP":"*"},
+00000720: 0d0a 2020 2020 2020 2020 7b22 504f 5322  ..        {"POS"
+00000730: 3a22 4155 5822 2c20 2244 4550 223a 2022  :"AUX", "DEP": "
+00000740: 6175 7870 6173 7322 2c20 224f 5022 3a22  auxpass", "OP":"
+00000750: 2b22 7d2c 0d0a 2020 2020 2020 2020 7b22  +"},..        {"
+00000760: 4445 5022 3a22 6e65 6722 2c20 2254 4147  DEP":"neg", "TAG
+00000770: 223a 2252 4222 2c20 224f 5022 3a22 2a22  ":"RB", "OP":"*"
+00000780: 7d2c 0d0a 2020 2020 2020 2020 7b22 4445  },..        {"DE
+00000790: 5022 3a22 4859 5048 222c 2022 4f50 223a  P":"HYPH", "OP":
+000007a0: 222a 227d 2c0d 0a20 2020 2020 2020 207b  "*"},..        {
+000007b0: 2244 4550 223a 2261 6476 6d6f 6422 2c20  "DEP":"advmod", 
+000007c0: 2254 4147 223a 2252 4222 2c20 224f 5022  "TAG":"RB", "OP"
+000007d0: 3a22 2a22 7d2c 0d0a 2020 2020 2020 2020  :"*"},..        
+000007e0: 7b22 504f 5322 3a22 5645 5242 222c 2022  {"POS":"VERB", "
+000007f0: 4445 5022 3a22 524f 4f54 222c 2022 4c45  DEP":"ROOT", "LE
+00000800: 4d4d 4122 3a7b 224e 4f54 5f49 4e22 203a  MMA":{"NOT_IN" :
+00000810: 2076 6572 6273 5f6c 6973 747d 7d2c 0d0a   verbs_list}},..
+00000820: 2020 2020 2020 2020 7b22 4445 5022 3a22          {"DEP":"
+00000830: 6363 227d 2c0d 0a20 2020 2020 2020 207b  cc"},..        {
+00000840: 2244 4550 223a 2261 6476 6d6f 6422 2c20  "DEP":"advmod", 
+00000850: 2254 4147 223a 2256 424e 222c 2022 4f50  "TAG":"VBN", "OP
+00000860: 223a 2022 2a22 2c20 224c 454d 4d41 223a  ": "*", "LEMMA":
+00000870: 207b 224e 4f54 5f49 4e22 3a5b 2270 7265   {"NOT_IN":["pre
+00000880: 225d 7d7d 2c0d 0a20 2020 2020 2020 207b  "]}},..        {
+00000890: 2244 4550 223a 2022 636f 6e6a 222c 2022  "DEP": "conj", "
+000008a0: 4c45 4d4d 4122 3a7b 224e 4f54 5f49 4e22  LEMMA":{"NOT_IN"
+000008b0: 203a 2076 6572 6273 5f6c 6973 747d 7d2c   : verbs_list}},
+000008c0: 0d0a 2020 2020 2020 2020 7b22 4445 5022  ..        {"DEP"
+000008d0: 3a22 6167 656e 7422 2c20 224f 5022 3a22  :"agent", "OP":"
+000008e0: 2122 7d0d 0a20 2020 205d 0d0a 0d0a 2020  !"}..    ]....  
+000008f0: 2020 2222 220d 0a20 2020 2055 7365 6420    """..    Used 
+00000900: 666f 7220 7468 6520 7365 636f 6e64 2070  for the second p
+00000910: 6172 7420 7769 7468 2022 616e 6420 2e2e  art with "and ..
+00000920: 2e22 200d 0a20 2020 2073 656e 7465 6e63  ." ..    sentenc
+00000930: 6520 3a20 6974 2077 6173 2064 6574 6572  e : it was deter
+00000940: 6d69 6e65 6420 616e 6420 666f 726d 6564  mined and formed
+00000950: 2e0d 0a20 2020 2064 6570 656e 6465 6e63  ...    dependenc
+00000960: 6965 7320 3a20 5b27 6e73 7562 6a70 6173  ies : ['nsubjpas
+00000970: 7327 2c20 2761 7578 7061 7373 272c 2027  s', 'auxpass', '
+00000980: 524f 4f54 272c 2027 6363 272c 2027 636f  ROOT', 'cc', 'co
+00000990: 6e6a 272c 2027 7075 6e63 7427 5d0d 0a20  nj', 'punct'].. 
+000009a0: 2020 2074 6167 7320 3a20 5b27 5052 5027     tags : ['PRP'
+000009b0: 2c20 2756 4244 272c 2027 5642 4e27 2c20  , 'VBD', 'VBN', 
+000009c0: 2743 4327 2c20 2756 424e 272c 2027 2e27  'CC', 'VBN', '.'
+000009d0: 5d0d 0a20 2020 2022 2222 0d0a 0d0a 0d0a  ]..    """......
+000009e0: 2020 2020 7061 7373 6976 655f 7275 6c65      passive_rule
+000009f0: 5f35 203d 205b 0d0a 2020 2020 2020 2020  _5 = [..        
+00000a00: 7b22 4445 5022 3a20 226e 7375 626a 227d  {"DEP": "nsubj"}
+00000a10: 2c0d 0a20 2020 2020 2020 207b 2244 4550  ,..        {"DEP
+00000a20: 223a 2022 524f 4f54 227d 2c0d 0a20 2020  ": "ROOT"},..   
+00000a30: 2020 2020 207b 2244 4550 223a 2022 6174       {"DEP": "at
+00000a40: 7472 222c 2022 5441 4722 3a20 2256 424e  tr", "TAG": "VBN
+00000a50: 222c 2022 4c45 4d4d 4122 3a7b 224e 4f54  ", "LEMMA":{"NOT
+00000a60: 5f49 4e22 203a 2076 6572 6273 5f6c 6973  _IN" : verbs_lis
+00000a70: 747d 7d2c 0d0a 2020 2020 2020 2020 7b22  t}},..        {"
+00000a80: 4445 5022 3a20 2270 7265 7022 2c20 2254  DEP": "prep", "T
+00000a90: 4147 223a 2022 494e 222c 2022 4f50 223a  AG": "IN", "OP":
+00000aa0: 222a 227d 2c0d 0a20 2020 2020 2020 207b  "*"},..        {
+00000ab0: 2244 4550 223a 2261 6765 6e74 222c 2022  "DEP":"agent", "
+00000ac0: 4f50 223a 2221 227d 0d0a 2020 2020 5d0d  OP":"!"}..    ].
+00000ad0: 0a0d 0a20 2020 2022 2222 0d0a 2020 2020  ...    """..    
+00000ae0: 7365 6e74 656e 6365 203a 2042 6561 7273  sentence : Bears
+00000af0: 2061 7265 2064 7265 616d 7420 6f66 2069   are dreamt of i
+00000b00: 6e20 796f 7572 2066 616e 7461 7369 6573  n your fantasies
+00000b10: 210d 0a20 2020 2064 6570 656e 6465 6e63  !..    dependenc
+00000b20: 6965 7320 3a20 5b27 6e73 7562 6a70 6173  ies : ['nsubjpas
+00000b30: 7327 2c20 2761 7578 7061 7373 272c 2027  s', 'auxpass', '
+00000b40: 524f 4f54 272c 2027 7072 6570 272c 2027  ROOT', 'prep', '
+00000b50: 7072 6570 272c 2027 706f 7373 272c 2027  prep', 'poss', '
+00000b60: 706f 626a 272c 2027 7075 6e63 7427 5d0d  pobj', 'punct'].
+00000b70: 0a20 2020 2074 6167 7320 3a20 5b27 4e4e  .    tags : ['NN
+00000b80: 5327 2c20 2756 4250 272c 2027 5642 4e27  S', 'VBP', 'VBN'
+00000b90: 2c20 2749 4e27 2c20 2749 4e27 2c20 2750  , 'IN', 'IN', 'P
+00000ba0: 5250 2427 2c20 274e 4e53 272c 2027 2e27  RP$', 'NNS', '.'
+00000bb0: 5d0d 0a20 2020 2022 2222 0d0a 0d0a 0d0a  ]..    """......
+00000bc0: 0d0a 2020 2020 2320 2d2d 2d2d 2d2d 2d2d  ..    # --------
+00000bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 6164 6469 6e67  ----------adding
+00000be0: 2072 756c 6573 2074 6f20 7468 6520 6d61   rules to the ma
+00000bf0: 7463 6865 722d 2d2d 2d2d 2d2d 2d2d 2d23  tcher----------#
+00000c00: 0d0a 0d0a 2020 2020 6d61 7463 6865 722e  ....    matcher.
+00000c10: 6164 6428 2270 6173 7369 7665 5f72 756c  add("passive_rul
+00000c20: 655f 3122 2c20 5b70 6173 7369 7665 5f72  e_1", [passive_r
+00000c30: 756c 655f 315d 2c20 6772 6565 6479 3d27  ule_1], greedy='
+00000c40: 4c4f 4e47 4553 5427 290d 0a20 2020 206d  LONGEST')..    m
+00000c50: 6174 6368 6572 2e61 6464 2822 7061 7373  atcher.add("pass
+00000c60: 6976 655f 7275 6c65 5f32 222c 205b 7061  ive_rule_2", [pa
+00000c70: 7373 6976 655f 7275 6c65 5f32 5d2c 2067  ssive_rule_2], g
+00000c80: 7265 6564 793d 274c 4f4e 4745 5354 2729  reedy='LONGEST')
+00000c90: 0d0a 2020 2020 6d61 7463 6865 722e 6164  ..    matcher.ad
+00000ca0: 6428 2270 6173 7369 7665 5f72 756c 655f  d("passive_rule_
+00000cb0: 3322 2c20 5b70 6173 7369 7665 5f72 756c  3", [passive_rul
+00000cc0: 655f 335d 2c20 6772 6565 6479 3d27 4c4f  e_3], greedy='LO
+00000cd0: 4e47 4553 5427 290d 0a20 2020 206d 6174  NGEST')..    mat
+00000ce0: 6368 6572 2e61 6464 2822 7061 7373 6976  cher.add("passiv
+00000cf0: 655f 7275 6c65 5f35 222c 205b 7061 7373  e_rule_5", [pass
+00000d00: 6976 655f 7275 6c65 5f35 5d2c 2067 7265  ive_rule_5], gre
+00000d10: 6564 793d 274c 4f4e 4745 5354 2729 0d0a  edy='LONGEST')..
+00000d20: 0d0a 2020 2020 2320 7072 696e 7428 274d  ..    # print('M
+00000d30: 6174 6368 6572 2069 7320 6275 696c 742e  atcher is built.
+00000d40: 2729 0d0a 0d0a 2020 2020 7265 7475 726e  ')....    return
+00000d50: 206e 6c70 2c20 6d61 7463 6865 72          nlp, matcher
```

### Comparing `PassivePy-0.2.22/README.md` & `PassivePy-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # PassivePy: A Tool to Automatically Identify Passive Voice in Big Text Data
 
-**_This repository is the code of the following paper, so if you use this package, please cite the work as:
-Sepehri, A., Markowitz, D. M., & Mir, M. (2022, February 3). PassivePy: A Tool to Automatically Identify Passive Voice in Big Text Data. [Preprint available](https://psyarxiv.com/bwp3t/)**
-
 
 Our aim with this work is to create a reliable (e.g., passive voice judgments are consistent), valid (e.g., passive voice judgments are accurate), flexible (e.g., texts can be assessed at different units of analysis), replicable (e.g., the approach can be performed by a range of research teams with varying levels of computational expertise), and scalable way (e.g., small and large collections of texts can be analyzed) to capture passive voice from different corpora for social and psychological evaluations of text. To achieve these aims, we introduce PassivePy, a fully transparent and documented Python library.
 
 For accessing the datasets in our paper, please click on [this link](https://osf.io/j2b6u/?view_only=0e78d7f4028041b693d6b64547b514ca). 
 
-If you haven't used Python before or need detailed instructions about how to use this package please visit [our website](https://passivepy.streamlit.app/).
+If you haven't used Python before or need detailed instructions about how to use this package please visit [our website](https://mitramir55.github.io/PassivePyWeb/).
 
 
 First we have to install the requirements in the following way (all requirements are needed for spaCy or other libraries we use.):
 ```
 !pip install -r https://raw.githubusercontent.com/mitramir55/PassivePy/main/PassivePyCode/PassivePySrc/requirements_lg.txt
-!pip install PassivePy==0.2.22
+!pip install PassivePy==0.2.3
 
 ```
 Then, import PassivePy and initiate the analyzer:
 
 ```
 from PassivePySrc import PassivePy
 
-passivepy = PassivePy.PassivePyAnalyzer(spacy_model = "en_core_web_lg")
+spacy_model = "en_core_web_lg"
+passivepy = PassivePy.PassivePyAnalyzer(spacy_model)
 ```
 Use passivepy for single sentences:
 ```
 # Try changing the sentence below:
 sample_text = "The painting has been drawn."
 passivepy.passivepy.match_text(sample_text, full_passive=True, truncated_passive=True)
 ```
@@ -74,15 +72,15 @@
 sentence : The detected sentence
 binary : Whether a passive was detected in that sentence
 passive_match(es) : The part of the record detected as passive voice
 raw_passive_count : Number of passive forms detected in the sentence
 
 ```
 
-If you needed to analyze each token of a sentence, i.g., print out the `DEP` (dependency), `POS` (coarse-grained part of speech tags), `TAG` (fine-grained part of speech tags), `LEMMA` (canonical form) of a word,  you can use the `parse_sentence` method of passivepy in the following way:
+If you needed to analyze each token of a sentence, i.g., print out the `DEP` (dependency), `POS` (coarse-grained POS tags), `TAG` (fine-grained part of speech tags), `LEMMA` (canonical form) of a word,  you can use the `parse_sentence` method of passivepy in the following way:
 
 ```
 sample_sentence = "She has been killed"
 passivepy.parse_sentence(sample_sentence)
 ```
 And the output will be like the sample below:
 ```
@@ -97,10 +95,7 @@
 
 
 If you do not need any columns to be appended to the main dataset, simply add `add_other_columns = False`, or if you don't what the percentages to show up add `percentage_of_passive_sentences = False` in any of the following functions.
 
 
 Accuracy on the CoLA dataset: 0.97
 Accuracy on the CrowdSource Dataset: 0.98
-
-
-
```

### Comparing `PassivePy-0.2.22/setup.py` & `PassivePy-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="PassivePy",
-    version="0.2.22",
+    version="0.2.3",
     author="Mitra Mirshafiee",
     author_email="mitra.mirshafiee@gmail.com",
     description="A package for processing large corpora and detecting passive voice.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mitramir55/PassivePy",
     project_urls={
```

