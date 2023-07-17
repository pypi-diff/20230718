# Comparing `tmp/databricks_vectorsearch_preview-0.13-py3-none-any.whl.zip` & `tmp/databricks_vectorsearch_preview-0.14-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18527 bytes, number of entries: 11
+Zip file size: 18551 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 04:20 databricks/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 04:20 databricks/vector_search/__init__.py
--rw-r--r--  2.0 unx    10087 b- defN 23-Jul-17 20:33 databricks/vector_search/client.py
+-rw-r--r--  2.0 unx    10033 b- defN 23-Jul-17 23:00 databricks/vector_search/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 04:20 databricks/vector_search/proto/__init__.py
 -rw-r--r--  2.0 unx    65338 b- defN 23-Jul-17 19:57 databricks/vector_search/proto/messages_pb2.py
 -rw-r--r--  2.0 unx    22870 b- defN 23-Jul-17 19:57 databricks/vector_search/proto/service_pb2.py
 -rw-r--r--  2.0 unx    38292 b- defN 23-Jul-17 19:57 databricks/vector_search/proto/taxonomy_pb2.py
--rw-r--r--  2.0 unx      570 b- defN 23-Jul-17 20:34 databricks_vectorsearch_preview-0.13.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 20:34 databricks_vectorsearch_preview-0.13.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-17 20:34 databricks_vectorsearch_preview-0.13.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1054 b- defN 23-Jul-17 20:34 databricks_vectorsearch_preview-0.13.dist-info/RECORD
-11 files, 138314 bytes uncompressed, 16687 bytes compressed:  87.9%
+-rw-r--r--  2.0 unx      570 b- defN 23-Jul-17 23:03 databricks_vectorsearch_preview-0.14.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 23:03 databricks_vectorsearch_preview-0.14.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-17 23:03 databricks_vectorsearch_preview-0.14.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Jul-17 23:03 databricks_vectorsearch_preview-0.14.dist-info/RECORD
+11 files, 138260 bytes uncompressed, 16711 bytes compressed:  87.9%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: databricks/vector_search/proto/service_pb2.py
 Comment: 
 
 Filename: databricks/vector_search/proto/taxonomy_pb2.py
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.13.dist-info/METADATA
+Filename: databricks_vectorsearch_preview-0.14.dist-info/METADATA
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.13.dist-info/WHEEL
+Filename: databricks_vectorsearch_preview-0.14.dist-info/WHEEL
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.13.dist-info/top_level.txt
+Filename: databricks_vectorsearch_preview-0.14.dist-info/top_level.txt
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.13.dist-info/RECORD
+Filename: databricks_vectorsearch_preview-0.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databricks/vector_search/client.py

```diff
@@ -1,39 +1,39 @@
 import json
 import logging
-from typing import List
+from typing import Optional, Dict, List
 
 import requests
 from google.protobuf.json_format import MessageToJson
 
 from databricks.vector_search.proto.messages_pb2 import (
     CreateVectorSearchCatalogRequest,
     CreateVectorSearchIndexRequest,
     QueryVectorSearchIndexRequest,
     VectorSearchIndexPipelineSpec,
 )
 
-logging.basicConfig(level=logging.WARNING)
-log = logging.getLogger("databricks.vector_search.client")
-log.setLevel(logging.INFO)
+# logging.basicConfig(level=logging.WARNING)
+# log = logging.getLogger("databricks.vector_search.client")
+# log.setLevel(logging.INFO)
 
 import requests
 from mlflow.utils import databricks_utils
 
 # Assign the class VectorSearchIndexPipelineSpec.VectorIndex to VectorIndex
 VectorIndex = VectorSearchIndexPipelineSpec.VectorIndex
 
 
 class VectorSearchClient:
     """
     Client for interacting with the Vector Search API for Databricks.
 
     Example usage:
 
-        client = VectorSearchClient(workspace_url="https://myworkspace.com", token="mytoken")
+        client = VectorSearchClient()
         response = client.create_catalog("my_catalog")
         print(response)
     """
 
     def __init__(self, workspace_url=None, token=None):
         """
         Initializes a VectorSearchClient instance.
@@ -59,15 +59,14 @@
             if self._workspace_url.endswith("/")
             else self._workspace_url
         )
         url = f"{cleaned_hostname}{endpoint}"
         response = requests.request(
             url=url, headers=headers, method=method, params=params, json=json
         )
-        log.info(response.text)
         return response.json()
 
     ### This method will create an vector search catalog in UC
     ### catalog will take 10 to 15 mins to get provisioned.
     ### before that any operation on the cluster will fail except get_cluster
     # catalog_name is the vector search catalog name to be created
     def create_catalog(self, catalog_name):
@@ -139,18 +138,15 @@
         :param index_column: Column that will be embedded as vectors and persisted in the index
         :param embedding_model_endpoint_name: Embedding model endpoint to use
 
         :return: The response from the API call.
 
         Example usage:
 
-        client = VectorSearchClient(workspace_url="https://myworkspace.com", token="mytoken")
-        vector_index = VectorIndex()
-        vector_index.column = "text"
-        vector_index.embedding_model_endpoint_name = "e5-large-v2"
+        client = VectorSearchClient()
         response = client.create_index(
             source_table_name="my_catalog.schema1.table1",
             dest_index_name="vector.schema1.table1_index",
             primary_key="doc_id",
             index_column="text",
             embedding_model_endpoint_name="e5-large-v2")
         print(response)
@@ -167,16 +163,14 @@
         index_request.index_pipeline_spec.dest_index = dest_index_name
         index_request.index_pipeline_spec.primary_key = primary_key
         index_request.index_pipeline_spec.vector_index.MergeFrom(vector_index_column)
         index_request.index_pipeline_spec.continuous.SetInParent()
 
         json_str = MessageToJson(index_request, preserving_proto_field_name=True)
 
-        log.info(json_str)
-
         return self._call_endpoint(
             "/api/2.0/vector-search/index", "POST", json=json.loads(json_str)
         )
 
     ### This method will get the index definition
     # index_name is the index name created under the online catalog, this must be in the format of <vector search catalog>.<schema>.<table>
     def get_index(self, index_name):
@@ -188,46 +182,56 @@
         :return: The response from the API call.
         """
         return self._call_endpoint(f"/api/2.0/vector-search/index/{index_name}", "GET")
 
     ### This method will perform a vector similarity search on an index
     # index_name is the index name created under the online catalog, this must be in the format of <vector search catalog>.<schema>.<table>
     # query_text is the query text
-    # filters_json is a json string
-    # k is the number of documents to be returned
+    # columns are the returned search results
+    # filter is a json object to filter the search results
+    # num_results is the number of documents to be returned
     def similarity_search(
-        self, index_name, query_text, filters_json, columns, num_results
+        self,
+        index_name: str,
+        query_text: str,
+        columns: List[str],
+        filter: Optional[Dict] = None,
+        num_results: int = 5
     ):
         """
         Performs a vector similarity search on the specified index.
 
         :param index_name: The name of the index.
         :param query_text: The query text for the search.
-        :param filters_json: The JSON string of filters for the search.
         :param columns: The columns to be returned in the search results.
-        :param num_results: The number of documents to be returned.
+        :param filter: The JSON object of filters for the search (optional).
+        :param num_results: The number of documents to be returned (optional).
 
         :return: The response from the API call.
 
         Example usage:
 
-        client = VectorSearchClient(workspace_url="https://myworkspace.com", token="mytoken")
-        response = client.similarity_search("vector.schema1.table1_index", "What is spark connect?", {"id NOT": ("10", "1")}, ["text", "source"], 3)
+        client = VectorSearchClient()
+        response = client.similarity_search(
+            index_name="vector.schema1.table1_index", 
+            query_text"What is spark connect?",
+            columns=["text", "source"],
+            filter={"id NOT": ("10", "1")},
+            num_results=3)
         print(response)
         """
         query_request = QueryVectorSearchIndexRequest()
         query_request.query = query_text
-        query_request.filters_json = json.dumps(filters_json)
+        if filter is not None:
+            query_request.filters_json = json.dumps(filter)
         query_request.columns.extend(columns)
         query_request.num_results = num_results
 
         json_str = MessageToJson(query_request, preserving_proto_field_name=True)
 
-        log.info(json_str)
-
         return self._call_endpoint(
             f"/api/2.0/vector-search/index/{index_name}/query",
             "GET",
             json=json.loads(json_str),
         )
 
     # index_name is the index name created under the online catalog, this must be in the format of <vector search catalog>.<schema>.<table>
```

## Comparing `databricks_vectorsearch_preview-0.13.dist-info/METADATA` & `databricks_vectorsearch_preview-0.14.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-vectorsearch-preview
-Version: 0.13
+Version: 0.14
 Summary: Databricks Vector Search Client
 Home-page: UNKNOWN
 Author: Databirkcs
 Author-email: feedback@databricks.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `databricks_vectorsearch_preview-0.13.dist-info/RECORD` & `databricks_vectorsearch_preview-0.14.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 databricks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databricks/vector_search/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-databricks/vector_search/client.py,sha256=lDmtRZW2tTG6kM00loRfqMIg2oAHGG8mNhpe-CirKB8,10087
+databricks/vector_search/client.py,sha256=17YTulzLthIJqj81vuFydQQevsY5GfPNUsWN8vP3Yao,10033
 databricks/vector_search/proto/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databricks/vector_search/proto/messages_pb2.py,sha256=z8DumqdRQrpXXNvREnZwCbNSGChRotuumEivwXMCVYQ,65338
 databricks/vector_search/proto/service_pb2.py,sha256=fprjawx10B1sao1YHwRYOZ-aGGHTG3pCykmrDBt8muY,22870
 databricks/vector_search/proto/taxonomy_pb2.py,sha256=YzToOng9nuUEtEe0th-7h8i_J3XjNeh7y3-n1syCEuA,38292
-databricks_vectorsearch_preview-0.13.dist-info/METADATA,sha256=RRrPzMYME4JMA2qi8L4JB0-At8H9aQ5AnbQfOFDKJlM,570
-databricks_vectorsearch_preview-0.13.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-databricks_vectorsearch_preview-0.13.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
-databricks_vectorsearch_preview-0.13.dist-info/RECORD,,
+databricks_vectorsearch_preview-0.14.dist-info/METADATA,sha256=i0kPHkByU7Jl1H3MKOvfUIS8fw_6ToHUSalB4akcbO0,570
+databricks_vectorsearch_preview-0.14.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+databricks_vectorsearch_preview-0.14.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
+databricks_vectorsearch_preview-0.14.dist-info/RECORD,,
```

