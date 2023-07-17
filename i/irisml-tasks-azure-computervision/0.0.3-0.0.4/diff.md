# Comparing `tmp/irisml-tasks-azure-computervision-0.0.3.tar.gz` & `tmp/irisml-tasks-azure-computervision-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-azure-computervision-0.0.3.tar", last modified: Fri Jul 14 23:23:38 2023, max compression
+gzip compressed data, was "irisml-tasks-azure-computervision-0.0.4.tar", last modified: Mon Jul 17 23:33:03 2023, max compression
```

## Comparing `irisml-tasks-azure-computervision-0.0.3.tar` & `irisml-tasks-azure-computervision-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.020494 irisml-tasks-azure-computervision-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-14 23:23:38.020494 irisml-tasks-azure-computervision-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.012493 irisml-tasks-azure-computervision-0.0.3/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.016493 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_caption_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_ocr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/delete_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/irisml/tasks/train_azure_computervision_custom_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.016493 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 23:23:38.000000 irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 23:23:38.020494 irisml-tasks-azure-computervision-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:23:38.016493 irisml-tasks-azure-computervision-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_caption_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_ocr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_delete_azure_computervision_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-14 23:21:01.000000 irisml-tasks-azure-computervision-0.0.3/test/test_train_azure_computervision_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:03.821794 irisml-tasks-azure-computervision-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-17 23:33:03.821794 irisml-tasks-azure-computervision-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:03.817793 irisml-tasks-azure-computervision-0.0.4/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:03.817793 irisml-tasks-azure-computervision-0.0.4/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/irisml/tasks/create_azure_computervision_caption_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/irisml/tasks/create_azure_computervision_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/irisml/tasks/create_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/irisml/tasks/create_azure_computervision_ocr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/irisml/tasks/delete_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/irisml/tasks/train_azure_computervision_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:03.817793 irisml-tasks-azure-computervision-0.0.4/irisml_tasks_azure_computervision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-17 23:33:03.000000 irisml-tasks-azure-computervision-0.0.4/irisml_tasks_azure_computervision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-17 23:33:03.000000 irisml-tasks-azure-computervision-0.0.4/irisml_tasks_azure_computervision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:33:03.000000 irisml-tasks-azure-computervision-0.0.4/irisml_tasks_azure_computervision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-17 23:33:03.000000 irisml-tasks-azure-computervision-0.0.4/irisml_tasks_azure_computervision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 23:33:03.000000 irisml-tasks-azure-computervision-0.0.4/irisml_tasks_azure_computervision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-17 23:33:03.821794 irisml-tasks-azure-computervision-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:33:03.821794 irisml-tasks-azure-computervision-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/test/test_create_azure_computervision_caption_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/test/test_create_azure_computervision_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/test/test_create_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/test/test_create_azure_computervision_ocr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/test/test_delete_azure_computervision_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-17 23:30:33.000000 irisml-tasks-azure-computervision-0.0.4/test/test_train_azure_computervision_custom_model.py
```

### Comparing `irisml-tasks-azure-computervision-0.0.3/LICENSE` & `irisml-tasks-azure-computervision-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/PKG-INFO` & `irisml-tasks-azure-computervision-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-computervision
-Version: 0.0.3
+Version: 0.0.4
 Summary: Azure Computer Vision API tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-computervision
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-computervision-0.0.3/README.md` & `irisml-tasks-azure-computervision-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_caption_model.py` & `irisml-tasks-azure-computervision-0.0.4/irisml/tasks/create_azure_computervision_caption_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_classification_model.py` & `irisml-tasks-azure-computervision-0.0.4/irisml/tasks/create_azure_computervision_classification_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     Model input is (image: Union[PIL.Image.Image, torch.Tensor], targets: Any). Output is a list of str.
 
     Config:
         endpoint (str): Azure Computer Vision endpoint. Must start with https://.
         api_key (str): Azure Computer Vision API key.
     """
-    VERSION = '0.1.0'
+    VERSION = '0.1.1'
 
     @dataclasses.dataclass
     class Config:
         endpoint: str
         api_key: str
 
     @dataclasses.dataclass
@@ -45,15 +45,15 @@
     def dry_run(self, inputs):
         return self.execute(inputs)
 
 
 def _should_retry(exception):
     if isinstance(exception, requests.exceptions.RequestException):
         response = getattr(exception, 'response', None)
-        if response and (response.status_code == 429 or response.status_code >= 500):
+        if response is not None and (response.status_code == 429 or response.status_code >= 500):
             return True
         if isinstance(exception, requests.exceptions.ConnectionError):
             return True
     return False
 
 
 class AzureComputerVisionModel(torch.nn.Module):
```

### Comparing `irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.4/irisml/tasks/create_azure_computervision_custom_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     Config:
         endpoint (str): Azure Computer Vision endpoint. Must start with https://.
         api_key (str): Azure Computer Vision API key.
         model_name (str): Custom model name to create.
         task_type (str): Task type. Either 'classification_multiclass' or 'object_detection'.
     """
-    VERSION = '0.1.0'
+    VERSION = '0.1.1'
 
     @dataclasses.dataclass
     class Inputs:
         class_names: typing.List[str]
 
     @dataclasses.dataclass
     class Config:
@@ -67,15 +67,15 @@
         tags = response_body['customModelResult']['tagsResult']['values']
         predictions = [0] * len(self._class_names)
         for t in tags:
             predictions[self._class_names.index(t['name'])] = t['confidence']
         return predictions
 
     def collate_result(self, batch):
-        return torch.tensor(batch)
+        return torch.tensor([b if b is not None else [0] * len(self._class_names) for b in batch])
 
 
 class AzureComputervisionCustomObjectDetectionModel(AzureComputervisionCustomModel):
     def parse_response(self, response_body):
         width = response_body['metadata']['width']
         height = response_body['metadata']['height']
         boxes = response_body['customModelResult']['objectsResult']['values']
@@ -88,8 +88,8 @@
             box = [x, y, x + w, y + h]
             for t in b['tags']:
                 class_index = self._class_names.index(t['name'])
                 predictions.append([class_index, t['confidence'], *box])
         return torch.tensor(predictions)
 
     def collate_result(self, batch):
-        return batch
+        return [b if b is not None else torch.empty(0, 6, dtype=torch.float32) for b in batch]
```

### Comparing `irisml-tasks-azure-computervision-0.0.3/irisml/tasks/create_azure_computervision_ocr_model.py` & `irisml-tasks-azure-computervision-0.0.4/irisml/tasks/create_azure_computervision_ocr_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/irisml/tasks/delete_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.4/irisml/tasks/delete_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/irisml/tasks/train_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.4/irisml/tasks/train_azure_computervision_custom_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,51 +27,76 @@
         endpoint (str): Azure Computer Vision endpoint. Must start with https://.
         api_key (str): Azure Computer Vision API key.
         task_type (str): Task type. Must be one of 'classification_multiclass' or 'object_detection'.
         azure_storage_blob_container_url (str): Azure Storage Blob container URL. Make sure the Computer Vision API resrouce has access to this storage.
         budget_in_hours (int): Budget in hours.
         keep_dataset (bool): Keep the dataset in the container after training.
     """
-    VERSION = '0.1.0'
+    VERSION = '0.1.1'
     CACHE_ENABLED = False
 
     @dataclasses.dataclass
     class Inputs:
         dataset: torch.utils.data.Dataset
         class_names: typing.List[str]
+        test_dataset: typing.Optional[torch.utils.data.Dataset] = None
 
     @dataclasses.dataclass
     class Config:
         endpoint: str
         api_key: str
         task_type: typing.Literal['classification_multiclass', 'object_detection']
         azure_storage_blob_container_url: str
         budget_in_hours: int = 1
         keep_dataset: bool = False
 
     @dataclasses.dataclass
     class Outputs:
         model_name: str
+        accuracy_top1: typing.Optional[float] = None
+        accuracy_top5: typing.Optional[float] = None
+        average_precision: typing.Optional[float] = None
+        mean_average_precision_30: typing.Optional[float] = None
+        mean_average_precision_50: typing.Optional[float] = None
+        mean_average_precision_75: typing.Optional[float] = None
 
     def execute(self, inputs):
         self._uvs_client = UVSClient(self.config.endpoint, self.config.api_key)
+
         dataset_name = f'dataset_{uuid.uuid4()}'
+        test_dataset_name = None
         logger.info(f"Uploading dataset to Azure Storage Blob. {dataset_name=}")
         self._upload_dataset(inputs.dataset, dataset_name, inputs.class_names)
 
+        if inputs.test_dataset:
+            test_dataset_name = f'{dataset_name}_test'
+            logger.info(f"Uploading test dataset to Azure Storage Blob. {test_dataset_name=}")
+            self._upload_dataset(inputs.test_dataset, test_dataset_name, inputs.class_names)
+
         model_name = f'model_{uuid.uuid4()}'
         logger.info(f"Training model. {model_name=}")
         start = time.time()
-        self._train_model(dataset_name, model_name)
+        self._train_model(dataset_name, model_name, test_dataset_name)
         logger.info(f"Training model finished. {model_name=}. Elapsed time: {time.time() - start:.2f} seconds")
         if not self.config.keep_dataset:
-            logger.info('Deleting dataset from Azure Storage Blob...')
+            logger.info(f"Deleting dataset from Azure Storage Blob...{dataset_name=}")
             self._delete_dataset(dataset_name)
+            if test_dataset_name:
+                logger.info(f"Deleting test dataset from Azure Storage Blob...{test_dataset_name=}")
+                self._delete_dataset(test_dataset_name)
+
+        if test_dataset_name:
+            evaluation_result = self._uvs_client.get_model(model_name)['modelPerformance']
+            logger.info(f"Evaluation result: {evaluation_result}")
+        else:
+            evaluation_result = {}
 
-        return self.Outputs(model_name=model_name)
+        return self.Outputs(model_name=model_name, accuracy_top1=evaluation_result.get('accuracyTop1'), accuracy_top5=evaluation_result.get('accuracyTop5'),
+                            average_precision=evaluation_result.get('averagePrecision'), mean_average_precision_30=evaluation_result.get('meanAveragePrecision30'),
+                            mean_average_precision_50=evaluation_result.get('meanAveragePrecision50'), mean_average_precision_75=evaluation_result.get('meanAveragePrecision75'))
 
     def dry_run(self, inputs):
         return self.Outputs(model_name=str(uuid.uuid4()))
 
     def _upload_dataset(self, dataset, dataset_name, class_names):
         container_client = ContainerClient.from_container_url(self.config.azure_storage_blob_container_url, credential=DefaultAzureCredential())
 
@@ -118,24 +143,27 @@
         container_client = ContainerClient.from_container_url(self.config.azure_storage_blob_container_url, credential=DefaultAzureCredential())
 
         for blob in container_client.list_blobs(name_starts_with=dataset_name):
             container_client.delete_blob(blob)
 
         self._uvs_client.unregister_dataset(dataset_name)
 
-    def _train_model(self, dataset_name, model_name):
-        self._uvs_client.create_model(dataset_name, model_name, self.config.task_type, self.config.budget_in_hours)
+    def _train_model(self, dataset_name, model_name, test_dataset_name):
+        self._uvs_client.create_model(dataset_name, model_name, self.config.task_type, self.config.budget_in_hours, test_dataset_name)
         logger.info(f"Training request sent. Waiting for training to complete... Training budget is {self.config.budget_in_hours} hours.")
-        status = None
-        while not status or status.lower() in ['notstarted', 'training']:
+        status = 'notstarted'
+        while status in ['notstarted', 'training']:
             time.sleep(60)
-            status = self._uvs_client.get_model_status(model_name)
+            model = self._uvs_client.get_model(model_name)
+            status = model['status'].lower()
 
-        if status.lower() == 'failed':
+        if status == 'failed':
             raise RuntimeError(f"Training failed. {model_name=}")
+        elif status in ['cancelling', 'cancelled']:
+            raise RuntimeError(f"Training cancelled. {model_name=}")
 
     @tenacity.retry(stop=tenacity.stop_after_attempt(5))
     def _upload_file(self, blob_name, data, content_type, container_client):
         try:
             blob_client = container_client.get_blob_client(blob_name)
             content_settings = ContentSettings(content_type=content_type)
             blob_client.upload_blob(data, content_settings=content_settings, timeout=300, overwrite=False)
@@ -153,28 +181,31 @@
         url = urllib.parse.urljoin(self._endpoint, f'/computervision/datasets/{dataset_name}?api-version=2023-04-01-preview')
         annotation_kind = {'classification_multiclass': 'imageClassification', 'object_detection': 'imageObjectDetection'}[task_type]
         response = requests.put(url, headers=self._headers, json={'annotationKind': annotation_kind, 'annotationFileUris': [file_url]}, timeout=60)
         response_json = response.json()
         logger.debug(f"API response: {response_json}")
         response.raise_for_status()
 
-    def create_model(self, dataset_name, model_name, task_type, budget_in_hours):
+    def create_model(self, dataset_name, model_name, task_type, budget_in_hours, test_dataset_name):
         url = urllib.parse.urljoin(self._endpoint, f'/computervision/models/{model_name}?api-version=2023-04-01-preview')
         model_kind = {'classification_multiclass': 'GenericClassifier', 'object_detection': 'GenericDetector'}[task_type]
-        response = requests.put(url, headers=self._headers,
-                                json={'trainingParameters': {'timeBudgetInHours': budget_in_hours, 'trainingDatasetName': dataset_name, 'modelKind': model_kind}}, timeout=60)
+        request_body = {'trainingParameters': {'timeBudgetInHours': budget_in_hours, 'trainingDatasetName': dataset_name, 'modelKind': model_kind}}
+        if test_dataset_name:
+            request_body['evaluationParameters'] = {'testDatasetName': test_dataset_name}
+
+        response = requests.put(url, headers=self._headers, json=request_body, timeout=60)
         response_json = response.json()
         logger.debug(f"API response: {response_json}")
         response.raise_for_status()
 
-    def get_model_status(self, model_name):
+    def get_model(self, model_name):
         url = urllib.parse.urljoin(self._endpoint, f'/computervision/models/{model_name}?api-version=2023-04-01-preview')
         response = requests.get(url, headers=self._headers, timeout=60)
         response_json = response.json()
         logger.debug(f"API response: {response_json}")
         response.raise_for_status()
-        return response_json['status']
+        return response_json
 
     def unregister_dataset(self, dataset_name):
         url = urllib.parse.urljoin(self._endpoint, f'/computervision/datasets/{dataset_name}?api-version=2023-04-01-preview')
         response = requests.delete(url, headers=self._headers, timeout=60)
         response.raise_for_status()
```

### Comparing `irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/PKG-INFO` & `irisml-tasks-azure-computervision-0.0.4/irisml_tasks_azure_computervision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-computervision
-Version: 0.0.3
+Version: 0.0.4
 Summary: Azure Computer Vision API tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-computervision
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-computervision-0.0.3/irisml_tasks_azure_computervision.egg-info/SOURCES.txt` & `irisml-tasks-azure-computervision-0.0.4/irisml_tasks_azure_computervision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/setup.cfg` & `irisml-tasks-azure-computervision-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-azure-computervision
-version = 0.0.3
+version = 0.0.4
 url = https://github.com/microsoft/irisml-tasks-azure-computervision
 description = Azure Computer Vision API tasks for IrisML
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_caption_model.py` & `irisml-tasks-azure-computervision-0.0.4/test/test_create_azure_computervision_caption_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_classification_model.py` & `irisml-tasks-azure-computervision-0.0.4/test/test_create_azure_computervision_classification_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.4/test/test_create_azure_computervision_custom_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,37 +3,55 @@
 import PIL.Image
 import torch
 from irisml.tasks.create_azure_computervision_custom_model import Task
 
 
 class TestCreateAzureComputervisionCustomModel(unittest.TestCase):
     def test_classification(self):
-        outputs = Task(Task.Config('https://example.com/', 'fake_api_key', 'fake_model_name', 'classification_multiclass')).execute(Task.Inputs(['label0', 'label1']))
-        self.assertIsInstance(outputs.model, torch.nn.Module)
-        model = outputs.model
-
-        with unittest.mock.patch('requests.post') as mock_post:
-            mock_post.return_value.json.side_effect = [
-                    {'customModelResult': {'tagsResult': {'values': [{'name': 'label0', 'confidence': 0.25}]}}},
-                    {'customModelResult': {'tagsResult': {'values': [{'name': 'label1', 'confidence': 0.5}]}}}
-                ]
-            model_outputs = model([PIL.Image.new('RGB', (100, 100)), PIL.Image.new('RGB', (128, 128))])
+        model_outputs = self._run_task('classification_multiclass', ['label0', 'label1'], [
+                {'customModelResult': {'tagsResult': {'values': [{'name': 'label0', 'confidence': 0.25}]}}},
+                {'customModelResult': {'tagsResult': {'values': [{'name': 'label1', 'confidence': 0.5}]}}}
+                ], [PIL.Image.new('RGB', (100, 100)), PIL.Image.new('RGB', (128, 128))])
 
         self.assertEqual(model_outputs.shape, torch.Size([2, 2]))
         self.assertEqual(model_outputs.tolist(), [[0.25, 0.0], [0.0, 0.5]])
 
     def test_object_detection(self):
-        outputs = Task(Task.Config('https://example.com/', 'fake_api_key', 'fake_model_name', 'object_detection')).execute(Task.Inputs(['label0', 'label1']))
-        self.assertIsInstance(outputs.model, torch.nn.Module)
-
-        with unittest.mock.patch('requests.post') as mock_post:
-            mock_post.return_value.json.side_effect = [
-                    {'metadata': {'width': 100, 'height': 100},
-                        'customModelResult': {'objectsResult': {'values': [{'boundingBox': {'x': 0, 'y': 0, 'w': 100, 'h': 100}, 'tags': [{'name': 'label0', 'confidence': 0.25}]}]}}},
-                    {'metadata': {'width': 200, 'height': 200},
-                        'customModelResult': {'objectsResult': {'values': [{'boundingBox': {'x': 0, 'y': 0, 'w': 100, 'h': 100}, 'tags': [{'name': 'label1', 'confidence': 0.5}]}]}}}
-                ]
-            model_outputs = outputs.model([PIL.Image.new('RGB', (100, 100)), PIL.Image.new('RGB', (200, 200))])
+        model_outputs = self._run_task('object_detection', ['label0', 'label1'], [
+            {'metadata': {'width': 100, 'height': 100},
+                'customModelResult': {'objectsResult': {'values': [{'boundingBox': {'x': 0, 'y': 0, 'w': 100, 'h': 100}, 'tags': [{'name': 'label0', 'confidence': 0.25}]}]}}},
+            {'metadata': {'width': 200, 'height': 200},
+                'customModelResult': {'objectsResult': {'values': [{'boundingBox': {'x': 0, 'y': 0, 'w': 100, 'h': 100}, 'tags': [{'name': 'label1', 'confidence': 0.5}]}]}}}
+            ], [PIL.Image.new('RGB', (100, 100)), PIL.Image.new('RGB', (200, 200))])
 
         self.assertEqual(len(model_outputs), 2)
         self.assertEqual(model_outputs[0].tolist(), [[0, 0.25, 0, 0, 1, 1]])
         self.assertEqual(model_outputs[1].tolist(), [[1, 0.5, 0, 0, 0.5, 0.5]])
+
+    def test_classification_with_error(self):
+        model_outputs = self._run_task('classification_multiclass', ['label0', 'label1'], [
+            {'customModelResult': {'tagsResult': {'values': [{'name': 'label0', 'confidence': 0.25}]}}},
+            RuntimeError('fake error')],
+            [PIL.Image.new('RGB', (100, 100)), PIL.Image.new('RGB', (128, 128))])
+
+        self.assertEqual(model_outputs.shape, torch.Size([2, 2]))
+        self.assertEqual(model_outputs.tolist(), [[0.25, 0.0], [0.0, 0.0]])
+
+    def test_object_detection_with_error(self):
+        model_outputs = self._run_task('object_detection', ['label0', 'label1'], [
+            {'metadata': {'width': 100, 'height': 100},
+                'customModelResult': {'objectsResult': {'values': [{'boundingBox': {'x': 0, 'y': 0, 'w': 100, 'h': 100}, 'tags': [{'name': 'label0', 'confidence': 0.25}]}]}}},
+            RuntimeError('fake error')],
+            [PIL.Image.new('RGB', (100, 100)), PIL.Image.new('RGB', (200, 200))])
+
+        self.assertEqual(len(model_outputs), 2)
+        self.assertEqual(model_outputs[0].tolist(), [[0, 0.25, 0, 0, 1, 1]])
+        self.assertEqual(model_outputs[1].shape, torch.Size([0, 6]))
+
+    def _run_task(self, task_type, class_names, responses, inputs):
+        outputs = Task(Task.Config('https://example.com/', 'fake_api_key', 'fake_model_name', task_type)).execute(Task.Inputs(class_names))
+        self.assertIsInstance(outputs.model, torch.nn.Module)
+        model = outputs.model
+
+        with unittest.mock.patch('requests.post') as mock_post:
+            mock_post.return_value.json.side_effect = responses
+            return model(inputs)
```

### Comparing `irisml-tasks-azure-computervision-0.0.3/test/test_create_azure_computervision_ocr_model.py` & `irisml-tasks-azure-computervision-0.0.4/test/test_create_azure_computervision_ocr_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/test/test_delete_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.4/test/test_delete_azure_computervision_custom_model.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-computervision-0.0.3/test/test_train_azure_computervision_custom_model.py` & `irisml-tasks-azure-computervision-0.0.4/test/test_train_azure_computervision_custom_model.py`

 * *Files identical despite different names*

