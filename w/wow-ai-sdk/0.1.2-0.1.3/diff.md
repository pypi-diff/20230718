# Comparing `tmp/wow_ai_sdk-0.1.2.tar.gz` & `tmp/wow_ai_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_sdk-0.1.2.tar", max compression
+gzip compressed data, was "wow_ai_sdk-0.1.3.tar", max compression
```

## Comparing `wow_ai_sdk-0.1.2.tar` & `wow_ai_sdk-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     7857 2023-03-15 03:37:59.294563 wow_ai_sdk-0.1.2/README.md
--rw-r--r--   0        0        0      262 2023-03-15 06:35:25.030908 wow_ai_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      149 2023-01-28 11:24:39.272410 wow_ai_sdk-0.1.2/wow_ai_sdk/__init__.py
--rw-r--r--   0        0        0     8869 2023-01-28 11:24:39.458541 wow_ai_sdk-0.1.2/wow_ai_sdk/client.py
--rw-r--r--   0        0        0     7914 2023-01-28 11:24:40.157550 wow_ai_sdk-0.1.2/wow_ai_sdk/data_manager.py
--rw-r--r--   0        0        0    65994 2023-01-28 11:24:41.665337 wow_ai_sdk-0.1.2/wow_ai_sdk/project.py
--rw-r--r--   0        0        0     1325 2023-01-28 11:24:40.436036 wow_ai_sdk-0.1.2/wow_ai_sdk/users.py
--rw-r--r--   0        0        0     4218 2023-01-28 11:24:40.801400 wow_ai_sdk-0.1.2/wow_ai_sdk/utils.py
--rw-r--r--   0        0        0     1889 2023-01-28 11:24:41.002364 wow_ai_sdk-0.1.2/wow_ai_sdk/workspaces.py
--rw-r--r--   0        0        0     8597 1970-01-01 00:00:00.000000 wow_ai_sdk-0.1.2/setup.py
--rw-r--r--   0        0        0     8289 1970-01-01 00:00:00.000000 wow_ai_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7857 2023-06-30 11:57:05.323031 wow_ai_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0      262 2023-07-18 02:55:48.257797 wow_ai_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-01-28 11:24:39.272410 wow_ai_sdk-0.1.3/wow_ai_sdk/__init__.py
+-rw-r--r--   0        0        0     8869 2023-01-28 11:24:39.458541 wow_ai_sdk-0.1.3/wow_ai_sdk/client.py
+-rw-r--r--   0        0        0     7914 2023-01-28 11:24:40.157550 wow_ai_sdk-0.1.3/wow_ai_sdk/data_manager.py
+-rw-r--r--   0        0        0    66648 2023-07-15 09:22:29.068399 wow_ai_sdk-0.1.3/wow_ai_sdk/project.py
+-rw-r--r--   0        0        0     1325 2023-01-28 11:24:40.436036 wow_ai_sdk-0.1.3/wow_ai_sdk/users.py
+-rw-r--r--   0        0        0     4218 2023-01-28 11:24:40.801400 wow_ai_sdk-0.1.3/wow_ai_sdk/utils.py
+-rw-r--r--   0        0        0     1889 2023-01-28 11:24:41.002364 wow_ai_sdk-0.1.3/wow_ai_sdk/workspaces.py
+-rw-r--r--   0        0        0     8289 1970-01-01 00:00:00.000000 wow_ai_sdk-0.1.3/PKG-INFO
```

### Comparing `wow_ai_sdk-0.1.2/README.md` & `wow_ai_sdk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.2/wow_ai_sdk/client.py` & `wow_ai_sdk-0.1.3/wow_ai_sdk/client.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.2/wow_ai_sdk/data_manager.py` & `wow_ai_sdk-0.1.3/wow_ai_sdk/data_manager.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.2/wow_ai_sdk/project.py` & `wow_ai_sdk-0.1.3/wow_ai_sdk/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -988,15 +988,27 @@
         ----------
         predictions: list of dicts
             List of dicts with predictions in the <a href="https://labelstud.io/guide/export.html#Label-Studio-JSON-format-of-annotated-tasks">
             Label Studio JSON format as for annotations</a>.
         """
         response = self.make_request('POST', f'/api/projects/{self.id}/import/predictions', json=predictions)
         return response.json()
+    def get_ml_backends(self):
+        """ List all configured ML backends for a specific project by ID.
+            Use the following cURL command:
+            curl https://localhost:8080/api/ml?project={project_id} -H 'Authorization: Token abc123'
 
+        Parameters
+        ----------
+        predictions: list of dicts
+            List of dicts with predictions in the <a href="https://labelstud.io/guide/export.html#Label-Studio-JSON-format-of-annotated-tasks">
+            Label Studio JSON format as for annotations</a>.
+        """
+        response = self.make_request('GET', f'/api/ml?project={self.id}', json={})
+        return response.json()
     def create_annotations_from_predictions(self, model_versions=None):
         """ Create annotations from all predictions that exist for project tasks from specific ML model versions.
 
         Parameters
         ----------
         model_versions: list or None
             Convert predictions with these model versions to annotations. If `None`, all existing model versions are used
```

### Comparing `wow_ai_sdk-0.1.2/wow_ai_sdk/users.py` & `wow_ai_sdk-0.1.3/wow_ai_sdk/users.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.2/wow_ai_sdk/utils.py` & `wow_ai_sdk-0.1.3/wow_ai_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.2/wow_ai_sdk/workspaces.py` & `wow_ai_sdk-0.1.3/wow_ai_sdk/workspaces.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.2/setup.py` & `wow_ai_sdk-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,195 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: wow-ai-sdk
+Version: 0.1.3
+Summary: 
+Author: TonyShark
+Author-email: quoi@wow-ai.inc
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-packages = \
-['wow_ai_sdk']
+---
+title: Python SDK Tutorial for WowDAO
+short: Python SDK Tutorial
+type: guide
+order: 675
+meta_title: WowDAO Python SDK Tutorial
+meta_description: Tutorial documentation for the WowDAO Python SDK that covers how and why to use the SDK to easily include data labeling project creation and annotated task parsing in your data pipeline python scripts for data science and machine learning projects.
+---
 
-package_data = \
-{'': ['*']}
+You can use the WowDAO Python SDK to make annotating data a more integrated part of your data science and machine learning pipelines. This software development kit (SDK) lets you call the WowDAO API directly from scripts using predefined classes and methods.
 
-setup_kwargs = {
-    'name': 'wow-ai-sdk',
-    'version': '0.1.2',
-    'description': '',
-    'long_description': '---\ntitle: Python SDK Tutorial for WowDAO\nshort: Python SDK Tutorial\ntype: guide\norder: 675\nmeta_title: WowDAO Python SDK Tutorial\nmeta_description: Tutorial documentation for the WowDAO Python SDK that covers how and why to use the SDK to easily include data labeling project creation and annotated task parsing in your data pipeline python scripts for data science and machine learning projects.\n---\n\nYou can use the WowDAO Python SDK to make annotating data a more integrated part of your data science and machine learning pipelines. This software development kit (SDK) lets you call the WowDAO API directly from scripts using predefined classes and methods.\n\nWith the WowDAO Python SDK, you can perform the following tasks in a Python script:\n\n- [Authenticate to the WowDAO API](#Start-using-the-WowDAO-Python-SDK)\n- [Create a WowDAO project](#Create-a-project-with-the-WowDAO-Python-SDK), including setting up a labeling configuration.\n- [Import tasks](#Import-tasks-with-the-WowDAO-Python-SDK).\n- [Manage pre-annotated tasks and model predictions](#Add-predictions-to-existing-tasks-with-the-WowDAO-Python-SDK).\n- [Connect to a cloud storage provider](https://github.com/heartexlabs/wow-ai-sdk/blob/master/examples/annotate_data_from_gcs/annotate_data_from_gcs.ipynb), such as Amazon S3, Microsoft Azure, or Google Cloud Services (GCS), to retrieve unlabeled tasks and store annotated tasks.\n- [Modify project settings](/sdk/project.html#wow_ai_sdk.project.Project.set_params), such as task sampling or the model version used to display predictions.\n\nSee the [full SDK reference documentation for all available modules](/sdk/index.html), or review the available [API endpoints](/api) for any tasks that the SDK does not cover.\n\n## Start using the WowDAO Python SDK\n\n1. Install the SDK:\n   `pip install wow-ai-sdk`\n2. In your Python script, do the following:\n   1. Import the SDK.\n   2. Define your API key and WowDAO URL (API key is available at _Account_ page).\n   3. Connect to the API.\n\n```python\n# Define the URL where WowDAO is accessible and the API key for your user account\nWOWAI_URL = \'http://localhost:8080\'\nAPI_KEY = \'d6f8a2622d39e9d89ff0dfef1a80ad877f4ee9e3\'\n\n# Import the SDK and the client module\nfrom wow_ai_sdk import Client\n\n# Connect to the WowDAO API and check the connection\nls = Client(url=WOWAI_URL, api_key=API_KEY)\nls.check_connection()\n```\n\n## Create a project with the WowDAO Python SDK\n\nCreate a project in WowDAO using the SDK. Specify the project title and the labeling configuration. Choose your labeling configuration based on the type of labeling that you wish to perform. See the available [templates for WowDAO projects](/templates), or set a blank configuration with `<View></View>`.\n\nFor example, create an audio transcription project in your Python code:\n\n```python\nproject = ls.start_project(\n    title=\'Object Detection with Bounding Boxes Project\',\n    label_config=\'\'\'\n    <View>\\n  <Image name=\\"image\\" value=\\"$image\\"/>\\n  <RectangleLabels name=\\"label\\" toName=\\"image\\">\\n    <Label value=\\"Airplane\\" background=\\"green\\"/>\\n    <Label value=\\"Car\\" background=\\"blue\\"/>\\n  </RectangleLabels>\\n</View>\\n\n    \'\'\'\n)\n```\n\nFor more about what you can do with the project module of the SDK, see the [project module SDK reference](/sdk/project.html).\n\n## Import tasks with the WowDAO Python SDK\n\nYou can import tasks from your script using the WowDAO Python SDK.\n\nFor a specific project, you can import tasks in [WowDAO JSON format](tasks.html#Basic-WowDAO-JSON-format) or [connect to cloud storage providers](https://github.com/heartexlabs/wow-ai-sdk/blob/master/examples/annotate_data_from_gcs/annotate_data_from_gcs.ipynb) and import image, audio, or video files directly.\n\n```python\nproject.import_tasks(\n    [\n        {\'image\': \'https://i.imgur.com/HaR6pIZ.jpeg\'},\n        {\'image\': \'https://i.imgur.com/WbISHgK.jpeg\'}\n    ]\n)\n```\n\nYou can also import predictions:\n\n- [Add predictions to an existing task](#Add-predictions-to-existing-tasks-with-the-WowDAO-Python-SDK)\n- [Import pre-annotated tasks](#Import-pre-annotated-tasks-into-WowDAO)\n\n### Add predictions to existing tasks with the WowDAO Python SDK\n\nYou can add predictions to existing tasks in WowDAO in your Python script.\n\nFor an existing simple image classification project, you can do the following to add predictions of "Dog" for image tasks that you retrieve:\n\n```python\ntask_ids = project.get_tasks_ids()\nproject.create_prediction(task_ids[0], result=\'Dog\', score=0.9)\n```\n\nFor complex cases, such as object detection with bounding boxes, you can specify structured results:\n\n```python\nproject.create_prediction(task_ids[1], result={"x": 10, "y": 20, "width": 30, "height": 40, "label": ["Dog"]}, score=0.9)\n```\n\nFor another example, see the [Jupyter notebook example of importing pre-annotated data](https://github.com/heartexlabs/wow-ai-sdk/blob/master/examples/import_preannotations/import_preannotations.ipynb).\n\n### Import pre-annotated tasks into WowDAO\n\nYou can also import predictions together with tasks as pre-annotated tasks. The SDK offers several ways that you can import pre-annotations into WowDAO.\n\nOne way is to import tasks in a simple JSON format, where one key in the JSON identifies the data object being labeled, and the other is the key containing the prediction.\n\nIn this example, import predictions for an image classification task:\n\n```python\nproject.import_tasks(\n    [{\'image\': f\'https://i.imgur.com/WbISHgK.jpeg\', \'label\': \'Car\'},\n    {\'image\': f\'https://i.imgur.com/HaR6pIZ.jpeg\', \'label\': \'Car\'}],\n    preannotated_from_fields=[\'label\']\n)\n```\n\nThe image is specified in the `image` key using a public URL, and the prediction is referenced in an arbitrary `pet` key, which is then specified in the `preannotated_from_fields()` method.\n\nFor more examples, see the [Jupyter notebook example of importing pre-annotated data](https://github.com/heartexlabs/wow-ai-sdk/blob/master/examples/import_preannotations/import_preannotations.ipynb).\n\n## Prepare and manage data with filters\n\nYou can also use the SDK to control how tasks appear in the data manager to annotators or reviewers. You can create custom filters and ordering for the tasks based on parameters that you specify with the SDK. This lets you have more granular control over which tasks in your dataset get labeled or reviewed, and in which order.\n\n### Prepare unlabeled data with filters\n\nFor example, you can create a filter to prepare tasks to be annotated. For example, if you want annotators to focus on tasks in the first 1000 tasks in a dataset that contain the word "possum" in the field "text" in the task data, do the following:\n\n```python\nfrom wow_ai_sdk.data_manager import Filters, Column, Type, Operator\n\nFilters.create(Filters.AND, [\n    Filters.item(\n        Column.id,\n        Operator.GREATER_OR_EQUAL,\n        Type.Number,\n        Filters.value(1)\n    ),\n        Filters.item(\n        Column.id,\n        Operator.LESS_OR_EQUAL,\n        Type.Number,\n        Filters.value(1000)\n    ),\n    Filters.item(\n        Column.data(text),\n        Operator.CONTAINS,\n        Type.String,\n        Filters.value("possum")\n    )\n])\n```\n\n### Manage annotations with filters\n\nFor example, to create a filter that displays only tasks with an ID greater than 42 or that were annotated between November 1, 2021, and now, do the following:\n\n```python\nfrom wow_ai_sdk.data_manager import Filters, Column, Type, Operator\n\nFilters.create(Filters.OR, [\n    Filters.item(\n        Column.id,\n        Operator.GREATER,\n        Type.Number,\n        Filters.value(42)\n    ),\n    Filters.item(\n        Column.completed_at,\n        Operator.IN,\n        Type.Datetime,\n        Filters.value(\n            datetime(2021, 11, 1),\n            datetime.now()\n        )\n    )\n])\n```\n\nYou can use this example filter to prepare completed tasks for review in WowDAO.ai\n',
-    'author': 'TonyShark',
-    'author_email': 'quoi@wow-ai.inc',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+With the WowDAO Python SDK, you can perform the following tasks in a Python script:
 
+- [Authenticate to the WowDAO API](#Start-using-the-WowDAO-Python-SDK)
+- [Create a WowDAO project](#Create-a-project-with-the-WowDAO-Python-SDK), including setting up a labeling configuration.
+- [Import tasks](#Import-tasks-with-the-WowDAO-Python-SDK).
+- [Manage pre-annotated tasks and model predictions](#Add-predictions-to-existing-tasks-with-the-WowDAO-Python-SDK).
+- [Connect to a cloud storage provider](https://github.com/heartexlabs/wow-ai-sdk/blob/master/examples/annotate_data_from_gcs/annotate_data_from_gcs.ipynb), such as Amazon S3, Microsoft Azure, or Google Cloud Services (GCS), to retrieve unlabeled tasks and store annotated tasks.
+- [Modify project settings](/sdk/project.html#wow_ai_sdk.project.Project.set_params), such as task sampling or the model version used to display predictions.
+
+See the [full SDK reference documentation for all available modules](/sdk/index.html), or review the available [API endpoints](/api) for any tasks that the SDK does not cover.
+
+## Start using the WowDAO Python SDK
+
+1. Install the SDK:
+   `pip install wow-ai-sdk`
+2. In your Python script, do the following:
+   1. Import the SDK.
+   2. Define your API key and WowDAO URL (API key is available at _Account_ page).
+   3. Connect to the API.
+
+```python
+# Define the URL where WowDAO is accessible and the API key for your user account
+WOWAI_URL = 'http://localhost:8080'
+API_KEY = 'd6f8a2622d39e9d89ff0dfef1a80ad877f4ee9e3'
+
+# Import the SDK and the client module
+from wow_ai_sdk import Client
+
+# Connect to the WowDAO API and check the connection
+ls = Client(url=WOWAI_URL, api_key=API_KEY)
+ls.check_connection()
+```
+
+## Create a project with the WowDAO Python SDK
+
+Create a project in WowDAO using the SDK. Specify the project title and the labeling configuration. Choose your labeling configuration based on the type of labeling that you wish to perform. See the available [templates for WowDAO projects](/templates), or set a blank configuration with `<View></View>`.
+
+For example, create an audio transcription project in your Python code:
+
+```python
+project = ls.start_project(
+    title='Object Detection with Bounding Boxes Project',
+    label_config='''
+    <View>\n  <Image name=\"image\" value=\"$image\"/>\n  <RectangleLabels name=\"label\" toName=\"image\">\n    <Label value=\"Airplane\" background=\"green\"/>\n    <Label value=\"Car\" background=\"blue\"/>\n  </RectangleLabels>\n</View>\n
+    '''
+)
+```
+
+For more about what you can do with the project module of the SDK, see the [project module SDK reference](/sdk/project.html).
+
+## Import tasks with the WowDAO Python SDK
+
+You can import tasks from your script using the WowDAO Python SDK.
+
+For a specific project, you can import tasks in [WowDAO JSON format](tasks.html#Basic-WowDAO-JSON-format) or [connect to cloud storage providers](https://github.com/heartexlabs/wow-ai-sdk/blob/master/examples/annotate_data_from_gcs/annotate_data_from_gcs.ipynb) and import image, audio, or video files directly.
+
+```python
+project.import_tasks(
+    [
+        {'image': 'https://i.imgur.com/HaR6pIZ.jpeg'},
+        {'image': 'https://i.imgur.com/WbISHgK.jpeg'}
+    ]
+)
+```
+
+You can also import predictions:
+
+- [Add predictions to an existing task](#Add-predictions-to-existing-tasks-with-the-WowDAO-Python-SDK)
+- [Import pre-annotated tasks](#Import-pre-annotated-tasks-into-WowDAO)
+
+### Add predictions to existing tasks with the WowDAO Python SDK
+
+You can add predictions to existing tasks in WowDAO in your Python script.
+
+For an existing simple image classification project, you can do the following to add predictions of "Dog" for image tasks that you retrieve:
+
+```python
+task_ids = project.get_tasks_ids()
+project.create_prediction(task_ids[0], result='Dog', score=0.9)
+```
+
+For complex cases, such as object detection with bounding boxes, you can specify structured results:
+
+```python
+project.create_prediction(task_ids[1], result={"x": 10, "y": 20, "width": 30, "height": 40, "label": ["Dog"]}, score=0.9)
+```
+
+For another example, see the [Jupyter notebook example of importing pre-annotated data](https://github.com/heartexlabs/wow-ai-sdk/blob/master/examples/import_preannotations/import_preannotations.ipynb).
+
+### Import pre-annotated tasks into WowDAO
+
+You can also import predictions together with tasks as pre-annotated tasks. The SDK offers several ways that you can import pre-annotations into WowDAO.
+
+One way is to import tasks in a simple JSON format, where one key in the JSON identifies the data object being labeled, and the other is the key containing the prediction.
+
+In this example, import predictions for an image classification task:
+
+```python
+project.import_tasks(
+    [{'image': f'https://i.imgur.com/WbISHgK.jpeg', 'label': 'Car'},
+    {'image': f'https://i.imgur.com/HaR6pIZ.jpeg', 'label': 'Car'}],
+    preannotated_from_fields=['label']
+)
+```
+
+The image is specified in the `image` key using a public URL, and the prediction is referenced in an arbitrary `pet` key, which is then specified in the `preannotated_from_fields()` method.
+
+For more examples, see the [Jupyter notebook example of importing pre-annotated data](https://github.com/heartexlabs/wow-ai-sdk/blob/master/examples/import_preannotations/import_preannotations.ipynb).
+
+## Prepare and manage data with filters
+
+You can also use the SDK to control how tasks appear in the data manager to annotators or reviewers. You can create custom filters and ordering for the tasks based on parameters that you specify with the SDK. This lets you have more granular control over which tasks in your dataset get labeled or reviewed, and in which order.
+
+### Prepare unlabeled data with filters
+
+For example, you can create a filter to prepare tasks to be annotated. For example, if you want annotators to focus on tasks in the first 1000 tasks in a dataset that contain the word "possum" in the field "text" in the task data, do the following:
+
+```python
+from wow_ai_sdk.data_manager import Filters, Column, Type, Operator
+
+Filters.create(Filters.AND, [
+    Filters.item(
+        Column.id,
+        Operator.GREATER_OR_EQUAL,
+        Type.Number,
+        Filters.value(1)
+    ),
+        Filters.item(
+        Column.id,
+        Operator.LESS_OR_EQUAL,
+        Type.Number,
+        Filters.value(1000)
+    ),
+    Filters.item(
+        Column.data(text),
+        Operator.CONTAINS,
+        Type.String,
+        Filters.value("possum")
+    )
+])
+```
+
+### Manage annotations with filters
+
+For example, to create a filter that displays only tasks with an ID greater than 42 or that were annotated between November 1, 2021, and now, do the following:
+
+```python
+from wow_ai_sdk.data_manager import Filters, Column, Type, Operator
+
+Filters.create(Filters.OR, [
+    Filters.item(
+        Column.id,
+        Operator.GREATER,
+        Type.Number,
+        Filters.value(42)
+    ),
+    Filters.item(
+        Column.completed_at,
+        Operator.IN,
+        Type.Datetime,
+        Filters.value(
+            datetime(2021, 11, 1),
+            datetime.now()
+        )
+    )
+])
+```
+
+You can use this example filter to prepare completed tasks for review in WowDAO.ai
 
-setup(**setup_kwargs)
```

