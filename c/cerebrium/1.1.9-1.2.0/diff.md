# Comparing `tmp/cerebrium-1.1.9.tar.gz` & `tmp/cerebrium-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.1.9.tar", max compression
+gzip compressed data, was "cerebrium-1.2.0.tar", max compression
```

## Comparing `cerebrium-1.1.9.tar` & `cerebrium-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0      371 2023-07-13 16:29:26.693686 cerebrium-1.1.9/EXTERNAL_README.md
--rw-r--r--   0        0        0    34594 2023-07-13 16:29:26.693686 cerebrium-1.1.9/LICENSE
--rw-r--r--   0        0        0      360 2023-07-13 16:32:25.612339 cerebrium-1.1.9/cerebrium/__init__.py
--rwxr-xr-x   0        0        0    25216 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/cli.py
--rw-r--r--   0        0        0    33936 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/conduit.py
--rw-r--r--   0        0        0     5048 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/core.py
--rw-r--r--   0        0        0     2488 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/errors.py
--rw-r--r--   0        0        0    10182 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/flow.py
--rw-r--r--   0        0        0     3070 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3990 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      600 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/models/base.py
--rw-r--r--   0        0        0      550 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      411 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/models/onnx.py
--rw-r--r--   0        0        0      793 2023-07-13 16:29:26.693686 cerebrium-1.1.9/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      270 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      273 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8545 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/requests.py
--rw-r--r--   0        0        0    11285 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/README_Diffusers.md
--rw-r--r--   0        0        0     5592 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/README_Transformers.md
--rw-r--r--   0        0        0      110 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/__init__.py
--rw-r--r--   0        0        0     1825 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/diffuser_config.yaml
--rw-r--r--   0        0        0    14934 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/diffuser_tuner.py
--rw-r--r--   0        0        0     9079 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/fine_tuner.py
--rw-r--r--   0        0        0     1716 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/finetuning_model.py
--rw-r--r--   0        0        0        0 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
--rw-r--r--   0        0        0     2647 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
--rw-r--r--   0        0        0     4040 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
--rw-r--r--   0        0        0     1614 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/trainer/transformer_config.yaml
--rw-r--r--   0        0        0     1048 2023-07-13 16:29:26.697686 cerebrium-1.1.9/cerebrium/utils.py
--rw-r--r--   0        0        0     2378 2023-07-13 16:32:25.612339 cerebrium-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 cerebrium-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0      372 2023-07-18 19:56:44.930073 cerebrium-1.2.0/EXTERNAL_README.md
+-rw-r--r--   0        0        0    34594 2023-07-18 19:56:44.930073 cerebrium-1.2.0/LICENSE
+-rw-r--r--   0        0        0      360 2023-07-18 19:59:43.627367 cerebrium-1.2.0/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    39278 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/cli.py
+-rw-r--r--   0        0        0    33936 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5048 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/core.py
+-rw-r--r--   0        0        0     2488 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/errors.py
+-rw-r--r--   0        0        0    10182 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/flow.py
+-rw-r--r--   0        0        0     3070 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3990 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      600 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/base.py
+-rw-r--r--   0        0        0      550 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      411 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0      793 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      270 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      273 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8545 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/requests.py
+-rw-r--r--   0        0        0    10957 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/README_Diffusers.md
+-rw-r--r--   0        0        0     5592 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/README_Transformers.md
+-rw-r--r--   0        0        0      110 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/__init__.py
+-rw-r--r--   0        0        0     1819 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/diffuser_config.yaml
+-rw-r--r--   0        0        0    15030 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/diffuser_tuner.py
+-rw-r--r--   0        0        0     1837 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/example_configs/falcon-40b.yaml
+-rw-r--r--   0        0        0     1804 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/example_configs/falcon-7b.yaml
+-rw-r--r--   0        0        0     9079 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/fine_tuner.py
+-rw-r--r--   0        0        0     1716 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/finetuning_model.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/__init__.py
+-rw-r--r--   0        0        0     2647 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py
+-rw-r--r--   0        0        0     4115 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py
+-rw-r--r--   0        0        0     1593 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/trainer/transformer_config.yaml
+-rw-r--r--   0        0        0     1048 2023-07-18 19:56:44.934073 cerebrium-1.2.0/cerebrium/utils.py
+-rw-r--r--   0        0        0     2378 2023-07-18 19:59:43.627367 cerebrium-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1582 1970-01-01 00:00:00.000000 cerebrium-1.2.0/PKG-INFO
```

### Comparing `cerebrium-1.1.9/LICENSE` & `cerebrium-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/conduit.py` & `cerebrium-1.2.0/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/core.py` & `cerebrium-1.2.0/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/errors.py` & `cerebrium-1.2.0/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/flow.py` & `cerebrium-1.2.0/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/logging/arize.py` & `cerebrium-1.2.0/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/logging/base.py` & `cerebrium-1.2.0/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/logging/censius.py` & `cerebrium-1.2.0/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/models/base.py` & `cerebrium-1.2.0/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/models/hf_pipeline.py` & `cerebrium-1.2.0/cerebrium/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/models/sklearn.py` & `cerebrium-1.2.0/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/requests.py` & `cerebrium-1.2.0/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/trainer/README_Diffusers.md` & `cerebrium-1.2.0/cerebrium/trainer/README_Diffusers.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,39 +31,39 @@
 Currently, the models that have been tested on the diffuser trainer are:
 
 > - [runwayml/stable-diffusion-v1-5](https://huggingface.co/runwayml/stable-diffusion-v1-5)
 
 ## Curating a dataset
 
 The follorwing are a set of guidelines to keep in mind when curating your dataset:
-- image size of 512 x 512 
+
+- image size of 512 x 512
 - images should be upright
 - Keep the number of training images low. Aim for between 10 and 15 as your model may not converge if you use too many.
 - For style-based fine-tuning, try keep the style and colouring consistent.
 - For object focused fine-tuning, each of your images should contribute new information on the subject.  
   You can do this by varying:
   - camera angle (although try keep the side of the object consistent. i.e. only take photos from the front)
   - pose
   - props or styles
   - background in the photos (if you would like varied backgrounds in your outputs.)
-  
+
 ### Using prior preservation
-Stable diffusion models are prone to catastrophic forgetting of classes when training. For example, if you have finetuned your model on a prompt of "Photo of a sdf dog" and supplied photos of a Labrador, your model may only predict photos of a labrador when asked for photos of a dog. 
+
+Stable diffusion models are prone to catastrophic forgetting of classes when training. For example, if you have finetuned your model on a prompt of "Photo of a sdf dog" and supplied photos of a Labrador, your model may only predict photos of a labrador when asked for photos of a dog.
 
 Therefore prior preservation works as a kind of regularizer for stable diffusion models that will still be generating other prompts in the same class.
 
 The idea is to supervise the fine-tuning process with the model's own generated samples of the class noun.
 In practice, this means having the model fit both the new images and the generated images simultaneously during training.
 
-To use a prior class in training, you need to supply a number of class images as well as a prompt to generate these images with.   
-Alternatively, you can generate these images beforehand and upload that prompt dataset and a prompt. When curating a prior class dataset, the goal is to select a wide variety of outputs from your model. 
-
-See [this section](#description-of-the-optional-parameters-to-deploy-your-model-with) for more information on the parameters to use. 
-
+To use a prior class in training, you need to supply a number of class images as well as a prompt to generate these images with.  
+Alternatively, you can generate these images beforehand and upload that prompt dataset and a prompt. When curating a prior class dataset, the goal is to select a wide variety of outputs from your model.
 
+See [this section](#description-of-the-optional-parameters-to-deploy-your-model-with) for more information on the parameters to use.
 
 ## Deploying a finetuning job
 
 ```bash
 cerebrium train-diffuser <<YOUR_JOB_NAME>> <<API_KEY_IF_NOT_LOGGED_IN>> <<HUGGINGFACE_MODEL_PATH>>  <<PATH_TO_YOUR_TRAINING_DATASET_IMAGES>> <<TRAINING_PROMPT>>
 ```
 
@@ -86,49 +86,47 @@
 | --prior-class-image-dir  | TEXT    | Path to directory containing images generated prior to training using a class prompt.                              |
 | --prior-class-prompt     | TEXT    | Prompt to generate images prior to training for the class.                                                         |
 | --num-prior-class-images | INTEGER | Number of images to generate prior to training for the class. [default: 0]                                         |
 | --training-args          | TEXT    | Json string of training keyword arguments for the model. Example: '{"num_train_epochs": 5, "learning_rate": 1e-4}' |
 | --revision               | TEXT    | Huggingface revision of the model to use. [default: main]                                                          |
 | --log-level              | TEXT    | Log level for the builder deployment. Can be one of 'DEBUG' or 'INFO' [default: INFO]                              |
 
-
 <!-- For added control, a finetuning task can be deployed using the python functions. If this is required, please contact the team for documentation and instructions. -->
 <br>
 
 ### Supported training kwargs reference
 
 <!-- **Table of possible training kwargs** -->
 
-| Key                                                                                                   | Default    | Description                                                                                 |
-| ----------------------------------------------------------------------------------------------------- | ---------- | ------------------------------------------------------------------------------------------- |
-| gradient_accumulation_steps                                                                           | 1          | Number of update steps to accumulate the gradient over before the backward/update pass.     |
-| learning_rate                                                                                         | 0.0005     | Initial learning rate to use in training.                                                   |
-| lr_schedule                                                                                           | "constant" | Schedule for the learning rate to follow.  Can be:["linear", "cosine", "cosine_with_restarts", "polynomial", "constant", "constant_with_warmup"] |
-| max_train_steps                                                                                       | None       | Total number of training steps to perform. Overrides num_train_epochs if provided.          |
-| num_train_epochs                                                                                      | 30         | Number of epochs to train for where one epoch is an iteration over the dataset              |
-| train_batch_size                                                                                      | 2          | Batch size per device to be used by the training image dataloader                           |
-| scale_lr                                                                                              | False      | Scale the learning rate by the number of GPUs, gradient accumulation steps, and batch size. |
-| warmup_steps                                                                                          | 0          | Number of gradient warmup steps before training                                             |
-| validation_epochs                                                                                     | 10         | Number of epochs before each validation step.                                               |
-| use_8bit_adam                                                                                         | True       | Use 8-bit adam from bitsandbytes for the optimisation                                       |
-
+| Key                         | Default    | Description                                                                                                                                     |
+| --------------------------- | ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
+| gradient_accumulation_steps | 1          | Number of update steps to accumulate the gradient over before the backward/update pass.                                                         |
+| learning_rate               | 0.0005     | Initial learning rate to use in training.                                                                                                       |
+| lr_schedule                 | "constant" | Schedule for the learning rate to follow. Can be:["linear", "cosine", "cosine_with_restarts", "polynomial", "constant", "constant_with_warmup"] |
+| max_train_steps             | None       | Total number of training steps to perform. Overrides num_train_epochs if provided.                                                              |
+| num_train_epochs            | 30         | Number of epochs to train for where one epoch is an iteration over the dataset                                                                  |
+| train_batch_size            | 2          | Batch size per device to be used by the training image dataloader                                                                               |
+| scale_lr                    | False      | Scale the learning rate by the number of GPUs, gradient accumulation steps, and batch size.                                                     |
+| warmup_steps                | 0          | Number of gradient warmup steps before training                                                                                                 |
+| validation_epochs           | 10         | Number of epochs before each validation step.                                                                                                   |
+| use_8bit_adam               | True       | Use 8-bit adam from bitsandbytes for the optimisation                                                                                           |
 
 <br>
 
 ---
 
 # Retrieving your training results
 
 Once your training is complete, you can download the training results using:
 
 ```bash
 cerebrium download-model <<JOB_ID>> <<API_KEY>>
 ```
 
-This will return a zip file which contains your attention processors and the validation images generated by your model during training.  
+This will return a zip file which contains your attention processors and the validation images generated by your model during training.
 
 # Using your Fine-tuned Diffuser
 
 Using your finetuning results is done as follows:
 
 ```python
```

### Comparing `cerebrium-1.1.9/cerebrium/trainer/README_Transformers.md` & `cerebrium-1.2.0/cerebrium/trainer/README_Transformers.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Contents
 
 - [Contents](#contents)
 - [Introduction](#introduction)
 - [Using the fine-tuner](#using-the-fine-tuner)
   - [Curating a dataset](#curating-a-dataset)
   - [Deploying a finetuning job](#deploying-a-finetuning-job)
@@ -20,14 +19,15 @@
 
 In future, we plan to release capabilities for custom prompting templates, however, at the moment we use the well-proven Alpaca-Lora prompt templating.
 For more information, see
 
 <!-- TODO link to templates. -->
 
 # Using the fine-tuner
+
 ## Curating a dataset
 
 The finetuning library has been built to leverage Parameter Efficient Finetuning and Low Rank Approximation to reduce the number of trainable parameters by >99.9% while, as shown by multiple experiments in the literature, providing results that are comparable to full fine-tuning.  
 Due to the much lower number of trainable parameters, the datasets used do not need to be greater than 1000 examples. In most situations, a dataset of 100-500 prompts is more than adequate to achieve good performance.
 
 For your convenience, an example dataset has been provided for Beta testing [here](../../examples/training-job/dataset.json). The dataset is a JSON or JSONL file which contains a "prompt", "completion", and if needed "context".
 
@@ -44,14 +44,15 @@
 <!-- For added control, a finetuning task can be deployed using the python functions. If this is required, please contact the team for documentation and instructions. -->
 
 ## Finetuning a different model
 
 At present, the models that have been tested on the fine-tuner environment are:
 
 > - Llama 7B
+
 <!-- TODO: Add to this list as we test.  -->
 
 To fine-tune a model that is not loaded with `transformers.AutoModelForCausalLM`, you can set the model type using the `--model-type` flag.  
 For example, to fine-tune a model such as T5 which requires `transformers.T5ForConditionalGeneration` you would use:
 
 ```bash
 cerebrium train my-t5-conditional <<YOUR_API_KEY>> "google/flan-t5-large" <<PATH_TO_YOUR_FINETUNING_DATASET>> --model-type "T5ForConditionalGeneration"
@@ -82,16 +83,16 @@
 
 ```bash
 cerebrium download-model <<JOB_ID>> <<API_KEY>>
 ```
 
 This will return a zip file which contains your **adapter** and **adapter config** which should be in the order of 10MB for your 7B parameter model due to the extreme efficiency of PEFT fine-tuning.
 
-
 # Using your Fine-tuned Adaptor
+
 Using your adapter can be done simply by adding two lines as shown here:
 
 ```python
   from transformers import AutoModelForCausalLM
   from peft import PeftModel, PeftConfig # Add the peft libraries we need for the adapter
 
   peft_model_id = "path/toYourAdapter"
@@ -102,17 +103,18 @@
 
   model = model.to("cuda")
   model.eval() # set the model to inference mode
 
 ```
 
 Now for inference, you just need to place the prompt into the template used for training. In this example we do it as follows
-``` python
+
+```python
   template =  "### Instruction:\n{instruction}\n\n### Response:\n"
-  question = template.format(instruction=prompt) 
+  question = template.format(instruction=prompt)
   inputs = tokenizer(question, return_tensors="pt")
 
   with torch.no_grad():
     outputs = model.generate(input_ids=inputs["input_ids"].to("cuda"), max_new_tokens=10)
     print(tokenizer.batch_decode(outputs.detach().cpu().numpy(), skip_special_tokens=True)[0])
 
 ```
```

### Comparing `cerebrium-1.1.9/cerebrium/trainer/diffuser_config.yaml` & `cerebrium-1.2.0/cerebrium/trainer/diffuser_config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 %YAML 1.2
 ---
 training_type: "diffuser" # Type of training to run. Either "diffuser" or "transformer".
 name: "test-config-file" # Name of the experiment.
 api-key: "YOUR API KEY HERE" # Your Cerebrium API key.
 hf_model_path: "runwayml/stable-diffusion-v1-5"
 revision: "main" # Revision of the diffuser model to use.
-train_prompt: "Photo of a tsdf dog." 
+train_prompt: "Photo of a tsdf dog."
 validation_prompt: ~ # an optional validation prompt to use. If ~, will use the training prompt.
 custom_tokenizer: "" # custom tokenizer from AutoTokenizer if required.
 log_level: "WARNING" # log_level level for logging.
 
-
 train_image_dir: data/training_class_images/ # Directory of training images.
 prior_class_image_dir: ~ # "data/prior_class_images" # Optional directory of images to use for prior class.
 prior_class_prompt: "Photo of a dog."
 
 # Training params
 training_args:
   # General training params
@@ -27,21 +26,20 @@
   train_batch_size: 2
   num_prior_class_images: 10
   prior_class_generation_batch_size: 2
   prior_loss_weight: 1.0 # Weight of prior loss in the total loss.
   max_train_steps: ~ # maximum training steps which overrides number of training epochs
   validation_epochs: 10 # number of epochs before running validation and checkpointing
 
-  
   # Training loop params
   gradient_accumulation_steps: 1
   lr_scheduler: "constant"
   lr_warmup_steps: 5
   lr_num_cycles: 1
   lr_power: 1.0
   allow_tf32: False
   max_grad_norm: 1.0
-  mixed_precision: 'no' # "fp16 or "bf16"
+  mixed_precision: "no" # "fp16 or "bf16"
   prior_generation_precision: ~
-  scale_lr: False 
+  scale_lr: False
   use_8bit_adam: True
   use_xformers: True # Whether to use xformers memory efficient attention or not.
```

### Comparing `cerebrium-1.1.9/cerebrium/trainer/diffuser_tuner.py` & `cerebrium-1.2.0/cerebrium/trainer/diffuser_tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         )
 
         prior_class_prompt = config.get("prior_class_prompt", "")
         if bool(prior_class_prompt or prior_class_image_dir):
             config["with_prior_preservation"] = True
             assert (
                 prior_class_prompt is not None
-            ), "Please provide a class prompt if you would like to use prior class images in training."
+            ), "Please provide a class prompt with your prior_class_image_dir if you would like to use prior class images in training."
+            print("🧱 Using prior class images in training.")
         else:
             config["with_prior_preservation"] = False
 
         # Set the logging log_level
         config["log_level"] = (
             log_level if log_level in ["", None] else config.get("log_level", "INFO")
         )
```

### Comparing `cerebrium-1.1.9/cerebrium/trainer/fine_tuner.py` & `cerebrium-1.2.0/cerebrium/trainer/fine_tuner.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/finetuning_model.py` & `cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/finetuning_model.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py` & `cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.9/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py` & `cerebrium-1.2.0/cerebrium/trainer/finetune_LLM/userDataset/data_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 from json.decoder import JSONDecodeError
 from pathlib import Path
 from typing import Union
-from jsonschema import Draft202012Validator
+from jsonschema import Draft202012Validator, validate
 
 
 # class to perform validation
 class Dataset_Validator:
     """
     Class to check JSON dataset and ensure the data is labeled for training.
     """
 
     def __init__(
         self,
-        prompt_column: Union[str, None] = None,
+        prompt_column: str = "prompt",
         context_column: str = "context",
         label_column: str = "completion",
         custom_schema: Union[dict, None] = None,
         verbose: bool = False,
         pd_json_kwargs: Union[dict, None] = None,
     ) -> None:
         """Init for dataset validator class
 
         Args:
-            prompt_column (str, optional): Dataset prompt column name. Defaults to None.
+            prompt_column (str, optional): Dataset prompt column name. Defaults to "prompt".
             context_column (str, optional): Dataset context column name. Defaults to "context".
             label_column (str, optional): Dataset label column name. Defaults to "completion".
             custom_schema (dict, optional): Your very own custom jsonschema to use instead. Defaults to None.
             verbose (bool, optional): Verbose or quiet. Defaults to False.
             pd_json_kwargs, (dict, optional): kwargs for pandas when loading dataset from JSON. Defaults to None.
         """
         self.verbose = verbose
@@ -35,68 +35,67 @@
         if pd_json_kwargs is None:
             pd_json_kwargs = {"lines": False, "orient": None}
         self.pd_json_kwargs = pd_json_kwargs
 
         # Init data validation object
         if not custom_schema:
             self.schema = {
-                # "type": "object",
+                "type": "object",
                 "properties": {
                     prompt_column: {"type": "string"},
-                    context_column: {"type": ["string", "null"]},
                     label_column: {"type": "string"},
                     "source": {"type": ["string", "null"]},
                 },
-                "required": ["prompt"],
+                "required": [prompt_column, label_column],
                 "additionalProperties": False,
             }
+            if context_column:  # if context column is provided, add it to the schema
+                self.schema["properties"][context_column] = {"type": "string"}
         else:
             self.schema = custom_schema
 
         Draft202012Validator.check_schema(self.schema)
-        self.validator = Draft202012Validator(self.schema)
 
-    def __call__(
-        self, filename: Path, return_dataframe: bool = False
-    ):
+    def __call__(self, filename: Path, return_dataframe: bool = False):
         # Check if the file exists
         assert os.path.exists(filename), f"The file '{filename}' could not be found"
         if self.verbose:
             print("Found dataset file.")
 
         # Check the json is valid for training.
         df_data = self.load_json_file(filename=filename)
         result = self.is_valid_for_training(df=df_data)
 
         return result
-        
 
     def is_valid_for_training(self, df) -> bool:
         if self.verbose:
             print(f"Found {len(df)} data entries")
         for _, row in df.iterrows():
             row = row.dropna()
-            pt = row.to_json()
-            result = self.validator.validate(pt)
+            pt = row.to_dict()
+            result = validate(instance=pt, schema=self.schema)
             if result is not None:
                 if self.verbose:
                     print(f"Found invalid entry: {pt}")
                 return False
 
         if self.verbose:
             print("All entries in the dataset passed validation ✅")
         return True
 
     def load_json_file(self, filename):
         try:
             import pandas as pd
         except ImportError as error:
-            print("Pandas is required for validating JSON datasets for the cerebrium trainer. Please install 'pandas' with pip or conda.")
+            print(
+                "Pandas is required for validating JSON datasets for the cerebrium trainer. Please install 'pandas' with pip or conda."
+            )
             raise error
-        
+
         extension = os.path.splitext(filename)[1]
 
         if extension in {".json", ".jsonl"}:
             if extension == ".jsonl":
                 self.pd_json_kwargs["orient"] = "records"
             if self.verbose:
                 print(f"Reading in JSON file at {filename}")
```

### Comparing `cerebrium-1.1.9/cerebrium/trainer/transformer_config.yaml` & `cerebrium-1.2.0/cerebrium/trainer/transformer_config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 %YAML 1.2
 ---
 training_type: "transformer" # Type of training to run. Either "diffuser" or "transformer".
 
 name: test-config-file # Name of the experiment.
-api_key: dev-private-4f293d340d112179542f # Your Cerebrium API key.
+api_key: YOUR API KEY HERE # Your Cerebrium API key.
 
 # Model params:
 hf_model_path: "decapoda-research/llama-7b-hf"
 model_type: "AutoModelForCausalLM"
 dataset_path: path/to/your/dataset.json # path to your local JSON dataset.
 custom_tokenizer: "" # custom tokenizer from AutoTokenizer if required.
 seed: 42 # random seed for reproducibility.
@@ -24,15 +24,14 @@
   learning_rate: 0.0001
   group_by_length: False
 
 base_model_args: # args for loading in the base model.
   load_in_8bit: True
   device_map: "auto"
 
-
 peft_lora_args: # peft lora args.
   r: 8
   lora_alpha: 32
   lora_dropout: 0.05
   target_modules: ["q_proj", "v_proj"]
   bias: "none"
   task_type: "CAUSAL_LM"
@@ -41,12 +40,12 @@
   # prompt_template: "short"
   # if you would like a custom prompt template it's possible to specify it here as below:
   prompt_template:
     description: "A shorter template to experiment with."
     prompt_input: "### Instruction:\n{instruction}\n\n### Input:\n{input}\n\n### Response:\n"
     prompt_no_input: "### Instruction:\n{instruction}\n\n### Response:\n"
     response_split: "### Response:"
-  instruction_column:  "prompt"
-  label_column:  "completion"
-  context_column:  "context"
-  cutoff_len:  512
-  train_val_ratio:  0.9
+  instruction_column: "prompt"
+  label_column: "completion"
+  context_column: "context"
+  cutoff_len: 512
+  train_val_ratio: 0.9
```

### Comparing `cerebrium-1.1.9/cerebrium/utils.py` & `cerebrium-1.2.0/cerebrium/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
 
-def _convert_input_data(data: Any) -> list:    # type: ignore
+def _convert_input_data(data: Any) -> list:  # type: ignore
     # sourcery skip: merge-duplicate-blocks, remove-redundant-if, remove-unnecessary-else, swap-if-else-branches
     """
     Convert the input data to a list.
 
     Args:
         data (Union[list, ndarray, Tensor]): The data to convert.
 
@@ -24,16 +24,18 @@
         numpy_installed = True
     except ImportError:
         numpy_installed = False
 
     if torch_installed:
         from torch import Tensor
         from numpy import ndarray
+
         if isinstance(data, Tensor):
             return data.tolist()
         elif isinstance(data, ndarray):
             return data.tolist()
     if numpy_installed:
         from numpy import ndarray
+
         return data.tolist() if isinstance(data, ndarray) else data
     else:
         return data
```

### Comparing `cerebrium-1.1.9/pyproject.toml` & `cerebrium-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.1.9"
+version = "1.2.0"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "EXTERNAL_README.md"
 exclude = ["tests/*", "dist/*", "webhook/*", "builder/*", "prebuilt/*", "common/*", "examples/*", "trainer/*", "README.md"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.1.9/PKG-INFO` & `cerebrium-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.1.9
+Version: 1.2.0
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -31,7 +31,8 @@
 Description-Content-Type: text/markdown
 
 # Cerebrium
 
 Cerebrium is the Python package built for use with the [Cerebrium](https://www.cerebrium.ai/) platform, which allows you to deploy your machine learning models as a REST API with a single line of code.
 
 For usage consult the [documentation](https://docs.cerebrium.ai/). The repo for the documentation can be found [here](https://github.com/CerebriumAI/docs).
+
```

