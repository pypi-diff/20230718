# Comparing `tmp/pydantic_neo4j-0.2.1.tar.gz` & `tmp/pydantic_neo4j-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_neo4j-0.2.1.tar", max compression
+gzip compressed data, was "pydantic_neo4j-0.3.0.tar", max compression
```

## Comparing `pydantic_neo4j-0.2.1.tar` & `pydantic_neo4j-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      709 2023-07-17 21:35:03.897555 pydantic_neo4j-0.2.1/pydantic_neo4j/__init__.py
--rw-r--r--   0        0        0     5756 2023-07-17 21:35:03.897555 pydantic_neo4j-0.2.1/pydantic_neo4j/create_operations.py
--rw-r--r--   0        0        0     4468 2023-07-17 21:35:03.902896 pydantic_neo4j-0.2.1/pydantic_neo4j/database_operations.py
--rw-r--r--   0        0        0     3131 2023-07-17 21:35:03.903866 pydantic_neo4j-0.2.1/pydantic_neo4j/graph_base_models.py
--rw-r--r--   0        0        0    10473 2023-07-17 21:35:03.903866 pydantic_neo4j-0.2.1/pydantic_neo4j/match_operations.py
--rw-r--r--   0        0        0     1268 2023-07-17 21:35:03.903866 pydantic_neo4j-0.2.1/pydantic_neo4j/pydantic_neo4j.py
--rw-r--r--   0        0        0      603 2023-07-17 21:41:40.813037 pydantic_neo4j-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4736 2023-07-17 21:41:20.964929 pydantic_neo4j-0.2.1/README.md
--rw-r--r--   0        0        0     5209 1970-01-01 00:00:00.000000 pydantic_neo4j-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      869 2023-07-18 03:47:13.989691 pydantic_neo4j-0.3.0/pydantic_neo4j/__init__.py
+-rw-r--r--   0        0        0     5756 2023-07-17 21:35:03.897555 pydantic_neo4j-0.3.0/pydantic_neo4j/create_operations.py
+-rw-r--r--   0        0        0     4872 2023-07-18 00:44:33.557638 pydantic_neo4j-0.3.0/pydantic_neo4j/database_operations.py
+-rw-r--r--   0        0        0     3369 2023-07-18 03:37:32.176332 pydantic_neo4j-0.3.0/pydantic_neo4j/graph_base_models.py
+-rw-r--r--   0        0        0     8489 2023-07-18 03:28:16.295585 pydantic_neo4j-0.3.0/pydantic_neo4j/match_operations.py
+-rw-r--r--   0        0        0     1268 2023-07-18 02:22:59.959087 pydantic_neo4j-0.3.0/pydantic_neo4j/pydantic_neo4j.py
+-rw-r--r--   0        0        0      601 2023-07-18 03:47:13.992694 pydantic_neo4j-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4039 2023-07-18 03:47:13.985687 pydantic_neo4j-0.3.0/README.md
+-rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 pydantic_neo4j-0.3.0/PKG-INFO
```

### Comparing `pydantic_neo4j-0.2.1/pydantic_neo4j/__init__.py` & `pydantic_neo4j-0.3.0/pydantic_neo4j/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from .pydantic_neo4j import PydanticNeo4j as PydanticNeo4j
 from .graph_base_models import NodeModel as NodeModel
 from .graph_base_models import RelationshipModel as RelationshipModel
 from .graph_base_models import RelationshipQueryModel as RelationshipQueryModel
-from .graph_base_models import SequenceCriteriaModel as SequenceCriteriaModel
+from .graph_base_models import SequenceCriteriaNodeModel as SequenceCriteriaNodeModel
+from .graph_base_models import SequenceCriteriaRelationshipModel as SequenceCriteriaRelationshipModel
 from .graph_base_models import SequenceQueryModel as SequenceQueryModel
 from .graph_base_models import SequenceNodeModel as SequenceNodeModel
 
-
 __all__ = [PydanticNeo4j,
            NodeModel,
            RelationshipModel,
            RelationshipQueryModel,
-           SequenceCriteriaModel,
+           SequenceCriteriaNodeModel,
+           SequenceCriteriaRelationshipModel,
            SequenceQueryModel,
            SequenceNodeModel]
```

### Comparing `pydantic_neo4j-0.2.1/pydantic_neo4j/create_operations.py` & `pydantic_neo4j-0.3.0/pydantic_neo4j/create_operations.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.2.1/pydantic_neo4j/database_operations.py` & `pydantic_neo4j-0.3.0/pydantic_neo4j/database_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 import datetime
 import importlib
 import random
 import string
 import uuid
+from enum import Enum, auto
 
 import neo4j
 
 from typing import Any, Type
 
-from .graph_base_models import Neo4jModel
+from .graph_base_models import Neo4jModel, NodeModel, RelationshipModel
+
+
+class NeoObjectType(Enum):
+    NODE = auto()
+    RELATIONSHIP = auto()
 
 
 class DatabaseOperations:
 
     def __init__(self, uri: str, username: str, password: str):
         self.driver = neo4j.AsyncGraphDatabase.driver(uri, auth=(username, password))
 
     async def run_query(self, query: str, **kwargs) -> neo4j.EagerResult:
         async with self.driver.session() as session:
             result = await session.run(query, **kwargs)
             eager_results = await result.to_eager_result()
         return eager_results
 
     @staticmethod
+    def get_object_type(neo_object: Type[Neo4jModel]):
+        if issubclass(neo_object, NodeModel):
+            return NeoObjectType.NODE
+        elif issubclass(neo_object, RelationshipModel):
+            return NeoObjectType.RELATIONSHIP
+
+    @staticmethod
     def str_to_class(model: Type[Neo4jModel], **kwargs) -> Any | None:
         """Return a class instance from a string reference"""
 
         try:
             module_ = importlib.import_module(model.__module__)
             # try:
             class_ = getattr(module_, model.__name__)(**kwargs)
```

### Comparing `pydantic_neo4j-0.2.1/pydantic_neo4j/graph_base_models.py` & `pydantic_neo4j-0.3.0/pydantic_neo4j/graph_base_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         """Fields needed for minimum compatibility between create and match modules"""
         fields = {}
         for field, value in self.__class__.model_fields.items():
             if value.is_required():
                 fields[field] = getattr(self, field)
         return fields
 
-
     def get_identifying_fields(self) -> Dict[str, Union[uuid.UUID]]:
         fields = {}
         for field, value in self.__class__.model_fields.items():
             if value.annotation == uuid.UUID or value.annotation == Optional[uuid.UUID]:
                 fields[field] = getattr(self, field)
         return fields
 
@@ -71,17 +70,26 @@
 
 class SequenceCriteriaModel(BaseModel):
     name: Optional[str] = Field(default="")
     criteria: Optional[Dict] = Field(default_factory=dict)
     include_with_return: Optional[bool] = Field(default=False)
 
 
+class SequenceCriteriaNodeModel(SequenceCriteriaModel):
+    pass
+
+
+class SequenceCriteriaRelationshipModel(SequenceCriteriaModel):
+    from_symbol: str = Field(default="-")
+    to_symbol: str = Field(default="-")
+
+
 class SequenceQueryModel(BaseModel):
-    node_sequence: Optional[list[SequenceCriteriaModel]] = Field(default_factory=list)
-    relationship_sequence: Optional[list[SequenceCriteriaModel]] = Field(
+    node_sequence: Optional[list[SequenceCriteriaNodeModel]] = Field(default_factory=list)
+    relationship_sequence: Optional[list[SequenceCriteriaRelationshipModel]] = Field(
         default_factory=list
     )
 
 
 class SequenceNodeModel(BaseModel):
     nodes: Optional[dict[str, NodeModel]] = Field(default_factory=dict)
     relationships: Optional[dict[str, RelationshipModel]] = Field(default_factory=dict)
```

### Comparing `pydantic_neo4j-0.2.1/pydantic_neo4j/pydantic_neo4j.py` & `pydantic_neo4j-0.3.0/pydantic_neo4j/pydantic_neo4j.py`

 * *Files identical despite different names*

### Comparing `pydantic_neo4j-0.2.1/pyproject.toml` & `pydantic_neo4j-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-neo4j"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["MichaelZag <Michael@MichaelZag.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = 'https://github.com/Michaelzag/PydanticNeo4j'
 repository = 'https://github.com/Michaelzag/PydanticNeo4j'
 keywords = ['neo4j-pydantic','Pydantic', 'Neo4j', 'OGM', 'Neo4j-OG','MichaelZag']
@@ -14,11 +14,10 @@
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0.3"
 neo4j = "^5.10.0"
 
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydantic_neo4j-0.2.1/PKG-INFO` & `pydantic_neo4j-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-neo4j
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/Michaelzag/PydanticNeo4j
 License: MIT
 Keywords: neo4j-pydantic,Pydantic,Neo4j,OGM,Neo4j-OG,MichaelZag
 Author: MichaelZag
 Author-email: Michael@MichaelZag.com
 Requires-Python: >=3.11,<4.0
@@ -29,15 +29,16 @@
 
 ## Usage
 + Import the package and models
 ```python
 from pydantic_neo4j import (PydanticNeo4j, 
                             RelationshipQueryModel,
                             NodeModel,
-                            SequenceCriteriaModel, 
+                            SequenceCriteriaNodeModel,
+                            SequenceCriteriaRelationshipModel,  
                             SequenceQueryModel, 
                             SequenceNodeModel)
 ```
 ___
 + Initialize the class and get the utilities
 ```python
 
@@ -97,14 +98,15 @@
 ```
 + Query the graph for multiple nodes. Lets find all nodes that are active
 ```python
 nodes = await match_util.node_query(criteria={'active': True})
 ```
 ___
 + Query the graph for a single relationship. Lets find a manufacturer that produces a red design
++ This will be depreciated soon, use sequence query instead
 ```python
 query = RelationshipQueryModel(
     start_node_name="Manufacturer",
     start_criteria={},
     end_node_name="Design",
     end_criteria={"color": "red"},
     relationship_name="Produces",
@@ -113,19 +115,19 @@
 ```
 ___
 + Query the graph for multiple relationships. Lets find all manufacturers that make a widget component
 + This uses a sequence, which is a series of relationships. Similar to Neo4j Path
 ```python
 sequence_query = SequenceQueryModel()
 
-sequence_query.node_sequence.append(SequenceCriteriaModel(name='Manufacturer'))
-sequence_query.relationship_sequence.append(SequenceCriteriaModel()) # a relationship with no criteria
-sequence_query.node_sequence.append(SequenceCriteriaModel() # a node with no criteria specified
-sequence_query.relationship_sequence.append(SequenceCriteriaModel()) #a realtoinship with no criteria
-sequence_query.node_sequence.append(SequenceCriteriaModel(component_type="widget", 
+sequence_query.node_sequence.append(SequenceCriteriaNodeModel(name='Manufacturer'))
+sequence_query.relationship_sequence.append(SequenceCriteriaRelationshipModel()) # a relationship with no criteria
+sequence_query.node_sequence.append(SequenceCriteriaNodeModel() # a node with no criteria specified
+sequence_query.relationship_sequence.append(SequenceCriteriaRelationshipModel()) #a realtoinship with no criteria
+sequence_query.node_sequence.append(SequenceCriteriaNodeModel(component_type="widget", 
                                                           include_with_return=True))
 ```
 + The sequence query must always have 1 more node than relationship.
 + The order is important, and is a sequence. node - relationship - node - relationship - node
 ```python
 result = await match_util.sequence_query(sequence_query=sequence_query)
 ```
@@ -136,37 +138,14 @@
 ```
 
 
 
 ### Not Implemented
 
 + Update a node
-```python
-nodes = await match_util.node_query(name='Manufacturer', criteria={name='Acme'})
-for graph_id, node in nodes.items():
-    node.name = "Acme2"
-    await create_util.update_node(node=node)
-```
 ___
-+ Update a relationship
-```python
-    query = RelationshipQueryModel(
-    start_node_name="Manufacturer",
-    start_criteria={},
-    end_node_name="Design",
-    end_criteria={"color": "red"},
-    relationship_name="Produces",
-    relationship_criteria={})
-    result = await match_util.match_relationship(query=query)
-    for graph_id, relationship in result.items():
-        relationship.design_revision = 4
-        await create_util.update_relationship(relationship=relationship)
-```
++ Update a sequence
 ___
 + Delete a node
-```python
-nodes = await match_util.node_query(name='Manufacturer', criteria={name='Acme'})
-for graph_id, node in nodes.items():
-    await create_util.delete_node(node=node)
-```
+___
```

