# Comparing `tmp/retake-0.1.8.tar.gz` & `tmp/retake-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retake-0.1.8.tar", max compression
+gzip compressed data, was "retake-0.1.9.tar", max compression
```

## Comparing `retake-0.1.8.tar` & `retake-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    10172 2023-07-16 17:39:33.445915 retake-0.1.8/LICENSE
--rw-r--r--   0        0        0     3136 2023-07-16 17:39:33.445915 retake-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/extract/__init__.py
--rw-r--r--   0        0        0      549 2023-07-16 17:39:33.445915 retake-0.1.8/core/extract/base.py
--rw-r--r--   0        0        0     2194 2023-07-16 17:39:33.445915 retake-0.1.8/core/extract/postgres.py
--rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/__init__.py
--rw-r--r--   0        0        0     1502 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/base.py
--rw-r--r--   0        0        0     5407 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/elasticsearch.py
--rw-r--r--   0        0        0      632 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/opensearch.py
--rw-r--r--   0        0        0     2707 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/pinecone.py
--rw-r--r--   0        0        0     2892 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/tests/test_pinecone.py
--rw-r--r--   0        0        0     2817 2023-07-16 17:39:33.445915 retake-0.1.8/core/load/weaviate.py
--rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/__init__.py
--rw-r--r--   0        0        0      996 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/embedding.py
--rw-r--r--   0        0        0     9040 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/pipeline.py
--rw-r--r--   0        0        0      629 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/realtime.py
--rw-r--r--   0        0        0     1438 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/sink.py
--rw-r--r--   0        0        0      453 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/source.py
--rw-r--r--   0        0        0     1823 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/target.py
--rw-r--r--   0        0        0       41 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/tests/test_pipeline.py
--rw-r--r--   0        0        0      853 2023-07-16 17:39:33.445915 retake-0.1.8/core/sdk/transform.py
--rw-r--r--   0        0        0        0 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/__init__.py
--rw-r--r--   0        0        0      192 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/base.py
--rw-r--r--   0        0        0      488 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/cohere.py
--rw-r--r--   0        0        0      323 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/custom.py
--rw-r--r--   0        0        0      463 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/openai.py
--rw-r--r--   0        0        0      415 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/sentence_transformers.py
--rw-r--r--   0        0        0     1198 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/tests/test_cohere.py
--rw-r--r--   0        0        0      629 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/tests/test_custom.py
--rw-r--r--   0        0        0     1002 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/tests/test_openai.py
--rw-r--r--   0        0        0     1180 2023-07-16 17:39:33.445915 retake-0.1.8/core/transform/tests/test_sentence_transformers.py
--rw-r--r--   0        0        0      965 2023-07-16 17:39:51.702107 retake-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      300 2023-07-16 17:39:33.449915 retake-0.1.8/retake/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 17:39:33.449915 retake-0.1.8/streams/__init__.py
--rw-r--r--   0        0        0     2722 2023-07-16 17:39:33.449915 retake-0.1.8/streams/app.py
--rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 retake-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    10172 2023-07-18 16:04:44.313640 retake-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3136 2023-07-18 16:04:44.313640 retake-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 16:04:44.313640 retake-0.1.9/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:04:44.313640 retake-0.1.9/core/extract/__init__.py
+-rw-r--r--   0        0        0      549 2023-07-18 16:04:44.313640 retake-0.1.9/core/extract/base.py
+-rw-r--r--   0        0        0     2194 2023-07-18 16:04:44.313640 retake-0.1.9/core/extract/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:04:44.313640 retake-0.1.9/core/load/__init__.py
+-rw-r--r--   0        0        0     1502 2023-07-18 16:04:44.313640 retake-0.1.9/core/load/base.py
+-rw-r--r--   0        0        0     5407 2023-07-18 16:04:44.313640 retake-0.1.9/core/load/elasticsearch.py
+-rw-r--r--   0        0        0      632 2023-07-18 16:04:44.313640 retake-0.1.9/core/load/opensearch.py
+-rw-r--r--   0        0        0     2707 2023-07-18 16:04:44.313640 retake-0.1.9/core/load/pinecone.py
+-rw-r--r--   0        0        0     2892 2023-07-18 16:04:44.313640 retake-0.1.9/core/load/tests/test_pinecone.py
+-rw-r--r--   0        0        0     2817 2023-07-18 16:04:44.313640 retake-0.1.9/core/load/weaviate.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:04:44.313640 retake-0.1.9/core/sdk/__init__.py
+-rw-r--r--   0        0        0      996 2023-07-18 16:04:44.313640 retake-0.1.9/core/sdk/embedding.py
+-rw-r--r--   0        0        0     9637 2023-07-18 16:04:44.313640 retake-0.1.9/core/sdk/pipeline.py
+-rw-r--r--   0        0        0      640 2023-07-18 16:04:44.313640 retake-0.1.9/core/sdk/realtime.py
+-rw-r--r--   0        0        0     1998 2023-07-18 16:04:44.313640 retake-0.1.9/core/sdk/sink.py
+-rw-r--r--   0        0        0      686 2023-07-18 16:04:44.313640 retake-0.1.9/core/sdk/source.py
+-rw-r--r--   0        0        0     1823 2023-07-18 16:04:44.313640 retake-0.1.9/core/sdk/target.py
+-rw-r--r--   0        0        0       41 2023-07-18 16:04:44.313640 retake-0.1.9/core/sdk/tests/test_pipeline.py
+-rw-r--r--   0        0        0      853 2023-07-18 16:04:44.313640 retake-0.1.9/core/sdk/transform.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/base.py
+-rw-r--r--   0        0        0      488 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/cohere.py
+-rw-r--r--   0        0        0      323 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/custom.py
+-rw-r--r--   0        0        0      463 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/openai.py
+-rw-r--r--   0        0        0      415 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/sentence_transformers.py
+-rw-r--r--   0        0        0     1198 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/tests/test_cohere.py
+-rw-r--r--   0        0        0      629 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/tests/test_custom.py
+-rw-r--r--   0        0        0     1002 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/tests/test_openai.py
+-rw-r--r--   0        0        0     1180 2023-07-18 16:04:44.313640 retake-0.1.9/core/transform/tests/test_sentence_transformers.py
+-rw-r--r--   0        0        0      965 2023-07-18 16:05:07.843202 retake-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      394 2023-07-18 16:04:44.321640 retake-0.1.9/retake/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:04:44.321640 retake-0.1.9/streams/__init__.py
+-rw-r--r--   0        0        0     5377 2023-07-18 16:04:44.321640 retake-0.1.9/streams/app.py
+-rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 retake-0.1.9/PKG-INFO
```

### Comparing `retake-0.1.8/LICENSE` & `retake-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/README.md` & `retake-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/extract/base.py` & `retake-0.1.9/core/extract/base.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/extract/postgres.py` & `retake-0.1.9/core/extract/postgres.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/load/base.py` & `retake-0.1.9/core/load/base.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/load/elasticsearch.py` & `retake-0.1.9/core/load/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/load/opensearch.py` & `retake-0.1.9/core/load/opensearch.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/load/pinecone.py` & `retake-0.1.9/core/load/pinecone.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/load/tests/test_pinecone.py` & `retake-0.1.9/core/load/tests/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/load/weaviate.py` & `retake-0.1.9/core/load/weaviate.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/sdk/embedding.py` & `retake-0.1.9/core/sdk/embedding.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/sdk/pipeline.py` & `retake-0.1.9/core/sdk/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 from core.extract.postgres import PostgresExtractor
 from core.transform.openai import OpenAIEmbedding as OpenAI
 from core.transform.sentence_transformers import (
     SentenceTransformerEmbedding as SentenceTransformer,
 )
 from core.transform.cohere import CohereEmbedding as Cohere
 from core.transform.custom import CustomEmbedding as Custom
-from streams.app import register_agents, start_worker
+from streams.app import (
+    register_connector_conf,
+    wait_for_config_success,
+    register_agents,
+    start_worker,
+)
 
 Source = Union[PostgresSource]
 Transform = Union[PostgresTransform]
 Embedding = Union[
     OpenAIEmbedding, SentenceTransformerEmbedding, CohereEmbedding, CustomEmbedding
 ]
 Sink = Union[ElasticSearchSink, PineconeSink, WeaviateSink]
@@ -41,15 +46,15 @@
 class Pipeline:
     def __init__(
         self,
         source: Source,
         sink: Sink,
         target: Target,
         embedding: Embedding,
-        transform: Optional[Transform] = None,
+        transform: Optional[Transform],
     ):
         self.source = source
         self.transform = transform
         self.embedding = embedding
         self.sink = sink
         self.target = target
 
@@ -219,29 +224,43 @@
                     metadata=metadata_list,
                 )
 
             progress_bar.update(BATCH_SIZE)
 
         progress_bar.close()
 
-    def pipe_real_time(self, realtime_server: RealtimeServer) -> None:
-        if not self.transform:
+    def create_real_time(self, server: RealtimeServer) -> None:
+        if self.transform is None:
+            raise ValueError(
+                "Transform expected but got None. Did you forget to provide a transform argument?"
+            )
+        index = self.target.index_name
+        db_schema_name = self.transform.schema_name
+        table_name = self.transform.relation
+
+        register_connector_conf(
+            server, index, db_schema_name, table_name, self.source, self.sink
+        )
+        wait_for_config_success(server)
+
+    def pipe_real_time(self, server: RealtimeServer) -> None:
+        if self.transform is None:
             raise ValueError(
                 "Transform expected but got None. Did you forget to provide a transform argument?"
             )
 
         index = self.target.index_name
         db_schema_name = self.transform.schema_name
-        relation = self.transform.relation
-        topic = f"{relation}.{db_schema_name}.{relation}"
+        table_name = self.transform.relation
+        topic = f"{table_name}.{db_schema_name}.{table_name}"
 
         worker = register_agents(
             topic,
             index,
-            realtime_server,
+            server,
             self.model.create_embeddings,
             self.transform.transform_func,
             self.transform.optional_metadata,
         )
         start_worker(worker)
 
     def teardown(self) -> None:
```

### Comparing `retake-0.1.8/core/sdk/realtime.py` & `retake-0.1.9/core/sdk/realtime.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from pydantic import BaseModel
 
-DEFAULT_BROKER_PORT = "9094"
-DEFAULT_SCHEMA_REGISTRY_PORT = "8081"
+DEFAULT_BROKER_PORT = 9094
+DEFAULT_SCHEMA_REGISTRY_PORT = 8081
 
 
 class RealtimeServer(BaseModel):
     host: str
-    broker_port: str = DEFAULT_BROKER_PORT
-    schema_registry_port: str = DEFAULT_SCHEMA_REGISTRY_PORT
+    broker_port: int = DEFAULT_BROKER_PORT
+    schema_registry_port: int = DEFAULT_SCHEMA_REGISTRY_PORT
     use_tls: bool = False  # TODO: make this default to True
 
     @property
     def broker_host(self) -> str:
-        return f"{self.host}:{self.broker_port}"
+        return f"{self.host}:{str(self.broker_port)}"
 
     @property
     def schema_registry_url(self) -> str:
         if self.use_tls:
-            return f"https://{self.host}:{self.schema_registry_port}"
+            return f"https://{self.host}:{str(self.schema_registry_port)}"
 
-        return f"http://{self.host}:{self.schema_registry_port}"
+        return f"http://{self.host}:{str(self.schema_registry_port)}"
```

### Comparing `retake-0.1.8/core/sdk/target.py` & `retake-0.1.9/core/sdk/target.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/sdk/transform.py` & `retake-0.1.9/core/sdk/transform.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/transform/tests/test_cohere.py` & `retake-0.1.9/core/transform/tests/test_cohere.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/transform/tests/test_custom.py` & `retake-0.1.9/core/transform/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/transform/tests/test_openai.py` & `retake-0.1.9/core/transform/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/core/transform/tests/test_sentence_transformers.py` & `retake-0.1.9/core/transform/tests/test_sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.8/pyproject.toml` & `retake-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retake"
-version = "0.1.8"
+version = "0.1.9"
 description = "Open Source Infrastructure for Vector Data Streams"
 authors = ["Ming Ying <ming.ying.nyc@gmail.com>", "Philippe Noël <philippemnoel@gmail.com>"]
 readme = "README.md"
 packages = [{include = "retake"}, {include = "core"}, {include = "streams"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `retake-0.1.8/PKG-INFO` & `retake-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retake
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Source Infrastructure for Vector Data Streams
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: retake Version: 0.1.8 Summary: Open Source
+Metadata-Version: 2.1 Name: retake Version: 0.1.9 Summary: Open Source
 Infrastructure for Vector Data Streams Author: Ming Ying Author-email:
 ming.ying.nyc@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: cohere (>=4.12.0,<5.0.0) Requires-
 Dist: confluent-kafka (>=2.2.0,<3.0.0) Requires-Dist: elasticsearch
 (>=8.8.2,<9.0.0) Requires-Dist: fastavro (>=1.8.0,<2.0.0) Requires-Dist: faust-
```

