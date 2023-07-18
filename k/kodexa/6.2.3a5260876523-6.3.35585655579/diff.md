# Comparing `tmp/kodexa-6.2.3a5260876523.tar.gz` & `tmp/kodexa-6.3.35585655579.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.2.3a5260876523.tar", max compression
+gzip compressed data, was "kodexa-6.3.35585655579.tar", max compression
```

## Comparing `kodexa-6.2.3a5260876523.tar` & `kodexa-6.3.35585655579.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-06-13 22:16:32.730222 kodexa-6.2.3a5260876523/LICENSE
--rw-r--r--   0        0        0     2804 2023-06-13 22:16:32.730222 kodexa-6.2.3a5260876523/README.md
--rw-r--r--   0        0        0      847 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/model/__init__.py
--rw-r--r--   0        0        0      753 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/model/base.py
--rw-r--r--   0        0        0    96608 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/model/model.py
--rw-r--r--   0        0        0   118104 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/model/objects.py
--rw-r--r--   0        0        0    38334 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19763 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   111822 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/platform/client.py
--rw-r--r--   0        0        0    26888 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-06-13 22:16:32.738222 kodexa-6.2.3a5260876523/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 22:16:32.742222 kodexa-6.2.3a5260876523/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1302 2023-06-13 22:16:56.267083 kodexa-6.2.3a5260876523/pyproject.toml
--rw-r--r--   0        0        0     4104 1970-01-01 00:00:00.000000 kodexa-6.2.3a5260876523/setup.py
--rw-r--r--   0        0        0     4159 1970-01-01 00:00:00.000000 kodexa-6.2.3a5260876523/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-18 09:23:24.306439 kodexa-6.3.35585655579/LICENSE
+-rw-r--r--   0        0        0     2804 2023-07-18 09:23:24.306439 kodexa-6.3.35585655579/README.md
+-rw-r--r--   0        0        0      847 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      856 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/model/base.py
+-rw-r--r--   0        0        0    97073 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/model/model.py
+-rw-r--r--   0        0        0   118091 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38744 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19505 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   112675 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/platform/client.py
+-rw-r--r--   0        0        0    28020 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 09:23:24.314439 kodexa-6.3.35585655579/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1261 2023-07-18 09:23:38.402340 kodexa-6.3.35585655579/pyproject.toml
+-rw-r--r--   0        0        0     4032 1970-01-01 00:00:00.000000 kodexa-6.3.35585655579/PKG-INFO
```

### Comparing `kodexa-6.2.3a5260876523/LICENSE` & `kodexa-6.3.35585655579/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/README.md` & `kodexa-6.3.35585655579/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/__init__.py` & `kodexa-6.3.35585655579/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/assistant/assistant.py` & `kodexa-6.3.35585655579/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/connectors/connectors.py` & `kodexa-6.3.35585655579/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/model/__init__.py` & `kodexa-6.3.35585655579/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/model/model.py` & `kodexa-6.3.35585655579/kodexa/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,27 +46,28 @@
         super().__init__(*args, **kwargs)
 
 
 class ContentException(Dict):
     """A content exception represents an issue identified during labeling or validation at the document level"""
 
     def __init__(self, exception_type: str, message: str, severity: str = 'ERROR', tag: Optional[str] = None,
-                 group_uuid: Optional[str] = None, tag_uuid: Optional[str] = None,
+                 group_uuid: Optional[str] = None, tag_uuid: Optional[str] = None, exception_type_id: Optional[str] = None,
                  exception_details: Optional[str] = None, node_uuid: Optional[str] = None, value: Optional[str] = None,
                  *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.tag = tag
         self.message = message
         self.exception_details = exception_details
         self.group_uuid = group_uuid
         self.tag_uuid = tag_uuid
         self.exception_type = exception_type
         self.node_uuid = node_uuid
         self.severity = severity
         self.value = value
+        self.exception_type_id = exception_type_id
 
 
 class Tag(Dict):
     """A tag represents the metadata for a label that is applies as a feature on a content node"""
 
     def __init__(self, start: Optional[int] = None, end: Optional[int] = None, value: Optional[str] = None,
                  uuid: Optional[str] = None, data: Any = None, *args, confidence: Optional[float] = None,
@@ -1840,15 +1841,15 @@
         return node
 
 
 class Document(object):
     """A Document is a collection of metadata and a set of content nodes."""
 
     PREVIOUS_VERSION: str = "1.0.0"
-    CURRENT_VERSION: str = "4.0.2"
+    CURRENT_VERSION: str = "6.0.0"
 
     def __str__(self):
         return f"kodexa://{self.uuid}"
 
     def add_exception(self, exception: ContentException):
         self._persistence_layer.add_exception(exception)
 
@@ -2324,19 +2325,25 @@
                     load the KDDB to it
             detached (bool): if reading from a file we will create a copy so we don't update in place
 
         :return: the document
         """
         if isinstance(source, str):
             if isinstance(source, str):
-                document = Document(kddb_path=source)
-            if detached:
-                return Document.from_kddb(document.to_kddb())
 
-            return document
+                # If we are using the detached flag we will create a copy of the KDDB file
+                if detached:
+                    import tempfile
+                    from kodexa import KodexaPlatform
+                    fp = tempfile.NamedTemporaryFile(suffix='.kddb', delete=False, dir=KodexaPlatform.get_tempdir())
+                    fp.write(open(source, 'rb').read())
+                    fp.close()
+                    return Document(kddb_path=fp.name, delete_on_close=True)
+
+                return Document(kddb_path=source)
 
         # We will assume the input is of byte type
         import tempfile
         from kodexa import KodexaPlatform
         fp = tempfile.NamedTemporaryFile(suffix='.kddb', delete=False, dir=KodexaPlatform.get_tempdir())
         fp.write(source)
         fp.close()
```

### Comparing `kodexa-6.2.3a5260876523/kodexa/model/objects.py` & `kodexa-6.3.35585655579/kodexa/model/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import AnyUrl, Field, constr
+from pydantic import AnyUrl, Field, constr, RootModel
 
-from kodexa.model.base import KodexaBaseModel
+from kodexa.model.base import KodexaBaseModel, StandardDateTime
 
 
 class ExceptionResponse(KodexaBaseModel):
-    date_time: Optional[datetime] = Field(None, alias='dateTime')
+    date_time: Optional[StandardDateTime] = Field(None, alias='dateTime')
     message: Optional[str] = None
     incident_id: Optional[str] = Field(None, alias='incidentId')
     context_path: Optional[str] = Field(None, alias='contextPath')
     errors: Optional[Dict[str, Any]] = None
     stack_trace: Optional[str] = Field(None, alias='stackTrace')
     root_cause_stack_trace: Optional[List[str]] = Field(
         None, alias='rootCauseStackTrace'
@@ -102,28 +102,28 @@
     reset_token: str = Field(..., alias='resetToken')
     password: str
 
 
 class Organization(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     name: str
-    slug: constr(regex=r'^[a-zA-Z0-9\-_]{0,100}$')
+    slug: constr(pattern=r'^[a-zA-Z0-9\-_]{0,100}$')
     public_access: Optional[bool] = Field(None, alias='publicAccess')
     description: Optional[str] = None
     has_image: Optional[bool] = Field(None, alias='hasImage')
 
 
 class Team(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     name: Optional[str] = None
     description: Optional[str] = None
     organization: Optional[Organization] = None
 
 
 class AssistantImplementation(KodexaBaseModel):
     """
@@ -403,16 +403,16 @@
 class ScheduleDefinition(KodexaBaseModel):
     """
     The default schedules that the assistant has
     """
 
     type: Optional[str] = None
     cron_expression: Optional[str] = Field(None, alias='cronExpression')
-    last_event: Optional[datetime] = Field(None, alias='lastEvent')
-    next_event: Optional[datetime] = Field(None, alias='nextEvent')
+    last_event: Optional[StandardDateTime] = Field(None, alias='lastEvent')
+    next_event: Optional[StandardDateTime] = Field(None, alias='nextEvent')
 
 
 class SelectionOption(KodexaBaseModel):
     """
     If data type is SELECTION, this is the list of available options
     """
 
@@ -431,26 +431,26 @@
         None, alias='schemaVersion', description='The version of the schema'
     )
     org_slug: Optional[str] = Field(
         None,
         alias='orgSlug',
         description='The slug of the organization that owns this metadata object',
     )
-    slug: constr(regex=r'^[a-zA-Z0-9\-_]{0,255}$') = Field(
+    slug: constr(pattern=r'^[a-zA-Z0-9\-_]{0,255}$') = Field(
         ..., description='The slug used when referencing this metadata object'
     )
     type: str = Field(..., description='The type of metadata object')
     name: str = Field(..., description='The name of the object')
     description: Optional[str] = Field(
         None, description='The description of the object'
     )
-    version: Optional[constr(regex=r'^\d+\.\d+\.\d+(?:\-\d+)?$')] = Field(
+    version: Optional[constr(pattern=r'^\d+\.\d+\.\d+(?:\-\d+)?$')] = Field(
         None, description='The version of the object'
     )
-    deployed: Optional[datetime] = Field(
+    deployed: Optional[StandardDateTime] = Field(
         None,
         description='The date/time the object was deployed into this Kodexa instance',
     )
     public_access: Optional[bool] = Field(
         None,
         alias='publicAccess',
         description='Is the metadata object publicly accessible by other organizations',
@@ -604,29 +604,29 @@
     family_ids: Optional[List[str]] = Field(None, alias='familyIds')
     all: Optional[bool] = None
 
 
 class AssistantSchedule(KodexaBaseModel):
     type: Optional[str] = None
     cron_expression: Optional[str] = Field(None, alias='cronExpression')
-    last_event: Optional[datetime] = Field(None, alias='lastEvent')
-    next_event: Optional[datetime] = Field(None, alias='nextEvent')
+    last_event: Optional[StandardDateTime] = Field(None, alias='lastEvent')
+    next_event: Optional[StandardDateTime] = Field(None, alias='nextEvent')
     id: Optional[str] = None
 
 
 class StatusType1(Enum):
     unresolved = 'UNRESOLVED'
     resolved = 'RESOLVED'
 
 
 class AttributeStatus(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     color: Optional[str] = None
     icon: Optional[str] = None
     status: Optional[str] = None
     status_type: Optional[StatusType1] = Field(None, alias='statusType')
 
 
 class ContentClassification(KodexaBaseModel):
@@ -679,16 +679,16 @@
     unresolved = 'UNRESOLVED'
     resolved = 'RESOLVED'
 
 
 class DocumentStatus(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     color: Optional[str] = None
     icon: Optional[str] = None
     status: str
     status_type: Optional[StatusType2] = Field(None, alias='statusType')
 
 
 class TransitionType(Enum):
@@ -702,22 +702,22 @@
 class DocumentTransition(KodexaBaseModel):
     """
     Provides the definition of a transition for a document, where a change was applied by an assistant, user or external process
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     unknown_fields: Optional[Dict[str, str]] = Field(None, alias='unknownFields')
     transition_type: Optional[TransitionType] = Field(
         None, alias='transitionType', description='The type of transition'
     )
     index: Optional[int] = None
-    date_time: Optional[datetime] = Field(
+    date_time: Optional[StandardDateTime] = Field(
         None, alias='dateTime', description='The date/time of the transition'
     )
     actor: Optional[DocumentActor] = None
     label: Optional[str] = Field(
         None,
         description='A label for the transition (this can be used later if we want to prune based on a label)',
     )
@@ -791,16 +791,16 @@
 class Label(KodexaBaseModel):
     """
     The labels from the latest content object in the family
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     name: str
     color: Optional[str] = None
     label: str
 
 
 class ProjectTag(KodexaBaseModel):
     """
@@ -822,30 +822,30 @@
 
 
 class ProjectMemory(KodexaBaseModel):
     recent_filters: Optional[Dict[str, List[str]]] = Field(None, alias='recentFilters')
 
 
 class ProjectMetadata(KodexaBaseModel):
-    tags: Optional[List[str]] = Field(default_factory=list, unique_items=True)
+    tags: Optional[List[str]] = Field(default_factory=list, set=True)
 
 
 class State1(Enum):
     open = 'OPEN'
     closed = 'CLOSED'
 
 
 class Session(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     state: State1
     token: Optional[str] = None
-    last_accessed: Optional[datetime] = Field(None, alias='lastAccessed')
+    last_accessed: Optional[StandardDateTime] = Field(None, alias='lastAccessed')
 
 
 class Status4(Enum):
     pending = 'PENDING'
     running = 'RUNNING'
     succeeded = 'SUCCEEDED'
     failed = 'FAILED'
@@ -863,16 +863,16 @@
     progress_max: Optional[int] = Field(None, alias='progressMax')
     progress: Optional[int] = None
 
 
 class ValidationError(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     message: Optional[str] = None
     option: Optional[str] = None
     description: Optional[str] = None
 
 
 class ValidationResults(KodexaBaseModel):
     instances: Optional[List[ValidationError]] = None
@@ -903,16 +903,16 @@
 class DataException(KodexaBaseModel):
     """
     A data exception
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     message: str
     exception_details: Optional[str] = Field(None, alias='exceptionDetails')
     severity: Optional[str] = None
     exception_type: Optional[str] = Field(None, alias='exceptionType')
     closing_comment: Optional[str] = Field(None, alias='closingComment')
     open: Optional[bool] = None
     data_object: Optional[DataObject] = Field(None, alias='dataObject')
@@ -979,16 +979,16 @@
     parameters: Optional[Dict[str, Any]] = None
     payload: Optional[Dict[str, Any]] = None
 
 
 class PlatformConfiguration(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     welcome_markdown: Optional[str] = Field(None, alias='welcomeMarkdown')
     news_markdown: Optional[str] = Field(None, alias='newsMarkdown')
     about_markdown: Optional[str] = Field(None, alias='aboutMarkdown')
     login_message: Optional[str] = Field(None, alias='loginMessage')
     base_org_slug: Optional[str] = Field(None, alias='baseOrgSlug')
     title: Optional[str] = None
     organization_title: Optional[str] = Field(None, alias='organizationTitle')
@@ -1015,17 +1015,17 @@
 
 class ModelTraining(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
     name: Optional[str] = None
     state: Optional[str] = None
     training_materials_generated: Optional[bool] = Field(None, alias='trainingMaterialsGenerated')
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
-    training_date: Optional[datetime] = Field(None, alias='trainingDate')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
+    training_date: Optional[StandardDateTime] = Field(None, alias='trainingDate')
     content: Optional[bool] = Field(None, description='Has content')
     user_test: Optional[bool] = Field(None, alias='userTest')
 
     properties: Optional[Dict[str, Any]] = None
     training_parameters: Optional[Dict[str, Any]] = Field(
         None,
         alias='trainingParameters',
@@ -1072,17 +1072,17 @@
     cancelled = 'CANCELLED'
     pending_reprocessing = 'PENDING_REPROCESSING'
 
 
 class ExecutionLogEntry(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
-    log_date: Optional[datetime] = Field(None, alias='logDate')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
+    log_date: Optional[StandardDateTime] = Field(None, alias='logDate')
     entry: Optional[str] = None
 
 
 class LoginRequest(KodexaBaseModel):
     email: str
     password: str
 
@@ -1161,21 +1161,21 @@
 class StoreStatistics(KodexaBaseModel):
     """
     Statistics for the contents of the store instance
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     statistic_name: Optional[str] = Field(None, alias='statisticName')
     label: Optional[str] = None
     count: Optional[int] = None
     size: Optional[int] = None
-    point_in_time: Optional[datetime] = Field(None, alias='pointInTime')
+    point_in_time: Optional[StandardDateTime] = Field(None, alias='pointInTime')
 
 
 class SearchEntity(KodexaBaseModel):
     """
     Entities identified in search content
     """
 
@@ -1193,15 +1193,15 @@
 
 
 class DataAttributeValues(KodexaBaseModel):
     value: Optional[str] = None
     truncated: Optional[bool] = None
     tag: str
     tag_uuid: Optional[str] = Field(None, alias='tagUuid')
-    date_value: Optional[datetime] = Field(None, alias='dateValue')
+    date_value: Optional[StandardDateTime] = Field(None, alias='dateValue')
     float_value: Optional[float] = Field(None, alias='floatValue')
     decimal_value: Optional[float] = Field(None, alias='decimalValue')
     number_value: Optional[int] = Field(None, alias='numberValue')
     boolean_value: Optional[bool] = Field(None, alias='booleanValue')
     string_value: Optional[str] = Field(None, alias='stringValue')
     attribute_status: Optional[AttributeStatus] = Field(None, alias='attributeStatus')
     confidence: Optional[float] = None
@@ -1215,23 +1215,23 @@
 class User(KodexaBaseModel):
     """
     A user within the Kodexa platform
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     email: str
     first_name: str = Field(..., alias='firstName')
     last_name: str = Field(..., alias='lastName')
     activated: Optional[bool] = None
     platform_admin: Optional[bool] = Field(None, alias='platformAdmin')
-    password_reset_date: Optional[datetime] = Field(None, alias='passwordResetDate')
-    last_connected: Optional[datetime] = Field(None, alias='lastConnected')
+    password_reset_date: Optional[StandardDateTime] = Field(None, alias='passwordResetDate')
+    last_connected: Optional[StandardDateTime] = Field(None, alias='lastConnected')
     user_storage: Optional[UserStorage] = Field(None, alias='userStorage')
     has_image: Optional[bool] = Field(None, alias='hasImage')
     show_developer_tools: Optional[bool] = Field(None, alias='showDeveloperTools')
 
 
 class DeploymentMetadata(KodexaBaseModel):
     deployment_type: Optional[DeploymentType] = Field(None, alias='deploymentType')
@@ -1275,26 +1275,26 @@
         None, alias='schemaVersion', description='The version of the schema'
     )
     org_slug: Optional[str] = Field(
         None,
         alias='orgSlug',
         description='The slug of the organization that owns this metadata object',
     )
-    slug: constr(regex=r'^[a-zA-Z0-9\-_]{0,255}$') = Field(
+    slug: constr(pattern=r'^[a-zA-Z0-9\-_]{0,255}$') = Field(
         ..., description='The slug used when referencing this metadata object'
     )
     type: str = Field(..., description='The type of metadata object')
     name: str = Field(..., description='The name of the object')
     description: Optional[str] = Field(
         None, description='The description of the object'
     )
-    version: Optional[constr(regex=r'^\d+\.\d+\.\d+(?:\-\d+)?$')] = Field(
+    version: Optional[constr(pattern=r'^\d+\.\d+\.\d+(?:\-\d+)?$')] = Field(
         None, description='The version of the object'
     )
-    deployed: Optional[datetime] = Field(
+    deployed: Optional[StandardDateTime] = Field(
         None,
         description='The date/time the object was deployed into this Kodexa instance',
     )
     public_access: Optional[bool] = Field(
         None,
         alias='publicAccess',
         description='Is the metadata object publicly accessible by other organizations',
@@ -1382,16 +1382,16 @@
 
     name: Optional[str] = None
     description: Optional[str] = None
     assistant_definition_ref: Optional[str] = Field(
         None, alias='assistantDefinitionRef'
     )
     options: Optional[Dict[str, Any]] = None
-    stores: Optional[List[str]] = Field(default_factory=list, unique_items=True)
-    schedules: Optional[List[ScheduleDefinition]] = Field(default_factory=list, unique_items=True)
+    stores: Optional[List[str]] = Field(default_factory=list)
+    schedules: Optional[List[ScheduleDefinition]] = Field(default_factory=list)
     subscription: Optional[str] = None
 
     logging_enabled: Optional[bool] = Field(None, alias='loggingEnabled')
     show_in_training: Optional[bool] = Field(None, alias='showInTraining')
 
 
 class Taxon(KodexaBaseModel):
@@ -1406,15 +1406,15 @@
         alias='generateName',
         description='Is the name generated, this allows that you can change displays without impacted existing content',
     )
     group: Optional[bool] = Field(
         None,
         description="Is this taxon a group, and therefore can't have a value, can only have children",
     )
-    name: constr(regex=r'^[a-zA-Z0-9\-_]{0,255}$') = Field(
+    name: constr(pattern=r'^[a-zA-Z0-9\-_]{0,255}$') = Field(
         ..., description='The name to be used'
     )
     external_name: Optional[str] = Field(
         None,
         alias='externalName',
         description='The name to be used when we are publishing this taxon to external systems',
     )
@@ -1528,40 +1528,40 @@
         description='Default attribute status ID',
     )
 
 
 class ContentObject(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     content_type: ContentType = Field(
         ..., alias='contentType', description='The type of content'
     )
     document_version: Optional[str] = Field(None, alias='documentVersion')
     index: Optional[int] = None
-    labels: Optional[List[Label]] = Field(default_factory=list, unique_items=True)
+    labels: Optional[List[Label]] = Field(default_factory=list)
     metadata: Optional[Dict[str, Any]] = None
-    mixins: Optional[List[str]] = Field(default_factory=list, unique_items=True)
-    created: Optional[datetime] = None
-    modified: Optional[datetime] = None
+    mixins: Optional[List[str]] = Field(default_factory=list)
+    created: Optional[StandardDateTime] = None
+    modified: Optional[StandardDateTime] = None
     size: Optional[int] = None
     store_ref: Optional[str] = Field(None, alias='storeRef')
     document_family_id: Optional[str] = Field(None, alias='documentFamilyId')
 
 
 class DocumentAssignment(KodexaBaseModel):
     """
     A list of the assignments to users for this document
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     user: User
 
 
 class ExceptionDetails(KodexaBaseModel):
     message: Optional[str] = None
     status_code: Optional[int] = Field(None, alias='statusCode')
     error_message: Optional[str] = Field(None, alias='errorMessage')
@@ -1584,46 +1584,46 @@
 class ExecutionStep(KodexaBaseModel):
     id: Optional[str] = None
     status: Optional[Status3] = None
     exception_details: Optional[ExceptionDetails] = Field(
         None, alias='exceptionDetails'
     )
     name: Optional[str] = None
-    start: Optional[datetime] = None
-    end: Optional[datetime] = None
+    start: Optional[StandardDateTime] = None
+    end: Optional[StandardDateTime] = None
     processing_time: Optional[int] = Field(None, alias='processingTime')
     options: Optional[Dict[str, Any]] = None
     option_types: Optional[Dict[str, str]] = Field(None, alias='optionTypes')
     context: Optional[Dict[str, Any]] = None
     content_objects: Optional[List[ContentObject]] = Field(
-        None, alias='contentObjects', unique_items=True
+        None, alias='contentObjects'
     )
     input_id: Optional[str] = Field(None, alias='inputId')
     output_id: Optional[str] = Field(None, alias='outputId')
     ref: Optional[str] = None
     extension_pack_ref: Optional[str] = Field(None, alias='extensionPackRef')
     step_type: Optional[StepType1] = Field(None, alias='stepType')
 
 
 class ProjectStatus(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     status: Optional[str] = Field(None, description='The status of the project')
     color: Optional[str] = None
     organization: Organization
     icon: Optional[str] = None
 
 
 class Project(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     organization: Optional[Organization] = None
     name: Optional[str] = None
     description: Optional[str] = None
     metadata: Optional[ProjectMetadata] = None
     show_tasks: Optional[bool] = Field(None, alias='showTasks')
     show_thumbnails: Optional[bool] = Field(None, alias='showThumbnails')
     show_notes_on_project: Optional[bool] = Field(None, alias='showNotesOnProject')
@@ -1633,18 +1633,18 @@
     show_tooltips_on_labeling: Optional[bool] = Field(None, alias='showTooltipsOnLabeling')
 
     has_image: Optional[bool] = Field(None, alias='hasImage')
 
     project_template_ref: Optional[str] = Field(None, alias='projectTemplateRef')
     memory: Optional[ProjectMemory] = None
     document_statuses: Optional[List[DocumentStatus]] = Field(
-        None, alias='documentStatuses', unique_items=True
+        None, alias='documentStatuses'
     )
     attribute_statuses: Optional[List[AttributeStatus]] = Field(
-        None, alias='attributeStatuses', unique_items=True
+        None, alias='attributeStatuses'
     )
     status: Optional[ProjectStatus] = None
     owner: Optional[User] = None
 
 
 class FeatureSet(KodexaBaseModel):
     node_features: Optional[List[NodeFeatures]] = Field(None, alias='nodeFeatures')
@@ -1674,16 +1674,16 @@
     data_form_states: Optional[List[DataFormState]] = Field(None, alias='dataFormStates')
     current_view_id: Optional[str] = Field(None, alias='currentViewId')
 
 
 class Workspace(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the workspace')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     project: Optional[Project] = None
     name: Optional[str] = None
     description: Optional[str] = None
     channel: Optional[Channel] = None
     workspace_storage: Optional[WorkspaceStorage] = Field(None, alias='workspaceStorage')
 
 
@@ -1692,16 +1692,16 @@
     description: Optional[str] = None
     workspace_storage: Optional[WorkspaceStorage] = Field(None, alias='workspaceStorage')
 
 
 class Channel(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the channel')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     workspace: Optional[Workspace] = None
 
 
 class MessageBlock(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the message block')
     type: Optional[str] = None
     properties: Optional[Dict[str, Any]] = None
@@ -1713,41 +1713,41 @@
     user_id: Optional[str] = Field(None, alias='userId')
     options: Optional[Dict[str, Any]] = None
 
 
 class Message(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the message')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     channel: Optional[Channel] = None
     message_blocks: Optional[MessageBlock] = Field(None, alias='messageBlock')
     message_type: Optional[str] = Field(None, alias='messageType')
     content: Optional[str] = None
     message_feedback: Optional[MessageFeedback] = Field(None, alias='messageFeedback')
     assistant: Optional[Assistant] = None
     user: Optional[User] = None
 
 
 class DataAttribute(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     value: Optional[str] = None
     truncated: Optional[bool] = None
     data_exceptions: Optional[List[DataException]] = Field(
         None,
         alias='dataExceptions',
         description='A list of the data exceptions',
-        unique_items=True,
+        
     )
     tag: str
     tag_uuid: Optional[str] = Field(None, alias='tagUuid')
-    date_value: Optional[datetime] = Field(None, alias='dateValue')
+    date_value: Optional[StandardDateTime] = Field(None, alias='dateValue')
     float_value: Optional[float] = Field(None, alias='floatValue')
     decimal_value: Optional[float] = Field(None, alias='decimalValue')
     number_value: Optional[int] = Field(None, alias='numberValue')
     boolean_value: Optional[bool] = Field(None, alias='booleanValue')
     string_value: Optional[str] = Field(None, alias='stringValue')
     attribute_status: Optional[AttributeStatus] = Field(None, alias='attributeStatus')
     confidence: Optional[float] = None
@@ -1763,39 +1763,39 @@
     data_obj_id: Optional[str] = Field(None, alias='dataObjId')
     label: Optional[str] = None
 
 
 class Note(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     user: Optional[User] = None
     content: Optional[str] = None
 
 
 class Role(KodexaBaseModel):
     """
     A role that can be used to manage rights
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     name: str
-    users: Optional[List[User]] = Field(default_factory=list, unique_items=True)
-    teams: Optional[List[Team]] = Field(default_factory=list, unique_items=True)
+    users: Optional[List[User]] = Field(default_factory=list)
+    teams: Optional[List[Team]] = Field(default_factory=list)
 
 
 class Membership(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     role: Optional[Role1] = None
     organization: Optional[Organization] = None
     user: Optional[User] = None
 
 
 class DataFormSourceMethod(KodexaBaseModel):
     name: Optional[str] = None
@@ -1993,15 +1993,15 @@
 
 
 class CustomEvent(KodexaBaseModel):
     """
     A Custom Event allows you to define an subtype of assistant event with options
     """
 
-    name: Optional[constr(regex=r'^[a-zA-Z0-9\-_]{0,40}$')] = Field(
+    name: Optional[constr(pattern=r'^[a-zA-Z0-9\-_]{0,40}$')] = Field(
         None, description='The name of the event'
     )
     icon: Optional[str] = Field(
         None, description='The name of a Material Design Icon to use for the event'
     )
     label: Optional[str] = Field(
         None, description='The label to use on the event in the UI'
@@ -2055,16 +2055,16 @@
 class ContentException(KodexaBaseModel):
     """
     A list of the content exceptions from the content objects
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     tag: Optional[str] = None
     message: str
     exception_type: str = Field(..., alias='exceptionType')
     severity: str
     exception_details: Optional[str] = Field(None, alias='exceptionDetails')
     group_uuid: Optional[str] = Field(None, alias='groupUuid')
     tag_uuid: Optional[str] = Field(None, alias='tagUuid')
@@ -2097,70 +2097,70 @@
     last: Optional[bool] = None
     empty: Optional[bool] = None
 
 
 class Execution(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     description: Optional[str] = None
     targets: Optional[ExecutionTargets] = None
     session: Optional[Session] = None
-    start_date: Optional[datetime] = Field(None, alias='startDate')
-    end_date: Optional[datetime] = Field(None, alias='endDate')
+    start_date: Optional[StandardDateTime] = Field(None, alias='startDate')
+    end_date: Optional[StandardDateTime] = Field(None, alias='endDate')
     processing_time: Optional[int] = Field(None, alias='processingTime')
     logging_enabled: Optional[bool] = Field(None, alias='loggingEnabled')
     status: Optional[Status1] = None
     exception_details: Optional[ExceptionDetails] = Field(
         None, alias='exceptionDetails'
     )
     status_details: Optional[StatusDetails] = Field(None, alias='statusDetails')
     pipeline: Optional[ExecutionPipeline] = None
     parameters: Optional[Dict[str, Any]] = None
     custom_options: Optional[Dict[str, Any]] = Field(
         None, alias='customOptions'
     )
     context: Optional[Dict[str, Any]] = None
     content_objects: Optional[List[ContentObject]] = Field(
-        None, alias='contentObjects', unique_items=True
+        None, alias='contentObjects'
     )
     child_executions: Optional[List[Execution]] = Field(
         None, alias='childExecutions'
     )
 
 
 class ExecutionSnapshot(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     description: Optional[str] = None
     targets: Optional[ExecutionTargets] = None
     session: Optional[Session] = None
-    start_date: Optional[datetime] = Field(None, alias='startDate')
-    end_date: Optional[datetime] = Field(None, alias='endDate')
+    start_date: Optional[StandardDateTime] = Field(None, alias='startDate')
+    end_date: Optional[StandardDateTime] = Field(None, alias='endDate')
     processing_time: Optional[int] = Field(None, alias='processingTime')
     logging_enabled: Optional[bool] = Field(None, alias='loggingEnabled')
     status: Optional[Status2] = None
     exception_details: Optional[ExceptionDetails] = Field(
         None, alias='exceptionDetails'
     )
     status_details: Optional[StatusDetails] = Field(None, alias='statusDetails')
     pipeline: Optional[ExecutionPipeline] = None
     parameters: Optional[Dict[str, Any]] = None
     custom_options: Optional[Dict[str, Any]] = Field(
         None, alias='customOptions'
     )
     context: Optional[Dict[str, Any]] = None
     child_executions: Optional[List[Execution]] = Field(
-        None, alias='childExecutions', unique_items=True
+        None, alias='childExecutions'
     )
     content_objects: Optional[List[ContentObject]] = Field(
-        None, alias='contentObjects', unique_items=True
+        None, alias='contentObjects'
     )
 
 
 class PageExecution(KodexaBaseModel):
     total_pages: Optional[int] = Field(None, alias='totalPages')
     total_elements: Optional[int] = Field(None, alias='totalElements')
     size: Optional[int] = None
@@ -2210,66 +2210,66 @@
 class DocumentFamily(KodexaBaseModel):
     """
     A document family is the representation of a single piece of external content (ie. a PDF) and all the related document representations of that file
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     document_status: Optional[DocumentStatus] = Field(None, alias='documentStatus')
     assignments: Optional[List[DocumentAssignment]] = Field(
         None,
         description='A list of the assignments to users for this document',
-        unique_items=True,
+        
     )
     store_ref: Optional[str] = Field(
         None,
         alias='storeRef',
         description='The reference to the store that is holding this document family',
     )
     path: str = Field(..., description='The path to the document family in the store')
     locked: Optional[bool] = Field(
         None,
         description='Is the document family locked. If locked then you can no longer modify or add any new document transitions',
     )
-    created: Optional[datetime] = Field(None, description='Date/Time Created')
-    modified: Optional[datetime] = Field(None, description='Date/Time Modified')
+    created: Optional[StandardDateTime] = Field(None, description='Date/Time Created')
+    modified: Optional[StandardDateTime] = Field(None, description='Date/Time Modified')
     size: Optional[int] = Field(
         None, description='Size of the original native content in bytes'
     )
     indexed: Optional[bool] = Field(
         None, description='Is the document family indexed for search'
     )
     content_objects: Optional[List[ContentObject]] = Field(
         None,
         alias='contentObjects',
         description='An ordered list of the content objects in the document family',
-        unique_items=True,
+        
     )
     content_exceptions: Optional[List[ContentException]] = Field(
         default_factory=list,
         alias='contentExceptions',
         description='A list of the content exceptions from the content objects',
-        unique_items=True,
+        
     )
     transitions: Optional[List[DocumentTransition]] = Field(
         None,
         description='An ordered list of the transitions in the document family',
-        unique_items=True,
+        
     )
     labels: Optional[List[Label]] = Field(
         None,
         description='The labels from the latest content object in the family',
-        unique_items=True,
+        
     )
     mixins: Optional[List[str]] = Field(
         None,
         description='The mixins from the latest content object in the family',
-        unique_items=True,
+        
     )
     metadata: Optional[Dict[str, Any]] = Field(
         None, description='The metadata from the latest document content object'
     )
     metadata_source: Optional[Dict[str, str]] = Field(
         None,
         alias='metadataSource',
@@ -2282,15 +2282,15 @@
         alias='labelStatistics',
         description='The statistics about the labels in the document family',
     )
 
     classes: Optional[List[ContentClassification]] = Field(
         None,
         description='The classification classes from the latest content object in the family',
-        unique_items=True,
+        
     )
 
 
 class DocumentFamilyStatistics(KodexaBaseModel):
     """
     A collection of statistics about the document family
     """
@@ -2300,18 +2300,18 @@
         None, alias='recentExecutions'
     )
 
 
 class ExecutionAssistant(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     subscription: Optional[str] = None
-    schedules: Optional[List[AssistantSchedule]] = Field(default_factory=list, unique_items=True)
+    schedules: Optional[List[AssistantSchedule]] = Field(default_factory=list)
     project: Optional[Project] = None
     name: str
     description: Optional[str] = None
     assistant_definition_ref: Optional[str] = Field(
         None, alias='assistantDefinitionRef'
     )
     logging_enabled: Optional[bool] = Field(None, alias='loggingEnabled')
@@ -2328,41 +2328,41 @@
     assistant: Optional[ExecutionAssistant] = None
     execution: Optional[ExecutionSnapshot] = None
 
 
 class DataObject(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     document_family: Optional[DocumentFamily] = Field(None, alias='documentFamily')
     data_exceptions: Optional[List[DataException]] = Field(
         default_factory=list,
         alias='dataExceptions',
         description='A list of the data exceptions',
-        unique_items=True,
+        
     )
     taxonomy_ref: Optional[str] = Field(None, alias='taxonomyRef')
     path: Optional[str] = None
     row_num: Optional[int] = Field(None, alias='rowNum')
     source_ordering: Optional[str] = Field(None, alias='sourceOrdering')
-    date_time: Optional[datetime] = Field(None, alias='dateTime')
+    date_time: Optional[StandardDateTime] = Field(None, alias='dateTime')
     lineage: Optional[DataLineage] = None
-    attributes: Optional[List[DataAttribute]] = Field(default_factory=list, unique_items=True)
+    attributes: Optional[List[DataAttribute]] = Field(default_factory=list)
     parent_id: Optional[str] = Field(None, alias='parentId')
     store_ref: Optional[str] = Field(None, alias='storeRef')
 
 
 class Assistant(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     subscription: Optional[str] = None
-    schedules: Optional[List[AssistantSchedule]] = Field(default_factory=list, unique_items=True)
+    schedules: Optional[List[AssistantSchedule]] = Field(default_factory=list)
     project: Optional[Project] = None
     name: str
     description: Optional[str] = None
     assistant_definition_ref: Optional[str] = Field(
         None, alias='assistantDefinitionRef'
     )
     logging_enabled: Optional[bool] = Field(None, alias='loggingEnabled')
@@ -2397,16 +2397,16 @@
             ContentEvent,
             DataObjectEvent,
             DocumentFamilyEvent,
             ScheduledEvent,
         ]
     ] = None
     response: Optional[AssistantExecutionResponse] = None
-    start_date: Optional[datetime] = Field(None, alias='startDate')
-    end_date: Optional[datetime] = Field(None, alias='endDate')
+    start_date: Optional[StandardDateTime] = Field(None, alias='startDate')
+    end_date: Optional[StandardDateTime] = Field(None, alias='endDate')
     processing_time: Optional[int] = Field(None, alias='processingTime')
 
 
 class AssistantExecutionResponse(KodexaBaseModel):
     text: Optional[str] = None
     pipelines: Optional[List[AssistantResponsePipeline]] = None
 
@@ -2417,23 +2417,23 @@
     write_back_to_store: Optional[bool] = Field(None, alias='writeBackToStore')
     data_source_ref: Optional[str] = Field(None, alias='dataSourceRef')
     taxonomy_refs: Optional[List[str]] = Field(None, alias='taxonomyRefs')
     labels_to_apply: Optional[List[str]] = Field(None, alias='labelsToApply')
     logging_enabled: Optional[bool] = Field(None, alias='loggingEnabled')
 
 
-class BaseEvent(KodexaBaseModel):
-    __root__: Union[
-        BaseEvent1,
-        DocumentFamilyEvent,
-        DataObjectEvent,
-        ContentEvent,
-        ScheduledEvent,
-        AssistantEvent,
-    ]
+class BaseEvent(RootModel[Union[
+    BaseEvent1,
+    'DocumentFamilyEvent',
+    'DataObjectEvent',
+    'ContentEvent',
+    'ScheduledEvent',
+    'AssistantEvent',
+]]):
+    pass
 
 
 class MessageEvent(KodexaBaseModel):
     message: Optional[Message] = None
 
 
 class ChannelEvent(KodexaBaseModel):
@@ -2441,16 +2441,16 @@
     channel: Optional[Channel] = None
     message_events: Optional[List[MessageEvent]] = Field(None, alias='messageEvents')
 
 
 class ExecutionEvent(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     type: Type1
     status: Optional[Status6] = None
     execution: Optional[Execution] = None
     store_ref: Optional[str] = Field(None, alias='storeRef')
     document_family_id: Optional[str] = Field(None, alias='documentFamilyId')
     data_object_id: Optional[str] = Field(None, alias='dataObjectId')
     session_id: str = Field(..., alias='sessionId')
@@ -2458,17 +2458,17 @@
     pipeline: Optional[ExecutionPipeline] = None
     assistant: Optional[AssistantExecution] = None
     source: Optional[Dict[str, Any]] = None
     payload: Optional[Dict[str, Any]] = None
     input_id: Optional[str] = Field(None, alias='inputId')
     platform_url: Optional[str] = Field(None, alias='platformUrl')
     session_call_back_url: Optional[str] = Field(None, alias='sessionCallBackUrl')
-    created: Optional[datetime] = None
-    start_date: Optional[datetime] = Field(None, alias='startDate')
-    end_date: Optional[datetime] = Field(None, alias='endDate')
+    created: Optional[StandardDateTime] = None
+    start_date: Optional[StandardDateTime] = Field(None, alias='startDate')
+    end_date: Optional[StandardDateTime] = Field(None, alias='endDate')
 
 
 class PageTaxonomy(KodexaBaseModel):
     total_pages: Optional[int] = Field(None, alias='totalPages')
     total_elements: Optional[int] = Field(None, alias='totalElements')
     size: Optional[int] = None
     content: Optional[List[Taxonomy]] = None
@@ -2509,16 +2509,16 @@
 class SearchContent(KodexaBaseModel):
     """
     A document family is the representation of a single peice of external content (ie. a PDF) and all the related document representations of that file
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     store: Optional[StoreMetadata] = None
     document_family: Optional[DocumentFamily] = Field(None, alias='documentFamily')
     container_type: Optional[str] = Field(
         None, alias='containerType', description='The container node type'
     )
     container_uuid: Optional[str] = Field(
         None, alias='containerUuid', description='The container node UUID'
@@ -2557,34 +2557,34 @@
     )
     organization: Optional[Organization] = None
     slug: str
     extension_pack_ref: Optional[str] = Field(None, alias='extensionPackRef')
     id: Optional[str] = None
     uuid: Optional[str] = None
     version: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     name: Optional[str] = None
     public_access: Optional[bool] = Field(
         None,
         alias='publicAccess',
         description='Is this component available to all organizations',
     )
     ref: Optional[str] = None
-    projects: Optional[List[Project]] = Field(default_factory=list, unique_items=True)
-    assistants: Optional[List[Assistant]] = Field(default_factory=list, unique_items=True)
+    projects: Optional[List[Project]] = Field(default_factory=list)
+    assistants: Optional[List[Assistant]] = Field(default_factory=list)
     metadata: Optional[Store] = None
 
 
 class PlatformEvent(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
-    date_time: Optional[datetime] = Field(None, alias='dateTime')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
+    date_time: Optional[StandardDateTime] = Field(None, alias='dateTime')
     assistant: Optional[Assistant] = None
     event_detail: Optional[
         Union[
             AssistantEvent,
             ContentEvent,
             DataObjectEvent,
             DocumentFamilyEvent,
@@ -2610,16 +2610,16 @@
 class AuditEvent(KodexaBaseModel):
     """
     An audit event captures a data to a data structure or document
     """
 
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
-    created_on: Optional[datetime] = Field(None, alias='createdOn')
-    updated_on: Optional[datetime] = Field(None, alias='updatedOn')
+    created_on: Optional[StandardDateTime] = Field(None, alias='createdOn')
+    updated_on: Optional[StandardDateTime] = Field(None, alias='updatedOn')
     platform_user: Optional[User] = Field(None, alias='platformUser')
     document_family: Optional[DocumentFamily] = Field(None, alias='documentFamily')
     data_object: Optional[DataObject] = Field(None, alias='dataObject')
     data_attribute: Optional[DataAttribute] = Field(None, alias='dataAttribute')
     tag: Optional[str] = None
     event_type: Optional[EventType] = Field(None, alias='eventType')
     old_value: Optional[DataAttributeValues] = Field(None, alias='oldValue')
@@ -2981,14 +2981,15 @@
     single_widget: Optional[DashboardWidget] = Field(None, alias='singleWidget')
 
 
 class DataForm(ExtensionPackProvided):
     entrypoints: Optional[List[str]] = None
     entrypoint: Optional[str] = None
     cards: Optional[List[Card]] = None
+    filters: Optional[str] = None
 
 
 class ProjectDataForm(KodexaBaseModel):
     slug: Optional[str] = None
     name: Optional[str] = None
     description: Optional[str] = None
 
@@ -2998,18 +2999,18 @@
 
 
 class ExtensionPack(ExtensionPackProvided):
     """
     Extension packs provide new components to the platform
     """
 
-    org_slug: Optional[constr(regex=r'^[a-zA-Z0-9\-_]{0,100}$')] = Field(
+    org_slug: Optional[constr(pattern=r'^[a-zA-Z0-9\-_]{0,100}$')] = Field(
         None, alias='orgSlug'
     )
-    slug: Optional[constr(regex=r'^[a-zA-Z0-9\-_]{0,100}$')] = None
+    slug: Optional[constr(pattern=r'^[a-zA-Z0-9\-_]{0,100}$')] = None
     name: Optional[str] = None
     description: Optional[str] = None
     public_access: Optional[bool] = Field(None, alias='publicAccess')
     pack_uri: Optional[str] = Field(None, alias='packUri')
     status: Optional[Status] = None
     deployable: Optional[bool] = None
     services: Optional[List[SlugBasedMetadata]] = None
@@ -3183,29 +3184,26 @@
         None, alias='schemaVersion', description='The version of the schema'
     )
     org_slug: Optional[str] = Field(
         None,
         alias='orgSlug',
         description='The slug of the organization that owns this metadata object',
     )
-    slug: Optional[constr(regex=r'^[a-zA-Z0-9\-_]{0,255}$')] = Field(
+    slug: Optional[constr(pattern=r'^[a-zA-Z0-9\-_]{0,255}$')] = Field(
         None, description='The slug used when referencing this metadata object'
     )
     type: Optional[str] = Field(None, description='The type of metadata object')
     name: Optional[str] = Field(None, description='The name of the object')
     description: Optional[str] = Field(
         None, description='The description of the object'
     )
-    version: Optional[constr(regex=r'^\d+\.\d+\.\d+(?:\-\d+)?$')] = Field(
+    version: Optional[constr(pattern=r'^\d+\.\d+\.\d+(?:\-\d+)?$')] = Field(
         None, description='The version of the object'
     )
-    deployed: Optional[datetime] = Field(
-        None,
-        description='The date/time the object was deployed into this Kodexa instance',
-    )
+
     public_access: Optional[bool] = Field(
         None,
         alias='publicAccess',
         description='Is the metadata object publicly accessible by other organizations',
     )
     image_url: Optional[str] = Field(
         None,
@@ -3258,61 +3256,61 @@
 class DocumentFamilyEvent(KodexaBaseModel):
     type: Optional[str] = None
     document_family: Optional[DocumentFamily] = Field(None, alias='documentFamily')
 
 
 class ScheduledEvent(KodexaBaseModel):
     type: Optional[str] = None
-    last_event: Optional[datetime] = Field(None, alias='lastEvent')
-    next_event: Optional[datetime] = Field(None, alias='nextEvent')
+    last_event: Optional[StandardDateTime] = Field(None, alias='lastEvent')
+    next_event: Optional[StandardDateTime] = Field(None, alias='nextEvent')
 
 
-ThrowableProblem.update_forward_refs()
-Option.update_forward_refs()
-Taxon.update_forward_refs()
-ContentMetadata1.update_forward_refs()
-SlugBasedMetadata.update_forward_refs()
-DocumentFamily.update_forward_refs()
-DocumentFamilyStatistics.update_forward_refs()
-ExecutionAssistant.update_forward_refs()
-Assistant.update_forward_refs()
-AssistantExecution.update_forward_refs()
-AssistantExecutionResponse.update_forward_refs()
-AssistantResponsePipeline.update_forward_refs()
-BaseEvent.update_forward_refs()
-PageTaxonomy.update_forward_refs()
-PageStore.update_forward_refs()
-SearchContent.update_forward_refs()
-StoreMetadata.update_forward_refs()
-PlatformEvent.update_forward_refs()
-PageRuleSet.update_forward_refs()
-PageProjectTemplate.update_forward_refs()
-PagePipeline.update_forward_refs()
-PageModelRuntime.update_forward_refs()
-PageSlugBasedMetadata.update_forward_refs()
-PageExtensionPack.update_forward_refs()
-PageDataForm.update_forward_refs()
-PageDashboard.update_forward_refs()
-PageCredentialDefinition.update_forward_refs()
-PageAssistantDefinition.update_forward_refs()
-PageAction.update_forward_refs()
-DocumentContentMetadata.update_forward_refs()
-ModelContentMetadata.update_forward_refs()
-Action.update_forward_refs()
-AssistantDefinition.update_forward_refs()
-CredentialDefinition.update_forward_refs()
-Dashboard.update_forward_refs()
-DataForm.update_forward_refs()
-ExtensionPack.update_forward_refs()
-ModelRuntime.update_forward_refs()
-Pipeline.update_forward_refs()
-ProjectTemplate.update_forward_refs()
-Store.update_forward_refs()
-Taxonomy.update_forward_refs()
-RuleSet.update_forward_refs()
-AssistantEvent.update_forward_refs()
-ContentEvent.update_forward_refs()
-DataObjectEvent.update_forward_refs()
-DocumentFamilyEvent.update_forward_refs()
-ScheduledEvent.update_forward_refs()
-DataException.update_forward_refs()
-Workspace.update_forward_refs()
+ThrowableProblem.model_rebuild()
+Option.model_rebuild()
+Taxon.model_rebuild()
+ContentMetadata1.model_rebuild()
+SlugBasedMetadata.model_rebuild()
+DocumentFamily.model_rebuild()
+DocumentFamilyStatistics.model_rebuild()
+ExecutionAssistant.model_rebuild()
+Assistant.model_rebuild()
+AssistantExecution.model_rebuild()
+AssistantExecutionResponse.model_rebuild()
+AssistantResponsePipeline.model_rebuild()
+BaseEvent.model_rebuild()
+PageTaxonomy.model_rebuild()
+PageStore.model_rebuild()
+SearchContent.model_rebuild()
+StoreMetadata.model_rebuild()
+PlatformEvent.model_rebuild()
+PageRuleSet.model_rebuild()
+PageProjectTemplate.model_rebuild()
+PagePipeline.model_rebuild()
+PageModelRuntime.model_rebuild()
+PageSlugBasedMetadata.model_rebuild()
+PageExtensionPack.model_rebuild()
+PageDataForm.model_rebuild()
+PageDashboard.model_rebuild()
+PageCredentialDefinition.model_rebuild()
+PageAssistantDefinition.model_rebuild()
+PageAction.model_rebuild()
+DocumentContentMetadata.model_rebuild()
+ModelContentMetadata.model_rebuild()
+Action.model_rebuild()
+AssistantDefinition.model_rebuild()
+CredentialDefinition.model_rebuild()
+Dashboard.model_rebuild()
+DataForm.model_rebuild()
+ExtensionPack.model_rebuild()
+ModelRuntime.model_rebuild()
+Pipeline.model_rebuild()
+ProjectTemplate.model_rebuild()
+Store.model_rebuild()
+Taxonomy.model_rebuild()
+RuleSet.model_rebuild()
+AssistantEvent.model_rebuild()
+ContentEvent.model_rebuild()
+DataObjectEvent.model_rebuild()
+DocumentFamilyEvent.model_rebuild()
+ScheduledEvent.model_rebuild()
+DataException.model_rebuild()
+Workspace.model_rebuild()
```

### Comparing `kodexa-6.2.3a5260876523/kodexa/model/persistence.py` & `kodexa-6.3.35585655579/kodexa/model/persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 from kodexa.model import Document, ContentNode, SourceMetadata
 from kodexa.model.model import ContentClassification, DocumentMetadata, ContentFeature, ContentException, ModelInsight
 
 logger = logging.getLogger()
 
 # Heavily used SQL
-EXCEPTION_INSERT = "INSERT INTO content_exceptions (tag, message, exception_details, group_uuid, tag_uuid, exception_type, severity, node_uuid) VALUES (?, ?, ?, ?, ?, ?, ?, ?)"
-EXCEPTION_SELECT = "select tag, message, exception_details, group_uuid, tag_uuid, exception_type, severity, node_uuid from content_exceptions"
+EXCEPTION_INSERT = "INSERT INTO content_exceptions (tag, message, exception_details, group_uuid, tag_uuid, exception_type, severity, node_uuid, exception_type_id) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?)"
+EXCEPTION_SELECT = "select tag, message, exception_details, group_uuid, tag_uuid, exception_type, severity, node_uuid, exception_type_id from content_exceptions"
 
 MODEL_INSIGHT_INSERT = "INSERT INTO model_insights (model_insight) VALUES (?)"
 MODEL_INSIGHT_SELECT = "select model_insight from model_insights"
 
 FEATURE_INSERT = "INSERT INTO ft (id, cn_id, f_type, binary_value, single, tag_uuid) VALUES (?,?,?,?,?,?)"
 FEATURE_DELETE = "DELETE FROM ft where cn_id=? and f_type=?"
 
@@ -222,19 +222,20 @@
                                         id           integer primary key,
                                         tag          text,
                                         message      text,
                                         exception_details text,
                                         group_uuid   text,
                                         tag_uuid     text,
                                         exception_type text,
+                                        exception_type_id text,
                                         severity     text,
                                         node_uuid    text
                                     )""")
         self.cursor.execute("CREATE TABLE model_insights (id integer primary key,model_insight text);")
-        self.document.version = "4.0.2"
+        self.document.version = "6.0.0"
 
         self.__update_metadata()
 
     def content_node_count(self):
         self.cursor.execute("select * from cn").fetchall()
 
     def get_feature_type_id(self, feature):
@@ -342,20 +343,21 @@
         if 'mixins' in metadata and metadata['mixins']:
             self.document._mixins = metadata['mixins']
         if 'classes' in metadata and metadata['classes']:
             self.document.classes = [ContentClassification.from_dict(content_class) for content_class in
                                      metadata['classes']]
         self.uuid = metadata.get('uuid')
 
+        import semver
         root_node = self.cursor.execute("select id, pid, nt, idx from cn where pid is null").fetchone()
         if root_node:
             self.document.content_node = self.__build_node(
                 root_node)
 
-        if self.document.version != '4.0.1' and self.document.version != '4.0.2':
+        if semver.compare(self.document.version, '4.0.1') < 0:
             # We need to migrate this to a 4.0.1 document
             self.cursor.execute("""CREATE TABLE ft
                                     (
                                         id           integer primary key,
                                         cn_id        integer,
                                         f_type       INTEGER,
                                         binary_value blob,
@@ -365,17 +367,16 @@
             self.cursor.execute(
                 "insert into ft select f.id, f.cn_id, f.f_type, fv.binary_value, fv.single, null from f, f_value fv where fv.id = f.fvalue_id")
             # we will create a new feature table
             self.cursor.execute("drop table f")
             self.cursor.execute("drop table f_value")
             self.cursor.execute("CREATE INDEX f_perf ON ft(cn_id);")
             self.cursor.execute("CREATE INDEX f_perf2 ON ft(tag_uuid);")
-            self.document.version = "4.0.1"
-            self.update_metadata()
 
+        # We always run this
         self.cursor.execute("""CREATE TABLE IF NOT EXISTS content_exceptions
                                     (
                                         id           integer primary key,
                                         tag          text,
                                         message      text,
                                         exception_details text,
                                         group_uuid   text,
@@ -385,15 +386,22 @@
                                         node_uuid    text
                                     )""")
         self.cursor.execute("""CREATE TABLE IF NOT EXISTS model_insights
                                     (
                                         id           integer primary key,
                                         model_insight text
                                     )""")
-        self.document.version = "4.0.2"
+
+        if semver.compare(self.document.version, "6.0.0") < 0:
+            from sqlite3 import OperationalError
+            try:
+                self.cursor.execute("ALTER TABLE content_exception ADD COLUMN exception_type_id text")
+            except OperationalError:
+                pass
+        self.document.version = "6.0.0"
         self.update_metadata()
 
     def get_content_parts(self, new_node):
         content_parts = self.cursor.execute(
             "select cn_id, pos, content, content_idx from cnp where cn_id = ? order by pos",
             [new_node.uuid]).fetchall()
 
@@ -558,23 +566,23 @@
 
         return model_insights
 
     def add_exception(self, exception: ContentException):
         # Add an exception to the exception table
         self.cursor.execute(EXCEPTION_INSERT,
                             [exception.tag, exception.message, exception.exception_details, exception.group_uuid,
-                             exception.tag_uuid, exception.exception_type, exception.severity, exception.node_uuid])
+                             exception.tag_uuid, exception.exception_type, exception.severity, exception.node_uuid, exception.exception_type_id])
 
     def get_exceptions(self) -> List[ContentException]:
         exceptions = []
         for exception in self.cursor.execute(EXCEPTION_SELECT).fetchall():
             exceptions.append(ContentException(tag=exception[0], message=exception[1], exception_details=exception[2],
                                                group_uuid=exception[3], tag_uuid=exception[4],
                                                exception_type=exception[5],
-                                               severity=exception[6], node_uuid=exception[7]))
+                                               severity=exception[6], node_uuid=exception[7], exception_type_id=exception[8]))
         return exceptions
 
     def replace_exceptions(self, exceptions: List[ContentException]):
         self.cursor.execute("delete from content_exceptions")
         for exception in exceptions:
             self.add_exception(exception)
```

### Comparing `kodexa-6.2.3a5260876523/kodexa/pipeline/pipeline.py` & `kodexa-6.3.35585655579/kodexa/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,19 +269,14 @@
 
             end = time.perf_counter()
             logger.info(f"Step completed (f{end - start:0.4f}s)")
 
             return result_document
         except:
             logger.warning("Step failed")
-            tt, value, tb = sys.exc_info()
-            document.exceptions.append({
-                "step": self.step.__name__ if callable(self.step) else type(self.step),
-                "traceback": traceback.format_exception(tt, value, tb)
-            })
             if context.stop_on_exception:
                 raise
 
             return document
 
 
 class LabelStep(object):
```

### Comparing `kodexa-6.2.3a5260876523/kodexa/platform/client.py` & `kodexa-6.3.35585655579/kodexa/platform/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 import glob
 import json
 import logging
 import os
 import time
 from pathlib import Path
-from typing import Type, Optional, List, Dict, Any
+from typing import Type, Optional, List, Dict, Any, ClassVar
 
 import requests
 from functional import seq
 from pydantic import BaseModel
-from pydantic_yaml import YamlModel
+from pydantic_yaml import to_yaml_str
 
 from kodexa.model import Taxonomy, Document
 from kodexa.model.base import BaseEntity
 from kodexa.model.objects import PageStore, PageTaxonomy, PageProject, PageOrganization, Project, Organization, \
     PlatformOverview, DocumentFamily, DocumentContentMetadata, ModelContentMetadata, ExtensionPack, Pipeline, \
     AssistantDefinition, Action, ModelRuntime, CredentialDefinition, Execution, PageAssistantDefinition, \
     PageCredentialDefinition, \
@@ -66,15 +66,15 @@
         :param organization:
         :return:
         """
         self.organization = organization
         return self
 
 
-class ClientEndpoint(YamlModel):
+class ClientEndpoint(BaseModel):
     """
     Represents a client endpoint
     """
     client: Optional["KodexaClient"] = None
 
     def set_client(self, client):
         """
@@ -96,15 +96,15 @@
             kwargs['exclude']['client']
         else:
             kwargs['exclude'] = {'client'}
 
         kwargs['exclude_unset'] = True
         kwargs['exclude_none'] = True
 
-        return YamlModel.yaml(self, **kwargs)
+        return to_yaml_str(self, **kwargs)
 
     def detach(self):
         """
         Detach the client from the endpoint
         """
         return self.copy(exclude={'client'})
 
@@ -172,20 +172,21 @@
         if sort is not None:
             params["sort"] = sort
 
         if filters is not None:
             params["filter"] = filters
 
         list_response = self.client.get(url, params=params)
-        return [self.get_instance_class().parse_obj(item).set_client(self.client) for item in list_response.json()]
+        return [self.get_instance_class().model_validate(item).set_client(self.client) for item in list_response.json()]
 
     def replace(self, components):
         url = f"/api/projects/{self.project.id}/{self.get_type()}"
         replace_response = self.client.put(url, [component.to_dict() for component in components])
-        return [self.get_instance_class().parse_obj(item).set_client(self.client) for item in replace_response.json()]
+        return [self.get_instance_class().model_validate(item).set_client(self.client) for item in
+                replace_response.json()]
 
     def find_by_name(self, name) -> Optional[Any]:
         """Find resource by name"""
         for resource in self.list():
             if resource.name == name:
                 return resource
         return None
@@ -246,15 +247,15 @@
             list_response = self.client.get(url, params=params)
 
             # If there are no more results, exit the loop
             if not list_response.json()["content"]:
                 break
 
             # Yield each endpoint in the current page
-            for endpoint in self.get_page_class(list_response.json()).parse_obj(list_response.json()).set_client(
+            for endpoint in self.get_page_class(list_response.json()).model_validate(list_response.json()).set_client(
                     self.client).to_endpoints():
                 yield endpoint
 
             # Move to the next page
             params["page"] += 1
 
     def list(self, query="*", page=1, page_size=10, sort=None, filters: List[str] = None):
@@ -268,44 +269,44 @@
             params["sort"] = sort
 
         if filters is not None:
             params["legacyFilter"] = True
             params["filter"] = filters
 
         list_response = self.client.get(url, params=params)
-        return self.get_page_class(list_response.json()).parse_obj(list_response.json()).set_client(
+        return self.get_page_class(list_response.json()).model_validate(list_response.json()).set_client(
             self.client).to_endpoints()
 
     def create(self, component):
         url = f"/api/{self.get_type()}/{self.organization.slug}/"
         get_response = self.client.post(url, component.to_dict())
-        return self.get_instance_class(get_response.json()).parse_obj(get_response.json()).set_client(self.client)
+        return self.get_instance_class(get_response.json()).model_validate(get_response.json()).set_client(self.client)
 
     def get_by_slug(self, slug, version=None):
         url = f"/api/{self.get_type()}/{self.organization.slug}/{slug}"
         if version is not None:
             url += f"/{version}"
 
         get_response = self.client.get(url)
-        return self.get_instance_class(get_response.json()).parse_obj(get_response.json())
+        return self.get_instance_class(get_response.json()).model_validate(get_response.json())
 
 
 class EntityEndpoint(BaseEntity, ClientEndpoint):
     """
     Represents an entity endpoint
     """
 
     def reload(self):
         """
         Reload the entity
         :return:
         """
         url = f"/api/{self.get_type()}/{self.id}"
         response = self.client.get(url)
-        return self.parse_obj(response.json()).set_client(self.client)
+        return self.model_validate(response.json()).set_client(self.client)
 
     def get_type(self) -> str:
         raise NotImplementedError()
 
     def create(self):
         """
         Create the entity
@@ -395,34 +396,34 @@
         if self.organization is not None:
             if 'filter' not in params:
                 params['filter'] = [f"organization.id: '{self.organization.id}'"]
             else:
                 params['filter'].append(f"organization.id={self.organization.id}")
 
         list_response = self.client.get(url, params=params)
-        return self.get_page_class().parse_obj(list_response.json()).set_client(self.client)
+        return self.get_page_class().model_validate(list_response.json()).set_client(self.client)
 
     def find_by_organization(self, organization: Organization) -> PageProject:
         """Find projects by organization"""
         url = f"/api/{self.get_type()}/"
         get_response = self.client.get(url, params={'filter': f'organization.id={organization.id}'})
-        return self.get_page_class().parse_obj(get_response.json()).set_client(self.client)
+        return self.get_page_class().model_validate(get_response.json()).set_client(self.client)
 
     def get(self, entity_id: str) -> "EntityEndpoint":
         """Get an entity by id"""
         url = f"/api/{self.get_type()}/{entity_id}"
         get_response = self.client.get(url)
-        return self.get_instance_class().parse_obj(get_response.json()).set_client(self.client)
+        return self.get_instance_class().model_validate(get_response.json()).set_client(self.client)
 
     def create(self, new_entity: EntityEndpoint) -> EntityEndpoint:
         """Create an entity"""
         url = f"/api/{self.get_type()}"
 
         create_response = self.client.post(url, body=json.loads(new_entity.json(exclude={'client'}, by_alias=True)))
-        return self.get_instance_class().parse_obj(create_response.json()).set_client(self.client)
+        return self.get_instance_class().model_validate(create_response.json()).set_client(self.client)
 
     def delete(self, self_id: str) -> None:
         """Delete an entity by id"""
         url = f"/api/{self.get_type()}/{self_id}"
         self.client.delete(url)
 
 
@@ -780,15 +781,15 @@
 class AssistantEndpoint(Assistant, ClientEndpoint):
     """Represents an assistant endpoint"""
 
     def update(self) -> "AssistantEndpoint":
         """Update the assistant"""
         url = f"/api/projects/{self.project.id}/assistants/{self.id}"
         response = self.client.put(url, body=self.to_dict())
-        return AssistantEndpoint.parse_obj(response.json()).set_client(self.client)
+        return AssistantEndpoint.model_validate(response.json()).set_client(self.client)
 
     def delete(self):
         """Delete the assistant"""
         url = f"/api/projects/{self.project.id}/assistants/{self.id}"
         self.client.delete(url)
 
     def activate(self):
@@ -812,21 +813,21 @@
         self.client.put(url, body=[store.to_dict() for store in stores])
         return self
 
     def get_stores(self) -> List["DocumentStoreEndpoint"]:
         """Get the stores of the assistant"""
         url = f"/api/projects/{self.project.id}/assistants/{self.id}/stores"
         response = self.client.get(url)
-        return [DocumentStoreEndpoint.parse_obj(store).set_client(self.client) for store in response.json()]
+        return [DocumentStoreEndpoint.model_validate(store).set_client(self.client) for store in response.json()]
 
     def executions(self) -> List["Execution"]:
         """Get the executions of the assistant"""
         url = f"/api/projects/{self.project.id}/assistants/{self.id}/executions"
         response = self.client.get(url)
-        return [Execution.parse_obj(execution) for execution in response.json()]
+        return [Execution.model_validate(execution) for execution in response.json()]
 
     def get_event_type(self, event_type: str) -> Optional["CustomEvent"]:
         """Get the event type of the assistant"""
         for event_type in self.definition.event_types:
             if event_type.name == event_type:
                 return event_type
 
@@ -849,15 +850,15 @@
         url = f"/api/projects/{self.project.id}/assistants/{self.id}/events"
         event_object = {
             "eventType": event_type,
             "options": json.dumps(options)
         }
         response = self.client.post(url, data=event_object, files={})
         process_response(response)
-        return ExecutionEndpoint.parse_obj(response.json()).set_client(self.client)
+        return ExecutionEndpoint.model_validate(response.json()).set_client(self.client)
 
 
 class ProjectAssistantsEndpoint(ProjectResourceEndpoint):
     """Represents a project assistants endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
@@ -878,15 +879,15 @@
                 return resource
         return None
 
     def create(self, assistant: Assistant) -> AssistantEndpoint:
         """Create an assistant"""
         url = f"/api/projects/{self.project.id}/assistants"
         response = self.client.post(url, body=assistant.to_dict())
-        return AssistantEndpoint.parse_obj(response.json()).set_client(self.client)
+        return AssistantEndpoint.model_validate(response.json()).set_client(self.client)
 
 
 class ProjectDocumentStoresEndpoint(ProjectResourceEndpoint):
     """Represents a project document stores endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
@@ -992,19 +993,19 @@
         response = self.client.delete(url)
         process_response(response)
 
     def list_document_families(self, page_size=10, page=1) -> PageDocumentFamilyEndpoint:
         url = f"/api/workspaces/{self.id}/documentFamilies"
         response = self.client.get(url, {"pageSize": page_size, "page": page})
         process_response(response)
-        return PageDocumentFamilyEndpoint.parse_obj(response.json()).set_client(self.client)
+        return PageDocumentFamilyEndpoint.model_validate(response.json()).set_client(self.client)
 
     def get_channel(self):
         if self.channel is not None:
-            return ChannelEndpoint.parse_obj(self.channel).set_client(self.client)
+            return ChannelEndpoint.model_validate(self.channel).set_client(self.client)
         else:
             raise ValueError("Workspace has no channel")
 
 
 class ProjectEndpoint(EntityEndpoint, Project):
     """Represents a project endpoint"""
 
@@ -1053,21 +1054,21 @@
     def assistants(self) -> ProjectAssistantsEndpoint:
         """Get the assistants endpoint of the project"""
         return ProjectAssistantsEndpoint().set_client(self.client).set_project(self)
 
     def get_tags(self) -> List[ProjectTag]:
         """Get the tags of the project"""
         response = self.client.get(f"/api/projects/{self.id}/tags")
-        return [ProjectTag.parse_obj(tag) for tag in response.json()]
+        return [ProjectTag.model_validate(tag) for tag in response.json()]
 
     def update_tags(self, tags: List[ProjectTag]) -> List[ProjectTag]:
         """Update the tags of the project"""
         response = self.client.put(f"/api/projects/{self.id}/tags",
                                    body=[tag.dict(exclude={'client'}, by_alias=True) for tag in tags])
-        return [ProjectTag.parse_obj(tag) for tag in response.json()]
+        return [ProjectTag.model_validate(tag) for tag in response.json()]
 
 
 class ChannelsEndpoint(EntitiesEndpoint):
     """Represents a channels endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
@@ -1112,21 +1113,21 @@
     def get_page_class(self, object_dict=None) -> Type[BaseModel]:
         """Get the page class of the endpoint"""
         return PageProjectEndpoint
 
     def find_by_name(self, project_name: str) -> Optional[ProjectEndpoint]:
         """Find a project by name"""
 
-        url = f"/api/{self.get_type()}/"
+        url = f"/api/{self.get_type()}"
         filters = {'filter': [f"name: '{project_name}'"]}
         if self.organization is not None:
             filters['filter'].append(f"organization.id: '{self.organization.id}'")
         get_response = self.client.get(url, params=filters)
         if len(get_response.json()['content']) > 0:
-            return ProjectEndpoint.parse_obj(get_response.json()['content'][0]).set_client(self.client)
+            return ProjectEndpoint.model_validate(get_response.json()['content'][0]).set_client(self.client)
         return None
 
     def stream_query(self, query: str = "*", sort=None):
         """
             Stream the query for the project endpoints
         :param query: the query to run
         :param sort: sorting order of the query
@@ -1159,15 +1160,15 @@
             params['sort'] = sort
 
         if self.organization is not None:
             params['filter'].append(f"organization.id: '{self.organization.id}'")
 
         get_response = self.client.get(f"/api/{self.get_type()}/", params=params)
 
-        return PageProjectEndpoint.parse_obj(get_response.json()).set_client(self.client)
+        return PageProjectEndpoint.model_validate(get_response.json()).set_client(self.client)
 
     def create(self, project: Project, template_ref: str = None) -> Project:
         """Create a project"""
         url = f"/api/{self.get_type()}"
 
         if self.organization is not None and project.organization is None:
             project.organization = self.organization.detach()
@@ -1178,15 +1179,15 @@
         if template_ref is not None:
             params = {"templateRef": template_ref}
         else:
             params = None
 
         create_response = self.client.post(url, body=json.loads(project.json(exclude={'client'}, by_alias=True)),
                                            params=params)
-        return ProjectEndpoint.parse_obj(create_response.json()).set_client(self.client)
+        return ProjectEndpoint.model_validate(create_response.json()).set_client(self.client)
 
 
 class StoresEndpoint(ComponentEndpoint, ClientEndpoint, OrganizationOwned):
     """Represents a stores endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
@@ -1225,15 +1226,15 @@
 
     def deploy_from_url(self, extension_pack_url: str,
                         deployment_options: DeploymentOptions) -> "ExtensionPackEndpoint":
         """Deploy an extension pack from a url"""
         url = f"/api/extensionPacks/{self.organization.slug}"
         create_response = self.client.post(url, body=json.loads(deployment_options.json(by_alias=True)),
                                            params={"uri": extension_pack_url})
-        return ExtensionPackEndpoint.parse_obj(create_response.json()).set_client(self.client)
+        return ExtensionPackEndpoint.model_validate(create_response.json()).set_client(self.client)
 
 
 class ProjectTemplatesEndpoint(ComponentEndpoint, ClientEndpoint, OrganizationOwned):
     """Represents a project templates endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
@@ -1506,17 +1507,18 @@
         start = time.time()
         execution = self
         while time.time() - start < timeout:
             execution = execution.reload()
             if execution.status == status:
                 if follow_child_executions:
                     all_executions = [execution]
-                    for child_execution in [ExecutionEndpoint.parse_obj(child_execution.dict()).set_client(self.client)
-                                            for child_execution in
-                                            execution.child_executions]:
+                    for child_execution in [
+                        ExecutionEndpoint.model_validate(child_execution.dict()).set_client(self.client)
+                        for child_execution in
+                        execution.child_executions]:
                         all_executions.extend(
                             child_execution.wait_for(status, fail_on_statuses, timeout, follow_child_executions))
                     return all_executions
                 else:
                     return [execution]
 
             if execution.status in fail_on_statuses:
@@ -1534,33 +1536,33 @@
         """Get the type of the endpoint"""
         return "users"
 
     def activate(self) -> "UserEndpoint":
         """Activate the user"""
         url = f"/api/users/{self.id}/activate"
         response = self.client.put(url)
-        return UserEndpoint.parse_obj(response.json()).set_client(self.client)
+        return UserEndpoint.model_validate(response.json()).set_client(self.client)
 
     def deactivate(self) -> "UserEndpoint":
         """Deactivate the user"""
         url = f"/api/users/{self.id}/activate"
         response = self.client.put(url)
-        return UserEndpoint.parse_obj(response.json()).set_client(self.client)
+        return UserEndpoint.model_validate(response.json()).set_client(self.client)
 
     def set_password(self, password: str, reset_token) -> "UserEndpoint":
         """Set the password of the user"""
         url = f"/api/users/{self.id}/password"
         response = self.client.put(url, body={"password": password, "resetToken": reset_token})
-        return UserEndpoint.parse_obj(response.json()).set_client(self.client)
+        return UserEndpoint.model_validate(response.json()).set_client(self.client)
 
     def get_memberships(self) -> List[MembershipEndpoint]:
         """Get the memberships of the user"""
         url = f"/api/users/{self.id}/memberships"
         response = self.client.get(url)
-        return [MembershipEndpoint.parse_obj(membership) for membership in response.json()]
+        return [MembershipEndpoint.model_validate(membership) for membership in response.json()]
 
 
 class ExecutionsEndpoint(EntitiesEndpoint):
     """Represents a executions endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
@@ -1616,15 +1618,15 @@
         self.data_object = data_object
 
     @property
     def notes(self) -> PageNote:
         """Get the notes of the data attribute"""
         url = f"/api/stores/{self.data_object.store_ref.replace(':', '/')}/dataObjects/{self.data_object.id}/attributes/{self.id}/notes"
         response = self.client.get(url)
-        return PageNote.parse_obj(response.json())
+        return PageNote.model_validate(response.json())
 
 
 class DataObjectEndpoint(DataObject, ClientEndpoint):
     """Represents a data object endpoint"""
 
     def update(self):
         """Update the data object"""
@@ -1637,15 +1639,15 @@
         self.client.delete(url)
 
     @property
     def attributes(self) -> List[DataAttributeEndpoint]:
         """Get the attributes of the data object"""
         url = f"/api/stores/{self.store_ref.replace(':', '/')}/dataObjects/{self.id}/attributes"
         response = self.client.get(url)
-        return [DataAttributeEndpoint.parse_obj(attribute) for attribute in response.json()]
+        return [DataAttributeEndpoint.model_validate(attribute) for attribute in response.json()]
 
 
 class DocumentFamilyEndpoint(DocumentFamily, ClientEndpoint):
     """Represents a document family endpoint"""
 
     def update(self):
         """Update the document family"""
@@ -1668,15 +1670,15 @@
     def wait_for(self, mixin: Optional[str] = None, label: Optional[str] = None,
                  timeout: int = 60) -> "DocumentFamilyEndpoint":
         """Wait for the document family to be ready"""
         logger.info("Waiting for mixin and/or label to be available on document family %s", self.id)
         start = time.time()
         while time.time() - start < timeout:
             url = f"/api/stores/{self.store_ref.replace(':', '/')}/families/{self.id}"
-            updated_document_family = DocumentFamilyEndpoint.parse_obj(self.client.get(url).json()).set_client(
+            updated_document_family = DocumentFamilyEndpoint.model_validate(self.client.get(url).json()).set_client(
                 self.client)
             if mixin and mixin in updated_document_family.mixins:
                 return updated_document_family
             if label and any(l.name == label for l in updated_document_family.labels):
                 return updated_document_family
 
             time.sleep(5)
@@ -1774,15 +1776,15 @@
         """Update the metadata of the store"""
         self.client.put(f"/api/stores/{self.ref.replace(':', '/')}/metadata",
                         body=json.loads(self.metadata.json(by_alias=True)))
 
     def get_metadata(self):
         """Get the metadata of the store"""
         metadata_response = self.client.get(f"/api/stores/{self.ref.replace(':', '/')}/metadata")
-        return self.get_metadata_class().parse_obj(metadata_response.json()) if self.get_metadata_class() else None
+        return self.get_metadata_class().model_validate(metadata_response.json()) if self.get_metadata_class() else None
 
     def post_deploy(self) -> List[str]:
         """Post deploy the store"""
         if self.metadata:
             # We need to determine in the subclass if we wil be uploading the
             # contents
             self.update_metadata()
@@ -1816,15 +1818,15 @@
 
         if filters is None:
             filters = []
 
         filters.append(f"dataObject.store.slug={self.data_store.slug}")
 
         page = super().list(query, page, page_size, sort, filters)
-        page.content = [DataExceptionEndpoint.parse_obj(data_exception.to_dict()).set_client(self.client) for
+        page.content = [DataExceptionEndpoint.model_validate(data_exception.to_dict()).set_client(self.client) for
                         data_exception in page.content]
         return page
 
 
 class DataStoreEndpoint(StoreEndpoint):
     """Represents a data store endpoint"""
 
@@ -1851,15 +1853,15 @@
         response = self.client.get(url, params=params)
         return response.text
 
     def get_taxonomies(self) -> List[Taxonomy]:
         """Get the taxonomies of the store"""
         url = f"/api/stores/{self.ref.replace(':', '/')}/taxonomies"
         taxonomy_response = self.client.get(url)
-        return [TaxonomyEndpoint.parse_obj(taxonomy_response) for taxonomy_response in taxonomy_response.json()]
+        return [TaxonomyEndpoint.model_validate(taxonomy_response) for taxonomy_response in taxonomy_response.json()]
 
     def get_data_objects_df(self, path: str, query: str = "*", document_family: Optional[DocumentFamily] = None,
                             include_id: bool = False, parent_id: Optional[str] = None):
         """
         Get the data objects as a pandas dataframe
 
         Args:
@@ -1948,15 +1950,15 @@
     def get_data_object(self, data_object_id: str):
         """Get a data object by id"""
 
         url = f"/api/stores/{self.ref.replace(':', '/')}/dataObjects/{data_object_id}"
         logger.info(f"Downloading a specific data object from {url}")
 
         data_object_response = self.client.get(url)
-        return DataObjectEndpoint.parse_obj(data_object_response.json())
+        return DataObjectEndpoint.model_validate(data_object_response.json())
 
     def get_data_objects_page_request(self, path: str, page_number: int = 1, page_size=20, query="*",
                                       document_family: Optional[DocumentFamily] = None,
                                       parent_id: Optional[str] = None) -> PageDataObject:
         """
         Get a page of data objects
 
@@ -1981,16 +1983,16 @@
         params = {"path": path, "page": page_number, "pageSize": page_size, "query": query}
 
         if document_family:
             params['documentFamilyId'] = document_family.id
             params['storeRef'] = document_family.store_ref
 
         data_objects_response = self.client.get(url, params=params)
-        data_object_page = PageDataObject.parse_obj(data_objects_response.json())
-        data_object_page.content = [DataObjectEndpoint.parse_obj(data_object) for data_object in
+        data_object_page = PageDataObject.model_validate(data_objects_response.json())
+        data_object_page.content = [DataObjectEndpoint.model_validate(data_object) for data_object in
                                     data_object_page.content]
         return data_object_page
 
     def get_stream_data_objects_request(self, path: str, query="*", document_family: Optional[DocumentFamily] = None,
                                         parent_id: Optional[str] = None):
         """
         Stream page request
@@ -2025,15 +2027,15 @@
         Returns:
 
         """
         url = f"/api/stores/{self.ref.replace(':', '/')}/dataObjects"
         logger.debug(f"Creating data objects in store {url}")
 
         create_response = requests.post(url, json=[data_object.dict(by_alias=True) for data_object in data_objects])
-        return [DataObjectEndpoint.parse_obj(data_object) for data_object in create_response.json()]
+        return [DataObjectEndpoint.model_validate(data_object) for data_object in create_response.json()]
 
 
 class DocumentStoreEndpoint(StoreEndpoint):
     """Represents a document store that can be used to store files and then their related document representations"""
 
     def delete_by_path(self, object_path: str):
         """
@@ -2058,15 +2060,15 @@
             with open(file_path, 'rb') as dfm_content:
                 files = {"familyZip": dfm_content}
                 content_object_response = self.client.post(
                     f"/api/stores/{self.ref.replace(':', '/')}/families",
                     params={'import': 'true'},
                     files=files)
                 logger.info(f"Uploaded ({content_object_response.status_code})")
-                return DocumentFamilyEndpoint.parse_obj(content_object_response.json()).set_client(self.client)
+                return DocumentFamilyEndpoint.model_validate(content_object_response.json()).set_client(self.client)
         else:
             raise Exception(f"{file_path} is not a file")
 
     def upload_file(self, file_path: str, object_path: Optional[str] = None, replace=False,
                     additional_metadata: Optional[dict] = None):
         """
         Upload a file to the store
@@ -2112,15 +2114,15 @@
 
         content_object_response = self.client.post(
             f"/api/stores/{self.ref.replace(':', '/')}/fs",
             params={"path": path},
             data=additional_metadata,
             files=files)
         logger.info(f"Uploaded {path} ({content_object_response.status_code})")
-        return DocumentFamilyEndpoint.parse_obj(content_object_response.json()).set_client(self.client)
+        return DocumentFamilyEndpoint.model_validate(content_object_response.json()).set_client(self.client)
 
     def get_bytes(self, object_path: str):
         """Get the bytes for the object at the given path, will return None if there is no object there
 
         Args:
           object_path: the object path
           object_path: str:
@@ -2176,15 +2178,15 @@
         return DocumentContentMetadata
 
     def get_family(self, document_family_id: str) -> DocumentFamilyEndpoint:
         """Get the document family with the given id"""
         logger.info(f"Getting document family id {document_family_id}")
         document_family_response = self.client.get(
             f"/api/stores/{self.ref.replace(':', '/')}/families/{document_family_id}")
-        return DocumentFamilyEndpoint.parse_obj(document_family_response.json()).set_client(self.client)
+        return DocumentFamilyEndpoint.model_validate(document_family_response.json()).set_client(self.client)
 
     def stream_query(self, query: str = "*", sort=None):
         """
             Stream the query for the document family
         :param query: the query to run
         :param sort: sorting order of the query
         :return:
@@ -2213,15 +2215,15 @@
 
         if sort is not None:
             params['sort'] = sort
 
         get_response = self.client.get(f"api/stores/{self.ref.replace(':', '/')}/families",
                                        params=params)
 
-        return PageDocumentFamilyEndpoint.parse_obj(get_response.json()).set_client(self.client)
+        return PageDocumentFamilyEndpoint.model_validate(get_response.json()).set_client(self.client)
 
     def stream_filter(self, filter_string: str = "", sort=None, limit=None):
         """
             Stream the filter for the document family
         :param query: the query to run
         :param sort: sorting order of the query
         :return:
@@ -2251,48 +2253,48 @@
 
         if sort is not None:
             params['sort'] = sort
 
         get_response = self.client.get(f"api/stores/{self.ref.replace(':', '/')}/families",
                                        params=params)
 
-        return PageDocumentFamilyEndpoint.parse_obj(get_response.json()).set_client(self.client)
+        return PageDocumentFamilyEndpoint.model_validate(get_response.json()).set_client(self.client)
 
     def upload_document(self, path: str, document: "Document") -> DocumentFamilyEndpoint:
         """Upload a document to the store at the given path"""
         logger.info(f"Putting document to path {path}")
 
         files = {"file": document.to_kddb()}
         data = {"path": path, "documentVersion": document.version, "document": True}
         document_family_response = self.client.post(
             f"/api/stores/{self.ref.replace(':', '/')}/fs",
             params={"path": path},
             files=files, data=data)
 
-        return DocumentFamilyEndpoint.parse_obj(document_family_response.json()).set_client(self.client)
+        return DocumentFamilyEndpoint.model_validate(document_family_response.json()).set_client(self.client)
 
     def exists_by_path(self, path: str) -> bool:
         """Check if the store has a document family at the given path"""
         return self.client.exists(f"/api/stores/{self.ref.replace(':', '/')}/fs", params={"path": path})
 
     def get_by_path(self, path: str) -> DocumentFamilyEndpoint:
         """Get the document family at the given path"""
         get_response = self.client.get(f"api/stores/{self.ref.replace(':', '/')}/fs",
                                        params={"path": path, "meta": True})
-        return DocumentFamilyEndpoint.parse_obj(get_response.json()).set_client(self.client)
+        return DocumentFamilyEndpoint.model_validate(get_response.json()).set_client(self.client)
 
     def delete_families(self):
         """Delete all the families in the store"""
         delete_response = self.client.delete(f"api/stores/{self.ref.replace(':', '/')}/families")
 
 
 class ModelStoreEndpoint(DocumentStoreEndpoint):
     """Represents a model store"""
-    IMPLEMENTATION_PREFIX = "model_implementation/"
-    TRAINED_MODELS_PREFIX = "trained_models/"
+    IMPLEMENTATION_PREFIX: ClassVar[str] = "model_implementation/"
+    TRAINED_MODELS_PREFIX: ClassVar[str] = "trained_models/"
 
     def get_metadata_class(self) -> Type[BaseModel]:
         """Get the metadata class for the store"""
         return ModelContentMetadata
 
     def upload_trained_model(self, training_run_id: str, base_path: Optional[str] = None):
         """Upload a trained model to the store"""
@@ -2355,32 +2357,32 @@
         url = f"/api/stores/{self.ref.replace(':', '/')}/trainings"
         new_training = ModelTraining(name=name, user_test=user_test)
 
         if training_parameters is not None:
             new_training.training_parameters = training_parameters
 
         response = self.client.post(url, body=json.loads(new_training.json(by_alias=True)))
-        return ModelTraining.parse_obj(response.json())
+        return ModelTraining.model_validate(response.json())
 
     def update_training(self, training: ModelTraining) -> ModelTraining:
         """Update a model training"""
         url = f"/api/stores/{self.ref.replace(':', '/')}/trainings/{training.id}"
         response = self.client.put(url, body=json.loads(training.json(exclude={'client'}, by_alias=True)))
-        return ModelTraining.parse_obj(response.json())
+        return ModelTraining.model_validate(response.json())
 
     def delete_training(self, training_id: str):
         """Delete a model training"""
         url = f"/api/stores/{self.ref.replace(':', '/')}/trainings/{training_id}"
         self.client.delete(url)
 
     def get_training(self, training_id: str) -> ModelTraining:
         """Get a model training"""
         url = f"/api/stores/{self.ref.replace(':', '/')}/trainings/{training_id}"
         response = self.client.get(url)
-        return ModelTraining.parse_obj(response.json())
+        return ModelTraining.model_validate(response.json())
 
     def list_trainings(self, query="*", page=1, page_size=10, sort=None,
                        filters: List[str] = None) -> PageModelTraining:
         """List all model trainings"""
         url = f"/api/stores/{self.ref.replace(':', '/')}/trainings"
         params = {"query": requests.utils.quote(query),
                   "page": page,
@@ -2389,15 +2391,15 @@
         if sort is not None:
             params["sort"] = sort
 
         if filters is not None:
             params["filter"] = filters
 
         response = self.client.get(url)
-        return PageModelTraining.parse_obj(response.json())
+        return PageModelTraining.model_validate(response.json())
 
     @staticmethod
     def build_implementation_zip(metadata: ModelContentMetadata):
         import zipfile
         num_hits = 0
 
         with zipfile.ZipFile('implementation.zip', 'w', zipfile.ZIP_DEFLATED) as zipf:
@@ -2624,69 +2626,72 @@
     def __init__(self, client: "KodexaClient"):
         self.client = client
 
     def extract_data_objects(self, taxonomy: Taxonomy, document: Document) -> List[DataObject]:
         response = self.client.post(f"/api/extractionEngine/extract",
                                     data={'taxonomyJson': taxonomy.json(exclude={'client'})},
                                     files={'document': document.to_kddb()})
-        return [DataObject.parse_obj(data_object) for data_object in response.json()]
+        return [DataObject.model_validate(data_object) for data_object in response.json()]
 
     def extract_data_objects_with_exceptions(self, taxonomy: Taxonomy, document: Document) -> Dict:
         response = self.client.post(f"/api/extractionEngine/extract", params="full",
                                     data={'taxonomyJson': taxonomy.json(exclude={'client'})},
                                     files={'document': document.to_kddb()})
         return {
-            'dataObjects': [DataObject.parse_obj(data_object) for data_object in response.json()['dataObjects']],
-            'exceptions': [ContentException.parse_obj(exception) for exception in response.json()['contentExceptions']]
+            'dataObjects': [DataObject.model_validate(data_object) for data_object in response.json()['dataObjects']],
+            'exceptions': [ContentException.model_validate(exception) for exception in
+                           response.json()['contentExceptions']]
         }
 
     def extract_to_format(self, taxonomy: Taxonomy, document: Document, format: str) -> str:
         response = self.client.post(f"/api/extractionEngine/extract",
                                     params={'format': format},
                                     data={'taxonomyJson': taxonomy.json(exclude={'client'})},
                                     files={'document': document.to_kddb()})
         return response.text
 
 
 class KodexaClient:
 
-    def __init__(self, url=None, access_token=None, profile=None):
+    def __init__(self, url=None, access_token=None, profile=None, insecure=None):
         from kodexa import KodexaPlatform
         self.base_url = url if url is not None else KodexaPlatform.get_url(profile)
         self.access_token = access_token if access_token is not None else KodexaPlatform.get_access_token(profile)
+        self.insecure = insecure if insecure is not None else KodexaPlatform.get_insecure(profile)
         self.organizations = OrganizationsEndpoint(self)
         self.projects = ProjectsEndpoint(self)
         self.workspaces = WorkspacesEndpoint(self)
         self.users = UsersEndpoint(self)
         self.memberships = MembershipsEndpoint(self)
         self.executions = ExecutionsEndpoint(self)
         self.channels = ChannelsEndpoint(self)
 
     @staticmethod
-    def login(url, email, password):
+    def login(url, email, password, insecure=False):
         from requests.auth import HTTPBasicAuth
         obj_response = requests.get(f"{url}/api/account/me/token",
                                     auth=HTTPBasicAuth(email, password),
-                                    headers={"content-type": "application/json"})
+                                    headers={"content-type": "application/json"},
+                                    verify=not insecure)
         if obj_response.status_code == 200:
-            return KodexaClient(url, obj_response.text)
+            return KodexaClient(url, obj_response.text, insecure=insecure)
 
         raise Exception(f"Check your URL and password [{obj_response.status_code}]")
 
     @property
     def me(self):
-        return UserEndpoint.parse_obj(self.get("/api/account/me").json()).set_client(self)
+        return UserEndpoint.model_validate(self.get("/api/account/me").json()).set_client(self)
 
     @property
     def extraction_engine(self):
         return ExtractionEngineEndpoint(self)
 
     @property
     def platform(self) -> PlatformOverview:
-        return PlatformOverview.parse_obj(self.get('/api').json())
+        return PlatformOverview.model_validate(self.get('/api').json())
 
     def change_password(self, old_password: str, new_password: str):
         return self.post("/api/account/passwordChange", body={"oldPassword": old_password, "newPassword": new_password})
 
     def reindex(self):
         self.post("/api/indices/_reindex")
 
@@ -2708,48 +2713,52 @@
     def get_object_by_ref(self, object_type: str, ref: str) -> BaseModel:
         return self.__build_object(ref, resolve_object_type(object_type)[1])
 
     def get_object_endpoint(self, object_type: str) -> BaseModel:
         pass
 
     def get_platform(self):
-        return PlatformOverview.parse_obj(self.get(f"{self.base_url}/api").json())
+        return PlatformOverview.model_validate(self.get(f"{self.base_url}/api").json())
 
     def exists(self, url, params=None) -> bool:
         response = requests.get(self.get_url(url), params=params, headers={"x-access-token": self.access_token,
                                                                            "content-type": "application/json"})
         if response.status_code == 200 or response.status_code == 404:
             return response.status_code == 200
         process_response(response)
 
     def get(self, url, params=None) -> requests.Response:
         response = requests.get(self.get_url(url), params=params, headers={"x-access-token": self.access_token,
-                                                                           "content-type": "application/json"})
+                                                                           "content-type": "application/json"},
+                                verify=not self.insecure)
         return process_response(response)
 
     def post(self, url, body=None, data=None, files=None, params=None) -> requests.Response:
         headers = {"x-access-token": self.access_token}
         if files is None:
             headers["content-type"] = "application/json"
 
         response = requests.post(self.get_url(url), json=body, data=data, files=files, params=params,
-                                 headers=headers)
+                                 headers=headers,
+                                 verify=not self.insecure)
         return process_response(response)
 
     def put(self, url, body=None, data=None, files=None, params=None) -> requests.Response:
         headers = {"x-access-token": self.access_token}
         if files is None:
             headers["content-type"] = "application/json"
 
         response = requests.put(self.get_url(url), json=body, data=data, files=files, params=params,
-                                headers=headers)
+                                headers=headers,
+                                verify=not self.insecure)
         return process_response(response)
 
     def delete(self, url, params=None) -> requests.Response:
-        response = requests.delete(self.get_url(url), params=params, headers={"x-access-token": self.access_token})
+        response = requests.delete(self.get_url(url), params=params, headers={"x-access-token": self.access_token},
+                                   verify=not self.insecure)
         return process_response(response)
 
     def get_url(self, url):
         if url.startswith("/"):
             return self.base_url + url
         else:
             return self.base_url + "/" + url
@@ -2808,67 +2817,67 @@
                 f.write(json.dumps(taxonomy.to_dict(), indent=4))
 
     def import_project(self, organization: OrganizationEndpoint, import_path: str):
         # The import path is the directory containing the export (or a zip file containing the export)
 
         project_metadata_file = os.path.join(import_path, "project_metadata.json")
         with open(project_metadata_file, "r") as f:
-            project = Project.parse_obj(json.load(f))
+            project = Project.model_validate(json.load(f))
             project.id = None
             project.uuid = None
             project.workflow = None
             project.organization = organization.detach()
             project.project_template_ref = None
             new_project = organization.projects.create(project, None)
 
         stores = []
         taxonomies = []
 
         import glob
 
         for assistant_file in glob.glob(os.path.join(import_path, "assistant-*.json")):
             with open(assistant_file, "r") as f:
-                assistant: AssistantEndpoint = AssistantEndpoint.parse_obj(json.load(f))
+                assistant: AssistantEndpoint = AssistantEndpoint.model_validate(json.load(f))
 
                 assistant.assistant_definition_ref = assistant.definition.ref.split(':')[0]
                 new_project.assistants.create(assistant)
 
         for document_store_file in glob.glob(os.path.join(import_path, "document-store-*.json")):
             with open(document_store_file, "r") as f:
-                document_store = DocumentStoreEndpoint.parse_obj(json.load(f)).set_client(self)
+                document_store = DocumentStoreEndpoint.model_validate(json.load(f)).set_client(self)
                 document_store.org_slug = None
                 document_store.ref = None
                 document_store = organization.stores.create(document_store)
                 stores.append(document_store)
 
                 for doc_fam in glob.glob(os.path.join(import_path, document_store_file.replace('.json', '/*.dfm'))):
                     document_store.import_family(doc_fam)
 
         for data_store_file in glob.glob(os.path.join(import_path, "data-store-*.json")):
             with open(data_store_file, "r") as f:
-                data_store = DataStoreEndpoint.parse_obj(json.load(f)).set_client(self)
+                data_store = DataStoreEndpoint.model_validate(json.load(f)).set_client(self)
                 data_store.org_slug = None
                 data_store.ref = None
                 data_store = organization.stores.create(data_store)
                 stores.append(data_store)
 
         for model_store_file in glob.glob(os.path.join(import_path, "model-store-*.json")):
             with open(model_store_file, "r") as f:
-                model_store = ModelStoreEndpoint.parse_obj(json.load(f)).set_client(self)
+                model_store = ModelStoreEndpoint.model_validate(json.load(f)).set_client(self)
                 model_store.org_slug = None
                 model_store.ref = None
                 model_store = organization.stores.create(model_store)
                 stores.append(model_store)
 
                 for doc_fam in glob.glob(os.path.join(import_path, model_store_file.replace('.json', '/*.dfm'))):
                     model_store.import_family(doc_fam)
 
         for taxonomy_file in glob.glob(os.path.join(import_path, "taxonomy-*.json")):
             with open(taxonomy_file, "r") as f:
-                taxonomy = TaxonomyEndpoint.parse_obj(json.load(f))
+                taxonomy = TaxonomyEndpoint.model_validate(json.load(f))
                 taxonomy.org_slug = None
                 taxonomy.ref = None
                 taxonomies.append(organization.taxonomies.create(taxonomy))
 
         import time
         time.sleep(4)
 
@@ -2877,35 +2886,35 @@
     def deserialize(self, component_dict: dict, component_type: Optional[str] = None) -> ComponentInstanceEndpoint:
         if "type" in component_dict or component_type is not None:
             component_type = component_type if component_type is not None else component_dict["type"]
             if component_type == 'store':
                 if "storeType" in component_dict:
                     store_type = component_dict["storeType"]
                     if store_type.lower() == "document":
-                        document_store = DocumentStoreEndpoint.parse_obj(component_dict)
+                        document_store = DocumentStoreEndpoint.model_validate(component_dict)
                         document_store.set_client(self)
 
                         # We need special handling of the metadata
                         if "metadata" in component_dict and component_dict["metadata"] is not None:
-                            document_store.metadata = DocumentContentMetadata.parse_obj(
+                            document_store.metadata = DocumentContentMetadata.model_validate(
                                 component_dict["metadata"])
 
                         return document_store
                     elif store_type.lower() == "model":
-                        model_store = ModelStoreEndpoint.parse_obj(component_dict)
+                        model_store = ModelStoreEndpoint.model_validate(component_dict)
                         model_store.set_client(self)
 
                         # We need special handling of the metadata
                         if "metadata" in component_dict and component_dict["metadata"] is not None:
-                            model_store.metadata = ModelContentMetadata.parse_obj(
+                            model_store.metadata = ModelContentMetadata.model_validate(
                                 component_dict["metadata"])
 
                         return model_store
                     if store_type.lower() == "data" or store_type.lower() == "table":
-                        return DataStoreEndpoint.parse_obj(component_dict).set_client(self)
+                        return DataStoreEndpoint.model_validate(component_dict).set_client(self)
 
                     raise Exception("Unknown store type: " + store_type)
 
                 raise Exception("A store must have a storeType")
 
             known_components = {
                 "taxonomy": TaxonomyEndpoint,
@@ -2925,22 +2934,22 @@
                 "execution": ExecutionEndpoint,
                 "assistant": AssistantDefinitionEndpoint,
                 "exception": DataExceptionEndpoint,
                 "workspace": WorkspaceEndpoint,
             }
 
             if component_type in known_components:
-                return known_components[component_type].parse_obj(component_dict).set_client(self)
+                return known_components[component_type].model_validate(component_dict).set_client(self)
             raise Exception("Unknown component type: " + component_type)
 
         raise Exception(f"Type not found in the dictionary, unable to deserialize ({component_type})")
 
     def get_project(self, project_id) -> ProjectEndpoint:
         project = self.get(f"/api/projects/{project_id}")
-        return ProjectEndpoint.parse_obj(project.json()).set_client(self)
+        return ProjectEndpoint.model_validate(project.json()).set_client(self)
 
     def get_object_type(self, object_type, organization: Optional[OrganizationEndpoint] = None) -> ClientEndpoint:
         obj_type, obj_metadata = resolve_object_type(object_type)
 
         if 'endpoint' in obj_metadata:
 
             if 'global' in obj_metadata and obj_metadata['global']:
```

### Comparing `kodexa-6.2.3a5260876523/kodexa/platform/kodexa.py` & `kodexa-6.3.35585655579/kodexa/platform/kodexa.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import logging
 import os
 import sys
 import time
 from json import JSONDecodeError
 
 import requests
-import yaml
 from addict import Dict
 from appdirs import AppDirs
 
 from kodexa.connectors import get_source
 from kodexa.connectors.connectors import get_caller_dir, FolderConnector
 from kodexa.model import Document, ExtensionPack
 from kodexa.model.objects import AssistantDefinition, Action, Taxonomy, ModelRuntime, CredentialDefinition, \
@@ -48,15 +47,16 @@
     if os.path.exists(path):
         with open(path, 'r') as outfile:
             kodexa_config = json.load(outfile)
             if profile and profile not in kodexa_config:
                 kodexa_config[profile] = {'url': None, 'access_token': None}
             return kodexa_config
     else:
-        return {'url': None, 'access_token': None} if not profile else {profile: {'url': None, 'access_token': None}}
+        return {'url': None, 'access_token': None, 'insecure': False} if not profile else {
+            profile: {'url': None, 'access_token': None, 'insecure': False}}
 
 
 def save_config(config_obj):
     """Saves the configuration dictionary for the user
 
     Args:
       config_obj: return:
@@ -70,14 +70,15 @@
             os.makedirs(os.path.dirname(path))
         except OSError as exc:  # Guard against race condition
             if exc.errno != errno.EEXIST:
                 raise
     with open(path, 'w') as outfile:
         json.dump(config_obj, outfile)
 
+
 OBJECT_TYPES = {
     "extensionPacks": {
         "name": "extension pack",
         "plural": "extension packs",
         "type": ExtensionPack
     },
     "pipelines": {
@@ -262,15 +263,16 @@
         Pull the access token details (including a list of the available organizations)
 
         Returns: Dict: details of the access token
 
         """
         response = requests.get(
             f"{KodexaPlatform.get_url()}/api/account/accessToken",
-            headers={"x-access-token": KodexaPlatform.get_access_token()})
+            headers={"x-access-token": KodexaPlatform.get_access_token()},
+            verify=not KodexaPlatform.get_insecure())
         if response.status_code == 200:
             return Dict(response.json())
 
         if response.status_code == 404:
             raise Exception("Unable to find access token")
 
         raise Exception("An error occurred connecting to the Kodexa platform")
@@ -285,51 +287,62 @@
 
         if len(ref.split('/')[1].split(":")) == 2:
             version = ref.split('/')[1].split(":")[1]
 
         return [org_slug, slug, version]
 
     @classmethod
-    def login(cls, kodexa_url, username, password, profile=None):
+    def login(cls, kodexa_url, username, password, profile=None, insecure=False):
         from requests.auth import HTTPBasicAuth
         obj_response = requests.get(f"{kodexa_url}/api/account/me/token",
                                     auth=HTTPBasicAuth(username, password),
-                                    headers={"content-type": "application/json"})
+                                    headers={"content-type": "application/json"},
+                                    verify=not insecure)
         if obj_response.status_code == 200:
             kodexa_config = get_config(profile)
             if profile and profile in kodexa_config:
                 kodexa_config[profile]['url'] = kodexa_url
                 kodexa_config[profile]['access_token'] = obj_response.text
+                kodexa_config[profile]['insecure'] = insecure
             else:
                 kodexa_config['url'] = kodexa_url
                 kodexa_config['access_token'] = obj_response.text
+                kodexa_config['insecure'] = insecure
             save_config(kodexa_config)
             print("Logged in")
         else:
             print(f"Check your URL and password [{obj_response.status_code}]")
 
     @classmethod
     def get_server_info(cls):
         """ """
         r = requests.get(f"{KodexaPlatform.get_url()}/api",
                          headers={"x-access-token": KodexaPlatform.get_access_token(),
-                                  "content-type": "application/json"})
+                                  "content-type": "application/json"},
+                         verify=not KodexaPlatform.get_insecure())
         if r.status_code == 401:
             raise Exception("Your access token was not authorized")
         if r.status_code == 200:
             return r.json()
 
         logger.warning(r.text)
         raise Exception("Unable to get server information, check your platform settings")
 
     @classmethod
     def get_tempdir(cls):
         import tempfile
         return os.getenv('KODEXA_TMP', tempfile.gettempdir())
 
+    @classmethod
+    def get_insecure(cls, profile=None):
+        kodexa_config = get_config(profile)
+        env_url = os.getenv('KODEXA_URL_INSECURE', None)
+        return env_url if env_url is not None else kodexa_config[profile]['insecure'] if profile else kodexa_config[
+            'insecure']
+
 
 class RemoteSession:
     """A Session on the Kodexa platform for leveraging pipelines and services"""
 
     def __init__(self, session_type, slug):
         self.session_type = session_type
         self.slug = slug
@@ -342,28 +355,30 @@
           ref:
 
         Returns:
 
         """
         logger.debug(f"Downloading metadata for action {ref}")
         r = requests.get(f"{KodexaPlatform.get_url()}/api/actions/{ref.replace(':', '/')}",
-                         headers={"x-access-token": KodexaPlatform.get_access_token()})
+                         headers={"x-access-token": KodexaPlatform.get_access_token()},
+                         verify=not KodexaPlatform.get_insecure())
         if r.status_code == 401:
             raise Exception("Your access token was not authorized")
         if r.status_code == 200:
             return r.json()
 
         logger.warning(r.text)
         raise Exception("Unable to get action metadata, check your reference and platform settings")
 
     def start(self):
         """ """
         logger.info(f"Creating session {self.slug} ({KodexaPlatform.get_url()})")
         r = requests.post(f"{KodexaPlatform.get_url()}/api/sessions", params={self.session_type: self.slug},
-                          headers={"x-access-token": KodexaPlatform.get_access_token()})
+                          headers={"x-access-token": KodexaPlatform.get_access_token()},
+                          verify=not KodexaPlatform.get_insecure())
 
         if r.status_code != 200:
             logger.warning("Unable to create session")
             logger.warning(r.text)
             raise Exception("Unable to create a session, check your URL and access token")
 
         self.cloud_session = Dict(json.loads(r.text))
@@ -380,15 +395,16 @@
         data = {"options": json.dumps(options), "document_metadata_json": json.dumps(document.metadata),
                 "context": json.dumps(context.context)}
 
         logger.info(f"Executing session {self.cloud_session.id}")
         r = requests.post(f"{KodexaPlatform.get_url()}/api/sessions/{self.cloud_session.id}/execute",
                           params={self.session_type: self.slug, "documentVersion": document.version},
                           data=data,
-                          headers={"x-access-token": KodexaPlatform.get_access_token()}, files=files)
+                          headers={"x-access-token": KodexaPlatform.get_access_token()}, files=files,
+                          verify=not KodexaPlatform.get_insecure())
         try:
             if r.status_code == 200:
                 execution = Dict(json.loads(r.text))
             else:
                 logger.warning("Execution creation failed [" + r.text + "], response " + str(r.status_code))
                 raise Exception("Execution creation failed [" + r.text + "], response " + str(r.status_code))
         except JSONDecodeError:
@@ -398,15 +414,16 @@
         return execution
 
     def wait_for_execution(self, execution):
         status = execution.status
         while execution.status == "PENDING" or execution.status == "RUNNING":
             r = requests.get(
                 f"{KodexaPlatform.get_url()}/api/sessions/{self.cloud_session.id}/executions/{execution.id}",
-                headers={"x-access-token": KodexaPlatform.get_access_token()})
+                headers={"x-access-token": KodexaPlatform.get_access_token()},
+                verify=not KodexaPlatform.get_insecure())
             try:
                 execution = Dict(json.loads(r.text))
             except JSONDecodeError:
                 logger.warning("Unable to handle response [" + r.text + "]")
                 raise
 
             if status != execution.status:
@@ -446,15 +463,16 @@
             the output document (or None if there isn't one)
 
         """
         if execution.outputId:
             logger.info(f"Downloading output document [{execution.outputId}]")
             doc = requests.get(
                 f"{KodexaPlatform.get_url()}/api/sessions/{self.cloud_session.id}/executions/{execution.id}/objects/{execution.outputId}",
-                headers={"x-access-token": KodexaPlatform.get_access_token()})
+                headers={"x-access-token": KodexaPlatform.get_access_token()},
+                verify=KodexaPlatform.get_insecure())
             return Document.from_kddb(doc.content)
 
         logger.info("No output document")
         return None
 
 
 class RemotePipeline:
@@ -682,25 +700,27 @@
 
     def log(self, message: str):
         response = requests.post(
             f"{KodexaPlatform.get_url()}/api/sessions/{self.event.session_id}/executions/{self.event.execution.id}/logs",
             json=[
                 {'entry': message}
             ],
-            headers={'x-access-token': KodexaPlatform.get_access_token()}, timeout=300)
+            headers={'x-access-token': KodexaPlatform.get_access_token()}, timeout=300,
+            verify=not KodexaPlatform.get_insecure())
         if response.status_code != 200:
             print(f"Logging failed {response.status_code}", flush=True)
 
     def get_content_object(self, content_object_id: str):
         logger.info(
             f"Getting content object {content_object_id} in event {self.event.id} in execution {self.event.execution.id}")
 
         co_response = requests.get(
             f"{KodexaPlatform.get_url()}/api/sessions/{self.event.session_id}/executions/{self.event.execution.id}/objects/{content_object_id}",
-            headers={'x-access-token': KodexaPlatform.get_access_token()}, timeout=300)
+            headers={'x-access-token': KodexaPlatform.get_access_token()}, timeout=300,
+            verify=not KodexaPlatform.get_insecure())
         if co_response.status_code != 200:
             logger.error(f"Response {co_response.status_code} {co_response.text}")
             raise Exception(f"Unable to find content object {content_object_id} in execution {self.event.execution.id}")
         return io.BytesIO(co_response.content)
 
     def put_content_object(self, content_object: ContentObject, content) -> ContentObject:
         files = {
@@ -710,24 +730,25 @@
             "contentObjectJson": json.dumps(content_object.dict(by_alias=True))
         }
         logger.info("Posting back content object to execution object")
         co_response = requests.post(
             f"{KodexaPlatform.get_url()}/api/sessions/{self.event.session_id}/executions/{self.event.execution.id}/objects",
             data=data,
             headers={'x-access-token': KodexaPlatform.get_access_token()},
-            files=files, timeout=300)
+            files=files, timeout=300,
+            verify=not KodexaPlatform.get_insecure())
 
         if co_response.status_code != 200:
             logger.info("Unable to post back object")
             logger.error(co_response.text)
             raise Exception("Unable to post back content object")
 
         logger.info("Object posted back")
 
-        return ContentObject.parse_obj(co_response.json())
+        return ContentObject.model_validate(co_response.json())
 
     def build_pipeline_context(self) -> PipelineContext:
         context = PipelineContext(context={}, content_provider=self, execution_id=self.event.execution.id)
 
         if self.event.store_ref and self.event.document_family_id:
             logger.info("We have storeRef and document family")
             rds: DocumentStoreEndpoint = KodexaClient().get_object_by_ref('store', self.event.store_ref)
```

### Comparing `kodexa-6.2.3a5260876523/kodexa/selectors/ast.py` & `kodexa-6.3.35585655579/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/selectors/core.py` & `kodexa-6.3.35585655579/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/selectors/lexrules.py` & `kodexa-6.3.35585655579/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/selectors/lextab.py` & `kodexa-6.3.35585655579/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/selectors/parserules.py` & `kodexa-6.3.35585655579/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/selectors/parsetab.py` & `kodexa-6.3.35585655579/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/spatial/azure_models.py` & `kodexa-6.3.35585655579/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/spatial/bbox_common.py` & `kodexa-6.3.35585655579/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/spatial/table_form_common.py` & `kodexa-6.3.35585655579/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/steps/common.py` & `kodexa-6.3.35585655579/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/testing/test_components.py` & `kodexa-6.3.35585655579/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/kodexa/testing/test_utils.py` & `kodexa-6.3.35585655579/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.3a5260876523/pyproject.toml` & `kodexa-6.3.35585655579/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.2.3a5260876523"
+version = "6.3.35585655579"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
@@ -17,33 +17,32 @@
     'Programming Language :: Python :: 3.9',
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
 addict = "2.4.0"
 requests = "^2.28.1"
-msgpack = "1.0.4"
-urllib3 = "^1.26.14"
+msgpack = "1.0.5"
+urllib3 = "^2.0.3"
 ply = ">=3.11,<4.0"
 pyyaml = "^6.0"
-deepdiff = "5.8.1"
+deepdiff = "6.3.1"
 appdirs = "^1.4.4"
-simpleeval = "0.9.12"
-jsonpickle = "2.2.0"
 python-dateutil = "^2.8.2"
-datamodel-code-generator = ">=0.13.0,<0.14.0"
+datamodel-code-generator = "^0.21.0"
 better-exceptions = ">=0.3.3,<0.4.0"
 pyfunctional = ">=1.4.3,<1.5.0"
-pydantic = "^1.10.4"
-pydantic-yaml = ">=0.8.0,<0.9.0"
+pydantic = "^2.0.2"
+pydantic-yaml = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs-material = "^9.0.3"
 pytest = "7.2.0"
 pytest-runner = "6.0.0"
 mypy = "^0.991"
 flake8 = "^6.0.0"
 pandas = "1.4.3"
+setuptools = "^65.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kodexa-6.2.3a5260876523/PKG-INFO` & `kodexa-6.3.35585655579/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.2.3a5260876523
+Version: 6.3.35585655579
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: addict (==2.4.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: better-exceptions (>=0.3.3,<0.4.0)
-Requires-Dist: datamodel-code-generator (>=0.13.0,<0.14.0)
-Requires-Dist: deepdiff (==5.8.1)
-Requires-Dist: jsonpickle (==2.2.0)
-Requires-Dist: msgpack (==1.0.4)
+Requires-Dist: datamodel-code-generator (>=0.21.0,<0.22.0)
+Requires-Dist: deepdiff (==6.3.1)
+Requires-Dist: msgpack (==1.0.5)
 Requires-Dist: ply (>=3.11,<4.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: pydantic-yaml (>=0.8.0,<0.9.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic-yaml (>=1.0.0,<2.0.0)
 Requires-Dist: pyfunctional (>=1.4.3,<1.5.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: simpleeval (==0.9.12)
-Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
+Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Kodexa
 
 [![Build and Package with Poetry](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml)
 
 ![img.png](https://docs.kodexa.com/img.png)
```

