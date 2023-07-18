# Comparing `tmp/dashvector-0.0.13-py3-none-any.whl.zip` & `tmp/dashvector-0.0.14-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,40 +1,40 @@
-Zip file size: 72033 bytes, number of entries: 38
+Zip file size: 72432 bytes, number of entries: 38
 -rw-r--r--  2.0 unx     1224 b- defN 23-Jul-12 09:23 dashvector/__init__.py
--rw-r--r--  2.0 unx      695 b- defN 23-Jul-13 07:54 dashvector/version.py
+-rw-r--r--  2.0 unx      695 b- defN 23-Jul-17 06:54 dashvector/version.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/common/__init__.py
 -rw-r--r--  2.0 unx      772 b- defN 23-Jul-12 09:23 dashvector/common/constants.py
--rw-r--r--  2.0 unx    10573 b- defN 23-Jul-12 09:23 dashvector/common/error.py
+-rw-r--r--  2.0 unx    10886 b- defN 23-Jul-17 06:53 dashvector/common/error.py
 -rw-r--r--  2.0 unx     4982 b- defN 23-Jul-12 09:23 dashvector/common/handler.py
 -rw-r--r--  2.0 unx     1659 b- defN 23-Jul-12 09:23 dashvector/common/logging.py
 -rw-r--r--  2.0 unx     4616 b- defN 23-Jul-12 09:23 dashvector/common/status.py
--rw-r--r--  2.0 unx    28038 b- defN 23-Jul-13 07:54 dashvector/common/types.py
+-rw-r--r--  2.0 unx    28038 b- defN 23-Jul-17 06:12 dashvector/common/types.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/core/__init__.py
--rw-r--r--  2.0 unx    17041 b- defN 23-Jul-13 07:54 dashvector/core/client.py
--rw-r--r--  2.0 unx    32235 b- defN 23-Jul-12 09:23 dashvector/core/collection.py
+-rw-r--r--  2.0 unx    17041 b- defN 23-Jul-18 07:35 dashvector/core/client.py
+-rw-r--r--  2.0 unx    33405 b- defN 23-Jul-18 11:38 dashvector/core/collection.py
 -rw-r--r--  2.0 unx     5285 b- defN 23-Jul-12 09:23 dashvector/core/doc.py
 -rw-r--r--  2.0 unx    11772 b- defN 23-Jul-12 09:23 dashvector/core/partition.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/core/handler/__init__.py
--rw-r--r--  2.0 unx    20176 b- defN 23-Jul-12 09:23 dashvector/core/handler/grpc_handler.py
+-rw-r--r--  2.0 unx    20149 b- defN 23-Jul-18 07:52 dashvector/core/handler/grpc_handler.py
 -rw-r--r--  2.0 unx    21454 b- defN 23-Jul-12 09:23 dashvector/core/handler/http_handler.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/core/models/__init__.py
--rw-r--r--  2.0 unx    10567 b- defN 23-Jul-13 07:54 dashvector/core/models/create_collection_request.py
+-rw-r--r--  2.0 unx    10567 b- defN 23-Jul-13 11:16 dashvector/core/models/create_collection_request.py
 -rw-r--r--  2.0 unx     2688 b- defN 23-Jul-12 09:23 dashvector/core/models/create_partition_request.py
 -rw-r--r--  2.0 unx     5843 b- defN 23-Jul-12 09:23 dashvector/core/models/delete_doc_request.py
 -rw-r--r--  2.0 unx     2139 b- defN 23-Jul-12 09:23 dashvector/core/models/describe_collection_request.py
 -rw-r--r--  2.0 unx     2107 b- defN 23-Jul-12 09:23 dashvector/core/models/drop_collection_request.py
 -rw-r--r--  2.0 unx     2667 b- defN 23-Jul-12 09:23 dashvector/core/models/drop_partition_request.py
 -rw-r--r--  2.0 unx     6361 b- defN 23-Jul-12 09:23 dashvector/core/models/get_doc_request.py
 -rw-r--r--  2.0 unx     1015 b- defN 23-Jul-12 09:23 dashvector/core/models/get_version_request.py
 -rw-r--r--  2.0 unx     1021 b- defN 23-Jul-12 09:23 dashvector/core/models/list_collection_request.py
--rw-r--r--  2.0 unx     9695 b- defN 23-Jul-12 09:23 dashvector/core/models/query_doc_request.py
+-rw-r--r--  2.0 unx     9656 b- defN 23-Jul-18 12:00 dashvector/core/models/query_doc_request.py
 -rw-r--r--  2.0 unx     2114 b- defN 23-Jul-12 09:23 dashvector/core/models/stats_collection_request.py
 -rw-r--r--  2.0 unx    16923 b- defN 23-Jul-12 09:23 dashvector/core/models/upsert_doc_request.py
 -rw-r--r--  2.0 unx      670 b- defN 23-Jul-12 09:23 dashvector/core/proto/__init__.py
 -rw-r--r--  2.0 unx   136016 b- defN 23-Jul-12 09:23 dashvector/core/proto/centaur_pb2.py
 -rw-r--r--  2.0 unx    21819 b- defN 23-Jul-12 09:23 dashvector/core/proto/centaur_pb2_grpc.py
--rw-r--r--  2.0 unx    12090 b- defN 23-Jul-13 07:54 dashvector-0.0.13.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4366 b- defN 23-Jul-13 07:54 dashvector-0.0.13.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 07:54 dashvector-0.0.13.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-13 07:54 dashvector-0.0.13.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3489 b- defN 23-Jul-13 07:54 dashvector-0.0.13.dist-info/RECORD
-38 files, 404895 bytes uncompressed, 66373 bytes compressed:  83.6%
+-rw-r--r--  2.0 unx    12090 b- defN 23-Jul-18 12:08 dashvector-0.0.14.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4366 b- defN 23-Jul-18 12:08 dashvector-0.0.14.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 12:08 dashvector-0.0.14.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-18 12:08 dashvector-0.0.14.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3489 b- defN 23-Jul-18 12:08 dashvector-0.0.14.dist-info/RECORD
+38 files, 406312 bytes uncompressed, 66772 bytes compressed:  83.6%
```

## zipnote {}

```diff
@@ -93,23 +93,23 @@
 
 Filename: dashvector/core/proto/centaur_pb2.py
 Comment: 
 
 Filename: dashvector/core/proto/centaur_pb2_grpc.py
 Comment: 
 
-Filename: dashvector-0.0.13.dist-info/LICENSE.txt
+Filename: dashvector-0.0.14.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dashvector-0.0.13.dist-info/METADATA
+Filename: dashvector-0.0.14.dist-info/METADATA
 Comment: 
 
-Filename: dashvector-0.0.13.dist-info/WHEEL
+Filename: dashvector-0.0.14.dist-info/WHEEL
 Comment: 
 
-Filename: dashvector-0.0.13.dist-info/top_level.txt
+Filename: dashvector-0.0.14.dist-info/top_level.txt
 Comment: 
 
-Filename: dashvector-0.0.13.dist-info/RECORD
+Filename: dashvector-0.0.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dashvector/version.py

```diff
@@ -13,8 +13,8 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
-__version__ = "0.0.13"
+__version__ = "0.0.14"
```

## dashvector/common/error.py

```diff
@@ -145,14 +145,19 @@
     DuplicateCollectionServerGroup = -30009
     IgnoreEtcdPath = -30010
     EmptyLoadBalancer = -30011
     MismatchedBatchResult = -30012
     IgnoreCollectionStatus = -30013
     IgnoreSegmentStatus = -30014
     IgnoreSegmentMeta = -30015
+    IgnorePartitionStatus = - 30016
+    InexistentPartition = -30017
+    DuplicatePartition = -30018
+    UnreadyPartition = -30019
+    EmptyPartitionName = -30020
     Unknown = -999
     Closed = -998
     Timeout = 408
     Success = 0
 
 
 class DashVectorCodeMap(object):
@@ -160,14 +165,15 @@
         DashVectorCode.EmptyCollectionName: DashVectorCode.InvalidArgument,
         DashVectorCode.EmptyColumnName: DashVectorCode.InvalidArgument,
         DashVectorCode.EmptyColumns : DashVectorCode.InvalidArgument,
         DashVectorCode.EmptyRepositoryTable: DashVectorCode.InvalidArgument,
         DashVectorCode.EmptyRepositoryName: DashVectorCode.InvalidArgument,
         DashVectorCode.EmptyUserName: DashVectorCode.InvalidArgument,
         DashVectorCode.EmptyPassword: DashVectorCode.InvalidArgument,
+        DashVectorCode.EmptyPartitionName: DashVectorCode.InvalidArgument,
         DashVectorCode.InvalidURI: DashVectorCode.InvalidArgument,
         DashVectorCode.InvalidCollectionStatus: DashVectorCode.InvalidArgument,
         DashVectorCode.InvalidRecord: DashVectorCode.InvalidArgument,
         DashVectorCode.InvalidQuery: DashVectorCode.InvalidArgument,
         DashVectorCode.InvalidIndexDataFormat: DashVectorCode.InvalidArgument,
         DashVectorCode.InvalidWriteRequest: DashVectorCode.InvalidArgument,
         DashVectorCode.InvalidVectorFormat: DashVectorCode.InvalidArgument,
@@ -178,14 +184,15 @@
         DashVectorCode.InvalidRevision: DashVectorCode.InvalidArgument,
         DashVectorCode.InvalidFeature: DashVectorCode.InvalidArgument,
         DashVectorCode.MismatchedSchema: DashVectorCode.InvalidArgument,
         DashVectorCode.EmptyPrimaryKey: DashVectorCode.InvalidArgument,
         DashVectorCode.EmptyDocList: DashVectorCode.InvalidArgument,
         DashVectorCode.InvalidField: DashVectorCode.InvalidArgument,
         DashVectorCode.DuplicateField: DashVectorCode.InvalidArgument,
+        DashVectorCode.DuplicatePartition: DashVectorCode.InvalidArgument,
         DashVectorCode.EmptyIndexField: DashVectorCode.InvalidArgument,
         DashVectorCode.UnsupportedConnection: DashVectorCode.InvalidArgument
     }
 
     @staticmethod
     def rewrite(code: DashVectorCode):
         if code not in DashVectorCodeMap._map_rules:
```

## dashvector/core/collection.py

```diff
@@ -13,20 +13,22 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 ##
 
 # -*- coding: utf-8 -*-
 
+import time
 import numpy as np
 from typing import List, Dict, Tuple, Union, Optional
 from dashvector.common.error import DashVectorException
 from dashvector.common.types import DashVectorCode, DashVectorResponse
 from dashvector.common.types import CollectionMeta, CollectionStats
 from dashvector.common.handler import RPCHandler, RPCResponse
+from dashvector.common.status import PartitionStatus
 from dashvector.core.models.describe_collection_request import DescribeCollectionRequest
 from dashvector.core.models.upsert_doc_request import UpsertDocRequest
 from dashvector.core.models.delete_doc_request import DeleteDocRequest
 from dashvector.core.models.get_doc_request import GetDocRequest
 from dashvector.core.models.query_doc_request import QueryDocRequest
 from dashvector.core.models.create_partition_request import CreatePartitionRequest
 from dashvector.core.models.drop_partition_request import DropPartitionRequest
@@ -387,21 +389,26 @@
                                               ids=ids,
                                               partition=partition)
         except DashVectorException as e:
             return DashVectorResponse(None, exception=e)
 
         return DashVectorResponse(self._handler.collection_delete_doc(delete_request, async_req=async_req))
 
-    def create_partition(self, name: str) -> DashVectorResponse:
+    def create_partition(self, 
+                         name: str,
+                         *,
+                         timeout: Optional[int] = None) -> DashVectorResponse:
 
         """
         Create a Partition in current Collection.
 
         Args:
            name (str): partition name
+           timeout (Optional[int]): timeout[second] for wait until the partition is ready, default is 'None' wait indefinitely
+
 
         Return:
            DashVectorResponse, include code / message / request_id,
                             code == DashVectorCode.Success means create partition success, otherwise means failure.
 
         Example:
             rsp = collection.create_partition("partition_name")
@@ -416,17 +423,50 @@
                                                               request_id=self.request_id))
 
         try:
             create_request = CreatePartitionRequest(collection_meta=self._collection_meta,
                                                     partition_name=name)
         except DashVectorException as e:
             return DashVectorResponse(None, exception=e)
-
-        return DashVectorResponse(self._handler.collection_create_partition(create_request, async_req=False))
-
+    
+        create_response = DashVectorResponse(self._handler.collection_create_partition(create_request, async_req=False))
+        if create_response.code != DashVectorCode.Success or timeout == -1:    
+            return create_response
+        
+        create_partition_timeout = timeout
+        rpc_error_count = 0
+        while True:
+            describe_response = self.describe_partition(name)
+
+            if describe_response.code ==DashVectorCode.Success:
+                if describe_response.output.state == PartitionStatus.SERVING:
+                    return create_response
+                elif describe_response.output.state in (PartitionStatus.ERROR, PartitionStatus.DROPPING):
+                    return DashVectorResponse(None, 
+                                           exception=DashVectorException(code=DashVectorCode.UnreadyPartition,
+                                                                      reason=f"Partition[{name}] Status is {describe_response.output.state}",
+                                                                      request_id=create_response.request_id))
+            else:
+                rpc_error_count += 1
+            
+            if rpc_error_count > 3:
+                return DashVectorResponse(None, 
+                                       exception = DashVectorException(code=describe_response.code,
+                                                                    reason=f"Get Partition Status failed and reason is {describe_response.message}",
+                                                                    request_id=create_response.request_id))
+            time.sleep(5)
+            if create_partition_timeout is None:
+                continue
+            create_partition_timeout -= 5
+            if create_partition_timeout < 0:
+                return DashVectorResponse(None, 
+                                       exception=DashVectorException(code=DashVectorCode.Timeout,
+                                                                  reason="Please call the describe_partition to confirm partition status",
+                                                                  request_id=create_response.request_id))
+            
     def delete_partition(self, name: str) -> DashVectorResponse:
 
         """
         Delete a Partition in current Collection.
 
         Args:
            name (str): partition name.
@@ -502,41 +542,14 @@
                                        exception=DashVectorException(code=DashVectorCode.NotFound,
                                                                   reason="DashVectorSDK Collection Partition NotFound"))
             describe_response.output = partitions_meta[name]
             return describe_response
         except DashVectorException as e:
             return DashVectorResponse(None, exception=e)
 
-    def has_partition(self, name: str) -> DashVectorResponse:
-
-        """
-        Determine a Partition exists in current Collection.
-
-        Return:
-           DashVectorResponse, include code / message / request_id / output,
-                            code == DashVectorCode.Success means output is a partition determine status.
-
-        Example:
-            rsp = collection.has_partition("partition_name")
-            if not rsp:
-                raise RuntimeError(f"HasPartition Failed, error:{rsp.code}, message:{rsp.message}")
-            has_partition = rsp.output
-            print("has_partition:", has_partition)
-        """
-
-        if self._code != DashVectorCode.Success:
-            return DashVectorResponse(None,
-                                   exception=DashVectorException(code=DashVectorCode.RuntimeError,
-                                                              reason="DashVectorSDK Collection initialize Failed",
-                                                              request_id=self.request_id))
-
-        describe_response = self.describe_partition(name)
-        describe_response.output = True if describe_response.code == DashVectorCode.Success else False
-        return describe_response
-
     def stats(self) -> DashVectorResponse:
 
         """
         Get Stats Info of current Collection.
 
         Return:
            DashVectorResponse, include code / message / request_id / output,
```

## dashvector/core/handler/grpc_handler.py

```diff
@@ -248,15 +248,15 @@
         try:
             rsp = self._stub.describe_collection.future(describe_request.to_proto(),
                                                         metadata=self._metadata,
                                                         timeout=self._timeout)
             return self._GRPCResponse(rsp, async_req=async_req, attr_name='collection')
         except grpc.RpcError as e:
             raise DashVectorGRPCException(code=e.code(),
-                                       reason=e.details(),
+                               
                                        request_id=self._parse_request_id_from_exception(e))
 
     def list_collections(self,
                          *,
                          async_req: bool = False) -> RPCResponse:
         try:
             rsp = self._stub.list_collections.future(ListCollectionRequest().to_proto(),
```

## dashvector/core/models/create_collection_request.py

```diff
@@ -129,15 +129,15 @@
 
                 if re.search('^[a-zA-Z][a-zA-Z0-9_-]{0,32}$', field_name) is None:
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                            reason=f"DashVectorSDK CreateCollectionRequest field_name in fields_schema Characters({field_name}) is Invalid and must be in [a-zA-Z0-9] and symbols[_]")
 
                 if field_name == DASHVECTOR_VECTOR_NAME:
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                           reason=f'DashVectorSDK CreateCollectionRequest field_name in fields_schema Value({DashVector_VECTOR_NAME}) is Reserved')
+                                           reason=f'DashVectorSDK CreateCollectionRequest field_name in fields_schema Value({DASHVECTOR_VECTOR_NAME}) is Reserved')
 
                 if not isinstance(field_dtype, type):
                     raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                            reason=f"DashVectorSDK CreateCollectionRequest field_dtype in fields_schema Type({type(field_dtype)}) is Invalid")
 
                 if field_dtype is not str \
                         and field_dtype is not int \
```

## dashvector/core/models/query_doc_request.py

```diff
@@ -43,15 +43,14 @@
         self._collection_feature_format = DataParser.data_type_to_format[self._collection_feature_schema.data_type]
 
         '''
         QueryRequest
         '''
         query_request = centaur_pb2.QueryRequest()
         query_request.collection_name = self._collection_name
-        query_request.topk = topk
 
         '''
         vector: Optional[VectorValueType] = None
         '''
         self._vector = None
         if isinstance(vector, list):
             if len(vector) != self._collection_feature_schema.dimension:
@@ -98,15 +97,15 @@
         '''
         self._topk = topk
         if not isinstance(topk, int):
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
                                    reason=f"DashVectorSDK QueryDocRequest topk Type({type(topk)}) is Invalid")
         if topk < 1 or topk > 1024:
             raise DashVectorException(code=DashVectorCode.InvalidArgument,
-                                   reason=f"DashVectorSDK GetDocRequest topk Value({len(topk)}) is Invalid and must be in [1, 1024]")
+                                   reason=f"DashVectorSDK GetDocRequest topk Value({topk}) is Invalid and must be in [1, 1024]")
         query_request.topk = self._topk
 
         '''
         filter: Optional[str] = None,
         '''
         self._filter = None
         if filter is not None:
```

## Comparing `dashvector-0.0.13.dist-info/LICENSE.txt` & `dashvector-0.0.14.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dashvector-0.0.13.dist-info/METADATA` & `dashvector-0.0.14.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashvector
-Version: 0.0.13
+Version: 0.0.14
 Summary: DashVector Client Python Sdk Library
 Home-page: https://github.com/alibaba/proxima
 Author: Alibaba
 Author-email: dashvector@alibaba-inc.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

## Comparing `dashvector-0.0.13.dist-info/RECORD` & `dashvector-0.0.14.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 dashvector/__init__.py,sha256=Cpl05fQAaj_mlaecjl7OA8Us1Nd80DPI0kt9enNHNsM,1224
-dashvector/version.py,sha256=aCQN3CO2paZl7YZM8_ou1lxbGiaUf8uvNt4W3xLtxf4,695
+dashvector/version.py,sha256=crZ5YBlj_T2bWtRfnTu220zB9f5Y1hA_3bMRuBLvhRo,695
 dashvector/common/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
 dashvector/common/constants.py,sha256=zpBWhp04ESp60M7Zj9HHXcOMk8Q_jH7dmanE4V1gfTI,772
-dashvector/common/error.py,sha256=SqtYTJnDUnLNeYJL0nDdoe2cNAHJ75orO15_RW1qkRo,10573
+dashvector/common/error.py,sha256=3Zq8ru1A582ZHypgpPPS81DSp23rGr7-bU2hgT76eI8,10886
 dashvector/common/handler.py,sha256=347-RKVaaF829PrnmcAWldVcCF8ivFFi5OMba53PsWw,4982
 dashvector/common/logging.py,sha256=Cw-KMQ_y94VfKxw4QEJ1HbjZVH2AIkkUuhsTC-9O_4c,1659
 dashvector/common/status.py,sha256=JvJI2-Yk8eimGjWOHotzYPY8DmjeVUW02zk_dGm954Q,4616
 dashvector/common/types.py,sha256=kAYwd9p3xknwJ_7ApulPWwjopLIzceiGTvfgWenyhfU,28038
 dashvector/core/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
 dashvector/core/client.py,sha256=YxVSSC3hDk5MwG70RcgVpWAGw8KymtHXiFY92VLmCag,17041
-dashvector/core/collection.py,sha256=1soUGaTnkCBlMQN2RZtQg3V4kAUleGZaqiISmgQ8878,32235
+dashvector/core/collection.py,sha256=JTXJOQfd4DNA33nMJKjDyQ4nq6qTwDtKFNQqpW0o7Jc,33405
 dashvector/core/doc.py,sha256=nSBmNInoE_5dzVnSdWBcGQ5WKd227hJ-6GlRhBLvUTo,5285
 dashvector/core/partition.py,sha256=G6WdshhvqoYrObe7yj2lCI2r3QUt5bNeA2BozvmPZwY,11772
 dashvector/core/handler/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
-dashvector/core/handler/grpc_handler.py,sha256=EZ7YQsaZdl93qSAquiVKcrga2JbJ04G9fuQGhOkDNu4,20176
+dashvector/core/handler/grpc_handler.py,sha256=WHQGa_mfYAsQQAb3_qkYxL8gyJQ-srM8GsuQWka5Eew,20149
 dashvector/core/handler/http_handler.py,sha256=rysglKNvNMM55-UbR1jKkgHr4FsUpHh_bEhdU_AOfvA,21454
 dashvector/core/models/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
-dashvector/core/models/create_collection_request.py,sha256=vCf4-tsBlcmNy8BC1SZAJyg_TUY6d_FCIsN2POC0n6U,10567
+dashvector/core/models/create_collection_request.py,sha256=F4t76iivpIbE-e217jzptGt67VZ554KidVl3hDLqvII,10567
 dashvector/core/models/create_partition_request.py,sha256=2Yow2FYjfht2uSmkoVEbG3uwgUthCuQB1ISuGadG5xY,2688
 dashvector/core/models/delete_doc_request.py,sha256=Ey2m0CfLH2iJRw4DJtODA_RJJi7qM_8xJS2MxYZFBS0,5843
 dashvector/core/models/describe_collection_request.py,sha256=DD8tef7Pm0oJUXkydbY0R10ZMPzt6fbBREq2aH3givw,2139
 dashvector/core/models/drop_collection_request.py,sha256=94TiA0cnymFPewc2U1IsDPp-TCnQmZG9_x-sk-tstC0,2107
 dashvector/core/models/drop_partition_request.py,sha256=Wdrn0Y7CaaXe2OKt-ryLXkjxog1ppgcr0oDaUpnE3dU,2667
 dashvector/core/models/get_doc_request.py,sha256=rbq2qRtsb0UCP2HatXWAVDd8M8NzZ5EKsYS0U51mJhE,6361
 dashvector/core/models/get_version_request.py,sha256=MJIU8UJ1heNJ09rpy_kXwSyPLsy0TA7GDJuTeBDdqVU,1015
 dashvector/core/models/list_collection_request.py,sha256=CoVqnp4HpfZ9co8Sf2L_AXG2G-GnSzTWMEdmLdx8xoQ,1021
-dashvector/core/models/query_doc_request.py,sha256=rvGFQG6OhhIfxLwEOYTzUiGpY3cG13gVaNPFR_p93Y8,9695
+dashvector/core/models/query_doc_request.py,sha256=LJ5mDWQZGKoAfU4Ndund-9IITW4uRboPGNzHEVW8F_Y,9656
 dashvector/core/models/stats_collection_request.py,sha256=CO8mzBbZ0OqXfZj1Ja49bjYuRyA8i1ss8LfTRc9oy9w,2114
 dashvector/core/models/upsert_doc_request.py,sha256=yacJ53eOhZ_w0OA8P_9sBTIuDVXAVb26S6tJ0jikJ0Y,16923
 dashvector/core/proto/__init__.py,sha256=q6xCixbAJHZFrFyB6QWQnRe4G-lrPOOZ6fwCIeFlFZg,670
 dashvector/core/proto/centaur_pb2.py,sha256=JqO3G1qYgTr7JSPhrcS652Q_dEVoCMh6PDj-4gopCEo,136016
 dashvector/core/proto/centaur_pb2_grpc.py,sha256=a2ED6WA43pi7BWe5-g3v9uj-RV4qRZeGYO6k96zPVzk,21819
-dashvector-0.0.13.dist-info/LICENSE.txt,sha256=GYJChq297x8HRI7yfGLcHdK-evsn6Sv7k68UCeGTu9w,12090
-dashvector-0.0.13.dist-info/METADATA,sha256=h4ybzje_Ci8ic67ePzMB4GnuGbhLyma1Hv2QWN3IoOE,4366
-dashvector-0.0.13.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
-dashvector-0.0.13.dist-info/top_level.txt,sha256=Ynh6NVKjpSk3PBj82cAq0AEs9j_KIV3ANXLCiLHntVk,11
-dashvector-0.0.13.dist-info/RECORD,,
+dashvector-0.0.14.dist-info/LICENSE.txt,sha256=GYJChq297x8HRI7yfGLcHdK-evsn6Sv7k68UCeGTu9w,12090
+dashvector-0.0.14.dist-info/METADATA,sha256=tsdLHUTrjMb2566n6T068YgMTV0n5eB_l6CslfTJy_o,4366
+dashvector-0.0.14.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
+dashvector-0.0.14.dist-info/top_level.txt,sha256=Ynh6NVKjpSk3PBj82cAq0AEs9j_KIV3ANXLCiLHntVk,11
+dashvector-0.0.14.dist-info/RECORD,,
```

