# Comparing `tmp/span_marker-1.2.3.tar.gz` & `tmp/span_marker-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "span_marker-1.2.3.tar", last modified: Tue Jun 20 10:23:50 2023, max compression
+gzip compressed data, was "span_marker-1.2.4.tar", last modified: Tue Jul 18 18:09:19 2023, max compression
```

## Comparing `span_marker-1.2.3.tar` & `span_marker-1.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:23:50.975869 span_marker-1.2.3/
--rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.2.3/LICENSE
--rw-rw-rw-   0        0        0    15586 2023-06-20 10:23:50.975869 span_marker-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    15018 2023-06-20 09:31:29.000000 span_marker-1.2.3/README.md
--rw-rw-rw-   0        0        0     2521 2023-06-20 09:21:34.000000 span_marker-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 10:23:50.975869 span_marker-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      140 2023-06-20 09:21:47.000000 span_marker-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:23:50.954844 span_marker-1.2.3/span_marker/
--rw-rw-rw-   0        0        0     1659 2023-06-20 10:22:50.000000 span_marker-1.2.3/span_marker/__init__.py
--rw-rw-rw-   0        0        0     7070 2023-06-15 09:34:01.000000 span_marker-1.2.3/span_marker/configuration.py
--rw-rw-rw-   0        0        0     6630 2023-06-13 22:30:33.000000 span_marker-1.2.3/span_marker/data_collator.py
--rw-rw-rw-   0        0        0     5276 2023-06-15 14:37:15.000000 span_marker-1.2.3/span_marker/evaluation.py
--rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.2.3/span_marker/label_normalizer.py
--rw-rw-rw-   0        0        0     2472 2023-06-13 22:30:43.000000 span_marker-1.2.3/span_marker/model_card.py
--rw-rw-rw-   0        0        0    31577 2023-06-20 07:05:23.000000 span_marker-1.2.3/span_marker/modeling.py
--rw-rw-rw-   0        0        0     2221 2023-06-13 22:30:33.000000 span_marker-1.2.3/span_marker/output.py
--rw-rw-rw-   0        0        0     3932 2023-06-20 10:16:09.000000 span_marker-1.2.3/span_marker/spacy_integration.py
--rw-rw-rw-   0        0        0    11828 2023-06-19 13:54:52.000000 span_marker-1.2.3/span_marker/tokenizer.py
--rw-rw-rw-   0        0        0    21019 2023-06-15 10:02:14.000000 span_marker-1.2.3/span_marker/trainer.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:23:50.971870 span_marker-1.2.3/span_marker.egg-info/
--rw-rw-rw-   0        0        0    15586 2023-06-20 10:23:50.000000 span_marker-1.2.3/span_marker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-06-20 10:23:50.000000 span_marker-1.2.3/span_marker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:23:50.000000 span_marker-1.2.3/span_marker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-06-20 10:23:50.000000 span_marker-1.2.3/span_marker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      267 2023-06-20 10:23:50.000000 span_marker-1.2.3/span_marker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 10:23:50.000000 span_marker-1.2.3/span_marker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 10:23:50.974870 span_marker-1.2.3/tests/
--rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.2.3/tests/test_configuration.py
--rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.2.3/tests/test_model_card.py
--rw-rw-rw-   0        0        0     9228 2023-06-15 09:34:01.000000 span_marker-1.2.3/tests/test_modeling.py
--rw-rw-rw-   0        0        0     1165 2023-06-20 09:23:58.000000 span_marker-1.2.3/tests/test_spacy_integration.py
--rw-rw-rw-   0        0        0    10372 2023-06-15 09:34:01.000000 span_marker-1.2.3/tests/test_trainer.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:19.641651 span_marker-1.2.4/
+-rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0    16029 2023-07-18 18:09:19.641651 span_marker-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15440 2023-07-04 18:59:28.000000 span_marker-1.2.4/README.md
+-rw-rw-rw-   0        0        0     2520 2023-07-18 18:05:25.000000 span_marker-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 18:09:19.642650 span_marker-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      140 2023-06-20 09:21:47.000000 span_marker-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:19.625717 span_marker-1.2.4/span_marker/
+-rw-rw-rw-   0        0        0     1659 2023-07-18 18:05:48.000000 span_marker-1.2.4/span_marker/__init__.py
+-rw-rw-rw-   0        0        0     7070 2023-06-15 09:34:01.000000 span_marker-1.2.4/span_marker/configuration.py
+-rw-rw-rw-   0        0        0     6630 2023-06-13 22:30:33.000000 span_marker-1.2.4/span_marker/data_collator.py
+-rw-rw-rw-   0        0        0     5276 2023-06-15 14:37:15.000000 span_marker-1.2.4/span_marker/evaluation.py
+-rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.2.4/span_marker/label_normalizer.py
+-rw-rw-rw-   0        0        0     2472 2023-06-20 18:26:14.000000 span_marker-1.2.4/span_marker/model_card.py
+-rw-rw-rw-   0        0        0    31837 2023-07-18 18:01:52.000000 span_marker-1.2.4/span_marker/modeling.py
+-rw-rw-rw-   0        0        0     2221 2023-06-13 22:30:33.000000 span_marker-1.2.4/span_marker/output.py
+-rw-rw-rw-   0        0        0     3932 2023-07-04 09:28:12.000000 span_marker-1.2.4/span_marker/spacy_integration.py
+-rw-rw-rw-   0        0        0    11828 2023-07-12 08:50:41.000000 span_marker-1.2.4/span_marker/tokenizer.py
+-rw-rw-rw-   0        0        0    21019 2023-06-15 10:02:14.000000 span_marker-1.2.4/span_marker/trainer.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:19.638142 span_marker-1.2.4/span_marker.egg-info/
+-rw-rw-rw-   0        0        0    16029 2023-07-18 18:09:19.000000 span_marker-1.2.4/span_marker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-07-18 18:09:19.000000 span_marker-1.2.4/span_marker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:09:19.000000 span_marker-1.2.4/span_marker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-18 18:09:19.000000 span_marker-1.2.4/span_marker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      267 2023-07-18 18:09:19.000000 span_marker-1.2.4/span_marker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 18:09:19.000000 span_marker-1.2.4/span_marker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 18:09:19.640652 span_marker-1.2.4/tests/
+-rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.2.4/tests/test_configuration.py
+-rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.2.4/tests/test_model_card.py
+-rw-rw-rw-   0        0        0     9228 2023-06-15 09:34:01.000000 span_marker-1.2.4/tests/test_modeling.py
+-rw-rw-rw-   0        0        0     1165 2023-07-04 09:28:17.000000 span_marker-1.2.4/tests/test_spacy_integration.py
+-rw-rw-rw-   0        0        0    10372 2023-06-15 09:34:01.000000 span_marker-1.2.4/tests/test_trainer.py
```

### Comparing `span_marker-1.2.3/LICENSE` & `span_marker-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/PKG-INFO` & `span_marker-1.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,21 @@
-Metadata-Version: 2.1
-Name: span_marker
-Version: 1.2.3
-Summary: Named Entity Recognition using Span Markers
-Author: Tom Aarsen
-Maintainer: Tom Aarsen
-Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
-Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
-Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: wandb
-License-File: LICENSE
-
 <div align="center">
 <h1>
 SpanMarker for Named Entity Recognition
 </h1>
 <a href="https://huggingface.co/tomaarsen/span-marker-roberta-large-ontonotes5" target="_blank">
     <img src="https://github.com/tomaarsen/SpanMarkerNER/assets/37621491/c76d6393-bb0b-44c3-9412-fd9c8313dcc1">
 </a>
 
 [🤗 Models](https://huggingface.co/models?library=span-marker) |
 [🛠️ Getting Started In Google Colab](https://colab.research.google.com/github/tomaarsen/SpanMarkerNER/blob/main/notebooks/getting_started.ipynb) |
-[📄 Documentation](https://tomaarsen.github.io/SpanMarkerNER)
+[📄 Documentation](https://tomaarsen.github.io/SpanMarkerNER) | 📊 [Thesis](https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf)
 </div>
 
-SpanMarker is a framework for training powerful Named Entity Recognition models using familiar encoders such as BERT, RoBERTa and DeBERTa.
+SpanMarker is a framework for training powerful Named Entity Recognition models using familiar encoders such as BERT, RoBERTa and ELECTRA.
 Built on top of the familiar [🤗 Transformers](https://github.com/huggingface/transformers) library, SpanMarker inherits a wide range of powerful functionalities, such as easily loading and saving models, hyperparameter optimization, automatic logging in various tools, checkpointing, callbacks, mixed precision training, 8-bit inference, and more.
 
 <!--Tightly implemented on top of the [🤗 Transformers](https://github.com/huggingface/transformers/) library, SpanMarker can take advantage of its valuable functionality.-->
 <!-- like performance dashboard integration, automatic mixed precision, 8-bit inference-->
 
 Based on the [PL-Marker](https://arxiv.org/pdf/2109.06067.pdf) paper, SpanMarker breaks the mold through its accessibility and ease of use. Crucially, SpanMarker works out of the box with many common encoders such as `bert-base-cased` and `roberta-large`, and automatically works with datasets using the `IOB`, `IOB2`, `BIOES`, `BILOU` or no label annotation scheme.
 
@@ -140,14 +124,16 @@
 <!-- Because this work is based on [PL-Marker](https://arxiv.org/pdf/2109.06067v5.pdf), you may expect similar results to its [Papers with Code Leaderboard](https://paperswithcode.com/paper/pack-together-entity-and-relation-extraction) results. -->
 
 ## Pretrained Models
 
 All models in this list contain `train.py` files that show the training scripts used to generate them. Additionally, all training scripts used are stored in the [training_scripts](training_scripts) directory.
 These trained models have Hosted Inference API widgets that you can use to experiment with the models on their Hugging Face model pages. Additionally, Hugging Face provides each model with a free API (`Deploy` > `Inference API` on the model page).
 
+These models are further elaborated on in my [thesis](https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf).
+
 ### FewNERD
 * [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is a model that I have trained in 2 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a 0.7053 Test F1, competitive in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup) using `bert-base`. My training script resembles the one that you can see above.
   * Try the model out online using this [🤗 Space](https://tomaarsen-span-marker-bert-base-fewnerd-fine-super.hf.space/).
 
 * [`tomaarsen/span-marker-roberta-large-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-roberta-large-fewnerd-fine-super) was trained in 6 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd) using `roberta-large`. It reached a 0.7103 Test F1, reaching a new state of the art in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup).
 * [`tomaarsen/span-marker-xlm-roberta-base-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-base-fewnerd-fine-super) is a multilingual model that I have trained in 1.5 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a 0.686 Test F1 on English, and works well on other languages like Spanish, French, German, Russian, Dutch, Polish, Icelandic, Greek and many more.
 
@@ -158,20 +144,20 @@
 * [`tomaarsen/span-marker-xlm-roberta-large-conll03`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conll03) is a SpanMarker model using `xlm-roberta-large` that was trained in 45 minutes. It reaches a state of the art 0.931 F1 on CoNLL03 without using document-level context. For reference, the current strongest spaCy model (`en_core_web_trf`) reaches 91.6.
 * [`tomaarsen/span-marker-xlm-roberta-large-conll03-doc-context`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conll03-doc-context) is another SpanMarker model using the `xlm-roberta-large` encoder. It uses [document-level context](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html) to reach a state of the art 0.944 F1. For the best performance, inference should be performed using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html#Inference)). This model was trained in 1 hour.
 
 ### CoNLL++
 * [`tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context) was trained in an hour using the `xlm-roberta-large` encoder on the CoNLL++ dataset. Using [document-level context](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html), it reaches a very competitive 0.955 F1. For the best performance, inference should be performed using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html#Inference)).
 
 ## Using pretrained SpanMarker models with spaCy
-All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the Documentation or API Reference for more information.
+All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the [Documentation](https://tomaarsen.github.io/SpanMarkerNER/notebooks/spacy_integration.html) or [API Reference](https://tomaarsen.github.io/SpanMarkerNER/api/span_marker.spacy_integration.html) for more information.
 ```python
 import spacy
 
 # Load the spaCy model with the span_marker pipeline component
-nlp = spacy.load("en_core_web_sm", disable=["ner"])
+nlp = spacy.load("en_core_web_sm", exclude=["ner"])
 nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
 # Feed some text through the model to get a spacy Doc
 text = """Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the \
 Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her \
 death in 30 BCE."""
 doc = nlp(text)
@@ -188,15 +174,14 @@
 ## Context
 <h1 align="center">
     <a href="https://github.com/argilla-io/argilla">
     <img src="https://github.com/dvsrepo/imgs/raw/main/rg.svg" alt="Argilla" width="150">
     </a>
 </h1>
 
-I have developed this library as a part of my thesis work at [Argilla](https://github.com/argilla-io/argilla).
-Feel free to ⭐ star or watch the SpanMarker repository to get notified when my thesis is published.
+I have developed this library as a part of my thesis work at [Argilla](https://github.com/argilla-io/argilla). Feel free to read my finished thesis [here](https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf) in this repository!
 
 ## Changelog
 See [CHANGELOG.md](CHANGELOG.md) for news on all SpanMarker versions.
 
 ## License
 See [LICENSE](LICENSE.md) for the current license.
```

#### html2text {}

```diff
@@ -1,24 +1,17 @@
-Metadata-Version: 2.1 Name: span_marker Version: 1.2.3 Summary: Named Entity
-Recognition using Span Markers Author: Tom Aarsen Maintainer: Tom Aarsen
-Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER Project-
-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER Keywords: data-
-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-
-learning,transformers Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev Provides-Extra: docs Provides-Extra: wandb
-License-File: LICENSE
              ****** SpanMarker for Named Entity Recognition ******
 [https://github.com/tomaarsen/SpanMarkerNER/assets/37621491/c76d6393-bb0b-44c3-
  9412-fd9c8313dcc1] [ð¤ Models](https://huggingface.co/models?library=span-
          marker) | [ð ï¸ Getting Started In Google Colab](https://
  colab.research.google.com/github/tomaarsen/SpanMarkerNER/blob/main/notebooks/
   getting_started.ipynb) | [ð Documentation](https://tomaarsen.github.io/
-                                SpanMarkerNER)
+  SpanMarkerNER) | ð [Thesis](https://raw.githubusercontent.com/tomaarsen/
+                        SpanMarkerNER/main/thesis.pdf)
 SpanMarker is a framework for training powerful Named Entity Recognition models
-using familiar encoders such as BERT, RoBERTa and DeBERTa. Built on top of the
+using familiar encoders such as BERT, RoBERTa and ELECTRA. Built on top of the
 familiar [ð¤ Transformers](https://github.com/huggingface/transformers)
 library, SpanMarker inherits a wide range of powerful functionalities, such as
 easily loading and saving models, hyperparameter optimization, automatic
 logging in various tools, checkpointing, callbacks, mixed precision training,
 8-bit inference, and more.   Based on the [PL-Marker](https://arxiv.org/pdf/
 2109.06067.pdf) paper, SpanMarker breaks the mold through its accessibility and
 ease of use. Crucially, SpanMarker works out of the box with many common
@@ -106,17 +99,19 @@
 0.9892390966415405, 'char_start_index': 78, 'char_end_index': 83}] ```  ##
 Pretrained Models All models in this list contain `train.py` files that show
 the training scripts used to generate them. Additionally, all training scripts
 used are stored in the [training_scripts](training_scripts) directory. These
 trained models have Hosted Inference API widgets that you can use to experiment
 with the models on their Hugging Face model pages. Additionally, Hugging Face
 provides each model with a free API (`Deploy` > `Inference API` on the model
-page). ### FewNERD * [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`]
-(https://huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is
-a model that I have trained in 2 hours on the finegrained, supervised [Few-NERD
+page). These models are further elaborated on in my [thesis](https://
+raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf). ### FewNERD
+* [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`](https://
+huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is a model
+that I have trained in 2 hours on the finegrained, supervised [Few-NERD
 dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a
 0.7053 Test F1, competitive in the all-time [Few-NERD leaderboard](https://
 paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup) using `bert-
 base`. My training script resembles the one that you can see above. * Try the
 model out online using this [ð¤ Space](https://tomaarsen-span-marker-bert-
 base-fewnerd-fine-super.hf.space/). * [`tomaarsen/span-marker-roberta-large-
 fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-roberta-
@@ -156,26 +151,29 @@
 SpanMarkerNER/notebooks/document_level_context.html), it reaches a very
 competitive 0.955 F1. For the best performance, inference should be performed
 using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/
 notebooks/document_level_context.html#Inference)). ## Using pretrained
 SpanMarker models with spaCy All [SpanMarker models on the Hugging Face Hub]
 (https://huggingface.co/models?library=span-marker) can also be easily used in
 spaCy. It's as simple as including 1 line to add the `span_marker` pipeline.
-See the Documentation or API Reference for more information. ```python import
-spacy # Load the spaCy model with the span_marker pipeline component nlp =
-spacy.load("en_core_web_sm", disable=["ner"]) nlp.add_pipe("span_marker",
-config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"}) # Feed some
-text through the model to get a spacy Doc text = """Cleopatra VII, also known
-as Cleopatra the Great, was the last active ruler of the \ Ptolemaic Kingdom of
-Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her \ death in
-30 BCE.""" doc = nlp(text) # And look at the entities print([(entity,
-entity.label_) for entity in doc.ents]) """ [(Cleopatra VII, "PERSON"),
-(Cleopatra the Great, "PERSON"), (the Ptolemaic Kingdom of Egypt, "GPE"), (69
-BCE, "DATE"), (Egypt, "GPE"), (51 BCE, "DATE"), (30 BCE, "DATE")] """ ``` !
-[image](https://user-images.githubusercontent.com/37621491/246170623-6351cb7e-
-bbb0-4472-af16-9a351a253da9.png) ## Context
+See the [Documentation](https://tomaarsen.github.io/SpanMarkerNER/notebooks/
+spacy_integration.html) or [API Reference](https://tomaarsen.github.io/
+SpanMarkerNER/api/span_marker.spacy_integration.html) for more information.
+```python import spacy # Load the spaCy model with the span_marker pipeline
+component nlp = spacy.load("en_core_web_sm", exclude=["ner"]) nlp.add_pipe
+("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-
+ontonotes5"}) # Feed some text through the model to get a spacy Doc text =
+"""Cleopatra VII, also known as Cleopatra the Great, was the last active ruler
+of the \ Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt
+from 51 BCE until her \ death in 30 BCE.""" doc = nlp(text) # And look at the
+entities print([(entity, entity.label_) for entity in doc.ents]) """ [
+(Cleopatra VII, "PERSON"), (Cleopatra the Great, "PERSON"), (the Ptolemaic
+Kingdom of Egypt, "GPE"), (69 BCE, "DATE"), (Egypt, "GPE"), (51 BCE, "DATE"),
+(30 BCE, "DATE")] """ ``` ![image](https://user-images.githubusercontent.com/
+37621491/246170623-6351cb7e-bbb0-4472-af16-9a351a253da9.png) ## Context
                             ****** [Argilla] ******
 I have developed this library as a part of my thesis work at [Argilla](https://
-github.com/argilla-io/argilla). Feel free to â­ star or watch the SpanMarker
-repository to get notified when my thesis is published. ## Changelog See
-[CHANGELOG.md](CHANGELOG.md) for news on all SpanMarker versions. ## License
-See [LICENSE](LICENSE.md) for the current license.
+github.com/argilla-io/argilla). Feel free to read my finished thesis [here]
+(https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf) in
+this repository! ## Changelog See [CHANGELOG.md](CHANGELOG.md) for news on all
+SpanMarker versions. ## License See [LICENSE](LICENSE.md) for the current
+license.
```

### Comparing `span_marker-1.2.3/README.md` & `span_marker-1.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,38 @@
+Metadata-Version: 2.1
+Name: span_marker
+Version: 1.2.4
+Summary: Named Entity Recognition using Span Markers
+Author: Tom Aarsen
+Maintainer: Tom Aarsen
+License: Apache-2.0
+Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
+Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
+Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: wandb
+License-File: LICENSE
+
 <div align="center">
 <h1>
 SpanMarker for Named Entity Recognition
 </h1>
 <a href="https://huggingface.co/tomaarsen/span-marker-roberta-large-ontonotes5" target="_blank">
     <img src="https://github.com/tomaarsen/SpanMarkerNER/assets/37621491/c76d6393-bb0b-44c3-9412-fd9c8313dcc1">
 </a>
 
 [🤗 Models](https://huggingface.co/models?library=span-marker) |
 [🛠️ Getting Started In Google Colab](https://colab.research.google.com/github/tomaarsen/SpanMarkerNER/blob/main/notebooks/getting_started.ipynb) |
-[📄 Documentation](https://tomaarsen.github.io/SpanMarkerNER)
+[📄 Documentation](https://tomaarsen.github.io/SpanMarkerNER) | 📊 [Thesis](https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf)
 </div>
 
-SpanMarker is a framework for training powerful Named Entity Recognition models using familiar encoders such as BERT, RoBERTa and DeBERTa.
+SpanMarker is a framework for training powerful Named Entity Recognition models using familiar encoders such as BERT, RoBERTa and ELECTRA.
 Built on top of the familiar [🤗 Transformers](https://github.com/huggingface/transformers) library, SpanMarker inherits a wide range of powerful functionalities, such as easily loading and saving models, hyperparameter optimization, automatic logging in various tools, checkpointing, callbacks, mixed precision training, 8-bit inference, and more.
 
 <!--Tightly implemented on top of the [🤗 Transformers](https://github.com/huggingface/transformers/) library, SpanMarker can take advantage of its valuable functionality.-->
 <!-- like performance dashboard integration, automatic mixed precision, 8-bit inference-->
 
 Based on the [PL-Marker](https://arxiv.org/pdf/2109.06067.pdf) paper, SpanMarker breaks the mold through its accessibility and ease of use. Crucially, SpanMarker works out of the box with many common encoders such as `bert-base-cased` and `roberta-large`, and automatically works with datasets using the `IOB`, `IOB2`, `BIOES`, `BILOU` or no label annotation scheme.
 
@@ -124,14 +141,16 @@
 <!-- Because this work is based on [PL-Marker](https://arxiv.org/pdf/2109.06067v5.pdf), you may expect similar results to its [Papers with Code Leaderboard](https://paperswithcode.com/paper/pack-together-entity-and-relation-extraction) results. -->
 
 ## Pretrained Models
 
 All models in this list contain `train.py` files that show the training scripts used to generate them. Additionally, all training scripts used are stored in the [training_scripts](training_scripts) directory.
 These trained models have Hosted Inference API widgets that you can use to experiment with the models on their Hugging Face model pages. Additionally, Hugging Face provides each model with a free API (`Deploy` > `Inference API` on the model page).
 
+These models are further elaborated on in my [thesis](https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf).
+
 ### FewNERD
 * [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is a model that I have trained in 2 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a 0.7053 Test F1, competitive in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup) using `bert-base`. My training script resembles the one that you can see above.
   * Try the model out online using this [🤗 Space](https://tomaarsen-span-marker-bert-base-fewnerd-fine-super.hf.space/).
 
 * [`tomaarsen/span-marker-roberta-large-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-roberta-large-fewnerd-fine-super) was trained in 6 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd) using `roberta-large`. It reached a 0.7103 Test F1, reaching a new state of the art in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup).
 * [`tomaarsen/span-marker-xlm-roberta-base-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-base-fewnerd-fine-super) is a multilingual model that I have trained in 1.5 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a 0.686 Test F1 on English, and works well on other languages like Spanish, French, German, Russian, Dutch, Polish, Icelandic, Greek and many more.
 
@@ -142,20 +161,20 @@
 * [`tomaarsen/span-marker-xlm-roberta-large-conll03`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conll03) is a SpanMarker model using `xlm-roberta-large` that was trained in 45 minutes. It reaches a state of the art 0.931 F1 on CoNLL03 without using document-level context. For reference, the current strongest spaCy model (`en_core_web_trf`) reaches 91.6.
 * [`tomaarsen/span-marker-xlm-roberta-large-conll03-doc-context`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conll03-doc-context) is another SpanMarker model using the `xlm-roberta-large` encoder. It uses [document-level context](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html) to reach a state of the art 0.944 F1. For the best performance, inference should be performed using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html#Inference)). This model was trained in 1 hour.
 
 ### CoNLL++
 * [`tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context) was trained in an hour using the `xlm-roberta-large` encoder on the CoNLL++ dataset. Using [document-level context](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html), it reaches a very competitive 0.955 F1. For the best performance, inference should be performed using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html#Inference)).
 
 ## Using pretrained SpanMarker models with spaCy
-All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the Documentation or API Reference for more information.
+All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the [Documentation](https://tomaarsen.github.io/SpanMarkerNER/notebooks/spacy_integration.html) or [API Reference](https://tomaarsen.github.io/SpanMarkerNER/api/span_marker.spacy_integration.html) for more information.
 ```python
 import spacy
 
 # Load the spaCy model with the span_marker pipeline component
-nlp = spacy.load("en_core_web_sm", disable=["ner"])
+nlp = spacy.load("en_core_web_sm", exclude=["ner"])
 nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
 # Feed some text through the model to get a spacy Doc
 text = """Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the \
 Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her \
 death in 30 BCE."""
 doc = nlp(text)
@@ -172,15 +191,14 @@
 ## Context
 <h1 align="center">
     <a href="https://github.com/argilla-io/argilla">
     <img src="https://github.com/dvsrepo/imgs/raw/main/rg.svg" alt="Argilla" width="150">
     </a>
 </h1>
 
-I have developed this library as a part of my thesis work at [Argilla](https://github.com/argilla-io/argilla).
-Feel free to ⭐ star or watch the SpanMarker repository to get notified when my thesis is published.
+I have developed this library as a part of my thesis work at [Argilla](https://github.com/argilla-io/argilla). Feel free to read my finished thesis [here](https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf) in this repository!
 
 ## Changelog
 See [CHANGELOG.md](CHANGELOG.md) for news on all SpanMarker versions.
 
 ## License
 See [LICENSE](LICENSE.md) for the current license.
```

#### html2text {}

```diff
@@ -1,16 +1,25 @@
+Metadata-Version: 2.1 Name: span_marker Version: 1.2.4 Summary: Named Entity
+Recognition using Span Markers Author: Tom Aarsen Maintainer: Tom Aarsen
+License: Apache-2.0 Project-URL: Documentation, https://tomaarsen.github.io/
+SpanMarkerNER Project-URL: Repository, https://github.com/tomaarsen/
+SpanMarkerNER Keywords: data-science,natural-language-processing,artificial-
+intelligence,mlops,nlp,machine-learning,transformers Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+docs Provides-Extra: wandb License-File: LICENSE
              ****** SpanMarker for Named Entity Recognition ******
 [https://github.com/tomaarsen/SpanMarkerNER/assets/37621491/c76d6393-bb0b-44c3-
  9412-fd9c8313dcc1] [ð¤ Models](https://huggingface.co/models?library=span-
          marker) | [ð ï¸ Getting Started In Google Colab](https://
  colab.research.google.com/github/tomaarsen/SpanMarkerNER/blob/main/notebooks/
   getting_started.ipynb) | [ð Documentation](https://tomaarsen.github.io/
-                                SpanMarkerNER)
+  SpanMarkerNER) | ð [Thesis](https://raw.githubusercontent.com/tomaarsen/
+                        SpanMarkerNER/main/thesis.pdf)
 SpanMarker is a framework for training powerful Named Entity Recognition models
-using familiar encoders such as BERT, RoBERTa and DeBERTa. Built on top of the
+using familiar encoders such as BERT, RoBERTa and ELECTRA. Built on top of the
 familiar [ð¤ Transformers](https://github.com/huggingface/transformers)
 library, SpanMarker inherits a wide range of powerful functionalities, such as
 easily loading and saving models, hyperparameter optimization, automatic
 logging in various tools, checkpointing, callbacks, mixed precision training,
 8-bit inference, and more.   Based on the [PL-Marker](https://arxiv.org/pdf/
 2109.06067.pdf) paper, SpanMarker breaks the mold through its accessibility and
 ease of use. Crucially, SpanMarker works out of the box with many common
@@ -98,17 +107,19 @@
 0.9892390966415405, 'char_start_index': 78, 'char_end_index': 83}] ```  ##
 Pretrained Models All models in this list contain `train.py` files that show
 the training scripts used to generate them. Additionally, all training scripts
 used are stored in the [training_scripts](training_scripts) directory. These
 trained models have Hosted Inference API widgets that you can use to experiment
 with the models on their Hugging Face model pages. Additionally, Hugging Face
 provides each model with a free API (`Deploy` > `Inference API` on the model
-page). ### FewNERD * [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`]
-(https://huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is
-a model that I have trained in 2 hours on the finegrained, supervised [Few-NERD
+page). These models are further elaborated on in my [thesis](https://
+raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf). ### FewNERD
+* [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`](https://
+huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is a model
+that I have trained in 2 hours on the finegrained, supervised [Few-NERD
 dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a
 0.7053 Test F1, competitive in the all-time [Few-NERD leaderboard](https://
 paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup) using `bert-
 base`. My training script resembles the one that you can see above. * Try the
 model out online using this [ð¤ Space](https://tomaarsen-span-marker-bert-
 base-fewnerd-fine-super.hf.space/). * [`tomaarsen/span-marker-roberta-large-
 fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-roberta-
@@ -148,26 +159,29 @@
 SpanMarkerNER/notebooks/document_level_context.html), it reaches a very
 competitive 0.955 F1. For the best performance, inference should be performed
 using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/
 notebooks/document_level_context.html#Inference)). ## Using pretrained
 SpanMarker models with spaCy All [SpanMarker models on the Hugging Face Hub]
 (https://huggingface.co/models?library=span-marker) can also be easily used in
 spaCy. It's as simple as including 1 line to add the `span_marker` pipeline.
-See the Documentation or API Reference for more information. ```python import
-spacy # Load the spaCy model with the span_marker pipeline component nlp =
-spacy.load("en_core_web_sm", disable=["ner"]) nlp.add_pipe("span_marker",
-config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"}) # Feed some
-text through the model to get a spacy Doc text = """Cleopatra VII, also known
-as Cleopatra the Great, was the last active ruler of the \ Ptolemaic Kingdom of
-Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her \ death in
-30 BCE.""" doc = nlp(text) # And look at the entities print([(entity,
-entity.label_) for entity in doc.ents]) """ [(Cleopatra VII, "PERSON"),
-(Cleopatra the Great, "PERSON"), (the Ptolemaic Kingdom of Egypt, "GPE"), (69
-BCE, "DATE"), (Egypt, "GPE"), (51 BCE, "DATE"), (30 BCE, "DATE")] """ ``` !
-[image](https://user-images.githubusercontent.com/37621491/246170623-6351cb7e-
-bbb0-4472-af16-9a351a253da9.png) ## Context
+See the [Documentation](https://tomaarsen.github.io/SpanMarkerNER/notebooks/
+spacy_integration.html) or [API Reference](https://tomaarsen.github.io/
+SpanMarkerNER/api/span_marker.spacy_integration.html) for more information.
+```python import spacy # Load the spaCy model with the span_marker pipeline
+component nlp = spacy.load("en_core_web_sm", exclude=["ner"]) nlp.add_pipe
+("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-
+ontonotes5"}) # Feed some text through the model to get a spacy Doc text =
+"""Cleopatra VII, also known as Cleopatra the Great, was the last active ruler
+of the \ Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt
+from 51 BCE until her \ death in 30 BCE.""" doc = nlp(text) # And look at the
+entities print([(entity, entity.label_) for entity in doc.ents]) """ [
+(Cleopatra VII, "PERSON"), (Cleopatra the Great, "PERSON"), (the Ptolemaic
+Kingdom of Egypt, "GPE"), (69 BCE, "DATE"), (Egypt, "GPE"), (51 BCE, "DATE"),
+(30 BCE, "DATE")] """ ``` ![image](https://user-images.githubusercontent.com/
+37621491/246170623-6351cb7e-bbb0-4472-af16-9a351a253da9.png) ## Context
                             ****** [Argilla] ******
 I have developed this library as a part of my thesis work at [Argilla](https://
-github.com/argilla-io/argilla). Feel free to â­ star or watch the SpanMarker
-repository to get notified when my thesis is published. ## Changelog See
-[CHANGELOG.md](CHANGELOG.md) for news on all SpanMarker versions. ## License
-See [LICENSE](LICENSE.md) for the current license.
+github.com/argilla-io/argilla). Feel free to read my finished thesis [here]
+(https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf) in
+this repository! ## Changelog See [CHANGELOG.md](CHANGELOG.md) for news on all
+SpanMarker versions. ## License See [LICENSE](LICENSE.md) for the current
+license.
```

### Comparing `span_marker-1.2.3/pyproject.toml` & `span_marker-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "span_marker"
 description = "Named Entity Recognition using Span Markers"
 readme = "README.md"
 requires-python = ">=3.7"
-license = {file = "LICENSE.txt"}
+license = {text = "Apache-2.0"}
 keywords = [
     "data-science",
     "natural-language-processing",
     "artificial-intelligence",
     "mlops",
     "nlp",
     "machine-learning",
```

### Comparing `span_marker-1.2.3/span_marker/__init__.py` & `span_marker-1.2.4/span_marker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 
 import logging
 from typing import Optional, Union
 
 import torch
 from transformers import AutoConfig, AutoModel, TrainingArguments
```

### Comparing `span_marker-1.2.3/span_marker/configuration.py` & `span_marker-1.2.4/span_marker/configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/span_marker/data_collator.py` & `span_marker-1.2.4/span_marker/data_collator.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/span_marker/evaluation.py` & `span_marker-1.2.4/span_marker/evaluation.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/span_marker/label_normalizer.py` & `span_marker-1.2.4/span_marker/label_normalizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/span_marker/model_card.py` & `span_marker-1.2.4/span_marker/model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/span_marker/modeling.py` & `span_marker-1.2.4/span_marker/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,25 +118,28 @@
         position_ids: torch.Tensor,
         start_marker_indices: torch.Tensor,
         num_marker_pairs: torch.Tensor,
         labels: Optional[torch.Tensor] = None,
         num_words: Optional[torch.Tensor] = None,
         document_ids: Optional[torch.Tensor] = None,
         sentence_ids: Optional[torch.Tensor] = None,
+        **kwargs,
     ) -> SpanMarkerOutput:
         """Forward call of the SpanMarkerModel.
 
         Args:
             input_ids (~torch.Tensor): Input IDs including start/end markers.
             attention_mask (~torch.Tensor): Attention mask matrix including one-directional attention for markers.
             position_ids (~torch.Tensor): Position IDs including start/end markers.
             start_marker_indices (~torch.Tensor): The indices where the start markers begin per batch sample.
             num_marker_pairs (~torch.Tensor): The number of start/end marker pairs per batch sample.
             labels (Optional[~torch.Tensor]): The labels for each span candidate. Defaults to None.
             num_words (Optional[~torch.Tensor]): The number of words for each batch sample. Defaults to None.
+            document_ids (Optional[~torch.Tensor]): The document ID of each batch sample. Defaults to None.
+            sentence_ids (Optional[~torch.Tensor]): The index of each sentence in their respective document. Defaults to None.
 
         Returns:
             SpanMarkerOutput: The output dataclass.
         """
         token_type_ids = torch.zeros_like(input_ids)
         outputs = self.encoder(
             input_ids,
@@ -165,15 +168,15 @@
                         last_hidden_state[i, start_marker_indices[i] : end_marker_indices[i]],
                         last_hidden_state[i, end_marker_indices[i] : end_marker_indices[i] + num_marker_pairs[i]],
                     ),
                     dim=-1,
                 )
             )
         padded_embeddings = [
-            F.pad(embedding, (0, 0, 0, sequence_length // 2 - len(embedding))) for embedding in embeddings
+            F.pad(embedding, (0, 0, 0, sequence_length // 2 - embedding.shape[0])) for embedding in embeddings
         ]
         feature_vector = torch.stack(padded_embeddings)
 
         # NOTE: This was wrong in the older tests
         feature_vector = self.dropout(feature_vector)
         logits = self.classifier(feature_vector)
```

### Comparing `span_marker-1.2.3/span_marker/output.py` & `span_marker-1.2.4/span_marker/output.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/span_marker/spacy_integration.py` & `span_marker-1.2.4/span_marker/spacy_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
          death in 30 BCE.'''
          doc = nlp(text)
 
     Example::
 
         >>> import spacy
         >>> import span_marker
-        >>> nlp = spacy.load("en_core_web_sm", disable=["ner"])
+        >>> nlp = spacy.load("en_core_web_sm", exclude=["ner"])
         >>> nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
         >>> text = '''Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the
         ... Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her
         ... death in 30 BCE.'''
         >>> doc = nlp(text)
         >>> doc.ents
         (Cleopatra VII, Cleopatra the Great, 69 BCE, Egypt, 51 BCE, 30 BCE)
```

### Comparing `span_marker-1.2.3/span_marker/tokenizer.py` & `span_marker-1.2.4/span_marker/tokenizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/span_marker/trainer.py` & `span_marker-1.2.4/span_marker/trainer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/span_marker.egg-info/PKG-INFO` & `span_marker-1.2.4/span_marker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: span-marker
-Version: 1.2.3
+Version: 1.2.4
 Summary: Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
+License: Apache-2.0
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
@@ -20,18 +21,18 @@
 </h1>
 <a href="https://huggingface.co/tomaarsen/span-marker-roberta-large-ontonotes5" target="_blank">
     <img src="https://github.com/tomaarsen/SpanMarkerNER/assets/37621491/c76d6393-bb0b-44c3-9412-fd9c8313dcc1">
 </a>
 
 [🤗 Models](https://huggingface.co/models?library=span-marker) |
 [🛠️ Getting Started In Google Colab](https://colab.research.google.com/github/tomaarsen/SpanMarkerNER/blob/main/notebooks/getting_started.ipynb) |
-[📄 Documentation](https://tomaarsen.github.io/SpanMarkerNER)
+[📄 Documentation](https://tomaarsen.github.io/SpanMarkerNER) | 📊 [Thesis](https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf)
 </div>
 
-SpanMarker is a framework for training powerful Named Entity Recognition models using familiar encoders such as BERT, RoBERTa and DeBERTa.
+SpanMarker is a framework for training powerful Named Entity Recognition models using familiar encoders such as BERT, RoBERTa and ELECTRA.
 Built on top of the familiar [🤗 Transformers](https://github.com/huggingface/transformers) library, SpanMarker inherits a wide range of powerful functionalities, such as easily loading and saving models, hyperparameter optimization, automatic logging in various tools, checkpointing, callbacks, mixed precision training, 8-bit inference, and more.
 
 <!--Tightly implemented on top of the [🤗 Transformers](https://github.com/huggingface/transformers/) library, SpanMarker can take advantage of its valuable functionality.-->
 <!-- like performance dashboard integration, automatic mixed precision, 8-bit inference-->
 
 Based on the [PL-Marker](https://arxiv.org/pdf/2109.06067.pdf) paper, SpanMarker breaks the mold through its accessibility and ease of use. Crucially, SpanMarker works out of the box with many common encoders such as `bert-base-cased` and `roberta-large`, and automatically works with datasets using the `IOB`, `IOB2`, `BIOES`, `BILOU` or no label annotation scheme.
 
@@ -140,14 +141,16 @@
 <!-- Because this work is based on [PL-Marker](https://arxiv.org/pdf/2109.06067v5.pdf), you may expect similar results to its [Papers with Code Leaderboard](https://paperswithcode.com/paper/pack-together-entity-and-relation-extraction) results. -->
 
 ## Pretrained Models
 
 All models in this list contain `train.py` files that show the training scripts used to generate them. Additionally, all training scripts used are stored in the [training_scripts](training_scripts) directory.
 These trained models have Hosted Inference API widgets that you can use to experiment with the models on their Hugging Face model pages. Additionally, Hugging Face provides each model with a free API (`Deploy` > `Inference API` on the model page).
 
+These models are further elaborated on in my [thesis](https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf).
+
 ### FewNERD
 * [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is a model that I have trained in 2 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a 0.7053 Test F1, competitive in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup) using `bert-base`. My training script resembles the one that you can see above.
   * Try the model out online using this [🤗 Space](https://tomaarsen-span-marker-bert-base-fewnerd-fine-super.hf.space/).
 
 * [`tomaarsen/span-marker-roberta-large-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-roberta-large-fewnerd-fine-super) was trained in 6 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd) using `roberta-large`. It reached a 0.7103 Test F1, reaching a new state of the art in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup).
 * [`tomaarsen/span-marker-xlm-roberta-base-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-base-fewnerd-fine-super) is a multilingual model that I have trained in 1.5 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a 0.686 Test F1 on English, and works well on other languages like Spanish, French, German, Russian, Dutch, Polish, Icelandic, Greek and many more.
 
@@ -158,20 +161,20 @@
 * [`tomaarsen/span-marker-xlm-roberta-large-conll03`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conll03) is a SpanMarker model using `xlm-roberta-large` that was trained in 45 minutes. It reaches a state of the art 0.931 F1 on CoNLL03 without using document-level context. For reference, the current strongest spaCy model (`en_core_web_trf`) reaches 91.6.
 * [`tomaarsen/span-marker-xlm-roberta-large-conll03-doc-context`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conll03-doc-context) is another SpanMarker model using the `xlm-roberta-large` encoder. It uses [document-level context](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html) to reach a state of the art 0.944 F1. For the best performance, inference should be performed using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html#Inference)). This model was trained in 1 hour.
 
 ### CoNLL++
 * [`tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context`](https://huggingface.co/tomaarsen/span-marker-xlm-roberta-large-conllpp-doc-context) was trained in an hour using the `xlm-roberta-large` encoder on the CoNLL++ dataset. Using [document-level context](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html), it reaches a very competitive 0.955 F1. For the best performance, inference should be performed using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/notebooks/document_level_context.html#Inference)).
 
 ## Using pretrained SpanMarker models with spaCy
-All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the Documentation or API Reference for more information.
+All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the [Documentation](https://tomaarsen.github.io/SpanMarkerNER/notebooks/spacy_integration.html) or [API Reference](https://tomaarsen.github.io/SpanMarkerNER/api/span_marker.spacy_integration.html) for more information.
 ```python
 import spacy
 
 # Load the spaCy model with the span_marker pipeline component
-nlp = spacy.load("en_core_web_sm", disable=["ner"])
+nlp = spacy.load("en_core_web_sm", exclude=["ner"])
 nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
 # Feed some text through the model to get a spacy Doc
 text = """Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the \
 Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her \
 death in 30 BCE."""
 doc = nlp(text)
@@ -188,15 +191,14 @@
 ## Context
 <h1 align="center">
     <a href="https://github.com/argilla-io/argilla">
     <img src="https://github.com/dvsrepo/imgs/raw/main/rg.svg" alt="Argilla" width="150">
     </a>
 </h1>
 
-I have developed this library as a part of my thesis work at [Argilla](https://github.com/argilla-io/argilla).
-Feel free to ⭐ star or watch the SpanMarker repository to get notified when my thesis is published.
+I have developed this library as a part of my thesis work at [Argilla](https://github.com/argilla-io/argilla). Feel free to read my finished thesis [here](https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf) in this repository!
 
 ## Changelog
 See [CHANGELOG.md](CHANGELOG.md) for news on all SpanMarker versions.
 
 ## License
 See [LICENSE](LICENSE.md) for the current license.
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: span-marker Version: 1.2.3 Summary: Named Entity
+Metadata-Version: 2.1 Name: span-marker Version: 1.2.4 Summary: Named Entity
 Recognition using Span Markers Author: Tom Aarsen Maintainer: Tom Aarsen
-Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER Project-
-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER Keywords: data-
-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-
-learning,transformers Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev Provides-Extra: docs Provides-Extra: wandb
-License-File: LICENSE
+License: Apache-2.0 Project-URL: Documentation, https://tomaarsen.github.io/
+SpanMarkerNER Project-URL: Repository, https://github.com/tomaarsen/
+SpanMarkerNER Keywords: data-science,natural-language-processing,artificial-
+intelligence,mlops,nlp,machine-learning,transformers Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
+docs Provides-Extra: wandb License-File: LICENSE
              ****** SpanMarker for Named Entity Recognition ******
 [https://github.com/tomaarsen/SpanMarkerNER/assets/37621491/c76d6393-bb0b-44c3-
  9412-fd9c8313dcc1] [ð¤ Models](https://huggingface.co/models?library=span-
          marker) | [ð ï¸ Getting Started In Google Colab](https://
  colab.research.google.com/github/tomaarsen/SpanMarkerNER/blob/main/notebooks/
   getting_started.ipynb) | [ð Documentation](https://tomaarsen.github.io/
-                                SpanMarkerNER)
+  SpanMarkerNER) | ð [Thesis](https://raw.githubusercontent.com/tomaarsen/
+                        SpanMarkerNER/main/thesis.pdf)
 SpanMarker is a framework for training powerful Named Entity Recognition models
-using familiar encoders such as BERT, RoBERTa and DeBERTa. Built on top of the
+using familiar encoders such as BERT, RoBERTa and ELECTRA. Built on top of the
 familiar [ð¤ Transformers](https://github.com/huggingface/transformers)
 library, SpanMarker inherits a wide range of powerful functionalities, such as
 easily loading and saving models, hyperparameter optimization, automatic
 logging in various tools, checkpointing, callbacks, mixed precision training,
 8-bit inference, and more.   Based on the [PL-Marker](https://arxiv.org/pdf/
 2109.06067.pdf) paper, SpanMarker breaks the mold through its accessibility and
 ease of use. Crucially, SpanMarker works out of the box with many common
@@ -106,17 +107,19 @@
 0.9892390966415405, 'char_start_index': 78, 'char_end_index': 83}] ```  ##
 Pretrained Models All models in this list contain `train.py` files that show
 the training scripts used to generate them. Additionally, all training scripts
 used are stored in the [training_scripts](training_scripts) directory. These
 trained models have Hosted Inference API widgets that you can use to experiment
 with the models on their Hugging Face model pages. Additionally, Hugging Face
 provides each model with a free API (`Deploy` > `Inference API` on the model
-page). ### FewNERD * [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`]
-(https://huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is
-a model that I have trained in 2 hours on the finegrained, supervised [Few-NERD
+page). These models are further elaborated on in my [thesis](https://
+raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf). ### FewNERD
+* [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`](https://
+huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is a model
+that I have trained in 2 hours on the finegrained, supervised [Few-NERD
 dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a
 0.7053 Test F1, competitive in the all-time [Few-NERD leaderboard](https://
 paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup) using `bert-
 base`. My training script resembles the one that you can see above. * Try the
 model out online using this [ð¤ Space](https://tomaarsen-span-marker-bert-
 base-fewnerd-fine-super.hf.space/). * [`tomaarsen/span-marker-roberta-large-
 fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-roberta-
@@ -156,26 +159,29 @@
 SpanMarkerNER/notebooks/document_level_context.html), it reaches a very
 competitive 0.955 F1. For the best performance, inference should be performed
 using document-level context ([docs](https://tomaarsen.github.io/SpanMarkerNER/
 notebooks/document_level_context.html#Inference)). ## Using pretrained
 SpanMarker models with spaCy All [SpanMarker models on the Hugging Face Hub]
 (https://huggingface.co/models?library=span-marker) can also be easily used in
 spaCy. It's as simple as including 1 line to add the `span_marker` pipeline.
-See the Documentation or API Reference for more information. ```python import
-spacy # Load the spaCy model with the span_marker pipeline component nlp =
-spacy.load("en_core_web_sm", disable=["ner"]) nlp.add_pipe("span_marker",
-config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"}) # Feed some
-text through the model to get a spacy Doc text = """Cleopatra VII, also known
-as Cleopatra the Great, was the last active ruler of the \ Ptolemaic Kingdom of
-Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her \ death in
-30 BCE.""" doc = nlp(text) # And look at the entities print([(entity,
-entity.label_) for entity in doc.ents]) """ [(Cleopatra VII, "PERSON"),
-(Cleopatra the Great, "PERSON"), (the Ptolemaic Kingdom of Egypt, "GPE"), (69
-BCE, "DATE"), (Egypt, "GPE"), (51 BCE, "DATE"), (30 BCE, "DATE")] """ ``` !
-[image](https://user-images.githubusercontent.com/37621491/246170623-6351cb7e-
-bbb0-4472-af16-9a351a253da9.png) ## Context
+See the [Documentation](https://tomaarsen.github.io/SpanMarkerNER/notebooks/
+spacy_integration.html) or [API Reference](https://tomaarsen.github.io/
+SpanMarkerNER/api/span_marker.spacy_integration.html) for more information.
+```python import spacy # Load the spaCy model with the span_marker pipeline
+component nlp = spacy.load("en_core_web_sm", exclude=["ner"]) nlp.add_pipe
+("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-
+ontonotes5"}) # Feed some text through the model to get a spacy Doc text =
+"""Cleopatra VII, also known as Cleopatra the Great, was the last active ruler
+of the \ Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt
+from 51 BCE until her \ death in 30 BCE.""" doc = nlp(text) # And look at the
+entities print([(entity, entity.label_) for entity in doc.ents]) """ [
+(Cleopatra VII, "PERSON"), (Cleopatra the Great, "PERSON"), (the Ptolemaic
+Kingdom of Egypt, "GPE"), (69 BCE, "DATE"), (Egypt, "GPE"), (51 BCE, "DATE"),
+(30 BCE, "DATE")] """ ``` ![image](https://user-images.githubusercontent.com/
+37621491/246170623-6351cb7e-bbb0-4472-af16-9a351a253da9.png) ## Context
                             ****** [Argilla] ******
 I have developed this library as a part of my thesis work at [Argilla](https://
-github.com/argilla-io/argilla). Feel free to â­ star or watch the SpanMarker
-repository to get notified when my thesis is published. ## Changelog See
-[CHANGELOG.md](CHANGELOG.md) for news on all SpanMarker versions. ## License
-See [LICENSE](LICENSE.md) for the current license.
+github.com/argilla-io/argilla). Feel free to read my finished thesis [here]
+(https://raw.githubusercontent.com/tomaarsen/SpanMarkerNER/main/thesis.pdf) in
+this repository! ## Changelog See [CHANGELOG.md](CHANGELOG.md) for news on all
+SpanMarker versions. ## License See [LICENSE](LICENSE.md) for the current
+license.
```

### Comparing `span_marker-1.2.3/span_marker.egg-info/SOURCES.txt` & `span_marker-1.2.4/span_marker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/tests/test_configuration.py` & `span_marker-1.2.4/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/tests/test_model_card.py` & `span_marker-1.2.4/tests/test_model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/tests/test_modeling.py` & `span_marker-1.2.4/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.3/tests/test_spacy_integration.py` & `span_marker-1.2.4/tests/test_spacy_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import spacy
 
 
 def test_span_marker_as_spacy_pipeline_component():
-    nlp = spacy.load("en_core_web_sm", disable=["ner"])
+    nlp = spacy.load("en_core_web_sm", exclude=["ner"])
     batch_size = 2
     wrapper = nlp.add_pipe(
         "span_marker", config={"model": "tomaarsen/span-marker-bert-tiny-conll03", "batch_size": batch_size}
     )
     assert wrapper.batch_size == batch_size
 
     doc = nlp("Amelia Earhart flew her single engine Lockheed Vega 5B across the Atlantic to Paris.")
```

### Comparing `span_marker-1.2.3/tests/test_trainer.py` & `span_marker-1.2.4/tests/test_trainer.py`

 * *Files identical despite different names*

