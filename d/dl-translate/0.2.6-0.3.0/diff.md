# Comparing `tmp/dl-translate-0.2.6.tar.gz` & `tmp/dl-translate-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl-translate-0.2.6.tar", last modified: Wed Jul 13 21:28:22 2022, max compression
+gzip compressed data, was "dl-translate-0.3.0.tar", last modified: Tue Jul 18 05:38:53 2023, max compression
```

## Comparing `dl-translate-0.2.6.tar` & `dl-translate-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 21:28:22.454971 dl-translate-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-07-13 21:28:13.000000 dl-translate-0.2.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-07-13 21:28:13.000000 dl-translate-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-13 21:28:13.000000 dl-translate-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13044 2022-07-13 21:28:22.454971 dl-translate-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12509 2022-07-13 21:28:13.000000 dl-translate-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 21:28:22.450971 dl-translate-0.2.6/dl_translate/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-07-13 21:28:13.000000 dl-translate-0.2.6/dl_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4066 2022-07-13 21:28:13.000000 dl-translate-0.2.6/dl_translate/_pairs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10049 2022-07-13 21:28:13.000000 dl-translate-0.2.6/dl_translate/_translation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 21:28:22.454971 dl-translate-0.2.6/dl_translate/lang/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-07-13 21:28:13.000000 dl-translate-0.2.6/dl_translate/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-07-13 21:28:13.000000 dl-translate-0.2.6/dl_translate/lang/m2m100.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-07-13 21:28:13.000000 dl-translate-0.2.6/dl_translate/lang/mbart50.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-07-13 21:28:13.000000 dl-translate-0.2.6/dl_translate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 21:28:22.454971 dl-translate-0.2.6/dl_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13044 2022-07-13 21:28:22.000000 dl-translate-0.2.6/dl_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-07-13 21:28:22.000000 dl-translate-0.2.6/dl_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-13 21:28:22.000000 dl-translate-0.2.6/dl_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-07-13 21:28:22.000000 dl-translate-0.2.6/dl_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-13 21:28:22.000000 dl-translate-0.2.6/dl_translate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-13 21:28:22.454971 dl-translate-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-07-13 21:28:13.000000 dl-translate-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:38:53.349707 dl-translate-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-18 05:38:41.000000 dl-translate-0.3.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 05:38:41.000000 dl-translate-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 05:38:41.000000 dl-translate-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-07-18 05:38:53.349707 dl-translate-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-07-18 05:38:41.000000 dl-translate-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:38:53.349707 dl-translate-0.3.0/dl_translate/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/_translation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:38:53.349707 dl-translate-0.3.0/dl_translate/lang/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/lang/m2m100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/lang/mbart50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/lang/nllb200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-18 05:38:41.000000 dl-translate-0.3.0/dl_translate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:38:53.349707 dl-translate-0.3.0/dl_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 05:38:53.000000 dl-translate-0.3.0/dl_translate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 05:38:53.349707 dl-translate-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-18 05:38:41.000000 dl-translate-0.3.0/setup.py
```

### Comparing `dl-translate-0.2.6/LICENSE` & `dl-translate-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dl-translate-0.2.6/PKG-INFO` & `dl-translate-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,18 @@
-Metadata-Version: 2.1
-Name: dl-translate
-Version: 0.2.6
-Summary: A deep learning-based translation library built on Huggingface transformers
-Home-page: https://github.com/xhlulu/dl-translate
-Author: Xing Han Lu
-Author-email: github@xinghanlu.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # DL Translate
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5230676.svg)](https://doi.org/10.5281/zenodo.5230676)
 [![Downloads](https://static.pepy.tech/personalized-badge/dl-translate?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/dl-translate)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/xhluca/dl-translate/blob/main/LICENSE)
 
 
 *A deep learning-based translation library built on Huggingface `transformers`*
 
 💻 [GitHub Repository](https://github.com/xhluca/dl-translate)<br>
-📚 [Documentation](https://xhluca.github.io/dl-translate) / [Readthedocs](https://dl-translate.readthedocs.io)<br>
+📚 [Documentation](https://xhluca.github.io/dl-translate)<br>
 🐍 [PyPi project](https://pypi.org/project/dl-translate/)<br>
 🧪 [Colab Demo](https://colab.research.google.com/github/xhluca/dl-translate/blob/main/demos/colab_demo.ipynb) / [Kaggle Demo](https://www.kaggle.com/xhlulu/dl-translate-demo/)
 
 
 
 ## Quickstart
 
@@ -71,32 +54,42 @@
 mt = dlt.TranslationModel(device="auto")
 ```
 
 By default, the value will be `device="auto"`, which means it will use a GPU if possible. You can also explicitly set `device="cpu"` or `device="gpu"`, or some other strings accepted by [`torch.device()`](https://pytorch.org/docs/stable/tensor_attributes.html#torch.torch.device). __In general, it is recommend to use a GPU if you want a reasonable processing time.__
 
 ### Choosing a different model
 
-Two model families are available at the moment: [m2m100](https://huggingface.co/transformers/model_doc/m2m_100.html) and [mBART-50 Large](https://huggingface.co/transformers/master/model_doc/mbart.html), which respective allow translation across over 100 languages and 50 languages. By default, the model will select `m2m100`, but you can also explicitly choose the model by specifying the shorthand (`"m2m100"` or `"mbart50"`) or the full repository name (e.g. `"facebook/m2m100_418M"`). For example:
+By default, the `m2m100` model will be used. However, there are a few options:
+
+* [mBART-50 Large](https://huggingface.co/transformers/master/model_doc/mbart.html):  Allows translations across 50 languages.
+* [m2m100](https://huggingface.co/transformers/model_doc/m2m_100.html): Allows translations across 100 languages.
+* [nllb-200](https://huggingface.co/docs/transformers/model_doc/nllb) (New in v0.3): Allows translations across 200 languages, and is faster than m2m100 (On RTX A6000, we can see speed up of 3x).
 
+Here's an example:
 ```python
-# The following ways are equivalent
-mt = dlt.TranslationModel("m2m100")  # Default
-mt = dlt.TranslationModel("facebook/m2m100_418M")
+# The default approval
+mt = dlt.TranslationModel("m2m100")  # Shorthand
+mt = dlt.TranslationModel("facebook/m2m100_418M")  # Huggingface repo
 
-# The following ways are equivalent
+# If you want to use mBART-50 Large
 mt = dlt.TranslationModel("mbart50")
 mt = dlt.TranslationModel("facebook/mbart-large-50-many-to-many-mmt")
+
+# Or NLLB-200 (faster and has 200 languages)
+mt = dlt.TranslationModel("nllb200")
+mt = dlt.TranslationModel("facebook/nllb-200-distilled-600M")
 ```
 
 Note that the language code will change depending on the model family. To find out the correct language codes, please read the doc page on available languages or run `mt.available_codes()`.
 
-By default, `dlt.TranslationModel` will download the model from the huggingface repo for [mbart50](https://huggingface.co/facebook/mbart-large-50-one-to-many-mmt) or [m2m100](https://huggingface.co/facebook/m2m100_418M) and cache it. It's possible to load the model from a path or a model with a similar format, but you will need to specify the `model_family`:
+By default, `dlt.TranslationModel` will download the model from the huggingface repo for [mbart50](https://huggingface.co/facebook/mbart-large-50-one-to-many-mmt), [m2m100](https://huggingface.co/facebook/m2m100_418M), or [nllb200](https://huggingface.co/facebook/nllb-200-distilled-600M) and cache it. It's possible to load the model from a path or a model with a similar format, but you will need to specify the `model_family`:
 ```python
 mt = dlt.TranslationModel("/path/to/model/directory/", model_family="mbart50")
 mt = dlt.TranslationModel("facebook/m2m100_1.2B", model_family="m2m100")
+mt = dlt.TranslationModel("facebook/nllb-200-distilled-600M", model_family="nllb200")
 ```
 
 Notes:
 * Make sure your tokenizer is also stored in the same directory if you load from a file. 
 * The available languages will change if you select a different model, so you will not be able to leverage `dlt.lang` or `dlt.utils`.
 
 ### Splitting into sentences
@@ -127,16 +120,16 @@
 
 ### `dlt.utils` module
 
 An alternative to `mt.available_languages()` is the `dlt.utils` module. You can use it to find out which languages and codes are available:
 
 ```python
 print(dlt.utils.available_languages('mbart50'))  # All languages that you can use
-print(dlt.utils.available_codes('mbart50'))  # Code corresponding to each language accepted
-print(dlt.utils.get_lang_code_map('mbart50'))  # Dictionary of lang -> code
+print(dlt.utils.available_codes('m2m100'))  # Code corresponding to each language accepted
+print(dlt.utils.get_lang_code_map('nllb200'))  # Dictionary of lang -> code
 ```
 
 ### Offline usage
 
 Unlike the Google translate or MSFT Translator APIs, this library can be fully used offline. However, you will need to first download the packages and models, and move them to your offline environment to be installed and loaded inside a venv.
 
 First, run in your terminal:
@@ -145,19 +138,19 @@
 cd dlt
 mkdir libraries
 pip download -d libraries/ dl-translate
 ```
 
 Once all the required packages are downloaded, you will need to use huggingface hub to download the files. Install it with `pip install huggingface-hub`. Then, run inside Python:
 ```python
-import os
+import shutil
 import huggingface_hub as hub
 
 dirname = hub.snapshot_download("facebook/m2m100_418M")
-os.rename(dirname, "cached_model_m2m100")
+shutil.copytree(dirname, "cached_model_m2m100")  # Copy to a permanent folder
 ```
 
 Now, move everything in the `dlt` directory to your offline environment. Create a virtual environment and run the following in terminal:
 ```bash
 pip install --no-index --find-links libraries/ dl-translate
 ```
 
@@ -172,15 +165,15 @@
 ## Advanced
 
 If you have knowledge of PyTorch and Huggingface Transformers, you can access advanced aspects of the library for more customization:
 * **Saving and loading**: If you wish to accelerate the loading time the translation model, you can use `save_obj` and reload it later with `load_obj`. This method is only recommended if you are familiar with `huggingface` and `torch`; please read the docs for more information.
 * **Interacting with underlying model and tokenizer**: When initializing `model`, you can pass in arguments for the underlying BART model and tokenizer with `model_options` and `tokenizer_options` respectively. You can also access the underlying `transformers` with `mt.get_transformers_model()`.
 * **Keyword arguments for the `generate()` method**: When running `mt.translate`, you can also give `generation_options` that is passed to the `generate()` method of the underlying transformer model.
 
-For more information, please visit the [advanced section of the user guide](https://xhluca.github.io/dl-translate/#advanced) (also available in the [readthedocs version](https://dl-translate.readthedocs.io/en/latest/#advanced)).
+For more information, please visit the [advanced section of the user guide](https://xhluca.github.io/dl-translate/#advanced).
 
 ## Acknowledgement
 
 `dl-translate` is built on top of Huggingface's implementation of two models created by Facebook AI Research.
 
 1. The multilingual BART finetuned on many-to-many translation of over 50 languages, which is [documented here](https://huggingface.co/transformers/master/model_doc/mbart.html) The original paper was written by Tang et. al from Facebook AI Research; you can [find it here](https://arxiv.org/pdf/2008.00401.pdf) and cite it using the following:
     ```
@@ -199,14 +192,27 @@
         year={2020},
         eprint={2010.11125},
         archivePrefix={arXiv},
         primaryClass={cs.CL}
     }
    ```
 
+3. The [no language left behind](https://arxiv.org/abs/2207.04672) model, which extends NMT to 200+ languages. You can cite it here:
+    ```
+    @misc{nllbteam2022language,
+        title={No Language Left Behind: Scaling Human-Centered Machine Translation}, 
+        author={NLLB Team and Marta R. Costa-jussà and James Cross and Onur Çelebi and Maha Elbayad and Kenneth Heafield and Kevin Heffernan and Elahe Kalbassi and Janice Lam and Daniel Licht and Jean Maillard and Anna Sun and Skyler Wang and Guillaume Wenzek and Al Youngblood and Bapi Akula and Loic Barrault and Gabriel Mejia Gonzalez and Prangthip Hansanti and John Hoffman and Semarley Jarrett and Kaushik Ram Sadagopan and Dirk Rowe and Shannon Spruit and Chau Tran and Pierre Andrews and Necip Fazil Ayan and Shruti Bhosale and Sergey Edunov and Angela Fan and Cynthia Gao and Vedanuj Goswami and Francisco Guzmán and Philipp Koehn and Alexandre Mourachko and Christophe Ropers and Safiyyah Saleem and Holger Schwenk and Jeff Wang},
+        year={2022},
+        eprint={2207.04672},
+        archivePrefix={arXiv},
+        primaryClass={cs.CL}
+    }
+    ```
+
+
 `dlt` is a wrapper with useful `utils` to save you time. For huggingface's `transformers`, the following snippet is shown as an example:
 ```python
 from transformers import MBartForConditionalGeneration, MBart50TokenizerFast
 
 article_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
 article_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
 
@@ -239,9 +245,7 @@
 translated_fr = mt.translate(article_hi, source=dlt.lang.HINDI, target=dlt.lang.FRENCH)
 translated_en = mt.translate(article_ar, source=dlt.lang.ARABIC, target=dlt.lang.ENGLISH)
 ```
 
 Notice you don't have to think about tokenizers, condition generation, pretrained models, and regional codes; you can just tell the model what to translate!
 
 If you are experienced with `huggingface`'s ecosystem, then you should be familiar enough with the example above that you wouldn't need this library. However, if you've never heard of huggingface or mBART, then I hope using this library will give you enough motivation to [learn more about them](https://github.com/huggingface/transformers) :)
-
-
```

### Comparing `dl-translate-0.2.6/README.md` & `dl-translate-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,228 +1,267 @@
-# DL Translate
-
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5230676.svg)](https://doi.org/10.5281/zenodo.5230676)
-[![Downloads](https://static.pepy.tech/personalized-badge/dl-translate?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/dl-translate)
-[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/xhluca/dl-translate/blob/main/LICENSE)
-
-
-*A deep learning-based translation library built on Huggingface `transformers`*
-
-💻 [GitHub Repository](https://github.com/xhluca/dl-translate)<br>
-📚 [Documentation](https://xhluca.github.io/dl-translate) / [Readthedocs](https://dl-translate.readthedocs.io)<br>
-🐍 [PyPi project](https://pypi.org/project/dl-translate/)<br>
-🧪 [Colab Demo](https://colab.research.google.com/github/xhluca/dl-translate/blob/main/demos/colab_demo.ipynb) / [Kaggle Demo](https://www.kaggle.com/xhlulu/dl-translate-demo/)
-
-
-
-## Quickstart
-
-Install the library with pip:
-```
-pip install dl-translate
-```
-
-To translate some text:
-
-```python
-import dl_translate as dlt
-
-mt = dlt.TranslationModel()  # Slow when you load it for the first time
-
-text_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
-mt.translate(text_hi, source=dlt.lang.HINDI, target=dlt.lang.ENGLISH)
-```
-
-Above, you can see that `dlt.lang` contains variables representing each of the 50 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
-```python
-text_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
-mt.translate(text_ar, source="Arabic", target="fr")
-```
-
-If you want to verify whether a language is available, you can check it:
-```python
-print(mt.available_languages())  # All languages that you can use
-print(mt.available_codes())  # Code corresponding to each language accepted
-print(mt.get_lang_code_map())  # Dictionary of lang -> code
-```
-
-## Usage
-
-### Selecting a device
-
-When you load the model, you can specify the device:
-```python
-mt = dlt.TranslationModel(device="auto")
-```
-
-By default, the value will be `device="auto"`, which means it will use a GPU if possible. You can also explicitly set `device="cpu"` or `device="gpu"`, or some other strings accepted by [`torch.device()`](https://pytorch.org/docs/stable/tensor_attributes.html#torch.torch.device). __In general, it is recommend to use a GPU if you want a reasonable processing time.__
-
-### Choosing a different model
-
-Two model families are available at the moment: [m2m100](https://huggingface.co/transformers/model_doc/m2m_100.html) and [mBART-50 Large](https://huggingface.co/transformers/master/model_doc/mbart.html), which respective allow translation across over 100 languages and 50 languages. By default, the model will select `m2m100`, but you can also explicitly choose the model by specifying the shorthand (`"m2m100"` or `"mbart50"`) or the full repository name (e.g. `"facebook/m2m100_418M"`). For example:
-
-```python
-# The following ways are equivalent
-mt = dlt.TranslationModel("m2m100")  # Default
-mt = dlt.TranslationModel("facebook/m2m100_418M")
-
-# The following ways are equivalent
-mt = dlt.TranslationModel("mbart50")
-mt = dlt.TranslationModel("facebook/mbart-large-50-many-to-many-mmt")
-```
-
-Note that the language code will change depending on the model family. To find out the correct language codes, please read the doc page on available languages or run `mt.available_codes()`.
-
-By default, `dlt.TranslationModel` will download the model from the huggingface repo for [mbart50](https://huggingface.co/facebook/mbart-large-50-one-to-many-mmt) or [m2m100](https://huggingface.co/facebook/m2m100_418M) and cache it. It's possible to load the model from a path or a model with a similar format, but you will need to specify the `model_family`:
-```python
-mt = dlt.TranslationModel("/path/to/model/directory/", model_family="mbart50")
-mt = dlt.TranslationModel("facebook/m2m100_1.2B", model_family="m2m100")
-```
-
-Notes:
-* Make sure your tokenizer is also stored in the same directory if you load from a file. 
-* The available languages will change if you select a different model, so you will not be able to leverage `dlt.lang` or `dlt.utils`.
-
-### Splitting into sentences
-
-It is not recommended to use extremely long texts as it takes more time to process. Instead, you can try to break them down into sentences with the help of `nltk`. First install the library with `pip install nltk`, then run:
-```python
-import nltk
-
-nltk.download("punkt")
-
-text = "Mr. Smith went to his favorite cafe. There, he met his friend Dr. Doe."
-sents = nltk.tokenize.sent_tokenize(text, "english")  # don't use dlt.lang.ENGLISH
-" ".join(mt.translate(sents, source=dlt.lang.ENGLISH, target=dlt.lang.FRENCH))
-```
-
-### Batch size during translation
-
-It's possible to set a batch size (i.e. the number of elements processed at once) for `mt.translate` and whether you want to see the progress bar or not:
-
-```python
-# ...
-mt = dlt.TranslationModel()
-mt.translate(text, source, target, batch_size=32, verbose=True)
-```
-
-If you set `batch_size=None`, it will compute the entire `text` at once rather than splitting into "chunks". We recommend lowering `batch_size` if you do not have a lot of RAM or VRAM and run into CUDA memory error. Set a higher value if you are using a high-end GPU and the VRAM is not fully utilized.
-
-
-### `dlt.utils` module
-
-An alternative to `mt.available_languages()` is the `dlt.utils` module. You can use it to find out which languages and codes are available:
-
-```python
-print(dlt.utils.available_languages('mbart50'))  # All languages that you can use
-print(dlt.utils.available_codes('mbart50'))  # Code corresponding to each language accepted
-print(dlt.utils.get_lang_code_map('mbart50'))  # Dictionary of lang -> code
-```
-
-### Offline usage
-
-Unlike the Google translate or MSFT Translator APIs, this library can be fully used offline. However, you will need to first download the packages and models, and move them to your offline environment to be installed and loaded inside a venv.
-
-First, run in your terminal:
-```bash
-mkdir dlt
-cd dlt
-mkdir libraries
-pip download -d libraries/ dl-translate
-```
-
-Once all the required packages are downloaded, you will need to use huggingface hub to download the files. Install it with `pip install huggingface-hub`. Then, run inside Python:
-```python
-import os
-import huggingface_hub as hub
-
-dirname = hub.snapshot_download("facebook/m2m100_418M")
-os.rename(dirname, "cached_model_m2m100")
-```
-
-Now, move everything in the `dlt` directory to your offline environment. Create a virtual environment and run the following in terminal:
-```bash
-pip install --no-index --find-links libraries/ dl-translate
-```
-
-Now, run inside Python:
-```python
-import dl_translate as dlt
-
-mt = dlt.TranslationModel("cached_model_m2m100", model_family="m2m100")
-```
-
-
-## Advanced
-
-If you have knowledge of PyTorch and Huggingface Transformers, you can access advanced aspects of the library for more customization:
-* **Saving and loading**: If you wish to accelerate the loading time the translation model, you can use `save_obj` and reload it later with `load_obj`. This method is only recommended if you are familiar with `huggingface` and `torch`; please read the docs for more information.
-* **Interacting with underlying model and tokenizer**: When initializing `model`, you can pass in arguments for the underlying BART model and tokenizer with `model_options` and `tokenizer_options` respectively. You can also access the underlying `transformers` with `mt.get_transformers_model()`.
-* **Keyword arguments for the `generate()` method**: When running `mt.translate`, you can also give `generation_options` that is passed to the `generate()` method of the underlying transformer model.
-
-For more information, please visit the [advanced section of the user guide](https://xhluca.github.io/dl-translate/#advanced) (also available in the [readthedocs version](https://dl-translate.readthedocs.io/en/latest/#advanced)).
-
-## Acknowledgement
-
-`dl-translate` is built on top of Huggingface's implementation of two models created by Facebook AI Research.
-
-1. The multilingual BART finetuned on many-to-many translation of over 50 languages, which is [documented here](https://huggingface.co/transformers/master/model_doc/mbart.html) The original paper was written by Tang et. al from Facebook AI Research; you can [find it here](https://arxiv.org/pdf/2008.00401.pdf) and cite it using the following:
-    ```
-    @article{tang2020multilingual,
-        title={Multilingual translation with extensible multilingual pretraining and finetuning},
-        author={Tang, Yuqing and Tran, Chau and Li, Xian and Chen, Peng-Jen and Goyal, Naman and Chaudhary, Vishrav and Gu, Jiatao and Fan, Angela},
-        journal={arXiv preprint arXiv:2008.00401},
-        year={2020}
-    }
-    ```
-2. The transformer model published in [Beyond English-Centric Multilingual Machine Translation](https://arxiv.org/abs/2010.11125) by Fan et. al, which supports over 100 languages. You can cite it here:
-   ```
-   @misc{fan2020englishcentric,
-        title={Beyond English-Centric Multilingual Machine Translation}, 
-        author={Angela Fan and Shruti Bhosale and Holger Schwenk and Zhiyi Ma and Ahmed El-Kishky and Siddharth Goyal and Mandeep Baines and Onur Celebi and Guillaume Wenzek and Vishrav Chaudhary and Naman Goyal and Tom Birch and Vitaliy Liptchinsky and Sergey Edunov and Edouard Grave and Michael Auli and Armand Joulin},
-        year={2020},
-        eprint={2010.11125},
-        archivePrefix={arXiv},
-        primaryClass={cs.CL}
-    }
-   ```
-
-`dlt` is a wrapper with useful `utils` to save you time. For huggingface's `transformers`, the following snippet is shown as an example:
-```python
-from transformers import MBartForConditionalGeneration, MBart50TokenizerFast
-
-article_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
-article_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
-
-model = MBartForConditionalGeneration.from_pretrained("facebook/mbart-large-50-many-to-many-mmt")
-tokenizer = MBart50TokenizerFast.from_pretrained("facebook/mbart-large-50-many-to-many-mmt")
-
-# translate Hindi to French
-tokenizer.src_lang = "hi_IN"
-encoded_hi = tokenizer(article_hi, return_tensors="pt")
-generated_tokens = model.generate(**encoded_hi, forced_bos_token_id=tokenizer.lang_code_to_id["fr_XX"])
-tokenizer.batch_decode(generated_tokens, skip_special_tokens=True)
-# => "Le chef de l 'ONU affirme qu 'il n 'y a pas de solution militaire en Syria."
-
-# translate Arabic to English
-tokenizer.src_lang = "ar_AR"
-encoded_ar = tokenizer(article_ar, return_tensors="pt")
-generated_tokens = model.generate(**encoded_ar, forced_bos_token_id=tokenizer.lang_code_to_id["en_XX"])
-tokenizer.batch_decode(generated_tokens, skip_special_tokens=True)
-# => "The Secretary-General of the United Nations says there is no military solution in Syria."
-```
-
-With `dlt`, you can run:
-```python
-import dl_translate as dlt
-
-article_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
-article_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
-
-mt = dlt.TranslationModel()
-translated_fr = mt.translate(article_hi, source=dlt.lang.HINDI, target=dlt.lang.FRENCH)
-translated_en = mt.translate(article_ar, source=dlt.lang.ARABIC, target=dlt.lang.ENGLISH)
-```
-
-Notice you don't have to think about tokenizers, condition generation, pretrained models, and regional codes; you can just tell the model what to translate!
-
-If you are experienced with `huggingface`'s ecosystem, then you should be familiar enough with the example above that you wouldn't need this library. However, if you've never heard of huggingface or mBART, then I hope using this library will give you enough motivation to [learn more about them](https://github.com/huggingface/transformers) :)
+Metadata-Version: 2.1
+Name: dl-translate
+Version: 0.3.0
+Summary: A deep learning-based translation library built on Huggingface transformers
+Home-page: https://github.com/xhlulu/dl-translate
+Author: Xing Han Lu
+Author-email: github@xinghanlu.com
+License: UNKNOWN
+Description: # DL Translate
+        
+        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5230676.svg)](https://doi.org/10.5281/zenodo.5230676)
+        [![Downloads](https://static.pepy.tech/personalized-badge/dl-translate?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/dl-translate)
+        [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/xhluca/dl-translate/blob/main/LICENSE)
+        
+        
+        *A deep learning-based translation library built on Huggingface `transformers`*
+        
+        💻 [GitHub Repository](https://github.com/xhluca/dl-translate)<br>
+        📚 [Documentation](https://xhluca.github.io/dl-translate)<br>
+        🐍 [PyPi project](https://pypi.org/project/dl-translate/)<br>
+        🧪 [Colab Demo](https://colab.research.google.com/github/xhluca/dl-translate/blob/main/demos/colab_demo.ipynb) / [Kaggle Demo](https://www.kaggle.com/xhlulu/dl-translate-demo/)
+        
+        
+        
+        ## Quickstart
+        
+        Install the library with pip:
+        ```
+        pip install dl-translate
+        ```
+        
+        To translate some text:
+        
+        ```python
+        import dl_translate as dlt
+        
+        mt = dlt.TranslationModel()  # Slow when you load it for the first time
+        
+        text_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
+        mt.translate(text_hi, source=dlt.lang.HINDI, target=dlt.lang.ENGLISH)
+        ```
+        
+        Above, you can see that `dlt.lang` contains variables representing each of the 50 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
+        ```python
+        text_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
+        mt.translate(text_ar, source="Arabic", target="fr")
+        ```
+        
+        If you want to verify whether a language is available, you can check it:
+        ```python
+        print(mt.available_languages())  # All languages that you can use
+        print(mt.available_codes())  # Code corresponding to each language accepted
+        print(mt.get_lang_code_map())  # Dictionary of lang -> code
+        ```
+        
+        ## Usage
+        
+        ### Selecting a device
+        
+        When you load the model, you can specify the device:
+        ```python
+        mt = dlt.TranslationModel(device="auto")
+        ```
+        
+        By default, the value will be `device="auto"`, which means it will use a GPU if possible. You can also explicitly set `device="cpu"` or `device="gpu"`, or some other strings accepted by [`torch.device()`](https://pytorch.org/docs/stable/tensor_attributes.html#torch.torch.device). __In general, it is recommend to use a GPU if you want a reasonable processing time.__
+        
+        ### Choosing a different model
+        
+        By default, the `m2m100` model will be used. However, there are a few options:
+        
+        * [mBART-50 Large](https://huggingface.co/transformers/master/model_doc/mbart.html):  Allows translations across 50 languages.
+        * [m2m100](https://huggingface.co/transformers/model_doc/m2m_100.html): Allows translations across 100 languages.
+        * [nllb-200](https://huggingface.co/docs/transformers/model_doc/nllb) (New in v0.3): Allows translations across 200 languages, and is faster than m2m100 (On RTX A6000, we can see speed up of 3x).
+        
+        Here's an example:
+        ```python
+        # The default approval
+        mt = dlt.TranslationModel("m2m100")  # Shorthand
+        mt = dlt.TranslationModel("facebook/m2m100_418M")  # Huggingface repo
+        
+        # If you want to use mBART-50 Large
+        mt = dlt.TranslationModel("mbart50")
+        mt = dlt.TranslationModel("facebook/mbart-large-50-many-to-many-mmt")
+        
+        # Or NLLB-200 (faster and has 200 languages)
+        mt = dlt.TranslationModel("nllb200")
+        mt = dlt.TranslationModel("facebook/nllb-200-distilled-600M")
+        ```
+        
+        Note that the language code will change depending on the model family. To find out the correct language codes, please read the doc page on available languages or run `mt.available_codes()`.
+        
+        By default, `dlt.TranslationModel` will download the model from the huggingface repo for [mbart50](https://huggingface.co/facebook/mbart-large-50-one-to-many-mmt), [m2m100](https://huggingface.co/facebook/m2m100_418M), or [nllb200](https://huggingface.co/facebook/nllb-200-distilled-600M) and cache it. It's possible to load the model from a path or a model with a similar format, but you will need to specify the `model_family`:
+        ```python
+        mt = dlt.TranslationModel("/path/to/model/directory/", model_family="mbart50")
+        mt = dlt.TranslationModel("facebook/m2m100_1.2B", model_family="m2m100")
+        mt = dlt.TranslationModel("facebook/nllb-200-distilled-600M", model_family="nllb200")
+        ```
+        
+        Notes:
+        * Make sure your tokenizer is also stored in the same directory if you load from a file. 
+        * The available languages will change if you select a different model, so you will not be able to leverage `dlt.lang` or `dlt.utils`.
+        
+        ### Splitting into sentences
+        
+        It is not recommended to use extremely long texts as it takes more time to process. Instead, you can try to break them down into sentences with the help of `nltk`. First install the library with `pip install nltk`, then run:
+        ```python
+        import nltk
+        
+        nltk.download("punkt")
+        
+        text = "Mr. Smith went to his favorite cafe. There, he met his friend Dr. Doe."
+        sents = nltk.tokenize.sent_tokenize(text, "english")  # don't use dlt.lang.ENGLISH
+        " ".join(mt.translate(sents, source=dlt.lang.ENGLISH, target=dlt.lang.FRENCH))
+        ```
+        
+        ### Batch size during translation
+        
+        It's possible to set a batch size (i.e. the number of elements processed at once) for `mt.translate` and whether you want to see the progress bar or not:
+        
+        ```python
+        # ...
+        mt = dlt.TranslationModel()
+        mt.translate(text, source, target, batch_size=32, verbose=True)
+        ```
+        
+        If you set `batch_size=None`, it will compute the entire `text` at once rather than splitting into "chunks". We recommend lowering `batch_size` if you do not have a lot of RAM or VRAM and run into CUDA memory error. Set a higher value if you are using a high-end GPU and the VRAM is not fully utilized.
+        
+        
+        ### `dlt.utils` module
+        
+        An alternative to `mt.available_languages()` is the `dlt.utils` module. You can use it to find out which languages and codes are available:
+        
+        ```python
+        print(dlt.utils.available_languages('mbart50'))  # All languages that you can use
+        print(dlt.utils.available_codes('m2m100'))  # Code corresponding to each language accepted
+        print(dlt.utils.get_lang_code_map('nllb200'))  # Dictionary of lang -> code
+        ```
+        
+        ### Offline usage
+        
+        Unlike the Google translate or MSFT Translator APIs, this library can be fully used offline. However, you will need to first download the packages and models, and move them to your offline environment to be installed and loaded inside a venv.
+        
+        First, run in your terminal:
+        ```bash
+        mkdir dlt
+        cd dlt
+        mkdir libraries
+        pip download -d libraries/ dl-translate
+        ```
+        
+        Once all the required packages are downloaded, you will need to use huggingface hub to download the files. Install it with `pip install huggingface-hub`. Then, run inside Python:
+        ```python
+        import shutil
+        import huggingface_hub as hub
+        
+        dirname = hub.snapshot_download("facebook/m2m100_418M")
+        shutil.copytree(dirname, "cached_model_m2m100")  # Copy to a permanent folder
+        ```
+        
+        Now, move everything in the `dlt` directory to your offline environment. Create a virtual environment and run the following in terminal:
+        ```bash
+        pip install --no-index --find-links libraries/ dl-translate
+        ```
+        
+        Now, run inside Python:
+        ```python
+        import dl_translate as dlt
+        
+        mt = dlt.TranslationModel("cached_model_m2m100", model_family="m2m100")
+        ```
+        
+        
+        ## Advanced
+        
+        If you have knowledge of PyTorch and Huggingface Transformers, you can access advanced aspects of the library for more customization:
+        * **Saving and loading**: If you wish to accelerate the loading time the translation model, you can use `save_obj` and reload it later with `load_obj`. This method is only recommended if you are familiar with `huggingface` and `torch`; please read the docs for more information.
+        * **Interacting with underlying model and tokenizer**: When initializing `model`, you can pass in arguments for the underlying BART model and tokenizer with `model_options` and `tokenizer_options` respectively. You can also access the underlying `transformers` with `mt.get_transformers_model()`.
+        * **Keyword arguments for the `generate()` method**: When running `mt.translate`, you can also give `generation_options` that is passed to the `generate()` method of the underlying transformer model.
+        
+        For more information, please visit the [advanced section of the user guide](https://xhluca.github.io/dl-translate/#advanced).
+        
+        ## Acknowledgement
+        
+        `dl-translate` is built on top of Huggingface's implementation of two models created by Facebook AI Research.
+        
+        1. The multilingual BART finetuned on many-to-many translation of over 50 languages, which is [documented here](https://huggingface.co/transformers/master/model_doc/mbart.html) The original paper was written by Tang et. al from Facebook AI Research; you can [find it here](https://arxiv.org/pdf/2008.00401.pdf) and cite it using the following:
+            ```
+            @article{tang2020multilingual,
+                title={Multilingual translation with extensible multilingual pretraining and finetuning},
+                author={Tang, Yuqing and Tran, Chau and Li, Xian and Chen, Peng-Jen and Goyal, Naman and Chaudhary, Vishrav and Gu, Jiatao and Fan, Angela},
+                journal={arXiv preprint arXiv:2008.00401},
+                year={2020}
+            }
+            ```
+        2. The transformer model published in [Beyond English-Centric Multilingual Machine Translation](https://arxiv.org/abs/2010.11125) by Fan et. al, which supports over 100 languages. You can cite it here:
+           ```
+           @misc{fan2020englishcentric,
+                title={Beyond English-Centric Multilingual Machine Translation}, 
+                author={Angela Fan and Shruti Bhosale and Holger Schwenk and Zhiyi Ma and Ahmed El-Kishky and Siddharth Goyal and Mandeep Baines and Onur Celebi and Guillaume Wenzek and Vishrav Chaudhary and Naman Goyal and Tom Birch and Vitaliy Liptchinsky and Sergey Edunov and Edouard Grave and Michael Auli and Armand Joulin},
+                year={2020},
+                eprint={2010.11125},
+                archivePrefix={arXiv},
+                primaryClass={cs.CL}
+            }
+           ```
+        
+        3. The [no language left behind](https://arxiv.org/abs/2207.04672) model, which extends NMT to 200+ languages. You can cite it here:
+            ```
+            @misc{nllbteam2022language,
+                title={No Language Left Behind: Scaling Human-Centered Machine Translation}, 
+                author={NLLB Team and Marta R. Costa-jussà and James Cross and Onur Çelebi and Maha Elbayad and Kenneth Heafield and Kevin Heffernan and Elahe Kalbassi and Janice Lam and Daniel Licht and Jean Maillard and Anna Sun and Skyler Wang and Guillaume Wenzek and Al Youngblood and Bapi Akula and Loic Barrault and Gabriel Mejia Gonzalez and Prangthip Hansanti and John Hoffman and Semarley Jarrett and Kaushik Ram Sadagopan and Dirk Rowe and Shannon Spruit and Chau Tran and Pierre Andrews and Necip Fazil Ayan and Shruti Bhosale and Sergey Edunov and Angela Fan and Cynthia Gao and Vedanuj Goswami and Francisco Guzmán and Philipp Koehn and Alexandre Mourachko and Christophe Ropers and Safiyyah Saleem and Holger Schwenk and Jeff Wang},
+                year={2022},
+                eprint={2207.04672},
+                archivePrefix={arXiv},
+                primaryClass={cs.CL}
+            }
+            ```
+        
+        
+        `dlt` is a wrapper with useful `utils` to save you time. For huggingface's `transformers`, the following snippet is shown as an example:
+        ```python
+        from transformers import MBartForConditionalGeneration, MBart50TokenizerFast
+        
+        article_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
+        article_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
+        
+        model = MBartForConditionalGeneration.from_pretrained("facebook/mbart-large-50-many-to-many-mmt")
+        tokenizer = MBart50TokenizerFast.from_pretrained("facebook/mbart-large-50-many-to-many-mmt")
+        
+        # translate Hindi to French
+        tokenizer.src_lang = "hi_IN"
+        encoded_hi = tokenizer(article_hi, return_tensors="pt")
+        generated_tokens = model.generate(**encoded_hi, forced_bos_token_id=tokenizer.lang_code_to_id["fr_XX"])
+        tokenizer.batch_decode(generated_tokens, skip_special_tokens=True)
+        # => "Le chef de l 'ONU affirme qu 'il n 'y a pas de solution militaire en Syria."
+        
+        # translate Arabic to English
+        tokenizer.src_lang = "ar_AR"
+        encoded_ar = tokenizer(article_ar, return_tensors="pt")
+        generated_tokens = model.generate(**encoded_ar, forced_bos_token_id=tokenizer.lang_code_to_id["en_XX"])
+        tokenizer.batch_decode(generated_tokens, skip_special_tokens=True)
+        # => "The Secretary-General of the United Nations says there is no military solution in Syria."
+        ```
+        
+        With `dlt`, you can run:
+        ```python
+        import dl_translate as dlt
+        
+        article_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
+        article_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
+        
+        mt = dlt.TranslationModel()
+        translated_fr = mt.translate(article_hi, source=dlt.lang.HINDI, target=dlt.lang.FRENCH)
+        translated_en = mt.translate(article_ar, source=dlt.lang.ARABIC, target=dlt.lang.ENGLISH)
+        ```
+        
+        Notice you don't have to think about tokenizers, condition generation, pretrained models, and regional codes; you can just tell the model what to translate!
+        
+        If you are experienced with `huggingface`'s ecosystem, then you should be familiar enough with the example above that you wouldn't need this library. However, if you've never heard of huggingface or mBART, then I hope using this library will give you enough motivation to [learn more about them](https://github.com/huggingface/transformers) :)
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `dl-translate-0.2.6/dl_translate/_translation_model.py` & `dl-translate-0.3.0/dl_translate/_translation_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Union, List, Dict
 
 import transformers
 import torch
 from tqdm.auto import tqdm
 
 from . import utils
+from .utils import _infer_model_family, _infer_model_or_path
 
 
 def _select_device(device_selection):
     selected = device_selection.lower()
     if selected == "auto":
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     elif selected == "cpu":
@@ -19,81 +20,66 @@
         device = torch.device("cuda")
     else:
         device = torch.device(selected)
 
     return device
 
 
-def _resolve_lang_codes(source: str, target: str, model_family: str):
+def _resolve_lang_codes(lang: str, name: str, model_family: str):
     def error_message(variable, value):
-        return f'Your {variable}="{value}" is not valid. Please run `print(mt.available_languages())` to see which languages are available.'
+        return f'Your {variable}="{value}" is not valid. Please run `print(mt.available_languages())` to see which languages are available. Make sure you are using the correct capital letters.'
 
     # If can't find in the lang -> code mapping, assumes it's already a code.
     lang_code_map = utils.get_lang_code_map(model_family)
-    source = lang_code_map.get(source.capitalize(), source)
-    target = lang_code_map.get(target.capitalize(), target)
+    if lang in lang_code_map:
+        code = lang_code_map[lang]
+    elif lang.capitalize() in lang_code_map:
+        code = lang_code_map[lang.capitalize()]
+    else:
+        lang_upper = lang.upper()
+        lang_code_map_upper = {k.upper(): v for k, v in lang_code_map.items()}
+
+        if lang_upper in lang_code_map_upper:
+            code = lang_code_map_upper[lang_upper]
+        else:
+            code = lang
 
     # If the code is not valid, raises an error
-    if source not in utils.available_codes(model_family):
-        raise ValueError(error_message("source", source))
-    if target not in utils.available_codes(model_family):
-        raise ValueError(error_message("target", target))
+    if code not in utils.available_codes(model_family):
+        raise ValueError(error_message(name, code))
 
-    return source, target
+    return code
 
 
 def _resolve_tokenizer(model_family):
     di = {
         "mbart50": transformers.MBart50TokenizerFast,
         "m2m100": transformers.M2M100Tokenizer,
+        "nllb200": transformers.AutoTokenizer,
     }
     if model_family in di:
         return di[model_family]
     else:
         error_msg = f"{model_family} is not a valid value for model_family. Please choose model_family to be equal to one of the following values: {list(di.keys())}"
         raise ValueError(error_msg)
 
 
 def _resolve_transformers_model(model_family):
     di = {
         "mbart50": transformers.MBartForConditionalGeneration,
         "m2m100": transformers.M2M100ForConditionalGeneration,
+        "nllb200": transformers.AutoModelForSeq2SeqLM,
     }
     if model_family in di:
         return di[model_family]
     else:
         error_msg = f"{model_family} is not a valid value for model_family. Please choose model_family to be equal to one of the following values: {list(di.keys())}"
         raise ValueError(error_msg)
 
 
-def _infer_model_family(model_or_path):
-    di = {
-        "facebook/mbart-large-50-many-to-many-mmt": "mbart50",
-        "facebook/m2m100_418M": "m2m100",
-        "facebook/m2m100_1.2B": "m2m100",
-    }
-
-    if model_or_path in di:
-        return di[model_or_path]
-    else:
-        error_msg = f'Unable to infer the model_family from "{model_or_path}". Try explicitly setting the value of model_family to "mbart50" or "m2m100".'
-        raise ValueError(error_msg)
-
-
-def _infer_model_or_path(model_or_path):
-    di = {
-        "mbart50": "facebook/mbart-large-50-many-to-many-mmt",
-        "m2m100": "facebook/m2m100_418M",
-        "m2m100-small": "facebook/m2m100_418M",
-        "m2m100-medium": "facebook/m2m100_1.2B",
-    }
-
-    return di.get(model_or_path, model_or_path)
-
-
 class TranslationModel:
     def __init__(
         self,
         model_or_path: str = "m2m100",
         tokenizer_path: str = None,
         device: str = "auto",
         model_family: str = None,
@@ -167,27 +153,30 @@
         Note:
         - Run `print(dlt.utils.available_languages())` to see what's available.
         - A smaller value is preferred for `batch_size` if your (video) RAM is limited.
         """
         if generation_options is None:
             generation_options = {}
 
-        source, target = _resolve_lang_codes(source, target, self.model_family)
+        source = _resolve_lang_codes(source, "source", self.model_family)
+        target = _resolve_lang_codes(target, "target", self.model_family)
+
         self._tokenizer.src_lang = source
 
         original_text_type = type(text)
         if original_text_type is str:
             text = [text]
 
         if batch_size is None:
             batch_size = len(text)
 
         generation_options.setdefault(
             "forced_bos_token_id", self._tokenizer.lang_code_to_id[target]
         )
+        generation_options.setdefault("max_new_tokens", 512)
 
         data_loader = torch.utils.data.DataLoader(text, batch_size=batch_size)
         output_text = []
 
         with torch.no_grad():
             for batch in tqdm(data_loader, disable=not verbose):
                 encoded = self._tokenizer(batch, return_tensors="pt", padding=True)
```

### Comparing `dl-translate-0.2.6/dl_translate/lang/m2m100.py` & `dl-translate-0.3.0/dl_translate/lang/m2m100.py`

 * *Files identical despite different names*

### Comparing `dl-translate-0.2.6/dl_translate/lang/mbart50.py` & `dl-translate-0.3.0/dl_translate/lang/mbart50.py`

 * *Files identical despite different names*

### Comparing `dl-translate-0.2.6/dl_translate.egg-info/PKG-INFO` & `dl-translate-0.3.0/dl_translate.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,247 +1,267 @@
 Metadata-Version: 2.1
 Name: dl-translate
-Version: 0.2.6
+Version: 0.3.0
 Summary: A deep learning-based translation library built on Huggingface transformers
 Home-page: https://github.com/xhlulu/dl-translate
 Author: Xing Han Lu
 Author-email: github@xinghanlu.com
 License: UNKNOWN
+Description: # DL Translate
+        
+        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5230676.svg)](https://doi.org/10.5281/zenodo.5230676)
+        [![Downloads](https://static.pepy.tech/personalized-badge/dl-translate?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/dl-translate)
+        [![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/xhluca/dl-translate/blob/main/LICENSE)
+        
+        
+        *A deep learning-based translation library built on Huggingface `transformers`*
+        
+        💻 [GitHub Repository](https://github.com/xhluca/dl-translate)<br>
+        📚 [Documentation](https://xhluca.github.io/dl-translate)<br>
+        🐍 [PyPi project](https://pypi.org/project/dl-translate/)<br>
+        🧪 [Colab Demo](https://colab.research.google.com/github/xhluca/dl-translate/blob/main/demos/colab_demo.ipynb) / [Kaggle Demo](https://www.kaggle.com/xhlulu/dl-translate-demo/)
+        
+        
+        
+        ## Quickstart
+        
+        Install the library with pip:
+        ```
+        pip install dl-translate
+        ```
+        
+        To translate some text:
+        
+        ```python
+        import dl_translate as dlt
+        
+        mt = dlt.TranslationModel()  # Slow when you load it for the first time
+        
+        text_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
+        mt.translate(text_hi, source=dlt.lang.HINDI, target=dlt.lang.ENGLISH)
+        ```
+        
+        Above, you can see that `dlt.lang` contains variables representing each of the 50 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
+        ```python
+        text_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
+        mt.translate(text_ar, source="Arabic", target="fr")
+        ```
+        
+        If you want to verify whether a language is available, you can check it:
+        ```python
+        print(mt.available_languages())  # All languages that you can use
+        print(mt.available_codes())  # Code corresponding to each language accepted
+        print(mt.get_lang_code_map())  # Dictionary of lang -> code
+        ```
+        
+        ## Usage
+        
+        ### Selecting a device
+        
+        When you load the model, you can specify the device:
+        ```python
+        mt = dlt.TranslationModel(device="auto")
+        ```
+        
+        By default, the value will be `device="auto"`, which means it will use a GPU if possible. You can also explicitly set `device="cpu"` or `device="gpu"`, or some other strings accepted by [`torch.device()`](https://pytorch.org/docs/stable/tensor_attributes.html#torch.torch.device). __In general, it is recommend to use a GPU if you want a reasonable processing time.__
+        
+        ### Choosing a different model
+        
+        By default, the `m2m100` model will be used. However, there are a few options:
+        
+        * [mBART-50 Large](https://huggingface.co/transformers/master/model_doc/mbart.html):  Allows translations across 50 languages.
+        * [m2m100](https://huggingface.co/transformers/model_doc/m2m_100.html): Allows translations across 100 languages.
+        * [nllb-200](https://huggingface.co/docs/transformers/model_doc/nllb) (New in v0.3): Allows translations across 200 languages, and is faster than m2m100 (On RTX A6000, we can see speed up of 3x).
+        
+        Here's an example:
+        ```python
+        # The default approval
+        mt = dlt.TranslationModel("m2m100")  # Shorthand
+        mt = dlt.TranslationModel("facebook/m2m100_418M")  # Huggingface repo
+        
+        # If you want to use mBART-50 Large
+        mt = dlt.TranslationModel("mbart50")
+        mt = dlt.TranslationModel("facebook/mbart-large-50-many-to-many-mmt")
+        
+        # Or NLLB-200 (faster and has 200 languages)
+        mt = dlt.TranslationModel("nllb200")
+        mt = dlt.TranslationModel("facebook/nllb-200-distilled-600M")
+        ```
+        
+        Note that the language code will change depending on the model family. To find out the correct language codes, please read the doc page on available languages or run `mt.available_codes()`.
+        
+        By default, `dlt.TranslationModel` will download the model from the huggingface repo for [mbart50](https://huggingface.co/facebook/mbart-large-50-one-to-many-mmt), [m2m100](https://huggingface.co/facebook/m2m100_418M), or [nllb200](https://huggingface.co/facebook/nllb-200-distilled-600M) and cache it. It's possible to load the model from a path or a model with a similar format, but you will need to specify the `model_family`:
+        ```python
+        mt = dlt.TranslationModel("/path/to/model/directory/", model_family="mbart50")
+        mt = dlt.TranslationModel("facebook/m2m100_1.2B", model_family="m2m100")
+        mt = dlt.TranslationModel("facebook/nllb-200-distilled-600M", model_family="nllb200")
+        ```
+        
+        Notes:
+        * Make sure your tokenizer is also stored in the same directory if you load from a file. 
+        * The available languages will change if you select a different model, so you will not be able to leverage `dlt.lang` or `dlt.utils`.
+        
+        ### Splitting into sentences
+        
+        It is not recommended to use extremely long texts as it takes more time to process. Instead, you can try to break them down into sentences with the help of `nltk`. First install the library with `pip install nltk`, then run:
+        ```python
+        import nltk
+        
+        nltk.download("punkt")
+        
+        text = "Mr. Smith went to his favorite cafe. There, he met his friend Dr. Doe."
+        sents = nltk.tokenize.sent_tokenize(text, "english")  # don't use dlt.lang.ENGLISH
+        " ".join(mt.translate(sents, source=dlt.lang.ENGLISH, target=dlt.lang.FRENCH))
+        ```
+        
+        ### Batch size during translation
+        
+        It's possible to set a batch size (i.e. the number of elements processed at once) for `mt.translate` and whether you want to see the progress bar or not:
+        
+        ```python
+        # ...
+        mt = dlt.TranslationModel()
+        mt.translate(text, source, target, batch_size=32, verbose=True)
+        ```
+        
+        If you set `batch_size=None`, it will compute the entire `text` at once rather than splitting into "chunks". We recommend lowering `batch_size` if you do not have a lot of RAM or VRAM and run into CUDA memory error. Set a higher value if you are using a high-end GPU and the VRAM is not fully utilized.
+        
+        
+        ### `dlt.utils` module
+        
+        An alternative to `mt.available_languages()` is the `dlt.utils` module. You can use it to find out which languages and codes are available:
+        
+        ```python
+        print(dlt.utils.available_languages('mbart50'))  # All languages that you can use
+        print(dlt.utils.available_codes('m2m100'))  # Code corresponding to each language accepted
+        print(dlt.utils.get_lang_code_map('nllb200'))  # Dictionary of lang -> code
+        ```
+        
+        ### Offline usage
+        
+        Unlike the Google translate or MSFT Translator APIs, this library can be fully used offline. However, you will need to first download the packages and models, and move them to your offline environment to be installed and loaded inside a venv.
+        
+        First, run in your terminal:
+        ```bash
+        mkdir dlt
+        cd dlt
+        mkdir libraries
+        pip download -d libraries/ dl-translate
+        ```
+        
+        Once all the required packages are downloaded, you will need to use huggingface hub to download the files. Install it with `pip install huggingface-hub`. Then, run inside Python:
+        ```python
+        import shutil
+        import huggingface_hub as hub
+        
+        dirname = hub.snapshot_download("facebook/m2m100_418M")
+        shutil.copytree(dirname, "cached_model_m2m100")  # Copy to a permanent folder
+        ```
+        
+        Now, move everything in the `dlt` directory to your offline environment. Create a virtual environment and run the following in terminal:
+        ```bash
+        pip install --no-index --find-links libraries/ dl-translate
+        ```
+        
+        Now, run inside Python:
+        ```python
+        import dl_translate as dlt
+        
+        mt = dlt.TranslationModel("cached_model_m2m100", model_family="m2m100")
+        ```
+        
+        
+        ## Advanced
+        
+        If you have knowledge of PyTorch and Huggingface Transformers, you can access advanced aspects of the library for more customization:
+        * **Saving and loading**: If you wish to accelerate the loading time the translation model, you can use `save_obj` and reload it later with `load_obj`. This method is only recommended if you are familiar with `huggingface` and `torch`; please read the docs for more information.
+        * **Interacting with underlying model and tokenizer**: When initializing `model`, you can pass in arguments for the underlying BART model and tokenizer with `model_options` and `tokenizer_options` respectively. You can also access the underlying `transformers` with `mt.get_transformers_model()`.
+        * **Keyword arguments for the `generate()` method**: When running `mt.translate`, you can also give `generation_options` that is passed to the `generate()` method of the underlying transformer model.
+        
+        For more information, please visit the [advanced section of the user guide](https://xhluca.github.io/dl-translate/#advanced).
+        
+        ## Acknowledgement
+        
+        `dl-translate` is built on top of Huggingface's implementation of two models created by Facebook AI Research.
+        
+        1. The multilingual BART finetuned on many-to-many translation of over 50 languages, which is [documented here](https://huggingface.co/transformers/master/model_doc/mbart.html) The original paper was written by Tang et. al from Facebook AI Research; you can [find it here](https://arxiv.org/pdf/2008.00401.pdf) and cite it using the following:
+            ```
+            @article{tang2020multilingual,
+                title={Multilingual translation with extensible multilingual pretraining and finetuning},
+                author={Tang, Yuqing and Tran, Chau and Li, Xian and Chen, Peng-Jen and Goyal, Naman and Chaudhary, Vishrav and Gu, Jiatao and Fan, Angela},
+                journal={arXiv preprint arXiv:2008.00401},
+                year={2020}
+            }
+            ```
+        2. The transformer model published in [Beyond English-Centric Multilingual Machine Translation](https://arxiv.org/abs/2010.11125) by Fan et. al, which supports over 100 languages. You can cite it here:
+           ```
+           @misc{fan2020englishcentric,
+                title={Beyond English-Centric Multilingual Machine Translation}, 
+                author={Angela Fan and Shruti Bhosale and Holger Schwenk and Zhiyi Ma and Ahmed El-Kishky and Siddharth Goyal and Mandeep Baines and Onur Celebi and Guillaume Wenzek and Vishrav Chaudhary and Naman Goyal and Tom Birch and Vitaliy Liptchinsky and Sergey Edunov and Edouard Grave and Michael Auli and Armand Joulin},
+                year={2020},
+                eprint={2010.11125},
+                archivePrefix={arXiv},
+                primaryClass={cs.CL}
+            }
+           ```
+        
+        3. The [no language left behind](https://arxiv.org/abs/2207.04672) model, which extends NMT to 200+ languages. You can cite it here:
+            ```
+            @misc{nllbteam2022language,
+                title={No Language Left Behind: Scaling Human-Centered Machine Translation}, 
+                author={NLLB Team and Marta R. Costa-jussà and James Cross and Onur Çelebi and Maha Elbayad and Kenneth Heafield and Kevin Heffernan and Elahe Kalbassi and Janice Lam and Daniel Licht and Jean Maillard and Anna Sun and Skyler Wang and Guillaume Wenzek and Al Youngblood and Bapi Akula and Loic Barrault and Gabriel Mejia Gonzalez and Prangthip Hansanti and John Hoffman and Semarley Jarrett and Kaushik Ram Sadagopan and Dirk Rowe and Shannon Spruit and Chau Tran and Pierre Andrews and Necip Fazil Ayan and Shruti Bhosale and Sergey Edunov and Angela Fan and Cynthia Gao and Vedanuj Goswami and Francisco Guzmán and Philipp Koehn and Alexandre Mourachko and Christophe Ropers and Safiyyah Saleem and Holger Schwenk and Jeff Wang},
+                year={2022},
+                eprint={2207.04672},
+                archivePrefix={arXiv},
+                primaryClass={cs.CL}
+            }
+            ```
+        
+        
+        `dlt` is a wrapper with useful `utils` to save you time. For huggingface's `transformers`, the following snippet is shown as an example:
+        ```python
+        from transformers import MBartForConditionalGeneration, MBart50TokenizerFast
+        
+        article_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
+        article_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
+        
+        model = MBartForConditionalGeneration.from_pretrained("facebook/mbart-large-50-many-to-many-mmt")
+        tokenizer = MBart50TokenizerFast.from_pretrained("facebook/mbart-large-50-many-to-many-mmt")
+        
+        # translate Hindi to French
+        tokenizer.src_lang = "hi_IN"
+        encoded_hi = tokenizer(article_hi, return_tensors="pt")
+        generated_tokens = model.generate(**encoded_hi, forced_bos_token_id=tokenizer.lang_code_to_id["fr_XX"])
+        tokenizer.batch_decode(generated_tokens, skip_special_tokens=True)
+        # => "Le chef de l 'ONU affirme qu 'il n 'y a pas de solution militaire en Syria."
+        
+        # translate Arabic to English
+        tokenizer.src_lang = "ar_AR"
+        encoded_ar = tokenizer(article_ar, return_tensors="pt")
+        generated_tokens = model.generate(**encoded_ar, forced_bos_token_id=tokenizer.lang_code_to_id["en_XX"])
+        tokenizer.batch_decode(generated_tokens, skip_special_tokens=True)
+        # => "The Secretary-General of the United Nations says there is no military solution in Syria."
+        ```
+        
+        With `dlt`, you can run:
+        ```python
+        import dl_translate as dlt
+        
+        article_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
+        article_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
+        
+        mt = dlt.TranslationModel()
+        translated_fr = mt.translate(article_hi, source=dlt.lang.HINDI, target=dlt.lang.FRENCH)
+        translated_en = mt.translate(article_ar, source=dlt.lang.ARABIC, target=dlt.lang.ENGLISH)
+        ```
+        
+        Notice you don't have to think about tokenizers, condition generation, pretrained models, and regional codes; you can just tell the model what to translate!
+        
+        If you are experienced with `huggingface`'s ecosystem, then you should be familiar enough with the example above that you wouldn't need this library. However, if you've never heard of huggingface or mBART, then I hope using this library will give you enough motivation to [learn more about them](https://github.com/huggingface/transformers) :)
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
-
-# DL Translate
-
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5230676.svg)](https://doi.org/10.5281/zenodo.5230676)
-[![Downloads](https://static.pepy.tech/personalized-badge/dl-translate?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/dl-translate)
-[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/xhluca/dl-translate/blob/main/LICENSE)
-
-
-*A deep learning-based translation library built on Huggingface `transformers`*
-
-💻 [GitHub Repository](https://github.com/xhluca/dl-translate)<br>
-📚 [Documentation](https://xhluca.github.io/dl-translate) / [Readthedocs](https://dl-translate.readthedocs.io)<br>
-🐍 [PyPi project](https://pypi.org/project/dl-translate/)<br>
-🧪 [Colab Demo](https://colab.research.google.com/github/xhluca/dl-translate/blob/main/demos/colab_demo.ipynb) / [Kaggle Demo](https://www.kaggle.com/xhlulu/dl-translate-demo/)
-
-
-
-## Quickstart
-
-Install the library with pip:
-```
-pip install dl-translate
-```
-
-To translate some text:
-
-```python
-import dl_translate as dlt
-
-mt = dlt.TranslationModel()  # Slow when you load it for the first time
-
-text_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
-mt.translate(text_hi, source=dlt.lang.HINDI, target=dlt.lang.ENGLISH)
-```
-
-Above, you can see that `dlt.lang` contains variables representing each of the 50 available languages with auto-complete support. Alternatively, you can specify the language (e.g. "Arabic") or the language code (e.g. "fr" for French):
-```python
-text_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
-mt.translate(text_ar, source="Arabic", target="fr")
-```
-
-If you want to verify whether a language is available, you can check it:
-```python
-print(mt.available_languages())  # All languages that you can use
-print(mt.available_codes())  # Code corresponding to each language accepted
-print(mt.get_lang_code_map())  # Dictionary of lang -> code
-```
-
-## Usage
-
-### Selecting a device
-
-When you load the model, you can specify the device:
-```python
-mt = dlt.TranslationModel(device="auto")
-```
-
-By default, the value will be `device="auto"`, which means it will use a GPU if possible. You can also explicitly set `device="cpu"` or `device="gpu"`, or some other strings accepted by [`torch.device()`](https://pytorch.org/docs/stable/tensor_attributes.html#torch.torch.device). __In general, it is recommend to use a GPU if you want a reasonable processing time.__
-
-### Choosing a different model
-
-Two model families are available at the moment: [m2m100](https://huggingface.co/transformers/model_doc/m2m_100.html) and [mBART-50 Large](https://huggingface.co/transformers/master/model_doc/mbart.html), which respective allow translation across over 100 languages and 50 languages. By default, the model will select `m2m100`, but you can also explicitly choose the model by specifying the shorthand (`"m2m100"` or `"mbart50"`) or the full repository name (e.g. `"facebook/m2m100_418M"`). For example:
-
-```python
-# The following ways are equivalent
-mt = dlt.TranslationModel("m2m100")  # Default
-mt = dlt.TranslationModel("facebook/m2m100_418M")
-
-# The following ways are equivalent
-mt = dlt.TranslationModel("mbart50")
-mt = dlt.TranslationModel("facebook/mbart-large-50-many-to-many-mmt")
-```
-
-Note that the language code will change depending on the model family. To find out the correct language codes, please read the doc page on available languages or run `mt.available_codes()`.
-
-By default, `dlt.TranslationModel` will download the model from the huggingface repo for [mbart50](https://huggingface.co/facebook/mbart-large-50-one-to-many-mmt) or [m2m100](https://huggingface.co/facebook/m2m100_418M) and cache it. It's possible to load the model from a path or a model with a similar format, but you will need to specify the `model_family`:
-```python
-mt = dlt.TranslationModel("/path/to/model/directory/", model_family="mbart50")
-mt = dlt.TranslationModel("facebook/m2m100_1.2B", model_family="m2m100")
-```
-
-Notes:
-* Make sure your tokenizer is also stored in the same directory if you load from a file. 
-* The available languages will change if you select a different model, so you will not be able to leverage `dlt.lang` or `dlt.utils`.
-
-### Splitting into sentences
-
-It is not recommended to use extremely long texts as it takes more time to process. Instead, you can try to break them down into sentences with the help of `nltk`. First install the library with `pip install nltk`, then run:
-```python
-import nltk
-
-nltk.download("punkt")
-
-text = "Mr. Smith went to his favorite cafe. There, he met his friend Dr. Doe."
-sents = nltk.tokenize.sent_tokenize(text, "english")  # don't use dlt.lang.ENGLISH
-" ".join(mt.translate(sents, source=dlt.lang.ENGLISH, target=dlt.lang.FRENCH))
-```
-
-### Batch size during translation
-
-It's possible to set a batch size (i.e. the number of elements processed at once) for `mt.translate` and whether you want to see the progress bar or not:
-
-```python
-# ...
-mt = dlt.TranslationModel()
-mt.translate(text, source, target, batch_size=32, verbose=True)
-```
-
-If you set `batch_size=None`, it will compute the entire `text` at once rather than splitting into "chunks". We recommend lowering `batch_size` if you do not have a lot of RAM or VRAM and run into CUDA memory error. Set a higher value if you are using a high-end GPU and the VRAM is not fully utilized.
-
-
-### `dlt.utils` module
-
-An alternative to `mt.available_languages()` is the `dlt.utils` module. You can use it to find out which languages and codes are available:
-
-```python
-print(dlt.utils.available_languages('mbart50'))  # All languages that you can use
-print(dlt.utils.available_codes('mbart50'))  # Code corresponding to each language accepted
-print(dlt.utils.get_lang_code_map('mbart50'))  # Dictionary of lang -> code
-```
-
-### Offline usage
-
-Unlike the Google translate or MSFT Translator APIs, this library can be fully used offline. However, you will need to first download the packages and models, and move them to your offline environment to be installed and loaded inside a venv.
-
-First, run in your terminal:
-```bash
-mkdir dlt
-cd dlt
-mkdir libraries
-pip download -d libraries/ dl-translate
-```
-
-Once all the required packages are downloaded, you will need to use huggingface hub to download the files. Install it with `pip install huggingface-hub`. Then, run inside Python:
-```python
-import os
-import huggingface_hub as hub
-
-dirname = hub.snapshot_download("facebook/m2m100_418M")
-os.rename(dirname, "cached_model_m2m100")
-```
-
-Now, move everything in the `dlt` directory to your offline environment. Create a virtual environment and run the following in terminal:
-```bash
-pip install --no-index --find-links libraries/ dl-translate
-```
-
-Now, run inside Python:
-```python
-import dl_translate as dlt
-
-mt = dlt.TranslationModel("cached_model_m2m100", model_family="m2m100")
-```
-
-
-## Advanced
-
-If you have knowledge of PyTorch and Huggingface Transformers, you can access advanced aspects of the library for more customization:
-* **Saving and loading**: If you wish to accelerate the loading time the translation model, you can use `save_obj` and reload it later with `load_obj`. This method is only recommended if you are familiar with `huggingface` and `torch`; please read the docs for more information.
-* **Interacting with underlying model and tokenizer**: When initializing `model`, you can pass in arguments for the underlying BART model and tokenizer with `model_options` and `tokenizer_options` respectively. You can also access the underlying `transformers` with `mt.get_transformers_model()`.
-* **Keyword arguments for the `generate()` method**: When running `mt.translate`, you can also give `generation_options` that is passed to the `generate()` method of the underlying transformer model.
-
-For more information, please visit the [advanced section of the user guide](https://xhluca.github.io/dl-translate/#advanced) (also available in the [readthedocs version](https://dl-translate.readthedocs.io/en/latest/#advanced)).
-
-## Acknowledgement
-
-`dl-translate` is built on top of Huggingface's implementation of two models created by Facebook AI Research.
-
-1. The multilingual BART finetuned on many-to-many translation of over 50 languages, which is [documented here](https://huggingface.co/transformers/master/model_doc/mbart.html) The original paper was written by Tang et. al from Facebook AI Research; you can [find it here](https://arxiv.org/pdf/2008.00401.pdf) and cite it using the following:
-    ```
-    @article{tang2020multilingual,
-        title={Multilingual translation with extensible multilingual pretraining and finetuning},
-        author={Tang, Yuqing and Tran, Chau and Li, Xian and Chen, Peng-Jen and Goyal, Naman and Chaudhary, Vishrav and Gu, Jiatao and Fan, Angela},
-        journal={arXiv preprint arXiv:2008.00401},
-        year={2020}
-    }
-    ```
-2. The transformer model published in [Beyond English-Centric Multilingual Machine Translation](https://arxiv.org/abs/2010.11125) by Fan et. al, which supports over 100 languages. You can cite it here:
-   ```
-   @misc{fan2020englishcentric,
-        title={Beyond English-Centric Multilingual Machine Translation}, 
-        author={Angela Fan and Shruti Bhosale and Holger Schwenk and Zhiyi Ma and Ahmed El-Kishky and Siddharth Goyal and Mandeep Baines and Onur Celebi and Guillaume Wenzek and Vishrav Chaudhary and Naman Goyal and Tom Birch and Vitaliy Liptchinsky and Sergey Edunov and Edouard Grave and Michael Auli and Armand Joulin},
-        year={2020},
-        eprint={2010.11125},
-        archivePrefix={arXiv},
-        primaryClass={cs.CL}
-    }
-   ```
-
-`dlt` is a wrapper with useful `utils` to save you time. For huggingface's `transformers`, the following snippet is shown as an example:
-```python
-from transformers import MBartForConditionalGeneration, MBart50TokenizerFast
-
-article_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
-article_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
-
-model = MBartForConditionalGeneration.from_pretrained("facebook/mbart-large-50-many-to-many-mmt")
-tokenizer = MBart50TokenizerFast.from_pretrained("facebook/mbart-large-50-many-to-many-mmt")
-
-# translate Hindi to French
-tokenizer.src_lang = "hi_IN"
-encoded_hi = tokenizer(article_hi, return_tensors="pt")
-generated_tokens = model.generate(**encoded_hi, forced_bos_token_id=tokenizer.lang_code_to_id["fr_XX"])
-tokenizer.batch_decode(generated_tokens, skip_special_tokens=True)
-# => "Le chef de l 'ONU affirme qu 'il n 'y a pas de solution militaire en Syria."
-
-# translate Arabic to English
-tokenizer.src_lang = "ar_AR"
-encoded_ar = tokenizer(article_ar, return_tensors="pt")
-generated_tokens = model.generate(**encoded_ar, forced_bos_token_id=tokenizer.lang_code_to_id["en_XX"])
-tokenizer.batch_decode(generated_tokens, skip_special_tokens=True)
-# => "The Secretary-General of the United Nations says there is no military solution in Syria."
-```
-
-With `dlt`, you can run:
-```python
-import dl_translate as dlt
-
-article_hi = "संयुक्त राष्ट्र के प्रमुख का कहना है कि सीरिया में कोई सैन्य समाधान नहीं है"
-article_ar = "الأمين العام للأمم المتحدة يقول إنه لا يوجد حل عسكري في سوريا."
-
-mt = dlt.TranslationModel()
-translated_fr = mt.translate(article_hi, source=dlt.lang.HINDI, target=dlt.lang.FRENCH)
-translated_en = mt.translate(article_ar, source=dlt.lang.ARABIC, target=dlt.lang.ENGLISH)
-```
-
-Notice you don't have to think about tokenizers, condition generation, pretrained models, and regional codes; you can just tell the model what to translate!
-
-If you are experienced with `huggingface`'s ecosystem, then you should be familiar enough with the example above that you wouldn't need this library. However, if you've never heard of huggingface or mBART, then I hope using this library will give you enough motivation to [learn more about them](https://github.com/huggingface/transformers) :)
-
-
```

### Comparing `dl-translate-0.2.6/setup.py` & `dl-translate-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dl-translate",
-    version="0.2.6",
+    version="0.3.0",
     author="Xing Han Lu",
     author_email="github@xinghanlu.com",
     description="A deep learning-based translation library built on Huggingface transformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xhlulu/dl-translate",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=[
-        "transformers>=4.4.0",
-        "torch",
+        "transformers>=4.30.2",
+        "torch>=2.0.0",
         "sentencepiece",
         "protobuf",
         "tqdm",
     ],
     extras_require={"dev": ["pytest", "black", "jinja2", "mkdocs", "mkdocs-material"]},
 )
```

