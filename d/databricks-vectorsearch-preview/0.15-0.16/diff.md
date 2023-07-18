# Comparing `tmp/databricks_vectorsearch_preview-0.15-py3-none-any.whl.zip` & `tmp/databricks_vectorsearch_preview-0.16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 18585 bytes, number of entries: 11
+Zip file size: 20386 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 16:27 databricks/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 16:27 databricks/vector_search/__init__.py
 -rw-r--r--  2.0 unx    10267 b- defN 23-Jul-18 16:31 databricks/vector_search/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 16:27 databricks/vector_search/proto/__init__.py
--rw-r--r--  2.0 unx    65338 b- defN 23-Jul-18 16:27 databricks/vector_search/proto/messages_pb2.py
--rw-r--r--  2.0 unx    22870 b- defN 23-Jul-18 16:27 databricks/vector_search/proto/service_pb2.py
+-rw-r--r--  2.0 unx    76905 b- defN 23-Jul-18 21:29 databricks/vector_search/proto/messages_pb2.py
+-rw-r--r--  2.0 unx     9837 b- defN 23-Jul-18 21:32 databricks/vector_search/proto/service_pb2.py
 -rw-r--r--  2.0 unx    38292 b- defN 23-Jul-18 16:27 databricks/vector_search/proto/taxonomy_pb2.py
--rw-r--r--  2.0 unx      570 b- defN 23-Jul-18 16:32 databricks_vectorsearch_preview-0.15.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 16:32 databricks_vectorsearch_preview-0.15.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-18 16:32 databricks_vectorsearch_preview-0.15.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1054 b- defN 23-Jul-18 16:32 databricks_vectorsearch_preview-0.15.dist-info/RECORD
-11 files, 138494 bytes uncompressed, 16745 bytes compressed:  87.9%
+-rw-r--r--  2.0 unx    13028 b- defN 23-Jul-18 21:36 databricks/vector_search/proto/well_known_types_pb2.py
+-rw-r--r--  2.0 unx      570 b- defN 23-Jul-18 21:41 databricks_vectorsearch_preview-0.16.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 21:41 databricks_vectorsearch_preview-0.16.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-18 21:41 databricks_vectorsearch_preview-0.16.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Jul-18 21:41 databricks_vectorsearch_preview-0.16.dist-info/RECORD
+12 files, 150167 bytes uncompressed, 18362 bytes compressed:  87.8%
```

## zipnote {}

```diff
@@ -15,20 +15,23 @@
 
 Filename: databricks/vector_search/proto/service_pb2.py
 Comment: 
 
 Filename: databricks/vector_search/proto/taxonomy_pb2.py
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.15.dist-info/METADATA
+Filename: databricks/vector_search/proto/well_known_types_pb2.py
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.15.dist-info/WHEEL
+Filename: databricks_vectorsearch_preview-0.16.dist-info/METADATA
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.15.dist-info/top_level.txt
+Filename: databricks_vectorsearch_preview-0.16.dist-info/WHEEL
 Comment: 
 
-Filename: databricks_vectorsearch_preview-0.15.dist-info/RECORD
+Filename: databricks_vectorsearch_preview-0.16.dist-info/top_level.txt
+Comment: 
+
+Filename: databricks_vectorsearch_preview-0.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databricks/vector_search/proto/messages_pb2.py

```diff
@@ -10,25 +10,26 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from mlflow.protos import databricks_pb2 as databricks__pb2
 from mlflow.protos.scalapb import scalapb_pb2 as scalapb_dot_scalapb__pb2 
 from . import taxonomy_pb2 as compliance_dot_taxonomy_dot_taxonomy__pb2
+from . import well_known_types_pb2 as brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_well__known__types__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='brickindex-scheduler/brickindex-scheduler/api/proto/messages.proto',
   package='databricks.brickindexscheduler',
   syntax='proto2',
   serialized_options=b'\n,com.databricks.api.proto.brickindexscheduler\240\001\001\342?\'\020\001\032#com.databricks.managedcatalog.api._',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\nBbrickindex-scheduler/brickindex-scheduler/api/proto/messages.proto\x12\x1e\x64\x61tabricks.brickindexscheduler\x1a\x10\x64\x61tabricks.proto\x1a\x15scalapb/scalapb.proto\x1a\"compliance/taxonomy/taxonomy.proto\"9\n\x1dVectorSearchCatalogDefinition\x12\x18\n\x04name\x18\x01 \x01(\tB\x04\xc0\xd2#\x07R\x04name\"\xcb\x01\n\x19VectorSearchCatalogStatus\x12U\n\x05state\x18\x01 \x01(\x0e\x32?.databricks.brickindexscheduler.VectorSearchCatalogStatus.StateR\x05state\"W\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x11\n\rSTATE_UNKNOWN\x10\x01\x12\x0f\n\x0bSTATE_READY\x10\x02\x12\x13\n\x0fSTATE_NOT_READY\x10\x03\"\xf1\x01\n\x17VectorSearchIndexStatus\x12S\n\x05state\x18\x01 \x01(\x0e\x32=.databricks.brickindexscheduler.VectorSearchIndexStatus.StateR\x05state\x12\x34\n\x16indexed_document_count\x18\x02 \x01(\x03R\x14indexedDocumentCount\"K\n\x05State\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0b\n\x07\x44\x45LETED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x12\t\n\x05READY\x10\x03\x12\r\n\tNOT_READY\x10\x04\"\xb1\x01\n\x1bVectorSearchIndexDefinition\x12\x18\n\x04name\x18\x01 \x01(\tB\x04\xc0\xd2#\x07R\x04name\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32=.databricks.brickindexscheduler.VectorSearchIndexPipelineSpecR\x04spec\x12%\n\x0bpipeline_id\x18\x03 \x01(\tB\x04\xc0\xd2#\x07R\npipelineId\"\x8e\x01\n\'VectorSearchIndexDefinitionKeyValuePair\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12Q\n\x05value\x18\x02 \x01(\x0b\x32;.databricks.brickindexscheduler.VectorSearchIndexDefinitionR\x05value\"\x93\x06\n\x1dVectorSearchIndexPipelineSpec\x12\x80\x01\n\ncontinuous\x18\x01 \x01(\x0b\x32X.databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.ContinuousSchedulingPolicyB\x04\xc0\xd2#AH\x00R\ncontinuous\x12}\n\ttriggered\x18\x02 \x01(\x0b\x32W.databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.TriggeredSchedulingPolicyB\x04\xc0\xd2#AH\x00R\ttriggered\x12\x33\n\tsrc_table\x18\x08 \x01(\tB\x16\xe2?\x0f\n\rTableFullName\xc0\xd2#(R\x08srcTable\x12\x35\n\ndest_index\x18\t \x01(\tB\x16\xe2?\x0f\n\rTableFullName\xc0\xd2#(R\tdestIndex\x12%\n\x0bprimary_key\x18\n \x01(\tB\x04\xc0\xd2#\'R\nprimaryKey\x12l\n\x0cvector_index\x18\x0b \x01(\x0b\x32I.databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.VectorIndexR\x0bvectorIndex\x12)\n\rreset_version\x18\x0c \x01(\x03\x42\x04\xc0\xd2#KR\x0cresetVersion\x1a\x1c\n\x1a\x43ontinuousSchedulingPolicy\x1a\x1b\n\x19TriggeredSchedulingPolicy\x1at\n\x0bVectorIndex\x12\x1c\n\x06\x63olumn\x18\x01 \x01(\tB\x04\xc0\xd2#\'R\x06\x63olumn\x12G\n\x1d\x65mbedding_model_endpoint_name\x18\x02 \x01(\tB\x04\xc0\xd2#\x08R\x1a\x65mbeddingModelEndpointNameB\x13\n\x11scheduling_policy\"d\n\x19VectorSearchIndexDocument\x12\x1f\n\x0bprimary_key\x18\x01 \x01(\tR\nprimaryKey\x12\x14\n\x05score\x18\x02 \x01(\x02R\x05score\x12\x10\n\x03\x64oc\x18\x03 \x01(\tR\x03\x64oc\"v\n CreateVectorSearchCatalogRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:>\xe2?;\n9com.databricks.rpc.RPC[CreateVectorSearchCatalogResponse]\"\x91\x01\n!CreateVectorSearchCatalogResponse\x12l\n\x12\x63\x61talog_definition\x18\x01 \x01(\x0b\x32=.databricks.brickindexscheduler.VectorSearchCatalogDefinitionR\x11\x63\x61talogDefinition\"v\n DeleteVectorSearchCatalogRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:>\xe2?;\n9com.databricks.rpc.RPC[DeleteVectorSearchCatalogResponse]\"#\n!DeleteVectorSearchCatalogResponse\"p\n\x1dGetVectorSearchCatalogRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:;\xe2?8\n6com.databricks.rpc.RPC[GetVectorSearchCatalogResponse]\"\xf0\x01\n\x1eGetVectorSearchCatalogResponse\x12l\n\x12\x63\x61talog_definition\x18\x01 \x01(\x0b\x32=.databricks.brickindexscheduler.VectorSearchCatalogDefinitionR\x11\x63\x61talogDefinition\x12`\n\x0e\x63\x61talog_status\x18\x02 \x01(\x0b\x32\x39.databricks.brickindexscheduler.VectorSearchCatalogStatusR\rcatalogStatus\"\xcd\x01\n\x1e\x43reateVectorSearchIndexRequest\x12m\n\x13index_pipeline_spec\x18\x01 \x01(\x0b\x32=.databricks.brickindexscheduler.VectorSearchIndexPipelineSpecR\x11indexPipelineSpec:<\xe2?9\n7com.databricks.rpc.RPC[CreateVectorSearchIndexResponse]\"\x93\x01\n\x1f\x43reateVectorSearchIndexResponse\x12p\n\x10index_definition\x18\x01 \x01(\x0b\x32;.databricks.brickindexscheduler.VectorSearchIndexDefinitionB\x08\x90\xb5\x18\x01\xc0\xd2#\x17R\x0findexDefinition\"l\n\x1bGetVectorSearchIndexRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:9\xe2?6\n4com.databricks.rpc.RPC[GetVectorSearchIndexResponse]\"\xec\x01\n\x1cGetVectorSearchIndexResponse\x12p\n\x10index_definition\x18\x01 \x01(\x0b\x32;.databricks.brickindexscheduler.VectorSearchIndexDefinitionB\x08\x90\xb5\x18\x01\xc0\xd2#\x17R\x0findexDefinition\x12Z\n\x0cindex_status\x18\x02 \x01(\x0b\x32\x37.databricks.brickindexscheduler.VectorSearchIndexStatusR\x0bindexStatus\"\x83\x01\n\x1cListVectorSearchIndexRequest\x12\'\n\x0c\x63\x61talog_name\x18\x01 \x01(\tB\x04\xc0\xd2#\x07R\x0b\x63\x61talogName::\xe2?7\n5com.databricks.rpc.RPC[ListVectorSearchIndexResponse]\"\x9f\x01\n\x1dListVectorSearchIndexResponse\x12~\n\x11index_definitions\x18\x01 \x03(\x0b\x32G.databricks.brickindexscheduler.VectorSearchIndexDefinitionKeyValuePairB\x08\x98\xb5\x18\x01\xc0\xd2#\x17R\x10indexDefinitions\"r\n\x1e\x44\x65leteVectorSearchIndexRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:<\xe2?9\n7com.databricks.rpc.RPC[DeleteVectorSearchIndexResponse]\"!\n\x1f\x44\x65leteVectorSearchIndexResponse\"\xe4\x01\n\x1dQueryVectorSearchIndexRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\x12\x1f\n\x0bnum_results\x18\x03 \x01(\x05R\nnumResults\x12\x18\n\x07\x63olumns\x18\x04 \x03(\tR\x07\x63olumns\x12!\n\x0c\x66ilters_json\x18\x05 \x01(\tR\x0b\x66iltersJson:;\xe2?8\n6com.databricks.rpc.RPC[QueryVectorSearchIndexResponse]\"\x90\x01\n\x1eQueryVectorSearchIndexResponse\x12M\n\x04\x64ocs\x18\x01 \x03(\x0b\x32\x39.databricks.brickindexscheduler.VectorSearchIndexDocumentR\x04\x64ocs\x12\x1f\n\x0bnum_results\x18\x02 \x01(\x05R\nnumResults\"h\n\x18VectorSearchInternalInfo\x12\x1c\n\x06region\x18\x01 \x01(\tB\x04\xc0\xd2#\x19R\x06region\x12.\n\x10k8s_cluster_name\x18\x02 \x01(\tB\x04\xc0\xd2#\x19R\x0ek8sClusterNameB[\n,com.databricks.api.proto.brickindexscheduler\xa0\x01\x01\xe2?\'\x10\x01\x1a#com.databricks.managedcatalog.api._'
+  serialized_pb=b'\nBbrickindex-scheduler/brickindex-scheduler/api/proto/messages.proto\x12\x1e\x64\x61tabricks.brickindexscheduler\x1a\x10\x64\x61tabricks.proto\x1a\x15scalapb/scalapb.proto\x1a\"compliance/taxonomy/taxonomy.proto\x1aJbrickindex-scheduler/brickindex-scheduler/api/proto/well_known_types.proto\"9\n\x1dVectorSearchCatalogDefinition\x12\x18\n\x04name\x18\x01 \x01(\tB\x04\xc0\xd2#\x07R\x04name\"\xcb\x01\n\x19VectorSearchCatalogStatus\x12U\n\x05state\x18\x01 \x01(\x0e\x32?.databricks.brickindexscheduler.VectorSearchCatalogStatus.StateR\x05state\"W\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x11\n\rSTATE_UNKNOWN\x10\x01\x12\x0f\n\x0bSTATE_READY\x10\x02\x12\x13\n\x0fSTATE_NOT_READY\x10\x03\"\xf1\x01\n\x17VectorSearchIndexStatus\x12S\n\x05state\x18\x01 \x01(\x0e\x32=.databricks.brickindexscheduler.VectorSearchIndexStatus.StateR\x05state\x12\x34\n\x16indexed_document_count\x18\x02 \x01(\x03R\x14indexedDocumentCount\"K\n\x05State\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0b\n\x07\x44\x45LETED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x12\t\n\x05READY\x10\x03\x12\r\n\tNOT_READY\x10\x04\"\x8a\x01\n\x1bVectorSearchIndexDefinition\x12\x18\n\x04name\x18\x01 \x01(\tB\x04\xc0\xd2#\x07R\x04name\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32=.databricks.brickindexscheduler.VectorSearchIndexPipelineSpecR\x04spec\"\xef\x01\n\x15VectorSearchIndexItem\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x66\n\x10index_definition\x18\x02 \x01(\x0b\x32;.databricks.brickindexscheduler.VectorSearchIndexDefinitionR\x0findexDefinition\x12Z\n\x0cindex_status\x18\x03 \x01(\x0b\x32\x37.databricks.brickindexscheduler.VectorSearchIndexStatusR\x0bindexStatus\"\x93\x06\n\x1dVectorSearchIndexPipelineSpec\x12\x80\x01\n\ncontinuous\x18\x01 \x01(\x0b\x32X.databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.ContinuousSchedulingPolicyB\x04\xc0\xd2#AH\x00R\ncontinuous\x12}\n\ttriggered\x18\x02 \x01(\x0b\x32W.databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.TriggeredSchedulingPolicyB\x04\xc0\xd2#AH\x00R\ttriggered\x12\x33\n\tsrc_table\x18\x08 \x01(\tB\x16\xe2?\x0f\n\rTableFullName\xc0\xd2#(R\x08srcTable\x12\x35\n\ndest_index\x18\t \x01(\tB\x16\xe2?\x0f\n\rTableFullName\xc0\xd2#(R\tdestIndex\x12%\n\x0bprimary_key\x18\n \x01(\tB\x04\xc0\xd2#\'R\nprimaryKey\x12l\n\x0cvector_index\x18\x0b \x01(\x0b\x32I.databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.VectorIndexR\x0bvectorIndex\x12)\n\rreset_version\x18\x0c \x01(\x03\x42\x04\xc0\xd2#KR\x0cresetVersion\x1a\x1c\n\x1a\x43ontinuousSchedulingPolicy\x1a\x1b\n\x19TriggeredSchedulingPolicy\x1at\n\x0bVectorIndex\x12\x1c\n\x06\x63olumn\x18\x01 \x01(\tB\x04\xc0\xd2#\'R\x06\x63olumn\x12G\n\x1d\x65mbedding_model_endpoint_name\x18\x02 \x01(\tB\x04\xc0\xd2#\x08R\x1a\x65mbeddingModelEndpointNameB\x13\n\x11scheduling_policy\"d\n\x19VectorSearchIndexDocument\x12\x1f\n\x0bprimary_key\x18\x01 \x01(\tR\nprimaryKey\x12\x14\n\x05score\x18\x02 \x01(\x02R\x05score\x12\x10\n\x03\x64oc\x18\x03 \x01(\tR\x03\x64oc\"v\n CreateVectorSearchCatalogRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:>\xe2?;\n9com.databricks.rpc.RPC[CreateVectorSearchCatalogResponse]\"\x91\x01\n!CreateVectorSearchCatalogResponse\x12l\n\x12\x63\x61talog_definition\x18\x01 \x01(\x0b\x32=.databricks.brickindexscheduler.VectorSearchCatalogDefinitionR\x11\x63\x61talogDefinition\"v\n DeleteVectorSearchCatalogRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:>\xe2?;\n9com.databricks.rpc.RPC[DeleteVectorSearchCatalogResponse]\"#\n!DeleteVectorSearchCatalogResponse\"p\n\x1dGetVectorSearchCatalogRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:;\xe2?8\n6com.databricks.rpc.RPC[GetVectorSearchCatalogResponse]\"\xf0\x01\n\x1eGetVectorSearchCatalogResponse\x12l\n\x12\x63\x61talog_definition\x18\x01 \x01(\x0b\x32=.databricks.brickindexscheduler.VectorSearchCatalogDefinitionR\x11\x63\x61talogDefinition\x12`\n\x0e\x63\x61talog_status\x18\x02 \x01(\x0b\x32\x39.databricks.brickindexscheduler.VectorSearchCatalogStatusR\rcatalogStatus\"\xcd\x01\n\x1e\x43reateVectorSearchIndexRequest\x12m\n\x13index_pipeline_spec\x18\x01 \x01(\x0b\x32=.databricks.brickindexscheduler.VectorSearchIndexPipelineSpecR\x11indexPipelineSpec:<\xe2?9\n7com.databricks.rpc.RPC[CreateVectorSearchIndexResponse]\"\x93\x01\n\x1f\x43reateVectorSearchIndexResponse\x12p\n\x10index_definition\x18\x01 \x01(\x0b\x32;.databricks.brickindexscheduler.VectorSearchIndexDefinitionB\x08\x90\xb5\x18\x01\xc0\xd2#\x17R\x0findexDefinition\"l\n\x1bGetVectorSearchIndexRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:9\xe2?6\n4com.databricks.rpc.RPC[GetVectorSearchIndexResponse]\"\xec\x01\n\x1cGetVectorSearchIndexResponse\x12p\n\x10index_definition\x18\x01 \x01(\x0b\x32;.databricks.brickindexscheduler.VectorSearchIndexDefinitionB\x08\x90\xb5\x18\x01\xc0\xd2#\x17R\x0findexDefinition\x12Z\n\x0cindex_status\x18\x02 \x01(\x0b\x32\x37.databricks.brickindexscheduler.VectorSearchIndexStatusR\x0bindexStatus\"\x83\x01\n\x1cListVectorSearchIndexRequest\x12\'\n\x0c\x63\x61talog_name\x18\x01 \x01(\tB\x04\xc0\xd2#\x07R\x0b\x63\x61talogName::\xe2?7\n5com.databricks.rpc.RPC[ListVectorSearchIndexResponse]\"v\n\x1dListVectorSearchIndexResponse\x12U\n\x07indexes\x18\x01 \x03(\x0b\x32\x35.databricks.brickindexscheduler.VectorSearchIndexItemB\x04\xc0\xd2#\x17R\x07indexes\"r\n\x1e\x44\x65leteVectorSearchIndexRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name:<\xe2?9\n7com.databricks.rpc.RPC[DeleteVectorSearchIndexResponse]\"!\n\x1f\x44\x65leteVectorSearchIndexResponse\"\xe4\x01\n\x1dQueryVectorSearchIndexRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\x12\x1f\n\x0bnum_results\x18\x03 \x01(\x05R\nnumResults\x12\x18\n\x07\x63olumns\x18\x04 \x03(\tR\x07\x63olumns\x12!\n\x0c\x66ilters_json\x18\x05 \x01(\tR\x0b\x66iltersJson:;\xe2?8\n6com.databricks.rpc.RPC[QueryVectorSearchIndexResponse]\"\xd8\x01\n\x1eQueryVectorSearchIndexResponse\x12J\n\x08manifest\x18\x01 \x01(\x0b\x32..databricks.brickindexscheduler.ResultManifestR\x08manifest\x12\x42\n\x06result\x18\x02 \x01(\x0b\x32*.databricks.brickindexscheduler.ResultDataR\x06result\x12&\n\x0fnext_page_token\x18\x03 \x01(\tR\rnextPageToken\"}\n\nResultData\x12\x1b\n\trow_count\x18\x01 \x01(\x05R\x08rowCount\x12R\n\ndata_array\x18\x02 \x03(\x0b\x32\x33.databricks.brickindexscheduler.wellknown.ListValueR\tdataArray\"N\n\x08TypedRow\x12\x42\n\x06values\x18\x01 \x03(\x0b\x32*.databricks.brickindexscheduler.TypedValueR\x06values\"h\n\nTypedValue\x12\x12\n\x03\x62it\x18\x01 \x01(\x08H\x00R\x03\x62it\x12\x18\n\x06\x62igint\x18\x02 \x01(\x12H\x00R\x06\x62igint\x12\x12\n\x03num\x18\x03 \x01(\x01H\x00R\x03num\x12\x12\n\x03str\x18\x04 \x01(\tH\x00R\x03strB\x04\n\x02\x61s\"y\n\x0eResultManifest\x12!\n\x0c\x63olumn_count\x18\x01 \x01(\x05R\x0b\x63olumnCount\x12\x44\n\x07\x63olumns\x18\x02 \x03(\x0b\x32*.databricks.brickindexscheduler.ColumnInfoR\x07\x63olumns\"1\n\nColumnInfo\x12#\n\x04name\x18\x01 \x01(\tB\x0f\xe2?\x0c\n\nColumnNameR\x04name\"h\n\x18VectorSearchInternalInfo\x12\x1c\n\x06region\x18\x01 \x01(\tB\x04\xc0\xd2#\x19R\x06region\x12.\n\x10k8s_cluster_name\x18\x02 \x01(\tB\x04\xc0\xd2#\x19R\x0ek8sClusterNameB[\n,com.databricks.api.proto.brickindexscheduler\xa0\x01\x01\xe2?\'\x10\x01\x1a#com.databricks.managedcatalog.api._'
   ,
-  dependencies=[databricks__pb2.DESCRIPTOR,scalapb_dot_scalapb__pb2.DESCRIPTOR,compliance_dot_taxonomy_dot_taxonomy__pb2.DESCRIPTOR,])
+  dependencies=[databricks__pb2.DESCRIPTOR,scalapb_dot_scalapb__pb2.DESCRIPTOR,compliance_dot_taxonomy_dot_taxonomy__pb2.DESCRIPTOR,brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_well__known__types__pb2.DESCRIPTOR,])
 
 
 
 _VECTORSEARCHCATALOGSTATUS_STATE = _descriptor.EnumDescriptor(
   name='State',
   full_name='databricks.brickindexscheduler.VectorSearchCatalogStatus.State',
   filename=None,
@@ -54,16 +55,16 @@
       name='STATE_NOT_READY', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=355,
-  serialized_end=442,
+  serialized_start=431,
+  serialized_end=518,
 )
 _sym_db.RegisterEnumDescriptor(_VECTORSEARCHCATALOGSTATUS_STATE)
 
 _VECTORSEARCHINDEXSTATUS_STATE = _descriptor.EnumDescriptor(
   name='State',
   full_name='databricks.brickindexscheduler.VectorSearchIndexStatus.State',
   filename=None,
@@ -94,16 +95,16 @@
       name='NOT_READY', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=611,
-  serialized_end=686,
+  serialized_start=687,
+  serialized_end=762,
 )
 _sym_db.RegisterEnumDescriptor(_VECTORSEARCHINDEXSTATUS_STATE)
 
 
 _VECTORSEARCHCATALOGDEFINITION = _descriptor.Descriptor(
   name='VectorSearchCatalogDefinition',
   full_name='databricks.brickindexscheduler.VectorSearchCatalogDefinition',
@@ -127,16 +128,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=179,
-  serialized_end=236,
+  serialized_start=255,
+  serialized_end=312,
 )
 
 
 _VECTORSEARCHCATALOGSTATUS = _descriptor.Descriptor(
   name='VectorSearchCatalogStatus',
   full_name='databricks.brickindexscheduler.VectorSearchCatalogStatus',
   filename=None,
@@ -160,16 +161,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=239,
-  serialized_end=442,
+  serialized_start=315,
+  serialized_end=518,
 )
 
 
 _VECTORSEARCHINDEXSTATUS = _descriptor.Descriptor(
   name='VectorSearchIndexStatus',
   full_name='databricks.brickindexscheduler.VectorSearchIndexStatus',
   filename=None,
@@ -200,16 +201,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=445,
-  serialized_end=686,
+  serialized_start=521,
+  serialized_end=762,
 )
 
 
 _VECTORSEARCHINDEXDEFINITION = _descriptor.Descriptor(
   name='VectorSearchIndexDefinition',
   full_name='databricks.brickindexscheduler.VectorSearchIndexDefinition',
   filename=None,
@@ -227,74 +228,74 @@
     _descriptor.FieldDescriptor(
       name='spec', full_name='databricks.brickindexscheduler.VectorSearchIndexDefinition.spec', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, json_name='spec', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='pipeline_id', full_name='databricks.brickindexscheduler.VectorSearchIndexDefinition.pipeline_id', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\300\322#\007', json_name='pipelineId', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=689,
-  serialized_end=866,
+  serialized_start=765,
+  serialized_end=903,
 )
 
 
-_VECTORSEARCHINDEXDEFINITIONKEYVALUEPAIR = _descriptor.Descriptor(
-  name='VectorSearchIndexDefinitionKeyValuePair',
-  full_name='databricks.brickindexscheduler.VectorSearchIndexDefinitionKeyValuePair',
+_VECTORSEARCHINDEXITEM = _descriptor.Descriptor(
+  name='VectorSearchIndexItem',
+  full_name='databricks.brickindexscheduler.VectorSearchIndexItem',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='databricks.brickindexscheduler.VectorSearchIndexDefinitionKeyValuePair.key', index=0,
+      name='name', full_name='databricks.brickindexscheduler.VectorSearchIndexItem.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='key', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=None, json_name='name', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='databricks.brickindexscheduler.VectorSearchIndexDefinitionKeyValuePair.value', index=1,
+      name='index_definition', full_name='databricks.brickindexscheduler.VectorSearchIndexItem.index_definition', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='value', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=None, json_name='indexDefinition', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='index_status', full_name='databricks.brickindexscheduler.VectorSearchIndexItem.index_status', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='indexStatus', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=869,
-  serialized_end=1011,
+  serialized_start=906,
+  serialized_end=1145,
 )
 
 
 _VECTORSEARCHINDEXPIPELINESPEC_CONTINUOUSSCHEDULINGPOLICY = _descriptor.Descriptor(
   name='ContinuousSchedulingPolicy',
   full_name='databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.ContinuousSchedulingPolicy',
   filename=None,
@@ -310,16 +311,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1605,
-  serialized_end=1633,
+  serialized_start=1739,
+  serialized_end=1767,
 )
 
 _VECTORSEARCHINDEXPIPELINESPEC_TRIGGEREDSCHEDULINGPOLICY = _descriptor.Descriptor(
   name='TriggeredSchedulingPolicy',
   full_name='databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.TriggeredSchedulingPolicy',
   filename=None,
   file=DESCRIPTOR,
@@ -334,16 +335,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1635,
-  serialized_end=1662,
+  serialized_start=1769,
+  serialized_end=1796,
 )
 
 _VECTORSEARCHINDEXPIPELINESPEC_VECTORINDEX = _descriptor.Descriptor(
   name='VectorIndex',
   full_name='databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.VectorIndex',
   filename=None,
   file=DESCRIPTOR,
@@ -372,16 +373,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1664,
-  serialized_end=1780,
+  serialized_start=1798,
+  serialized_end=1914,
 )
 
 _VECTORSEARCHINDEXPIPELINESPEC = _descriptor.Descriptor(
   name='VectorSearchIndexPipelineSpec',
   full_name='databricks.brickindexscheduler.VectorSearchIndexPipelineSpec',
   filename=None,
   file=DESCRIPTOR,
@@ -450,16 +451,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='scheduling_policy', full_name='databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.scheduling_policy',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=1014,
-  serialized_end=1801,
+  serialized_start=1148,
+  serialized_end=1935,
 )
 
 
 _VECTORSEARCHINDEXDOCUMENT = _descriptor.Descriptor(
   name='VectorSearchIndexDocument',
   full_name='databricks.brickindexscheduler.VectorSearchIndexDocument',
   filename=None,
@@ -496,16 +497,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1803,
-  serialized_end=1903,
+  serialized_start=1937,
+  serialized_end=2037,
 )
 
 
 _CREATEVECTORSEARCHCATALOGREQUEST = _descriptor.Descriptor(
   name='CreateVectorSearchCatalogRequest',
   full_name='databricks.brickindexscheduler.CreateVectorSearchCatalogRequest',
   filename=None,
@@ -528,16 +529,16 @@
   ],
   serialized_options=b'\342?;\n9com.databricks.rpc.RPC[CreateVectorSearchCatalogResponse]',
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1905,
-  serialized_end=2023,
+  serialized_start=2039,
+  serialized_end=2157,
 )
 
 
 _CREATEVECTORSEARCHCATALOGRESPONSE = _descriptor.Descriptor(
   name='CreateVectorSearchCatalogResponse',
   full_name='databricks.brickindexscheduler.CreateVectorSearchCatalogResponse',
   filename=None,
@@ -560,16 +561,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2026,
-  serialized_end=2171,
+  serialized_start=2160,
+  serialized_end=2305,
 )
 
 
 _DELETEVECTORSEARCHCATALOGREQUEST = _descriptor.Descriptor(
   name='DeleteVectorSearchCatalogRequest',
   full_name='databricks.brickindexscheduler.DeleteVectorSearchCatalogRequest',
   filename=None,
@@ -592,16 +593,16 @@
   ],
   serialized_options=b'\342?;\n9com.databricks.rpc.RPC[DeleteVectorSearchCatalogResponse]',
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2173,
-  serialized_end=2291,
+  serialized_start=2307,
+  serialized_end=2425,
 )
 
 
 _DELETEVECTORSEARCHCATALOGRESPONSE = _descriptor.Descriptor(
   name='DeleteVectorSearchCatalogResponse',
   full_name='databricks.brickindexscheduler.DeleteVectorSearchCatalogResponse',
   filename=None,
@@ -617,16 +618,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2293,
-  serialized_end=2328,
+  serialized_start=2427,
+  serialized_end=2462,
 )
 
 
 _GETVECTORSEARCHCATALOGREQUEST = _descriptor.Descriptor(
   name='GetVectorSearchCatalogRequest',
   full_name='databricks.brickindexscheduler.GetVectorSearchCatalogRequest',
   filename=None,
@@ -649,16 +650,16 @@
   ],
   serialized_options=b'\342?8\n6com.databricks.rpc.RPC[GetVectorSearchCatalogResponse]',
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2330,
-  serialized_end=2442,
+  serialized_start=2464,
+  serialized_end=2576,
 )
 
 
 _GETVECTORSEARCHCATALOGRESPONSE = _descriptor.Descriptor(
   name='GetVectorSearchCatalogResponse',
   full_name='databricks.brickindexscheduler.GetVectorSearchCatalogResponse',
   filename=None,
@@ -688,16 +689,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2445,
-  serialized_end=2685,
+  serialized_start=2579,
+  serialized_end=2819,
 )
 
 
 _CREATEVECTORSEARCHINDEXREQUEST = _descriptor.Descriptor(
   name='CreateVectorSearchIndexRequest',
   full_name='databricks.brickindexscheduler.CreateVectorSearchIndexRequest',
   filename=None,
@@ -720,16 +721,16 @@
   ],
   serialized_options=b'\342?9\n7com.databricks.rpc.RPC[CreateVectorSearchIndexResponse]',
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2688,
-  serialized_end=2893,
+  serialized_start=2822,
+  serialized_end=3027,
 )
 
 
 _CREATEVECTORSEARCHINDEXRESPONSE = _descriptor.Descriptor(
   name='CreateVectorSearchIndexResponse',
   full_name='databricks.brickindexscheduler.CreateVectorSearchIndexResponse',
   filename=None,
@@ -752,16 +753,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2896,
-  serialized_end=3043,
+  serialized_start=3030,
+  serialized_end=3177,
 )
 
 
 _GETVECTORSEARCHINDEXREQUEST = _descriptor.Descriptor(
   name='GetVectorSearchIndexRequest',
   full_name='databricks.brickindexscheduler.GetVectorSearchIndexRequest',
   filename=None,
@@ -784,16 +785,16 @@
   ],
   serialized_options=b'\342?6\n4com.databricks.rpc.RPC[GetVectorSearchIndexResponse]',
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3045,
-  serialized_end=3153,
+  serialized_start=3179,
+  serialized_end=3287,
 )
 
 
 _GETVECTORSEARCHINDEXRESPONSE = _descriptor.Descriptor(
   name='GetVectorSearchIndexResponse',
   full_name='databricks.brickindexscheduler.GetVectorSearchIndexResponse',
   filename=None,
@@ -823,16 +824,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3156,
-  serialized_end=3392,
+  serialized_start=3290,
+  serialized_end=3526,
 )
 
 
 _LISTVECTORSEARCHINDEXREQUEST = _descriptor.Descriptor(
   name='ListVectorSearchIndexRequest',
   full_name='databricks.brickindexscheduler.ListVectorSearchIndexRequest',
   filename=None,
@@ -855,48 +856,48 @@
   ],
   serialized_options=b'\342?7\n5com.databricks.rpc.RPC[ListVectorSearchIndexResponse]',
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3395,
-  serialized_end=3526,
+  serialized_start=3529,
+  serialized_end=3660,
 )
 
 
 _LISTVECTORSEARCHINDEXRESPONSE = _descriptor.Descriptor(
   name='ListVectorSearchIndexResponse',
   full_name='databricks.brickindexscheduler.ListVectorSearchIndexResponse',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='index_definitions', full_name='databricks.brickindexscheduler.ListVectorSearchIndexResponse.index_definitions', index=0,
+      name='indexes', full_name='databricks.brickindexscheduler.ListVectorSearchIndexResponse.indexes', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=b'\230\265\030\001\300\322#\027', json_name='indexDefinitions', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=b'\300\322#\027', json_name='indexes', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3529,
-  serialized_end=3688,
+  serialized_start=3662,
+  serialized_end=3780,
 )
 
 
 _DELETEVECTORSEARCHINDEXREQUEST = _descriptor.Descriptor(
   name='DeleteVectorSearchIndexRequest',
   full_name='databricks.brickindexscheduler.DeleteVectorSearchIndexRequest',
   filename=None,
@@ -919,16 +920,16 @@
   ],
   serialized_options=b'\342?9\n7com.databricks.rpc.RPC[DeleteVectorSearchIndexResponse]',
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3690,
-  serialized_end=3804,
+  serialized_start=3782,
+  serialized_end=3896,
 )
 
 
 _DELETEVECTORSEARCHINDEXRESPONSE = _descriptor.Descriptor(
   name='DeleteVectorSearchIndexResponse',
   full_name='databricks.brickindexscheduler.DeleteVectorSearchIndexResponse',
   filename=None,
@@ -944,16 +945,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3806,
-  serialized_end=3839,
+  serialized_start=3898,
+  serialized_end=3931,
 )
 
 
 _QUERYVECTORSEARCHINDEXREQUEST = _descriptor.Descriptor(
   name='QueryVectorSearchIndexRequest',
   full_name='databricks.brickindexscheduler.QueryVectorSearchIndexRequest',
   filename=None,
@@ -1004,55 +1005,262 @@
   ],
   serialized_options=b'\342?8\n6com.databricks.rpc.RPC[QueryVectorSearchIndexResponse]',
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3842,
-  serialized_end=4070,
+  serialized_start=3934,
+  serialized_end=4162,
 )
 
 
 _QUERYVECTORSEARCHINDEXRESPONSE = _descriptor.Descriptor(
   name='QueryVectorSearchIndexResponse',
   full_name='databricks.brickindexscheduler.QueryVectorSearchIndexResponse',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='docs', full_name='databricks.brickindexscheduler.QueryVectorSearchIndexResponse.docs', index=0,
+      name='manifest', full_name='databricks.brickindexscheduler.QueryVectorSearchIndexResponse.manifest', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='manifest', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='result', full_name='databricks.brickindexscheduler.QueryVectorSearchIndexResponse.result', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='result', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='next_page_token', full_name='databricks.brickindexscheduler.QueryVectorSearchIndexResponse.next_page_token', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='nextPageToken', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4165,
+  serialized_end=4381,
+)
+
+
+_RESULTDATA = _descriptor.Descriptor(
+  name='ResultData',
+  full_name='databricks.brickindexscheduler.ResultData',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='row_count', full_name='databricks.brickindexscheduler.ResultData.row_count', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='rowCount', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='data_array', full_name='databricks.brickindexscheduler.ResultData.data_array', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='dataArray', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4383,
+  serialized_end=4508,
+)
+
+
+_TYPEDROW = _descriptor.Descriptor(
+  name='TypedRow',
+  full_name='databricks.brickindexscheduler.TypedRow',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='values', full_name='databricks.brickindexscheduler.TypedRow.values', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='docs', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=None, json_name='values', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4510,
+  serialized_end=4588,
+)
+
+
+_TYPEDVALUE = _descriptor.Descriptor(
+  name='TypedValue',
+  full_name='databricks.brickindexscheduler.TypedValue',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
     _descriptor.FieldDescriptor(
-      name='num_results', full_name='databricks.brickindexscheduler.QueryVectorSearchIndexResponse.num_results', index=1,
-      number=2, type=5, cpp_type=1, label=1,
+      name='bit', full_name='databricks.brickindexscheduler.TypedValue.bit', index=0,
+      number=1, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='bit', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='bigint', full_name='databricks.brickindexscheduler.TypedValue.bigint', index=1,
+      number=2, type=18, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='numResults', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+      serialized_options=None, json_name='bigint', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='num', full_name='databricks.brickindexscheduler.TypedValue.num', index=2,
+      number=3, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='num', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='str', full_name='databricks.brickindexscheduler.TypedValue.str', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='str', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
+    _descriptor.OneofDescriptor(
+      name='as', full_name='databricks.brickindexscheduler.TypedValue.as',
+      index=0, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=4073,
-  serialized_end=4217,
+  serialized_start=4590,
+  serialized_end=4694,
+)
+
+
+_RESULTMANIFEST = _descriptor.Descriptor(
+  name='ResultManifest',
+  full_name='databricks.brickindexscheduler.ResultManifest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='column_count', full_name='databricks.brickindexscheduler.ResultManifest.column_count', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='columnCount', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='columns', full_name='databricks.brickindexscheduler.ResultManifest.columns', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, json_name='columns', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4696,
+  serialized_end=4817,
+)
+
+
+_COLUMNINFO = _descriptor.Descriptor(
+  name='ColumnInfo',
+  full_name='databricks.brickindexscheduler.ColumnInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='databricks.brickindexscheduler.ColumnInfo.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=b'\342?\014\n\nColumnName', json_name='name', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4819,
+  serialized_end=4868,
 )
 
 
 _VECTORSEARCHINTERNALINFO = _descriptor.Descriptor(
   name='VectorSearchInternalInfo',
   full_name='databricks.brickindexscheduler.VectorSearchInternalInfo',
   filename=None,
@@ -1082,24 +1290,25 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4219,
-  serialized_end=4323,
+  serialized_start=4870,
+  serialized_end=4974,
 )
 
 _VECTORSEARCHCATALOGSTATUS.fields_by_name['state'].enum_type = _VECTORSEARCHCATALOGSTATUS_STATE
 _VECTORSEARCHCATALOGSTATUS_STATE.containing_type = _VECTORSEARCHCATALOGSTATUS
 _VECTORSEARCHINDEXSTATUS.fields_by_name['state'].enum_type = _VECTORSEARCHINDEXSTATUS_STATE
 _VECTORSEARCHINDEXSTATUS_STATE.containing_type = _VECTORSEARCHINDEXSTATUS
 _VECTORSEARCHINDEXDEFINITION.fields_by_name['spec'].message_type = _VECTORSEARCHINDEXPIPELINESPEC
-_VECTORSEARCHINDEXDEFINITIONKEYVALUEPAIR.fields_by_name['value'].message_type = _VECTORSEARCHINDEXDEFINITION
+_VECTORSEARCHINDEXITEM.fields_by_name['index_definition'].message_type = _VECTORSEARCHINDEXDEFINITION
+_VECTORSEARCHINDEXITEM.fields_by_name['index_status'].message_type = _VECTORSEARCHINDEXSTATUS
 _VECTORSEARCHINDEXPIPELINESPEC_CONTINUOUSSCHEDULINGPOLICY.containing_type = _VECTORSEARCHINDEXPIPELINESPEC
 _VECTORSEARCHINDEXPIPELINESPEC_TRIGGEREDSCHEDULINGPOLICY.containing_type = _VECTORSEARCHINDEXPIPELINESPEC
 _VECTORSEARCHINDEXPIPELINESPEC_VECTORINDEX.containing_type = _VECTORSEARCHINDEXPIPELINESPEC
 _VECTORSEARCHINDEXPIPELINESPEC.fields_by_name['continuous'].message_type = _VECTORSEARCHINDEXPIPELINESPEC_CONTINUOUSSCHEDULINGPOLICY
 _VECTORSEARCHINDEXPIPELINESPEC.fields_by_name['triggered'].message_type = _VECTORSEARCHINDEXPIPELINESPEC_TRIGGEREDSCHEDULINGPOLICY
 _VECTORSEARCHINDEXPIPELINESPEC.fields_by_name['vector_index'].message_type = _VECTORSEARCHINDEXPIPELINESPEC_VECTORINDEX
 _VECTORSEARCHINDEXPIPELINESPEC.oneofs_by_name['scheduling_policy'].fields.append(
@@ -1111,21 +1320,37 @@
 _CREATEVECTORSEARCHCATALOGRESPONSE.fields_by_name['catalog_definition'].message_type = _VECTORSEARCHCATALOGDEFINITION
 _GETVECTORSEARCHCATALOGRESPONSE.fields_by_name['catalog_definition'].message_type = _VECTORSEARCHCATALOGDEFINITION
 _GETVECTORSEARCHCATALOGRESPONSE.fields_by_name['catalog_status'].message_type = _VECTORSEARCHCATALOGSTATUS
 _CREATEVECTORSEARCHINDEXREQUEST.fields_by_name['index_pipeline_spec'].message_type = _VECTORSEARCHINDEXPIPELINESPEC
 _CREATEVECTORSEARCHINDEXRESPONSE.fields_by_name['index_definition'].message_type = _VECTORSEARCHINDEXDEFINITION
 _GETVECTORSEARCHINDEXRESPONSE.fields_by_name['index_definition'].message_type = _VECTORSEARCHINDEXDEFINITION
 _GETVECTORSEARCHINDEXRESPONSE.fields_by_name['index_status'].message_type = _VECTORSEARCHINDEXSTATUS
-_LISTVECTORSEARCHINDEXRESPONSE.fields_by_name['index_definitions'].message_type = _VECTORSEARCHINDEXDEFINITIONKEYVALUEPAIR
-_QUERYVECTORSEARCHINDEXRESPONSE.fields_by_name['docs'].message_type = _VECTORSEARCHINDEXDOCUMENT
+_LISTVECTORSEARCHINDEXRESPONSE.fields_by_name['indexes'].message_type = _VECTORSEARCHINDEXITEM
+_QUERYVECTORSEARCHINDEXRESPONSE.fields_by_name['manifest'].message_type = _RESULTMANIFEST
+_QUERYVECTORSEARCHINDEXRESPONSE.fields_by_name['result'].message_type = _RESULTDATA
+_RESULTDATA.fields_by_name['data_array'].message_type = brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_well__known__types__pb2._LISTVALUE
+_TYPEDROW.fields_by_name['values'].message_type = _TYPEDVALUE
+_TYPEDVALUE.oneofs_by_name['as'].fields.append(
+  _TYPEDVALUE.fields_by_name['bit'])
+_TYPEDVALUE.fields_by_name['bit'].containing_oneof = _TYPEDVALUE.oneofs_by_name['as']
+_TYPEDVALUE.oneofs_by_name['as'].fields.append(
+  _TYPEDVALUE.fields_by_name['bigint'])
+_TYPEDVALUE.fields_by_name['bigint'].containing_oneof = _TYPEDVALUE.oneofs_by_name['as']
+_TYPEDVALUE.oneofs_by_name['as'].fields.append(
+  _TYPEDVALUE.fields_by_name['num'])
+_TYPEDVALUE.fields_by_name['num'].containing_oneof = _TYPEDVALUE.oneofs_by_name['as']
+_TYPEDVALUE.oneofs_by_name['as'].fields.append(
+  _TYPEDVALUE.fields_by_name['str'])
+_TYPEDVALUE.fields_by_name['str'].containing_oneof = _TYPEDVALUE.oneofs_by_name['as']
+_RESULTMANIFEST.fields_by_name['columns'].message_type = _COLUMNINFO
 DESCRIPTOR.message_types_by_name['VectorSearchCatalogDefinition'] = _VECTORSEARCHCATALOGDEFINITION
 DESCRIPTOR.message_types_by_name['VectorSearchCatalogStatus'] = _VECTORSEARCHCATALOGSTATUS
 DESCRIPTOR.message_types_by_name['VectorSearchIndexStatus'] = _VECTORSEARCHINDEXSTATUS
 DESCRIPTOR.message_types_by_name['VectorSearchIndexDefinition'] = _VECTORSEARCHINDEXDEFINITION
-DESCRIPTOR.message_types_by_name['VectorSearchIndexDefinitionKeyValuePair'] = _VECTORSEARCHINDEXDEFINITIONKEYVALUEPAIR
+DESCRIPTOR.message_types_by_name['VectorSearchIndexItem'] = _VECTORSEARCHINDEXITEM
 DESCRIPTOR.message_types_by_name['VectorSearchIndexPipelineSpec'] = _VECTORSEARCHINDEXPIPELINESPEC
 DESCRIPTOR.message_types_by_name['VectorSearchIndexDocument'] = _VECTORSEARCHINDEXDOCUMENT
 DESCRIPTOR.message_types_by_name['CreateVectorSearchCatalogRequest'] = _CREATEVECTORSEARCHCATALOGREQUEST
 DESCRIPTOR.message_types_by_name['CreateVectorSearchCatalogResponse'] = _CREATEVECTORSEARCHCATALOGRESPONSE
 DESCRIPTOR.message_types_by_name['DeleteVectorSearchCatalogRequest'] = _DELETEVECTORSEARCHCATALOGREQUEST
 DESCRIPTOR.message_types_by_name['DeleteVectorSearchCatalogResponse'] = _DELETEVECTORSEARCHCATALOGRESPONSE
 DESCRIPTOR.message_types_by_name['GetVectorSearchCatalogRequest'] = _GETVECTORSEARCHCATALOGREQUEST
@@ -1136,14 +1361,19 @@
 DESCRIPTOR.message_types_by_name['GetVectorSearchIndexResponse'] = _GETVECTORSEARCHINDEXRESPONSE
 DESCRIPTOR.message_types_by_name['ListVectorSearchIndexRequest'] = _LISTVECTORSEARCHINDEXREQUEST
 DESCRIPTOR.message_types_by_name['ListVectorSearchIndexResponse'] = _LISTVECTORSEARCHINDEXRESPONSE
 DESCRIPTOR.message_types_by_name['DeleteVectorSearchIndexRequest'] = _DELETEVECTORSEARCHINDEXREQUEST
 DESCRIPTOR.message_types_by_name['DeleteVectorSearchIndexResponse'] = _DELETEVECTORSEARCHINDEXRESPONSE
 DESCRIPTOR.message_types_by_name['QueryVectorSearchIndexRequest'] = _QUERYVECTORSEARCHINDEXREQUEST
 DESCRIPTOR.message_types_by_name['QueryVectorSearchIndexResponse'] = _QUERYVECTORSEARCHINDEXRESPONSE
+DESCRIPTOR.message_types_by_name['ResultData'] = _RESULTDATA
+DESCRIPTOR.message_types_by_name['TypedRow'] = _TYPEDROW
+DESCRIPTOR.message_types_by_name['TypedValue'] = _TYPEDVALUE
+DESCRIPTOR.message_types_by_name['ResultManifest'] = _RESULTMANIFEST
+DESCRIPTOR.message_types_by_name['ColumnInfo'] = _COLUMNINFO
 DESCRIPTOR.message_types_by_name['VectorSearchInternalInfo'] = _VECTORSEARCHINTERNALINFO
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 VectorSearchCatalogDefinition = _reflection.GeneratedProtocolMessageType('VectorSearchCatalogDefinition', (_message.Message,), {
   'DESCRIPTOR' : _VECTORSEARCHCATALOGDEFINITION,
   '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
   # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.VectorSearchCatalogDefinition)
@@ -1167,20 +1397,20 @@
 VectorSearchIndexDefinition = _reflection.GeneratedProtocolMessageType('VectorSearchIndexDefinition', (_message.Message,), {
   'DESCRIPTOR' : _VECTORSEARCHINDEXDEFINITION,
   '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
   # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.VectorSearchIndexDefinition)
   })
 _sym_db.RegisterMessage(VectorSearchIndexDefinition)
 
-VectorSearchIndexDefinitionKeyValuePair = _reflection.GeneratedProtocolMessageType('VectorSearchIndexDefinitionKeyValuePair', (_message.Message,), {
-  'DESCRIPTOR' : _VECTORSEARCHINDEXDEFINITIONKEYVALUEPAIR,
+VectorSearchIndexItem = _reflection.GeneratedProtocolMessageType('VectorSearchIndexItem', (_message.Message,), {
+  'DESCRIPTOR' : _VECTORSEARCHINDEXITEM,
   '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
-  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.VectorSearchIndexDefinitionKeyValuePair)
+  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.VectorSearchIndexItem)
   })
-_sym_db.RegisterMessage(VectorSearchIndexDefinitionKeyValuePair)
+_sym_db.RegisterMessage(VectorSearchIndexItem)
 
 VectorSearchIndexPipelineSpec = _reflection.GeneratedProtocolMessageType('VectorSearchIndexPipelineSpec', (_message.Message,), {
 
   'ContinuousSchedulingPolicy' : _reflection.GeneratedProtocolMessageType('ContinuousSchedulingPolicy', (_message.Message,), {
     'DESCRIPTOR' : _VECTORSEARCHINDEXPIPELINESPEC_CONTINUOUSSCHEDULINGPOLICY,
     '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
     # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.VectorSearchIndexPipelineSpec.ContinuousSchedulingPolicy)
@@ -1324,26 +1554,60 @@
 QueryVectorSearchIndexResponse = _reflection.GeneratedProtocolMessageType('QueryVectorSearchIndexResponse', (_message.Message,), {
   'DESCRIPTOR' : _QUERYVECTORSEARCHINDEXRESPONSE,
   '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
   # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.QueryVectorSearchIndexResponse)
   })
 _sym_db.RegisterMessage(QueryVectorSearchIndexResponse)
 
+ResultData = _reflection.GeneratedProtocolMessageType('ResultData', (_message.Message,), {
+  'DESCRIPTOR' : _RESULTDATA,
+  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
+  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.ResultData)
+  })
+_sym_db.RegisterMessage(ResultData)
+
+TypedRow = _reflection.GeneratedProtocolMessageType('TypedRow', (_message.Message,), {
+  'DESCRIPTOR' : _TYPEDROW,
+  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
+  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.TypedRow)
+  })
+_sym_db.RegisterMessage(TypedRow)
+
+TypedValue = _reflection.GeneratedProtocolMessageType('TypedValue', (_message.Message,), {
+  'DESCRIPTOR' : _TYPEDVALUE,
+  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
+  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.TypedValue)
+  })
+_sym_db.RegisterMessage(TypedValue)
+
+ResultManifest = _reflection.GeneratedProtocolMessageType('ResultManifest', (_message.Message,), {
+  'DESCRIPTOR' : _RESULTMANIFEST,
+  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
+  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.ResultManifest)
+  })
+_sym_db.RegisterMessage(ResultManifest)
+
+ColumnInfo = _reflection.GeneratedProtocolMessageType('ColumnInfo', (_message.Message,), {
+  'DESCRIPTOR' : _COLUMNINFO,
+  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
+  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.ColumnInfo)
+  })
+_sym_db.RegisterMessage(ColumnInfo)
+
 VectorSearchInternalInfo = _reflection.GeneratedProtocolMessageType('VectorSearchInternalInfo', (_message.Message,), {
   'DESCRIPTOR' : _VECTORSEARCHINTERNALINFO,
   '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.messages_pb2'
   # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.VectorSearchInternalInfo)
   })
 _sym_db.RegisterMessage(VectorSearchInternalInfo)
 
 
 DESCRIPTOR._options = None
 _VECTORSEARCHCATALOGDEFINITION.fields_by_name['name']._options = None
 _VECTORSEARCHINDEXDEFINITION.fields_by_name['name']._options = None
-_VECTORSEARCHINDEXDEFINITION.fields_by_name['pipeline_id']._options = None
 _VECTORSEARCHINDEXPIPELINESPEC_VECTORINDEX.fields_by_name['column']._options = None
 _VECTORSEARCHINDEXPIPELINESPEC_VECTORINDEX.fields_by_name['embedding_model_endpoint_name']._options = None
 _VECTORSEARCHINDEXPIPELINESPEC.fields_by_name['continuous']._options = None
 _VECTORSEARCHINDEXPIPELINESPEC.fields_by_name['triggered']._options = None
 _VECTORSEARCHINDEXPIPELINESPEC.fields_by_name['src_table']._options = None
 _VECTORSEARCHINDEXPIPELINESPEC.fields_by_name['dest_index']._options = None
 _VECTORSEARCHINDEXPIPELINESPEC.fields_by_name['primary_key']._options = None
@@ -1353,13 +1617,14 @@
 _GETVECTORSEARCHCATALOGREQUEST._options = None
 _CREATEVECTORSEARCHINDEXREQUEST._options = None
 _CREATEVECTORSEARCHINDEXRESPONSE.fields_by_name['index_definition']._options = None
 _GETVECTORSEARCHINDEXREQUEST._options = None
 _GETVECTORSEARCHINDEXRESPONSE.fields_by_name['index_definition']._options = None
 _LISTVECTORSEARCHINDEXREQUEST.fields_by_name['catalog_name']._options = None
 _LISTVECTORSEARCHINDEXREQUEST._options = None
-_LISTVECTORSEARCHINDEXRESPONSE.fields_by_name['index_definitions']._options = None
+_LISTVECTORSEARCHINDEXRESPONSE.fields_by_name['indexes']._options = None
 _DELETEVECTORSEARCHINDEXREQUEST._options = None
 _QUERYVECTORSEARCHINDEXREQUEST._options = None
+_COLUMNINFO.fields_by_name['name']._options = None
 _VECTORSEARCHINTERNALINFO.fields_by_name['region']._options = None
 _VECTORSEARCHINTERNALINFO.fields_by_name['k8s_cluster_name']._options = None
 # @@protoc_insertion_point(module_scope)
```

## databricks/vector_search/proto/service_pb2.py

```diff
@@ -12,407 +12,115 @@
 
 
 from mlflow.protos import databricks_pb2 as databricks__pb2
 from mlflow.protos.scalapb import scalapb_pb2 as scalapb_dot_scalapb__pb2 
 from . import taxonomy_pb2 as compliance_dot_taxonomy_dot_taxonomy__pb2
 import messages_pb2 as brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2
 
-
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='brickindex-scheduler/brickindex-scheduler/api/proto/service.proto',
   package='databricks.brickindexscheduler',
   syntax='proto2',
-  serialized_options=b'\n,com.databricks.api.proto.brickindexscheduler\240\001\001\342?\002\020\001',
+  serialized_options=b'\n,com.databricks.api.proto.brickindexscheduler\240\001\001\342?2\020\001\032.com.databricks.api.proto.brickindexscheduler._',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\nAbrickindex-scheduler/brickindex-scheduler/api/proto/service.proto\x12\x1e\x64\x61tabricks.brickindexscheduler\x1a\"compliance/taxonomy/taxonomy.proto\x1a\x10\x64\x61tabricks.proto\x1a\x15scalapb/scalapb.proto\x1a\x42\x62rickindex-scheduler/brickindex-scheduler/api/proto/messages.proto\"~\n\x14GetTestResultRequest\x12\x16\n\x03key\x18\x01 \x01(\tB\x04\xc0\xd2#\x19R\x03key\x12\x1a\n\x05value\x18\x02 \x01(\tB\x04\xc0\xd2#\x19R\x05value:2\xe2?/\n-com.databricks.rpc.RPC[GetTestResultResponse]\"\xc8\x01\n\x15GetTestResultResponse\x12\x1c\n\x06result\x18\x01 \x01(\tB\x04\xc0\xd2#\x19R\x06result\x12W\n\x05state\x18\x02 \x01(\x0e\x32;.databricks.brickindexscheduler.GetTestResultResponse.StateB\x04\xc0\xd2#\x19R\x05state\"8\n\x05State\x12\x15\n\x11STATE_UNSPECIFIED\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\x0b\n\x07\x46\x41ILURE\x10\x02\"#\n\tPageToken\x12\x16\n\x06\x63ursor\x18\x01 \x01(\x05R\x06\x63ursor\"\x90\x01\n\x13ListTestKeysRequest\x12!\n\tpage_size\x18\x01 \x01(\x05\x42\x04\xc0\xd2#\x19R\x08pageSize\x12#\n\npage_token\x18\x02 \x01(\tB\x04\xc0\xd2#\x19R\tpageToken:1\xe2?.\n,com.databricks.rpc.RPC[ListTestKeysResponse]\"^\n\x14ListTestKeysResponse\x12\x18\n\x04keys\x18\x01 \x03(\tB\x04\xc0\xd2#\x19R\x04keys\x12,\n\x0fnext_page_token\x18\x02 \x01(\tB\x04\xc0\xd2#\x19R\rnextPageToken2\xe0\x0f\n\x1a\x42rickindexSchedulerService\x12\xac\x01\n\rGetTestResult\x12\x34.databricks.brickindexscheduler.GetTestResultRequest\x1a\x35.databricks.brickindexscheduler.GetTestResultResponse\".\x82\xb5\x18*\n&\n\x03GET\x12\x19/brickindex-scheduler/get\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xaa\x01\n\x0cListTestKeys\x12\x33.databricks.brickindexscheduler.ListTestKeysRequest\x1a\x34.databricks.brickindexscheduler.ListTestKeysResponse\"/\x82\xb5\x18+\n\'\n\x03GET\x12\x1a/brickindex-scheduler/list\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xce\x01\n\x19\x43reateVectorSearchCatalog\x12@.databricks.brickindexscheduler.CreateVectorSearchCatalogRequest\x1a\x41.databricks.brickindexscheduler.CreateVectorSearchCatalogResponse\",\x82\xb5\x18(\n$\n\x04POST\x12\x16/vector-search/catalog\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xcb\x01\n\x16GetVectorSearchCatalog\x12=.databricks.brickindexscheduler.GetVectorSearchCatalogRequest\x1a>.databricks.brickindexscheduler.GetVectorSearchCatalogResponse\"2\x82\xb5\x18.\n*\n\x03GET\x12\x1d/vector-search/catalog/{name}\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xd7\x01\n\x19\x44\x65leteVectorSearchCatalog\x12@.databricks.brickindexscheduler.DeleteVectorSearchCatalogRequest\x1a\x41.databricks.brickindexscheduler.DeleteVectorSearchCatalogResponse\"5\x82\xb5\x18\x31\n-\n\x06\x44\x45LETE\x12\x1d/vector-search/catalog/{name}\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xc6\x01\n\x17\x43reateVectorSearchIndex\x12>.databricks.brickindexscheduler.CreateVectorSearchIndexRequest\x1a?.databricks.brickindexscheduler.CreateVectorSearchIndexResponse\"*\x82\xb5\x18&\n\"\n\x04POST\x12\x14/vector-search/index\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xbd\x01\n\x14GetVectorSearchIndex\x12;.databricks.brickindexscheduler.GetVectorSearchIndexRequest\x1a<.databricks.brickindexscheduler.GetVectorSearchIndexResponse\"*\x82\xb5\x18&\n\"\n\x03GET\x12\x1b/vector-search/index/{name}\x10\x03\x12\xbf\x01\n\x15ListVectorSearchIndex\x12<.databricks.brickindexscheduler.ListVectorSearchIndexRequest\x1a=.databricks.brickindexscheduler.ListVectorSearchIndexResponse\")\x82\xb5\x18%\n!\n\x03GET\x12\x14/vector-search/index\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xcf\x01\n\x17\x44\x65leteVectorSearchIndex\x12>.databricks.brickindexscheduler.DeleteVectorSearchIndexRequest\x1a?.databricks.brickindexscheduler.DeleteVectorSearchIndexResponse\"3\x82\xb5\x18/\n+\n\x06\x44\x45LETE\x12\x1b/vector-search/index/{name}\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xcf\x01\n\x16QueryVectorSearchIndex\x12=.databricks.brickindexscheduler.QueryVectorSearchIndexRequest\x1a>.databricks.brickindexscheduler.QueryVectorSearchIndexResponse\"6\x82\xb5\x18\x32\n.\n\x03GET\x12!/vector-search/index/{name}/query\x1a\x04\x08\x02\x10\x00\x10\x03\x42\x36\n,com.databricks.api.proto.brickindexscheduler\xa0\x01\x01\xe2?\x02\x10\x01'
+  serialized_pb=b'\nAbrickindex-scheduler/brickindex-scheduler/api/proto/service.proto\x12\x1e\x64\x61tabricks.brickindexscheduler\x1a\"compliance/taxonomy/taxonomy.proto\x1a\x10\x64\x61tabricks.proto\x1a\x15scalapb/scalapb.proto\x1a\x42\x62rickindex-scheduler/brickindex-scheduler/api/proto/messages.proto2\x84\r\n\x1a\x42rickindexSchedulerService\x12\xce\x01\n\x19\x43reateVectorSearchCatalog\x12@.databricks.brickindexscheduler.CreateVectorSearchCatalogRequest\x1a\x41.databricks.brickindexscheduler.CreateVectorSearchCatalogResponse\",\x82\xb5\x18(\n$\n\x04POST\x12\x16/vector-search/catalog\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xcb\x01\n\x16GetVectorSearchCatalog\x12=.databricks.brickindexscheduler.GetVectorSearchCatalogRequest\x1a>.databricks.brickindexscheduler.GetVectorSearchCatalogResponse\"2\x82\xb5\x18.\n*\n\x03GET\x12\x1d/vector-search/catalog/{name}\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xd7\x01\n\x19\x44\x65leteVectorSearchCatalog\x12@.databricks.brickindexscheduler.DeleteVectorSearchCatalogRequest\x1a\x41.databricks.brickindexscheduler.DeleteVectorSearchCatalogResponse\"5\x82\xb5\x18\x31\n-\n\x06\x44\x45LETE\x12\x1d/vector-search/catalog/{name}\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xc6\x01\n\x17\x43reateVectorSearchIndex\x12>.databricks.brickindexscheduler.CreateVectorSearchIndexRequest\x1a?.databricks.brickindexscheduler.CreateVectorSearchIndexResponse\"*\x82\xb5\x18&\n\"\n\x04POST\x12\x14/vector-search/index\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xbd\x01\n\x14GetVectorSearchIndex\x12;.databricks.brickindexscheduler.GetVectorSearchIndexRequest\x1a<.databricks.brickindexscheduler.GetVectorSearchIndexResponse\"*\x82\xb5\x18&\n\"\n\x03GET\x12\x1b/vector-search/index/{name}\x10\x03\x12\xbf\x01\n\x15ListVectorSearchIndex\x12<.databricks.brickindexscheduler.ListVectorSearchIndexRequest\x1a=.databricks.brickindexscheduler.ListVectorSearchIndexResponse\")\x82\xb5\x18%\n!\n\x03GET\x12\x14/vector-search/index\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xcf\x01\n\x17\x44\x65leteVectorSearchIndex\x12>.databricks.brickindexscheduler.DeleteVectorSearchIndexRequest\x1a?.databricks.brickindexscheduler.DeleteVectorSearchIndexResponse\"3\x82\xb5\x18/\n+\n\x06\x44\x45LETE\x12\x1b/vector-search/index/{name}\x1a\x04\x08\x02\x10\x00\x10\x03\x12\xcf\x01\n\x16QueryVectorSearchIndex\x12=.databricks.brickindexscheduler.QueryVectorSearchIndexRequest\x1a>.databricks.brickindexscheduler.QueryVectorSearchIndexResponse\"6\x82\xb5\x18\x32\n.\n\x03GET\x12!/vector-search/index/{name}/query\x1a\x04\x08\x02\x10\x00\x10\x03\x42\x66\n,com.databricks.api.proto.brickindexscheduler\xa0\x01\x01\xe2?2\x10\x01\x1a.com.databricks.api.proto.brickindexscheduler._'
   ,
   dependencies=[compliance_dot_taxonomy_dot_taxonomy__pb2.DESCRIPTOR,databricks__pb2.DESCRIPTOR,scalapb_dot_scalapb__pb2.DESCRIPTOR,brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2.DESCRIPTOR,])
 
 
 
-_GETTESTRESULTRESPONSE_STATE = _descriptor.EnumDescriptor(
-  name='State',
-  full_name='databricks.brickindexscheduler.GetTestResultResponse.State',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
-    _descriptor.EnumValueDescriptor(
-      name='STATE_UNSPECIFIED', index=0, number=0,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='SUCCESS', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='FAILURE', index=2, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=519,
-  serialized_end=575,
-)
-_sym_db.RegisterEnumDescriptor(_GETTESTRESULTRESPONSE_STATE)
-
-
-_GETTESTRESULTREQUEST = _descriptor.Descriptor(
-  name='GetTestResultRequest',
-  full_name='databricks.brickindexscheduler.GetTestResultRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='key', full_name='databricks.brickindexscheduler.GetTestResultRequest.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\300\322#\031', json_name='key', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='value', full_name='databricks.brickindexscheduler.GetTestResultRequest.value', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\300\322#\031', json_name='value', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'\342?/\n-com.databricks.rpc.RPC[GetTestResultResponse]',
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=246,
-  serialized_end=372,
-)
-
-
-_GETTESTRESULTRESPONSE = _descriptor.Descriptor(
-  name='GetTestResultResponse',
-  full_name='databricks.brickindexscheduler.GetTestResultResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='result', full_name='databricks.brickindexscheduler.GetTestResultResponse.result', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\300\322#\031', json_name='result', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='state', full_name='databricks.brickindexscheduler.GetTestResultResponse.state', index=1,
-      number=2, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\300\322#\031', json_name='state', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-    _GETTESTRESULTRESPONSE_STATE,
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=375,
-  serialized_end=575,
-)
-
-
-_PAGETOKEN = _descriptor.Descriptor(
-  name='PageToken',
-  full_name='databricks.brickindexscheduler.PageToken',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='cursor', full_name='databricks.brickindexscheduler.PageToken.cursor', index=0,
-      number=1, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, json_name='cursor', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=577,
-  serialized_end=612,
-)
-
-
-_LISTTESTKEYSREQUEST = _descriptor.Descriptor(
-  name='ListTestKeysRequest',
-  full_name='databricks.brickindexscheduler.ListTestKeysRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='page_size', full_name='databricks.brickindexscheduler.ListTestKeysRequest.page_size', index=0,
-      number=1, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\300\322#\031', json_name='pageSize', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='page_token', full_name='databricks.brickindexscheduler.ListTestKeysRequest.page_token', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\300\322#\031', json_name='pageToken', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'\342?.\n,com.databricks.rpc.RPC[ListTestKeysResponse]',
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=615,
-  serialized_end=759,
-)
-
-
-_LISTTESTKEYSRESPONSE = _descriptor.Descriptor(
-  name='ListTestKeysResponse',
-  full_name='databricks.brickindexscheduler.ListTestKeysResponse',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='keys', full_name='databricks.brickindexscheduler.ListTestKeysResponse.keys', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\300\322#\031', json_name='keys', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='next_page_token', full_name='databricks.brickindexscheduler.ListTestKeysResponse.next_page_token', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=b'\300\322#\031', json_name='nextPageToken', file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=761,
-  serialized_end=855,
-)
-
-_GETTESTRESULTRESPONSE.fields_by_name['state'].enum_type = _GETTESTRESULTRESPONSE_STATE
-_GETTESTRESULTRESPONSE_STATE.containing_type = _GETTESTRESULTRESPONSE
-DESCRIPTOR.message_types_by_name['GetTestResultRequest'] = _GETTESTRESULTREQUEST
-DESCRIPTOR.message_types_by_name['GetTestResultResponse'] = _GETTESTRESULTRESPONSE
-DESCRIPTOR.message_types_by_name['PageToken'] = _PAGETOKEN
-DESCRIPTOR.message_types_by_name['ListTestKeysRequest'] = _LISTTESTKEYSREQUEST
-DESCRIPTOR.message_types_by_name['ListTestKeysResponse'] = _LISTTESTKEYSRESPONSE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-GetTestResultRequest = _reflection.GeneratedProtocolMessageType('GetTestResultRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETTESTRESULTREQUEST,
-  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.service_pb2'
-  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.GetTestResultRequest)
-  })
-_sym_db.RegisterMessage(GetTestResultRequest)
-
-GetTestResultResponse = _reflection.GeneratedProtocolMessageType('GetTestResultResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETTESTRESULTRESPONSE,
-  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.service_pb2'
-  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.GetTestResultResponse)
-  })
-_sym_db.RegisterMessage(GetTestResultResponse)
-
-PageToken = _reflection.GeneratedProtocolMessageType('PageToken', (_message.Message,), {
-  'DESCRIPTOR' : _PAGETOKEN,
-  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.service_pb2'
-  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.PageToken)
-  })
-_sym_db.RegisterMessage(PageToken)
-
-ListTestKeysRequest = _reflection.GeneratedProtocolMessageType('ListTestKeysRequest', (_message.Message,), {
-  'DESCRIPTOR' : _LISTTESTKEYSREQUEST,
-  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.service_pb2'
-  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.ListTestKeysRequest)
-  })
-_sym_db.RegisterMessage(ListTestKeysRequest)
-
-ListTestKeysResponse = _reflection.GeneratedProtocolMessageType('ListTestKeysResponse', (_message.Message,), {
-  'DESCRIPTOR' : _LISTTESTKEYSRESPONSE,
-  '__module__' : 'brickindex_scheduler.brickindex_scheduler.api.proto.service_pb2'
-  # @@protoc_insertion_point(class_scope:databricks.brickindexscheduler.ListTestKeysResponse)
-  })
-_sym_db.RegisterMessage(ListTestKeysResponse)
-
 
 DESCRIPTOR._options = None
-_GETTESTRESULTREQUEST.fields_by_name['key']._options = None
-_GETTESTRESULTREQUEST.fields_by_name['value']._options = None
-_GETTESTRESULTREQUEST._options = None
-_GETTESTRESULTRESPONSE.fields_by_name['result']._options = None
-_GETTESTRESULTRESPONSE.fields_by_name['state']._options = None
-_LISTTESTKEYSREQUEST.fields_by_name['page_size']._options = None
-_LISTTESTKEYSREQUEST.fields_by_name['page_token']._options = None
-_LISTTESTKEYSREQUEST._options = None
-_LISTTESTKEYSRESPONSE.fields_by_name['keys']._options = None
-_LISTTESTKEYSRESPONSE.fields_by_name['next_page_token']._options = None
 
 _BRICKINDEXSCHEDULERSERVICE = _descriptor.ServiceDescriptor(
   name='BrickindexSchedulerService',
   full_name='databricks.brickindexscheduler.BrickindexSchedulerService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=858,
-  serialized_end=2874,
+  serialized_start=247,
+  serialized_end=1915,
   methods=[
   _descriptor.MethodDescriptor(
-    name='GetTestResult',
-    full_name='databricks.brickindexscheduler.BrickindexSchedulerService.GetTestResult',
-    index=0,
-    containing_service=None,
-    input_type=_GETTESTRESULTREQUEST,
-    output_type=_GETTESTRESULTRESPONSE,
-    serialized_options=b'\202\265\030*\n&\n\003GET\022\031/brickindex-scheduler/get\032\004\010\002\020\000\020\003',
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='ListTestKeys',
-    full_name='databricks.brickindexscheduler.BrickindexSchedulerService.ListTestKeys',
-    index=1,
-    containing_service=None,
-    input_type=_LISTTESTKEYSREQUEST,
-    output_type=_LISTTESTKEYSRESPONSE,
-    serialized_options=b'\202\265\030+\n\'\n\003GET\022\032/brickindex-scheduler/list\032\004\010\002\020\000\020\003',
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
     name='CreateVectorSearchCatalog',
     full_name='databricks.brickindexscheduler.BrickindexSchedulerService.CreateVectorSearchCatalog',
-    index=2,
+    index=0,
     containing_service=None,
     input_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._CREATEVECTORSEARCHCATALOGREQUEST,
     output_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._CREATEVECTORSEARCHCATALOGRESPONSE,
     serialized_options=b'\202\265\030(\n$\n\004POST\022\026/vector-search/catalog\032\004\010\002\020\000\020\003',
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetVectorSearchCatalog',
     full_name='databricks.brickindexscheduler.BrickindexSchedulerService.GetVectorSearchCatalog',
-    index=3,
+    index=1,
     containing_service=None,
     input_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._GETVECTORSEARCHCATALOGREQUEST,
     output_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._GETVECTORSEARCHCATALOGRESPONSE,
     serialized_options=b'\202\265\030.\n*\n\003GET\022\035/vector-search/catalog/{name}\032\004\010\002\020\000\020\003',
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='DeleteVectorSearchCatalog',
     full_name='databricks.brickindexscheduler.BrickindexSchedulerService.DeleteVectorSearchCatalog',
-    index=4,
+    index=2,
     containing_service=None,
     input_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._DELETEVECTORSEARCHCATALOGREQUEST,
     output_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._DELETEVECTORSEARCHCATALOGRESPONSE,
     serialized_options=b'\202\265\0301\n-\n\006DELETE\022\035/vector-search/catalog/{name}\032\004\010\002\020\000\020\003',
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='CreateVectorSearchIndex',
     full_name='databricks.brickindexscheduler.BrickindexSchedulerService.CreateVectorSearchIndex',
-    index=5,
+    index=3,
     containing_service=None,
     input_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._CREATEVECTORSEARCHINDEXREQUEST,
     output_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._CREATEVECTORSEARCHINDEXRESPONSE,
     serialized_options=b'\202\265\030&\n\"\n\004POST\022\024/vector-search/index\032\004\010\002\020\000\020\003',
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetVectorSearchIndex',
     full_name='databricks.brickindexscheduler.BrickindexSchedulerService.GetVectorSearchIndex',
-    index=6,
+    index=4,
     containing_service=None,
     input_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._GETVECTORSEARCHINDEXREQUEST,
     output_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._GETVECTORSEARCHINDEXRESPONSE,
     serialized_options=b'\202\265\030&\n\"\n\003GET\022\033/vector-search/index/{name}\020\003',
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ListVectorSearchIndex',
     full_name='databricks.brickindexscheduler.BrickindexSchedulerService.ListVectorSearchIndex',
-    index=7,
+    index=5,
     containing_service=None,
     input_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._LISTVECTORSEARCHINDEXREQUEST,
     output_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._LISTVECTORSEARCHINDEXRESPONSE,
     serialized_options=b'\202\265\030%\n!\n\003GET\022\024/vector-search/index\032\004\010\002\020\000\020\003',
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='DeleteVectorSearchIndex',
     full_name='databricks.brickindexscheduler.BrickindexSchedulerService.DeleteVectorSearchIndex',
-    index=8,
+    index=6,
     containing_service=None,
     input_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._DELETEVECTORSEARCHINDEXREQUEST,
     output_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._DELETEVECTORSEARCHINDEXRESPONSE,
     serialized_options=b'\202\265\030/\n+\n\006DELETE\022\033/vector-search/index/{name}\032\004\010\002\020\000\020\003',
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='QueryVectorSearchIndex',
     full_name='databricks.brickindexscheduler.BrickindexSchedulerService.QueryVectorSearchIndex',
-    index=9,
+    index=7,
     containing_service=None,
     input_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._QUERYVECTORSEARCHINDEXREQUEST,
     output_type=brickindex__scheduler_dot_brickindex__scheduler_dot_api_dot_proto_dot_messages__pb2._QUERYVECTORSEARCHINDEXRESPONSE,
     serialized_options=b'\202\265\0302\n.\n\003GET\022!/vector-search/index/{name}/query\032\004\010\002\020\000\020\003',
     create_key=_descriptor._internal_create_key,
   ),
 ])
```

## Comparing `databricks_vectorsearch_preview-0.15.dist-info/METADATA` & `databricks_vectorsearch_preview-0.16.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-vectorsearch-preview
-Version: 0.15
+Version: 0.16
 Summary: Databricks Vector Search Client
 Home-page: UNKNOWN
 Author: Databirkcs
 Author-email: feedback@databricks.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `databricks_vectorsearch_preview-0.15.dist-info/RECORD` & `databricks_vectorsearch_preview-0.16.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 databricks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databricks/vector_search/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databricks/vector_search/client.py,sha256=7RggwONKHBDYd2fVxNZQ7gkU_yvvRh0YbKap9FyKnBM,10267
 databricks/vector_search/proto/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-databricks/vector_search/proto/messages_pb2.py,sha256=z8DumqdRQrpXXNvREnZwCbNSGChRotuumEivwXMCVYQ,65338
-databricks/vector_search/proto/service_pb2.py,sha256=fprjawx10B1sao1YHwRYOZ-aGGHTG3pCykmrDBt8muY,22870
+databricks/vector_search/proto/messages_pb2.py,sha256=oAU9bd4ku1TdkdTKb4NG_ZNC4YLUfMizydZW46VjyBo,76905
+databricks/vector_search/proto/service_pb2.py,sha256=9IlHXOdBJ-AphTysLa9ZFShnPgQGystEw0jvDdzfTuI,9837
 databricks/vector_search/proto/taxonomy_pb2.py,sha256=YzToOng9nuUEtEe0th-7h8i_J3XjNeh7y3-n1syCEuA,38292
-databricks_vectorsearch_preview-0.15.dist-info/METADATA,sha256=0JhsOgpebSEBmHLPLA0VYscRuduzrV7JNZoJ8fFm-V0,570
-databricks_vectorsearch_preview-0.15.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-databricks_vectorsearch_preview-0.15.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
-databricks_vectorsearch_preview-0.15.dist-info/RECORD,,
+databricks/vector_search/proto/well_known_types_pb2.py,sha256=VTfu0qDsXwns6O1mm_fwyfTS74iRt6aHMfNt7mbVdmk,13028
+databricks_vectorsearch_preview-0.16.dist-info/METADATA,sha256=6_UXxHQMBEjwNHQ9zMJos3J6PDSmPI7rlQQj5tqFxgE,570
+databricks_vectorsearch_preview-0.16.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+databricks_vectorsearch_preview-0.16.dist-info/top_level.txt,sha256=7kRdatoSgU0EUurRQJ_3F1Nv4EOSHWAr6ng25tJOJKU,11
+databricks_vectorsearch_preview-0.16.dist-info/RECORD,,
```

