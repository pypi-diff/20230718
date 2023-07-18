# Comparing `tmp/brainchain-0.3.7.tar.gz` & `tmp/brainchain-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.3.7.tar", max compression
+gzip compressed data, was "brainchain-0.3.8.tar", max compression
```

## Comparing `brainchain-0.3.7.tar` & `brainchain-0.3.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.7/brainchain/.aider.chat.history.md
--rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.7/brainchain/.aider.input.history
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.7/brainchain/README.md
--rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.7/brainchain/__init__.py
--rw-r--r--   0        0        0     6423 2023-07-13 16:13:29.433811 brainchain-0.3.7/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.7/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.7/brainchain/coredata.py
--rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.7/brainchain/factcheck.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.7/brainchain/requirements.txt
--rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.7/brainchain/sales_intel.py
--rw-r--r--   0        0        0      532 2023-07-13 16:08:46.031550 brainchain-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     6082 2023-07-06 19:49:19.686228 brainchain-0.3.8/brainchain/.aider.chat.history.md
+-rw-r--r--   0        0        0     1874 2023-07-06 19:48:47.151645 brainchain-0.3.8/brainchain/.aider.input.history
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.3.8/brainchain/README.md
+-rw-r--r--   0        0        0      167 2023-07-06 20:56:21.342669 brainchain-0.3.8/brainchain/__init__.py
+-rw-r--r--   0        0        0    10418 2023-07-18 19:20:56.394998 brainchain-0.3.8/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.3.8/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2023-07-06 00:06:03.958510 brainchain-0.3.8/brainchain/coredata.py
+-rw-r--r--   0        0        0      652 2023-06-20 22:25:05.537757 brainchain-0.3.8/brainchain/factcheck.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.3.8/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6333 2023-07-06 18:26:20.604519 brainchain-0.3.8/brainchain/sales_intel.py
+-rw-r--r--   0        0        0      581 2023-07-18 19:20:56.395563 brainchain-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 brainchain-0.3.8/PKG-INFO
```

### Comparing `brainchain-0.3.7/brainchain/.aider.chat.history.md` & `brainchain-0.3.8/brainchain/.aider.chat.history.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.7/brainchain/.aider.input.history` & `brainchain-0.3.8/brainchain/.aider.input.history`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.7/brainchain/README.md` & `brainchain-0.3.8/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.7/brainchain/brainchain.py` & `brainchain-0.3.8/brainchain/brainchain.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import sys
 import json
 import requests
 from urllib.parse import quote
 from . import SalesIntel, FactCheck
 
 class Brainchain:
-    def __init__(self, env: str = "prod", api_key: str = os.environ["BRAINCHAIN_API_KEY"], service_url="https://brainchain--agent.modal.run/", salesintel_api_key=os.environ["SALESINTEL_API_KEY"]):
+    def __init__(self, env: str = "prod", api_key: str = os.environ["BRAINCHAIN_API_KEY"],
+                 service_url="https://brainchain--agent.modal.run/", salesintel_api_key=os.environ[
+                "SALESINTEL_API_KEY"]):
         self.api_key = api_key
         self.env = env
         self.fact_check_instance = FactCheck(environment=env)
         self.sales_intel_client = SalesIntel(salesintel_api_key)
         self.environments = ["prod", "dev"]
         self.services = {
             "agent": {
@@ -28,14 +30,20 @@
             "search": {
                 "prod": "https://brainchain--search.modal.run/",
                 "dev":  "https://brainchain--search-dev.modal.run/"
             },
             "electrolaser": {
                 "prod": "https://brainchain--electrolaser.modal.run/",
                 "dev": "https://brainchain--electrolaser-dev.modal.run/"
+            },
+            "weaviate_ingestion": {
+                "ingest": "https://brainchain--weaviate-ingestion-fastapi-app.modal.run/ingest/",
+                "query": "https://brainchain--weaviate-ingestion-fastapi-app.modal.run/query/",
+                "retrieve": "https://brainchain--weaviate-ingestion-fastapi-app.modal.run/retrieve/",
+                "preview": "https://brainchain--weaviate-ingestion-fastapi-app.modal.run/preview/"
             }
         }
 
     def fact_check(self, statement):
         return self.fact_check_instance.fact_check(statement)
 
     def search(self, query):
@@ -79,14 +87,103 @@
         response = requests.post(endpoint, headers=headers, json=payload)
 
         if response.status_code == 200:
             return response.json()
         else:
             response.raise_for_status()
 
+    def ingest(self, url: str):
+        """
+        Ingest a document into Weaviate, via URL. For now, this only works with PDFs. URL has to be publicly
+        accessible and point directly to the document, e.g. https://www.example.com/document.pdf.
+
+        Note: if you want to monitor the status of your doc's ingestion, look at the Modal logs for the
+        "weaviate-ingestion" app.
+
+        :param url: URL of document to ingest.
+        """
+        endpoint = self.services["weaviate_ingestion"]["ingest"]
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+        payload = {'url': url}
+        response = requests.post(endpoint, headers=headers, json=payload)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            response.raise_for_status()
+
+    def preview(self, class_name: str) -> dict:
+        """
+        Preview a Weaviate class/collection. By default, 3 items are returned (all possible fields in schema are
+        returned per item).
+
+        :param class_name: Name of class you want to preview.
+        :return: Dictionary containing metadata about the class + an `objects` list containing the items.
+        """
+        endpoint = self.services["weaviate_ingestion"]["preview"]
+        endpoint += class_name
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+        response = requests.get(endpoint, headers=headers)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            response.raise_for_status()
+
+    def query(self, concept: str, fields: str = 'title') -> dict[dict[list[dict[str, str]]]]:
+        """
+        Query Weaviate IngestDocs collection. By default, only titles are returned. If you want to add fields,
+        simply add them as a comma-separated string. For example, fields='title,authors,chunk'.
+
+        Example use:
+        ```
+        from brainchain import Brainchain
+        bc = Brainchain()
+        results = bc.query('water', fields='title,authors,chunk')
+        ```
+
+        :param concept: Query you want to send to Weaviate.
+        :param fields: Fields you want returned from Weaviate.
+        :return: Weaviate response.
+        """
+        endpoint = self.services["weaviate_ingestion"]["query"]
+        endpoint += concept
+
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+        if fields:
+            endpoint += f'?fields={fields}'
+            response = requests.get(endpoint, headers=headers)
+        else:
+            response = requests.get(endpoint, headers=headers)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            response.raise_for_status()
+
+    def retrieve(self, doc_uuid: str):
+        """
+        Retrieve a document from Weaviate IngestDocs collection, as stored in Amazon S3, via `doc_uuid`.
+
+        Example use:
+        ```
+        from brainchain import Brainchain
+        bc = Brainchain()
+        bc.retrieve(doc_uuid='ed2535defea94c03b1f5bb2e7486bb17')
+        >>> 'Congrats, you have downloaded your file locally!'
+        ```
+
+        :param doc_uuid: Document UUID as stored in Weaviate.
+        """
+        endpoint = self.services["weaviate_ingestion"]["retrieve"]
+        endpoint += doc_uuid
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+        response = requests.get(endpoint, headers=headers)
+        if response.status_code == 200:
+            return response.json()
+        else:
+            response.raise_for_status()
+
     def obtain_title(self, text_first_page: str = None):
         endpoint = self.services["prompt-completion-service"]["get_pdf_title"]
         payload = {}
 
         if text_first_page:
             payload["document_text"] = text_first_page
```

### Comparing `brainchain-0.3.7/brainchain/carnivore.py` & `brainchain-0.3.8/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.7/brainchain/coredata.py` & `brainchain-0.3.8/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.7/brainchain/factcheck.py` & `brainchain-0.3.8/brainchain/factcheck.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.7/brainchain/requirements.txt` & `brainchain-0.3.8/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.7/brainchain/sales_intel.py` & `brainchain-0.3.8/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.3.7/pyproject.toml` & `brainchain-0.3.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.3.7"
+version = "0.3.8"
 description = "Brainchain API client"
-authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
+authors = ["Arthur M. Collé <arthur@brainchain.ai>", "Audrey Lorberfeld <alorberfeld@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "2.31.0"
 promptlayer = "0.1.92"
 openai = "0.27.8"
 modal-client = "0.50.2627"
```

### Comparing `brainchain-0.3.7/PKG-INFO` & `brainchain-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.3.7
+Version: 0.3.8
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

