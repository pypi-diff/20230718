# Comparing `tmp/sa_app-0.0.1.tar.gz` & `tmp/sa_app-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sa_app-0.0.1.tar", max compression
+gzip compressed data, was "sa_app-0.0.2.tar", max compression
```

## Comparing `sa_app-0.0.1.tar` & `sa_app-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      659 2023-07-14 14:17:52.013941 sa_app-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 21:15:51.027113 sa_app-0.0.1/sa_app/__init__.py
--rw-r--r--   0        0        0     4321 2023-07-14 11:40:37.096062 sa_app-0.0.1/sa_app/app.py
--rw-r--r--   0        0        0        0 2023-07-09 21:15:51.035113 sa_app-0.0.1/sa_app/common/__init__.py
--rw-r--r--   0        0        0      907 2023-07-09 21:12:28.469460 sa_app-0.0.1/sa_app/common/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 21:59:49.642256 sa_app-0.0.1/sa_app/data/__init__.py
--rw-r--r--   0        0        0     5583 2023-07-14 11:40:37.104062 sa_app-0.0.1/sa_app/data/data.py
--rw-r--r--   0        0        0     2456 2023-07-05 15:42:48.849737 sa_app-0.0.1/sa_app/data/data_cleaner.py
--rw-r--r--   0        0        0     2248 2023-07-05 13:49:12.964131 sa_app-0.0.1/sa_app/data/kaggle_dataset.py
--rw-r--r--   0        0        0        0 2023-07-05 21:00:18.938516 sa_app-0.0.1/sa_app/inference/__init__.py
--rw-r--r--   0        0        0     2168 2023-07-14 14:10:19.971774 sa_app-0.0.1/sa_app/inference/inference.py
--rw-r--r--   0        0        0      796 2023-07-14 14:10:19.975774 sa_app-0.0.1/sa_app/inference_app.py
--rw-r--r--   0        0        0        0 2023-07-01 14:33:52.363077 sa_app-0.0.1/sa_app/models/__init__.py
--rw-r--r--   0        0        0      415 2023-07-03 21:28:48.416607 sa_app-0.0.1/sa_app/models/model.py
--rw-r--r--   0        0        0        0 2023-07-01 14:34:08.146982 sa_app-0.0.1/sa_app/training/__init__.py
--rw-r--r--   0        0        0     4953 2023-07-14 11:34:21.137593 sa_app-0.0.1/sa_app/training/lightning_model_wrapper.py
--rw-r--r--   0        0        0     1515 2023-07-04 21:07:31.864810 sa_app-0.0.1/sa_app/training/optmizer.py
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 sa_app-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      659 2023-07-18 09:10:06.274105 sa_app-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 21:15:51.027113 sa_app-0.0.2/sa_app/__init__.py
+-rw-r--r--   0        0        0     4609 2023-07-17 22:40:29.961467 sa_app-0.0.2/sa_app/app.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:15:51.035113 sa_app-0.0.2/sa_app/common/__init__.py
+-rw-r--r--   0        0        0     1097 2023-07-17 22:40:29.961467 sa_app-0.0.2/sa_app/common/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:59:49.642256 sa_app-0.0.2/sa_app/data/__init__.py
+-rw-r--r--   0        0        0     5570 2023-07-17 22:40:29.965467 sa_app-0.0.2/sa_app/data/data.py
+-rw-r--r--   0        0        0     2456 2023-07-05 15:42:48.849737 sa_app-0.0.2/sa_app/data/data_cleaner.py
+-rw-r--r--   0        0        0     2248 2023-07-05 13:49:12.964131 sa_app-0.0.2/sa_app/data/kaggle_dataset.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:00:18.938516 sa_app-0.0.2/sa_app/inference/__init__.py
+-rw-r--r--   0        0        0     2168 2023-07-14 14:10:19.971774 sa_app-0.0.2/sa_app/inference/inference.py
+-rw-r--r--   0        0        0      860 2023-07-17 22:15:09.364444 sa_app-0.0.2/sa_app/inference_app.py
+-rw-r--r--   0        0        0        0 2023-07-01 14:33:52.363077 sa_app-0.0.2/sa_app/models/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-03 21:28:48.416607 sa_app-0.0.2/sa_app/models/model.py
+-rw-r--r--   0        0        0        0 2023-07-01 14:34:08.146982 sa_app-0.0.2/sa_app/training/__init__.py
+-rw-r--r--   0        0        0     4998 2023-07-16 14:21:52.329050 sa_app-0.0.2/sa_app/training/lightning_model_wrapper.py
+-rw-r--r--   0        0        0     1515 2023-07-04 21:07:31.864810 sa_app-0.0.2/sa_app/training/optmizer.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 sa_app-0.0.2/PKG-INFO
```

### Comparing `sa_app-0.0.1/pyproject.toml` & `sa_app-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sa_app"
-version = "0.0.1"
+version = "0.0.2"
 authors = ["prabhu <prabhupad26@gmail.com>"]
 description="Sentiment analyzer app"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `sa_app-0.0.1/sa_app/app.py` & `sa_app-0.0.2/sa_app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import Dict, List, Tuple
 
 import pytorch_lightning as pl
 import torch
 import wandb
 import yaml
 from pytorch_lightning.callbacks import LearningRateMonitor, ModelCheckpoint
@@ -9,15 +10,15 @@
 from sa_app.common.utils import init_model_loggers, parse_args
 from sa_app.data.data import InitializeDataset, SentimentIterableDataset
 from sa_app.models.model import Model
 from sa_app.training.lightning_model_wrapper import LightningModelWrapper
 from transformers import AutoConfig, AutoModelForSequenceClassification, AutoTokenizer
 
 
-def init_model_callbacks(training_params: dict) -> List:
+def init_model_callbacks(training_params: dict) -> List[LearningRateMonitor | ModelCheckpoint]:
     model_checkpoint = ModelCheckpoint(
         dirpath=training_params["callbacks"]["dirpath"],
         filename="best_model",
         monitor=training_params["callbacks"]["monitor_var"],
         mode=training_params["callbacks"]["monitor_var_mode"],
         save_top_k=3,  # Save the top 3 models based on the monitored metric
     )
@@ -75,20 +76,23 @@
         callbacks=callbacks,
         **training_params["trainer"],
     )
     return trainer
 
 
 def train(config: dict, device: str, training_params: Dict, dataset_params: Dict, seed: int, inference_params: Dict):
+    # wandb login
+    wandb.login(key=os.getenv("WANDB_API_KEY"))
+
     # Global seeding
     pl.seed_everything(seed=seed)
     model_config, model = load_model(training_params)
     tokenizer = AutoTokenizer.from_pretrained(training_params.get("base-model-name"))
     train_dataset, valid_dataset = get_dataset(dataset_params, tokenizer)
-    loggers = init_model_loggers(training_params["logging"]["log_dir"])
+    loggers = init_model_loggers(dataset_params, training_params)
     callbacks = init_model_callbacks(training_params)
 
     # PL wrapper
     model_wrapped = LightningModelWrapper(
         model=model,
         optimizer_params=training_params["optimizer"],
         lr_scheduler_params=training_params["lr_scheduler"] if "lr_scheduler" in training_params else None,
@@ -105,22 +109,26 @@
 
     # Trainer initialization
     trainer = get_trainer(loggers, devices, accelerator, callbacks, training_params)
 
     # Initiate trainer
     trainer.fit(model=model_wrapped, train_dataloaders=train_dataset, val_dataloaders=valid_dataset, ckpt_path="last")
 
+    artifact = wandb.Artifact("best_model_checkpoint", type="trained-model")
+    artifact.add_file(callbacks[1].best_model_path)
+    wandb.run.log_artifact(artifact)
+
     wandb.finish()
 
 
 def main():
     args = parse_args()
     config = yaml.safe_load(open(args.config, "r"))
     device = "cuda" if torch.cuda.is_available() else "cpu"
     if args.mode == "train":
         train(config=config, device=device, **config)
-    # else:
-    #     inference(config=config, device=device, **config)
+    else:
+        raise NotImplementedError(f"Method {args.mode} not implemented")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sa_app-0.0.1/sa_app/common/utils.py` & `sa_app-0.0.2/sa_app/common/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import argparse
 import csv
-from typing import List
+from typing import Dict, List
 
 from pytorch_lightning.loggers import WandbLogger
 
 
-def init_model_loggers(log_dir: str) -> List[WandbLogger]:
-    wandb_logger = WandbLogger(project="sa-roberta", save_dir=log_dir)
+def init_model_loggers(dataset_params: Dict, training_params: Dict) -> List[WandbLogger]:
+    wandb_project_name = dataset_params.get("wandb_storage").get("wandb_project_name")
+    log_dir = training_params.get("logging").get("log_dir")
+    wandb_logger = WandbLogger(project=wandb_project_name, save_dir=log_dir)
     return [
         wandb_logger,
     ]
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
```

### Comparing `sa_app-0.0.1/sa_app/data/data.py` & `sa_app-0.0.2/sa_app/data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os.path
 from glob import glob
 from typing import Dict, Generator, List, Optional, Tuple
 
 import pandas as pd
 import torch
+import wandb
 from sa_app.data.data_cleaner import StackedPreprocessor
 from sa_app.data.kaggle_dataset import get_dataset_length, get_file_names, split_dataset
 from torch.utils.data import IterableDataset
 from tqdm import tqdm
 from transformers import AutoTokenizer
 
 
@@ -26,16 +27,14 @@
             wandb_user_id = wandb_storage.get("wandb_user_id")
             wandb_project_name = wandb_storage.get("wandb_project_name")
             wandb_artifact_name = wandb_storage.get("wandb_artifact_name")
             wandb_artifact_type = wandb_storage.get("wandb_artifact_type")
             wandb_file_type = wandb_storage.get("training_file_type")
             wandb_artifact_version = wandb_storage.get("wandb_artifact_version")
             labels_mapping_file_name = wandb_storage.get("labels_mapping_file_name")
-            import wandb
-
             run = wandb.init(entity=wandb_user_id, project=wandb_project_name, job_type="download_dataset")
             artifact = run.use_artifact(
                 f"{wandb_user_id}/{wandb_project_name}/{wandb_artifact_name}:{wandb_artifact_version}",
                 type=f"{wandb_artifact_type}",
             )
             artifact_dir = artifact.download()
             assert len(glob(f"{artifact_dir}/*.{wandb_file_type}")) > 0, "CSV file download failed"
```

### Comparing `sa_app-0.0.1/sa_app/data/data_cleaner.py` & `sa_app-0.0.2/sa_app/data/data_cleaner.py`

 * *Files identical despite different names*

### Comparing `sa_app-0.0.1/sa_app/data/kaggle_dataset.py` & `sa_app-0.0.2/sa_app/data/kaggle_dataset.py`

 * *Files identical despite different names*

### Comparing `sa_app-0.0.1/sa_app/inference/inference.py` & `sa_app-0.0.2/sa_app/inference/inference.py`

 * *Files identical despite different names*

### Comparing `sa_app-0.0.1/sa_app/inference_app.py` & `sa_app-0.0.2/sa_app/inference_app.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,9 +18,14 @@
 
 @app.route("/sentiment_analysis", methods=["POST"])
 def get_sentiment():
     new_tweet = {"id": request.json["id"], "tweet_content": request.json["tweet_content"]}
     return jsonify(ie_obj.perform_inference(new_tweet["tweet_content"]))
 
 
+@app.route("/home")
+def test_fn():
+    return "Hello World!!"
+
+
 if __name__ == "__main__":
     app.run()
```

### Comparing `sa_app-0.0.1/sa_app/training/lightning_model_wrapper.py` & `sa_app-0.0.2/sa_app/training/lightning_model_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from typing import Any, Dict, Optional, Union
 
 import pytorch_lightning as pl
 import torch
 from sa_app.training.optmizer import LearningRateScheduler, Optimizer
 from torch.nn import CrossEntropyLoss
 from torchmetrics import Accuracy, MeanMetric, Metric
-from transformers import PreTrainedModel
+from transformers import AutoModelForSequenceClassification
 
 
 class Split(str, Enum):
     TRAIN = "train"
     VALID = "valid"
     TEST = "test"
 
     def __str__(self):
         return self.value
 
 
 class LightningModelWrapper(pl.LightningModule):
     def __init__(
         self,
-        model: PreTrainedModel,
+        model: AutoModelForSequenceClassification,
         optimizer_params: Optional[dict] = None,
         lr_scheduler_params: Optional[dict] = None,
         unique_config: Optional[dict] = None,
     ):
         super().__init__()
 
         self.model = model
@@ -116,15 +116,15 @@
             }
 
         if scheduler:
             return [optimizer], [scheduler]
         else:
             return optimizer
 
-    def sav(self, path: Union[str, Path]) -> None:
+    def save_model(self, path: Union[str, Path]) -> None:
         """Save the model using the original HF AutoModel.
 
         This is useful for when you'd like to export the model to the hub.
         Args:
             path: Path to save the model to.
         """
         self.model.save_pretrained(path)
```

### Comparing `sa_app-0.0.1/sa_app/training/optmizer.py` & `sa_app-0.0.2/sa_app/training/optmizer.py`

 * *Files identical despite different names*

### Comparing `sa_app-0.0.1/PKG-INFO` & `sa_app-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sa-app
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sentiment analyzer app
 Author: prabhu
 Author-email: prabhupad26@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

