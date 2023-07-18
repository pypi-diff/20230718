# Comparing `tmp/easylaser-0.1.2.tar.gz` & `tmp/easylaser-0.1.3.tar.gz`

## Comparing `easylaser-0.1.2.tar` & `easylaser-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 easylaser-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/__init__.py
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/align.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/get_model.py
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/laser.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/embed.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/encoder.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/laserLstmEncoder.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/laserTransformerEncoder.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/embed/multiGpuEncoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/lib/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/lib/constants.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 easylaser-0.1.2/easylaser/lib/text_processing.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 easylaser-0.1.2/test/fake_data.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 easylaser-0.1.2/test/test_laser.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 easylaser-0.1.2/.gitignore
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 easylaser-0.1.2/LICENSE
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 easylaser-0.1.2/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 easylaser-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 easylaser-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 easylaser-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/__init__.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/align.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/get_model.py
+-rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/laser.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/embed.py
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/encoder.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/laserLstmEncoder.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/laserTransformerEncoder.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/embed/multiGpuEncoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/lib/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/lib/constants.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 easylaser-0.1.3/easylaser/lib/text_processing.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 easylaser-0.1.3/test/fake_data.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 easylaser-0.1.3/test/test_laser.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 easylaser-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 easylaser-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 easylaser-0.1.3/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 easylaser-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 easylaser-0.1.3/PKG-INFO
```

### Comparing `easylaser-0.1.2/easylaser/align.py` & `easylaser-0.1.3/easylaser/align.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/easylaser/get_model.py` & `easylaser-0.1.3/easylaser/get_model.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/easylaser/laser.py` & `easylaser-0.1.3/easylaser/laser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import torch
+import sentencepiece as spm
 
 from .align import get_best_neighbors, match_sentences_with_best_neighbors
 from .embed.embed import embed_sentences
 from .embed.encoder import load_model
 from .embed.multiGpuEncoder import MultiGpuEncoder
 from .get_model import load_or_download_file
 from .lib.constants import langs_with_specific_vocab, laser3_langs
@@ -39,23 +40,25 @@
     :param verbose: if True, will print some information about the embedding process
     """
 
     def __init__(
         self,
         lang: str = None,
         device: list[str] | str = None,
+        batch_size: int = 32,
         verbose=False,
     ):
         if device is None:
             if torch.cuda.is_available():
                 device = "cuda"
             else:
                 device = "cpu"
         self.set_lang(lang=lang)
         self.device = device
+        self.batch_size = batch_size
         self.verbose = verbose
         self.encoder = None
 
     def __enter__(self):
         self.start_encoder()
         return self
 
@@ -70,34 +73,34 @@
 
     def is_encoder_active(self):
         try:
             return not self.encoder is None
         except AttributeError:
             return False
 
-    def start_encoder(self, device: list[str] | str = None):
+    def start_encoder(self, device: list[str] | str = None, batch_size: int = None):
         """
         Start the encoder, you can overwrite the target_device and cpu parameters, else it will use the one specified at init
         :param target_device: ids of a GPU to use for embedding, if None, will use the first GPU available. If you want to use multiple GPUs, use launchMultiGpuEncoder
         :param cpu: if True, will use CPU for embedding and ignore target_devices
         """
         if device is not None:
             self.device = device
+        if batch_size is not None:
+            self.batch_size = batch_size
 
         multi_gpu = True if isinstance(self.device, list) else False
         self.encoder = self._load_encoder()
         if multi_gpu:
             self.encoder = MultiGpuEncoder(self.device, self.encoder)
         else:
             self.encoder._choose_encoder_device(device=self.device)
 
     def _load_encoder(
         self,
-        max_sentences=10000,
-        max_tokens=12000,
     ):
         version = 0
         if self.lang:
             version = 1
             pt = load_or_download_file(f"laser3-{self.lang}.v{version}.pt")
         else:
             pt = load_or_download_file("laser2.pt")
@@ -105,20 +108,20 @@
             self.spm = load_or_download_file(
                 f"laser3-{self.lang}.v{version}.spm"
             ).as_posix()
             load_or_download_file(f"laser3-{self.lang}.v{version}.cvocab")
         else:
             self.spm = str(load_or_download_file("laser2.spm").as_posix())
             load_or_download_file("laser2.cvocab")
+        self.sp = spm.SentencePieceProcessor(model_file=self.spm)
         encoder = load_model(
             encoder_path=str(pt),
             spm_model=self.spm,
             verbose=self.verbose,
-            max_sentences=max_sentences,
-            max_tokens=max_tokens,
+            max_sentences=self.batch_size,
         )
         return encoder
 
     def set_verbose(self, verbose: bool):
         self.verbose = verbose
 
     def set_lang(self, lang: str):
```

### Comparing `easylaser-0.1.2/easylaser/embed/embed.py` & `easylaser-0.1.3/easylaser/embed/embed.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,16 +77,15 @@
     return E
 
 
 def embed_sentences(
     sentences: list[str],
     encoder: MultiGpuEncoder | SentenceEncoder = None,
     encoder_path: Path = None,
-    spm_lang: Optional[str] = "en",
-    spm_model: Path = None,
+    sp = None,
     verbose: bool = False,
     buffer_size: int = 10000,
     max_sentences: Optional[int] = None,
     fp16: bool = False,
 ):
     if verbose:
         logging.getLogger().setLevel(logging.INFO)
@@ -94,11 +93,11 @@
         logging.getLogger().setLevel(logging.ERROR)
     assert encoder or encoder_path, "Provide initialised encoder or encoder_path"
     buffer_size = max(buffer_size, 1)
     assert (
         not max_sentences or max_sentences <= buffer_size
     ), "--max-sentences/--batch-size cannot be larger than --buffer-size"
     tSMP = time.time()
-    sentences = SPMApply(sentences, spm_model, spm_lang)
+    sentences = SPMApply(sentences, sp)
     if verbose:
         logger.info(f" - Preprocessing finished at {time.time() - tSMP}")
     return EncodeText(encoder, sentences, fp16=fp16, verbose=verbose)
```

### Comparing `easylaser-0.1.2/easylaser/embed/encoder.py` & `easylaser-0.1.3/easylaser/embed/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         verbose=False,
         sort_kind="quicksort",
     ):
         self.verbose = verbose
         if self.verbose:
             logger.info(f"loading encoder: {model_path}")
         self.max_sentences = max_sentences
+        logger.info("max_sentences: %s", self.max_sentences)
         self.max_tokens = max_tokens
         if self.max_tokens is None and self.max_sentences is None:
             self.max_sentences = 1
         state_dict = torch.load(model_path)
         if "params" in state_dict:
             self.encoder = LaserLstmEncoder(**state_dict["params"])
             self.encoder.load_state_dict(state_dict["model"])
```

### Comparing `easylaser-0.1.2/easylaser/embed/laserLstmEncoder.py` & `easylaser-0.1.3/easylaser/embed/laserLstmEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/easylaser/embed/laserTransformerEncoder.py` & `easylaser-0.1.3/easylaser/embed/laserTransformerEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/easylaser/embed/multiGpuEncoder.py` & `easylaser-0.1.3/easylaser/embed/multiGpuEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/easylaser/lib/constants.py` & `easylaser-0.1.3/easylaser/lib/constants.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/easylaser/lib/text_processing.py` & `easylaser-0.1.3/easylaser/lib/text_processing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import logging
 import sentencepiece as spm
 import ftfy
-from mosestokenizer import MosesPunctuationNormalizer
+#from mosestokenizer import MosesPunctuationNormalizer
 
 # from transliterate import translit
 import sys
 
 logging.basicConfig(
     stream=sys.stdout,
     level=logging.INFO,
     format="%(asctime)s | %(levelname)s | %(name)s | %(message)s",
 )
 logger = logging.getLogger("preprocess")
 
 
 def SPMApply(
     sentences,
-    spm_model,
+    sp,
     lang="en",
     lower_case=True,
     descape=False,
     verbose=False,
 ):
     assert lower_case, "lower case is needed by all the models"
     if verbose:
         logger.info("SPM processing")
-    mosesPunctuationNormalizer = MosesPunctuationNormalizer(lang)
+    #mosesPunctuationNormalizer = MosesPunctuationNormalizer(lang)
     sentences = [
-        mosesPunctuationNormalizer(ftfy.fix_text(s).lower()) for s in sentences
+        #mosesPunctuationNormalizer(ftfy.fix_text(s).lower()) for s in sentences
+        ftfy.fix_text(s).lower() for s in sentences
     ]
     # line = translit(line, language_code=, reversed=True)
-    sp = spm.SentencePieceProcessor(model_file=spm_model)
     # in 3.11 might need to do transformrf_sentences = [sp.EncodeAsPieces(sentence) for sentence in sentences]
     transformed_sentences = sp.EncodeAsPieces(sentences)
 
     return [" ".join([word for word in sentence]) for sentence in transformed_sentences]
```

### Comparing `easylaser-0.1.2/test/fake_data.py` & `easylaser-0.1.3/test/fake_data.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/test/test_laser.py` & `easylaser-0.1.3/test/test_laser.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/LICENSE` & `easylaser-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/README.md` & `easylaser-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.2/pyproject.toml` & `easylaser-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "easylaser"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Lingua Custodia", email="it@linguacustodia.com" },
 ]
 description = "An easy to use interface to LASER"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.10",
@@ -16,12 +16,12 @@
     "Development Status :: 4 - Beta",
 ]
 requires-python = ">=3.7"
 dependencies = [
   "sentencepiece",
   "requests",
   "ftfy",
-  "mosestokenizer",
+  #"mosestokenizer",
   "fairseq", # will install torch and numpy
   "faiss-cpu",
 ]
 [project.urls]
```

### Comparing `easylaser-0.1.2/PKG-INFO` & `easylaser-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: easylaser
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy to use interface to LASER
 Author-email: Lingua Custodia <it@linguacustodia.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Requires-Dist: fairseq
 Requires-Dist: faiss-cpu
 Requires-Dist: ftfy
-Requires-Dist: mosestokenizer
 Requires-Dist: requests
 Requires-Dist: sentencepiece
 Description-Content-Type: text/markdown
 
 # EasyLaser
 
 This package is created to use simply [LASER](https://github.com/facebookresearch/LASER) from MetaAI to create embeddings. It uses list of string as input and returns list of numpy arrays as output instead of using files. It also does not require external tools to be installed. The package automatically downloads the required laser models.
```

