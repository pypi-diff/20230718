# Comparing `tmp/ag_llama_hub-0.0.8.tar.gz` & `tmp/ag_llama_hub-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_hub-0.0.8.tar", last modified: Mon Jul 17 13:33:58 2023, max compression
+gzip compressed data, was "dist\ag_llama_hub-0.0.9.tar", last modified: Tue Jul 18 13:52:23 2023, max compression
```

## Comparing `ag_llama_hub-0.0.8.tar` & `ag_llama_hub-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 13:33:58.163577 ag_llama_hub-0.0.8/
--rw-rw-rw-   0        0        0      832 2023-07-17 13:33:58.162581 ag_llama_hub-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 13:33:58.149615 ag_llama_hub-0.0.8/ag_llama_hub/
--rw-rw-rw-   0        0        0     2105 2023-07-12 14:53:21.000000 ag_llama_hub-0.0.8/ag_llama_hub/__init__.py
--rw-rw-rw-   0        0        0     4794 2023-07-17 11:48:25.000000 ag_llama_hub-0.0.8/ag_llama_hub/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.8/ag_llama_hub/choice.py
--rw-rw-rw-   0        0        0    16470 2023-07-17 13:33:49.000000 ag_llama_hub-0.0.8/ag_llama_hub/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.8/ag_llama_hub/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:33:58.158592 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/
--rw-rw-rw-   0        0        0      832 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-17 13:33:58.000000 ag_llama_hub-0.0.8/ag_llama_hub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 13:33:58.164576 ag_llama_hub-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2567 2023-07-12 13:13:29.000000 ag_llama_hub-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 13:33:58.161584 ag_llama_hub-0.0.8/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.8/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.8/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:52:23.771278 ag_llama_hub-0.0.9/
+-rw-rw-rw-   0        0        0      832 2023-07-18 13:52:23.770282 ag_llama_hub-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 13:52:23.757315 ag_llama_hub-0.0.9/ag_llama_hub/
+-rw-rw-rw-   0        0        0     2105 2023-07-12 14:53:21.000000 ag_llama_hub-0.0.9/ag_llama_hub/__init__.py
+-rw-rw-rw-   0        0        0     4794 2023-07-17 11:48:25.000000 ag_llama_hub-0.0.9/ag_llama_hub/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.9/ag_llama_hub/choice.py
+-rw-rw-rw-   0        0        0    16533 2023-07-18 13:52:19.000000 ag_llama_hub-0.0.9/ag_llama_hub/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.9/ag_llama_hub/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:52:23.766291 ag_llama_hub-0.0.9/ag_llama_hub.egg-info/
+-rw-rw-rw-   0        0        0      832 2023-07-18 13:52:23.000000 ag_llama_hub-0.0.9/ag_llama_hub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-18 13:52:23.000000 ag_llama_hub-0.0.9/ag_llama_hub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:52:23.000000 ag_llama_hub-0.0.9/ag_llama_hub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-07-18 13:52:23.000000 ag_llama_hub-0.0.9/ag_llama_hub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-18 13:52:23.000000 ag_llama_hub-0.0.9/ag_llama_hub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:52:23.772276 ag_llama_hub-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2567 2023-07-12 13:13:29.000000 ag_llama_hub-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:52:23.769284 ag_llama_hub-0.0.9/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.9/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_hub-0.0.9/utils/render.py
```

### Comparing `ag_llama_hub-0.0.8/PKG-INFO` & `ag_llama_hub-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_hub
-Version: 0.0.8
+Version: 0.0.9
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub-0.0.8/ag_llama_hub/__init__.py` & `ag_llama_hub-0.0.9/ag_llama_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.8/ag_llama_hub/__main__.py` & `ag_llama_hub-0.0.9/ag_llama_hub/__main__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.8/ag_llama_hub/choice.py` & `ag_llama_hub-0.0.9/ag_llama_hub/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.8/ag_llama_hub/model.py` & `ag_llama_hub-0.0.9/ag_llama_hub/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A text generation model with stream decoding.
 """
+import os
 import gc
 import copy
 import pynvml
 import torch
 from sentencepiece import SentencePieceProcessor
 from transformers import (
     AutoModelForCausalLM,
@@ -385,14 +386,15 @@
     load_in_8bit=False,
     load_in_4bit=False,
     local_files_only=False,
     trust_remote_code=False,
     half_precision=False,
 ):
     """Load a text generation model and make it stream-able."""
+    logger.info(f"Working directory: {os.getcwd()}")
     logger.info(f"Loading tokenizer from {name_or_path}")
     kwargs = {
         "local_files_only": local_files_only,
         "trust_remote_code": trust_remote_code,
     }
     if revision:
         kwargs["revision"] = revision
```

### Comparing `ag_llama_hub-0.0.8/ag_llama_hub/tokenizer.py` & `ag_llama_hub-0.0.9/ag_llama_hub/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.8/ag_llama_hub.egg-info/PKG-INFO` & `ag_llama_hub-0.0.9/ag_llama_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-hub
-Version: 0.0.8
+Version: 0.0.9
 Summary: ag_llama_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama_hub-0.0.8/setup.py` & `ag_llama_hub-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.8/utils/download.py` & `ag_llama_hub-0.0.9/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_hub-0.0.8/utils/render.py` & `ag_llama_hub-0.0.9/utils/render.py`

 * *Files identical despite different names*

