# Comparing `tmp/kodexa-6.3.35586420712.tar.gz` & `tmp/kodexa-6.3.35592112892.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.3.35586420712.tar", max compression
+gzip compressed data, was "kodexa-6.3.35592112892.tar", max compression
```

## Comparing `kodexa-6.3.35586420712.tar` & `kodexa-6.3.35592112892.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-07-18 10:42:22.415647 kodexa-6.3.35586420712/LICENSE
--rw-r--r--   0        0        0     2804 2023-07-18 10:42:22.415647 kodexa-6.3.35586420712/README.md
--rw-r--r--   0        0        0      847 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/model/__init__.py
--rw-r--r--   0        0        0      856 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/model/base.py
--rw-r--r--   0        0        0    97073 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/model/model.py
--rw-r--r--   0        0        0   118091 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/model/objects.py
--rw-r--r--   0        0        0    38744 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19505 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   112675 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/platform/client.py
--rw-r--r--   0        0        0    28020 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 10:42:22.423647 kodexa-6.3.35586420712/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1279 2023-07-18 10:42:40.136050 kodexa-6.3.35586420712/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35586420712/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-18 20:32:57.639345 kodexa-6.3.35592112892/LICENSE
+-rw-r--r--   0        0        0     2804 2023-07-18 20:32:57.639345 kodexa-6.3.35592112892/README.md
+-rw-r--r--   0        0        0      847 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      856 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/model/base.py
+-rw-r--r--   0        0        0    97073 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/model/model.py
+-rw-r--r--   0        0        0   118132 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38744 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19505 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   112470 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/platform/client.py
+-rw-r--r--   0        0        0    28020 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-07-18 20:32:57.647345 kodexa-6.3.35592112892/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-07-18 20:32:57.651345 kodexa-6.3.35592112892/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-07-18 20:32:57.651345 kodexa-6.3.35592112892/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-07-18 20:32:57.651345 kodexa-6.3.35592112892/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-18 20:32:57.651345 kodexa-6.3.35592112892/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-07-18 20:32:57.651345 kodexa-6.3.35592112892/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-07-18 20:32:57.651345 kodexa-6.3.35592112892/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 20:32:57.651345 kodexa-6.3.35592112892/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1279 2023-07-18 20:33:18.259702 kodexa-6.3.35592112892/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35592112892/PKG-INFO
```

### Comparing `kodexa-6.3.35586420712/LICENSE` & `kodexa-6.3.35592112892/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/README.md` & `kodexa-6.3.35592112892/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/__init__.py` & `kodexa-6.3.35592112892/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/assistant/assistant.py` & `kodexa-6.3.35592112892/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/connectors/connectors.py` & `kodexa-6.3.35592112892/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/model/__init__.py` & `kodexa-6.3.35592112892/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/model/base.py` & `kodexa-6.3.35592112892/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/model/model.py` & `kodexa-6.3.35592112892/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/model/objects.py` & `kodexa-6.3.35592112892/kodexa/model/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -3310,7 +3310,8 @@
 AssistantEvent.model_rebuild()
 ContentEvent.model_rebuild()
 DataObjectEvent.model_rebuild()
 DocumentFamilyEvent.model_rebuild()
 ScheduledEvent.model_rebuild()
 DataException.model_rebuild()
 Workspace.model_rebuild()
+AssistantResponsePipeline.model_rebuild()
```

### Comparing `kodexa-6.3.35586420712/kodexa/model/persistence.py` & `kodexa-6.3.35592112892/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/pipeline/pipeline.py` & `kodexa-6.3.35592112892/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/platform/client.py` & `kodexa-6.3.35592112892/kodexa/platform/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import time
 from pathlib import Path
 from typing import Type, Optional, List, Dict, Any, ClassVar
 
 import requests
 from functional import seq
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from pydantic_yaml import to_yaml_str
 
 from kodexa.model import Taxonomy, Document
 from kodexa.model.base import BaseEntity
 from kodexa.model.objects import PageStore, PageTaxonomy, PageProject, PageOrganization, Project, Organization, \
     PlatformOverview, DocumentFamily, DocumentContentMetadata, ModelContentMetadata, ExtensionPack, Pipeline, \
     AssistantDefinition, Action, ModelRuntime, CredentialDefinition, Execution, PageAssistantDefinition, \
@@ -70,15 +70,15 @@
         return self
 
 
 class ClientEndpoint(BaseModel):
     """
     Represents a client endpoint
     """
-    client: Optional["KodexaClient"] = None
+    client: Optional["KodexaClient"] = Field(exclude=True)
 
     def set_client(self, client):
         """
         Set the client that this endpoint is associated with
         :param client: The client to set
         :return: The endpoint
         """
@@ -88,29 +88,24 @@
         return self
 
     def yaml(self, **kwargs):
         """
         Convert the client endpoint to a yaml string
         :return: A yaml string representation of the endpoint
         """
-        if 'exclude' in kwargs:
-            kwargs['exclude']['client']
-        else:
-            kwargs['exclude'] = {'client'}
-
         kwargs['exclude_unset'] = True
         kwargs['exclude_none'] = True
 
         return to_yaml_str(self, **kwargs)
 
     def detach(self):
         """
         Detach the client from the endpoint
         """
-        return self.copy(exclude={'client'})
+        return self.model_copy()
 
 
 class ProjectResourceEndpoint(ClientEndpoint):
     """
     Represents a project resource endpoint
     """
     project: Optional["ProjectEndpoint"]
@@ -414,15 +409,15 @@
         get_response = self.client.get(url)
         return self.get_instance_class().model_validate(get_response.json()).set_client(self.client)
 
     def create(self, new_entity: EntityEndpoint) -> EntityEndpoint:
         """Create an entity"""
         url = f"/api/{self.get_type()}"
 
-        create_response = self.client.post(url, body=json.loads(new_entity.json(exclude={'client'}, by_alias=True)))
+        create_response = self.client.post(url, body=json.loads(new_entity.model_dump_json(by_alias=True)))
         return self.get_instance_class().model_validate(create_response.json()).set_client(self.client)
 
     def delete(self, self_id: str) -> None:
         """Delete an entity by id"""
         url = f"/api/{self.get_type()}/{self_id}"
         self.client.delete(url)
 
@@ -494,15 +489,15 @@
 
     def to_endpoints(self):
         """
         Convert the page to endpoints
         :return:
         """
         self.content = seq(self.content).map(
-            lambda x: self.client.deserialize(x.dict(exclude={'client'}, by_alias=True),
+            lambda x: self.client.deserialize(x.dict(by_alias=True),
                                               component_type=self.get_type())).to_list()
         return self
 
 
 class PageTaxonomyEndpoint(PageTaxonomy, PageEndpoint):
     pass
 
@@ -1059,15 +1054,15 @@
         """Get the tags of the project"""
         response = self.client.get(f"/api/projects/{self.id}/tags")
         return [ProjectTag.model_validate(tag) for tag in response.json()]
 
     def update_tags(self, tags: List[ProjectTag]) -> List[ProjectTag]:
         """Update the tags of the project"""
         response = self.client.put(f"/api/projects/{self.id}/tags",
-                                   body=[tag.dict(exclude={'client'}, by_alias=True) for tag in tags])
+                                   body=[tag.to_dict(by_alias=True) for tag in tags])
         return [ProjectTag.model_validate(tag) for tag in response.json()]
 
 
 class ChannelsEndpoint(EntitiesEndpoint):
     """Represents a channels endpoint"""
 
     def get_type(self) -> str:
@@ -1177,15 +1172,15 @@
                 raise Exception("Organization not set on the project")
 
         if template_ref is not None:
             params = {"templateRef": template_ref}
         else:
             params = None
 
-        create_response = self.client.post(url, body=json.loads(project.json(exclude={'client'}, by_alias=True)),
+        create_response = self.client.post(url, body=json.loads(project.model_dump_json(by_alias=True)),
                                            params=params)
         return ProjectEndpoint.model_validate(create_response.json()).set_client(self.client)
 
 
 class StoresEndpoint(ComponentEndpoint, ClientEndpoint, OrganizationOwned):
     """Represents a stores endpoint"""
 
@@ -2362,15 +2357,15 @@
 
         response = self.client.post(url, body=json.loads(new_training.json(by_alias=True)))
         return ModelTraining.model_validate(response.json())
 
     def update_training(self, training: ModelTraining) -> ModelTraining:
         """Update a model training"""
         url = f"/api/stores/{self.ref.replace(':', '/')}/trainings/{training.id}"
-        response = self.client.put(url, body=json.loads(training.json(exclude={'client'}, by_alias=True)))
+        response = self.client.put(url, body=json.loads(training.model_dump_json(by_alias=True)))
         return ModelTraining.model_validate(response.json())
 
     def delete_training(self, training_id: str):
         """Delete a model training"""
         url = f"/api/stores/{self.ref.replace(':', '/')}/trainings/{training_id}"
         self.client.delete(url)
 
@@ -2624,32 +2619,32 @@
     """
 
     def __init__(self, client: "KodexaClient"):
         self.client = client
 
     def extract_data_objects(self, taxonomy: Taxonomy, document: Document) -> List[DataObject]:
         response = self.client.post(f"/api/extractionEngine/extract",
-                                    data={'taxonomyJson': taxonomy.json(exclude={'client'})},
+                                    data={'taxonomyJson': taxonomy.model_dump_json()},
                                     files={'document': document.to_kddb()})
         return [DataObject.model_validate(data_object) for data_object in response.json()]
 
     def extract_data_objects_with_exceptions(self, taxonomy: Taxonomy, document: Document) -> Dict:
         response = self.client.post(f"/api/extractionEngine/extract", params="full",
-                                    data={'taxonomyJson': taxonomy.json(exclude={'client'})},
+                                    data={'taxonomyJson': taxonomy.model_dump_json()},
                                     files={'document': document.to_kddb()})
         return {
             'dataObjects': [DataObject.model_validate(data_object) for data_object in response.json()['dataObjects']],
             'exceptions': [ContentException.model_validate(exception) for exception in
                            response.json()['contentExceptions']]
         }
 
     def extract_to_format(self, taxonomy: Taxonomy, document: Document, format: str) -> str:
         response = self.client.post(f"/api/extractionEngine/extract",
                                     params={'format': format},
-                                    data={'taxonomyJson': taxonomy.json(exclude={'client'})},
+                                    data={'taxonomyJson': taxonomy.model_dump_json()},
                                     files={'document': document.to_kddb()})
         return response.text
 
 
 class KodexaClient:
 
     def __init__(self, url=None, access_token=None, profile=None, insecure=None):
```

### Comparing `kodexa-6.3.35586420712/kodexa/platform/kodexa.py` & `kodexa-6.3.35592112892/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/selectors/ast.py` & `kodexa-6.3.35592112892/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/selectors/core.py` & `kodexa-6.3.35592112892/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/selectors/lexrules.py` & `kodexa-6.3.35592112892/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/selectors/lextab.py` & `kodexa-6.3.35592112892/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/selectors/parserules.py` & `kodexa-6.3.35592112892/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/selectors/parsetab.py` & `kodexa-6.3.35592112892/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/spatial/azure_models.py` & `kodexa-6.3.35592112892/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/spatial/bbox_common.py` & `kodexa-6.3.35592112892/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/spatial/table_form_common.py` & `kodexa-6.3.35592112892/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/steps/common.py` & `kodexa-6.3.35592112892/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/testing/test_components.py` & `kodexa-6.3.35592112892/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/kodexa/testing/test_utils.py` & `kodexa-6.3.35592112892/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35586420712/pyproject.toml` & `kodexa-6.3.35592112892/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.3.35586420712"
+version = "6.3.35592112892"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.3.35586420712/PKG-INFO` & `kodexa-6.3.35592112892/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.3.35586420712
+Version: 6.3.35592112892
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

