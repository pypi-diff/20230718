# Comparing `tmp/selfcheckgpt-0.1.3.tar.gz` & `tmp/selfcheckgpt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcheckgpt-0.1.3.tar", last modified: Thu May 25 14:47:15 2023, max compression
+gzip compressed data, was "selfcheckgpt-0.1.4.tar", last modified: Tue Jul 18 16:45:58 2023, max compression
```

## Comparing `selfcheckgpt-0.1.3.tar` & `selfcheckgpt-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-05-25 14:47:15.000000 selfcheckgpt-0.1.3/
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     1426 2023-03-23 22:46:15.000000 selfcheckgpt-0.1.3/DESCRIPTION.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     1073 2023-03-22 00:15:36.000000 selfcheckgpt-0.1.3/LICENSE
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       40 2023-03-22 15:18:29.000000 selfcheckgpt-0.1.3/MANIFEST.in
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     2001 2023-05-25 14:47:15.000000 selfcheckgpt-0.1.3/PKG-INFO
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     6232 2023-05-25 14:17:07.000000 selfcheckgpt-0.1.3/README.md
-drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt/
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       45 2023-03-23 20:55:46.000000 selfcheckgpt-0.1.3/selfcheckgpt/__init__.py
--rw-rw-r--   0 pm574    (44166) pm574    (44167)    13292 2023-03-27 14:34:54.000000 selfcheckgpt-0.1.3/selfcheckgpt/modeling_mqag.py
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     6285 2023-05-25 14:31:33.000000 selfcheckgpt-0.1.3/selfcheckgpt/modeling_ngram.py
--rw-rw-r--   0 pm574    (44166) pm574    (44167)    12130 2023-05-25 14:17:07.000000 selfcheckgpt-0.1.3/selfcheckgpt/modeling_selfcheck.py
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     3317 2023-03-27 14:34:54.000000 selfcheckgpt-0.1.3/selfcheckgpt/utils.py
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       22 2023-03-30 22:06:16.000000 selfcheckgpt-0.1.3/selfcheckgpt/version.py
-drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-05-25 14:47:15.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     2001 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/PKG-INFO
--rw-rw-r--   0 pm574    (44166) pm574    (44167)      400 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/SOURCES.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)        1 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/dependency_links.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       61 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/requires.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       13 2023-05-25 14:47:14.000000 selfcheckgpt-0.1.3/selfcheckgpt.egg-info/top_level.txt
--rw-rw-r--   0 pm574    (44166) pm574    (44167)       38 2023-05-25 14:47:15.000000 selfcheckgpt-0.1.3/setup.cfg
--rw-rw-r--   0 pm574    (44166) pm574    (44167)     1164 2023-03-30 22:05:51.000000 selfcheckgpt-0.1.3/setup.py
+drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-07-18 16:45:58.000000 selfcheckgpt-0.1.4/
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     1426 2023-03-23 22:46:15.000000 selfcheckgpt-0.1.4/DESCRIPTION.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     1073 2023-03-22 00:15:36.000000 selfcheckgpt-0.1.4/LICENSE
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       40 2023-03-22 15:18:29.000000 selfcheckgpt-0.1.4/MANIFEST.in
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     2001 2023-07-18 16:45:58.000000 selfcheckgpt-0.1.4/PKG-INFO
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     9691 2023-07-18 15:25:13.000000 selfcheckgpt-0.1.4/README.md
+drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-07-18 16:45:58.000000 selfcheckgpt-0.1.4/selfcheckgpt/
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       45 2023-03-23 20:55:46.000000 selfcheckgpt-0.1.4/selfcheckgpt/__init__.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)    13292 2023-03-27 14:34:54.000000 selfcheckgpt-0.1.4/selfcheckgpt/modeling_mqag.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     6285 2023-05-25 14:31:33.000000 selfcheckgpt-0.1.4/selfcheckgpt/modeling_ngram.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)    15229 2023-07-18 16:35:08.000000 selfcheckgpt-0.1.4/selfcheckgpt/modeling_selfcheck.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     3389 2023-07-18 15:28:31.000000 selfcheckgpt-0.1.4/selfcheckgpt/utils.py
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       22 2023-07-18 15:52:43.000000 selfcheckgpt-0.1.4/selfcheckgpt/version.py
+drwxrwsr-x   0 pm574    (44166) pm574    (44167)        0 2023-07-18 16:45:58.000000 selfcheckgpt-0.1.4/selfcheckgpt.egg-info/
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     2001 2023-07-18 16:45:57.000000 selfcheckgpt-0.1.4/selfcheckgpt.egg-info/PKG-INFO
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)      400 2023-07-18 16:45:58.000000 selfcheckgpt-0.1.4/selfcheckgpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)        1 2023-07-18 16:45:57.000000 selfcheckgpt-0.1.4/selfcheckgpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       61 2023-07-18 16:45:57.000000 selfcheckgpt-0.1.4/selfcheckgpt.egg-info/requires.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       13 2023-07-18 16:45:57.000000 selfcheckgpt-0.1.4/selfcheckgpt.egg-info/top_level.txt
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)       38 2023-07-18 16:45:58.000000 selfcheckgpt-0.1.4/setup.cfg
+-rw-rw-r--   0 pm574    (44166) pm574    (44167)     1164 2023-03-30 22:05:51.000000 selfcheckgpt-0.1.4/setup.py
```

### Comparing `selfcheckgpt-0.1.3/DESCRIPTION.txt` & `selfcheckgpt-0.1.4/DESCRIPTION.txt`

 * *Files identical despite different names*

### Comparing `selfcheckgpt-0.1.3/LICENSE` & `selfcheckgpt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `selfcheckgpt-0.1.3/PKG-INFO` & `selfcheckgpt-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcheckgpt
-Version: 0.1.3
+Version: 0.1.4
 Summary: SelfCheckGPT: Assessing text-based responses from LLMs
 Home-page: https://github.com/potsawee/selfcheckgpt
 Author: Potsawee Manakul
 Author-email: m.potsawee@gmail.com
 License: MIT
 Keywords: selfcheckgpt
 Platform: UNKNOWN
```

### Comparing `selfcheckgpt-0.1.3/selfcheckgpt/modeling_mqag.py` & `selfcheckgpt-0.1.4/selfcheckgpt/modeling_mqag.py`

 * *Files identical despite different names*

### Comparing `selfcheckgpt-0.1.3/selfcheckgpt/modeling_ngram.py` & `selfcheckgpt-0.1.4/selfcheckgpt/modeling_ngram.py`

 * *Files identical despite different names*

### Comparing `selfcheckgpt-0.1.3/selfcheckgpt/modeling_selfcheck.py` & `selfcheckgpt-0.1.4/selfcheckgpt/modeling_selfcheck.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import torch
 from typing import Dict, List, Set, Tuple, Union
 from transformers import logging
 logging.set_verbosity_error()
 
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM
 from transformers import LongformerTokenizer, LongformerForMultipleChoice, LongformerForSequenceClassification
-from selfcheckgpt.utils import MQAGConfig, expand_list1, expand_list2
+from transformers import DebertaV2ForSequenceClassification, DebertaV2Tokenizer
+from selfcheckgpt.utils import MQAGConfig, expand_list1, expand_list2, NLIConfig
 from selfcheckgpt.modeling_mqag import question_generation_sentence_level, answering
 from selfcheckgpt.modeling_ngram import UnigramModel, NgramModel
 
 # ---------------------------------------------------------------------------------------- #
 # Functions for counting
 def method_simple_counting(
     prob,
@@ -234,17 +235,25 @@
 
         return np.array(sent_scores)
 
 class SelfCheckBERTScore:
     """
     SelfCheckGPT (BERTScore variant): Checking LLM's text against its own sampled texts via BERTScore (against best-matched sampled sentence)
     """
-    def __init__(self, default_model="en"):
+    def __init__(self, default_model="en", rescale_with_baseline=True):
+        """
+        :default_model: model for BERTScore
+        :rescale_with_baseline:
+            - whether or not to rescale the score. If False, the values of BERTScore will be very high
+            - this issue was observed and later added to the BERTScore package,
+            - see https://github.com/Tiiiger/bert_score/blob/master/journal/rescale_baseline.md
+        """
         self.nlp = spacy.load("en_core_web_sm")
         self.default_model = default_model # en => roberta-large
+        self.rescale_with_baseline = rescale_with_baseline
         print("SelfCheck-BERTScore initialized")
 
     @torch.no_grad()
     def predict(
         self,
         sentences: List[str],
         sampled_passages: List[str],
@@ -263,15 +272,19 @@
             sentences_sample = [sent for sent in self.nlp(sample_passage).sents] # List[spacy.tokens.span.Span]
             sentences_sample = [sent.text.strip() for sent in sentences_sample if len(sent) > 3]
             num_sentences_sample  = len(sentences_sample)
 
             refs  = expand_list1(sentences, num_sentences_sample) # r1,r1,r1,....
             cands = expand_list2(sentences_sample, num_sentences) # s1,s2,s3,...
 
-            P, R, F1 = bert_score.score(cands, refs, lang=self.default_model, verbose=False)
+            P, R, F1 = bert_score.score(
+                    cands, refs,
+                    lang=self.default_model, verbose=False,
+                    rescale_with_baseline=self.rescale_with_baseline,
+            )
             F1_arr = F1.reshape(num_sentences, num_sentences_sample)
             F1_arr_max_axis1 = F1_arr.max(axis=1).values
             F1_arr_max_axis1 = F1_arr_max_axis1.numpy()
 
             bertscore_array[:,s] = F1_arr_max_axis1
 
         bertscore_mean_per_sent = bertscore_array.mean(axis=-1)
@@ -306,7 +319,59 @@
             raise ValueError("n must be integer >= 1")
         ngram_model.add(passage)
         for sampled_passge in sampled_passages:
             ngram_model.add(sampled_passge)
         ngram_model.train(k=0)
         ngram_pred = ngram_model.evaluate(sentences)
         return ngram_pred
+
+class SelfCheckNLI:
+    """
+    SelfCheckGPT (NLI variant): Checking LLM's text against its own sampled texts via DeBERTa-v3 finetuned to Multi-NLI
+    """
+    def __init__(
+        self,
+        nli_model: str = None,
+        device = None
+    ):
+        nli_model = nli_model if nli_model is not None else NLIConfig.nli_model
+        self.tokenizer = DebertaV2Tokenizer.from_pretrained(nli_model)
+        self.model = DebertaV2ForSequenceClassification.from_pretrained(nli_model)
+        self.model.eval()
+        if device is None:
+            device = torch.device("cpu")
+        self.model.to(device)
+        self.device = device
+        print("SelfCheck-NLI initialized to device", device)
+
+    @torch.no_grad()
+    def predict(
+        self,
+        sentences: List[str],
+        sampled_passages: List[str],
+    ):
+        """
+        This function takes sentences (to be evaluated) with sampled passages (evidence), and return sent-level scores
+        :param sentences: list[str] -- sentences to be evaluated, e.g. GPT text response spilt by spacy
+        :param sampled_passages: list[str] -- stochastically generated responses (without sentence splitting)
+        :return sent_scores: sentence-level score which is P(condict|sentence, sample)
+        note that we normalize the probability on "entailment" or "contradiction" classes only
+        and the score is the probability of the "contradiction" class
+        """
+        num_sentences = len(sentences)
+        num_samples = len(sampled_passages)
+        scores = np.zeros((num_sentences, num_samples))
+        for sent_i, sentence in enumerate(sentences):
+            for sample_i, sample in enumerate(sampled_passages):
+                inputs = self.tokenizer.batch_encode_plus(
+                    batch_text_or_text_pairs=[(sentence, sample)],
+                    add_special_tokens=True, padding="longest",
+                    truncation=True, return_tensors="pt",
+                    return_token_type_ids=True, return_attention_mask=True,
+                )
+                inputs = inputs.to(self.device)
+                logits = self.model(**inputs).logits # neutral is already removed
+                probs = torch.softmax(logits, dim=-1)
+                prob_ = probs[0][1].item() # prob(contradiction)
+                scores[sent_i, sample_i] = prob_
+        scores_per_sentence = scores.mean(axis=-1)
+        return scores_per_sentence
```

### Comparing `selfcheckgpt-0.1.3/selfcheckgpt/utils.py` & `selfcheckgpt-0.1.4/selfcheckgpt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 class MQAGConfig:
     generation1_squad: str = "potsawee/t5-large-generation-squad-QuestionAnswer"
     generation1_race: str = "potsawee/t5-large-generation-race-QuestionAnswer"
     generation2: str = "potsawee/t5-large-generation-race-Distractor"
     answering: str = "potsawee/longformer-large-4096-answering-race"
     answerability: str = "potsawee/longformer-large-4096-answerable-squad2"
 
+class NLIConfig:
+    nli_model: str = "potsawee/deberta-v3-large-mnli"
+
 # Question Generation & Answering Input Processing
 def prepare_qa_input(t5_tokenizer, context, device):
     """
     input: context
     output: question <sep> answer
     """
     encoding = t5_tokenizer(
```

### Comparing `selfcheckgpt-0.1.3/selfcheckgpt.egg-info/PKG-INFO` & `selfcheckgpt-0.1.4/selfcheckgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcheckgpt
-Version: 0.1.3
+Version: 0.1.4
 Summary: SelfCheckGPT: Assessing text-based responses from LLMs
 Home-page: https://github.com/potsawee/selfcheckgpt
 Author: Potsawee Manakul
 Author-email: m.potsawee@gmail.com
 License: MIT
 Keywords: selfcheckgpt
 Platform: UNKNOWN
```

### Comparing `selfcheckgpt-0.1.3/setup.py` & `selfcheckgpt-0.1.4/setup.py`

 * *Files identical despite different names*

