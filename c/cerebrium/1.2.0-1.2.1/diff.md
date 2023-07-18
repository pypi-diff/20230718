# Comparing `tmp/cerebrium-1.2.0.tar.gz` & `tmp/cerebrium-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.2.0.tar", max compression
+gzip compressed data, was "cerebrium-1.2.1.tar", max compression
```

## Comparing `cerebrium-1.2.0.tar` & `cerebrium-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      372 2023-07-18 19:56:44.930073 cerebrium-1.2.0/EXTERNAL_README.md
--rw-r--r--   0        0        0    34594 2023-07-18 19:56:44.930073 cerebrium-1.2.0/LICENSE
--rw-r--r--   0        0        0      360 2023-07-18 19:59:43.627367 cerebrium-1.2.0/cerebrium/__init__.py
--rwxr-xr-x   0        0        0    39278 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/cli.py
--rw-r--r--   0        0        0    33936 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/conduit.py
--rw-r--r--   0        0        0     5048 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/core.py
--rw-r--r--   0        0        0     2488 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/errors.py
--rw-r--r--   0        0        0    10182 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/flow.py
--rw-r--r--   0        0        0     3070 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3990 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      600 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/base.py
--rw-r--r--   0        0        0      550 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      411 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/onnx.py
--rw-r--r--   0        0        0      793 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      270 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      273 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8545 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/requests.py
--rw-r--r--   0        0        0    10957 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/README_Diffusers.md
--rw-r--r--   0        0        0     5592 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/README_Transformers.md
--rw-r--r--   0        0        0      110 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/__init__.py
--rw-r--r--   0        0        0     1819 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/diffuser_config.yaml
--rw-r--r--   0        0        0    15030 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/diffuser_tuner.py
--rw-r--r--   0        0        0     1837 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/example_configs/falcon-40b.yaml
--rw-r--r--   0        0        0     1804 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/example_configs/falcon-7b.yaml
--rw-r--r--   0        0        0     9079 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/fine_tuner.py
--rw-r--r--   0        0        0     1716 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/finetuning_model.py
--rw-r--r--   0        0        0        0 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
--rw-r--r--   0        0        0     2647 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
--rw-r--r--   0        0        0     4115 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
--rw-r--r--   0        0        0     1593 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/transformer_config.yaml
--rw-r--r--   0        0        0     1048 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/utils.py
--rw-r--r--   0        0        0     2378 2023-07-18 19:59:43.627367 cerebrium-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1582 1970-01-01 00:00:00.000000 cerebrium-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      372 2023-07-18 20:41:09.296294 cerebrium-1.2.1/EXTERNAL_README.md
+-rw-r--r--   0        0        0    34594 2023-07-18 20:41:09.296294 cerebrium-1.2.1/LICENSE
+-rw-r--r--   0        0        0      360 2023-07-18 20:44:03.112494 cerebrium-1.2.1/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    39278 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/cli.py
+-rw-r--r--   0        0        0    33936 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5048 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/core.py
+-rw-r--r--   0        0        0     2488 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/errors.py
+-rw-r--r--   0        0        0    10182 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/flow.py
+-rw-r--r--   0        0        0     3070 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3990 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      600 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/models/base.py
+-rw-r--r--   0        0        0      550 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      411 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0      793 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      270 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      273 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8545 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/requests.py
+-rw-r--r--   0        0        0    10957 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/README_Diffusers.md
+-rw-r--r--   0        0        0     5592 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/README_Transformers.md
+-rw-r--r--   0        0        0      110 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/__init__.py
+-rw-r--r--   0        0        0     1819 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/diffuser_config.yaml
+-rw-r--r--   0        0        0    15030 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/diffuser_tuner.py
+-rw-r--r--   0        0        0     1836 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/example_configs/falcon-40b.yaml
+-rw-r--r--   0        0        0     1804 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/example_configs/falcon-7b.yaml
+-rw-r--r--   0        0        0     9079 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/fine_tuner.py
+-rw-r--r--   0        0        0     1716 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/finetune_LLM/finetuning_model.py
+-rw-r--r--   0        0        0        0 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
+-rw-r--r--   0        0        0     2647 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
+-rw-r--r--   0        0        0     4115 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
+-rw-r--r--   0        0        0     1593 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/trainer/transformer_config.yaml
+-rw-r--r--   0        0        0     1048 2023-07-18 20:41:09.296294 cerebrium-1.2.1/cerebrium/utils.py
+-rw-r--r--   0        0        0     2378 2023-07-18 20:44:03.108494 cerebrium-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1582 1970-01-01 00:00:00.000000 cerebrium-1.2.1/PKG-INFO
```

### Comparing `cerebrium-1.2.0/LICENSE` & `cerebrium-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/cli.py` & `cerebrium-1.2.1/cerebrium/cli.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/conduit.py` & `cerebrium-1.2.1/cerebrium/conduit.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,26 +286,26 @@
                             "Transformers not installed. Please install `transformers` with pip or conda to run this model type."
                         ) from e
 
                     hf_pipeline: pipeline = HFPipeline(pipeline(**model_initialization))  # type: ignore
                     self.graph.append(hf_pipeline)
 
             # If there are processors, create a processors.py file with the respective processors
-            # Save the processors.py file in the /usr/local/lib/python3.11/dist-packages/conduit_processors directory
+            # Save the processors.py file in the /usr/local/lib/python3.10/dist-packages/conduit_processors directory
 
             self.write_processors()
             self.ready = True
 
     def write_processors(self):
         if not self._processors:
             return
         app_name = os.getenv("APP_NAME", "")
         assert app_name != "", "APP_NAME environment variable not set"
         # get python version from the runtime
-        processor_path = f"/miniconda/envs/{app_name}/lib/python3.11/conduit_processors"
+        processor_path = f"/miniconda/envs/{app_name}/lib/python3.10/conduit_processors"
         os.makedirs(processor_path, exist_ok=True)
         # Create the processors.py file
         with open(
             f"{processor_path}/processors.py",
             "w",
         ) as f:
             f.write(
```

### Comparing `cerebrium-1.2.0/cerebrium/core.py` & `cerebrium-1.2.1/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/errors.py` & `cerebrium-1.2.1/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/flow.py` & `cerebrium-1.2.1/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/logging/arize.py` & `cerebrium-1.2.1/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/logging/base.py` & `cerebrium-1.2.1/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/logging/censius.py` & `cerebrium-1.2.1/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/models/base.py` & `cerebrium-1.2.1/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/models/hf_pipeline.py` & `cerebrium-1.2.1/cerebrium/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/models/sklearn.py` & `cerebrium-1.2.1/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/requests.py` & `cerebrium-1.2.1/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/README_Diffusers.md` & `cerebrium-1.2.1/cerebrium/trainer/README_Diffusers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/README_Transformers.md` & `cerebrium-1.2.1/cerebrium/trainer/README_Transformers.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/diffuser_config.yaml` & `cerebrium-1.2.1/cerebrium/trainer/diffuser_config.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/diffuser_tuner.py` & `cerebrium-1.2.1/cerebrium/trainer/diffuser_tuner.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/example_configs/falcon-40b.yaml` & `cerebrium-1.2.1/cerebrium/trainer/example_configs/falcon-40b.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 seed: 42 # random seed for reproducibility.
 log_level: "INFO" # log_level level for logging.
 
 # Training params:
 training_args:
   logging_steps: 100
   per_device_train_batch_size: 2 # These batch sizes have not been optimised as they are hardware dependent.
-  per_device_eval_batch_size: 2 
+  per_device_eval_batch_size: 2
   warmup_steps: 0
   gradient_accumulation_steps: 4
   num_train_epochs: 30
   learning_rate: 2.0e-4
   group_by_length: False
   fp16: True
   max_grad_norm: 0.3
```

### Comparing `cerebrium-1.2.0/cerebrium/trainer/example_configs/falcon-7b.yaml` & `cerebrium-1.2.1/cerebrium/trainer/example_configs/falcon-7b.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/fine_tuner.py` & `cerebrium-1.2.1/cerebrium/trainer/fine_tuner.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/finetuning_model.py` & `cerebrium-1.2.1/cerebrium/trainer/finetune_LLM/finetuning_model.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py` & `cerebrium-1.2.1/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py` & `cerebrium-1.2.1/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/trainer/transformer_config.yaml` & `cerebrium-1.2.1/cerebrium/trainer/transformer_config.yaml`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/cerebrium/utils.py` & `cerebrium-1.2.1/cerebrium/utils.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.2.0/pyproject.toml` & `cerebrium-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.2.0"
+version = "1.2.1"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "EXTERNAL_README.md"
 exclude = ["tests/*", "dist/*", "webhook/*", "builder/*", "prebuilt/*", "common/*", "examples/*", "trainer/*", "README.md"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.2.0/PKG-INFO` & `cerebrium-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

