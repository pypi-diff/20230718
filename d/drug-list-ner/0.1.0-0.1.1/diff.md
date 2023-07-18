# Comparing `tmp/drug_list_ner-0.1.0.tar.gz` & `tmp/drug_list_ner-0.1.1.tar.gz`

## Comparing `drug_list_ner-0.1.0.tar` & `drug_list_ner-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/.DS_Store
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/Pipfile
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/pyvenv.cfg
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/drug_list_ner/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/drug_list_ner/__init__.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/drug_list_ner/example.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/drug_list_ner/model2/.DS_Store
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/drug_list_ner/model2/config.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/drug_list_ner/tokenizer2/special_tokens_map.json
--rw-r--r--   0        0        0   716830 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/drug_list_ner/tokenizer2/tokenizer.json
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/drug_list_ner/tokenizer2/tokenizer_config.json
--rw-r--r--   0        0        0   227845 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/src/drug_list_ner/tokenizer2/vocab.txt
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/LICENSE
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/README.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 drug_list_ner-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/.DS_Store
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/Pipfile
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/Pipfile.lock
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/pyvenv.cfg
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/drug_list_ner/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/drug_list_ner/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/drug_list_ner/example.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/drug_list_ner/model2/.DS_Store
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/drug_list_ner/model2/config.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/drug_list_ner/tokenizer2/special_tokens_map.json
+-rw-r--r--   0        0        0   716830 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/drug_list_ner/tokenizer2/tokenizer.json
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/drug_list_ner/tokenizer2/tokenizer_config.json
+-rw-r--r--   0        0        0   227845 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/src/drug_list_ner/tokenizer2/vocab.txt
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/LICENSE
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/README.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 drug_list_ner-0.1.1/PKG-INFO
```

### Comparing `drug_list_ner-0.1.0/.DS_Store` & `drug_list_ner-0.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/Pipfile.lock` & `drug_list_ner-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/requirements.txt` & `drug_list_ner-0.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/src/.DS_Store` & `drug_list_ner-0.1.1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/src/drug_list_ner/.DS_Store` & `drug_list_ner-0.1.1/src/drug_list_ner/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/src/drug_list_ner/example.py` & `drug_list_ner-0.1.1/src/drug_list_ner/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def drug_search(sentence):
     if not os.path.exists(os.path.join(model_path, "pytorch_model.bin")):
         hf_hub_download(repo_id="ronoys/testDeploy", filename="pytorch_model.bin", local_dir = "./model2")
 
 
-    model = AutoModelForTokenClassification.from_pretrained("model2")
+    model = AutoModelForTokenClassification.from_pretrained("ronoys/testDeploy")
 
     effect_ner_model = pipeline(task="ner", model=model, tokenizer=tokenizer)
     val = effect_ner_model(sentence)
 
     result = []
     curr = ""
```

### Comparing `drug_list_ner-0.1.0/src/drug_list_ner/model2/.DS_Store` & `drug_list_ner-0.1.1/src/drug_list_ner/model2/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/src/drug_list_ner/model2/config.json` & `drug_list_ner-0.1.1/src/drug_list_ner/model2/config.json`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/src/drug_list_ner/tokenizer2/tokenizer.json` & `drug_list_ner-0.1.1/src/drug_list_ner/tokenizer2/tokenizer.json`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/src/drug_list_ner/tokenizer2/vocab.txt` & `drug_list_ner-0.1.1/src/drug_list_ner/tokenizer2/vocab.txt`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/LICENSE` & `drug_list_ner-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.1.0/pyproject.toml` & `drug_list_ner-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "drug_list_ner"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Ronoy Sarkar", email="ronoysarkar.mail@gmail.com" },
 ]
 description = "An NER model to identify prescription drugs in a text sample"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `drug_list_ner-0.1.0/PKG-INFO` & `drug_list_ner-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drug_list_ner
-Version: 0.1.0
+Version: 0.1.1
 Summary: An NER model to identify prescription drugs in a text sample
 Author-email: Ronoy Sarkar <ronoysarkar.mail@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

